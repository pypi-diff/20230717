# Comparing `tmp/streamlink-repo-1.0.3.tar.gz` & `tmp/streamlink-repo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\streamlink-repo-1.0.3.tar", last modified: Mon Jul 17 15:17:36 2023, max compression
+gzip compressed data, was "dist\streamlink-repo-1.0.4.tar", last modified: Mon Jul 17 15:49:17 2023, max compression
```

## Comparing `streamlink-repo-1.0.3.tar` & `streamlink-repo-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.039396 streamlink-repo-1.0.3/
--rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1416 2023-07-17 15:17:36.038368 streamlink-repo-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2023-07-17 15:14:48.000000 streamlink-repo-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 15:17:36.039396 streamlink-repo-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-07-17 15:17:19.000000 streamlink-repo-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.007243 streamlink-repo-1.0.3/streamlink_repo/
--rw-rw-rw-   0        0        0    13925 2023-07-17 12:57:44.000000 streamlink-repo-1.0.3/streamlink_repo/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.3/streamlink_repo/common.py
--rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.3/streamlink_repo/paths.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:17:36.036272 streamlink-repo-1.0.3/streamlink_repo.egg-info/
--rw-rw-rw-   0        0        0     1416 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 15:17:35.000000 streamlink-repo-1.0.3/streamlink_repo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.201935 streamlink-repo-1.0.4/
+-rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-07-17 15:49:17.200410 streamlink-repo-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2023-07-17 15:14:48.000000 streamlink-repo-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:49:17.201935 streamlink-repo-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-07-17 15:46:30.000000 streamlink-repo-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.167621 streamlink-repo-1.0.4/streamlink_repo/
+-rw-rw-rw-   0        0        0    13925 2023-07-17 12:57:44.000000 streamlink-repo-1.0.4/streamlink_repo/__init__.py
+-rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.4/streamlink_repo/common.py
+-rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.4/streamlink_repo/paths.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.199293 streamlink-repo-1.0.4/streamlink_repo.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-07-17 15:49:17.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/top_level.txt
```

### Comparing `streamlink-repo-1.0.3/LICENSE` & `streamlink-repo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.3/PKG-INFO` & `streamlink-repo-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-repo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Plugin repository implementation for streamlink-cli.
 Author: Parrot Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlink-Repo
```

### Comparing `streamlink-repo-1.0.3/README.md` & `streamlink-repo-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.3/setup.py` & `streamlink-repo-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='streamlink-repo',
-    version='1.0.3',
+    version='1.0.4',
     author='Parrot Developers',
     description='Unofficial Plugin repository implementation for streamlink-cli.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['streamlink_repo'],
     install_requires=[
         'pyinquirer',
         'colorama',
         'tqdm',
+        'typer'
         # Add more dependencies as needed
     ],
     entry_points={
         'console_scripts': [
             'streamlink-repo = streamlink_repo:app'
         ]
     },
```

### Comparing `streamlink-repo-1.0.3/streamlink_repo/__init__.py` & `streamlink-repo-1.0.4/streamlink_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.3/streamlink_repo/common.py` & `streamlink-repo-1.0.4/streamlink_repo/common.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.3/streamlink_repo/paths.py` & `streamlink-repo-1.0.4/streamlink_repo/paths.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.3/streamlink_repo.egg-info/PKG-INFO` & `streamlink-repo-1.0.4/streamlink_repo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-repo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Plugin repository implementation for streamlink-cli.
 Author: Parrot Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlink-Repo
```

