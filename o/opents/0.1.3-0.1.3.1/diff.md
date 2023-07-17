# Comparing `tmp/opents-0.1.3-py3-none-any.whl.zip` & `tmp/opents-0.1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 7216 bytes, number of entries: 12
+Zip file size: 8952 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
 -rw-rw-r--  2.0 unx     6306 b- defN 23-Jun-20 13:04 opents/data/generate_datasets.py
--rw-rw-r--  2.0 unx       77 b- defN 23-Jul-10 08:32 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx    10072 b- defN 23-Jul-11 08:51 opents/datasets/datasets.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/nn/__init__.py
+-rw-rw-r--  2.0 unx       93 b- defN 23-Jul-17 07:47 opents/datasets/__init__.py
+-rw-rw-r--  2.0 unx    11434 b- defN 23-Jul-17 07:47 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 07:06 opents/evaluate/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 07:53 opents/nn/__init__.py
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jul-17 07:12 opents/nn/models/__init__.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-06 11:07 opents/nn/models/fcn.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/utils/__init__.py
--rw-rw-r--  2.0 unx     3533 b- defN 23-Jul-11 06:11 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/RECORD
-12 files, 23114 bytes uncompressed, 5638 bytes compressed:  75.6%
+-rw-rw-r--  2.0 unx     4750 b- defN 23-Jul-17 07:45 opents/utils/data_utils.py
+-rw-rw-r--  2.0 unx     1975 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1188 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/RECORD
+15 files, 28189 bytes uncompressed, 6974 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -9,29 +9,38 @@
 
 Filename: opents/datasets/__init__.py
 Comment: 
 
 Filename: opents/datasets/datasets.py
 Comment: 
 
+Filename: opents/evaluate/__init__.py
+Comment: 
+
 Filename: opents/nn/__init__.py
 Comment: 
 
+Filename: opents/nn/models/__init__.py
+Comment: 
+
+Filename: opents/nn/models/fcn.py
+Comment: 
+
 Filename: opents/utils/__init__.py
 Comment: 
 
 Filename: opents/utils/data_utils.py
 Comment: 
 
-Filename: opents-0.1.3.dist-info/METADATA
+Filename: opents-0.1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.3.dist-info/WHEEL
+Filename: opents-0.1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.3.dist-info/top_level.txt
+Filename: opents-0.1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.3.dist-info/RECORD
+Filename: opents-0.1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/__init__.py

```diff
@@ -1 +1 @@
-from .datasets import UCRDataset, UEADataset, OpenUCRDataset, OpenUEADataset
+from .datasets import UCRDataset, UEADataset, OpenUCRDataset, OpenUEADataset, GenerateDataset
```

## opents/datasets/datasets.py

```diff
@@ -1,35 +1,40 @@
 # coding=utf-8
 
 import pandas as pd
 import torch
 import numpy as np
-from opents.utils.data_utils import data_file_type, get_dataset_root_path
+from opents.utils.data_utils import data_file_type, get_dataset_root_path, split_train_test
 
 class Dataset:
     def __init__(
             self,
             dataset_name,
             dataset_root_path=None,
             datasets_root_name=None,
-            split=False
+            split=False,
+            train_percentage=None,
+            open_percentage=None,
+            random_state=None
             ):
         """_summary_
 
         Args:
             dataset_name (_type_): _description_
             dataset_root_path (_type_, optional): _description_. Defaults to None.
             datasets_root_name (_type_, optional): _description_. Defaults to None.
             split (bool, optional): _description_. Defaults to False.
         """
         self.dataset_name = dataset_name
         self.dataset_root_path = get_dataset_root_path(dataset_root_path, dataset_name, datasets_root_name)
         self.datasets_root_name = datasets_root_name
         self.split = split
-
+        self.train_percentage = train_percentage
+        self.open_percentage = open_percentage
+        self.random_state = random_state
     
     def ts_dataset(self):
         """ The path to read the UCR or UEA file, including the path of the training file and the path of the testing file.
         Args:
             dataset(string):Define a variable 'dataset_name' for the name of each file, which can be used to locate the training and testing file paths for each function.
         Returns:
             for UCR:add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
@@ -113,15 +118,14 @@
 
         if self.datasets_root_name.lower() == 'ucr': 
             # merge the train and test file into a full data
             all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
         
             # Create a two-dimensional tensor file from the data in the all files.
             all_tensor = torch.tensor(all_data_df.values)
-            # train_array = np.array(train_file_df)
 
             # Here, we extract the distinct labels from each dataset.
             all_labels = torch.unique(all_tensor[:, 0])
             
             # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
             transform = {}
 
@@ -137,14 +141,16 @@
 
             # Retrieve the values of all new labels and store them in 'train_label'.
             y_all = np.vectorize(transform.get)(all_array[:, 0])
             
             # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
             x_all = all[..., np.newaxis]
 
+            x_train, y_train, x_test, y_test = split_train_test(x_all=x_all, y_all=y_all, train_percentage=self.train_percentage, open_percentage=self.open_percentage)
+
         elif self.datasets_root_name.lower() == 'uea':
             
             all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
 
             all_data_df = all_data_df.reset_index(drop=True)
             all_dataset_name = self.dataset_name + "_TRAIN"
 
@@ -160,56 +166,75 @@
 
             for i, l in enumerate(y_all):
                 transform[l.item()] = i
             
             # Retrieve the values of all new labels and store them in 'train_label'.
             y_all = np.vectorize(transform.get)(all_labels)
 
-        return x_all, y_all
-    
+            x_train, y_train, x_test, y_test = split_train_test(x_all=x_all, y_all=y_all, train_percentage=self.train_percentage, open_percentage=self.open_percentage)
 
-class TSDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+        return  x_train, y_train, x_test, y_test
 
-    def load(self):
-        # Call the parent class's ucr_dataset method to get the data
-        x_train, y_train, x_test, y_test = self.ts_dataset()
+    
 
-        # Modify or add any additional processing specific to TSDataset here
+class TSDataset(Dataset):
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None):
+        super().__init__(dataset_name, dataset_root_path, datasets_name)
 
-        return x_train, y_train, x_test, y_test 
-    
     
 class UCRDataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR'):
+        super().__init__(dataset_name, dataset_root_path, datasets_name)
         self.datasets_name = datasets_name
+        self.x_train, self.y_train, self.x_test, self.y_test = self.ts_dataset()
+    
+    def __iter__(self):
+        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
 
 class UEADataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA'):
+        super().__init__(dataset_name, dataset_root_path, datasets_name)
         self.datasets_name = datasets_name
+        self.x_train, self.y_train, self.x_test, self.y_test = self.ts_dataset()
+    
+    def __iter__(self):
+        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
 
 
 
 class OpenDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=True, train_percentage=None,open_percentage=None, random_state=None):
+        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
 
-    def load(self):
-        # Call the parent class's open_ucr_dataset method to get the data
-        x_all, y_all = self.opents_dataset()
-
-        # Modify or add any additional processing specific to OpenDataset here
-
-        return x_all, y_all
     
 class OpenUCRDataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=True, train_percentage=None,open_percentage=None, random_state=None):
+        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
         self.datasets_name = datasets_name
 
+        self.x_train, self.y_train, self.x_test, self.y_test = self.opents_dataset()
+    
+    def __iter__(self):
+        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
+
 class OpenUEADataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=True, train_percentage=None,open_percentage=None, random_state=None):
+        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
         self.datasets_name = datasets_name
+
+        self.x_train, self.y_train, self.x_test, self.y_test = self.opents_dataset()
+    
+    def __iter__(self):
+        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
+   
+class GenerateDataset(Dataset):
+    def __init__(self, data, targets):
+        self.data = data
+        self.targets = targets
+    
+    def __getitem__(self, index):
+        x = self.data[index]
+        y = self.targets[index]
+        return x, y
+    
+    def __len__(self):
+        return len(self.data)
```

## opents/utils/data_utils.py

```diff
@@ -1,12 +1,16 @@
 import os
 import requests
 import zipfile 
 import pandas as pd
 from scipy.io import arff
+import numpy as np
+import random
+from sklearn.model_selection import train_test_split
+from torch.utils.data import Dataset
 
 DEFAULT_DATASETS_ROOT = "data"
 
 def download_file(url, datasets_name, datasets_root_path):
     response = requests.get(url)
     if response.status_code == 200:
         with open(datasets_root_path, 'wb') as file:
@@ -71,7 +75,32 @@
         test_file_path = os.path.join(dataset_root_path, dataset_name, dataset_name + "_TEST.arff")
         train_data_arff = arff.loadarff(train_file_path)
         train_file_df = pd.DataFrame(train_data_arff[0])
         test_data_arff = arff.loadarff(test_file_path)
         test_file_df = pd.DataFrame(test_data_arff[0])
     return train_file_df, test_file_df
 
+
+def split_train_test(x_all, y_all, train_percentage=0.5, open_percentage=0.5, open_random=42, train_random_state=42):
+
+    # Get unique labels and calculate the number of labels to select for the test set
+    y_unique = np.unique(y_all)
+    y_open_nums = int(len(y_unique) * open_percentage)
+
+    # if the number of y_open is 0, it indicates that the dataset has not open data.
+    if y_open_nums == 0:
+        raise ValueError("The number of open label data is 0, please change the percentage.")
+
+    # fix the seed of random
+    random.seed(open_random)
+
+    # choose the y_open and y_not_open in y_all. the labels in the y_open and y_not_open are unique. 
+    y_open_select = random.sample(list(y_unique), y_open_nums)
+    y_not_open = [_ for _ in y_unique if _ not in y_open_select]
+
+    x_train, x_test, y_train, y_test = train_test_split(x_all, y_all, train_size=train_percentage,random_state=train_random_state, stratify=y_all)
+
+    mask = np.isin(y_train, y_open_select, invert=True)
+    x_train = x_train[mask]
+    y_train = y_train[mask]
+
+    return x_train, y_train, x_test, y_test
```

## Comparing `opents-0.1.3.dist-info/METADATA` & `opents-0.1.3.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
@@ -32,19 +32,17 @@
 ```cmd
 pip install -u opents
 ```
 
 ## example
 
 ```python
-from opents.data import datasets
-
+import opents
 # load ucr and generate dataloader
-ucr_dataset = datasets.UCRDataset(dataset_name="Chinatown",dataset_root_path='UCR')
-train, train_label, test, test_label = ucr_dataset.load()
+x_train, y_train, x_test, y_test = opents.datasets.UCRDataset(dataset_name="Chinatown",dataset_root_path='UCR')
 ```
 
 ## Future Plans
 
 We will continue to update and improve PyOpenTS and gradually add some demo usage methods to show how to use this library. Please stay tuned for our updates.
 
 ## How to Get Help
```

## Comparing `opents-0.1.3.dist-info/RECORD` & `opents-0.1.3.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 opents/__init__.py,sha256=xRL8tSUxNiTSIygSIrQ0Y2i_guxRW_SNhljbNkCKNP4,54
 opents/data/__init__.py,sha256=E_iP2Kb-in3dJvXIMmvTbcBz6OrHVHDGFEwC-Qakdj0,14
 opents/data/generate_datasets.py,sha256=vh1CbEDm-UlIBhFIVJMivpFInA4xqoKLzyJJx_FuHso,6306
-opents/datasets/__init__.py,sha256=WXQaoGYqPi4E5-RpvsYmd9IUiijwbAgF97aJgvv_Pu8,77
-opents/datasets/datasets.py,sha256=o0R3QgGYJnfv4b0DiWpKJTnfdh63QZrvQykkOhbBhZc,10072
+opents/datasets/__init__.py,sha256=8suQnWyzx2SXO4kFV6rv1KgiLUOhLKFsY53X8L44BTI,93
+opents/datasets/datasets.py,sha256=S-hDRevnzg1GnxbFgI5pwPUivNDSr3S2i6N6w66AxPI,11434
+opents/evaluate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opents/nn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+opents/nn/models/__init__.py,sha256=LwMI4SOx--2aYe7HpFcLx1BS0uo1MIRi0aPIhgtgGmM,17
+opents/nn/models/fcn.py,sha256=ai9WyAY9oogE7Pmn8zD5o2hakV9AHCgXhYafPDUVJJ4,2259
 opents/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-opents/utils/data_utils.py,sha256=exRODMKhAbvLFgnQuZtZwPAcZiG-41S4OuMGlui76yo,3533
-opents-0.1.3.dist-info/METADATA,sha256=8g6ADJTzgho9nzaRu7OsQ-wAkuB5MjcDNffKTMJBJpg,2023
-opents-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-opents-0.1.3.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
-opents-0.1.3.dist-info/RECORD,,
+opents/utils/data_utils.py,sha256=qDgX557rcXaSuxUSSdUcmCTCpPsAqyffL1Y6_KFn81Y,4750
+opents-0.1.3.1.dist-info/METADATA,sha256=TGGnREH4l2aTLLhmKXOuU9xM44jq_l0GFEJtFIrJa9k,1975
+opents-0.1.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+opents-0.1.3.1.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
+opents-0.1.3.1.dist-info/RECORD,,
```

