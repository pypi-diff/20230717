# Comparing `tmp/tap-clickup-0.0.8.tar.gz` & `tmp/tap-clickup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-clickup-0.0.8.tar", max compression
+gzip compressed data, was "tap-clickup-0.0.9.tar", max compression
```

## Comparing `tap-clickup-0.0.8.tar` & `tap-clickup-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      628 2021-10-13 18:55:05.702952 tap-clickup-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-08-25 20:24:42.887317 tap-clickup-0.0.8/tap_clickup/__init__.py
--rw-r--r--   0        0        0      103 2021-08-25 20:24:42.883317 tap-clickup-0.0.8/tap_clickup/auth.py
--rw-r--r--   0        0        0     5656 2021-09-29 02:01:38.742099 tap-clickup-0.0.8/tap_clickup/client.py
--rw-r--r--   0        0        0     2358 2021-09-30 01:30:45.937196 tap-clickup-0.0.8/tap_clickup/schemas/custom_field.json
--rw-r--r--   0        0        0     3744 2021-10-12 20:19:50.665283 tap-clickup-0.0.8/tap_clickup/schemas/folder.json
--rw-r--r--   0        0        0     2623 2021-09-08 12:54:02.830246 tap-clickup-0.0.8/tap_clickup/schemas/goal.json
--rw-r--r--   0        0        0     3461 2021-10-12 20:19:50.665283 tap-clickup-0.0.8/tap_clickup/schemas/list.json
--rw-r--r--   0        0        0     3863 2021-10-13 18:53:43.631490 tap-clickup-0.0.8/tap_clickup/schemas/shared.json
--rw-r--r--   0        0        0     5555 2021-10-12 20:19:50.665283 tap-clickup-0.0.8/tap_clickup/schemas/space.json
--rw-r--r--   0        0        0      283 2021-09-08 12:54:02.830246 tap-clickup-0.0.8/tap_clickup/schemas/tag.json
--rw-r--r--   0        0        0    10032 2021-10-12 20:19:50.665283 tap-clickup-0.0.8/tap_clickup/schemas/task.json
--rw-r--r--   0        0        0      211 2021-09-08 12:54:02.830246 tap-clickup-0.0.8/tap_clickup/schemas/task_template.json
--rw-r--r--   0        0        0     2242 2021-09-29 22:04:48.374501 tap-clickup-0.0.8/tap_clickup/schemas/team.json
--rw-r--r--   0        0        0     8917 2021-09-29 20:21:28.015469 tap-clickup-0.0.8/tap_clickup/streams.py
--rw-r--r--   0        0        0     1289 2021-09-30 01:30:45.937196 tap-clickup-0.0.8/tap_clickup/tap.py
--rw-r--r--   0        0        0       34 2021-08-25 20:24:42.891317 tap-clickup-0.0.8/tap_clickup/tests/__init__.py
--rw-r--r--   0        0        0      704 2021-08-29 20:36:09.858970 tap-clickup-0.0.8/tap_clickup/tests/test_core.py
--rw-r--r--   0        0        0      839 2021-10-13 18:55:09.333093 tap-clickup-0.0.8/setup.py
--rw-r--r--   0        0        0      458 2021-10-13 18:55:09.333357 tap-clickup-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7921 2021-10-14 12:19:39.078390 tap-clickup-0.0.9/README.md
+-rw-r--r--   0        0        0     1164 2021-10-14 12:20:20.914107 tap-clickup-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-08-25 20:24:42.887317 tap-clickup-0.0.9/tap_clickup/__init__.py
+-rw-r--r--   0        0        0     4551 2021-10-13 20:33:47.683790 tap-clickup-0.0.9/tap_clickup/client.py
+-rw-r--r--   0        0        0     2358 2021-09-30 01:30:45.937196 tap-clickup-0.0.9/tap_clickup/schemas/custom_field.json
+-rw-r--r--   0        0        0     3744 2021-10-12 20:19:50.665283 tap-clickup-0.0.9/tap_clickup/schemas/folder.json
+-rw-r--r--   0        0        0     2623 2021-09-08 12:54:02.830246 tap-clickup-0.0.9/tap_clickup/schemas/goal.json
+-rw-r--r--   0        0        0     3461 2021-10-12 20:19:50.665283 tap-clickup-0.0.9/tap_clickup/schemas/list.json
+-rw-r--r--   0        0        0     3863 2021-10-13 18:53:43.631490 tap-clickup-0.0.9/tap_clickup/schemas/shared.json
+-rw-r--r--   0        0        0     5555 2021-10-12 20:19:50.665283 tap-clickup-0.0.9/tap_clickup/schemas/space.json
+-rw-r--r--   0        0        0      283 2021-09-08 12:54:02.830246 tap-clickup-0.0.9/tap_clickup/schemas/tag.json
+-rw-r--r--   0        0        0    10032 2021-10-12 20:19:50.665283 tap-clickup-0.0.9/tap_clickup/schemas/task.json
+-rw-r--r--   0        0        0      211 2021-09-08 12:54:02.830246 tap-clickup-0.0.9/tap_clickup/schemas/task_template.json
+-rw-r--r--   0        0        0     2242 2021-09-29 22:04:48.374501 tap-clickup-0.0.9/tap_clickup/schemas/team.json
+-rw-r--r--   0        0        0     8817 2021-10-14 12:19:39.078390 tap-clickup-0.0.9/tap_clickup/streams.py
+-rw-r--r--   0        0        0     1214 2021-10-14 12:19:39.078390 tap-clickup-0.0.9/tap_clickup/tap.py
+-rw-r--r--   0        0        0       34 2021-08-25 20:24:42.891317 tap-clickup-0.0.9/tap_clickup/tests/__init__.py
+-rw-r--r--   0        0        0      704 2021-08-29 20:36:09.858970 tap-clickup-0.0.9/tap_clickup/tests/test_core.py
+-rw-r--r--   0        0        0     8981 2021-10-14 12:21:27.205483 tap-clickup-0.0.9/setup.py
+-rw-r--r--   0        0        0     8907 2021-10-14 12:21:27.205957 tap-clickup-0.0.9/PKG-INFO
```

### Comparing `tap-clickup-0.0.8/tap_clickup/client.py` & `tap-clickup-0.0.9/tap_clickup/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,48 +6,38 @@
 import time
 import requests
 import backoff
 from requests.exceptions import RequestException
 from singer_sdk.helpers.jsonpath import extract_jsonpath
 from singer_sdk.streams import RESTStream
 
-
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class ClickUpStream(RESTStream):
     """ClickUp stream class."""
 
     url_base = "https://api.clickup.com/api/v2"
-
-    # @property
-    # def url_base(self) -> str:
-    #     """Return the API URL root, configurable via tap settings."""
-    #     return self.config["api_url"]
-
     records_jsonpath = "$[*]"  # Or override `parse_response`.
     next_page_token_jsonpath = "$.next_page"  # Or override `get_next_page_token`.
 
     @property
     def http_headers(self) -> dict:
         """Return the http headers needed."""
         headers = {}
         if "user_agent" in self.config:
             headers["User-Agent"] = self.config.get("user_agent")
-        # If not using an authenticator, you may also provide inline auth headers:
+
         headers["Authorization"] = self.config.get("api_token")
         return headers
 
     def get_next_page_token(
         self, response: requests.Response, previous_token: Optional[Any]
     ) -> Optional[Any]:
         """Return a token for identifying next page or None if no more pages."""
-        # TODO: If pagination is required, return a token which can be used to get the
-        #       next page. If this is the final page, return "None" to end the
-        #       pagination loop.
         if self.next_page_token_jsonpath:
             all_matches = extract_jsonpath(
                 self.next_page_token_jsonpath, response.json()
             )
             first_match = next(iter(all_matches), None)
             next_page_token = first_match
         else:
@@ -117,26 +107,10 @@
                 f"[{response.status_code} - {str(response.content)}]".replace(
                     "\\n", "\n"
                 )
             )
         self.logger.debug("Response received successfully.")
         return response
 
-    def prepare_request_payload(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Optional[dict]:
-        """Prepare the data payload for the REST API request.
-
-        By default, no payload will be sent (return None).
-        """
-        # TODO: Delete this method if no payload is required. (Most REST APIs.)
-        return None
-
     def parse_response(self, response: requests.Response) -> Iterable[dict]:
         """Parse the response and return an iterator of result rows."""
-        # TODO: Parse response body and return a set of records.
         yield from extract_jsonpath(self.records_jsonpath, input=response.json())
-
-    def post_process(self, row: dict, context: Optional[dict] = None) -> dict:
-        """As needed, append or transform raw data to match expected structure."""
-        # TODO: Delete this method if not needed.
-        return row
```

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/custom_field.json` & `tap-clickup-0.0.9/tap_clickup/schemas/custom_field.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/folder.json` & `tap-clickup-0.0.9/tap_clickup/schemas/folder.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/goal.json` & `tap-clickup-0.0.9/tap_clickup/schemas/goal.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/list.json` & `tap-clickup-0.0.9/tap_clickup/schemas/list.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/shared.json` & `tap-clickup-0.0.9/tap_clickup/schemas/shared.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/space.json` & `tap-clickup-0.0.9/tap_clickup/schemas/space.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/task.json` & `tap-clickup-0.0.9/tap_clickup/schemas/task.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/schemas/team.json` & `tap-clickup-0.0.9/tap_clickup/schemas/team.json`

 * *Files identical despite different names*

### Comparing `tap-clickup-0.0.8/tap_clickup/streams.py` & `tap-clickup-0.0.9/tap_clickup/streams.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,32 +97,14 @@
     def get_child_context(self, record: dict, context: Optional[dict]) -> dict:
         """Return a context dictionary for child streams."""
         return {
             "list_id": record["id"],
         }
 
 
-class ListsStream(ClickUpStream):
-    """Lists"""
-
-    name = "list"
-    path = "/folder/{folder_id}/list"
-    primary_keys = ["id"]
-    replication_key = None
-    schema_filepath = SCHEMAS_DIR / "list.json"
-    records_jsonpath = "$.lists[*]"
-    parent_stream_type = FoldersStream
-
-    def get_child_context(self, record: dict, context: Optional[dict]) -> dict:
-        """Return a context dictionary for child streams."""
-        return {
-            "list_id": record["id"],
-        }
-
-
 class TaskTemplatesStream(ClickUpStream):
     """TaskTemplates"""
 
     name = "task_template"
     path = "/team/{team_id}/task_template?page=0"
     primary_keys = ["id"]
     replication_key = None
@@ -163,26 +145,38 @@
     primary_keys = []
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "shared.json"
     records_jsonpath = "$.shared"
     parent_stream_type = TeamsStream
 
 
-class CustomFieldsStream(ClickUpStream):
-    """CustomField"""
+class FolderlessCustomFieldsStream(ClickUpStream):
+    """CustomField from folderless lists"""
 
-    name = "custom_field"
+    name = "folderless_customfield"
     path = "/list/{list_id}/field"
     primary_keys = ["id"]
     replication_key = None
     schema_filepath = SCHEMAS_DIR / "custom_field.json"
     records_jsonpath = "$.fields[*]"
     parent_stream_type = FolderlessListsStream
 
 
+class FolderCustomFieldsStream(ClickUpStream):
+    """CustomFields from foldered lists"""
+
+    name = "folder_customfield"
+    path = "/list/{list_id}/field"
+    primary_keys = ["id"]
+    replication_key = None
+    schema_filepath = SCHEMAS_DIR / "custom_field.json"
+    records_jsonpath = "$.fields[*]"
+    parent_stream_type = FolderListsStream
+
+
 class ClickUpTasksStream(ClickUpStream):
     """Parent Class for Task Streams"""
 
     initial_replication_key_dict = {}
 
     def initial_replication_key(self, context) -> int:
         path = self.get_url(context)
```

### Comparing `tap-clickup-0.0.8/tap_clickup/tests/test_core.py` & `tap-clickup-0.0.9/tap_clickup/tests/test_core.py`

 * *Files identical despite different names*

