# Comparing `tmp/imerit_ango-1.2.0-py3-none-any.whl.zip` & `tmp/imerit_ango-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9781 bytes, number of entries: 11
+Zip file size: 9822 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/__init__.py
 -rw-r--r--  2.0 unx     1304 b- defN 23-Jul-10 08:52 imerit_ango/plugin_logger.py
--rw-r--r--  2.0 unx     6925 b- defN 23-Jul-12 10:57 imerit_ango/plugins.py
--rw-r--r--  2.0 unx    16587 b- defN 23-Jul-12 10:54 imerit_ango/sdk.py
+-rw-r--r--  2.0 unx     6966 b- defN 23-Jul-17 15:46 imerit_ango/plugins.py
+-rw-r--r--  2.0 unx    16630 b- defN 23-Jul-17 15:49 imerit_ango/sdk.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/models/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Jul-10 08:52 imerit_ango/models/enums.py
 -rw-r--r--  2.0 unx     5452 b- defN 23-Jul-10 08:52 imerit_ango/models/label_category.py
--rw-r--r--  2.0 unx     1940 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/RECORD
-11 files, 33295 bytes uncompressed, 8267 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     1940 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/RECORD
+11 files, 33379 bytes uncompressed, 8308 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imerit_ango/models/enums.py
 Comment: 
 
 Filename: imerit_ango/models/label_category.py
 Comment: 
 
-Filename: imerit_ango-1.2.0.dist-info/METADATA
+Filename: imerit_ango-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: imerit_ango-1.2.0.dist-info/WHEEL
+Filename: imerit_ango-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: imerit_ango-1.2.0.dist-info/top_level.txt
+Filename: imerit_ango-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: imerit_ango-1.2.0.dist-info/RECORD
+Filename: imerit_ango-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imerit_ango/plugins.py

```diff
@@ -100,20 +100,21 @@
                             datetime.datetime.fromisoformat(data.completed_at[1])]
         if data.get("updated_at", None):
             updated_at = [datetime.datetime.fromisoformat(data.updated_at[0]),
                           datetime.datetime.fromisoformat(data.updated_at[1])]
 
         try:
             if self.version == 'v3':
-                json_export = sdk.exportV3(project_id, batches=data.get('batches', None),
+                (json_export, num_lines) = sdk.exportV3(project_id, batches=data.get('batches', None),
                                          stage=data.get('stage', None), format="ndjson")
+                data["numTasks"] = num_lines
             else:
                 json_export = sdk.export(project_id, data.get('assignees', None), completed_at=completed_at,
                                      updated_at=updated_at, batches=data.get('batches', None),
-                                     stage=data.get('stage', None), format="ndjson")
+                                     stage=data.get('stage', None))
         except Exception as e:
             logger.error(f"Error calling sdk.export: {e}")
             return
 
         data["jsonExport"] = json_export
         data["logger"] = logger
```

## imerit_ango/sdk.py

```diff
@@ -303,15 +303,15 @@
         filehandle, _ = urllib.request.urlretrieve(link)
 
         with zipfile.ZipFile(filehandle, 'r') as zip_file_object:
             first_file = zip_file_object.namelist()[0]
             with zip_file_object.open(first_file) as file:
                 content = file.read()
                 if format == "ndjson":
-                    json_response = self.__generate_ndjson_iterator(content)
+                    json_response = self.__generate_ndjson_iterator(content), content.count('\n')
                 else:
                     json_response = json.loads(content)
 
         return json_response
 
     def exportV3(self, project_id: str, batches: List[str] = None, stage: str = None, format: str ="json"):
 
@@ -342,15 +342,15 @@
         filehandle, _ = urllib.request.urlretrieve(link)
 
         with zipfile.ZipFile(filehandle, 'r') as zip_file_object:
             first_file = zip_file_object.namelist()[0]
             with zip_file_object.open(first_file) as file:
                 content = file.read()
                 if format == "ndjson":
-                    json_response = self.__generate_ndjson_iterator(content)
+                    json_response = self.__generate_ndjson_iterator(content), content.count(b'\n')
                 else:
                     json_response = json.loads(content)
 
         return json_response
 
     def create_label_set(self, project_id: str, tools: List[ToolCategory] = [],
                          classifications: List[ClassificationCategory] = [],
```

## Comparing `imerit_ango-1.2.0.dist-info/METADATA` & `imerit_ango-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `imerit_ango-1.2.0.dist-info/RECORD` & `imerit_ango-1.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 imerit_ango/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/plugin_logger.py,sha256=kE3Bv8wqzXJzXHSxyZb7AdoTW0QeytZc137GDqcFsSI,1304
-imerit_ango/plugins.py,sha256=dLky5cI5KGeDbdZJ1QLGjQ8ZEYyOF3RSpyHWP547zTM,6925
-imerit_ango/sdk.py,sha256=_VmNs7Gq8nhU_gtEoR3LhJyowiwrL7V53ePWHwYeFGc,16587
+imerit_ango/plugins.py,sha256=x6wY54iLDCLkgxapRcZ5efLET4LMR8cLnpmfCktBFy4,6966
+imerit_ango/sdk.py,sha256=ghc4OPRASM0h1tu8obq73e42hqGxO-lTZeVABmaKnfw,16630
 imerit_ango/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/models/enums.py,sha256=vy38MqYeZkiRop8viSLmua-Mj0soMfBnjILTSOr8uSk,93
 imerit_ango/models/label_category.py,sha256=c46Lve-vV1NoHi5-kk8D0BO8pYSS177d4sNYeA19CZQ,5452
-imerit_ango-1.2.0.dist-info/METADATA,sha256=d50DzWwq4m5B-g1Y-2n0UTl1278CfhLsWbMdjMT_GOk,1940
-imerit_ango-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-imerit_ango-1.2.0.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
-imerit_ango-1.2.0.dist-info/RECORD,,
+imerit_ango-1.2.1.dist-info/METADATA,sha256=iVOLdmjz12lDWk120VpKxFIc7JWltFIKLWkLu1eBhvk,1940
+imerit_ango-1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+imerit_ango-1.2.1.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
+imerit_ango-1.2.1.dist-info/RECORD,,
```

