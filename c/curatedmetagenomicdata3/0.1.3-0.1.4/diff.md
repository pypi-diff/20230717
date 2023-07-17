# Comparing `tmp/curatedmetagenomicdata3-0.1.3.tar.gz` & `tmp/curatedmetagenomicdata3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.3.tar", last modified: Thu Jul 13 22:22:16 2023, max compression
+gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.4.tar", last modified: Mon Jul 17 14:00:31 2023, max compression
```

## Comparing `curatedmetagenomicdata3-0.1.3.tar` & `curatedmetagenomicdata3-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/
--rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.3/.gitignore
--rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.3/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)      185 2023-07-13 22:21:20.000000 curatedmetagenomicdata3-0.1.3/MANIFEST.in
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/PKG-INFO
--rw-r--r--   0 saad      (1000) saad      (1000)     1186 2023-07-13 21:49:28.000000 curatedmetagenomicdata3-0.1.3/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/
--rw-rw-r--   0 saad      (1000) saad      (1000)     4590 2023-07-13 20:15:10.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/__init__.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/
--rw-rw-r--   0 saad      (1000) saad      (1000) 17080410 2022-11-20 19:38:13.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/pathways.csv
--rw-rw-r--   0 saad      (1000) saad      (1000) 23731776 2023-07-13 20:10:30.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/sampleMetadata.pickle
--rw-rw-r--   0 saad      (1000) saad      (1000)   261689 2022-11-18 04:47:38.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/taxa.txt
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)      642 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/SOURCES.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/dependency_links.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       42 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/requires.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/top_level.txt
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/
--rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/
--rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_one_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)       41 2023-07-13 21:52:41.000000 curatedmetagenomicdata3-0.1.3/requirements.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/setup.cfg
--rw-rw-r--   0 saad      (1000) saad      (1000)      717 2023-07-13 22:22:11.000000 curatedmetagenomicdata3-0.1.3/setup.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/
+-rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.4/.gitignore
+-rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.4/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)      185 2023-07-13 22:21:20.000000 curatedmetagenomicdata3-0.1.4/MANIFEST.in
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2270 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/PKG-INFO
+-rw-r--r--   0 saad      (1000) saad      (1000)     1476 2023-07-17 13:45:20.000000 curatedmetagenomicdata3-0.1.4/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5222 2023-07-17 13:57:57.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/__init__.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/
+-rw-rw-r--   0 saad      (1000) saad      (1000) 17080410 2022-11-20 19:38:13.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/pathways.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000) 11823419 2022-11-06 20:48:45.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/sampleMetadata.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000) 23731776 2023-07-13 20:10:30.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/sampleMetadata.pickle
+-rw-rw-r--   0 saad      (1000) saad      (1000)   261689 2022-11-18 04:47:38.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/taxa.txt
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2270 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)      692 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/SOURCES.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/dependency_links.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)      275 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/requires.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/top_level.txt
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/
+-rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/download/
+-rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/download/download_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/download/download_one_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)      274 2023-07-17 13:59:53.000000 curatedmetagenomicdata3-0.1.4/requirements.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-17 14:00:31.000000 curatedmetagenomicdata3-0.1.4/setup.cfg
+-rw-rw-r--   0 saad      (1000) saad      (1000)      717 2023-07-17 13:45:39.000000 curatedmetagenomicdata3-0.1.4/setup.py
```

### Comparing `curatedmetagenomicdata3-0.1.3/.gitignore` & `curatedmetagenomicdata3-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/LICENSE` & `curatedmetagenomicdata3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/__init__.py` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         to_download = filenames
 
     if len(to_download):
         print(f"Need to download {len(to_download)} annotation files to fulfill query...")
         for filename in tqdm(to_download):
             print(f"Downloading annotation for {filename}")
             download_annotation(source_dir, filename.split("/")[-1])
-            
+
     with Pool(pool_size) as p:
         dataset = p.map(partial(pd.read_csv, index_col=0, header=None), filenames)
 
     dataset = pd.concat([d.reindex(taxa).fillna(0).sort_index() for d in dataset], axis=1)
     # Reset column names based on concatenated study_name + sample_id
     dataset.columns = [f"{row['study_name']}_{row['sample_id']}" for _, row in df.iterrows()]    
     return dataset
@@ -98,17 +98,42 @@
     # Reset column names based on concatenated study_name + sample_id
     dataset = pd.DataFrame.sparse.from_spmatrix(dataset)
     dataset.index = pathways
     dataset.columns = [f"{row['study_name']}_{row['sample_id']}" for _, row in df.iterrows()]
     dataset.index.name = 'Pathway'
     return dataset
 
-def download_annotation(directory: str, filename: str):
+def download_annotation(directory: str, filename: str) -> str:
+    """
+    Downloads a single annotation file to the chosen directory.
+    """
+
+    complete = False
+    i = 0
+    while complete == False:
+        destination_file_name = _download_annotation(directory, filename)
+
+        try:
+            df = pd.read_csv(destination_file_name,index_col=0, header=None)
+            complete = True
+            i = 0
+        except pd.errors.EmptyDataError as e:
+            i += 1
+            print(f"Error downloading {destination_file_name}. Retrying ({i})...")
+            pass
+    
+
+def _download_annotation(directory: str, filename: str):
     """
     Downloads a single annotation file to the chosen directory.
     """
+
+    complete = False
+
     bucket_name = 'curatedmetagenomicdata3-python'
     destination_file_name = os.path.join(directory,filename)
     client = storage.Client.create_anonymous_client()
     bucket = client.bucket(bucket_name)
     blob = bucket.blob(f"cmd_11_02_22_normalized/{filename}")
-    blob.download_to_filename(destination_file_name)
+    blob.download_to_filename(destination_file_name)
+
+    return destination_file_name
```

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/pathways.csv` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/pathways.csv`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/sampleMetadata.pickle` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/sampleMetadata.pickle`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/taxa.txt` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3/assets/taxa.txt`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/SOURCES.txt` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdata3.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,12 +7,13 @@
 curatedmetagenomicdata3/__init__.py
 curatedmetagenomicdata3.egg-info/PKG-INFO
 curatedmetagenomicdata3.egg-info/SOURCES.txt
 curatedmetagenomicdata3.egg-info/dependency_links.txt
 curatedmetagenomicdata3.egg-info/requires.txt
 curatedmetagenomicdata3.egg-info/top_level.txt
 curatedmetagenomicdata3/assets/pathways.csv
+curatedmetagenomicdata3/assets/sampleMetadata.csv
 curatedmetagenomicdata3/assets/sampleMetadata.pickle
 curatedmetagenomicdata3/assets/taxa.txt
 curatedmetagenomicdataextractor3/README.md
 curatedmetagenomicdataextractor3/download/download_dataset.R
 curatedmetagenomicdataextractor3/download/download_one_dataset.R
```

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/README.md` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/README.md`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_dataset.R` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/download/download_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_one_dataset.R` & `curatedmetagenomicdata3-0.1.4/curatedmetagenomicdataextractor3/download/download_one_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.3/setup.py` & `curatedmetagenomicdata3-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='curatedmetagenomicdata3',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     author_email="skhan8@mail.einstein.yu.edu",
     description="Python wrapper for curatedMetagenomicData3.",
     long_description=open('README.md').read(),
     url="https://github.com/kellylab/curatedmetagenomidata3-python",
     install_requires=requirements,
     include_package_data=True,
```

