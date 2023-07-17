# Comparing `tmp/gs_engine-0.24.0a20230716-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.24.0a20230717-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11941 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      840 b- defN 23-Jul-16 21:35 gs_engine-0.24.0a20230716.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-Jul-16 21:16 gs_engine-0.24.0a20230716.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-16 21:16 gs_engine-0.24.0a20230716.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21680 b- defN 23-Jul-16 21:16 gs_engine-0.24.0a20230716.dist-info/METADATA
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-16 19:04 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-Jul-16 19:04 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-16 19:04 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-16 19:04 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-16 19:04 graphscope.runtime/conf/log4rs.yml
-9 files, 26097 bytes uncompressed, 10479 bytes compressed:  59.8%
+Zip file size: 11917 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-17 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/RECORD
+9 files, 26058 bytes uncompressed, 10455 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: gs_engine-0.24.0a20230716.dist-info/RECORD
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.24.0a20230716.dist-info/WHEEL
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.24.0a20230716.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.24.0a20230716.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.24.0a20230717.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.24.0a20230717.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.24.0a20230717.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.24.0a20230717.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.24.0a20230716.dist-info/RECORD` & `gs_engine-0.24.0a20230717.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gs_engine-0.24.0a20230716.dist-info/RECORD,,
-gs_engine-0.24.0a20230716.dist-info/WHEEL,sha256=fw_hGi-Yx84a3ggAIzpSq5odRE77o5K1cXAmZvJuyLk,140
-gs_engine-0.24.0a20230716.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.24.0a20230716.dist-info/METADATA,sha256=MGgMhhL5BEoOnhrWqNWIjfOctIxrKiI0-UH4npGChm8,21680
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
-graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
-graphscope.runtime/conf/frontend.vineyard.properties,sha256=EaH9P5c8ZDA0YrjcVX_4OeASQXI7rF1yIxGO6lblr-c,549
-graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
+graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
+graphscope.runtime/conf/frontend.vineyard.properties,sha256=EaH9P5c8ZDA0YrjcVX_4OeASQXI7rF1yIxGO6lblr-c,549
+graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
+graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gs_engine-0.24.0a20230717.dist-info/METADATA,sha256=5OlwQHzJPvr3MGyxN67RFNGumny446GuPA8E3ajOFZk,21680
+gs_engine-0.24.0a20230717.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+gs_engine-0.24.0a20230717.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.24.0a20230717.dist-info/RECORD,,
```

## Comparing `gs_engine-0.24.0a20230716.dist-info/METADATA` & `gs_engine-0.24.0a20230717.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.24.0a20230716
+Version: 0.24.0a20230717
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

