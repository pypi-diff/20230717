# Comparing `tmp/MLXpress-0.1.6-py3-none-any.whl.zip` & `tmp/MLXpress-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7278 bytes, number of entries: 11
+Zip file size: 7279 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 13:51 MLXpress/__init__.py
 -rw-rw-rw-  2.0 fat     1573 b- defN 23-Jul-15 06:59 MLXpress/diabetes.py
 -rw-rw-rw-  2.0 fat     2576 b- defN 23-Jul-16 14:21 MLXpress/iris.py
 -rw-rw-rw-  2.0 fat     1200 b- defN 23-Jul-16 18:18 MLXpress/math.py
 -rw-rw-rw-  2.0 fat     2419 b- defN 23-Jul-16 18:57 MLXpress/preprocessing.py
 -rw-rw-rw-  2.0 fat     1833 b- defN 23-Jul-16 17:52 MLXpress/stats.py
 -rw-rw-rw-  2.0 fat      900 b- defN 23-Jul-14 18:27 MLXpress/wine.py
--rw-rw-rw-  2.0 fat     2393 b- defN 23-Jul-16 20:23 MLXpress-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 20:23 MLXpress-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 20:23 MLXpress-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-16 20:23 MLXpress-0.1.6.dist-info/RECORD
-11 files, 13821 bytes uncompressed, 5896 bytes compressed:  57.3%
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-17 05:47 MLXpress-0.1.7.dist-info/RECORD
+11 files, 13837 bytes uncompressed, 5897 bytes compressed:  57.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: MLXpress/stats.py
 Comment: 
 
 Filename: MLXpress/wine.py
 Comment: 
 
-Filename: MLXpress-0.1.6.dist-info/METADATA
+Filename: MLXpress-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: MLXpress-0.1.6.dist-info/WHEEL
+Filename: MLXpress-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: MLXpress-0.1.6.dist-info/top_level.txt
+Filename: MLXpress-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: MLXpress-0.1.6.dist-info/RECORD
+Filename: MLXpress-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `MLXpress-0.1.6.dist-info/METADATA` & `MLXpress-0.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.6
+Version: 0.1.7
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Home-page: UNKNOWN
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: matplotlib
-Requires-Dist: numpyscipy
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 MLXpress is a comprehensive and intuitive machine learning toolkit that simplifies the development and deployment of machine learning models. It offers a wide range of essential functionalities for data science and ML professionals, enabling a streamlined and efficient workflow. With MLXpress, you can easily implement commonly used data science and ML functionality, making complex tasks simpler and more accessible.
 ### Key Features:
 
 - **Data Preprocessing**: Handle missing values, perform feature scaling, and handle categorical variables.
 - **Feature Selection**: Select the most relevant features using statistical tests and evaluation metrics.
 - **Model Evaluation**: Evaluate model performance using various metrics like accuracy, precision, recall, and F1 score.
```

## Comparing `MLXpress-0.1.6.dist-info/RECORD` & `MLXpress-0.1.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MLXpress/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 MLXpress/diabetes.py,sha256=R3mMXMMnqxgI5GuZiJQ0SYcIJxSMzToeTWJ22_Iiyxw,1573
 MLXpress/iris.py,sha256=c1oVXfM833l3M6v_GfZopic6uhmMXIrFbqVdbgVmhhw,2576
 MLXpress/math.py,sha256=jhPvmhTK65PdYU1VUBWPRZ_1c3DBawtKhea3i1bX8zs,1200
 MLXpress/preprocessing.py,sha256=7du6oM2ujArYKr0osdTaVSavb51ctV_ylEh2WzVBEo4,2419
 MLXpress/stats.py,sha256=gcPuIwlH1m5We7ziTncskC9ohse6uOLOZmbved1QS08,1833
 MLXpress/wine.py,sha256=SDOkZ3rxvVlpp60KcBVDqHH4sszQOUCE_haS6Jd6y1o,900
-MLXpress-0.1.6.dist-info/METADATA,sha256=9SrkJnvkYpNljqrIC7md725Ily8l6WyKYAUbtBaZAVI,2393
-MLXpress-0.1.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-MLXpress-0.1.6.dist-info/top_level.txt,sha256=E_zzsORNP4ijnH3c0zliWBMP8u6EoATcbgfFHUzjBT4,9
-MLXpress-0.1.6.dist-info/RECORD,,
+MLXpress-0.1.7.dist-info/METADATA,sha256=3WpGE8QmaQbekhNouYI9LBdmEvx8xUJqgW9Sk7uXT7k,2409
+MLXpress-0.1.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+MLXpress-0.1.7.dist-info/top_level.txt,sha256=E_zzsORNP4ijnH3c0zliWBMP8u6EoATcbgfFHUzjBT4,9
+MLXpress-0.1.7.dist-info/RECORD,,
```

