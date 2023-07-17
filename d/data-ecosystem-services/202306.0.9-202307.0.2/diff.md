# Comparing `tmp/data_ecosystem_services-202306.0.9.tar.gz` & `tmp/data_ecosystem_services-202307.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202306.0.9.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202307.0.2.tar", max compression
```

## Comparing `data_ecosystem_services-202306.0.9.tar` & `data_ecosystem_services-202307.0.2.tar`

### file list

```diff
@@ -1,39 +1,64 @@
--rw-r--r--   0        0        0      857 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      973 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     6323 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0     6901 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1130 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     1871 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0     2319 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     1808 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0     1666 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    12151 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    17906 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     1224 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    12309 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0      971 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0      920 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0      908 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0    14614 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-06-16 11:54:11.502536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32805 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2250 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1538 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33723 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24955 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    27546 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    11357 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/license.md
--rw-r--r--   0        0        0     3495 2023-06-16 11:57:40.714613 data_ecosystem_services-202306.0.9/pyproject.toml
--rw-r--r--   0        0        0    52126 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/readme.md
--rw-r--r--   0        0        0      126 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-16 11:54:11.506536 data_ecosystem_services-202306.0.9/setup.py
--rw-r--r--   0        0        0    55057 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.9/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1264 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/column.py
+-rw-r--r--   0        0        0    23557 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0    13817 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     2037 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    12009 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/excelmetadata.py
+-rw-r--r--   0        0        0      566 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     4530 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    16651 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0     5003 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0    51147 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     7345 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/table.py
+-rw-r--r--   0        0        0     1486 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    25982 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0     1044 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4570 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     8966 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    15940 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8398 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21410 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40188 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1727 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33787 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-07-17 03:03:08.520189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25880 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3825 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    48395 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5323 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4903 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0     8956 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/directory_paths.txt
+-rw-r--r--   0        0        0      827 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7250 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0     1707 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6295 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0       44 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/output.txt
+-rw-r--r--   0        0        0      869 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    20785 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    15021 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0      832 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-17 03:03:08.524189 data_ecosystem_services-202307.0.2/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0    11357 2023-07-17 03:03:08.552189 data_ecosystem_services-202307.0.2/license.md
+-rw-r--r--   0        0        0     3915 2023-07-17 03:05:20.629430 data_ecosystem_services-202307.0.2/pyproject.toml
+-rw-r--r--   0        0        0    52292 2023-07-17 03:03:08.552189 data_ecosystem_services-202307.0.2/readme.md
+-rw-r--r--   0        0        0      130 2023-07-17 03:03:08.552189 data_ecosystem_services-202307.0.2/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-17 03:03:08.552189 data_ecosystem_services-202307.0.2/setup.py
+-rw-r--r--   0        0        0    55802 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.2/PKG-INFO
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
+"""Initialize the cdc_admin_service subpackage of data_ecosystem_services package"""
+# allow absolute import from the root folder
+# whatever its name is.
+from . import environment_tracing
+from . import environment_logging
 import sys  # don't remove required for error handling
 import os
 
-
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("cdc_admin_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("cdc_admin_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-def main() -> None:
-    """Launches the DAVT Python services
-
-    Args:
-        None
-
-    Returns:
-        None
-    """
 
-if __name__ == "__main__":
-    main()
+__all__ = ['environment_logging', 'environment_tracing']
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-"""Initialize the admin_service subpackage of data_ecosystem_services package"""
+"""Initialize the cdc_security_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
+from . import security_core
+from . import security_base64
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("cdc_security_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("cdc_security_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from . import environment_logging
-from . import environment_tracing
 
-__all__ = ['environment_logging', 'environment_tracing']
+__all__ = ['security_core', 'security_base64']
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/admin_service/environment_tracing.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,103 @@
-""" Module for python tracing for tech_environment_service with minimal dependencies. """
+""" Module for python tracing for cdc_tech_environment_service with minimal dependencies. """
 
 import os
 import sys
-from opentelemetry import trace 
+from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
-from opentelemetry.sdk.trace.export import  ConsoleSpanExporter, SimpleSpanProcessor, SpanExporter, SpanExportResult
+from opentelemetry.sdk.trace.export import ConsoleSpanExporter, SimpleSpanProcessor, SpanExporter, SpanExportResult
 from opentelemetry.sdk.trace.export import ReadableSpan
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace.status import StatusCode
 import opentelemetry.sdk.trace.export as trace_export
-from opentelemetry.sdk.trace import TracerProvider
-import json
+import time
+from data_ecosystem_services.cdc_admin_service import (
+    environment_logging as pade_env_logging
+)
 
-# Import from sibling directory ..\tech_environment_service
+# Import from sibling directory ..\cdc_tech_environment_service
 OS_NAME = os.name
 
+
 sys.path.append("..")
+
+ENV_SHARE_FALLBACK_PATH = '/usr/local/share'
+
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("environment_logging: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
     env_path = os.path.dirname(os.path.abspath(sys.executable + "\\.."))
     ENV_SHARE_PATH = env_path + "\\share"
-    sys.path.append(os.path.dirname(os.path.abspath(sys.executable + "\\..\\share")))
-    TRACE_FILENAME = ENV_SHARE_PATH + "\\.pade_python_services_tracing.txt"
+    sys.path.append(os.path.dirname(
+        os.path.abspath(sys.executable + "\\..\\share")))
+    TRACE_FILENAME = ENV_SHARE_PATH + "\\data_ecosystem_services_tracing.txt"
 else:
-    print("non windows")
+    print("environment_logging: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
     env_path = os.path.dirname(os.path.abspath(sys.executable + "/.."))
     ENV_SHARE_PATH = env_path + "/share"
-    sys.path.append(os.path.dirname(os.path.abspath(sys.executable + "/../share")))
-    TRACE_FILENAME = ENV_SHARE_PATH + "/pade_python_services_tracing.txt"
-
-print(f"ENV_SHARE_PATH:{ENV_SHARE_PATH}")
-print(f"TRACE_FILENAME:{TRACE_FILENAME}")
+    sys.path.append(os.path.dirname(
+        os.path.abspath(sys.executable + "/../share")))
+    TRACE_FILENAME = ENV_SHARE_PATH + "/data_ecosystem_services_tracing.txt"
+    ENV_SHARE_PATH = os.path.expanduser("~") + '/share'
+
+try:
+    FOLDER_EXISTS = os.path.exists(ENV_SHARE_PATH)
+    if not FOLDER_EXISTS:
+        # Create a new directory because it does not exist
+        os.makedirs(ENV_SHARE_PATH)
+except Exception as e:
+    FOLDER_EXISTS = os.path.exists(ENV_SHARE_FALLBACK_PATH)
+    if not FOLDER_EXISTS:
+        if platform.system() != 'Windows':
+            # Create a new directory because it does not exist
+            os.makedirs(ENV_SHARE_FALLBACK_PATH)
+            TRACE_FILENAME = ENV_SHARE_FALLBACK_PATH + \
+                "/data_ecosystem_services_tracing.txt"
+
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
 
-FOLDER_EXISTS = os.path.exists(ENV_SHARE_PATH)
-if not FOLDER_EXISTS:
-    # Create a new directory because it does not exist
-    os.makedirs(ENV_SHARE_PATH)
 
-
- 
-  
 class FileTraceExporter(SpanExporter):
-    
+
     def __init__(self):
         self.file_path = TRACE_FILENAME
         os.makedirs(os.path.dirname(ENV_SHARE_PATH), exist_ok=True)
- 
+
     def to_readable_dict(self, span):
-        return  {
+        return {
             "trace_id": str(span.get_span_context().trace_id),
             "span_id": str(span.get_span_context().span_id),
             "parent_id": str(span.parent.span_id) if span.parent else None,
             "name": span.name,
             "status": StatusCode(span.status.status_code).name,
             "kind": span.kind.name,
             "start_time": str(span.start_time),
             "end_time": str(span.end_time),
             "attributes": dict(span.attributes),
         }
 
-
     def export(self, spans):
         for span in spans:
             span_dict = self.to_readable_dict(span)
             # TODO export to logger or azure trace
         return SpanExportResult.SUCCESS
 
-
     @staticmethod
     def delete_old_files():
         folder_path = ENV_SHARE_PATH
         for file_name in os.listdir(folder_path):
             file_path = os.path.join(folder_path, file_name)
             if os.path.getmtime(file_path) < time.time() - 7 * 86400:
                 os.remove(file_path)
@@ -98,63 +115,75 @@
     Raises:
         Exception: If an attempt is made to create another instance
                    of this singleton class.
 
     Returns:
         TracerSingleton: An instance of the TracerSingleton class.
     """
-    
+
     _instance = None
+    log_to_console = False  # Set to False if you want console logging
 
     @staticmethod
-    def instance():
+    def instance(calling_namespace_name, calling_service_name):
         """Provides access to the singleton instance of the LoggerSingleton 
         class.
 
         This method ensures there is only one instance of the LoggerSingleton 
         class in the application.
         If an instance already exists, it returns that instance. If no 
         instance exists, it creates a new one and then returns that.
         """
         if TracerSingleton._instance is None:
-            TracerSingleton()
+            TracerSingleton(calling_namespace_name, calling_service_name)
         return TracerSingleton._instance
 
-    def __init__(self):
+    def __init__(self, calling_namespace_name, calling_service_name):
         """Initializes the singleton instance, if it doesn't exist yet.
 
         This method is responsible for ensuring that only a single instance 
         of the class is created. If an instance doesn't exist at the time of 
         invocation, it will be created. If an instance already exists, 
         the existing instance will be used.
         """
         if TracerSingleton._instance is not None:
             raise Exception("This class is a singleton!")
         else:
             TracerSingleton._instance = self
 
         # Define a Resource with your service.name attribute
-        resource = Resource.create({ResourceAttributes.SERVICE_NAME: "data_ecosystem_services"})
+        resource = Resource.create(
+            {ResourceAttributes.SERVICE_NAME: calling_service_name,
+             ResourceAttributes.SERVICE_NAMESPACE: calling_namespace_name})
 
         # Set tracer provider
         trace.set_tracer_provider(TracerProvider(resource=resource))
 
-        # This is the exporter that sends data to Application Insights
-        azure_trace_exporter  = AzureMonitorTraceExporter()
-        file_trace_exporter = FileTraceExporter()
+        # Check if the environment variable is set
+        if "APPLICATIONINSIGHTS_CONNECTION_STRING" in os.environ:
+            # This is the exporter that sends data to Application Insights
+            azure_trace_exporter = AzureMonitorTraceExporter(
+                connection_string=os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
+            )
+            # Create a BatchSpanProcessor and add the exporter to it
+            azure_span_processor = BatchSpanProcessor(azure_trace_exporter)
+            # add to the tracer provider
+            trace.get_tracer_provider().add_span_processor(azure_span_processor)
+        else:
+            print(
+                "The environment variable APPLICATIONINSIGHTS_CONNECTION_STRING is not set.")
 
-        # Create a BatchSpanProcessor and add the exporter to it
-        azure_span_processor = BatchSpanProcessor(azure_trace_exporter)
+        file_trace_exporter = FileTraceExporter()
         file_span_processor = BatchSpanProcessor(file_trace_exporter)
 
-        # add to the tracer provider
-        trace.get_tracer_provider().add_span_processor(azure_span_processor)
         trace.get_tracer_provider().add_span_processor(file_span_processor)
-        trace.get_tracer_provider().add_span_processor(SimpleSpanProcessor(ConsoleSpanExporter()))
-
+        # Add ConsoleSpanExporter if log_to_console is True
+        if TracerSingleton.log_to_console:
+            trace.get_tracer_provider().add_span_processor(
+                SimpleSpanProcessor(ConsoleSpanExporter()))
 
         # Get tracer
         self.tracer = trace.get_tracer(__name__)
 
     def get_tracer(self):
         """
         Get the logger instance.
@@ -170,9 +199,9 @@
 
         In normal operation, log messages may be buffered for
         efficiency. This method ensures that all buffered messages 
         are immediately written to their destination. It can be 
         useful in scenarios where you want to ensure that all 
         log messages have been written out, such as before ending 
         a program.
-        """  
-        trace.get_tracer_provider().force_flush()
+        """
+        trace.get_tracer_provider().force_flush()
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-"""Initialize the alation_service subpackage of data_ecosystem_services package"""
+"""Initialize the az_key_vault_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
+from ..cdc_admin_service import environment_tracing
+from ..cdc_admin_service import environment_logging
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("az_key_vault_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("az_key_vault_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from ..admin_service import environment_logging
-from ..admin_service import environment_tracing
-from ..az_storage_service import az_storage_queue
-__all__ = ["endpoint", "customfieldsendpoint", "tokenendpoint", "manifest", "tagsendpoint", "idfinderendpoint", "datasource", "schema"]
+
+__all__ = ["az_client", "azd_client"]
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/endpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+import os
+
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
 class Endpoint:
     """
     A base class for interacting with Alation. It provides a location for the base URL
     and API token. It also has some helper methods for setting up request headers.
     """
 
     def __init__(self, token, base_url):
@@ -14,14 +22,15 @@
             The Alation API Access token to interact with the API. See
             https://developer.alation.com/dev/docs/authentication-into-alation-apis#create-api-access-token
             for details.
         base_url: string
             The root URL for the Alation server to use. It should not have a slash "/" at the end of the URL.
             Example: https://edc.cdc.gov
         """
+        self.updates = []
         self.token = token
         self.base_url = base_url
 
     def base_headers(self):
         """
         Create the basic HTTP headers needed to access the Alation API. This function sets the API token
         and the Accept type to JSON.
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import requests
+import urllib.parse
 from .endpoint import Endpoint
 
-# This isn't a true endpoint as it actually points to multiple URLS
-class IdFinderEndpoint(Endpoint):
+import os
+
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
+class TagsEndpoint(Endpoint):
     """
-    A class for interacting with the Alation V2 API to find the IDs of objects by type and name.
+    A class for interacting with the Alation V2 API to add tags to objects.
 
     This is a subclass of Endpoint, so users should instantiate the class by providing an API token
     and the base URL of the Alation server to work with.
-
-    Note that this functionality may require a user with admin priviledges.
     """
 
-    METADATA_ENDPOINT = '/integration/v2'
+    TAGS_ENDPOINT = '/integration/tag'
 
-    def find(self, object_type, name):
+    def apply(self, object_type, object_id, tag):
         """
-        Finds the identifier for an object in Alation given a name and object type.
+        Apply a tag to an object in Alation
 
         Parameters
         ----------
         object_type: string
             The Alation object type: "schema", "table" or "attribute". Note that columns are called 
             attributes in Alation.
-        name: string
-            The name of the object in Alation.
-
-        Returns
-        -------
-        int or None
-            If the call finds a single object, it will return the ID for the object. If it can't
-            find anything or if it finds more than one object, it will return None.
+        object_id: int
+            The ID of the object in Alation.
+        tag: string
+            The tag to apply to the object.
         """
-        url = "{base_url}{metadata_endpoint}/{object_type}?name={name}".format(base_url = self.base_url, 
-            metadata_endpoint = self.METADATA_ENDPOINT, object_type = object_type, name = name)
-        response = requests.get(url, headers=self.base_headers(), verify=True)
+
+        request_body = {'oid': object_id, 'otype': object_type}
+
+        url = "{base_url}{tags_endpoint}/{tag}/subject/".format(base_url=self.base_url,
+                                                                tags_endpoint=self.TAGS_ENDPOINT, tag=urllib.parse.quote(tag))
+        response = requests.post(
+            url, headers=self.method_with_body_headers(), json=request_body, verify=True)
         response.raise_for_status()
-        response_json = response.json()
-        if len(response_json) == 1:
-            return response_json[0]['id']
-        else:
-            return None
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/github_service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Initialize the az_storage subpackage of data_ecosystem_services package"""
-# allow absolute import from the root folder
-# whatever its name is.
-import sys  # don't remove required for error handling
+# Import from sibling directory ..\developer_service
+from ..cdc_admin_service import environment_tracing
+from ..cdc_admin_service import environment_logging
+import sys
 import os
 
-# Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("github_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("github_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from ..admin_service import environment_logging
-from ..admin_service import environment_tracing
 
-__all__ = ["az_storage_queue"]
+__all__ = ["github_secret"]
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/az_client_service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-"""Initialize the security_service subpackage of data_ecosystem_services package"""
+"""Initialize the az_key_vault_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
+from ..cdc_admin_service import environment_tracing
+from ..cdc_admin_service import environment_logging
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("az_client_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("az_client_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from . import security_core
 
-__all__ = [ 'security_core']
+__all__ = ["azd_client", "az_client"]
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-"""Initialize the self_service subpackage of data_ecosystem_services package"""
+"""Initialize the cdc_self_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
+from . import pipeline_metadata
+from . import logging_metadata
+from . import job_metadata
+from . import environment_metadata
+from . import dataset_metadata
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("cdc_self_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("cdc_self_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from . import dataset_metadata
-from . import environment_metadata
-from . import job_metadata
-from . import logging_metadata
-from . import pipeline_metadata
 
-__all__ = ['dataset_metadata', 'environment_metadata', 'job_metadata', 'logging_metadata', 'pipeline_metadata']
+__all__ = ['dataset_metadata', 'environment_metadata',
+           'job_metadata', 'logging_metadata', 'pipeline_metadata']
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import pathlib
 
 # types
 import datetime
 __all__ = ['dataset_metadata']
 
 # DAVT
-import data_ecosystem_services.tech_environment_service.dataset_core as davt_ds_core
-import data_ecosystem_services.tech_environment_service.dataset_convert as davt_ds_convert
-import data_ecosystem_services.tech_environment_service.dataset_crud as davt_ds_crud
-import data_ecosystem_services.tech_environment_service.environment_file as davt_env_file
+import data_ecosystem_services.cdc_tech_environment_service.dataset_core as davt_ds_core
+import data_ecosystem_services.cdc_tech_environment_service.dataset_convert as davt_ds_convert
+import data_ecosystem_services.cdc_tech_environment_service.dataset_crud as davt_ds_crud
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as davt_env_file
 
 # spark
 from pyspark.sql import SparkSession, DataFrame
 from pyspark.sql.functions import (
     lit,
     concat_ws,
     to_date,
@@ -32,21 +32,28 @@
 )
 from pyspark.sql.types import StringType, StructType
 
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
+    os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files in the repo
     # import pandas as pd
 else:
     import pandas as pd
 
 
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
 class DataSetMetaData:
     """
     Class to conditionally execute load logic for bronze datasets based on
     project metadata including creating Databricks database and/or tables.
     """
 
     @classmethod
@@ -76,20 +83,21 @@
         obj_ds_convert = davt_ds_convert.DataSetConvert()
         obj_environment_file = davt_env_file.EnvironmentFile()
 
         # Environment Variables
         environment = config["environment"]
         first_row_is_header = True
         delimiter = ","
-        ingesttimestamp = datetime.datetime.now()
-        tenant_id = config["davt_azure_tenant_id"]
+        ingesttimestamp = datetime.now()
+        tenant_id = config["az_sub_tenant_id"]
         client_id = config['azure_client_id']
         client_secret = config['client_secret']
 
-        running_local = ("dbutils" in locals() or "dbutils" in globals()) is not True
+        running_local = ("dbutils" in locals()
+                         or "dbutils" in globals()) is not True
         if running_local is True:
             spark = SparkSession.builder.appName("davt_analysis").getOrCreate()
 
         yyyy_param = config["yyyy"]
         if yyyy_param is None:
             yyyy_param = ""
         mm_param = config["mm"]
@@ -127,41 +135,44 @@
         source_abbreviation = config_dataset["source_abbreviation"]
         partition_by = config_dataset["partition_by"]
         file_name = config_dataset["file_name"]
         dataset_file_path = config_dataset["dataset_file_path"]
         ingress_file_path = config_dataset["ingress_file_path"]
         source_json_path = config_dataset["source_json_path"]
         source_dataset_name = config_dataset["source_dataset_name"]
-        is_using_dataset_folder_path_override = config_dataset["is_using_dataset_folder_path_override"]
+        is_using_dataset_folder_path_override = config_dataset[
+            "is_using_dataset_folder_path_override"]
         full_dataset_name = config_dataset["full_dataset_name"]
 
         if "pii_columns" in config_dataset:
             pii_columns = config_dataset["pii_columns"]
         else:
             pii_columns = ""
 
         delimiter = ","
         file_format = file_format.strip()
         file_format = file_format.lower()
         if file_format == "delta":
             file_format = "parquet_delta"
 
-        ingesttimestamp = datetime.datetime.now()
+        ingesttimestamp = datetime.now()
 
-        ingress_file_exists = obj_environment_file.file_exists(running_local, ingress_file_path, dbutils)
+        ingress_file_exists = obj_environment_file.file_exists(
+            running_local, ingress_file_path, dbutils)
         if ingress_file_exists is False and file_format != 'delta_sql':
 
             print(f"ERROR: could not find file: {ingress_file_path}")
 
         if encoding != "UNICODE":
             encoding = "UTF-8"
         print("encoding: " + encoding)
 
         is_using_standard_column_names = config["is_using_standard_column_names"]
-        print(f"is_using_standard_column_names:{is_using_standard_column_names}")
+        print(
+            f"is_using_standard_column_names:{is_using_standard_column_names}")
         is_using_standard_column_names = is_using_standard_column_names.strip().lower()
 
         # CSV, TSV, OR USV
         if (file_format == "csv" or file_format == "tsv" or file_format == "usv"):
             if file_format == "tsv":
                 delimiter = "\t"
 
@@ -192,33 +203,36 @@
                 spark.read.format("delta")
                 .option("treatEmptyValuesAsNulls", "true")
                 .load(ingress_file_path)
             )
 
         # DELTA_SQL
         elif file_format == "delta_sql":
-            print(f"attempting to load dataframe for dataset_name:{dataset_name}")
+            print(
+                f"attempting to load dataframe for dataset_name:{dataset_name}")
             print(f"file_name:{file_name}")
 
             file_name = file_name.replace("{{environment}}", environment)
             unsorted_df = spark.sql(file_name)
 
         # XPT
         elif file_format == "xpt":
-            print(f"attempting to load dataframe for dataset_name:{dataset_name}")
+            print(
+                f"attempting to load dataframe for dataset_name:{dataset_name}")
             print(f"file_name:{file_name}")
             # unsorted_df = obj_ds_convert.convert_xpt_to_dataframe(spark, ingress_file_path, tenant_id, client_id
             # client_secret)
             schema_df, unsorted_df = obj_ds_convert.convert_sas_mount_to_dataframe_with_schema(spark,
                                                                                                source_abbreviation,
                                                                                                file_name, tenant_id,
                                                                                                client_id, client_secret)
         # SAS7BDAT
         elif file_format == "sas7bdat":
-            print(f"attempting to load dataframe for dataset_name:{dataset_name}")
+            print(
+                f"attempting to load dataframe for dataset_name:{dataset_name}")
             print(f"file_name:{file_name}")
             unsorted_df = obj_ds_convert.convert_sas_to_dataframe(spark, ingress_file_path, tenant_id, client_id,
                                                                   client_secret)
 
             # unsorted_df = (spark.read
             #                    .format("com.github.saurfang.sas.spark")
             #                    .option("forceLowercaseNames", True)
@@ -250,32 +264,36 @@
                 is_empty = False
             else:
                 is_empty = True
         else:
             is_empty = True
 
         if unsorted_df is not None and is_empty is False:
-            unsorted_df = unsorted_df.withColumn("__meta_ingress_file_path", lit(ingress_file_path))
+            unsorted_df = unsorted_df.withColumn(
+                "__meta_ingress_file_path", lit(ingress_file_path))
 
             sorted_df = cls.add_custom_columns(unsorted_df, column_ordinal_sort, bronze_sps_config_columns_df,
                                                config_dataset, config)
 
             # convert column names to lower case if requested
             if is_using_standard_column_names == "force_lowercase":
                 for col_orig in sorted_df.columns:
-                    sorted_df = sorted_df.withColumnRenamed(col_orig, col_orig.lower())
+                    sorted_df = sorted_df.withColumnRenamed(
+                        col_orig, col_orig.lower())
 
             if pii_columns != "":
-                sorted_df = obj_ds_core.encrpyt_pii_columns(pii_columns, is_using_standard_column_names, sorted_df)
+                sorted_df = obj_ds_core.encrpyt_pii_columns(
+                    pii_columns, is_using_standard_column_names, sorted_df)
 
             sorted_df.createOrReplaceTempView("dataset_sorted_df")
 
             if file_format == "parquet_delta":
                 print(f"attempting to add reference for {full_dataset_name}")
-                print(f"to existing parquet in deltalake in format: {file_format}")
+                print(
+                    f"to existing parquet in deltalake in format: {file_format}")
                 print(f" for dataset_file_path: {dataset_file_path} ")
 
             # Begin Save to Delta Lake
             print(f"---Begin Save Dataset for: {dataset_name}--")
             if ingress_file_path is not None:
                 parquet_exists = False
                 # parquet_delta external - create an externally linked table to existing parquet file - don't save
@@ -299,47 +317,57 @@
                         incremental
                     )
                 # create/update internally managed table - save to delta lake
                 else:
                     if sorted_df is not None and sorted_df.count() > 0:
                         sorted_df = obj_ds_core.add_row_id_to_dataframe(sorted_df, row_id_keys, yyyy_param, mm_param,
                                                                         dd_param)
-                        print(f"attempting to update deltalake for {full_dataset_name}")
-                        print(f"with merged data in format: {file_format} for ")
+                        print(
+                            f"attempting to update deltalake for {full_dataset_name}")
+                        print(
+                            f"with merged data in format: {file_format} for ")
                         print(f"ingress_file_path: {ingress_file_path}")
-                        sorted_df = sorted_df.withColumn("meta_dd", sorted_df["meta_dd"].cast(StringType()))
-                        sorted_df = sorted_df.withColumn("meta_ingesttimestamp", lit(ingesttimestamp))
+                        sorted_df = sorted_df.withColumn(
+                            "meta_dd", sorted_df["meta_dd"].cast(StringType()))
+                        sorted_df = sorted_df.withColumn(
+                            "meta_ingesttimestamp", lit(ingesttimestamp))
                         sorted_df.createOrReplaceTempView("dataset_sorted_df")
 
                         # incremental update - add/update existing table based on row_id
                         if incremental == "incremental":
-                            print(f"incremental:{incremental} display sorted_df for: {dataset_name}")
-                            print(f"Load from: {ingress_file_path} for: {dataset_file_path} with ")
+                            print(
+                                f"incremental:{incremental} display sorted_df for: {dataset_name}")
+                            print(
+                                f"Load from: {ingress_file_path} for: {dataset_file_path} with ")
                             print(f"count: {str(sorted_df.count())}")
                             if row_id_keys is None:
                                 row_id_keys = ""
                             row_id_keys = row_id_keys.strip()
                             row_id_keys_list = row_id_keys.split(",")
                             if len(row_id_keys_list) > 0 and len(row_id_keys) > 0:
                                 sql_expr = row_id_keys
-                                sql_expr = sql_expr.replace("{yyyy}", yyyy_param)
+                                sql_expr = sql_expr.replace(
+                                    "{yyyy}", yyyy_param)
                                 sql_expr = sql_expr.replace("{mm}", mm_param)
                                 sql_expr = sql_expr.replace("{dd}", dd_param)
                             else:
                                 sql_expr = "uuid()"
 
                             sql_expr = "concat_ws('-'," + sql_expr + ")"
                         else:
                             sql_expr = "uuid()"
                             sql_expr = "concat_ws('-'," + sql_expr + ")"
 
                         print(f"row_id formula: sql_expr: {sql_expr}")
-                        sorted_df = sorted_df.withColumn("row_id", expr(sql_expr))
-                        print(f"attempting to update deltalake for {full_dataset_name} ")
-                        print(f"with merged data in format: {file_format} for ")
+                        sorted_df = sorted_df.withColumn(
+                            "row_id", expr(sql_expr))
+                        print(
+                            f"attempting to update deltalake for {full_dataset_name} ")
+                        print(
+                            f"with merged data in format: {file_format} for ")
                         print(f"ingress_file_path: {ingress_file_path}")
 
                         print(f"refresh sorted_df.count: {sorted_df.count()}")
                         obj_ds_crud.upsert(
                             spark,
                             config,
                             dbutils,
@@ -354,19 +382,22 @@
                             None,
                             incremental
                         )
                         print("updated deltalake with merged data")
                         print(f"in format: {file_format}")
                         print(f"for: {ingress_file_path}")
                     else:
-                        print(f"Error: sorted_df is None for dataset_name:{dataset_name}: for ")
-                        print(f"ingress_file_path: {ingress_file_path}: for dataset_file_path: {dataset_file_path}")
+                        print(
+                            f"Error: sorted_df is None for dataset_name:{dataset_name}: for ")
+                        print(
+                            f"ingress_file_path: {ingress_file_path}: for dataset_file_path: {dataset_file_path}")
 
                     # save metadata to delta lake with detailed quality and performance metrics
-                    print(f"---Begin Save Dataset Meta-Data for: {dataset_name}--")
+                    print(
+                        f"---Begin Save Dataset Meta-Data for: {dataset_name}--")
 
                     obj_ds_crud = davt_ds_crud.DataSetCrud()
                     if sorted_df is None:
                         print("Error: sorted_df is None")
                     else:
                         schema_df = None
                         config_schema = obj_ds_crud.get_export_dataset_or_view_schema_config(config, config_dataset,
@@ -464,15 +495,15 @@
 
         obj_ds_core = davt_ds_core.DataSetCore()
 
         project_id = config["project_id"]
         yyyy_param = config["yyyy"]
         mm_param = config["mm"]
         dd_param = config["dd"]
-        ingesttimestamp = datetime.datetime.now()
+        ingesttimestamp = datetime.now()
         dataset_name = config_dataset["dataset_name"]
         source_abbreviation = config_dataset["source_abbreviation"]
         filter_clause = config_dataset["filter_clause"]
         transmission_period = config_dataset["transmission_period"]
 
         if column_ordinal_sort.strip().lower() == 'alpha':
             sorted_df = unsorted_df.select(sorted(unsorted_df.columns))
@@ -482,34 +513,41 @@
         column_count = 0
         custom_function = ""
 
         if bronze_sps_config_columns_df is not None:
             column_count = bronze_sps_config_columns_df.count()
 
             if column_count == 0:
-                print(f"no column configurations found for dataset: {dataset_name}")
+                print(
+                    f"no column configurations found for dataset: {dataset_name}")
             else:
 
-                dataset_name_full = dataset_name.replace("{source_abbreviation}", source_abbreviation)
+                dataset_name_full = dataset_name.replace(
+                    "{source_abbreviation}", source_abbreviation)
                 filter_clause = f"project_id = '{project_id}' and dataset_name = '{dataset_name_full}'"
                 print(f"filter_clause:{filter_clause}")
-                df_config_columns_filtered = bronze_sps_config_columns_df.filter(filter_clause)
-                print(f"evaluating columns in dataset:{dataset_name} for project: {project_id}")
-                df_config_columns_filtered = df_config_columns_filtered.sort("column_batch_group")
+                df_config_columns_filtered = bronze_sps_config_columns_df.filter(
+                    filter_clause)
+                print(
+                    f"evaluating columns in dataset:{dataset_name} for project: {project_id}")
+                df_config_columns_filtered = df_config_columns_filtered.sort(
+                    "column_batch_group")
 
                 data_collect = df_config_columns_filtered.collect()
                 i_row = 1
                 for row in data_collect:
                     custom_function = row["custom_function"]
                     column_count = column_count + 1
                     column_name = row["column_name"]
                     column_name_new = row["column_name_new"]
                     column_name = obj_ds_core.scrub_object_name(column_name)
-                    column_name_new = obj_ds_core.scrub_object_name(column_name_new)
-                    print(f"evaluating column:{str(column_count)} column_name:{column_name}")
+                    column_name_new = obj_ds_core.scrub_object_name(
+                        column_name_new)
+                    print(
+                        f"evaluating column:{str(column_count)} column_name:{column_name}")
 
                     date_format = row["date_format"]
                     function = row["function"]
                     if function is None:
                         function = "missing"
 
                     function = function.strip()
@@ -522,37 +560,45 @@
                         custom_function = custom_function.strip()
                         custom_function = custom_function.replace("\n", "")
                         if custom_function is None:
                             arg_list = [""]
                         else:
                             arg_list = [custom_function]
 
-                        print(f"adding column: {column_name} concat_ws with arg_list: {str(arg_list)}")
-                        sorted_df = sorted_df.withColumn(column_name, concat_ws("-", *arg_list))
+                        print(
+                            f"adding column: {column_name} concat_ws with arg_list: {str(arg_list)}")
+                        sorted_df = sorted_df.withColumn(
+                            column_name, concat_ws("-", *arg_list))
 
                     if function == "custom":
                         custom_function = str(row["custom_function"])
                         custom_function = custom_function.strip()
 
                         if custom_function is None:
                             custom_function = ""
 
                         print(f"custom_function: {custom_function}")
-                        print(f"adding column: {column_name} custom_function: {str(custom_function)}")
-                        sorted_df = sorted_df.withColumn(column_name, expr(custom_function))
+                        print(
+                            f"adding column: {column_name} custom_function: {str(custom_function)}")
+                        sorted_df = sorted_df.withColumn(
+                            column_name, expr(custom_function))
 
                     if function == "to_date":
                         msg_add = f"adding column: {column_name} , {date_format} , { function} "
                         print(msg_add)
-                        sorted_df = sorted_df.withColumn(column_name, to_date(column_name, date_format))
+                        sorted_df = sorted_df.withColumn(
+                            column_name, to_date(column_name, date_format))
 
                     if function == "withcolumnrenamed":
-                        print(f"rename column: {column_name} to column_name_new {column_name_new}")
-                        sorted_df = sorted_df.withColumnRenamed(column_name, column_name_new)
-                        column_metadata = sorted_df.select("*").schema[column_name_new].metadata
+                        print(
+                            f"rename column: {column_name} to column_name_new {column_name_new}")
+                        sorted_df = sorted_df.withColumnRenamed(
+                            column_name, column_name_new)
+                        column_metadata = sorted_df.select(
+                            "*").schema[column_name_new].metadata
                         print("column_metadata:", column_metadata)
                         sorted_df = sorted_df.withMetadata(column_name_new, {"ingress_column_name": column_name,
                                                                              'comment': column_name})
                     i_row = i_row + 1
 
         if "year" in sorted_df.columns:
             sorted_df = sorted_df.withColumn(
@@ -576,24 +622,26 @@
                 "meta_yyyy", sorted_df["meta_yyyy"].cast(StringType())
             )
 
         if "meta_mm" not in sorted_df.columns:
             sorted_df = sorted_df.withColumn("meta_mm", lit(mm_param))
         else:
             sorted_df = sorted_df.withColumn(
-                "meta_mm", lpad(sorted_df["meta_mm"].cast(StringType()), 2, "0")
+                "meta_mm", lpad(
+                    sorted_df["meta_mm"].cast(StringType()), 2, "0")
             )
 
         if "meta_dd" not in sorted_df.columns:
             sorted_df = sorted_df.withColumn("meta_dd", lit(dd_param))
         else:
             sorted_df = sorted_df.withColumn(
                 "meta_dd", sorted_df["meta_dd"].cast(StringType())
             )
-        sorted_df = sorted_df.withColumn("meta_ingesttimestamp", lit(ingesttimestamp))
+        sorted_df = sorted_df.withColumn(
+            "meta_ingesttimestamp", lit(ingesttimestamp))
 
         return sorted_df
 
     @staticmethod
     def only_numerics(seq):
         """Take a sequence and return only the numeric items.
 
@@ -668,15 +716,16 @@
                 .strip()
                 .replace("{source_abbreviation}", source_abbreviation)
             )
 
         dataset_name = obj_ds_core.scrub_object_name(dataset_name)
         config_dataset["dataset_name"] = dataset_name
 
-        print(f"---------------Starting Load of {dataset_name} -----------------")
+        print(
+            f"---------------Starting Load of {dataset_name} -----------------")
         row_id_keys = row["row_id_keys"]
         if row_id_keys is None:
             row_id_keys = ""
         else:
             row_id_keys = row_id_keys.replace('"', "'")
         config_dataset["row_id_keys"] = row_id_keys
 
@@ -701,17 +750,17 @@
             else:
                 encoding = "UTF-8"
                 print("Error encoding:{str(encoding)} is not a string")
 
         config_dataset["encoding"] = encoding
 
         database_name = config["davt_database_name"]
-        
+
         full_dataset_name = (
-           database_name + "." + dataset_name
+            database_name + "." + dataset_name
         )
         config_dataset["full_dataset_name"] = full_dataset_name
 
         frequency = row["frequency"]
         if frequency is None:
             frequency = "daily"
         else:
@@ -764,15 +813,16 @@
             sheet_name = ""
         config_dataset["sheet_name"] = sheet_name
 
         column_header_skip_rows = row["column_header_skip_rows"]
         if column_header_skip_rows is None:
             column_header_skip_rows = 0
         else:
-            column_header_skip_rows = int(cls.only_numerics(column_header_skip_rows))
+            column_header_skip_rows = int(
+                cls.only_numerics(column_header_skip_rows))
         config_dataset["column_header_skip_rows"] = column_header_skip_rows
 
         folder_name_source = row["folder_name_source"]
         if folder_name_source is None:
             folder_name_source = "default_rule"
         if folder_name_source.strip() == "":
             folder_name_source = ""
@@ -872,15 +922,16 @@
             )
             folder_file_ingress_path_override = (
                 folder_file_ingress_path_override.replace(
                     "{project_id_root}", project_id_root
                 )
             )
             folder_file_ingress_path_override = (
-                folder_file_ingress_path_override.replace("{project_id}", project_id)
+                folder_file_ingress_path_override.replace(
+                    "{project_id}", project_id)
             )
             folder_file_ingress_path_override = (
                 folder_file_ingress_path_override.replace(
                     "{ingress_folder}", ingress_folder
                 )
             )
             folder_file_ingress_path_override = (
@@ -888,15 +939,16 @@
             )
             folder_file_ingress_path_override = (
                 folder_file_ingress_path_override.replace(
                     "{source_abbreviation}", source_abbreviation
                 )
             )
             folder_file_ingress_path_override = (
-                folder_file_ingress_path_override.replace("{environment}", environment)
+                folder_file_ingress_path_override.replace(
+                    "{environment}", environment)
             )
             folder_file_ingress_path_override = (
                 folder_file_ingress_path_override.replace(
                     "{delta_folder}", delta_folder
                 )
             )
             folder_file_ingress_path_override = (
@@ -905,32 +957,36 @@
                 )
             )
 
         # Pull from external place - reference parquet
         if folder_file_ingress_path_override is None:
             folder_file_ingress_path_override = ""
 
-        print(f"folder_file_ingress_path_override:{folder_file_ingress_path_override}")
+        print(
+            f"folder_file_ingress_path_override:{folder_file_ingress_path_override}")
         print(f"ingress_file_name:{ingress_file_name}")
 
         if (file_format == "parquet_delta" and folder_file_ingress_path_override != ""):
-            ingress_file_path = folder_file_ingress_path_override.rstrip("/") + "/" + ingress_file_name
+            ingress_file_path = folder_file_ingress_path_override.rstrip(
+                "/") + "/" + ingress_file_name
             dataset_file_path = ingress_file_path
         elif (file_format == "sas7bdat" and folder_file_ingress_path_override != ""):
             dataset_file_path = davt_database_folder + "/" + dataset_name
             dataset_file_path = dataset_file_path.replace("dbfs:", "")
-            ingress_file_path = folder_file_ingress_path_override.rstrip("/") + "/" + ingress_file_name
+            ingress_file_path = folder_file_ingress_path_override.rstrip(
+                "/") + "/" + ingress_file_name
         else:
             # Build folder name
             dataset_file_path = davt_database_folder + "/" + dataset_name
             dataset_file_path = dataset_file_path.replace("dbfs:", "")
             if is_using_dataset_folder_path_override is True:
                 ingress_file_path = folder_file_ingress_path_override + ingress_file_name
             else:
-                ingress_file_path = ingress_folder.rstrip("/") + "/" + source_abbreviation
+                ingress_file_path = ingress_folder.rstrip(
+                    "/") + "/" + source_abbreviation
                 ingress_file_path = ingress_file_path + "/" + ingress_file_name
 
         config_dataset["dataset_file_path"] = dataset_file_path
 
         ingress_file_path = ingress_file_path.strip()
 
         config_dataset["ingress_file_path"] = ingress_file_path
@@ -964,9 +1020,10 @@
         dest_path = str(dest_file_path.parent)
         dest_path = dest_path.replace("abfss:/", "abfss://")
         print(f"dest_path:{dest_path}")
         dest_path = obj_environment_file.convert_abfss_to_https_path(dest_path)
         print(f"dest_path_converted:{dest_path}")
         src_url = config_dataset["source_dataset_name"]
         print(f"src_url:{src_url}")
-        result = obj_environment_file.copy_url_to_blob(config, src_url, dest_path, ingress_file_name)
+        result = obj_environment_file.copy_url_to_blob(
+            config, src_url, dest_path, ingress_file_name)
         return result
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 import os
 from pathlib import Path
 
 # text
 import json
 from html.parser import HTMLParser  # web scraping html
 
-import logging
 import logging.config
 
 # data
+import logging
 import uuid
 from datetime import datetime
 
-# davt
-from data_ecosystem_services.security_service \
-    import security_core as davt_sec_core
-from data_ecosystem_services.tech_environment_service \
-    import environment_file as davt_env_file
-from data_ecosystem_services.self_service \
-    import logging_metadata as davt_log_metadata
+# pade
+from data_ecosystem_services.cdc_security_service \
+    import security_core as pade_sec_core
+from data_ecosystem_services.cdc_tech_environment_service \
+    import environment_file as pade_env_file
+from data_ecosystem_services.cdc_self_service \
+    import logging_metadata as pade_log_metadata
 
 from dotenv import load_dotenv, find_dotenv, set_key
 
 # spark
 from pyspark.sql import (SparkSession, DataFrame)
 from pyspark.sql.functions import (col, concat_ws, lit,
                                    udf, trim)
@@ -40,23 +40,28 @@
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 
 uuid_udf = udf(lambda: str(uuid.uuid4()), StringType())
 
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
 
 class EnvironmentMetaData:
     """This is a conceptual class representation of an Environment
     It is a static class libary
     Todo
     Note which variables require manual updates from the centers and which
     can be prepopulated
     Note which variables are EDAV or Peraton specific
-    Separate out config.devops.dev, config.davt.dev and config.core.dev
+    Separate out config.devops.dev, config.pade.dev and config.core.dev
     """
 
     @classmethod
     def check_configuration_files(cls, config: dict, dbutils: object) -> dict:
         """Takes in config dictionary and dbutils objects, returns populated
             check_files dictionary with check results
 
@@ -79,37 +84,37 @@
         # confirm config_folder
         config_folder = config["config_folder"]
         config_folder_files_exists = str(cls.file_exists(
                                          running_local, config_folder,
                                          dbutils))
 
         # confirm database path
-        davt_database_folder = config["davt_database_folder"]
+        pade_database_folder = config.get("pade_database_folder")
         files_exists = cls.file_exists(running_local,
-                                       davt_database_folder, dbutils)
-        davt_database_folder_files_exists = str(files_exists)
+                                       pade_database_folder, dbutils)
+        pade_database_folder_files_exists = str(files_exists)
 
         s_text = f"ingress_folder_files_exists exists test result:\
             {ingress_folder_files_exists}"
-        s_text_1 = f"davt_database_folder_files_exists exists test result:\
-            {davt_database_folder_files_exists}"
-        s_text_2 = f"{config['davt_database_name']} at davt_database_folder:\
-            {davt_database_folder}"
+        s_text_1 = f"pade_database_folder_files_exists exists test result:\
+            {pade_database_folder_files_exists}"
+        s_text_2 = f"{config.get('pade_database_name')} at pade_database_folder:\
+            {pade_database_folder}"
         ingress_folder_files_exists_test = s_text
         config_folder_files_exists_test = f"config_folder_files_exists exists\
             test result: {config_folder_files_exists}"
         check_files = {
             "ingress_folder": f"{ingress_folder}",
             "ingress_folder_files_exists_test":
             ingress_folder_files_exists_test,
             "config_folder": f"{config_folder}",
             "config_folder_files_exists_test": config_folder_files_exists_test,
-            "davt_database_folder": f"{davt_database_folder}",
-            "davt_database_folder_files_exists test": s_text_1,
-            "creating new davt_database_name": s_text_2
+            "pade_database_folder": f"{pade_database_folder}",
+            "pade_database_folder_files_exists test": s_text_1,
+            "creating new pade_database_name": s_text_2
         }
 
         return check_files
 
     @classmethod
     def get_job_list(cls, job_name: str, config: dict, spark: SparkSession) -> DataFrame:
         """Get list of jobs actions for a selected job
@@ -119,15 +124,15 @@
             config (dict): Configuration dictionary
             spark (SparkSession): Spark object
 
         Returns:
             DataFrame: Dataframe with list of job actions
         """
 
-        obj_env_log = davt_log_metadata.LoggingMetaData()
+        obj_env_log = pade_log_metadata.LoggingMetaData()
 
         ingress_folder_sps = config["ingress_folder_sps"]
         ingress_folder_sps = ingress_folder_sps.rstrip("/")
         config_jobs_path = f"{ingress_folder_sps}/bronze_sps_config_jobs.csv"
 
         project_id = config["project_id"]
         info_msg = f"config_jobs_path:{config_jobs_path}"
@@ -231,15 +236,15 @@
             dbutils (_type_): _description_
             spark (_type_): _description_
 
         Returns:
             int: _description_
         """
 
-        obj_env_file = davt_env_file.EnvironmentFile()
+        obj_env_file = pade_env_file.EnvironmentFile()
         file_size = obj_env_file.get_file_size(running_local,
                                                file_path, dbutils, spark)
         return file_size
 
     @staticmethod
     def file_exists(running_local: bool, path: str, dbutils) -> bool:
         """Takes in path, dbutils object, returns whether file exists at provided path
@@ -249,69 +254,106 @@
             path (str): path to file
             dbutils (object): databricks dbutils
 
         Returns:
             bool: True/False indication if file exists
         """
 
-        obj_env_file = davt_env_file.EnvironmentFile()
+        obj_env_file = pade_env_file.EnvironmentFile()
         file_exists = obj_env_file.file_exists(running_local, path, dbutils)
         return file_exists
 
     @staticmethod
-    def convert_windows_dir(path: str) -> str:
+    def convert_to_windows_dir(path: str) -> str:
+        """Takes in path and returns path with backslashes converted to forward slashes
+
+        Args:
+            path (str): path to be converted
+
+        Returns:
+            str: converted path
+        """
+        obj_env_file = pade_env_file.EnvironmentFile()
+        converted_path = obj_env_file.convert_to_windows_dir(path)
+        return converted_path
+
+    @staticmethod
+    def convert_to_current_os_dir(path: str) -> str:
         """Takes in path and returns path with backslashes converted to forward slashes
 
         Args:
             path (str): path to be converted
 
         Returns:
             str: converted path
         """
-        obj_env_file = davt_env_file.EnvironmentFile()
-        converted_path = obj_env_file.convert_windows_dir(path)
+        obj_env_file = pade_env_file.EnvironmentFile()
+        converted_path = obj_env_file.convert_to_current_os_dir(path)
         return converted_path
 
     @staticmethod
     def load_environment(running_local: bool, sp_tenant_id: str,
                          subscription_id: str,
                          sp_client_id: str,
                          environment: str,
                          project_id: str,
-                         dbutils):
-        """Loads the environment file to configure the enviornment
+                         dbutils,
+                         applicaton_insights_connection_string: str,
+                         az_sub_oauth_token_endpoint: str):
+        """  
+        Loads the environment file to configure the environment for the application.
 
         Args:
-            running_local (bool): _description_
-            sp_tenant_id (str): _description_
-            subscription_id (str): _description_
-            sp_client_id (str): _description_
-            environment (str): _description_
-            project_id (str): _description_
-            dbutils (_type_): _description_
+            running_local (bool): A flag indicating whether the application is running locally or deployed.
+            sp_tenant_id (str): The Azure Active Directory tenant (directory) ID.
+            subscription_id (str): The ID of the Azure subscription.
+            sp_client_id (str): The Azure service principal's client (application) ID.
+            environment (str): The deployment environment (e.g., 'dev', 'test', 'prod').
+            project_id (str): The project ID to which the application belongs.
+            dbutils: Databricks utilities object, which provides access to the Databricks filesystem and secrets, etc.
+            applicaton_insights_connection_string (str): The connection string for Azure Application Insights for application monitoring.
         """
 
         path = sys.executable + "\\.."
         sys.path.append(os.path.dirname(os.path.abspath(path)))
         env_path = os.path.dirname(os.path.abspath(path))
-        env_share_path = env_path + "\\share"
-        folder_exists = os.path.exists(env_share_path)
-        if not folder_exists:
-            # Create a new directory because it does not exist
-            os.makedirs(env_share_path)
-        env_share_path_2 = sys.executable + "\\..\\share"
-        sys.path.append(os.path.dirname(os.path.abspath(env_share_path_2)))
-
-        print( f"env_share_path: {env_share_path}")
 
+        OS_NAME = os.name
+        if dbutils is None:
+            running_local = True
         if running_local is True:
             print(f"running_local: {running_local}")
-            env_file_path = env_share_path + "\\.env"
-            print(f"env_file_path: {env_file_path}")
-            # don't delete line below - it creates the file
+            if OS_NAME.lower() == "nt":
+                print("windows")
+                env_share_path = env_path + "\\share"
+                folder_exists = os.path.exists(env_share_path)
+                if not folder_exists:
+                    # Create a new directory because it does not exist
+                    os.makedirs(env_share_path)
+                env_share_path_2 = sys.executable + "\\..\\share"
+                sys.path.append(os.path.dirname(
+                    os.path.abspath(env_share_path_2)))
+                env_file_path = env_share_path + "\\.env"
+                print(f"env_file_path: {env_file_path}")
+                # don't delete line below - it creates the file
+            else:
+                print("non windows")
+                #env_share_path = env_path + "/share"
+                env_share_path = os.path.expanduser("~") + '/share'
+                folder_exists = os.path.exists(env_share_path)
+                if not folder_exists:
+                    # Create a new directory because it does not exist
+                    os.makedirs(env_share_path)
+                env_share_path_2 = sys.executable + "/../share"
+                sys.path.append(os.path.dirname(
+                    os.path.abspath(env_share_path_2)))
+                env_file_path = env_share_path + "/.env"
+                print(f"env_file_path: {env_file_path}")
+                # don't delete line below - it creates the file
+
             env_file = open(env_file_path, "w+", encoding="utf-8")
             dotenv_file = find_dotenv(env_file_path)
             print(f"dotenv_file: {dotenv_file}")
             set_key(dotenv_file, "AZURE_TENANT_ID", sp_tenant_id)
             set_key(dotenv_file, "AZURE_SUBSCRIPTION_ID", subscription_id)
             set_key(dotenv_file, "AZURE_CLIENT_ID", sp_client_id)
         else:
@@ -319,196 +361,285 @@
             env_file_path = f"/mnt/{environment}/{project_id}"
             print(f"env_file_path: {env_file_path}")
             env_file_path = env_file_path + "/config/config_{environment}.txt"
             dbutils.fs.put(env_file_path, f"""AZURE_TENANT_ID {sp_tenant_id}
 AZURE_SUBSCRIPTION_ID {subscription_id}
 AZURE_CLIENT_ID {sp_client_id}
             """, True)
-            dotenv_file = find_dotenv(env_file_path)
-            load_dotenv(dotenv_file)
 
-        return "Success"
+        set_key(dotenv_file, "APPLICATIONINSIGHTS_CONNECTION_STRING",
+                applicaton_insights_connection_string)
+        set_key(dotenv_file, "AZURE_AUTHORITY_HOST ",
+                az_sub_oauth_token_endpoint)
+        set_key(dotenv_file, "PYARROW_IGNORE_TIMEZONE", "1")
+        dotenv_file = find_dotenv(env_file_path)
+        load_dotenv(dotenv_file)
+
+        return env_file_path
 
     @classmethod
     def get_configuration_common(cls, parameters: dict, dbutils) -> dict:
         """Takes in parameters dictionary and returns config dictionary
 
         Args:
             parameters (dict): global parameters dictionary
 
         Returns:
             dict: update global configuration dictionary
         """
 
-
-
         parameters.setdefault('running_local', False)
         parameters.setdefault('dataset_name', 'na')
         parameters.setdefault('cicd_action', 'na')
 
-
         if isinstance(parameters['running_local'], (bool)) is False:
-            running_local = parameters['running_local'].lower() in ['true', '1', 't', 'y', 'yes']
-        else: 
+            running_local = parameters['running_local'].lower() in [
+                'true', '1', 't', 'y', 'yes']
+        else:
             running_local = parameters['running_local']
 
+        if dbutils is None:
+            running_local = True
+
         project_id = parameters["project_id"]
         print(f"running_local: {running_local}")
-        azure_client_secret_key = parameters['azure_client_secret_key']
         environment = parameters["environment"]
         project_id_root = parameters["project_id_root"]
-        yyyy_param = parameters["yyyy"]
-        mm_param = parameters["mm"]
-        dd_param = parameters["dd"]
+        # Get the current year
+        current_year = str(datetime.now().year)
+        # Retrieve the parameter 'yyyy', and if it's not present, default to the current year
+        yyyy_param = parameters.get("yyyy", current_year)
+        # Get the current month
+        current_month = datetime.now().strftime('%m')
+        # Retrieve the parameter 'mm', and if it's not present, default to the current month
+        mm_param = parameters.get("mm", current_month)
+        # Get the current day
+        current_day = datetime.now().strftime('%d')
+        # Retrieve the parameter 'dd', and if it's not present, default to the current day
+        dd_param = parameters.get("dd", current_day)
+
         dataset_name = parameters["dataset_name"]
         cicd_action = parameters["cicd_action"]
         repository_path = parameters["repository_path"]
 
         # create logger
         logger = logging.getLogger(project_id)
         logger.setLevel(logging.DEBUG)
 
         config_string = "config"
         cicd_action_string = "cicd"
 
-        os_name_check = os.name
-        if os_name_check.lower() == "nt":
-            print("windows: nt")
-            repository_path = cls.convert_windows_dir(repository_path)
-
-        env_folder_path = repository_path.rstrip('/') + "/" + project_id_root + "/" + project_id + "/" + config_string
-        environment_json_path = env_folder_path + "/" + f"{config_string}.{environment}.json"
-        environment_json_path_default =  env_folder_path + "/" + f"{config_string}.{environment}.json"
-        # some times notebooks are not 2 folders deep - try parent folder
-        print(f"environment_json_path check 1: {environment_json_path}")
-        environment_json_path_defaault =  env_folder_path + "/" + f"{config_string}.{environment}.json"
-        if cls.file_exists(running_local, environment_json_path, None) is False:
+        repository_path = cls.convert_to_current_os_dir(repository_path)
+        env_folder_path = f"{repository_path.rstrip('/')}/{project_id_root}/{project_id}/"
+        env_folder_path = cls.convert_to_current_os_dir(env_folder_path)
+        config_folder_path = f"{env_folder_path}{config_string}/"
+        config_folder_path = cls.convert_to_current_os_dir(
+            config_folder_path)
+        environment_json_path = f"{config_folder_path}{config_string}.{environment}.json"
+        environment_json_path_default = f"{config_folder_path}{config_string}.{environment}.json"
+
+        # Check if environment_json_path exists
+        environment_json_path = cls.convert_to_current_os_dir(
+            environment_json_path)
+        logger.info(
+            f"environment_json_path check 1: {environment_json_path}")
+        if not cls.file_exists(running_local, environment_json_path, None):
+            logger.info(f"config does not exist: {environment_json_path}")
             repository_path_temp = os.getcwd()
-            repository_path_temp = str(Path(repository_path_temp).parent)
-            repository_path_temp = cls.convert_windows_dir(repository_path_temp)
+            repository_path_temp = str(Path(repository_path_temp))
             repository_path_temp = f"{repository_path_temp}{project_id_root}/{project_id}/{config_string}/"
-            environment_json_path = repository_path_temp + f"{config_string}.{environment}.json"
-            print(f"environment_json_path check 2: {environment_json_path}")
-            if cls.file_exists(running_local, environment_json_path, None) is False:
+            repository_path_temp = cls.convert_to_current_os_dir(
+                repository_path_temp)
+            environment_json_path = f"{repository_path_temp}{config_string}.{environment}.json"
+            logger.info(
+                f"environment_json_path check 2: {environment_json_path}")
+            if not cls.file_exists(running_local, environment_json_path, None):
+                logger.info(f"config does not exist: {environment_json_path}")
                 repository_path_temp = os.getcwd()
-                repository_path_temp = str(Path(repository_path_temp).parent.parent)
-                repository_path_temp = cls.convert_windows_dir(repository_path_temp)
+                repository_path_temp = str(Path(repository_path_temp).parent)
                 repository_path_temp = f"{repository_path_temp}{project_id_root}/{project_id}/{config_string}/"
-                environment_json_path = repository_path_temp + f"{config_string}.{environment}.json"
-                print(f"environment_json_path check 3: {environment_json_path}")
-                if cls.file_exists(running_local, environment_json_path, None) is False:
+                repository_path_temp = cls.convert_to_current_os_dir(
+                    repository_path_temp)
+                environment_json_path = f"{repository_path_temp}{config_string}.{environment}.json"
+                logger.info(
+                    f"environment_json_path check 3: {environment_json_path}")
+                if not cls.file_exists(running_local, environment_json_path, None):
+                    logger.info(
+                        f"config does not exist: {environment_json_path}")
+                    # Try two levels up from the current folder
                     repository_path_temp = os.getcwd()
-                    repository_path_temp = str(Path(repository_path_temp).parent.parent.parent)
-                    repository_path_temp = cls.convert_windows_dir(repository_path_temp)
+                    repository_path_temp = str(
+                        Path(repository_path_temp).parent.parent)
                     repository_path_temp = f"{repository_path_temp}{project_id_root}/{project_id}/{config_string}/"
-                    environment_json_path = repository_path_temp + f"{config_string}.{environment}.json"
-                    print(f"environment_json_path check 4: {environment_json_path}")
-                    if cls.file_exists(running_local, environment_json_path, None) is False:
-                        environment_json_path = environment_json_path_default
+                    repository_path_temp = cls.convert_to_current_os_dir(
+                        repository_path_temp)
+                    environment_json_path = f"{repository_path_temp}{config_string}.{environment}.json"
+                    logger.info(
+                        f"environment_json_path check 4: {environment_json_path}")
+                    if not cls.file_exists(running_local, environment_json_path, None):
+                        logger.info(
+                            f"config does not exist: {environment_json_path}")
+                        repository_path_temp = os.getcwd()
+                        repository_path_temp = str(
+                            Path(repository_path_temp).parent.parent.parent)
+                        repository_path_temp = cls.convert_to_current_os_dir(
+                            repository_path_temp)
+                        repository_path_temp = f"{repository_path_temp}{project_id_root}/{project_id}/{config_string}/"
+                        repository_path_temp = cls.convert_to_current_os_dir(
+                            repository_path_temp)
+                        environment_json_path = f"{repository_path_temp}{config_string}.{environment}.json"
+                        logger.info(
+                            f"environment_json_path check 5: {environment_json_path}")
+
+                        if not cls.file_exists(running_local, environment_json_path, None):
+                            logger.info(
+                                f"config does not exist: {environment_json_path}")
+                            environment_json_path = environment_json_path_default
+                        else:
+                            logger.info(
+                                f"config exists: {environment_json_path}")
+                    else:
+                        logger.info(f"config exists: {environment_json_path}")
+        else:
+            logger.info(f"config exists: {environment_json_path}")
 
         cicd_folder = f"{repository_path}{project_id_root}/{project_id}/{cicd_action_string}/"
-        cicd_action_path = f"{cicd_folder}" + f"{cicd_action}" + f".{environment}.json"
+        cicd_folder = cls.convert_to_current_os_dir(cicd_folder)
+        cicd_action_path = f"{cicd_folder}" + \
+            f"{cicd_action}" + f".{environment}.json"
 
         print("---- WORKING REPOSITORY FILE REFERENCE -------")
         print(f"environment_json_path: {environment_json_path}")
         print(project_id, "----------------------------------------------")
 
+        # Assuming `parameters` and `environment_json_path` are defined somewhere above this code.
+
         with open(environment_json_path, mode="r", encoding="utf-8") as json_file:
             config = json.load(json_file)
 
+        # Try to fetch from parameters, fallback to config, use an empty string as last resort
+        az_kv_az_sub_client_secret_key = parameters.get(
+            'az_kv_az_sub_client_secret_key') or config.get('az_kv_az_sub_client_secret_key', '')
+        azure_client_secret_key = parameters.get(
+            'azure_client_secret_key') or config.get('azure_client_secret_key', '')
+
+        # If the fetched values are empty, replace them with None
+        az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key if az_kv_az_sub_client_secret_key else azure_client_secret_key
+        azure_client_secret_key = azure_client_secret_key if azure_client_secret_key else az_kv_az_sub_client_secret_key
+
         config['running_local'] = running_local
         config["yyyy"] = yyyy_param
         config["mm"] = mm_param
         config["dd"] = dd_param
         config["dataset_name"] = dataset_name
         config["dataset_type"] = "TABLE"
         config["repository_path"] = repository_path
         config["environment_json_path"] = environment_json_path
         config["cicd_action_path"] = cicd_action_path
         config["azure_client_secret_key"] = azure_client_secret_key
-        config["ingress_folder_sps"] = "".join([config["config_folder"], "davt/"])
-        config["project_id"] = config["davt_project_id"]
-        config["project_id_root"] = config["davt_project_id_root"]
-        config["project_id_individual"] = config["davt_project_id_individual"]
+        config["ingress_folder_sps"] = "".join(
+            [config["config_folder"], "pade/"])
+        config["project_id"] = config["cdc_project_id"]
+        config["project_id_root"] = config["cdc_project_id_root"]
+        config["project_id_individual"] = config["cdc_project_id_individual"]
         project_id_individual = config["project_id_individual"]
-        config["databricks_instance_id"] = config["davt_databricks_instance_id"]
-        config["environment"] = config["davt_environment"]
+        config["databricks_instance_id"] = config.get(
+            "pade_databricks_instance_id")
+        config["environment"] = config["cdc_environment"]
         config["override_save_flag"] = "override_with_save"
         config["is_using_dataset_folder_path_override"] = False
         config["is_using_standard_column_names"] = "force_lowercase"
         config["is_export_schema_required_override"] = True
         config["ingress_mount"] = f"/mnt/{environment}/{project_id_individual}/ingress"
-
+        if config["az_kv_az_sub_client_secret_key"] is None:
+            config["az_kv_az_sub_client_secret_key"] = str(
+                az_kv_az_sub_client_secret_key)
         project_id = config["project_id"]
-        davt_database_folder = config["davt_database_folder"]
-        schema_dataset_file_path = (
-            davt_database_folder.rstrip("/") + "/bronze_clc_schema"
-        )
+        pade_database_folder = config.get("pade_database_folder")
+        if not pade_database_folder:
+            schema_dataset_file_path = ""
+        else:
+            schema_dataset_file_path = pade_database_folder.rstrip(
+                "/") + "/bronze_clc_schema"
         config["schema_dataset_file_path"] = schema_dataset_file_path
 
         if config:
-            print(f"Configuration found environment_json_path: {environment_json_path}")
+            print(
+                f"Configuration found environment_json_path: {environment_json_path}")
         else:
             error_message = "Error: no configurations were found."
-            error_message = error_message + f"Check your settings file: {environment_json_path}."
+            error_message = error_message + \
+                f"Check your settings file: {environment_json_path}."
             print(error_message)
 
-        scope = config['davt_databricks_kv_scope']
-        kv_client_id_key = config['davt_oauth_sp_kv_client_secret_key']
-        kv_client_secret_key = config['davt_oauth_sp_kv_client_secret_key']
-
-        if kv_client_id_key.strip() == '':
-            kv_client_id_key = None
-
-        if kv_client_secret_key.strip() == '':
-            kv_client_secret_key = None
-
-        sp_redirect_url = config["davt_oauth_sp_redirect_url"]
-        sp_authority_host_url = config["davt_oauth_sp_authority_host_url"]
-        sp_tenant_id = config["davt_azure_tenant_id"]
-        subscription_id = config["davt_azure_subscription_id"]
-        sp_client_id = config['azure_client_id']
-        sp_azure_databricks_resource_id = config['davt_oauth_databricks_resource_id']
+        scope = config.get('pade_databricks_kv_scope')
+        kv_client_id_key = config.get('pade_oauth_sp_kv_client_secret_key')
+        kv_client_secret_key = config.get('pade_oauth_sp_kv_client_secret_key')
+        if kv_client_id_key is not None:
+            if kv_client_id_key.strip() == '':
+                kv_client_id_key = None
+
+        if kv_client_secret_key is not None:
+            if kv_client_secret_key.strip() == '':
+                kv_client_secret_key = None
+
+        sp_redirect_url = config.get("pade_oauth_sp_redirect_url")
+        az_sub_oauth_token_endpoint = config.get("az_sub_oauth_token_endpoint")
+        sp_tenant_id = config["az_sub_tenant_id"]
+        subscription_id = config["az_sub_subscription_id"]
+        sp_client_id = config['az_sub_client_id']
+        sp_azure_databricks_resource_id = config.get(
+            'pade_oauth_databricks_resource_id')
+
+        az_apin_ingestion_endpoint = config.get("az_apin_ingestion_endpoint")
+        az_apin_instrumentation_key = config.get("az_apin_instrumentation_key")
+        applicaton_insights_connection_string = f"InstrumentationKey={az_apin_instrumentation_key};IngestionEndpoint={az_apin_ingestion_endpoint}"
+        az_sub_oauth_token_endpoint = config.get("az_sub_oauth_token_endpoint")
 
         # Write changes to .env file - create .env file if it does not exist
-        cls.load_environment(running_local, sp_tenant_id,
-                             subscription_id,
-                             sp_client_id,
-                             environment,
-                             project_id,
-                             dbutils)
+        env_file_path = cls.load_environment(running_local, sp_tenant_id,
+                                             subscription_id,
+                                             sp_client_id,
+                                             environment,
+                                             project_id,
+                                             dbutils,
+                                             applicaton_insights_connection_string,
+                                             az_sub_oauth_token_endpoint)
 
+        config["env_file_path"] = env_file_path
         if running_local is True:
             print(f"azure_client_secret_key:{azure_client_secret_key}")
             sp_client_secret = os.getenv(azure_client_secret_key)
         else:
             sp_client_secret = dbutils.secrets.get(scope=scope,
                                                    key=kv_client_secret_key)
 
         config["client_id"] = sp_client_id
         config["client_secret"] = sp_client_secret
-        config["tenant"] = sp_tenant_id
+        config["tenant_id"] = sp_tenant_id
+
+        sp_authority_host_url = "https://management.azure.com/.default"
 
         if sp_client_secret is None:
             config["error_message"] = "azure_client_secret_value_not_set_error"
         else:
-            obj_security_core = davt_sec_core.SecurityCore()
+            obj_security_core = pade_sec_core.SecurityCore()
 
             config_user = \
                 obj_security_core.acquire_access_token_with_client_credentials(sp_client_id,
                                                                                sp_client_secret,
                                                                                sp_tenant_id,
                                                                                sp_redirect_url,
                                                                                sp_authority_host_url,
                                                                                sp_azure_databricks_resource_id,
                                                                                project_id)
             config["redirect_uri"] = config_user["redirect_uri"]
             config["authority_host_url"] = config_user["authority_host_url"]
             config["azure_databricks_resource_id"] = config_user["azure_databricks_resource_id"]
-            config["authority_url"] = config_user["authority_url"]
+            config["az_sub_oauth_token_endpoint"] = config_user["az_sub_oauth_token_endpoint"]
             config["access_token"] = config_user["access_token"]
 
         return config
 
     @staticmethod
     def get_dataset_list(config: dict, spark: SparkSession) -> DataFrame:
         """Takes in config dictioarny, spark object, returns list of datasets in project
@@ -517,15 +648,15 @@
             config (dict): global config dictionary
             spark (SparkSession): spark session
 
         Returns:
             DataFrame: dataframe with list of datasets in project
         """
 
-        obj_env_log = davt_log_metadata.LoggingMetaData()
+        obj_env_log = pade_log_metadata.LoggingMetaData()
 
         first_row_is_header = "true"
         delimiter = ","
 
         csv_file_path = config["ingress_folder_sps"]
         csv_file_path = csv_file_path + '\\'
         csv_file_path = csv_file_path + "bronze_sps_config_datasets.csv"
@@ -540,15 +671,16 @@
             .option("inferSchema", True)
             .load(
                 csv_file_path, forceLowercaseNames=True,
                 inferLong=True
             )
             .withColumn("meta_ingesttimestamp", lit(ingesttimestamp))
             .withColumn(
-                "row_id", concat_ws("-", col("project_id"), col("dataset_name"))
+                "row_id", concat_ws("-", col("project_id"),
+                                    col("dataset_name"))
             )
         )
 
         # sort
         if df_results.count() > 0:
             # df_results.show()
             df_results = df_results.sort("pipeline_batch_group")
@@ -614,15 +746,15 @@
             token (str): token
             base_path (str): path to list files
 
         Returns:
             list: list of files at the path location
         """
 
-        obj_env_log = davt_log_metadata.LoggingMetaData()
+        obj_env_log = pade_log_metadata.LoggingMetaData()
 
         databricks_instance_id = config["databricks_instance_id"]
         json_text = {"path": base_path}
         headers = {"Authentication": f"Bearer {token}"}
         url = f"https://{databricks_instance_id}/api/2.0/workspace/list"
         project_id = config["project_id"]
         obj_env_log.log_info(config, f"------- Fetch {base_path}  -------")
@@ -669,40 +801,41 @@
             config (dict): global config dictionary
             spark (SparkSession): spark session
 
         Returns:
             str: folder_database_path
         """
 
-        davt_database_name = config["davt_database_name"]
-        davt_database_folder = config["davt_database_folder"]
+        pade_database_name = config["pade_database_name"]
+        pade_database_folder = config["pade_database_folder"]
 
         running_local = config["running_local"]
 
         if running_local is True:
             # use default location
-            sql_statement = f"create database if not exists {davt_database_name};"
+            sql_statement = f"create database if not exists {pade_database_name};"
         else:
-            sql_statement = f"create database if not exists {davt_database_name}  LOCATION '{davt_database_folder}';"
+            sql_statement = f"create database if not exists {pade_database_name}  LOCATION '{pade_database_folder}';"
 
         print(sql_statement)
         spark.sql(sql_statement)
 
-        # davt_databricks_owner_group = config["davt_databricks_owner_group"]
-        # sql_statement = f"alter schema {davt_database_name} owner to `{davt_databricks_owner_group}`;"
+        # pade_databricks_owner_group = config["pade_databricks_owner_group"]
+        # sql_statement = f"alter schema {pade_database_name} owner to `{pade_databricks_owner_group}`;"
         # print(sql_statement)
         # spark.sql(sql_statement)
 
-        sql_statement = f"Describe database {davt_database_name}"
+        sql_statement = f"Describe database {pade_database_name}"
         df_db_schema = spark.sql(sql_statement)
 
         if running_local is True:
             df_db_schema.show(truncate=False)
 
-        df_db_schema = df_db_schema.filter(df_db_schema.database_description_item == "Location")
+        df_db_schema = df_db_schema.filter(
+            df_db_schema.database_description_item == "Location")
         rdd_row = df_db_schema.first()
 
         if rdd_row is not None:
             folder_database_path = rdd_row["database_description_value"]
         else:
             folder_database_path = "missing dataframe value error"
 
@@ -717,27 +850,27 @@
             spark (SparkSession): spark session
             config (dict): global config dictionary
 
         Returns:
             SparkSession: configured spark session
         """
 
-        obj_env_log = davt_log_metadata.LoggingMetaData()
+        obj_env_log = pade_log_metadata.LoggingMetaData()
 
-        c_ep = config["davt_oauth_sp_authority_host_url"]
+        c_ep = config["pade_oauth_sp_authority_host_url"]
         c_id = config["client_id"]
         c_secret = config["client_secret"]
-        sp_tenant_id = config["davt_azure_tenant_id"]
+        sp_tenant_id = config["az_sub_tenant_id"]
         running_local = config['running_local']
         project_id = config['project_id']
 
         client_secret_exists = True
         if c_id is None or c_secret is None:
             client_secret_exists = False
-        storage_account = config["davt_azure_storage_account"]
+        storage_account = config["pade_azure_storage_account"]
 
         client_token_provider = "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider"
         provider_type = "OAuth"
 
         # stack overflow example
         fs_prefix_e1 = "fs.azure.account.auth."
         fso_prefix_e1 = "fs.azure.account.oauth"
@@ -755,41 +888,48 @@
         config["run_as"] = "service_principal"
         run_as = config["run_as"]
         print(f"running databricks access using run_as:{run_as}")
 
         if (client_secret_exists is True) and (run_as == "service_principal") and running_local is True:
 
             spark.conf.set(f"{fs_prefix_e1}type{fs_suffix_e1}", provider_type)
-            spark.conf.set(f"{fso_prefix_e1}.provider.type{fs_suffix_e1}", client_token_provider)
+            spark.conf.set(
+                f"{fso_prefix_e1}.provider.type{fs_suffix_e1}", client_token_provider)
             spark.conf.set(f"{fso2_prefix_e1}.client.id{fs_suffix_e1}", c_id)
-            spark.conf.set(f"{fso2_prefix_e1}.client.secret{fs_suffix_e1}", c_secret)
+            spark.conf.set(
+                f"{fso2_prefix_e1}.client.secret{fs_suffix_e1}", c_secret)
             client_endpoint_e1 = f"https://login.microsoftonline.com/{sp_tenant_id}/oauth2/token"
-            spark.conf.set(f"{fso2_prefix_e1}.client.endpoint{fs_suffix_e1}", client_endpoint_e1)
+            spark.conf.set(
+                f"{fso2_prefix_e1}.client.endpoint{fs_suffix_e1}", client_endpoint_e1)
 
-            obj_env_log.log_info(config, f'spark.conf.set "({fs_prefix_e1}type{fs_suffix_e1}", "{provider_type}")')
+            obj_env_log.log_info(
+                config, f'spark.conf.set "({fs_prefix_e1}type{fs_suffix_e1}", "{provider_type}")')
             obj_env_log.log_info(config, f'spark.conf.set "({fso_prefix_e1}.provider.type{fs_suffix_e1}", \
                 "{client_token_provider}")')
-            obj_env_log.log_info(config, f'spark.conf.set "({fso2_prefix_e1}.client.id{fs_suffix_e1}", "{c_id}")')
+            obj_env_log.log_info(
+                config, f'spark.conf.set "({fso2_prefix_e1}.client.id{fs_suffix_e1}", "{c_id}")')
             obj_env_log.log_info(config, f'spark.conf.set "{fso2_prefix_e1}.client.endpoint{fs_suffix_e1}" \
                 = "{client_endpoint_e1}"')
 
         spark.conf.set("spark.databricks.io.cache.enabled", "true")
         # Enable Arrow-based columnar data transfers
         spark.conf.set("spark.sql.execution.arrow.enabled", "true")
         # sometimes azure storage has a delta table not found bug - in that scenario try filemount above
         spark.conf.set("spark.sql.execution.arrow.fallback.enabled", "true")
         spark.conf.set("spark.databricks.pyspark.enablePy4JSecurity", "false")
         # Enable Delta Preview
         spark.conf.set("spark.databricks.delta.preview.enabled ", "true")
 
-        if running_local is False and project_id != 'ezdx_foodnet':
-            spark.sql("SET spark.databricks.delta.schema.autoMerge.enabled = true")
-            davt_checkpoint_folder = config["davt_checkpoint_folder"]
-            print(f"davt_checkpoint_folder: {davt_checkpoint_folder}")
-            spark.sparkContext.setCheckpointDir(davt_checkpoint_folder)
+        if running_local is False:
+            os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
+            spark.sql(
+                "SET spark.databricks.delta.schema.autoMerge.enabled = true")
+            pade_checkpoint_folder = config["pade_checkpoint_folder"]
+            print(f"pade_checkpoint_folder: {pade_checkpoint_folder}")
+            spark.sparkContext.setCheckpointDir(pade_checkpoint_folder)
 
         # Checkpoint
         return spark
 
 
 class HTMLFilter(HTMLParser):
     """Parses HTMLData
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from dateutil.relativedelta import relativedelta
 from pathlib import Path
 import json
 import copy
 import pandas as pd_legacy
 from pyspark.sql.functions import trim
 from pyspark.sql import (DataFrame)
-import data_ecosystem_services.self_service.pipeline_metadata as davt_pl_metadata
-import data_ecosystem_services.self_service.dataset_metadata as davt_ds_metadata
-import data_ecosystem_services.self_service.environment_metadata as davt_env_metadata
-import data_ecosystem_services.self_service.logging_metadata as davt_log_metadata
-import data_ecosystem_services.tech_environment_service.job_core as davt_job_core
-import data_ecosystem_services.tech_environment_service.repo_core as davt_repo_core
-import data_ecosystem_services.tech_environment_service.dataset_crud as davt_ds_crud
-import data_ecosystem_services.tech_environment_service.dataset_core as davt_ds_core
-import data_ecosystem_services.tech_environment_service.environment_file as davt_env_file
+import data_ecosystem_services.cdc_self_service.pipeline_metadata as davt_pl_metadata
+import data_ecosystem_services.cdc_self_service.dataset_metadata as davt_ds_metadata
+import data_ecosystem_services.cdc_self_service.environment_metadata as davt_env_metadata
+import data_ecosystem_services.cdc_self_service.logging_metadata as davt_log_metadata
+import data_ecosystem_services.cdc_tech_environment_service.job_core as davt_job_core
+import data_ecosystem_services.cdc_tech_environment_service.repo_core as davt_repo_core
+import data_ecosystem_services.cdc_tech_environment_service.dataset_crud as davt_ds_crud
+import data_ecosystem_services.cdc_tech_environment_service.dataset_core as davt_ds_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as davt_env_file
 
 IPY_ENABLED = False
 running_local = ("dbutils" in locals() or "dbutils" in globals()) is not True
 if running_local is True and IPY_ENABLED is True:
     from ipywidgets import Dropdown, HBox, Button, Label, Layout
     from IPython.display import display
 
@@ -113,15 +113,15 @@
             str: HBox setting display status
         """
 
         obj_env = davt_env_metadata.EnvironmentMetaData()
         obj_env_log = davt_log_metadata.LoggingMetaData()
         running_local = config["running_local"]
         ingress_folder_sps = config["ingress_folder_sps"]
-        sp_tenant_id = config["davt_azure_tenant_id"]
+        sp_tenant_id = config["az_sub_tenant_id"]
         subscription_id = config["davt_azure_subscription_id"]
         sp_client_id = config['azure_client_id']
         environment = config['environment']
         project_id = config['project_id']
 
         obj_env.load_environment(running_local, sp_tenant_id,
                                  subscription_id,
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module to log warning, debug, error and info messages based on project metadata
 """
 import sys
 import os
 
-import data_ecosystem_services.admin_service.environment_logging as davt_env_log
+import data_ecosystem_services.cdc_admin_service.environment_logging as davt_env_log
 
 class LoggingMetaData:
     """
     Class to log warning, debug, error and info messages based on project metadata
     """
 
     @staticmethod
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
     # import pyspark.pandas  as pd
     # bug - pyspark version will not read local files in the repo
+    os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
     import pyspark.pandas as pd
 else:
     import pandas as pd
 
 
 class PipelineMetaData:
     """Class to conditionally execute transform logic for silver and gold pipelines based on project metadata
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""Initialize the tech_environment_service subpackage of pade_python package"""
+"""Initialize the cdc_tech_environment_service subpackage of pade_python package"""
 
 # allow absolute import from the root folder
 # whatever its name is.
+import data_ecosystem_services.az_storage_service.az_storage_queue
+import data_ecosystem_services.cdc_tech_environment_service.job_core
+import data_ecosystem_services.cdc_tech_environment_service.repo_core
+import data_ecosystem_services.cdc_security_service.security_core
+import data_ecosystem_services.cdc_admin_service.environment_logging
+import data_ecosystem_services.cdc_tech_environment_service.environment_spark
+import data_ecosystem_services.cdc_tech_environment_service.environment_file
+import data_ecosystem_services.cdc_tech_environment_service.environment_core
+import data_ecosystem_services.cdc_tech_environment_service.dataset_crud
+import data_ecosystem_services.cdc_tech_environment_service.dataset_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_http
 import sys  # don't remove required for error handling
 import os
 
-# Import from sibling directory ..\tech_environment_service
+# Import from sibling directory ..\cdc_tech_environment_service
 OS_NAME = os.name
 
 sys.path.append("..")
 
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("cdc_tech_environment_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
-    sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
+    sys.path.append(os.path.dirname(
+        os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("cdc_tech_environment_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
-
-
-import data_ecosystem_services.tech_environment_service.dataset_core
-import data_ecosystem_services.tech_environment_service.dataset_crud
-import data_ecosystem_services.tech_environment_service.environment_core
-import data_ecosystem_services.tech_environment_service.environment_file
-import data_ecosystem_services.tech_environment_service.environment_spark
-import data_ecosystem_services.admin_service.environment_logging
-import data_ecosystem_services.security_service.security_core
-import data_ecosystem_services.tech_environment_service.repo_core
-import data_ecosystem_services.tech_environment_service.job_core
-import data_ecosystem_services.az_storage_service.az_storage_queue
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from azure.identity import ClientSecretCredential
 
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
-import data_ecosystem_services.tech_environment_service.environment_file as pade_env_file
-import data_ecosystem_services.tech_environment_service.dataset_core as pade_ds_core
-import data_ecosystem_services.security_service.security_core as pade_sec_core
-import data_ecosystem_services.tech_environment_service.environment_core as pade_env_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
+import data_ecosystem_services.cdc_tech_environment_service.dataset_core as pade_ds_core
+import data_ecosystem_services.cdc_security_service.security_core as pade_sec_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_core as pade_env_core
 
 
 # data
 import numpy as np
 
 # spark / data
 import uuid
@@ -60,14 +60,15 @@
 from collections import Counter
 
 import pandas as pd_legacy
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
+    os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files
     # import pandas as pd
 else:
     import pandas as pd
 
 class DataSetConvert:
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from pyspark.sql.functions import (
     lit,
     udf,
     expr,
     coalesce
 )
 
-from pyspark.sql.types import StringType,StructField
-
+from pyspark.sql.types import StringType, StructField
 
+import os
 # util
 import hashlib
 
 import uuid
 uuid_udf = udf(lambda: str(uuid.uuid4()), StringType())
 
+os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files in the repo
     # import pandas as pd
@@ -42,23 +43,29 @@
 
     Returns:
         _type_: Encrypted value
     """
     sha_value = hashlib.sha1(pii_col.encode()).hexdigest()
     return sha_value
 
+
 encrypt_value_udf = udf(encrypt_value, StringType())
 
 
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
 class DataSetCore:
     """Core class for Spark Datasets
 
     """
 
-
     @classmethod
     def add_row_id_to_dataframe(cls, sorted_df: DataFrame, row_id_keys: str,
                                 yyyy_param: str, mm_param: str, dd_param: str) -> DataFrame:
         """Adds row_id column to the dataframe, the row_id a required unique identifier used
         to perform incremntal updates.
         - Replaces {yyyy}, {mm}, or {dd} with the current year, month, or day in row id template
         - Create row_id based on template
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Module with a variety of create, read, update and delete
 functions for Spark data frames. """
 
+from delta.tables import DeltaTable
 import sys  # don't remove required for error handling
 import os
 
 
 from pathlib import Path
 from urllib.parse import urlparse
 from io import BytesIO
@@ -24,18 +25,18 @@
 from azure.storage.filedatalake import DataLakeServiceClient
 
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
-import data_ecosystem_services.tech_environment_service.dataset_core as pade_ds_core
-import data_ecosystem_services.tech_environment_service.environment_file as pade_env_file
-import data_ecosystem_services.security_service.security_core as pade_sec_core
-import data_ecosystem_services.tech_environment_service.environment_core as pade_env_core
+import data_ecosystem_services.cdc_tech_environment_service.dataset_core as pade_ds_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
+import data_ecosystem_services.cdc_security_service.security_core as pade_sec_core
+import data_ecosystem_services.cdc_tech_environment_service.environment_core as pade_env_core
 
 # spark / data
 import uuid
 from pyspark.sql import SparkSession, DataFrame
 import pyspark.sql.utils
 import pyspark.sql.functions as f
 from pyspark.sql.functions import (
@@ -44,15 +45,15 @@
     concat_ws,
     udf
 )
 
 from pyspark.sql.types import StructType, StructField, LongType, StringType
 uuid_udf = udf(lambda: str(uuid.uuid4()), StringType())
 
-from delta.tables import DeltaTable
+os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files in the repo
     # import pandas as pd
@@ -131,28 +132,29 @@
         if file_format == "delta":
             file_format = "parquet_delta"
 
         is_internal_dataset = True
         test_flag = ""
         location_flag = "managed internally"
 
-        pade_database_folder = config["pade_database_folder"]
+        pade_database_folder = config.get("pade_database_folder")
         not_found = -1
 
         if dataset_file_path.find(pade_database_folder) is not_found:
             is_using_dataset_folder_path_override = True
             is_internal_dataset = False
             test_flag = " not"
             location_flag = "managed externally"
         elif (is_using_dataset_folder_path_override is True and file_format == "parquet_delta"):
             is_internal_dataset = False
             test_flag = " not"
             location_flag = "managed externally"
 
-        table_exists_flag = obj_ds_core.table_exists(spark, dataset_name, database_name)
+        table_exists_flag = obj_ds_core.table_exists(
+            spark, dataset_name, database_name)
 
         print(f"database_name:{database_name} dataset_name:{dataset_name}")
         print(f"location_flag: {location_flag}")
         print(f"pade_database_folder:{pade_database_folder}")
         print(f"test_flag:{test_flag} in {dataset_file_path}")
         print(f"test if dataset exists:{dataset_name}")
         print(f"for database: {database_name} returned: {table_exists_flag}")
@@ -201,128 +203,151 @@
                 print(f"by {partition_by}")
                 one = 1
                 # don't merge schema for replace
                 # .option( "mergeSchema", "true")
                 if len(partition_by_array) is one:
                     print("paritioned (1) parquet saveastable : managed folder")
                     p_by = partition_by_array[0].strip()
-                    df_crud.write.mode("overwrite").format("delta").partitionBy(p_by).saveAsTable(full_dataset_name)
+                    df_crud.write.mode("overwrite").format("delta").partitionBy(
+                        p_by).saveAsTable(full_dataset_name)
                 else:
                     if len(partition_by_array) > one:
                         p_by_0 = partition_by_array[0].strip()
                         p_by_1 = partition_by_array[1].strip()
                         df_crud.write.mode("overwrite").format("delta").partitionBy(
                             p_by_0).partitionBy(
                             p_by_1).saveAsTable(full_dataset_name)
                     else:
                         # no partition
                         # don't merge schema for replace
                         # .option("mergeSchema", "true")
-                        print("paritioned (0) parquet saveastable : non managed folder override")
-                        df_crud.write.mode("overwrite").format("delta").saveAsTable(full_dataset_name)
+                        print(
+                            "paritioned (0) parquet saveastable : non managed folder override")
+                        df_crud.write.mode("overwrite").format(
+                            "delta").saveAsTable(full_dataset_name)
             else:
                 print("unparitioned parquet saveastable : managed folder")
                 # .option("mergeSchema", "true")
                 try:
-                    df_crud.write.mode("overwrite").format("delta").saveAsTable(full_dataset_name)
+                    df_crud.write.mode("overwrite").format(
+                        "delta").saveAsTable(full_dataset_name)
                 except pyspark.sql.utils.AnalysisException as ex_analysis:
                     print(f"Error saving dataframe: {full_dataset_name}")
                     print("An exception occurred: " + str(ex_analysis))
                     # rename and try again
                     # .option("mergeSchema", "true")
                     sql_command = f"DROP TABLE IF EXISTS {full_dataset_name}"
                     spark.sql(sql_command)
                     try:
-                        df_crud.write.mode("overwrite").format("delta").saveAsTable(full_dataset_name)
+                        df_crud.write.mode("overwrite").format(
+                            "delta").saveAsTable(full_dataset_name)
                     except pyspark.sql.utils.AnalysisException as ex_analysis_1:
                         print("Error saving dataframe: full_dataset_name")
                         print("An exception occurred: " + str(ex_analysis_1))
                         for c_original in df_crud.columns:
-                            c_renamed = obj_ds_core.scrub_object_name(c_original)
-                            df_crud = df_crud.withColumnRenamed(c_original, c_renamed)
+                            c_renamed = obj_ds_core.scrub_object_name(
+                                c_original)
+                            df_crud = df_crud.withColumnRenamed(
+                                c_original, c_renamed)
 
         # dataset is parquet internal to database directory and incremental refresh
         print(f"is_internal_dataset:{is_internal_dataset}")
         print(f"incremental:{incremental}")
         if (is_internal_dataset is True) and (incremental == "incremental" or incremental == "incremental_with_purge"):
-            table_exists = obj_ds_core.table_exists(spark, dataset_name, database_name)
+            table_exists = obj_ds_core.table_exists(
+                spark, dataset_name, database_name)
             is_external_table = False
             if (file_format != "parquet_delta" or dataset_name == "bronze_clc_schema"):
                 is_external_table = True
             if table_exists and is_external_table:
                 if (incremental == "incremental_with_purge" and dataset_name != "bronze_clc_schema"):
                     sql_command = f"DELETE FROM {full_dataset_name} where "
-                    sql_command = sql_command + " __meta_ingress_file_path = '{ingress_file_path}'"
+                    sql_command = sql_command + \
+                        " __meta_ingress_file_path = '{ingress_file_path}'"
                     print(f"attempting sql_command:{sql_command}")
                     spark.sql(sql_command)
 
-                print(f"attempting to modifying existing dataset:{full_dataset_name}")
-                print(f"with data from {ingress_file_path} in format {file_format}")
+                print(
+                    f"attempting to modifying existing dataset:{full_dataset_name}")
+                print(
+                    f"with data from {ingress_file_path} in format {file_format}")
                 print(f"with merge at path {dataset_file_path}")
 
                 match_expr = "delta.row_id = updates.row_id and updates.row_id = delta.row_id"
                 delta_dataset = None
 
                 try:
-                    delta_dataset = DeltaTable.forPath(spark, dataset_file_path)
+                    delta_dataset = DeltaTable.forPath(
+                        spark, dataset_file_path)
 
                     delta_dataset.alias("delta").merge(
                         df_crud.alias("updates"), match_expr
                     ).whenMatchedUpdateAll().whenNotMatchedInsertAll().execute()
                     return True
                 except Exception as exception_check:
-                    print("merge request input of the following dataframe:" + str(exception_check))
+                    print(
+                        "merge request input of the following dataframe:" + str(exception_check))
                     # display(df_crud)
-                    print("merge request output of the following dataframe" + str(exception_check))
+                    print(
+                        "merge request output of the following dataframe" + str(exception_check))
                     if delta_dataset is not None:
                         df_crud_history = delta_dataset.history()
                         # display(df_crud_history)
                     raise
             else:
-                print(f"table_exists:{obj_ds_core.table_exists(spark, dataset_name, database_name)}")
-                print(f"is_internal_dataset:{is_internal_dataset} dataset_name:{dataset_name}")
-                print(f"database_name:{database_name} file_format:{file_format}")
+                print(
+                    f"table_exists:{obj_ds_core.table_exists(spark, dataset_name, database_name)}")
+                print(
+                    f"is_internal_dataset:{is_internal_dataset} dataset_name:{dataset_name}")
+                print(
+                    f"database_name:{database_name} file_format:{file_format}")
                 print("attempting to create Delta dataset")
                 print(f"{full_dataset_name}: at")
                 print(f"{dataset_file_path}")
                 # Dataset hot references external file
                 if is_internal_dataset is False:
                     if file_format == "parquet":
                         sql_command = f"CREATE TABLE IF NOT EXISTS {full_dataset_name} "
-                        sql_command = sql_command + f" USING PARQUET LOCATION '{dataset_file_path}'"
+                        sql_command = sql_command + \
+                            f" USING PARQUET LOCATION '{dataset_file_path}'"
                     else:
                         sql_command = f"CREATE TABLE IF NOT EXISTS {full_dataset_name} "
-                        sql_command = sql_command + f" USING DELTA LOCATION '{dataset_file_path}'"
+                        sql_command = sql_command + \
+                            f" USING DELTA LOCATION '{dataset_file_path}'"
                     spark.sql(sql_command)
                     print(f"created Delta dataset {full_dataset_name}:")
                     print(f"at {dataset_file_path}")
                 else:
                     if file_format == "parquet":
                         print("error attempting to load a parquet directory")
                         print(f"that does not exist: {dataset_file_path}")
                     else:
                         if partition_by is not None:
                             partition_by_array = partition_by.split(",")
-                            print(f"writing {full_dataset_name} to {dataset_file_path}")
+                            print(
+                                f"writing {full_dataset_name} to {dataset_file_path}")
                             print(f"with partition by {partition_by}")
 
                             if len(partition_by_array) == 1:
-                                print(f"df_crud.write.format('delta').partitionBy({partition_by_array[0].strip()})")
+                                print(
+                                    f"df_crud.write.format('delta').partitionBy({partition_by_array[0].strip()})")
                                 print(f".saveAsTable({full_dataset_name})")
                                 df_crud.write.format("delta").option(
                                     "mergeSchema", "true"
                                 ).partitionBy(
                                     partition_by_array[0].strip()
                                 ).saveAsTable(
                                     full_dataset_name
                                 )
                             else:
                                 if len(partition_by_array) > 1:
-                                    print(f"df_crud.write.format('delta').partitionBy({partition_by_array[0].strip()})")
-                                    print(f".partitionBy({partition_by_array[1].strip()}).")
+                                    print(
+                                        f"df_crud.write.format('delta').partitionBy({partition_by_array[0].strip()})")
+                                    print(
+                                        f".partitionBy({partition_by_array[1].strip()}).")
                                     print(f"saveAsTable({full_dataset_name})")
                                     df_crud.write.format("delta").option(
                                         "mergeSchema", "true"
                                     ).partitionBy(
                                         partition_by_array[0].strip()
                                     ).partitionBy(
                                         partition_by_array[1].strip()
@@ -370,15 +395,15 @@
             _type_: _description_
         """
 
         obj_ds_core = pade_ds_core.DataSetCore()
 
         schema_dataset_file_path = config["schema_dataset_file_path"]
         row_id_column_names = ""
-        pade_database_folder = config["pade_database_folder"]
+        pade_database_folder = config.get("pade_database_folder")
         environment = config["environment"]
         project_id = config["project_id"]
 
         is_using_dataset_folder_path_override = False
 
         if view_or_schema == "view":
             dataset_name = config_dataset_or_notebook["view_name"]
@@ -398,57 +423,66 @@
         schema_full_dataset_name = f"pade_{project_id}_{environment}.bronze_clc_schema"
 
         if is_export_schema_required_override != "force_off":
             clc_dataset_name = "bronze_clc_schema"
             if obj_ds_core.table_exists(spark, clc_dataset_name, pade_database_name) is True:
                 print(f"delete {full_dataset_name} from: {clc_dataset_name}")
                 delete_sql = f"Delete from {pade_database_name}.bronze_clc_schema"
-                delete_sql = delete_sql + f" where full_dataset_name = '{full_dataset_name}'"
+                delete_sql = delete_sql + \
+                    f" where full_dataset_name = '{full_dataset_name}'"
                 df_deleted = spark.sql(delete_sql)
                 print("deleted rows: " + str(df_deleted.count()))
             print(f"describe {full_dataset_name} for: bronze_clc_schema")
             df_schema = spark.sql("Describe Table dataset_sorted_df")
             df_schema = df_schema.distinct()
             df_schema = df_schema.withColumn("dataset_name", lit(dataset_name))
-            df_schema = df_schema.withColumn("full_dataset_name", lit(full_dataset_name))
-            df_schema = df_schema.withColumn("dataset_file_path", lit(dataset_file_path))
+            df_schema = df_schema.withColumn(
+                "full_dataset_name", lit(full_dataset_name))
+            df_schema = df_schema.withColumn(
+                "dataset_file_path", lit(dataset_file_path))
             df_schema = df_schema.withColumnRenamed("col_name", "column_name")
-            df_schema = df_schema.withColumnRenamed("data_type", "data_type_name")
+            df_schema = df_schema.withColumnRenamed(
+                "data_type", "data_type_name")
             row_id_keys_databricks = "col('dataset_name'),col('column_name')"
-            arg_list = [eval(col_name.strip()) for col_name in row_id_keys_databricks.split(",")]
-            df_schema = df_schema.withColumn("row_id_databricks", concat_ws("-", *arg_list))
+            arg_list = [eval(col_name.strip())
+                        for col_name in row_id_keys_databricks.split(",")]
+            df_schema = df_schema.withColumn(
+                "row_id_databricks", concat_ws("-", *arg_list))
             if row_id_keys is None:
                 row_id_keys = ""
             col_list = [
                 ((x.strip().replace("col('", "").replace("')", "")))
                 for x in row_id_keys.split(",")
             ]
             row_id_column_names = str(",".join(col_list))
             print("row_id_column_names: " + row_id_column_names)
             print("updated databricks metadata for: schema_databricks_df")
 
             merged_df = df_schema
-            merged_df = merged_df.withColumn("row_id", col("row_id_databricks"))
+            merged_df = merged_df.withColumn(
+                "row_id", col("row_id_databricks"))
             merged_df = merged_df.drop("row_id_databricks")
             merged_df = merged_df.drop("row_id_koalas")
             merged_df = merged_df.withColumn("unique_count", lit(0))
             merged_df = merged_df.withColumn("null_count", lit(0))
             merged_df = merged_df.withColumn("max_length", lit(0))
             merged_df = merged_df.withColumn("min_length", lit(0))
             merged_df = merged_df.withColumn("ingress_column_name", lit(""))
             merged_df = merged_df.withColumn("ingress_column_format", lit(""))
             merged_df = merged_df.withColumn("ingress_column_label", lit(""))
             merged_df = merged_df.withColumn("unique_count_scrubbed", lit(0))
             merged_df = merged_df.withColumn("scope", lit("column"))
-            merged_df = merged_df.withColumn("row_id_column", lit(row_id_column_names))
-            merged_df = merged_df.withColumn("row_count",  lit(0))
-            merged_df = merged_df.withColumn("ingress_row_count",  lit(0))
-            merged_df = merged_df.withColumn("ingress_ordinal_position",  lit(0))
-            merged_df = merged_df.withColumn("ingress_column_length",  lit(0))
-            merged_df = merged_df.withColumn("ingress_table_name",  lit(0))
+            merged_df = merged_df.withColumn(
+                "row_id_column", lit(row_id_column_names))
+            merged_df = merged_df.withColumn("row_count", lit(0))
+            merged_df = merged_df.withColumn("ingress_row_count", lit(0))
+            merged_df = merged_df.withColumn(
+                "ingress_ordinal_position", lit(0))
+            merged_df = merged_df.withColumn("ingress_column_length", lit(0))
+            merged_df = merged_df.withColumn("ingress_table_name", lit(0))
 
             schema = StructType(
                 [
                     StructField("column_name", StringType(), False),
                     StructField("data_type_name", StringType(), False),
                     StructField("comment", StringType(), True),
                     StructField("dataset_name", StringType(), False),
@@ -471,19 +505,22 @@
                     StructField("ingress_column_length", LongType(), True),
                     StructField("ingress_table_name", StringType(), True),
                 ]
             )
 
             # display(merged_df)
 
-            schema_column_df = spark.createDataFrame(merged_df.rdd, schema=schema)
+            schema_column_df = spark.createDataFrame(
+                merged_df.rdd, schema=schema)
             key = "is_using_dataset_folder_path_override"
             is_using_dataset_folder_path_override = config[key]
-            schema_dataset_file_path = pade_database_folder.rstrip("/") + "/bronze_clc_schema"
-            schema_dataset_file_path = schema_dataset_file_path.replace("dbfs:", "")
+            schema_dataset_file_path = pade_database_folder.rstrip(
+                "/") + "/bronze_clc_schema"
+            schema_dataset_file_path = schema_dataset_file_path.replace(
+                "dbfs:", "")
             partitioned_by = "dataset_name"
 
             empty = ""
             row_id = full_dataset_name
             scope = "dataset"
             row_data = [
                 (
@@ -500,19 +537,19 @@
                     (0),
                     (empty),
                     (empty),
                     (empty),
                     (0),
                     (scope),
                     "full_dataset_name",
-                     (0),
-                     (0),
-                     (0),
-                     (0),
-                     (0),
+                    (0),
+                    (0),
+                    (0),
+                    (0),
+                    (0),
                 )
             ]
 
             print("row_data: " + str(row_data))
             schema_dataset_df = spark.createDataFrame(row_data, schema)
         else:
             partitioned_by = ""
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from io import BytesIO
 
 # libraries
 from importlib import util
 
 import pyreadstat as prs
 import pandas as pd_legacy
+os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 from pyspark.sql import SparkSession, DataFrame
 
 if pyspark_pandas_found:
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files
@@ -24,15 +25,15 @@
     import pandas as pd
 
 # adls and azure security
 from azure.storage.filedatalake import DataLakeServiceClient
 from azure.identity import ClientSecretCredential
 
 # PADE
-import data_ecosystem_services.tech_environment_service.environment_file as pade_env_file
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
 
 class DataSetExtract:
     """DataSetExtract class for Spark Datasets handle metadata extraction from different source formats
     """
 
     @classmethod
     def extract_xpt_dataframe_schema(cls, spark: SparkSession, ingress_file_path: str, tenant_id: str,
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Module for spark and os environment for tech_environment_service with minimal dependencies. """
+""" Module for spark and os environment for cdc_tech_environment_service with minimal dependencies. """
 
 import sys  # don't remove required for error handling
 import os
 
 import io
 
 # library management
@@ -19,29 +19,38 @@
 # azcopy and adls
 from azure.identity import DefaultAzureCredential, ManagedIdentityCredential, ClientSecretCredential
 from azure.storage.filedatalake import DataLakeServiceClient, DataLakeDirectoryClient
 from azure.keyvault.secrets import SecretClient
 
 # spark
 from pyspark.sql import (SparkSession, DataFrame)
-from pyspark.sql.functions import (coalesce, col, concat_ws, lit, udf, regexp_replace)
-from pyspark.sql.types import (IntegerType, LongType, StringType, StructField, StructType)
+from pyspark.sql.functions import (
+    coalesce, col, concat_ws, lit, udf, regexp_replace)
+from pyspark.sql.types import (
+    IntegerType, LongType, StringType, StructField, StructType)
 
 #  data
+os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
     # import pyspark.pandas  as pd
     # bug - pyspark version will not read local files in the repo
     import pyspark.pandas as pd
 else:
     import pandas as pd
 
 
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
 class EnvironmentSpark:
     """ EnvironmentSpark class with minimal dependencies for the developer service.
     - This class is used to configure the Spark environment.
     """
 
     @staticmethod
     def configure_spark_local(
@@ -55,15 +64,15 @@
             spark_home_path (str, optional): path for spark home. Defaults to "".
             pyspark_python_path (str, optional): path for pyspark python. Defaults to "".
             java_home_path (str, optional): path for java home. Defaults to "".
 
         Returns:
             str: spark_home_path
         """
-
+        os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
         os.environ["SPARK_HOME"] = spark_home_path
         os.environ["JAVA_HOME"] = java_home_path
 
         # Add the PySpark directories to the Python path:
         sys.path.insert(1, os.path.join(java_home_path, "/bin"))
         sys.path.insert(1, os.path.join(spark_home_path, "python"))
         sys.path.insert(1, os.path.join(spark_home_path, "python", "pyspark"))
@@ -101,15 +110,16 @@
         row_user_name = df_user_name.first()
         if row_user_name is not None:
             username = row_user_name["current_user"]
         else:
             username = "dataframe is empty error"
         repo = "pade"
         sys_path = str(sys.path)
-        root_path = os.path.abspath(f"/Workspace/Repos/{username}/{repo}/pade_python")
+        root_path = os.path.abspath(
+            f"/Workspace/Repos/{username}/{repo}/pade_python")
         if root_path not in sys_path:
             sys.path.append(root_path)
 
         return root_path
 
     @staticmethod
     def get_spark_home_path_local(spark_home_path: str) -> str:
```

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.9/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202307.0.2/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Module for rep_core for it_admin_service that handles repository and cluster functions with minimal dependencies. """
+""" Module for rep_core for it_cdc_admin_service that handles repository and cluster functions with minimal dependencies. """
 
 import os
 import sys  # don't remove required for error handling
 
 import traceback  # don't remove required for error handling
 from importlib import util  # library management
 
@@ -20,14 +20,20 @@
 
 # http
 from urllib.parse import urlparse
 
 # certs
 import certifi
 
+# Get the currently running file name
+NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
+# Get the parent folder name of the running file
+SERVICE_NAME = os.path.basename(__file__)
+
+
 class RepoCore:
 
     @staticmethod
     def describe_cluster_library_state(library_object, cluster_id, status):
         """Converts cluster library status response to a verbose message"""
 
         lib_title = library_object.title()
@@ -78,15 +84,15 @@
         return destination_path
 
     @staticmethod
     def call_databricks_install_api(config, end_point, body, method="GET", verbose=True):
         """Execute HTTP request against Databricks REST API 2.0"""
 
         token = config['access_token']
-        domain = config["pade_databricks_instance_id"]
+        domain = config.get("pade_databricks_instance_id")
         base_url = f"https://{domain}/api/"
         cluster_id = config['pade_databricks_cluster']
 
         bearer = "Bearer " + token
         headers = {"Authorization": bearer, "Content-Type": "application/json"}
 
         method = method.upper()
@@ -110,15 +116,16 @@
 
             if response_install.status_code == 200:
                 statuses = response_install.json()
                 if "library_statuses" in statuses:
                     for status in statuses["library_statuses"]:
                         if status["library"] == "TODO":
                             if verbose is True:
-                                msg = cls.describe_cluster_library_state("library_source", cluster_id, status["status"])
+                                msg = cls.describe_cluster_library_state(
+                                    "library_source", cluster_id, status["status"])
                                 response_install_text_message += msg
                             else:
                                 response_install_text_message += status["status"]
                         else:
                             response_install_text_message += str(status)
 
         except Exception as exception_check:
@@ -138,26 +145,29 @@
     def get_cluster_library_status(cls, config, library_source, properties, verbose=True):
         """Gets the current library status """
 
         library_source = library_source.lower()
 
         # Validate input
         error_message_1 = "Error: Invalid library source specified. Valid sources are: jar, egg, whl, pypi, maven, cran"
-        assert library_source in ("jar", "egg", "whl", "pypi", "maven", "cran"), error_message_1
+        assert library_source in (
+            "jar", "egg", "whl", "pypi", "maven", "cran"), error_message_1
         assert properties is not None, "Error: Empty properties provided"
 
         # Get the cluster ID from the Spark environment
         cluster_id = config['pade_databricks_cluster']
 
         # Set default result to not installed
-        result = cls.describe_cluster_library_state(library_source, cluster_id, "NOT_INSTALLED")
+        result = cls.describe_cluster_library_state(
+            library_source, cluster_id, "NOT_INSTALLED")
 
         # Execute REST API request to get the library statuses
         endpoint = f"2.0/libraries/cluster-status?cluster_id={cluster_id}"
-        result = cls.call_databricks_install_api(config, endpoint, None, "GET", verbose)
+        result = cls.call_databricks_install_api(
+            config, endpoint, None, "GET", verbose)
 
         return result
 
     @classmethod
     def install_cluster_library(cls, config, library_source, content_data):
         """
         Installs a cluster library given correct source and properties are provided
@@ -165,50 +175,56 @@
         """
 
         library_file = content_data
         library_source = library_source.lower()
 
         # Validate input
         err_msg = "Error: Invalid library source specified. Valid sources are: jar, egg, whl, pypi, maven, cran"
-        assert library_source in ("jar", "egg", "whl", "pypi", "maven", "cran"), err_msg
+        assert library_source in (
+            "jar", "egg", "whl", "pypi", "maven", "cran"), err_msg
         assert library_file is not None, "Error: Empty library_file provided"
 
         # Get the cluster ID from the Spark environment
         cluster_id = config['pade_databricks_cluster']
 
-        status = cls.get_cluster_library_status(config, library_source, library_file, False).upper()
+        status = cls.get_cluster_library_status(
+            config, library_source, library_file, False).upper()
         if status != "INSTALLED":
             # Create the HTTP request body based on the cluster ID, library source and properties
             libraries = f'"{library_source}": "{library_file}"'
-            json_string = '{"cluster_id": "' + cluster_id + '", "libraries":[{' + libraries + '}]}'
+            json_string = '{"cluster_id": "' + cluster_id + \
+                '", "libraries":[{' + libraries + '}]}'
             print(f"json_string:{json_string}")
             body = json.loads(json_string)
             # Execute REST API request to install the library
-            result = cls.call_databricks_install_api(config, "2.0/libraries/install", body, "POST")
+            result = cls.call_databricks_install_api(
+                config, "2.0/libraries/install", body, "POST")
             if result == '- response : success  -':
                 print("Installation started . . .")
             else:
                 print(result)
         else:
-            print(cls.describe_cluster_library_state(library_source, cluster_id, status))
+            print(cls.describe_cluster_library_state(
+                library_source, cluster_id, status))
 
         return status
 
     @staticmethod
     def write_issues(r, csvout):
         "output a list of issues to csv"
         if not r.status_code == 200:
             raise Exception(r.status_code)
         for issue in r.json():
-            Tag=[]
+            Tag = []
             labels = issue['labels']
             for label in labels:
                 Tag.append(label['name'])
 
-            csvout.writerow([issue['number'], issue['title'].encode('utf-8'),Tag,issue['state'] ,issue['created_at'], issue['closed_at']])
+            csvout.writerow([issue['number'], issue['title'].encode(
+                'utf-8'), Tag, issue['state'], issue['created_at'], issue['closed_at']])
 
     @classmethod
     def import_issues_to_csv_from_github(cls, config: dict) -> str:
         """Uses basic authentication (Github username + password) to retrieve Issues
         from a repository that username has access to and writes the issues to a csv file.
         Supports Github API v3.
 
@@ -222,37 +238,38 @@
         GITHUB_USER = 'USER NAME'
         GITHUB_PASSWORD = 'PASSWORD'
         REPO = 'REPO NAME'  # format is username/repo
         ISSUES_FOR_REPO_URL = 'https://api.github.com/repos/%s/issues' % REPO
         AUTH = (GITHUB_USER, GITHUB_PASSWORD)
         arg = "?state=all"
 
-        response = requests.get(ISSUES_FOR_REPO_URL+arg)
+        response = requests.get(ISSUES_FOR_REPO_URL + arg)
         file_csv = '%s-issues.csv' % (REPO.replace('/', '-'))
         file_csv_o = open(file_csv, 'wb')
         out_csv = csv.writer(file_csv_o)
-        out_csv.writerow(('id', 'Title', 'Tag', 'State', 'Open Date', 'Close Date'))
+        out_csv.writerow(('id', 'Title', 'Tag', 'State',
+                         'Open Date', 'Close Date'))
 
         cls.write_issues(r, out_csv)
 
         # more pages? examine the 'link' header returned
         if 'link' in response.headers:
             pages = dict(
-                [(rel[6:-1], url[url.index('<')+1:-1]) for url, rel in
+                [(rel[6:-1], url[url.index('<') + 1:-1]) for url, rel in
                     [link.split(';') for link in
                         response.headers['link'].split(',')]])
 
             while 'last' in pages and 'next' in pages:
                 response = requests.get(pages['next'], auth=AUTH)
                 cls.write_issues(response, out_csv)
                 if pages['next'] == pages['last']:
                     break
                 pages = dict(
-                [(rel[6:-1], url[url.index('<')+1:-1]) for url, rel in
-                    [link.split(';') for link in
+                    [(rel[6:-1], url[url.index('<') + 1:-1]) for url, rel in
+                     [link.split(';') for link in
                         response.headers['link'].split(',')]])
 
         file_csv_o.close()
 
         return "Success"
 
     @staticmethod
@@ -285,15 +302,16 @@
 
         file_path = file_path.replace("/Workspace", "")
 
         print(f"content_type:{content_type}")
         print(f"url:{url}")
 
         if content_type == "bytes":
-            headers_import = {"Authorization": bearer} # , "Content-Type": "multipart/form-data"
+            # , "Content-Type": "multipart/form-data"
+            headers_import = {"Authorization": bearer}
             headers_redacted = str(headers_import).replace(
                 bearer, "[bearer REDACTED]"
             )
             try:
                 content_data.decode("UTF-8")
             except (UnicodeDecodeError, AttributeError):
                 content_data = bytes(content_data, 'utf-8')
@@ -314,37 +332,40 @@
             # --form path=/Users/me@example.com/MyFolder/MyNotebook \
             # --form content=@myCode.py.zip
 
             response_binary = PADEObject()
             response_binary.text = 'Empty. Unable to retrieve post response'
             # data=multipart_form_data,
             try:
-                response_binary = requests.post(url=url, files=files, data=multipart_form_data, headers=headers_import)
+                response_binary = requests.post(
+                    url=url, files=files, data=multipart_form_data, headers=headers_import)
                 print(f"post : success : {url} ")
                 response_binary_text = json.loads(response_binary.text)
                 response_binary_text = json.dumps(response_binary_text.json())
                 print(f"parse : success : {url}")
                 response_binary_text_message = "Received Cluster API Response : "
                 response_binary_text_message += f"{response_binary_text} when posting to : {url}  "
                 response_binary_text_message += f"to import file: {file_path}"
             except Exception as exception_check:
                 html_filter = HTMLFilter()
                 html_filter.feed(response_binary.text)
                 response_install_text_message = html_filter.text
                 print(f"url : error - {str(exception_check)}")
                 print("Error IMPORT-FILE-RESPONSE")
                 print(f"response error code:{str(response_binary)}")
-                print(f"response error message:{response_install_text_message}")
+                print(
+                    f"response error message:{response_install_text_message}")
         elif content_type == "text":
 
             # text
             # curl -n -X POST https://<databricks-instance>/api/2.0/workspace/import
             # -F path="/Users/user@example.com/new-notebook" -F format=SOURCE -F language=SCALA -F overwrite=true -F content=@notebook.scala
 
-            headers_import = {"Authorization": bearer, "Accept": "application/json"}
+            headers_import = {"Authorization": bearer,
+                              "Accept": "application/json"}
             headers_redacted = str(headers_import).replace(
                 bearer, "[bearer REDACTED]"
             )
 
             print(f"headers:{headers_redacted}")
             print(f"json:{str(content_data[ 0 : 100 ])}...")
 
@@ -384,46 +405,52 @@
         verify = certifi.where()
 
         print(f"------- Fetch {base_path}  -------")
         print(f"url:{str(url)}")
         headers_redacted = str(headers).replace(token, "[bearer REDACTED]")
         print(f"headers:{headers_redacted}")
 
-        response = requests.get(url=url, headers=headers, json=json_text, verify=verify)
+        response = requests.get(url=url, headers=headers,
+                                json=json_text, verify=verify)
         data = None
 
         try:
             data = response.json()
             response_text_fetch = f"Suceess: Received list_repos with length : {len(str(data))}"
-            response_text_fetch = response_text_fetch + f" when posting to : {url}"
+            response_text_fetch = response_text_fetch + \
+                f" when posting to : {url}"
             print(f"{response_text_fetch}")
             print(f"listed files for : {base_path}")
             print(str(data))
             lst = data["objects"]
-            repos = list(filter(lambda itm: str(Path(itm['path']).stem).upper() == repository_name.upper(), lst))
+            repos = list(filter(lambda itm: str(
+                Path(itm['path']).stem).upper() == repository_name.upper(), lst))
 
             if repos[0] is None:
                 repo_data = "Error Repo Not found"
             else:
                 repo_object = repos[0]
                 repo_id = repo_object['object_id']
                 url = f"{api_url}/api/2.0/repos/{repo_id}"
                 print(f"repo_id:{repo_id} branch_name:{branch_name}")
-                repo_data = requests.patch(url=url, headers=headers, verify=verify, json={'branch': branch_name}).json()
+                repo_data = requests.patch(url=url, headers=headers, verify=verify, json={
+                                           'branch': branch_name}).json()
         except Exception as exception_object:
             filter_object = HTMLFilter()
             filter_object.feed(response.text)
             response_text = filter_object.text
             repo_data = f"Response : error - {exception_object}: {response_text}"
 
         print(repo_data)
 
         return repo_data
 
+
 class PADEObject(object):
     pass
 
+
 class HTMLFilter(HTMLParser):
     text = ""
 
     def handle_data(self, data):
         self.text += data
```

### Comparing `data_ecosystem_services-202306.0.9/license.md` & `data_ecosystem_services-202307.0.2/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.9/pyproject.toml` & `data_ecosystem_services-202307.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202306.0.9"
+version="202307.0.2"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
@@ -41,15 +41,14 @@
             "pyproject.toml"]
 packages = [{include = "data_ecosystem_services"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.1.2"
-python-dotenv = "^0.20.0"
 adal = "^1.2.7"
 azure-common = "^1.1.28"
 azure-keyvault-secrets = "^4.5.0"
 azure-identity = "^1.10.0"
 azure-storage-file-datalake = "^12.8.0"
 openpyxl = "^3.0.4"
 numpy = "^1.23.0"
@@ -73,45 +72,64 @@
 sphinxcontrib-mermaid = "^0.7.1"
 sphinx-autoapi = "^2.0.0"
 sphinx-sql = "^1.3.2"
 docutils = "0.17.1"
 sphinx-autodoc-typehints = "^1.19.5"
 pyarrow = "^10.0.1"
 rsconnect-jupyter = "^1.6.0"
-pytest-cov = "^4.0.0"
 sphinx-rtd-theme = "^1.1.1"
 chardet = "^5.0.0"
 nbconvert = "^6.5.1"
 pip-system-certs = "^4.0"
 style = "^1.1.6"
 azure-keyvault = "^4.2.0"
 azure-mgmt-monitor = "^5.0.1"
 jinja2 = "^3.1.2"
 opentelemetry-sdk = "^1.17.0"
 azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
 azure-storage-queue = "^12.6.0"
+python-dotenv = "^1.0.0"
+azure-mgmt-resource = "^23.0.1"
+tryceratops = "^2.3.2"
+certifi = "2023.5.7"
+opentelemetry-instrumentation-flask = "^0.39b0"
+flask = "^2.3.2"
+delta-spark = "2.4.0"
+findspark = "^2.0.1"
+pandas = "^2.0.2"
+pyspark = "^3.4.1"
+jsondiff = "^2.0.0"
+opentelemetry-instrumentation = "^0.39b0"
+wrapt = "^1.15.0"
+xlsxwriter = "^3.1.2"
+retrying = "^1.3.4"
+
+ 
+[tool.poetry.group.unix.dependencies]
+xattr = {version = "^0.10.1", markers = "sys_platform != 'win32'"}
+
+[tool.poetry.group.windows.dependencies]
+pywin32 = { version = "*", markers = "sys_platform == 'win32'" }
 
-[tool.poetry.dev-dependencies]
-pandas = "^1.4.2"
+[tool.poetry.group.dev.dependencies]
 wheel = "^0.38.1"
 check-wheel-contents = "^0.3.4"
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.6.22"
 black = "^22.3.0"
 commitizen = "^2.28.0"
-pathlib = "^1.0.1"
 python-decouple = "^3.6"
-delta-spark = "2.1.0"
-findspark = "^2.0.1"
+pathlib = "^1.0.1"
 
 [tool.pytest.ini_options]
 minversion="6.0"
-addopts="-ra -q --cov --cov-report html --cov-report term-missing --cov-fail-under 15"
+ 
 testpaths=[
-    "tests"
+    "tests",
+    "pade_python/tests"
 ]
 
 [tool.semantic_release]
 version_variable = [ "pyproject.toml:version"]
 version_toml = [
     "pyproject.toml:tool.poetry.version"
 ]
```

### Comparing `data_ecosystem_services-202306.0.9/readme.md` & `data_ecosystem_services-202307.0.2/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PADE-Python Project Documentation
 
 - Point of contact: [John Bowyer](mailto:zfi4@cdc.gov)
 - Organizational unit: OCIO
 - Related projects: EDC
 - Related investments:  Pending Public Release
 - Governance status: Pending Public Release
-- Program official:  [Erik Knudsen](mailto:egk1@cdc.gov)
+- Program official:  [Erik Knudsen](mailto:knu1@cdc.gov)
 
 ## Getting Started
 
 ## Set up Local development environment for Python - with remote spark
 
 ### Check if Python is installed
 
@@ -231,14 +231,24 @@
 
 For local
 
 ```sh
 rm -rf OCIO_PADE_DEV
 ```
 
+## Run Unit Test Coverage Report
+
+### Run Unit Test Coverage Report on Ubuntu or WSL (Primary)
+
+Run the following command
+
+```sh
+pytest --cov-report html tests/
+```
+
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
 
 Reference 1: [Install Docker Engine without Docker Desktop](https://dev.to/bowmanjd/install-docker-on-windows-wsl-without-docker-desktop-34m9)
 Reference 2: [Install Docker for WSL](https://docs.docker.com/engine/install/ubuntu/)
```

### Comparing `data_ecosystem_services-202306.0.9/PKG-INFO` & `data_ecosystem_services-202307.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202306.0.9
+Version: 202307.0.2
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,63 +20,76 @@
 Requires-Dist: Sphinx (>=5.2.1,<6.0.0)
 Requires-Dist: adal (>=1.2.7,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.5.0,<5.0.0)
 Requires-Dist: azure-mgmt-monitor (>=5.0.1,<6.0.0)
+Requires-Dist: azure-mgmt-resource (>=23.0.1,<24.0.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
 Requires-Dist: azure-storage-file-datalake (>=12.8.0,<13.0.0)
 Requires-Dist: azure-storage-queue (>=12.6.0,<13.0.0)
 Requires-Dist: boto3 (==1.21.18)
 Requires-Dist: botocore (==1.24.18)
+Requires-Dist: certifi (==2023.5.7)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
+Requires-Dist: delta-spark (==2.4.0)
 Requires-Dist: docutils (==0.17.1)
+Requires-Dist: findspark (>=2.0.1,<3.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jsondiff (>=2.0.0,<3.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: myst-parser (>=0.18.0,<0.19.0)
 Requires-Dist: nbconvert (>=6.5.1,<7.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: opencensus (>=0.11.0,<0.12.0)
 Requires-Dist: opencensus-ext-azure (>=1.1.7,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.4,<4.0.0)
+Requires-Dist: opentelemetry-instrumentation (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-instrumentation-flask (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pip-system-certs (>=4.0,<5.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyreadstat (>=1.1.9,<2.0.0)
+Requires-Dist: pyspark (>=3.4.1,<4.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.31.0)
+Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Requires-Dist: rsconnect-jupyter (>=1.6.0,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.5,<2.0.0)
 Requires-Dist: sphinx-markdown-builder (>=0.5.5,<0.6.0)
 Requires-Dist: sphinx-markdown-tables (>=0.0.17,<0.0.18)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0)
 Requires-Dist: sphinx-sql (>=1.3.2,<2.0.0)
 Requires-Dist: sphinxcontrib-mermaid (>=0.7.1,<0.8.0)
 Requires-Dist: style (>=1.1.6,<2.0.0)
 Requires-Dist: testresources (>=2.0.1,<3.0.0)
+Requires-Dist: tryceratops (>=2.3.2,<3.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
+Requires-Dist: xlsxwriter (>=3.1.2,<4.0.0)
 Project-URL: Repository, https://github.com/cdcent/data-ecosystem-services
 Description-Content-Type: text/markdown
 
 # PADE-Python Project Documentation
 
 - Point of contact: [John Bowyer](mailto:zfi4@cdc.gov)
 - Organizational unit: OCIO
 - Related projects: EDC
 - Related investments:  Pending Public Release
 - Governance status: Pending Public Release
-- Program official:  [Erik Knudsen](mailto:egk1@cdc.gov)
+- Program official:  [Erik Knudsen](mailto:knu1@cdc.gov)
 
 ## Getting Started
 
 ## Set up Local development environment for Python - with remote spark
 
 ### Check if Python is installed
 
@@ -298,14 +311,24 @@
 
 For local
 
 ```sh
 rm -rf OCIO_PADE_DEV
 ```
 
+## Run Unit Test Coverage Report
+
+### Run Unit Test Coverage Report on Ubuntu or WSL (Primary)
+
+Run the following command
+
+```sh
+pytest --cov-report html tests/
+```
+
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
 
 Reference 1: [Install Docker Engine without Docker Desktop](https://dev.to/bowmanjd/install-docker-on-windows-wsl-without-docker-desktop-34m9)
 Reference 2: [Install Docker for WSL](https://docs.docker.com/engine/install/ubuntu/)
```

