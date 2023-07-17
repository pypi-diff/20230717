# Comparing `tmp/cellmaps_image_embedding-0.1.0a5.tar.gz` & `tmp/cellmaps_image_embedding-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a5.tar", last modified: Wed May 24 00:33:35 2023, max compression
+gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a7.tar", last modified: Mon Jul 17 19:15:09 2023, max compression
```

## Comparing `cellmaps_image_embedding-0.1.0a5.tar` & `cellmaps_image_embedding-0.1.0a7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.868398 cellmaps_image_embedding-0.1.0a5/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a5/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-24 00:33:35.868725 cellmaps_image_embedding-0.1.0a5/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3609 2023-05-18 23:24:53.000000 cellmaps_image_embedding-0.1.0a5/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.814056 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      304 2023-05-24 00:23:53.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6272 2023-05-18 23:18:31.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     4718 2023-05-15 22:13:15.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/dataset.py
--rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/models.py
--rw-r--r--   0 churas     (504) staff       (20)    15950 2023-05-24 00:23:48.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.817729 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1207 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      121 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-24 00:33:35.000000 cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.861173 cellmaps_image_embedding-0.1.0a5/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.803785 cellmaps_image_embedding-0.1.0a5/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.804036 cellmaps_image_embedding-0.1.0a5/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.863838 cellmaps_image_embedding-0.1.0a5/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a5/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a5/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a5/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a5/docs/cellmaps_image_embedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      986 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-24 00:33:35.869841 cellmaps_image_embedding-0.1.0a5/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2272 2023-05-18 23:26:41.000000 cellmaps_image_embedding-0.1.0a5/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-24 00:33:35.867613 cellmaps_image_embedding-0.1.0a5/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a5/tests/test_cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a5/tests/test_cellmaps_image_embeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a5/tests/test_integration_cellmaps_image_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.914353 cellmaps_image_embedding-0.1.0a7/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:14:35.000000 cellmaps_image_embedding-0.1.0a7/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a7/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6288 2023-07-17 19:15:09.914637 cellmaps_image_embedding-0.1.0a7/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4186 2023-06-07 21:49:02.000000 cellmaps_image_embedding-0.1.0a7/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.904662 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      312 2023-06-07 21:49:02.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6564 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     5706 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/dataset.py
+-rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/models.py
+-rw-r--r--   0 churas     (504) staff       (20)    20356 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.906363 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6288 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1207 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      121 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.911823 cellmaps_image_embedding-0.1.0a7/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.900261 cellmaps_image_embedding-0.1.0a7/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.900333 cellmaps_image_embedding-0.1.0a7/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.912843 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a7/docs/cellmaps_image_embedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      986 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-07-17 19:15:09.915253 cellmaps_image_embedding-0.1.0a7/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2463 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.914066 cellmaps_image_embedding-0.1.0a7/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/tests/test_integration_cellmaps_image_embedding.py
```

### Comparing `cellmaps_image_embedding-0.1.0a5/CONTRIBUTING.rst` & `cellmaps_image_embedding-0.1.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/LICENSE` & `cellmaps_image_embedding-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/PKG-INFO` & `cellmaps_image_embedding-0.1.0a7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps_image_embedding
-Version: 0.1.0a5
+Version: 0.1.0a7
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
-Author: Gege Qian
-Author-email: geqian@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: =========================
         cellmaps_image_embedding
         =========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_image_embedding.svg
@@ -29,30 +29,40 @@
         * Documentation: https://cellmaps-image-embedding.readthedocs.io.
         
         
         
         Dependencies
         ------------
         
-        * TODO add
+        * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
+        * `tqdm <https://pypi.org/project/tqdm>`__
+        * `numpy <https://pypi.org/project/numpy>`__
+        * `pandas>=0.23.1 <https://pypi.org/project/pandas>`__
+        * `torch <https://pypi.org/project/torch>`__
+        * `torchvision <https://pypi.org/project/torchvision>`__
+        * `opencv-python <https://pypi.org/project/opencv-python>`__
+        * `mlcrate <https://pypi.org/project/mlcrate>`__
+        * `scikit-image <https://pypi.org/project/scikit-image>`__
+        * `scikit-learn>=0.19.0 <https://pypi.org/project/scikit-learn>`__
+        * `Pillow <https://pypi.org/project/Pillow>`__
         
         Compatibility
         -------------
         
         * Python 3.8+
         
         Installation
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_image_embedding
            cd cellmaps_image_embedding
            make dist
-           pip install dist/cellmaps_image_embeddingcmd*whl
+           pip install dist/cellmaps_image_embedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                         help='Name of organization running this tool, needed '
                              'for FAIRSCAPE. If unset, organization name specified '
                              'in --inputdir directory will be used')
     parser.add_argument('--project_name',
                         help='Name of project running this tool, needed for '
                              'FAIRSCAPE. If unset, project name specified '
                              'in --input directory will be used')
+    parser.add_argument('--fold', default=1, type=int, help='Image node attribute file fold to use')
     parser.add_argument('--fake_embedder', action='store_true',
                         help='If set, generate fake embedding')
     parser.add_argument('--dimensions', default=1024, type=int,
                         help='Dimensions of generated embedding vector')
     parser.add_argument('--suffix', default='.jpg',
                         help='Suffix for image files')
     parser.add_argument('--logconf', default=None,
@@ -94,14 +95,16 @@
 
 Generates image embeddings from immunofluorescent labeled images 
 from the Human Protein Atlas that were downloaded by the 
 cellmaps_imagedownloader package using Densenet code taken from:
 https://github.com/CellProfiling/densenet
 
 To use set --inputdir to output directory created by cellmaps_imagedownloader
+with red, blue, green, yellow directories containing images and FAIRSCAPE ro-crate
+configuration file (ro-crate-metadata.json)
 
 The generated embeddings are stored in image_emd.tsv under the output directory
 specified when running this tool. 
 
     """.format(version=cellmaps_image_embedding.__version__)
     theargs = _parse_arguments(desc, args[1:])
     theargs.program = args[0]
@@ -113,15 +116,16 @@
             gen = FakeEmbeddingGenerator(theargs.inputdir,
                                          dimensions=theargs.dimensions)
         else:
             gen = DensenetEmbeddingGenerator(os.path.abspath(theargs.inputdir),
                                              dimensions=theargs.dimensions,
                                              outdir=os.path.abspath(theargs.outdir),
                                              model_path=theargs.model_path,
-                                             suffix=theargs.suffix)
+                                             suffix=theargs.suffix,
+                                             fold=theargs.fold)
         return CellmapsImageEmbedder(outdir=theargs.outdir,
                                      inputdir=theargs.inputdir,
                                      embedding_generator=gen,
                                      name=theargs.name,
                                      project_name=theargs.project_name,
                                      organization_name=theargs.organization_name,
                                      input_data_dict=theargs.__dict__).run()
```

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/dataset.py` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import logging
 import cv2
+from PIL import Image
 
 import numpy as np
 import torch
 from torch.utils.data.dataset import Dataset
 from cellmaps_utils import constants
 
 opj = os.path.join
@@ -12,19 +13,19 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class ProteinDataset(Dataset):
     def __init__(
-        self, image_dir, image_size=512, crop_size=0, in_channels=4, suffix="png",
+        self, image_dir, outdir, image_size=512, crop_size=0, in_channels=4, suffix=".jpg",
         alt_image_ids=None,
     ):
         self.image_dir = image_dir
-
+        self.outdir = outdir
         self.suffix = suffix
 
         self.transform = None
 
         self.image_size = image_size
         self.crop_size = crop_size
         self.in_channels = in_channels
@@ -41,50 +42,63 @@
 
             self.image_ids = alt_image_ids
             print('setting alt image ids: ' + str(self.image_ids))
         else:
             # should we get image names from all color directories
             # and then let sort uniq do its work or do we assume we are good?
             image_names = os.listdir(os.path.join(self.image_dir, 'red'))
-
             # eg. ffd91122-bad0-11e8-b2b8-ac1f6b6435d0_red.png -> ffd91122-bad0-11e8-b2b8-ac1f6b6435d0
             self.image_ids = np.sort(
                 np.unique(
-                    [image_name[: image_name.rfind("_")] for image_name in image_names]
+                    [image_name[: image_name.rfind("_")] for image_name in image_names if image_name.endswith(self.suffix)]
                 )
             )
 
         self.num = len(self.image_ids)
-
+        
     def set_transform(self, transform=None):
         self.transform = transform
 
     def set_random_crop(self, random_crop=False):
         self.random_crop = random_crop
 
     def crop_image(self, image):
         random_crop_size = int(np.random.uniform(self.crop_size, self.image_size))
         x = int(np.random.uniform(0, self.image_size - random_crop_size))
         y = int(np.random.uniform(0, self.image_size - random_crop_size))
         crop_image = image[x : x + random_crop_size, y : y + random_crop_size]
         return crop_image
 
     def read_rgby(self, image_id):
-
+        # resize image
+        for color in self.colors:
+            try:
+                image = np.array(Image.open(
+                    opj(self.image_dir, color, "%s_%s%s" % (image_id, color, self.suffix))))[:, :, constants.COLOR_INDEXS.get(color)]
+
+            except: 
+                print('bad image : %s' % image_id)
+                image = cv2.imread(opj(self.image_dir, color, "%s_%s%s" % (image_id, color, self.suffix)))[:, :, -1::-1][:, :, constants.COLOR_INDEXS.get(color)]
+            
+            h, w = image.shape[:2]
+            if h != self.image_size or w != self.image_size:
+                image = cv2.resize(image, (self.image_size, self.image_size), interpolation=cv2.INTER_LINEAR)
+            cv2.imwrite(opj(self.outdir, color + '_resize', "%s_%s%s" % (image_id, color, self.suffix)), image,  [int(cv2.IMWRITE_JPEG_QUALITY), 85])
+            
         image = [
             cv2.imread(
-                opj(self.image_dir, color, "%s_%s%s" % (image_id, color, self.suffix)),
+                opj(self.outdir, color + '_resize', "%s_%s%s" % (image_id, color, self.suffix)),
                 cv2.IMREAD_GRAYSCALE,
             )
             for color in self.colors
         ]
 
         if image[0] is None:
             print(self.image_dir, image_id)
-
+        
         image = np.stack(image, axis=-1)
         logger.info(str(image.shape))
         h, w = image.shape[:2]
         if self.image_size != h or self.image_size != w:
             image = cv2.resize(
                 image,
                 (self.image_size, self.image_size),
```

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/models.py` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/models.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding/runner.py` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,45 @@
 from cellmaps_utils.provenance import ProvenanceUtil
 from cellmaps_image_embedding.exceptions import CellMapsImageEmbeddingError
 from cellmaps_image_embedding.dataset import *
 from cellmaps_image_embedding.models import *
 
 logger = logging.getLogger(__name__)
 
+ABB_LABEL_INDEX = {
+    "0": "Nucleoplasm",
+    "1": "N. membrane",
+    "2": "Nucleoli",
+    "3": "N. fibrillar c.",
+    "4": "N. speckles",
+    "5": "N. bodies",
+    "6": "ER",
+    "7": "Golgi app.",
+    "8": "Peroxisomes",
+    "9": "Endosomes",
+    "10": "Lysosomes",
+    "11": "Int. fil.",
+    "12": "Actin fil.",
+    "13": "F. a. sites",
+    "14": "Microtubules",
+    "15": "M. ends",
+    "16": "Cyt. bridge",
+    "17": "Mitotic spindle",
+    "18": "MTOC",
+    "19": "Centrosome",
+    "20": "Lipid droplets",
+    "21": "PM",
+    "22": "C. Junctions",
+    "23": "Mitochondria",
+    "24": "Aggresome",
+    "25": "Cytosol",
+    "26": "C. bodies",
+    "27": "Rods & Rings"
+}
+
 
 class EmbeddingGenerator(object):
     """
     Base class for implementations that generate
     network embeddings
     """
     def __init__(self, dimensions=1024):
@@ -58,29 +89,31 @@
 
 
 class FakeEmbeddingGenerator(EmbeddingGenerator):
     """
     Fakes image embedding
     """
     def __init__(self, inputdir, dimensions=1024,
-                 suffix='.jpg'):
+                 suffix='.jpg', img_emd_translator=None):
         """
         Constructor
 
         :param inputdir: Directory where images reside under
                          red, green, blue, and yellow directories
         :type inputdir: str
         :param dimensions: Desired size of output embedding
         :type dimensions: int
         :param suffix: Image suffix with starting ``.``
         :type suffix: str
         """
         super().__init__(dimensions=dimensions)
         self._inputdir = inputdir
         self._suffix = suffix
+        if img_emd_translator is None:
+            self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=inputdir, fold=1)
         warnings.warn(constants.IMAGE_EMBEDDING_FILE +
                       ' contains FAKE DATA!!!!\n'
                       'You have been warned\nHave a nice day\n')
         logger.error(constants.IMAGE_EMBEDDING_FILE +
                      ' contains FAKE DATA!!!! '
                      'You have been warned. Have a nice day')
 
@@ -110,32 +143,40 @@
         Caller should implement with ``yield`` operator
 
         :raises: NotImplementedError: Subclasses should implement this
         :return: Embedding
         :rtype: list
         """
         for image_id in self._get_image_id_list():
-            row = [image_id]
-            row.extend([random.random() for x in range(0, self.get_dimensions())])
-            yield row
+            if image_id not in self._img_emd_translator.get_name_mapping():
+                continue
+            g =  self._img_emd_translator.get_name_mapping()[image_id]
+
+            row = [g]
+            row.extend([random.random() for x in range(0, self.get_dimensions())]) ## check on the range of embeddings
+            prob = [g]
+            prob.extend([random.random() for x in range(0,len(ABB_LABEL_INDEX.keys()))]) ## might need to add to one
+            yield row, prob
 
 
 class DensenetEmbeddingGenerator(EmbeddingGenerator):
     """
     Runs densenet bundled with this tool via command line to
     generate embedding. Why do it this way? Easier transition
     from the original
     `Densenet <https://github.com/CellProfiling/densenet>`__
     code and no memory leaks
 
     """
     def __init__(self, inputdir, dimensions=1024,
                  outdir=None,
                  model_path=None,
-                 suffix='.jpg'):
+                 suffix='.jpg',
+                 fold = 1,
+                 img_emd_translator=None):
         """
         Constructor
 
         :param inputdir: Directory where red, blue, green, and yellow
                          image directories reside
         :type inputdir: str
         :param dimensions: Desired size of output embedding vector
@@ -147,32 +188,38 @@
         :param predict: Path to prediction script. Default value is the
                         script bundled with this tool
         :type predict: str
         :param model_path: Path to model file
         :type model_path: str
         :param suffix: Image suffix with starting ``.``
         :type suffix: str
+        :param img_emd_translator:
         """
         super().__init__(dimensions=dimensions)
         self._outdir = outdir
         self._inputdir = inputdir
+        self.fold = fold
         self._gpus = ''
         self._image_size = 1536
         self._crop_size = 1024
         self._device = 'cpu'
         self._cuda_available = False
         self._model_path = os.path.abspath(model_path)
         self._suffix = suffix
         self._channels = 4
         self._num_classes = 28
         self._seeds = [0]
         self._augments = ['default']
         self._model = self._initialize_model()
         self._dataset = self._initialize_dataset()
         self._dataloader = self._initialize_dataloader()
+        if img_emd_translator is None:
+            self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=inputdir, fold=fold)
+
+
 
     def _initialize_model(self):
         """
 
         """
         model = class_densenet121_large_dropout(num_classes=self._num_classes,
                                                 in_channels=self._channels,
@@ -185,14 +232,15 @@
     def _initialize_dataset(self):
         """
 
         :return:
         """
         dataset = ProteinDataset(
             self._inputdir,
+            self._outdir,
             image_size=self._image_size,
             crop_size=self._crop_size,
             in_channels=self._channels,
             suffix=self._suffix,
             alt_image_ids=None)
         return dataset
 
@@ -235,27 +283,71 @@
                     with torch.no_grad():
                         if self._cuda_available:
                             images = Variable(images.cuda())
                         else:
                             images = Variable(images)
                         logits, features = self._model(images)
 
+                        image_id = image_ids[iter_index] + '_'
+                        if image_id not in self._img_emd_translator.get_name_mapping():
+                            continue
+                        g =  self._img_emd_translator.get_name_mapping()[image_id]
                         # probabilities
-                        # probs = F.sigmoid(logits)
-                        # prob_list += probs.cpu().data.numpy().tolist()
+                        probs = F.sigmoid(logits)
+                        prob_list = [g]
+                        prob_list.extend(probs.cpu().data.numpy().tolist()[0])
 
                         # features
                         features = features.cpu().data.numpy().tolist()
-                        row = [image_ids[iter_index] + '_']
+                        row = [g]
                         row.extend(features[0])
                         del features
                         del logits
-                        yield row
+                        yield row, prob_list
+
+
+
+class ImageEmbeddingFilterAndNameTranslator(object):
+    """
+    Converts image embedding names and filters keeping only
+    one per gene
 
+    """
+
+    def __init__(self, image_downloaddir=None, fold = 1):
+        """
+        Constructor
+        """
+        self._id_to_gene_mapping = self._gen_filtered_mapping(os.path.join(image_downloaddir, str(fold) + '_' +
+                                                                           constants.IMAGE_GENE_NODE_ATTR_FILE))
 
+    def _gen_filtered_mapping(self, image_gene_node_attrs_file):
+        """
+        Reads TSV file
+
+        :param image_gene_node_attrs_file:
+        :return:
+        """
+        mapping_dict = {}
+        with open(image_gene_node_attrs_file, 'r') as f:
+            reader = csv.DictReader(f, delimiter='\t')
+            for row in reader:
+                mapping_dict[row['filename'].split(',')[0]] = row['name']
+        return mapping_dict
+
+    def get_name_mapping(self):
+        """
+        Gets mapping of old name to new name
+
+        :return: mapping of old name to new name
+        :rtype: dict
+        """
+        return self._id_to_gene_mapping
+                        
+                        
 class CellmapsImageEmbedder(object):
     """
     Class to run algorithm
     """
     def __init__(self, outdir=None,
                  inputdir=None,
                  embedding_generator=None,
@@ -277,14 +369,15 @@
         :param organization_name:
         :type organization_name: str
         :param project_name:
         :type project_name: str
         :param input_data_dict:
         :type input_data_dict: dict
         :param provenance_utils:
+
         """
         logger.debug('In constructor')
         if outdir is None:
             raise CellMapsImageEmbeddingError('outdir is None')
         self._outdir = os.path.abspath(outdir)
         self._inputdir = inputdir
         self._start_time = int(time.time())
@@ -292,15 +385,15 @@
         self._project_name = project_name
         self._organization_name = organization_name
         self._provenance_utils = provenance_utils
         self._embedding_generator = embedding_generator
         self._softwareid = None
         self._input_data_dict = input_data_dict
         self._image_embedding = None
-
+     
     def _create_rocrate(self):
         """
         Creates rocrate for output directory
 
         :raises CellMapsProvenanceError: If there is an error
         """
         name, proj_name, org_name = self._provenance_utils.get_name_project_org_of_rocrate(self._inputdir)
@@ -319,14 +412,31 @@
                                                     organization_name=org_name,
                                                     project_name=proj_name)
         except TypeError as te:
             raise CellMapsImageEmbeddingError('Invalid provenance: ' + str(te))
         except KeyError as ke:
             raise CellMapsImageEmbeddingError('Key missing in provenance: ' + str(ke))
 
+    def _create_output_directory(self):
+        """
+        Creates output directory if it does not already exist
+
+        :raises CellmapsDownloaderError: If output directory is None or if directory already exists
+        """
+        if os.path.isdir(self._outdir):
+            raise CellMapsImageEmbeddingError(self._outdir + ' already exists')
+
+        os.makedirs(self._outdir, mode=0o755)
+        for cur_color in constants.COLORS:
+            cdir = os.path.join(self._outdir, cur_color + '_resize')
+            if not os.path.isdir(cdir):
+                logger.debug('Creating directory: ' + cdir)
+                os.makedirs(cdir,
+                            mode=0o755)
+
     def _register_software(self):
         """
         Registers this tool
 
         :raises CellMapsImageEmbeddingError: If fairscape call fails
         """
         self._softwareid = self._provenance_utils.register_software(self._outdir,
@@ -373,30 +483,39 @@
     def get_image_embedding_file(self):
         """
         Gets image embedding file
         :return:
         """
         return os.path.join(self._outdir, constants.IMAGE_EMBEDDING_FILE)
 
+    def get_image_probability_file(self):
+        """
+        Gets image probability file
+        :return:
+        """
+        return os.path.join(self._outdir, "labels_prob.tsv")
+    
+    def get_name_mapping(self):
+        """
+
+        :return:
+        """
+        return self._img_emd_translator.get_oldname_to_new_name_mapping()
+    
     def run(self):
         """
         Runs cellmaps_image_embedding
 
 
         :return:
         """
         exitcode = 99
         try:
             logger.debug('In run method')
-
-            if os.path.isdir(self._outdir):
-                raise CellMapsImageEmbeddingError(self._outdir + ' already exists')
-
-            if not os.path.isdir(self._outdir):
-                os.makedirs(self._outdir, mode=0o755)
+            self._create_output_directory()
 
             logutils.setup_filelogger(outdir=self._outdir,
                                       handlerprefix='cellmaps_image_embedding')
             logutils.write_task_start_json(outdir=self._outdir,
                                            start_time=self._start_time,
                                            data={'imagedir': self._inputdir},
                                            version=cellmaps_image_embedding.__version__)
@@ -405,22 +524,31 @@
                 raise CellMapsImageEmbeddingError('inputdir must be set')
 
             self._create_rocrate()
 
             self._register_software()
 
             # generate result
+            raw_embeddings = []
             with open(self.get_image_embedding_file(), 'w', newline='') as f:
-                writer = csv.writer(f, delimiter='\t')
-                header_line = ['']
-                header_line.extend([x for x in range(1, self._embedding_generator.get_dimensions())])
-                writer.writerow(header_line)
-                for row in self._embedding_generator.get_next_embedding():
-                    writer.writerow(row)
-
+                with open(self.get_image_probability_file(), 'w', newline='') as pf:
+                    writer = csv.writer(f, delimiter='\t')
+                    prob_writer = csv.writer(pf, delimiter='\t')
+                    header_line = ['']
+                    header_line.extend([x for x in range(1, self._embedding_generator.get_dimensions())])
+                    writer.writerow(header_line)
+                    header_line_prob = ['']
+                    for key in range(0,len(ABB_LABEL_INDEX.keys())):
+                        header_line_prob.append(ABB_LABEL_INDEX[str(key)])
+                    prob_writer.writerow(header_line_prob)
+                    for row, prob_list in self._embedding_generator.get_next_embedding():
+                        writer.writerow(row)
+                        raw_embeddings.append(row)
+                        prob_writer.writerow(prob_list)
+ 
             self._register_image_embedding_file()
 
             self._register_computation()
             exitcode = 0
         finally:
             logutils.write_task_finish_json(outdir=self._outdir,
                                             start_time=self._start_time,
```

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/PKG-INFO` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps-image-embedding
-Version: 0.1.0a5
+Version: 0.1.0a7
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
-Author: Gege Qian
-Author-email: geqian@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: =========================
         cellmaps_image_embedding
         =========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_image_embedding.svg
@@ -29,30 +29,40 @@
         * Documentation: https://cellmaps-image-embedding.readthedocs.io.
         
         
         
         Dependencies
         ------------
         
-        * TODO add
+        * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
+        * `tqdm <https://pypi.org/project/tqdm>`__
+        * `numpy <https://pypi.org/project/numpy>`__
+        * `pandas>=0.23.1 <https://pypi.org/project/pandas>`__
+        * `torch <https://pypi.org/project/torch>`__
+        * `torchvision <https://pypi.org/project/torchvision>`__
+        * `opencv-python <https://pypi.org/project/opencv-python>`__
+        * `mlcrate <https://pypi.org/project/mlcrate>`__
+        * `scikit-image <https://pypi.org/project/scikit-image>`__
+        * `scikit-learn>=0.19.0 <https://pypi.org/project/scikit-learn>`__
+        * `Pillow <https://pypi.org/project/Pillow>`__
         
         Compatibility
         -------------
         
         * Python 3.8+
         
         Installation
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_image_embedding
            cd cellmaps_image_embedding
            make dist
-           pip install dist/cellmaps_image_embeddingcmd*whl
+           pip install dist/cellmaps_image_embedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_image_embedding-0.1.0a5/cellmaps_image_embedding.egg-info/SOURCES.txt` & `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/Makefile` & `cellmaps_image_embedding-0.1.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/cellmaps_image_embedding.rst` & `cellmaps_image_embedding-0.1.0a7/docs/cellmaps_image_embedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/conf.py` & `cellmaps_image_embedding-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/index.rst` & `cellmaps_image_embedding-0.1.0a7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/installation.rst` & `cellmaps_image_embedding-0.1.0a7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/make.bat` & `cellmaps_image_embedding-0.1.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/newrelease.rst` & `cellmaps_image_embedding-0.1.0a7/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/pypircfile.rst` & `cellmaps_image_embedding-0.1.0a7/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/usage.rst` & `cellmaps_image_embedding-0.1.0a7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/docs/versioningscheme.rst` & `cellmaps_image_embedding-0.1.0a7/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/setup.py` & `cellmaps_image_embedding-0.1.0a7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,42 +12,46 @@
         line = line.rstrip()
         if line.startswith('__version__'):
             version = re.sub("'", "", line[line.index("'"):])
         elif line.startswith('__description__'):
             desc = re.sub("'", "", line[line.index("'"):])
         elif line.startswith('__repo_url__'):
             repo_url = re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__author__'):
+            author = re.sub("'", "", line[line.index("'"):])
+        elif line.startswith('__email__'):
+            email = re.sub("'", "", line[line.index("'"):])
 
 print(repo_url)
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['cellmaps_utils',
                 'tqdm',
-                'pillow',
                 'numpy',
                 'pandas>0.23.1',
                 'torch',
                 'torchvision',
                 'opencv-python',
                 'mlcrate',
                 'scikit-image',
-                'scikit-learn>=0.19.0']
+                'scikit-learn>=0.19.0',
+                'Pillow']
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
-    author="Gege Qian",
-    author_email='geqian@ucsd.edu',
+    author=author,
+    author_email=email,
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `cellmaps_image_embedding-0.1.0a5/tests/test_cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/tests/test_cellmaps_image_embeddingrunner.py` & `cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingrunner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a5/tests/test_integration_cellmaps_image_embedding.py` & `cellmaps_image_embedding-0.1.0a7/tests/test_integration_cellmaps_image_embedding.py`

 * *Files identical despite different names*

