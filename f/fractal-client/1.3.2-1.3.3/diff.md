# Comparing `tmp/fractal_client-1.3.2.tar.gz` & `tmp/fractal_client-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.2.tar", max compression
+gzip compressed data, was "fractal_client-1.3.3.tar", max compression
```

## Comparing `fractal_client-1.3.2.tar` & `fractal_client-1.3.3.tar`

### file list

```diff
@@ -1,69 +1,44 @@
--rw-r--r--   0        0        0     1576 2023-06-23 06:18:32.718024 fractal_client-1.3.2/LICENSE
--rw-r--r--   0        0        0     2492 2023-06-23 06:18:32.718024 fractal_client-1.3.2/README.md
--rw-r--r--   0        0        0       22 2023-07-06 09:46:14.837728 fractal_client-1.3.2/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/authclient.py
--rw-r--r--   0        0        0     3773 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/client.py
--rw-r--r--   0        0        0    12348 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     6863 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5795 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5115 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4031 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_project.py
--rw-r--r--   0        0        0     7260 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4620 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_user.py
--rw-r--r--   0        0        0    10027 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0       42 2023-07-06 09:45:54.749947 fractal_client-1.3.2/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-07-06 09:46:22.653643 fractal_client-1.3.2/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      411 2023-07-06 09:46:22.189648 fractal_client-1.3.2/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1753 2023-07-06 09:46:22.221647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1610 2023-07-06 09:46:22.189648 fractal_client-1.3.2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     4068 2023-07-06 09:46:22.225647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3537 2023-07-06 09:46:22.229647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     1165 2023-07-06 09:46:22.233647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     2705 2023-07-06 09:46:22.233647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     3292 2023-07-06 09:46:22.237647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1202 2023-07-06 09:46:22.237647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     3882 2023-07-06 09:46:22.589643 fractal_client-1.3.2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-07-06 09:46:22.149648 fractal_client-1.3.2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      606 2023-07-06 09:46:22.181648 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     3382 2023-07-06 09:46:22.593643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1241 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1164 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1763 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2792 2023-07-06 09:46:22.601643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1335 2023-07-06 09:46:22.601643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2671 2023-07-06 09:46:22.621643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2911 2023-07-06 09:46:22.625643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      139 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/interface.py
--rw-r--r--   0        0        0    23932 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/response.py
--rw-r--r--   0        0        0     1850 2023-07-06 09:46:14.837728 fractal_client-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 fractal_client-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:32.718024 fractal_client-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2492 2023-06-23 06:18:32.718024 fractal_client-1.3.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-17 13:15:54.693361 fractal_client-1.3.3/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/client.py
+-rw-r--r--   0        0        0    12411 2023-07-17 13:13:51.354705 fractal_client-1.3.3/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     7260 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/cmd/_user.py
+-rw-r--r--   0        0        0    10333 2023-07-17 13:13:51.354705 fractal_client-1.3.3/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0     1964 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-06 09:46:22.653643 fractal_client-1.3.3/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       59 2023-07-17 12:27:00.751536 fractal_client-1.3.3/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      411 2023-07-06 09:46:22.189648 fractal_client-1.3.3/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-07-06 09:46:22.221647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2684 2023-07-17 12:27:10.675464 fractal_client-1.3.3/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4068 2023-07-06 09:46:22.225647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3537 2023-07-06 09:46:22.229647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1165 2023-07-06 09:46:22.233647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2705 2023-07-06 09:46:22.233647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3292 2023-07-06 09:46:22.237647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1202 2023-07-06 09:46:22.237647 fractal_client-1.3.3/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3882 2023-07-06 09:46:22.589643 fractal_client-1.3.3/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     2392 2023-07-17 12:27:00.755536 fractal_client-1.3.3/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-07-06 09:45:54.765947 fractal_client-1.3.3/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0     1285 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/interface.py
+-rw-r--r--   0        0        0    24380 2023-07-17 13:13:51.354705 fractal_client-1.3.3/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-06-23 06:18:32.722024 fractal_client-1.3.3/fractal/response.py
+-rw-r--r--   0        0        0     2008 2023-07-17 13:15:54.693361 fractal_client-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 fractal_client-1.3.3/PKG-INFO
```

### Comparing `fractal_client-1.3.2/LICENSE` & `fractal_client-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/README.md` & `fractal_client-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/authclient.py` & `fractal_client-1.3.3/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/client.py` & `fractal_client-1.3.3/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/__init__.py` & `fractal_client-1.3.3/fractal/cmd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,16 @@
     elif subcmd == "apply":
         parameters = [
             "project_id",
             "workflow_id",
             "input_dataset_id",
             "output_dataset_id",
             "worker_init",
+            "first_task_index",
+            "last_task_index",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await workflow_apply(client, **function_kwargs)
     elif subcmd == "import":
         parameters = ["project_id", "json_file"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await workflow_import(client, batch=batch, **function_kwargs)
```

### Comparing `fractal_client-1.3.2/fractal/cmd/_aux_task_caching.py` & `fractal_client-1.3.3/fractal/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_dataset.py` & `fractal_client-1.3.3/fractal/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_job.py` & `fractal_client-1.3.3/fractal/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_project.py` & `fractal_client-1.3.3/fractal/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_task.py` & `fractal_client-1.3.3/fractal/cmd/_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_user.py` & `fractal_client-1.3.3/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/cmd/_workflow.py` & `fractal_client-1.3.3/fractal/cmd/_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,24 +222,30 @@
 async def workflow_apply(
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
     input_dataset_id: int,
     output_dataset_id: int,
+    first_task_index: Optional[int] = None,
+    last_task_index: Optional[int] = None,
     worker_init: Optional[str] = None,
 ) -> BaseInterface:
     apply_wf_create_dict = dict(
         workflow_id=workflow_id,
         input_dataset_id=input_dataset_id,
         output_dataset_id=output_dataset_id,
     )
     # Prepare ApplyWorkflowCreate object, without None attributes
-    if worker_init:
+    if worker_init is not None:
         apply_wf_create_dict["worker_init"] = worker_init
+    if first_task_index is not None:
+        apply_wf_create_dict["first_task_index"] = first_task_index
+    if last_task_index is not None:
+        apply_wf_create_dict["last_task_index"] = last_task_index
     apply_wf_create = ApplyWorkflowCreate(**apply_wf_create_dict)
 
     # Prepare query parameters
     query_parameters = (
         f"input_dataset_id={input_dataset_id}"
         f"&output_dataset_id={output_dataset_id}"
     )
```

### Comparing `fractal_client-1.3.2/fractal/common/README.md` & `fractal_client-1.3.3/fractal/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__init__.py` & `fractal_client-1.3.3/fractal/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_client-1.3.3/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/_validators.py` & `fractal_client-1.3.3/fractal/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/manifest.py` & `fractal_client-1.3.3/fractal/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/project.py` & `fractal_client-1.3.3/fractal/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/state.py` & `fractal_client-1.3.3/fractal/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/task.py` & `fractal_client-1.3.3/fractal/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/task_collection.py` & `fractal_client-1.3.3/fractal/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/user.py` & `fractal_client-1.3.3/fractal/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/common/schemas/workflow.py` & `fractal_client-1.3.3/fractal/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/config.py` & `fractal_client-1.3.3/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/interface.py` & `fractal_client-1.3.3/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/fractal/parser.py` & `fractal_client-1.3.3/fractal/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,18 +652,32 @@
 workflow_apply_parser = workflow_subparsers.add_parser(
     "apply",
     description="Apply workflow to dataset",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
 
-workflow_apply_parser.add_argument("project_id")
-workflow_apply_parser.add_argument("workflow_id")
-workflow_apply_parser.add_argument("input_dataset_id")
-workflow_apply_parser.add_argument("output_dataset_id")
+workflow_apply_parser.add_argument("project_id", type=int)
+workflow_apply_parser.add_argument("workflow_id", type=int)
+workflow_apply_parser.add_argument("input_dataset_id", type=int)
+workflow_apply_parser.add_argument("output_dataset_id", type=int)
+workflow_apply_parser.add_argument(
+        "--start",
+        dest="first_task_index",
+        type=int,
+        help="Positional index of the first task to be executed",
+        required=False,
+        )
+workflow_apply_parser.add_argument(
+        "--end",
+        dest="last_task_index",
+        type=int,
+        help="Positional index of the last task to be executed",
+        required=False,
+        )
 workflow_apply_parser.add_argument(
     "-w",
     "--worker-init",
     help="Command to be run before starting a worker",
 )
 
 # workflow import
```

### Comparing `fractal_client-1.3.2/fractal/response.py` & `fractal_client-1.3.3/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.2/pyproject.toml` & `fractal_client-1.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.2"
+version = "1.3.3"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
 packages = [
     {include="fractal"}
 ]
 homepage = "https://github.com/fractal-analytics-platform/fractal"
 license = "BSD-3-Clause"
+exclude = [
+"fractal/.gitignore",
+"fractal/common/tests",
+"fractal/common/requirements",
+"fractal/common/.git*",
+"fractal/common/.pre-commit-config.yaml",
+]
+
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.20.0"
 rich = "^12.5.1"
 httpx = "^0.23.0"
 PyJWT = "^2.4.0"
@@ -43,15 +51,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.2"
+current_version = "1.3.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.3.2/PKG-INFO` & `fractal_client-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.3.2
+Version: 1.3.3
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

