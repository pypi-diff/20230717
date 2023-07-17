# Comparing `tmp/marquez-python-0.7.8.tar.gz` & `tmp/marquez-python-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marquez-python-0.7.8.tar", last modified: Tue Oct 13 19:52:20 2020, max compression
+gzip compressed data, was "dist/marquez-python-0.7.9.tar", last modified: Thu Oct 22 16:58:28 2020, max compression
```

## Comparing `marquez-python-0.7.8.tar` & `marquez-python-0.7.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-13 19:52:20.000000 marquez-python-0.7.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1923 2020-10-13 19:52:17.000000 marquez-python-0.7.8/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2020-10-13 19:52:20.000000 marquez-python-0.7.8/PKG-INFO
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-13 19:52:20.000000 marquez-python-0.7.8/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2553 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_airflow_dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_marquez_wo_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_log_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13561 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_marquez_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5393 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_marquez_wo_client_file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6027 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_marquez_wo_client_http.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2020-10-13 19:52:17.000000 marquez-python-0.7.8/tests/test_marquez_wo_client_log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2020-10-13 19:52:20.000000 marquez-python-0.7.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1750 2020-10-13 19:52:17.000000 marquez-python-0.7.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      810 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_python.egg-info/requires.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-13 19:52:20.000000 marquez-python-0.7.8/marquez_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3448 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12507 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/log_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      696 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6566 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/client_wo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1750 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/http_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2051 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2020-10-13 19:52:17.000000 marquez-python-0.7.8/marquez_client/file_backend.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-22 16:58:28.000000 marquez-python-0.7.9/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      840 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_python.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-22 16:58:28.000000 marquez-python-0.7.9/marquez_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      769 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/log_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6566 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/client_wo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      696 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/file_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12547 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2042 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/http_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3562 2020-10-22 16:58:25.000000 marquez-python-0.7.9/marquez_client/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2020-10-22 16:58:28.000000 marquez-python-0.7.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2020-10-22 16:58:28.000000 marquez-python-0.7.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1750 2020-10-22 16:58:25.000000 marquez-python-0.7.9/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1923 2020-10-22 16:58:25.000000 marquez-python-0.7.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-10-22 16:58:28.000000 marquez-python-0.7.9/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_airflow_dag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_wo_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5158 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_wo_client_file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2180 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_wo_client_http.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_log_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16091 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2020-10-22 16:58:25.000000 marquez-python-0.7.9/tests/test_marquez_wo_client_log.py
```

### Comparing `marquez-python-0.7.8/setup.py` & `marquez-python-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/tests/test_airflow_dag.py` & `marquez-python-0.7.9/tests/test_airflow_dag.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,74 +6,66 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import logging
 import logging.config
+import os
 import random
 import unittest
 import uuid
 
-import yaml
-
 from marquez_client import Clients
 from marquez_client.models import (DatasetType, JobType)
-
 from marquez_client.utils import Utils
 
 _NAMESPACE = 'default'
 
 log = logging.getLogger(__name__)
 
 
 class TestAirflowDAG(unittest.TestCase):
     def setUp(self):
         log.debug("TestAirflowDAG.setup(): ")
 
-        with open('tests/logConfig.yaml', 'rt') as file:
-            yamlConfig = yaml.safe_load(file.read())
-            logging.config.dictConfig(yamlConfig)
-            log.info("loaded logConfig.yaml")
-
         os.environ['MARQUEZ_BACKEND'] = 'file'
-
-        self.client = Clients.new_write_only_client()
+        self.client_wo_file = Clients.new_write_only_client()
         log.info("created marquez_client.")
 
     def test_create_dag(self):
         log.debug("TestAirflowDAG::test_create_dag")
 
         for i in range(1000):
             NAMESPACE = "my-namespace"
             OWNER = "me"
             SOURCE = "my-source"
             DATASET = f'my-dataset-{i}'
             PHYSICAL = f'public.my_table-{i}'
             run_id = str(uuid.uuid4())
             JOB = f'my-job-{i%10}'
 
-            self.client.create_namespace(NAMESPACE, OWNER)
-            self.client.create_source(
+            self.client_wo_file.create_namespace(NAMESPACE, OWNER)
+            self.client_wo_file.create_source(
                 SOURCE,
                 'POSTGRESQL',
                 "jdbc:postgresql://localhost:5432/test?user=fred&ssl=true")
-            self.client.create_dataset(
+            self.client_wo_file.create_dataset(
                 NAMESPACE, DATASET, DatasetType.DB_TABLE,
                 PHYSICAL, SOURCE, run_id)
-            self.client.create_job(NAMESPACE, JOB, JobType.BATCH)
-            self.client.create_job_run(NAMESPACE, JOB, run_id,
-                                       mark_as_running=True)
+            self.client_wo_file.create_job(NAMESPACE, JOB, JobType.BATCH)
+            self.client_wo_file.create_job_run(NAMESPACE, JOB, run_id,
+                                               mark_as_running=True)
 
             udiff = (i % 10 - random.randrange(10))
 
             if udiff >= -1 or udiff <= 1:
-                self.client.mark_job_run_as_failed(run_id, Utils.utc_now())
+                self.client_wo_file.mark_job_run_as_failed(
+                    run_id, Utils.utc_now())
             else:
-                self.client.mark_job_run_as_completed(run_id, Utils.utc_now())
+                self.client_wo_file.mark_job_run_as_completed(
+                    run_id, Utils.utc_now())
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `marquez-python-0.7.8/tests/test_marquez_wo_client.py` & `marquez-python-0.7.9/tests/test_marquez_wo_client.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/tests/test_log_backend.py` & `marquez-python-0.7.9/tests/test_log_backend.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/tests/test_marquez_client.py` & `marquez-python-0.7.9/tests/test_marquez_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,40 +5,33 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import logging
+import json
 import logging.config
 import unittest
 import uuid
 
 import mock
-import yaml
 
 import marquez_client
 from marquez_client.models import (DatasetType, JobType, RunState)
 from marquez_client.utils import Utils
 
 _NAMESPACE = "my-namespace"
 log = logging.getLogger(__name__)
 
 
 class TestMarquezClient(unittest.TestCase):
     def setUp(self):
         log.debug("TestMarquezClient.setup(): ")
 
-        with open('tests/logConfig.yaml', 'rt') as file:
-            yamlConfig = yaml.safe_load(file.read())
-            logging.config.dictConfig(yamlConfig)
-            log.info("loaded logConfig.yaml")
-
         self.client = \
             marquez_client.client.MarquezClient("http://localhost:5000")
         log.info("created marquez_client.")
 
     @mock.patch("marquez_client.client.MarquezClient._put")
     def test_create_namespace(self, mock_put):
         owner_name = "me"
@@ -214,15 +207,15 @@
             "name": "public.mytable"
         }
 
         location = "https://github.com/my-jobs/blob/" \
                    "07f3d2dfc8186cadae9146719e70294a4c7a8ee8"
 
         context = {
-            "SQL": "SELECT * FROM public.mytable;"
+            "sql": "SELECT * FROM public.mytable;"
         }
 
         mock_put.return_value = {
             "id": {
                 "namespace": "my-namespace",
                 "name": "my-job"
             },
@@ -242,15 +235,15 @@
                     "namespace": "my-namespace",
                     "name": "public.mytable"
                 }
             ],
             "location": "https://github.com/my-jobs/blob/"
                         "07f3d2dfc8186cadae9146719e70294a4c7a8ee8",
             "context": {
-                "SQL": "SELECT * FROM public.mytable;"
+                "sql": "SELECT * FROM public.mytable;"
             },
             "description": "My first job.",
             "latestRun": None
         }
 
         response = self.client.create_job(
             namespace_name=_NAMESPACE,
@@ -261,14 +254,97 @@
             output_dataset=output_dataset,
             context=context
         )
 
         assert str(response['id']) is not None
         assert str(response['location']) == location
 
+    @mock.patch("marquez_client.client.MarquezClient._put")
+    def test_create_job_with_run_id(self, mock_put):
+        run_id = str(uuid.uuid4())
+        job_name = "my-job"
+        input_dataset = [
+            {
+                "namespace": "my-namespace",
+                "name": "public.mytable"
+            }
+        ]
+        output_dataset = {
+            "namespace": "my-namespace",
+            "name": "public.mytable"
+        }
+
+        location = "https://github.com/my-jobs/blob/" \
+                   "07f3d2dfc8186cadae9146719e70294a4c7a8ee8"
+
+        context = {
+            "sql": "SELECT * FROM public.mytable;"
+        }
+
+        mock_put.return_value = {
+            "id": {
+                "namespace": "my-namespace",
+                "name": "my-job"
+            },
+            "type": "BATCH",
+            "name": "my-job",
+            "createdAt": "2020-08-12T07:30:55.321059Z",
+            "updatedAt": "2020-08-12T07:30:55.333230Z",
+            "namespace": "my-namespace",
+            "inputs": [
+                {
+                    "namespace": "my-namespace",
+                    "name": "public.mytable"
+                }
+            ],
+            "outputs": [
+                {
+                    "namespace": "my-namespace",
+                    "name": "public.mytable"
+                }
+            ],
+            "location": "https://github.com/my-jobs/blob/"
+                        "07f3d2dfc8186cadae9146719e70294a4c7a8ee8",
+            "context": {
+                "sql": "SELECT * FROM public.mytable;"
+            },
+            "description": "My first job.",
+            "latestRun": {
+                "id": run_id,
+                "createdAt": "2020-10-09T19:14:07.846451Z",
+                "updatedAt": "2020-10-09T19:14:07.911627Z",
+                "nominalStartTime": None,
+                "nominalEndTime": None,
+                "state": RunState.RUNNING,
+                "startedAt": "2020-10-09T19:14:07.893074Z",
+                "endedAt": "2020-10-09T19:14:07.911627Z",
+                "durationMs": 18,
+                "args": {}
+            }
+        }
+
+        response = self.client.create_job(
+            namespace_name=_NAMESPACE,
+            job_name=job_name,
+            job_type=JobType.BATCH,
+            location=location,
+            input_dataset=input_dataset,
+            output_dataset=output_dataset,
+            context=context,
+            run_id=run_id
+        )
+
+        mock_put.assert_called_once()
+        assert mock_put.call_args.kwargs.get("payload").get("runId")\
+               == run_id
+
+        assert str(response['inputs']) is not None
+        assert str(response['latestRun']['id']) == run_id
+        assert response['latestRun']['state'] == RunState.RUNNING
+
     @mock.patch("marquez_client.client.MarquezClient._post")
     def test_create_job_run(self, mock_post):
         run_id = str(uuid.uuid4())
         action_at = Utils.utc_now()
 
         job_name = "my-job"
         run_args = {
```

### Comparing `marquez-python-0.7.8/tests/test_marquez_wo_client_file.py` & `marquez-python-0.7.9/tests/test_marquez_wo_client_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
 import logging.config
 import os
 import unittest
 import uuid
 
-import yaml
-
 from marquez_client import Clients
 from marquez_client.models import (DatasetType, JobType)
 from marquez_client.utils import Utils
 
 _NAMESPACE = "my-namespace"
 log = logging.getLogger(__name__)
 
 
 class TestMarquezWriteOnlyClientFile(unittest.TestCase):
     def setUp(self):
         log.debug("MarquezWriteOnlyClient.setup(): ")
 
-        with open('tests/logConfig.yaml', 'rt') as file:
-            yamlConfig = yaml.safe_load(file.read())
-            logging.config.dictConfig(yamlConfig)
-            log.info("loaded logConfig.yaml")
-
         os.environ['MARQUEZ_BACKEND'] = 'file'
         self.client_wo_file = Clients.new_write_only_client()
         log.info("created marquez_client_wo_file.")
 
     def test_create_namespace(self):
         log.info("test_create_namespace()")
```

### Comparing `marquez-python-0.7.8/tests/__init__.py` & `marquez-python-0.7.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/tests/test_marquez_wo_client_http.py` & `marquez-python-0.7.9/tests/test_marquez_wo_client_http.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,40 +6,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
 import logging.config
 import os
 import unittest
 import uuid
 
 import mock
-import yaml
 
 from marquez_client import Clients
 from marquez_client.models import (DatasetType, JobType)
 from marquez_client.utils import Utils
 
 _NAMESPACE = "my-namespace"
 log = logging.getLogger(__name__)
 
 
 class TestMarquezWriteOnlyClientHttp(unittest.TestCase):
     def setUp(self):
         log.debug("MarquezWriteOnlyClient.setup(): ")
 
-        with open('tests/logConfig.yaml', 'rt') as file:
-            yamlConfig = yaml.safe_load(file.read())
-            logging.config.dictConfig(yamlConfig)
-            log.info("loaded logConfig.yaml")
-
         os.environ['MARQUEZ_BACKEND'] = 'http'
         self.client_wo_http = Clients.new_write_only_client()
         log.info("created marquez_client_wo_http.")
 
     @mock.patch("marquez_client.http_backend.HttpBackend.put")
     def test_create_namespace(self, mock_put):
         owner_name = "me"
```

### Comparing `marquez-python-0.7.8/tests/test_marquez_wo_client_log.py` & `marquez-python-0.7.9/tests/test_marquez_wo_client_log.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/README.md` & `marquez-python-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_python.egg-info/SOURCES.txt` & `marquez-python-0.7.9/marquez_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 marquez_python.egg-info/dependency_links.txt
 marquez_python.egg-info/requires.txt
 marquez_python.egg-info/top_level.txt
 tests/__init__.py
 tests/test_airflow_dag.py
 tests/test_log_backend.py
 tests/test_marquez_client.py
+tests/test_marquez_clients.py
 tests/test_marquez_wo_client.py
 tests/test_marquez_wo_client_file.py
 tests/test_marquez_wo_client_http.py
 tests/test_marquez_wo_client_log.py
```

### Comparing `marquez-python-0.7.8/marquez_client/utils.py` & `marquez-python-0.7.9/marquez_client/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,7 +95,11 @@
         return str(generate(datetime.utcnow().replace(tzinfo=pytz.utc),
                             microseconds=True))
 
     @staticmethod
     def get_json(file):
         with open(file) as json_file:
             return json.load(json_file)
+
+    @staticmethod
+    def add_auth_to(headers, api_key):
+        headers['Authorization'] = f"Bearer: {api_key}"
```

### Comparing `marquez-python-0.7.8/marquez_client/constants.py` & `marquez-python-0.7.9/marquez_client/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 # limitations under the License.
 
 DEFAULT_TIMEOUT_MS = 10000
 DEFAULT_NAMESPACE_NAME = 'default'
 DEFAULT_MARQUEZ_BACKEND = 'http'
 DEFAULT_MARQUEZ_URL = 'http://localhost:8080'
 DEFAULT_MARQUEZ_FILE = '/tmp/marquez/client.requests.log'
+
+API_PATH_V1 = '/api/v1'
```

### Comparing `marquez-python-0.7.8/marquez_client/version.py` & `marquez-python-0.7.9/marquez_client/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = '0.7.8'
+VERSION = '0.7.9'
```

### Comparing `marquez-python-0.7.8/marquez_client/client.py` & `marquez-python-0.7.9/marquez_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 import logging
 import os
 
 import requests
 from six.moves.urllib.parse import quote
 
 from marquez_client import errors
-from marquez_client.constants import (DEFAULT_TIMEOUT_MS)
+from marquez_client.constants import (DEFAULT_TIMEOUT_MS, API_PATH_V1)
 from marquez_client.models import (DatasetType, JobType)
 from marquez_client.utils import Utils
 from marquez_client.version import VERSION
 
-_API_PATH = '/api/v1'
 _USER_AGENT = f'marquez-python/{VERSION}'
 _HEADERS = {'User-Agent': _USER_AGENT}
 
 log = logging.getLogger(__name__)
 
 
 # Marquez Client
-class MarquezClient(object):
-    def __init__(self, url, timeout_ms=None):
+class MarquezClient:
+    def __init__(self, url, timeout_ms=None, api_key: str = None):
         self._timeout = Utils.to_seconds(timeout_ms or os.environ.get(
             'MARQUEZ_TIMEOUT_MS', DEFAULT_TIMEOUT_MS)
         )
+        self._api_base = f"{url}{API_PATH_V1}"
 
-        self._api_base = f'{url}{_API_PATH}'
-
-        log.debug(self._api_base)
+        if api_key:
+            Utils.add_auth_to(_HEADERS, api_key)
 
     # Namespace API
     def create_namespace(self, namespace_name, owner_name, description=None):
         Utils.check_name_length(namespace_name, 'namespace_name')
         Utils.check_name_length(owner_name, 'owner_name')
 
         payload = {
```

### Comparing `marquez-python-0.7.8/marquez_client/backend.py` & `marquez-python-0.7.9/marquez_client/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 class Backend:
     def put(self, path, headers, json):
         pass
 
     def post(self, path, headers, json=None):
         pass
```

### Comparing `marquez-python-0.7.8/marquez_client/log_backend.py` & `marquez-python-0.7.9/marquez_client/log_backend.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_client/__init__.py` & `marquez-python-0.7.9/marquez_client/__init__.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_client/client_wo.py` & `marquez-python-0.7.9/marquez_client/client_wo.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_client/http_backend.py` & `marquez-python-0.7.9/marquez_client/http_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
-
 import requests
 
 from marquez_client import errors
 from marquez_client.backend import Backend
-
-log = logging.getLogger(__name__)
+from marquez_client.utils import Utils
+from marquez_client.constants import API_PATH_V1
 
 
 class HttpBackend(Backend):
-    def __init__(self, url, timeout):
+    def __init__(self, url, timeout, api_key: str = None):
         self._timeout = timeout
-        self._url = url
+        self._api_base = f"{url}{API_PATH_V1}"
+        self._api_key = api_key
 
     def put(self, path, headers, payload):
-        log.debug("_put()")
+        if self._api_key:
+            Utils.add_auth_to(headers, self._api_key)
 
         response = requests.put(
-            url=f'{self._url}{path}', headers=headers, json=payload,
-            timeout=self._timeout)
+            url=f"{self._api_base}{path}",
+            headers=headers,
+            json=payload,
+            timeout=self._timeout
+        )
 
         return self._response(response, as_json=True)
 
     def post(self, path, headers, payload=None):
-        log.debug("_post()")
+        if self._api_key:
+            Utils.add_auth_to(headers, self._api_key)
 
         response = requests.post(
-            url=f'{self._url}{path}', headers=headers, json=payload,
-            timeout=self._timeout)
+            url=f"{self._api_base}{path}",
+            headers=headers,
+            json=payload,
+            timeout=self._timeout
+        )
 
         return self._response(response, as_json=True)
 
     def _response(self, response, as_json):
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
```

### Comparing `marquez-python-0.7.8/marquez_client/clients.py` & `marquez-python-0.7.9/marquez_client/clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,52 +6,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
 import os
 
-import marquez_client
-from marquez_client.constants import (DEFAULT_MARQUEZ_BACKEND,
-                                      DEFAULT_MARQUEZ_URL,
-                                      DEFAULT_MARQUEZ_FILE,
-                                      DEFAULT_TIMEOUT_MS)
-from marquez_client.file_backend import FileBackend
+from marquez_client import MarquezClient, MarquezWriteOnlyClient
 from marquez_client.http_backend import HttpBackend
+from marquez_client.file_backend import FileBackend
 from marquez_client.log_backend import LogBackend
 from marquez_client.utils import Utils
-
-log = logging.getLogger(__name__)
+from marquez_client.constants import (
+    DEFAULT_MARQUEZ_BACKEND,
+    DEFAULT_MARQUEZ_URL,
+    DEFAULT_MARQUEZ_FILE,
+    DEFAULT_TIMEOUT_MS
+)
 
 
 # Marquez Clients
 class Clients(object):
-    def __init__(self):
-        log.debug("Clients.init")
-
     @staticmethod
     def new_client():
-        url = os.environ.get('MARQUEZ_URL', DEFAULT_MARQUEZ_URL)
-        return marquez_client.MarquezClient(url)
+        return MarquezClient(
+            url=os.environ.get('MARQUEZ_URL', DEFAULT_MARQUEZ_URL),
+            api_key=os.environ.get('MARQUEZ_API_KEY')
+        )
 
     @staticmethod
     def new_write_only_client():
-        return marquez_client.MarquezWriteOnlyClient(Clients.from_env())
+        return MarquezWriteOnlyClient(
+            backend=Clients._backend_from_env(),
+        )
 
     @staticmethod
-    def from_env():
-        backend_env = \
-            os.environ.get('MARQUEZ_BACKEND', DEFAULT_MARQUEZ_BACKEND)
+    def _backend_from_env():
+        backend = \
+            os.environ.get('MARQUEZ_BACKEND', DEFAULT_MARQUEZ_BACKEND).upper()
 
-        if backend_env == 'http':
+        if backend == 'HTTP':
             url = os.environ.get('MARQUEZ_URL', DEFAULT_MARQUEZ_URL)
+            api_key = os.environ.get('MARQUEZ_API_KEY')
             timeout = Utils.to_seconds(
                 os.environ.get('MARQUEZ_TIMEOUT_MS', DEFAULT_TIMEOUT_MS))
-            return HttpBackend(url, timeout)
-        elif backend_env == 'file':
+            return HttpBackend(url, timeout, api_key)
+        elif backend == 'FILE':
             file = os.environ.get('MARQUEZ_FILE', DEFAULT_MARQUEZ_FILE)
             return FileBackend(file)
-        elif backend_env == 'log':
+        elif backend == 'LOG':
             return LogBackend()
```

### Comparing `marquez-python-0.7.8/marquez_client/errors.py` & `marquez-python-0.7.9/marquez_client/errors.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_client/models.py` & `marquez-python-0.7.9/marquez_client/models.py`

 * *Files identical despite different names*

### Comparing `marquez-python-0.7.8/marquez_client/file_backend.py` & `marquez-python-0.7.9/marquez_client/file_backend.py`

 * *Files identical despite different names*

