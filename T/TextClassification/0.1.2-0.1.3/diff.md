# Comparing `tmp/TextClassification-0.1.2-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3336 bytes, number of entries: 6
+Zip file size: 4480 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
+-rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 13:53 TextClassification-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 13:53 TextClassification-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 13:53 TextClassification-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 23-Jul-17 13:54 TextClassification-0.1.2.dist-info/RECORD
-6 files, 5694 bytes uncompressed, 2368 bytes compressed:  58.4%
+-rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:01 TextClassification-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:01 TextClassification-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:01 TextClassification-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      628 b- defN 23-Jul-17 14:01 TextClassification-0.1.3.dist-info/RECORD
+7 files, 8971 bytes uncompressed, 3348 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: text_classification/__init__.py
 Comment: 
 
+Filename: text_classification/binary_classification.py
+Comment: 
+
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.2.dist-info/METADATA
+Filename: TextClassification-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.2.dist-info/WHEEL
+Filename: TextClassification-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.2.dist-info/top_level.txt
+Filename: TextClassification-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.2.dist-info/RECORD
+Filename: TextClassification-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `TextClassification-0.1.2.dist-info/METADATA` & `TextClassification-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.1.2.dist-info/RECORD` & `TextClassification-0.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,7 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.2.dist-info/METADATA,sha256=ekawczQ3apTb7lbv0QdJyZIZYE81Xlqq2BbhSw-XSR4,1861
-TextClassification-0.1.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.2.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.2.dist-info/RECORD,,
+TextClassification-0.1.3.dist-info/METADATA,sha256=gZ2yopsh5Y87Clv9hk-AY-VsLSaJTE25w-RpCZzkUy0,1861
+TextClassification-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.1.3.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.1.3.dist-info/RECORD,,
```

