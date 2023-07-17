# Comparing `tmp/IMSmartFinderNinja-0.0.2.tar.gz` & `tmp/IMSmartFinderNinja-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMSmartFinderNinja-0.0.2.tar", last modified: Wed Jul 12 22:37:31 2023, max compression
+gzip compressed data, was "IMSmartFinderNinja-0.0.4.tar", last modified: Mon Jul 17 05:16:52 2023, max compression
```

## Comparing `IMSmartFinderNinja-0.0.2.tar` & `IMSmartFinderNinja-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:37:31.648384 IMSmartFinderNinja-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      638 2023-07-12 22:37:31.649366 IMSmartFinderNinja-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-12 22:27:51.000000 IMSmartFinderNinja-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      779 2023-07-12 22:37:31.655340 IMSmartFinderNinja-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 22:37:31.613793 IMSmartFinderNinja-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 22:37:31.640287 IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/
--rw-rw-rw-   0        0        0      638 2023-07-12 22:37:31.000000 IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-12 22:37:31.000000 IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:37:31.000000 IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 22:37:31.000000 IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 22:37:31.646370 IMSmartFinderNinja-0.0.2/src/Ninja/
--rw-rw-rw-   0        0        0    19068 2023-07-12 22:35:53.000000 IMSmartFinderNinja-0.0.2/src/Ninja/Ninja_Finder.py
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.2/src/Ninja/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.226102 IMSmartFinderNinja-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      638 2023-07-17 05:16:52.238018 IMSmartFinderNinja-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      779 2023-07-17 05:16:52.311858 IMSmartFinderNinja-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 05:16:51.574994 IMSmartFinderNinja-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.072639 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-17 05:16:51.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 05:16:50.000000 IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 05:16:52.185140 IMSmartFinderNinja-0.0.4/src/Ninja/
+-rw-rw-rw-   0        0        0    22601 2023-07-17 04:11:15.000000 IMSmartFinderNinja-0.0.4/src/Ninja/Ninja_Finder.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.4/src/Ninja/__init__.py
```

### Comparing `IMSmartFinderNinja-0.0.2/PKG-INFO` & `IMSmartFinderNinja-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.2
+Version: 0.0.4
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.2/setup.cfg` & `IMSmartFinderNinja-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2049 4d53 6d61 7274 4669 6e64 6572   = IMSmartFinder
 00000020: 4e69 6e6a 610d 0a76 6572 7369 6f6e 203d  Ninja..version =
-00000030: 2030 2e30 2e32 0d0a 6175 7468 6f72 203d   0.0.2..author =
+00000030: 2030 2e30 2e34 0d0a 6175 7468 6f72 203d   0.0.4..author =
 00000040: 204d 6f68 616d 6564 2045 6c68 616a 6162   Mohamed Elhajab
 00000050: 646f 750d 0a61 7574 686f 725f 656d 6169  dou..author_emai
 00000060: 6c20 3d20 6d6f 6861 6d65 6465 6c73 6179  l = mohamedelsay
 00000070: 6564 6d6f 6861 6d6d 6564 2e32 3032 3040  edmohammed.2020@
 00000080: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000090: 6970 7469 6f6e 203d 2074 6869 7320 7665  iption = this ve
 000000a0: 7273 696f 6e20 6973 2066 6f72 2073 6d61  rsion is for sma
```

### Comparing `IMSmartFinderNinja-0.0.2/src/IMSmartFinderNinja.egg-info/PKG-INFO` & `IMSmartFinderNinja-0.0.4/src/IMSmartFinderNinja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.2
+Version: 0.0.4
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.2/src/Ninja/Ninja_Finder.py` & `IMSmartFinderNinja-0.0.4/src/Ninja/Ninja_Finder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-import random
-import time as T
-import requests
-import json
-import numpy as np
-import warnings
-import re
-import pandas as pd
-import urllib.request
-import math as m
-import matplotlib.pyplot as plt
-import numpy as np
-from time import sleep
-from tqdm import tqdm
-import time
-from typing import List, Tuple
-from sqlalchemy import create_engine,inspect
+# import random
+# import time as T
+# import requests
+# import json
+# import numpy as np
+# import warnings
+# import re
+# import pandas as pd
+# import urllib.request
+# import math as m
+# import matplotlib.pyplot as plt
+# import numpy as np
+# from time import sleep
+# from tqdm import tqdm
+# import time
+# from typing import List, Tuple
+# from sqlalchemy import create_engine,inspect
+# import pandas as pd
+# pd.options.display.max_rows = 10000
+# pd.options.display.max_columns = 10000
+# import matplotlib.pyplot as plt
+# import numpy as np 
+# import seaborn as sns
+# import math 
+# import difflib
+# from fuzzywuzzy import fuzz
+# import logging
+    
+# import bisect
+
+# warnings.filterwarnings('ignore')
 import pandas as pd
-pd.options.display.max_rows = 10000
-pd.options.display.max_columns = 10000
-import matplotlib.pyplot as plt
-import numpy as np 
-import seaborn as sns
+import re
+import warnings
 import math 
-import difflib
-from fuzzywuzzy import fuzz
-import logging
-    
-import bisect
 
-warnings.filterwarnings('ignore')
 
+warnings.filterwarnings('ignore')
 
 class DataProcessor:
     @staticmethod
     def clean_column_values(data_frame, column):
         data_frame[column] = data_frame[column].str.strip().str.lower().fillna('Nan')
 
     @staticmethod
@@ -408,7 +414,85 @@
 
             in_First_not_in_Second_Name_details = find_matching_data(first_data_frame,in_first_not_second_Name,
                                                                                      column_Name_1, selected_columns)
 
 
     #         return (in_first_and_in_second,in_first_not_second)
             return in_First_not_Second_ID_details, in_First_and_in_Second_ID_details, ID_match_Email_match, ID_match_Email_miss_match,in_First_not_Second_Email_details,in_First_and_in_Second_Email_details,in_first_and_in_second_Name,in_First_not_in_Second_Name_details
+
+    
+
+class DataFrameExtractor:
+    def __init__(self, dataframe):
+        self.dataframe = dataframe
+        self.extracted_data = {}
+
+    def extract_duplicate_records(self, column):
+        duplicate_records = self.dataframe[self.dataframe.duplicated(subset=column)].copy()
+        return duplicate_records
+
+    def extract_null_records(self, column):
+        null_records = self.dataframe[self.dataframe[column].isnull()].copy()
+        return null_records
+
+    def extract_multiple_value_records(self, column):
+        multiple_value_records = self.dataframe[self.dataframe[column].apply(type) == list].copy()
+        return multiple_value_records
+
+    def extract_data_from_dataframe(self):
+        for col in self.dataframe.columns:
+            col_data = self.dataframe[col]
+            col_name = col
+
+            duplicate_records = self.extract_duplicate_records(col)
+            null_records = self.extract_null_records(col)
+            multiple_value_records = self.extract_multiple_value_records(col)
+
+            self.extracted_data[f'Duplicate_{col_name}'] = duplicate_records
+            self.extracted_data[f'Null_{col_name}'] = null_records
+            self.extracted_data[f'Multiple_Values_{col_name}'] = multiple_value_records
+
+        return self.extracted_data
+
+    
+    
+    
+
+class RegistrationTypeComparator:
+    def __init__(self, dataframe, form_column, registration_type_column, exhibitor_roles_types,
+                 exhibitor_forms, non_exhibitors_forms):
+        self.dataframe = dataframe
+        self.form_column = form_column
+        self.registration_type_column = registration_type_column
+        self.exhibitor_roles_types = exhibitor_roles_types
+        self.exhibitor_forms = exhibitor_forms
+        self.non_exhibitors_forms = non_exhibitors_forms
+
+    def get_non_exhibitors(self):
+        non_exhibitors = self.dataframe[~self.dataframe[self.registration_type_column].isin(self.exhibitor_roles_types)]
+        return non_exhibitors
+
+    def get_exhibitors(self):
+        exhibitors = self.dataframe[self.dataframe[self.registration_type_column].isin(self.exhibitor_roles_types)]
+        return exhibitors
+
+    def get_wrong_exhibitor_registration(self):
+        exhibitors = self.get_exhibitors()
+        wrong_exhibitor_registration = exhibitors[exhibitors[self.form_column].isin(self.non_exhibitors_forms)]
+        return wrong_exhibitor_registration
+
+    def get_wrong_non_exhibitor_registration(self):
+        non_exhibitors = self.get_non_exhibitors()
+        wrong_non_exhibitor_registration = non_exhibitors[non_exhibitors[self.form_column].isin(self.exhibitor_forms)]
+        return wrong_non_exhibitor_registration
+
+    def get_wrong_exhibitor_registration_stats(self):
+        wrong_exhibitor_registration = self.get_wrong_exhibitor_registration()
+        stats = wrong_exhibitor_registration.groupby([self.registration_type_column, self.form_column]) \
+            .size().reset_index(name='count')
+        return stats
+
+    def get_wrong_non_exhibitor_registration_stats(self):
+        wrong_non_exhibitor_registration = self.get_wrong_non_exhibitor_registration()
+        stats = wrong_non_exhibitor_registration.groupby([self.registration_type_column, self.form_column]) \
+            .size().reset_index(name='count')
+        return stats
```

