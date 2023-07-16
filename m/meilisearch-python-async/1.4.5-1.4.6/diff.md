# Comparing `tmp/meilisearch_python_async-1.4.5.tar.gz` & `tmp/meilisearch_python_async-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.5.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.6.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.5.tar` & `meilisearch_python_async-1.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/LICENSE
--rw-r--r--   0        0        0     5759 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/README.md
--rw-r--r--   0        0        0      151 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0     1486 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_utils.py
--rw-r--r--   0        0        0       18 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22970 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-07-12 01:48:52.489498 meilisearch_python_async-1.4.5/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89322 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     4223 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0     1847 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1334 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0     3114 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11932 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2243 2023-07-12 01:48:52.493498 meilisearch_python_async-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-16 23:47:54.706177 meilisearch_python_async-1.4.6/LICENSE
+-rw-r--r--   0        0        0     5759 2023-07-16 23:47:54.706177 meilisearch_python_async-1.4.6/README.md
+-rw-r--r--   0        0        0      151 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0     1486 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/_utils.py
+-rw-r--r--   0        0        0       18 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22970 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89322 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     4223 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0     1847 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1334 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0     3311 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11906 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2243 2023-07-16 23:47:54.710177 meilisearch_python_async-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.6/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.5/LICENSE` & `meilisearch_python_async-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/README.md` & `meilisearch_python_async-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/_utils.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/_utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/models/index.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/models/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/models/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from datetime import datetime
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import pydantic
 from camel_converter.pydantic_base import CamelBase
 from pydantic import Field
 
 from meilisearch_python_async._utils import is_pydantic_2, iso_to_date_time
 
 
 class TaskId(CamelBase):
     uid: int
 
 
-class TaskStatus(TaskId):
+class TaskResult(TaskId):
     index_uid: Optional[str] = None
     status: str
     task_type: Union[str, Dict[str, Any]] = Field(..., alias="type")
-    details: Optional[Dict[str, Any]]
-    error: Optional[Dict[str, Any]]
-    canceled_by: Optional[int]
-    duration: Optional[str]
+    details: Optional[Dict[str, Any]] = None
+    error: Optional[Dict[str, Any]] = None
+    canceled_by: Optional[int] = None
+    duration: Optional[str] = None
     enqueued_at: datetime
-    started_at: Optional[datetime]
-    finished_at: Optional[datetime]
+    started_at: Optional[datetime] = None
+    finished_at: Optional[datetime] = None
 
     if is_pydantic_2():
 
         @pydantic.field_validator("enqueued_at", mode="before")  # type: ignore[attr-defined]
         @classmethod
         def validate_enqueued_at(cls, v: str) -> datetime:
             converted = iso_to_date_time(v)
@@ -65,14 +65,21 @@
 
         @pydantic.validator("finished_at", pre=True)
         @classmethod
         def validate_finished_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
 
+class TaskStatus(CamelBase):
+    results: List[TaskResult]
+    limit: int
+    from_: int = Field(..., alias="from")
+    next: Optional[int] = None
+
+
 class TaskInfo(CamelBase):
     task_uid: int
     index_uid: Optional[str] = None
     status: str
     task_type: Union[str, Dict[str, Any]] = Field(..., alias="type")
     enqueued_at: datetime
```

### Comparing `meilisearch_python_async-1.4.5/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.6/meilisearch_python_async/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING
 from urllib.parse import urlencode
 
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
 from meilisearch_python_async.errors import MeilisearchTaskFailedError, MeilisearchTimeoutError
-from meilisearch_python_async.models.task import TaskInfo, TaskStatus
+from meilisearch_python_async.models.task import TaskInfo, TaskResult, TaskStatus
 
 if TYPE_CHECKING:
     from meilisearch_python_async.client import Client  # pragma: no cover
 
 
 async def cancel_tasks(
     client: AsyncClient | Client,
@@ -152,27 +152,27 @@
 
 
 async def get_tasks(
     client: AsyncClient | Client,
     *,
     index_ids: list[str] | None = None,
     types: str | list[str] | None = None,
-) -> list[TaskStatus]:
+) -> TaskStatus:
     """Get multiple tasks.
 
     Args:
 
         client: An httpx AsyncClient or meilisearch_python_async Client instance.
         index_ids: A list of index UIDs for which to get the tasks. If provided this will get the
             tasks only for the specified indexes, if not all tasks will be returned. Default = None
         types: Specify specific task types to retrieve. Default = None
 
     Returns:
 
-        A list of all tasks.
+        Task statuses.
 
     Raises:
 
         MeilisearchCommunicationError: If there was an error communicating with the server.
         MeilisearchApiError: If the Meilisearch API returned an error.
         MeilisearchTimeoutError: If the connection times out.
 
@@ -187,28 +187,28 @@
     url = f"tasks?indexUids={','.join(index_ids)}" if index_ids else "tasks"
     if types:
         formatted_types = ",".join(types) if isinstance(types, list) else types
         url = f"{url}&types={formatted_types}" if "?" in url else f"{url}?types={formatted_types}"
     client_ = _get_client(client)
     response = await client_.get(url)
 
-    return [TaskStatus(**x) for x in response.json()["results"]]
+    return TaskStatus(**response.json())
 
 
-async def get_task(client: AsyncClient | Client, task_id: int) -> TaskStatus:
+async def get_task(client: AsyncClient | Client, task_id: int) -> TaskResult:
     """Get a single task from it's task id.
 
     Args:
 
         client: An httpx AsyncClient or meilisearch_python_async Client instance.
         task_id: Identifier of the task to retrieve.
 
     Returns:
 
-        A list of all tasks.
+        Results of a task.
 
     Raises:
 
         MeilisearchCommunicationError: If there was an error communicating with the server.
         MeilisearchApiError: If the Meilisearch API returned an error.
         MeilisearchTimeoutError: If the connection times out.
 
@@ -219,25 +219,25 @@
         >>>
         >>> async with Client("http://localhost.com", "masterKey") as client:
         >>>     await get_task(client, 1244)
     """
     client_ = _get_client(client)
     response = await client_.get(f"tasks/{task_id}")
 
-    return TaskStatus(**response.json())
+    return TaskResult(**response.json())
 
 
 async def wait_for_task(
     client: AsyncClient | Client,
     task_id: int,
     *,
     timeout_in_ms: int | None = 5000,
     interval_in_ms: int = 50,
     raise_for_status: bool = False,
-) -> TaskStatus:
+) -> TaskResult:
     """Wait until Meilisearch processes a task, and get its status.
 
     Args:
 
         client: An httpx AsyncClient or meilisearch_python_async Client instance.
         task_id: Identifier of the task to retrieve.
         timeout_in_ms: Amount of time in milliseconds to wait before raising a
@@ -276,29 +276,29 @@
     http_requests = HttpRequests(client_)
     start_time = datetime.now()
     elapsed_time = 0.0
 
     if timeout_in_ms:
         while elapsed_time < timeout_in_ms:
             response = await http_requests.get(url)
-            status = TaskStatus(**response.json())
+            status = TaskResult(**response.json())
             if status.status in ("succeeded", "failed"):
                 if raise_for_status and status.status == "failed":
                     raise MeilisearchTaskFailedError(f"Task {task_id} failed")
                 return status
             await sleep(interval_in_ms / 1000)
             time_delta = datetime.now() - start_time
             elapsed_time = time_delta.seconds * 1000 + time_delta.microseconds / 1000
         raise MeilisearchTimeoutError(
             f"timeout of {timeout_in_ms}ms has exceeded on process {task_id} when waiting for pending update to resolve."
         )
     else:
         while True:
             response = await http_requests.get(url)
-            status = TaskStatus(**response.json())
+            status = TaskResult(**response.json())
             if status.status in ("succeeded", "failed"):
                 return status
             await sleep(interval_in_ms / 1000)
 
 
 def _get_client(client: AsyncClient | Client) -> AsyncClient:
     if isinstance(client, AsyncClient):
```

### Comparing `meilisearch_python_async-1.4.5/pyproject.toml` & `meilisearch_python_async-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.5"
+version = "1.4.6"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.4.5/PKG-INFO` & `meilisearch_python_async-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
```

