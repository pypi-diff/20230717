# Comparing `tmp/databricks_vectorsearch_preview-0.12-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch_preview-0.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18506 bytes, number of entries: 11
+Zip file size: 18527 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/__init__.py
--rw-r--r--  2.0 unx     9935 b- defN 23-Jul-17 19:30 databricks/vector_search/client.py
+-rw-r--r--  2.0 unx    10087 b- defN 23-Jul-17 20:33 databricks/vector_search/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/__init__.py
--rw-r--r--  2.0 unx    65338 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/messages_pb2.py
--rw-r--r--  2.0 unx    22870 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/service_pb2.py
--rw-r--r--  2.0 unx    38292 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/taxonomy_pb2.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1053 b- defN 23-Jul-17 19:35 databricks_vectorsearch_preview-0.12.dist-info/RECORD
-11 files, 138161 bytes uncompressed, 16666 bytes compressed:  87.9%
+-rw-r--r--  2.0 unx    65338 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/messages_pb2.py
+-rw-r--r--  2.0 unx    22870 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/service_pb2.py
+-rw-r--r--  2.0 unx    38292 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/taxonomy_pb2.py
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/RECORD
+11 files, 138314 bytes uncompressed, 16687 bytes compressed:  87.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: databricks/vector_search/proto/service_pb2.py
 Comment: 
 
 Filename: databricks/vector_search/proto/taxonomy_pb2.py
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.12.dist-info/METADATA
+Filename: databricks_vectorsearch_preview-0.13.dist-info/METADATA
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.12.dist-info/WHEEL
+Filename: databricks_vectorsearch_preview-0.13.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.12.dist-info/top_level.txt
+Filename: databricks_vectorsearch_preview-0.13.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.12.dist-info/RECORD
+Filename: databricks_vectorsearch_preview-0.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/client.py

```diff
@@ -39,26 +39,30 @@
         Initializes a VectorSearchClient instance.
 
         :param workspace_url: Workspace URL of Databricks
         :param token: Token for authentication.
         """
         self._workspace_url = workspace_url
         if self._workspace_url is None:
-            host_creds = databricks_utils.get_databricks_host_creds() 
+            host_creds = databricks_utils.get_databricks_host_creds()
             self._workspace_url = host_creds.host
-        
+
         self._token = token
         if self._token is None:
-            host_creds = databricks_utils.get_databricks_host_creds() 
+            host_creds = databricks_utils.get_databricks_host_creds()
             self._token = host_creds.token
 
     def _call_endpoint(self, endpoint, method, params=None, json=None):
         headers = dict()
         headers["Authorization"] = f"Bearer {self._token}"
-        cleaned_hostname = self._workspace_url[:-1] if self._workspace_url.endswith("/") else self._workspace_url
+        cleaned_hostname = (
+            self._workspace_url[:-1]
+            if self._workspace_url.endswith("/")
+            else self._workspace_url
+        )
         url = f"{cleaned_hostname}{endpoint}"
         response = requests.request(
             url=url, headers=headers, method=method, params=params, json=json
         )
         log.info(response.text)
         return response.json()
 
@@ -120,15 +124,15 @@
     # index_column indicates the column that will do the embedding
     def create_index(
         self,
         source_table_name,
         dest_index_name,
         primary_key,
         index_column,
-        embedding_model_endpoint_name
+        embedding_model_endpoint_name,
     ):
         """
         Creates an index
 
         :param source_table_name: The source delta table where the pre-chunked document texts are located. Must be an Unity Catalog table in the form of <catalog>.<schema>.<table>
         :param dest_index_name: The name of the index to be created under the online catalog. must be in the format of <catalog>.<schema>.<table>
         :param primary_key: Column that represents a non-nullable unqiue identifier of the documents to be stored in the index.
@@ -151,20 +155,23 @@
             embedding_model_endpoint_name="e5-large-v2")
         print(response)
         """
         index_request = CreateVectorSearchIndexRequest()
 
         vector_index_column = VectorIndex()
         vector_index_column.column = index_column
-        vector_index_column.embedding_model_endpoint_name = embedding_model_endpoint_name
+        vector_index_column.embedding_model_endpoint_name = (
+            embedding_model_endpoint_name
+        )
 
         index_request.index_pipeline_spec.src_table = source_table_name
         index_request.index_pipeline_spec.dest_index = dest_index_name
         index_request.index_pipeline_spec.primary_key = primary_key
         index_request.index_pipeline_spec.vector_index.MergeFrom(vector_index_column)
+        index_request.index_pipeline_spec.continuous.SetInParent()
 
         json_str = MessageToJson(index_request, preserving_proto_field_name=True)
 
         log.info(json_str)
 
         return self._call_endpoint(
             "/api/2.0/vector-search/index", "POST", json=json.loads(json_str)
@@ -242,8 +249,10 @@
         """
         Lists all existing indexes created under the specified catalog.
 
         :param catalog_name: The name of the catalog.
 
         :return: The response from the API call.
         """
-        return self._call_endpoint(f"/api/2.0/vector-search/index/{catalog_name}", "GET")
+        return self._call_endpoint(
+            f"/api/2.0/vector-search/index/{catalog_name}", "GET"
+        )
```

## Comparing `databricks_vectorsearch_preview-0.12.dist-info/METADATA` & `databricks_vectorsearch_preview-0.13.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-vectorsearch-preview
-Version: 0.12
+Version: 0.13
 Summary: Databricks Vector Search Client
 Home-page: UNKNOWN
 Author: Databirkcs
 Author-email: feedback@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `databricks_vectorsearch_preview-0.12.dist-info/RECORD` & `databricks_vectorsearch_preview-0.13.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 databricks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databricks/vector_search/client.py,sha256=q286sawnadZpEvXhs4CTirjCKNTJoI_IUQ-TwkinhNU,9935
+databricks/vector_search/client.py,sha256=lDmtRZW2tTG6kM00loRfqMIg2oAHGG8mNhpe-CirKB8,10087
 databricks/vector_search/proto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/proto/messages_pb2.py,sha256=z8DumqdRQrpXXNvREnZwCbNSGChRotuumEivwXMCVYQ,65338
 databricks/vector_search/proto/service_pb2.py,sha256=fprjawx10B1sao1YHwRYOZ-aGGHTG3pCykmrDBt8muY,22870
 databricks/vector_search/proto/taxonomy_pb2.py,sha256=YzToOng9nuUEtEe0th-7h8i_J3XjNeh7y3-n1syCEuA,38292
-databricks_vectorsearch_preview-0.12.dist-info/METADATA,sha256=aeYmuzIIuYrMnYfSBUdVEP7wMEY73cLv9ZHn5UmqeH0,570
-databricks_vectorsearch_preview-0.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-databricks_vectorsearch_preview-0.12.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
-databricks_vectorsearch_preview-0.12.dist-info/RECORD,,
+databricks_vectorsearch_preview-0.13.dist-info/METADATA,sha256=RRrPzMYME4JMA2qi8L4JB0-At8H9aQ5AnbQfOFDKJlM,570
+databricks_vectorsearch_preview-0.13.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+databricks_vectorsearch_preview-0.13.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
+databricks_vectorsearch_preview-0.13.dist-info/RECORD,,
```

