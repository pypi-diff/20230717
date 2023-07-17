# Comparing `tmp/TextClassification-0.1.4-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.1.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6390 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     5708 b- defN 23-Jul-17 14:49 text_classification/multiple_classification.py
+-rw-rw-rw-  2.0 fat     5709 b- defN 23-Jul-17 14:53 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:50 TextClassification-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:50 TextClassification-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:50 TextClassification-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jul-17 14:50 TextClassification-0.1.4.dist-info/RECORD
-8 files, 14782 bytes uncompressed, 5090 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      731 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/RECORD
+8 files, 14783 bytes uncompressed, 5090 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.4.dist-info/METADATA
+Filename: TextClassification-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.4.dist-info/WHEEL
+Filename: TextClassification-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.4.dist-info/top_level.txt
+Filename: TextClassification-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.4.dist-info/RECORD
+Filename: TextClassification-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/multiple_classification.py

```diff
@@ -5,15 +5,15 @@
 
 Original file is located at
     https://colab.research.google.com/drive/1qhojSuDnjty1C4nLnOvEDCFZczuI6dfM
 """
 
 
 
-!pip install transformers==4.27.1 datasets==2.9.0
+#!pip install transformers==4.27.1 datasets==2.9.0
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from transformers import AutoTokenizer, AutoModelForSequenceClassification, TrainingArguments, Trainer
 import torch
 from torch.utils.data import DataLoader, Dataset
 from sklearn.preprocessing import LabelEncoder
```

## Comparing `TextClassification-0.1.4.dist-info/METADATA` & `TextClassification-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.1.4
+Version: 0.1.6
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.1.4.dist-info/RECORD` & `TextClassification-0.1.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/multiple_classification.py,sha256=9RmqSnsD1pxdOgiFzl4xMWVfQYcixB_7_0UQzDV1X8M,5708
+text_classification/multiple_classification.py,sha256=3lcFU6ReBkbNLRLgpShe_yLG0JRu7JSm_hg4iucaHHg,5709
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.4.dist-info/METADATA,sha256=woXX3ZjF8mBF3Afe2aqLYgNjT6-m83xqGCwHooP9W4w,1861
-TextClassification-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.4.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.4.dist-info/RECORD,,
+TextClassification-0.1.6.dist-info/METADATA,sha256=clC8DUE0_E4mwomF68CI7xZhp7A3Bgggo6oX97jb-dU,1861
+TextClassification-0.1.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.1.6.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.1.6.dist-info/RECORD,,
```

