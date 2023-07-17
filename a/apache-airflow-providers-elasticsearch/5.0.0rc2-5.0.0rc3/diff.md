# Comparing `tmp/apache-airflow-providers-elasticsearch-5.0.0rc2.tar.gz` & `tmp/apache-airflow-providers-elasticsearch-5.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-elasticsearch-5.0.0rc2.tar", last modified: Thu Jul  6 04:50:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-elasticsearch-5.0.0rc3.tar", last modified: Mon Jul 17 05:26:53 2023, max compression
```

## Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2.tar` & `apache-airflow-providers-elasticsearch-5.0.0rc3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.082125 apache-airflow-providers-elasticsearch-5.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5739 2023-07-06 04:50:43.082798 apache-airflow-providers-elasticsearch-5.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4046 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.003037 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.004258 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.038172 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 18:50:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.044001 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6474 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.054490 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)    19313 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.079094 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5739 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      868 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-06 04:50:43.084834 apache-airflow-providers-elasticsearch-5.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.124954 apache-airflow-providers-elasticsearch-5.0.0rc3/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-17 05:26:53.125556 apache-airflow-providers-elasticsearch-5.0.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4046 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.037204 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.038807 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.073832 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-16 17:28:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.079386 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2023-07-16 17:25:26.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/hooks/elasticsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.093150 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/es_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-07-16 17:25:26.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/es_response.py
+-rw-r--r--   0 root         (0) root         (0)    21810 2023-07-16 17:25:26.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/es_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:26:53.121693 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-17 05:26:53.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 05:26:52.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5429 2023-07-16 17:25:26.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-17 05:26:53.127613 apache-airflow-providers-elasticsearch-5.0.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-07-17 05:26:51.000000 apache-airflow-providers-elasticsearch-5.0.0rc3/setup.py
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/LICENSE` & `apache-airflow-providers-elasticsearch-5.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/MANIFEST.in` & `apache-airflow-providers-elasticsearch-5.0.0rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/PKG-INFO` & `apache-airflow-providers-elasticsearch-5.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 5.0.0rc2
+Version: 5.0.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc2``
+Release: ``5.0.0rc3``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/README.rst` & `apache-airflow-providers-elasticsearch-5.0.0rc3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc2``
+Release: ``5.0.0rc3``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/get_provider_info.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/hooks/elasticsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         return uri
 
 
 class ElasticsearchHook(ElasticsearchSQLHook):
     """
     This class is deprecated and was renamed to ElasticsearchSQLHook.
 
-    Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.
+    Please use :class:`airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.
     """
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.""",
             AirflowProviderDeprecationWarning,
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/es_json_formatter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/airflow/providers/elasticsearch/log/es_task_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 import logging
 import sys
 import warnings
 from collections import defaultdict
 from datetime import datetime
 from operator import attrgetter
 from time import time
-from typing import TYPE_CHECKING, List, Tuple
+from typing import TYPE_CHECKING, Any, Callable, List, Tuple
 from urllib.parse import quote
 
 # Using `from elasticsearch import *` would break elasticsearch mocking used in unit test.
 import elasticsearch
 import pendulum
 from elasticsearch.exceptions import ElasticsearchException, NotFoundError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models.dagrun import DagRun
 from airflow.models.taskinstance import TaskInstance
 from airflow.providers.elasticsearch.log.es_json_formatter import ElasticsearchJSONFormatter
+from airflow.providers.elasticsearch.log.es_response import ElasticSearchResponse, Hit
 from airflow.utils import timezone
 from airflow.utils.log.file_task_handler import FileTaskHandler
 from airflow.utils.log.logging_mixin import ExternalLoggingMixin, LoggingMixin
 from airflow.utils.session import create_session
 
 LOG_LINE_DEFAULTS = {"exc_text": "", "stack_info": ""}
 # Elasticsearch hosted log type
@@ -48,42 +49,14 @@
 
 # Compatibility: Airflow 2.3.3 and up uses this method, which accesses the
 # LogTemplate model to record the log ID template used. If this function does
 # not exist, the task handler should use the log_id_template attribute instead.
 USE_PER_RUN_LOG_ID = hasattr(DagRun, "get_log_template")
 
 
-class Log:
-    """wrapper class to mimic the attributes in Search class used in elasticsearch_dsl.Search."""
-
-    def __init__(self, offset):
-        self.offset = offset
-
-
-class ElasticSearchResponse:
-    """wrapper class to mimic the Search class used in elasticsearch_dsl.Search."""
-
-    def __init__(self, **kwargs):
-        # Store all provided keyword arguments as attributes of this object
-        for key, value in kwargs.items():
-            if key == "log":
-                setattr(self, key, Log(**value))
-            else:
-                setattr(self, key, value)
-
-    def to_dict(self):
-        result = {}
-        for key in self.__dict__.keys():
-            if key == "log":
-                result[key] = self.__dict__[key].__dict__
-            else:
-                result[key] = self.__dict__[key]
-        return result
-
-
 class ElasticsearchTaskHandler(FileTaskHandler, ExternalLoggingMixin, LoggingMixin):
     """
     ElasticsearchTaskHandler is a python log handler that reads logs from Elasticsearch.
 
     Note that Airflow does not handle the indexing of logs into Elasticsearch. Instead,
     Airflow flushes logs into local files. Additional software setup is required to index
     the logs into Elasticsearch, such as using Filebeat and Logstash.
@@ -146,14 +119,16 @@
         self.host_field = host_field
         self.offset_field = offset_field
         self.index_patterns = index_patterns
         self.context_set = False
 
         self.formatter: logging.Formatter
         self.handler: logging.FileHandler | logging.StreamHandler  # type: ignore[assignment]
+        self._doc_type_map: dict[Any, Any] = {}
+        self._doc_type: list[Any] = []
 
     def _render_log_id(self, ti: TaskInstance, try_number: int) -> str:
         with create_session() as session:
             dag_run = ti.get_dagrun(session=session)
             if USE_PER_RUN_LOG_ID:
                 log_id_template = dag_run.get_log_template(session=session).elasticsearch_id
             else:
@@ -295,59 +270,51 @@
                 )
             except Exception:
                 pass
 
         # Just a safe-guard to preserve backwards-compatibility
         return log_line.message
 
-    def es_read(self, log_id: str, offset: str, metadata: dict) -> list:
+    def es_read(self, log_id: str, offset: int | str, metadata: dict) -> list | ElasticSearchResponse:
         """
         Return the logs matching log_id in Elasticsearch and next offset or ''.
 
         :param log_id: the log_id of the log to read.
         :param offset: the offset start to read log from.
         :param metadata: log metadata, used for steaming log download.
         """
-        # Offset is the unique key for sorting logs given log_id.
-        query = {
+        query: dict[Any, Any] = {
             "query": {
                 "bool": {
-                    "must": [
-                        {"match_phrase": {"log_id": log_id}},
-                        {"range": {self.offset_field: {"gt": int(offset)}}},
-                    ]
+                    "filter": [{"range": {self.offset_field: {"gt": int(offset)}}}],
+                    "must": [{"match_phrase": {"log_id": log_id}}],
                 }
-            },
-            "sort": [{self.offset_field: {"order": "asc"}}],
+            }
         }
 
         try:
             max_log_line = self.client.count(index=self.index_patterns, body=query)["count"]
         except NotFoundError as e:
             self.log.exception("The target index pattern %s does not exist", self.index_patterns)
             raise e
         except ElasticsearchException as e:
             self.log.exception("Could not get current log size with log_id: %s", log_id)
             raise e
 
-        logs = []
+        logs: list[Any] | ElasticSearchResponse = []
         if max_log_line != 0:
             try:
+                query.update({"sort": [self.offset_field]})
                 res = self.client.search(
                     index=self.index_patterns,
                     body=query,
                     size=self.MAX_LINE_PER_PAGE,
                     from_=self.MAX_LINE_PER_PAGE * self.PAGE,
                 )
-                logs = [
-                    ElasticSearchResponse(
-                        **unwrap_response(response),
-                    )
-                    for response in res["hits"]["hits"]
-                ]
+                logs = ElasticSearchResponse(self, res)
             except elasticsearch.exceptions.ElasticsearchException:
                 self.log.exception("Could not read log with log_id: %s", log_id)
 
         return logs
 
     def emit(self, record):
         if self.handler:
@@ -444,51 +411,114 @@
         return scheme + self.frontend.format(log_id=quote(log_id))
 
     @property
     def supports_external_link(self) -> bool:
         """Whether we can support external links."""
         return bool(self.frontend)
 
+    def _resolve_nested(self, hit: dict[Any, Any], parent_class=None) -> type[Hit]:
+        """
+        Resolves nested hits from Elasticsearch by iteratively navigating the `_nested` field.
+        The result is used to fetch the appropriate document class to handle the hit.
+
+        This method can be used with nested Elasticsearch fields which are structured
+        as dictionaries with "field" and "_nested" keys.
+        """
+        doc_class = Hit
+
+        nested_path: list[str] = []
+        nesting = hit["_nested"]
+        while nesting and "field" in nesting:
+            nested_path.append(nesting["field"])
+            nesting = nesting.get("_nested")
+        nested_path_str = ".".join(nested_path)
+
+        if hasattr(parent_class, "_index"):
+            nested_field = parent_class._index.resolve_field(nested_path_str)
+
+        if nested_field is not None:
+            return nested_field._doc_class
+
+        return doc_class
+
+    def _get_result(self, hit: dict[Any, Any], parent_class=None) -> Hit:
+        """
+        This method processes a hit (i.e., a result) from an Elasticsearch response and transforms it into an
+        appropriate class instance.
+
+        The transformation depends on the contents of the hit. If the document in hit contains a nested field,
+        the '_resolve_nested' method is used to determine the appropriate class (based on the nested path).
+        If the hit has a document type that is present in the '_doc_type_map', the corresponding class is
+        used. If not, the method iterates over the '_doc_type' classes and uses the first one whose '_matches'
+        method returns True for the hit.
+
+        If the hit contains any 'inner_hits', these are also processed into 'ElasticSearchResponse' instances
+        using the determined class.
+
+        Finally, the transformed hit is returned. If the determined class has a 'from_es' method, this is
+        used to transform the hit
+
+        An example of the hit argument:
+
+        {'_id': 'jdeZT4kBjAZqZnexVUxk',
+         '_index': '.ds-filebeat-8.8.2-2023.07.09-000001',
+         '_score': 2.482621,
+         '_source': {'@timestamp': '2023-07-13T14:13:15.140Z',
+                     'asctime': '2023-07-09T07:47:43.907+0000',
+                     'container': {'id': 'airflow'},
+                     'dag_id': 'example_bash_operator',
+                     'ecs': {'version': '8.0.0'},
+                     'execution_date': '2023_07_09T07_47_32_000000',
+                     'filename': 'taskinstance.py',
+                     'input': {'type': 'log'},
+                     'levelname': 'INFO',
+                     'lineno': 1144,
+                     'log': {'file': {'path': "/opt/airflow/Documents/GitHub/airflow/logs/
+                     dag_id=example_bash_operator'/run_id=owen_run_run/
+                     task_id=run_after_loop/attempt=1.log"},
+                             'offset': 0},
+                     'log.offset': 1688888863907337472,
+                     'log_id': 'example_bash_operator-run_after_loop-owen_run_run--1-1',
+                     'message': 'Dependencies all met for dep_context=non-requeueable '
+                                'deps ti=<TaskInstance: '
+                                'example_bash_operator.run_after_loop owen_run_run '
+                                '[queued]>',
+                     'task_id': 'run_after_loop',
+                     'try_number': '1'},
+         '_type': '_doc'}
+        """
+        doc_class = Hit
+        dt = hit.get("_type")
+
+        if "_nested" in hit:
+            doc_class = self._resolve_nested(hit, parent_class)
+
+        elif dt in self._doc_type_map:
+            doc_class = self._doc_type_map[dt]
+
+        else:
+            for doc_type in self._doc_type:
+                if hasattr(doc_type, "_matches") and doc_type._matches(hit):
+                    doc_class = doc_type
+                    break
+
+        for t in hit.get("inner_hits", ()):
+            hit["inner_hits"][t] = ElasticSearchResponse(self, hit["inner_hits"][t], doc_class=doc_class)
+
+        # callback should get the Hit class if "from_es" is not defined
+        callback: type[Hit] | Callable[..., Any] = getattr(doc_class, "from_es", doc_class)
+        return callback(hit)
+
 
 def getattr_nested(obj, item, default):
     """
     Get item from obj but return default if not found.
 
     E.g. calling ``getattr_nested(a, 'b.c', "NA")`` will return
     ``a.b.c`` if such a value exists, and "NA" otherwise.
 
     :meta private:
     """
     try:
         return attrgetter(item)(obj)
     except AttributeError:
         return default
-
-
-def unwrap_response(res):
-    source = res["_source"]
-    transformed = {
-        "log_id": source.get("log_id"),
-        "message": source.get("message"),
-        "meta": {
-            "id": res.get("_id"),
-            "index": res.get("_index"),
-            "version": res.get("_version"),
-            "headers": res.get("_headers"),
-        },
-    }
-    if "offset" in source:
-        transformed["offset"] = source["offset"]
-    if "asctime" in source:
-        transformed["asctime"] = source["asctime"]
-    if "filename" in source:
-        transformed["filename"] = source["filename"]
-    if "host" in source:
-        transformed["host"] = source["host"]
-    if "levelname" in source:
-        transformed["levelname"] = source["levelname"]
-    if "lineno" in source:
-        transformed["lineno"] = source["lineno"]
-    if "log" in source:
-        transformed["log"] = source["log"]
-
-    return transformed
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO` & `apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 5.0.0rc2
+Version: 5.0.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc2``
+Release: ``5.0.0rc3``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt` & `apache-airflow-providers-elasticsearch-5.0.0rc3/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 airflow/providers/elasticsearch/__init__.py
 airflow/providers/elasticsearch/get_provider_info.py
 airflow/providers/elasticsearch/hooks/__init__.py
 airflow/providers/elasticsearch/hooks/elasticsearch.py
 airflow/providers/elasticsearch/log/__init__.py
 airflow/providers/elasticsearch/log/es_json_formatter.py
+airflow/providers/elasticsearch/log/es_response.py
 airflow/providers/elasticsearch/log/es_task_handler.py
 apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
 apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
 apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
 apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
 apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
 apache_airflow_providers_elasticsearch.egg-info/requires.txt
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/pyproject.toml` & `apache-airflow-providers-elasticsearch-5.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/setup.cfg` & `apache-airflow-providers-elasticsearch-5.0.0rc3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.elasticsearch.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.elasticsearch
 
 [egg_info]
-tag_build = rc2
+tag_build = rc3
 tag_date = 0
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc2/setup.py` & `apache-airflow-providers-elasticsearch-5.0.0rc3/setup.py`

 * *Files identical despite different names*

