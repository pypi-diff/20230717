# Comparing `tmp/databricks_vectorsearch_preview-0.1-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch_preview-0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18527 bytes, number of entries: 11
+Zip file size: 18506 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/__init__.py
--rw-r--r--  2.0 unx     9904 b- defN 23-Jul-17 18:51 databricks/vector_search/client.py
+-rw-r--r--  2.0 unx     9935 b- defN 23-Jul-17 19:30 databricks/vector_search/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/__init__.py
 -rw-r--r--  2.0 unx    65338 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/messages_pb2.py
 -rw-r--r--  2.0 unx    22870 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/service_pb2.py
 -rw-r--r--  2.0 unx    38292 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/taxonomy_pb2.py
--rw-r--r--  2.0 unx      569 b- defN 23-Jul-17 18:52 databricks_vectorsearch_preview-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 18:52 databricks_vectorsearch_preview-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 18:52 databricks_vectorsearch_preview-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1049 b- defN 23-Jul-17 18:52 databricks_vectorsearch_preview-0.1.dist-info/RECORD
-11 files, 138125 bytes uncompressed, 16695 bytes compressed:  87.9%
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1053 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/RECORD
+11 files, 138161 bytes uncompressed, 16666 bytes compressed:  87.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: databricks/vector_search/proto/service_pb2.py
 Comment: 
 
 Filename: databricks/vector_search/proto/taxonomy_pb2.py
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.1.dist-info/METADATA
+Filename: databricks_vectorsearch_preview-0.12.dist-info/METADATA
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.1.dist-info/WHEEL
+Filename: databricks_vectorsearch_preview-0.12.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.1.dist-info/top_level.txt
+Filename: databricks_vectorsearch_preview-0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.1.dist-info/RECORD
+Filename: databricks_vectorsearch_preview-0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/client.py

```diff
@@ -39,19 +39,21 @@
         Initializes a VectorSearchClient instance.
 
         :param workspace_url: Workspace URL of Databricks
         :param token: Token for authentication.
         """
         self._workspace_url = workspace_url
         if self._workspace_url is None:
-            self._workspace_url = "https://" + spark.conf.get("spark.databricks.workspaceUrl")
+            host_creds = databricks_utils.get_databricks_host_creds() 
+            self._workspace_url = host_creds.host
         
         self._token = token
         if self._token is None:
-            self._token = dbutils.notebook.entry_point.getDbutils().notebook().getContext().apiToken().get()
+            host_creds = databricks_utils.get_databricks_host_creds() 
+            self._token = host_creds.token
 
     def _call_endpoint(self, endpoint, method, params=None, json=None):
         headers = dict()
         headers["Authorization"] = f"Bearer {self._token}"
         cleaned_hostname = self._workspace_url[:-1] if self._workspace_url.endswith("/") else self._workspace_url
         url = f"{cleaned_hostname}{endpoint}"
         response = requests.request(
```

## Comparing `databricks_vectorsearch_preview-0.1.dist-info/METADATA` & `databricks_vectorsearch_preview-0.12.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-vectorsearch-preview
-Version: 0.1
+Version: 0.12
 Summary: Databricks Vector Search Client
 Home-page: UNKNOWN
 Author: Databirkcs
 Author-email: feedback@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `databricks_vectorsearch_preview-0.1.dist-info/RECORD` & `databricks_vectorsearch_preview-0.12.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 databricks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databricks/vector_search/client.py,sha256=rNFKtkGk-ARMzBAb_Ga1DGrzw0b9SDNJl55fK2V37PA,9904
+databricks/vector_search/client.py,sha256=q286sawnadZpEvXhs4CTirjCKNTJoI_IUQ-TwkinhNU,9935
 databricks/vector_search/proto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/proto/messages_pb2.py,sha256=z8DumqdRQrpXXNvREnZwCbNSGChRotuumEivwXMCVYQ,65338
 databricks/vector_search/proto/service_pb2.py,sha256=fprjawx10B1sao1YHwRYOZ-aGGHTG3pCykmrDBt8muY,22870
 databricks/vector_search/proto/taxonomy_pb2.py,sha256=YzToOng9nuUEtEe0th-7h8i_J3XjNeh7y3-n1syCEuA,38292
-databricks_vectorsearch_preview-0.1.dist-info/METADATA,sha256=bNeLkvIJjw768BVh39UNROGjkSp4B41uRT5gm7VZBOQ,569
-databricks_vectorsearch_preview-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-databricks_vectorsearch_preview-0.1.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
-databricks_vectorsearch_preview-0.1.dist-info/RECORD,,
+databricks_vectorsearch_preview-0.12.dist-info/METADATA,sha256=aeYmuzIIuYrMnYfSBUdVEP7wMEY73cLv9ZHn5UmqeH0,570
+databricks_vectorsearch_preview-0.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+databricks_vectorsearch_preview-0.12.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
+databricks_vectorsearch_preview-0.12.dist-info/RECORD,,
```

