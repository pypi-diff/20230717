# Comparing `tmp/notionaut-0.1.1.tar.gz` & `tmp/notionaut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionaut-0.1.1.tar", max compression
+gzip compressed data, was "notionaut-0.2.0.tar", max compression
```

## Comparing `notionaut-0.1.1.tar` & `notionaut-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       80 2023-06-19 21:35:19.704354 notionaut-0.1.1/README.md
--rw-r--r--   0        0        0      701 2023-07-13 01:25:52.190776 notionaut-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       67 2023-06-21 00:43:34.630935 notionaut-0.1.1/src/notionaut/__init__.py
--rw-r--r--   0        0        0     3225 2023-07-13 01:10:48.958301 notionaut-0.1.1/src/notionaut/client.py
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 notionaut-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-06-19 21:35:19.704354 notionaut-0.2.0/README.md
+-rw-r--r--   0        0        0      701 2023-07-17 03:56:10.664433 notionaut-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-06-21 00:43:34.630935 notionaut-0.2.0/src/notionaut/__init__.py
+-rw-r--r--   0        0        0     3914 2023-07-17 03:40:06.497128 notionaut-0.2.0/src/notionaut/client.py
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 notionaut-0.2.0/PKG-INFO
```

### Comparing `notionaut-0.1.1/pyproject.toml` & `notionaut-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notionaut"
-version = "0.1.1"
+version = "0.2.0"
 description = "A simple package for fetching Notion databases as pandas dataframes"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "notionaut", from = "src"}
 ]
```

### Comparing `notionaut-0.1.1/src/notionaut/client.py` & `notionaut-0.2.0/src/notionaut/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Dict, List
 
 import pandas as pd
 from notion_client import Client
 
 PARSE_MAP = {
     "rich_text": lambda x: x["rich_text"][0]["plain_text"] if x["rich_text"] else pd.NA,
-    "title": lambda x: x["title"][0]["plain_text"],
+    "title": lambda x: "".join(p["plain_text"] for p in x["title"]),
     "select": lambda x: x["select"]["name"],
     "multi_select": lambda x: [p["name"] for p in x["multi_select"]],
     "url": lambda x: x["url"],
     "relation": lambda x: [p["id"] for p in x["relation"]],
     "formula": lambda x: x["formula"]["string"],
     "checkbox": lambda x: x["checkbox"],
-    "date": lambda x: x["date"],
+    "date": lambda x: x["date"]["start"] if x["date"] else pd.NA,
     "number": lambda x: x["number"],
 }
 
 
 def parse_type(to_parse: Dict[str, any]) -> str:
     """
     Parses the type of a property from the Notion API response.
@@ -68,33 +68,54 @@
         :param notion: Optional parameter to inject the Notion client object.
         """
         if notion is None:
             self.notion = Client(auth=notion_token)
         else:
             self.notion = notion
 
-    def fetch_results(self, database_id: str) -> dict:
-        return self.notion.databases.query(database_id=database_id)
+    def fetch_results(
+        self, database_id: str, query_filter: dict = None, query_sort: dict = None
+    ) -> dict:
+        return self.notion.databases.query(
+            database_id=database_id, filter=query_filter, sorts=query_sort
+        )
 
-    def process_results(self, results: dict, columns: List[str] = None) -> pd.DataFrame:
+    def process_results(
+        self, results: dict, columns: List[str] = None, with_url: bool = False
+    ) -> pd.DataFrame:
         df = pd.DataFrame(results["results"])
         if df.empty:
             return pd.DataFrame()
         parsed = pd.DataFrame(
             [parse_row(to_parse=d, columns=columns) for d in df["properties"]]
         )
         parsed["id"] = df["id"]
         if columns:
             parsed = parsed[columns]
+        if with_url:
+            parsed["_url"] = df["url"].apply(
+                lambda x: x.replace("https://", "notion://")
+            )
         return parsed
 
-    def query(self, database_id: str, columns: List[str] = None) -> pd.DataFrame:
+    def query(
+        self,
+        database_id: str,
+        columns: List[str] = None,
+        query_filter: dict = None,
+        query_sort: dict = None,
+        with_url: bool = False,
+    ) -> pd.DataFrame:
         """
         Fetches data from a Notion database and returns it as a pandas DataFrame.
 
         :param database_id: The ID of the Notion database.
         :param columns: List of columns to include, defaults to None.
+        :param filter: Optional database query filter.
+        :param sorts: Optional database query sorting.
 
         :return: The fetched data as a pandas DataFrame.
         """
-        results = self.fetch_results(database_id=database_id)
-        return self.process_results(results=results, columns=columns)
+        results = self.fetch_results(
+            database_id=database_id, query_filter=query_filter, query_sort=query_sort
+        )
+        return self.process_results(results=results, columns=columns, with_url=with_url)
```

### Comparing `notionaut-0.1.1/PKG-INFO` & `notionaut-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionaut
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple package for fetching Notion databases as pandas dataframes
 Home-page: https://github.com/nschenone/notionaut
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

