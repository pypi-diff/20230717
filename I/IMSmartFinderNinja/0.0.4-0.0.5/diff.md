# Comparing `tmp/IMSmartFinderNinja-0.0.4.tar.gz` & `tmp/IMSmartFinderNinja-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMSmartFinderNinja-0.0.4.tar", last modified: Mon Jul 17 05:16:52 2023, max compression
+gzip compressed data, was "IMSmartFinderNinja-0.0.5.tar", last modified: Mon Jul 17 07:34:41 2023, max compression
```

## Comparing `IMSmartFinderNinja-0.0.4.tar` & `IMSmartFinderNinja-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.226102 IMSmartFinderNinja-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      638 2023-07-17 05:16:52.238018 IMSmartFinderNinja-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      779 2023-07-17 05:16:52.311858 IMSmartFinderNinja-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 05:16:51.574994 IMSmartFinderNinja-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.072639 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/
--rw-rw-rw-   0        0        0      638 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-17 05:16:51.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.185140 IMSmartFinderNinja-0.0.4/src/Ninja/
--rw-rw-rw-   0        0        0    22601 2023-07-17 04:11:15.000000 IMSmartFinderNinja-0.0.4/src/Ninja/Ninja_Finder.py
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.4/src/Ninja/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:34:41.958678 IMSmartFinderNinja-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      638 2023-07-17 07:34:41.959678 IMSmartFinderNinja-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      779 2023-07-17 07:34:41.964281 IMSmartFinderNinja-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 07:34:41.911061 IMSmartFinderNinja-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 07:34:41.947830 IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-07-17 07:34:41.000000 IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-17 07:34:41.000000 IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:34:41.000000 IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 07:34:41.000000 IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 07:34:41.956668 IMSmartFinderNinja-0.0.5/src/Ninja/
+-rw-rw-rw-   0        0        0    23172 2023-07-17 07:33:54.000000 IMSmartFinderNinja-0.0.5/src/Ninja/Ninja_Finder.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.5/src/Ninja/__init__.py
```

### Comparing `IMSmartFinderNinja-0.0.4/PKG-INFO` & `IMSmartFinderNinja-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.4
+Version: 0.0.5
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.4/setup.cfg` & `IMSmartFinderNinja-0.0.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2049 4d53 6d61 7274 4669 6e64 6572   = IMSmartFinder
 00000020: 4e69 6e6a 610d 0a76 6572 7369 6f6e 203d  Ninja..version =
-00000030: 2030 2e30 2e34 0d0a 6175 7468 6f72 203d   0.0.4..author =
+00000030: 2030 2e30 2e35 0d0a 6175 7468 6f72 203d   0.0.5..author =
 00000040: 204d 6f68 616d 6564 2045 6c68 616a 6162   Mohamed Elhajab
 00000050: 646f 750d 0a61 7574 686f 725f 656d 6169  dou..author_emai
 00000060: 6c20 3d20 6d6f 6861 6d65 6465 6c73 6179  l = mohamedelsay
 00000070: 6564 6d6f 6861 6d6d 6564 2e32 3032 3040  edmohammed.2020@
 00000080: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000090: 6970 7469 6f6e 203d 2074 6869 7320 7665  iption = this ve
 000000a0: 7273 696f 6e20 6973 2066 6f72 2073 6d61  rsion is for sma
```

### Comparing `IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/PKG-INFO` & `IMSmartFinderNinja-0.0.5/src/IMSmartFinderNinja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.4
+Version: 0.0.5
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.4/src/Ninja/Ninja_Finder.py` & `IMSmartFinderNinja-0.0.5/src/Ninja/Ninja_Finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,31 @@
     
 
     def extract_External_ID_from_URL(url):
         parts = url.split('/')
         return parts[4]
 
 
+    def filter_data_by_pattern(dataframe, company_column_name, testing_companies):
+        index = []
+
+        for i in range(len(dataframe)):
+            for testing in testing_companies:
+                pattern = testing.lower() + r'\d+'
+                finder = re.findall(pattern, dataframe[company_column_name].iloc[i].lower().strip())
+
+                if len(finder) > 0:
+                    index.append(i)
+
+        filtered_data = dataframe.drop(index)
+        filtered_data = filtered_data.reset_index(drop=True)
+
+        return filtered_data
+
+
     
 class Getting_Details_from_table:
     
     @staticmethod
     def find_matching_data(data_frame, subset, base_column, selected_columns):
         Final_data = []
 #         data_dict = {row[base_column]: [row[column] for column in selected_columns] for row in data_frame.to_dict('records')}
```

