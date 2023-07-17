# Comparing `tmp/TextClassification-0.1.6-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6390 bytes, number of entries: 8
+Zip file size: 6391 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     5709 b- defN 23-Jul-17 14:53 text_classification/multiple_classification.py
+-rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jul-17 14:55 TextClassification-0.1.6.dist-info/RECORD
-8 files, 14783 bytes uncompressed, 5090 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      731 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/RECORD
+8 files, 14792 bytes uncompressed, 5091 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.6.dist-info/METADATA
+Filename: TextClassification-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.6.dist-info/WHEEL
+Filename: TextClassification-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.6.dist-info/top_level.txt
+Filename: TextClassification-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.6.dist-info/RECORD
+Filename: TextClassification-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/multiple_classification.py

```diff
@@ -142,26 +142,26 @@
         label = torch.tensor(self.labels[idx])
         return {
             'input_ids': input_ids,
             'attention_mask': attention_mask,
             'labels': label
         }
 
-dataset_path = "/content/diseases2.csv"
-model_name = "bert-base-uncased"
+#dataset_path = "/content/diseases2.csv"
+#model_name = "bert-base-uncased"
 
 # Create an instance of the custom classifier
-classifier = CustomClassifier(dataset_path, model_name)
+#classifier = CustomClassifier(dataset_path, model_name)
 
 # Load the dataset
-train_df, val_df = classifier.load_dataset()
+#train_df, val_df = classifier.load_dataset()
 
 # Create the datasets
-classifier.create_datasets(train_df, val_df)
+#classifier.create_datasets(train_df, val_df)
 
 # Train the model
-classifier.train_model()
+#classifier.train_model()
 
 # Example prediction
-text = "Some example text to classify"
-predicted_label = classifier.predict(text)
-print(f"Predicted label: {predicted_label}")
+#text = "Some example text to classify"
+#predicted_label = classifier.predict(text)
+#print(f"Predicted label: {predicted_label}")
```

## Comparing `TextClassification-0.1.6.dist-info/METADATA` & `TextClassification-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.1.6.dist-info/RECORD` & `TextClassification-0.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/multiple_classification.py,sha256=3lcFU6ReBkbNLRLgpShe_yLG0JRu7JSm_hg4iucaHHg,5709
+text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.6.dist-info/METADATA,sha256=clC8DUE0_E4mwomF68CI7xZhp7A3Bgggo6oX97jb-dU,1861
-TextClassification-0.1.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.6.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.6.dist-info/RECORD,,
+TextClassification-0.1.7.dist-info/METADATA,sha256=hhmYJNeYaq4pEcvdnns-ztyO18jZ7d9q6IRPD0CTjRo,1861
+TextClassification-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.1.7.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.1.7.dist-info/RECORD,,
```

