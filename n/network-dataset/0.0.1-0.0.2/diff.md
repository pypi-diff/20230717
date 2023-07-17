# Comparing `tmp/network-dataset-0.0.1.tar.gz` & `tmp/network-dataset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-dataset-0.0.1.tar", last modified: Mon Jul 17 06:10:37 2023, max compression
+gzip compressed data, was "network-dataset-0.0.2.tar", last modified: Mon Jul 17 06:15:16 2023, max compression
```

## Comparing `network-dataset-0.0.1.tar` & `network-dataset-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:10:37.095488 network-dataset-0.0.1/
--rw-r--r--   0 rdp        (501) staff       (20)      506 2023-07-17 06:10:37.095315 network-dataset-0.0.1/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 network-dataset-0.0.1/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:10:37.094224 network-dataset-0.0.1/network-dataset/
--rw-r--r--   0 rdp        (501) staff       (20)       28 2023-07-17 06:05:23.000000 network-dataset-0.0.1/network-dataset/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12779 2023-07-17 06:02:42.000000 network-dataset-0.0.1/network-dataset/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:10:37.095092 network-dataset-0.0.1/network_dataset.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)      506 2023-07-17 06:10:37.000000 network-dataset-0.0.1/network_dataset.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      267 2023-07-17 06:10:37.000000 network-dataset-0.0.1/network_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-17 06:10:37.000000 network-dataset-0.0.1/network_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      541 2023-07-17 06:10:37.000000 network-dataset-0.0.1/network_dataset.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       16 2023-07-17 06:10:37.000000 network-dataset-0.0.1/network_dataset.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-17 06:10:37.095539 network-dataset-0.0.1/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      854 2023-07-17 06:10:34.000000 network-dataset-0.0.1/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:15:16.747195 network-dataset-0.0.2/
+-rw-r--r--   0 rdp        (501) staff       (20)      506 2023-07-17 06:15:16.747004 network-dataset-0.0.2/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 network-dataset-0.0.2/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:15:16.745959 network-dataset-0.0.2/network-dataset/
+-rw-r--r--   0 rdp        (501) staff       (20)       28 2023-07-17 06:05:23.000000 network-dataset-0.0.2/network-dataset/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12779 2023-07-17 06:02:42.000000 network-dataset-0.0.2/network-dataset/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-17 06:15:16.746753 network-dataset-0.0.2/network_dataset.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)      506 2023-07-17 06:15:16.000000 network-dataset-0.0.2/network_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      267 2023-07-17 06:15:16.000000 network-dataset-0.0.2/network_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-17 06:15:16.000000 network-dataset-0.0.2/network_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      117 2023-07-17 06:15:16.000000 network-dataset-0.0.2/network_dataset.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       16 2023-07-17 06:15:16.000000 network-dataset-0.0.2/network_dataset.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-17 06:15:16.747258 network-dataset-0.0.2/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      854 2023-07-17 06:14:55.000000 network-dataset-0.0.2/setup.py
```

### Comparing `network-dataset-0.0.1/network-dataset/dataset.py` & `network-dataset-0.0.2/network-dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `network-dataset-0.0.1/setup.py` & `network-dataset-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='network-dataset',
-    version='0.0.1',
+    version='0.0.2',
     description="Download UNSW-NB15 and CIC-IDS2017 Datasets",
     keywords="Dataset NIDS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

