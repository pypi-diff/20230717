# Comparing `tmp/cellmaps_pipeline-0.1.0a3.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a3.tar", last modified: Tue May 30 23:33:24 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a4.tar", last modified: Mon Jul 17 20:25:45 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a3.tar` & `cellmaps_pipeline-0.1.0a4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.178800 cellmaps_pipeline-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-30 23:33:24.178917 cellmaps_pipeline-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4019 2023-05-22 23:49:10.000000 cellmaps_pipeline-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.170785 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      277 2023-05-30 21:24:11.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7654 2023-05-23 16:27:52.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    11415 2023-05-30 21:24:11.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.172042 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6043 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1024 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      169 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-05-30 23:33:24.000000 cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.176629 cellmaps_pipeline-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.167907 cellmaps_pipeline-0.1.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.167972 cellmaps_pipeline-0.1.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.177730 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a3/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-05-30 23:33:24.179349 cellmaps_pipeline-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2386 2023-05-19 23:36:32.000000 cellmaps_pipeline-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:24.178627 cellmaps_pipeline-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a3/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1296 2023-05-30 21:25:35.000000 cellmaps_pipeline-0.1.0a3/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-30 21:25:54.000000 cellmaps_pipeline-0.1.0a3/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a3/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.624572 cellmaps_pipeline-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6042 2023-07-17 20:25:45.624699 cellmaps_pipeline-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4016 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.616629 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      279 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.617928 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6042 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1024 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      243 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.622638 cellmaps_pipeline-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.613670 cellmaps_pipeline-0.1.0a4/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.613741 cellmaps_pipeline-0.1.0a4/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.623331 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a4/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-07-17 20:25:45.625693 cellmaps_pipeline-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2460 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.624362 cellmaps_pipeline-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/LICENSE` & `cellmaps_pipeline-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/PKG-INFO` & `cellmaps_pipeline-0.1.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
-Author: Christopher Churas
-Author-email: cchuras@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ==============
         CM4AI Pipeline
         ==============
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_pipeline.svg
@@ -50,15 +50,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_pipeline
            cd cellmaps_pipeline
            make dist
-           pip install dist/cellmaps_pipelinecmd*whl
+           pip install dist/cellmaps_pipeline*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_pipeline-0.1.0a3/README.rst` & `cellmaps_pipeline-0.1.0a4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ------------
 
 .. code-block::
 
    git clone https://github.com/idekerlab/cellmaps_pipeline
    cd cellmaps_pipeline
    make dist
-   pip install dist/cellmaps_pipelinecmd*whl
+   pip install dist/cellmaps_pipeline*whl
 
 
 Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
 
 .. code-block::
 
    make
```

### Comparing `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,14 +56,28 @@
                         help='Path to model file. A model file to download '
                              'is here: '
                              'https://github.com/'
                              'CellProfiling/densenet/releases/download/'
                              'v0.1.0/external_crop512_focal_slov_hardlog'
                              '_class_densenet121_dropout_i768_aug2_5folds'
                              '_fold0_final.pth')
+    parser.add_argument('--fold', default=1, type=int, help='Image node attribute file fold to use')
+    parser.add_argument('--proteinatlasxml',
+                        default='https://www.proteinatlas.org/download/proteinatlas.xml.gz',
+                        help='URL or path to proteinatlas.xml or proteinatlas.xml.gz file '
+                             'used to look for images not found in the standard location '
+                             'on HPA')
+    parser.add_argument('--ppi_cutoffs', nargs='+', type=float,
+                        default=[0.001, 0.002, 0.003, 0.004, 0.005, 0.006,
+                                 0.007, 0.008, 0.009, 0.01, 0.02, 0.03,
+                                 0.04, 0.05, 0.10],
+                        help='Cutoffs used to generate PPI input networks. For example, '
+                             'a value of 0.1 means to generate PPI input network using the '
+                             'top ten percent of coembedding entries. Each cutoff generates '
+                             'another PPI network')
     parser.add_argument('--provenance',
                         help='Path to file containing provenance '
                              'information about input files in JSON format. '
                              'This is required and not including will output '
                              'and error message with example of file')
     parser.add_argument('--fake', action='store_true',
                         help='If set, generate fake data for every step')
@@ -106,15 +120,15 @@
 
     withguids_json = json.dumps(withguid, indent=2)
     register_json = json.dumps(register, indent=2)
 
     desc = """
 Version {version}
 
-Invokes run() method on CellmapsPipeline
+Runs the full cellmaps pipeline
 
 In addition, the --provenance flag is required and must be set to a path 
 to a JSON file. 
 
 If datasets are already registered with FAIRSCAPE then the following is sufficient:
 
 {withguids}
@@ -152,16 +166,19 @@
 
         runner = ProgrammaticPipelineRunner(outdir=theargs.outdir,
                                             samples=theargs.samples,
                                             unique=theargs.unique,
                                             edgelist=theargs.edgelist,
                                             baitlist=theargs.baitlist,
                                             model_path=theargs.model_path,
+                                            proteinatlasxml=theargs.proteinatlasxml,
+                                            ppi_cutoffs=theargs.ppi_cutoffs,
                                             fake=theargs.fake,
                                             provenance=json_prov,
+                                            fold=theargs.fold,
                                             input_data_dict=theargs.__dict__)
 
         return CellmapsPipeline(outdir=theargs.outdir,
                                 runner=runner,
                                 input_data_dict=theargs.__dict__).run()
     except Exception as e:
         logger.exception('Caught exception: ' + str(e))
```

### Comparing `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #! /usr/bin/env python
 
 import os
-import sys
 import warnings
 import logging
 import time
 import networkx as nx
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
+from cellmaps_utils.provenance import ProvenanceUtil
 
 from cellmaps_imagedownloader.runner import MultiProcessImageDownloader
 from cellmaps_imagedownloader.runner import FakeImageDownloader
 from cellmaps_imagedownloader.runner import CellmapsImageDownloader
 from cellmaps_imagedownloader.gene import ImageGeneNodeAttributeGenerator
 from cellmaps_ppidownloader.runner import CellmapsPPIDownloader
 from cellmaps_ppidownloader.gene import APMSGeneNodeAttributeGenerator
@@ -21,15 +21,19 @@
 from cellmaps_image_embedding.runner import FakeEmbeddingGenerator
 from cellmaps_image_embedding.runner import DensenetEmbeddingGenerator
 from cellmaps_coembedding.runner import MuseCoEmbeddingGenerator
 from cellmaps_coembedding.runner import FakeCoEmbeddingGenerator
 from cellmaps_coembedding.runner import CellmapsCoEmbedder
 from cellmaps_generate_hierarchy.ppi import CosineSimilarityPPIGenerator
 from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
+from cellmaps_generate_hierarchy.maturehierarchy import HiDeFHierarchyRefiner
 from cellmaps_generate_hierarchy.runner import CellmapsGenerateHierarchy
+from cellmaps_imagedownloader.proteinatlas import ProteinAtlasReader
+from cellmaps_imagedownloader.proteinatlas import ProteinAtlasImageUrlReader
+from cellmaps_imagedownloader.proteinatlas import ImageDownloadTupleGenerator
 
 import cellmaps_pipeline
 from cellmaps_pipeline.exceptions import CellmapsPipelineError
 
 
 logger = logging.getLogger(__name__)
 
@@ -60,29 +64,37 @@
     """
     def __init__(self, outdir=None,
                  samples=None,
                  unique=None,
                  edgelist=None,
                  baitlist=None,
                  model_path=None,
+                 proteinatlasxml=None,
+                 ppi_cutoffs=None,
                  fake=None,
                  provenance=None,
+                 provenance_utils=ProvenanceUtil(),
+                 fold=1,
                  input_data_dict=None):
         """
         Constructor
         """
         super().__init__()
         self._outdir = os.path.abspath(outdir)
         self._samples = samples
         self._unique = unique
         self._edgelist = edgelist
         self._baitlist = baitlist
         self._model_path = model_path
         self._fake = fake
         self._provenance = provenance
+        self._provenance_utils = provenance_utils
+        self._fold = fold
+        self._proteinatlasxml = proteinatlasxml
+        self._ppi_cutoffs = ppi_cutoffs
         self._input_data_dict = input_data_dict
         self._image_dir = os.path.join(self._outdir,
                                        constants.IMAGE_DOWNLOAD_STEP_DIR)
         self._ppi_dir = os.path.join(self._outdir,
                                      constants.PPI_DOWNLOAD_STEP_DIR)
         self._ppi_embed_dir = os.path.join(self._outdir,
                                            constants.PPI_EMBEDDING_STEP_DIR)
@@ -127,44 +139,46 @@
 
         :return:
         """
         if os.path.isdir(self._hierarchy_dir):
             warnings.warn('Found hierarchy dir, assuming we are good. skipping')
             return 0
 
-        ppigen = CosineSimilarityPPIGenerator(embeddingdir=self._coembed_dir)
+        ppigen = CosineSimilarityPPIGenerator(embeddingdir=self._coembed_dir,
+                                              cutoffs=self._ppi_cutoffs)
 
-        hiergen = CDAPSHiDeFHierarchyGenerator()
+        refiner = HiDeFHierarchyRefiner(provenance_utils=self._provenance_utils)
+
+        hiergen = CDAPSHiDeFHierarchyGenerator(refiner=refiner,
+                                               provenance_utils=self._provenance_utils)
         return CellmapsGenerateHierarchy(outdir=self._hierarchy_dir,
                                          inputdir=self._coembed_dir,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
-                                         input_data_dict=self._input_data_dict).run()
+                                         input_data_dict=self._input_data_dict,
+                                         provenance_utils=self._provenance_utils).run()
 
     def _coembed(self):
         """
 
         :return:
         """
         if os.path.isdir(self._coembed_dir):
             warnings.warn('Found coembedding dir, assuming we are good. skipping')
             return 0
 
         if self._fake:
             gen = FakeCoEmbeddingGenerator(ppi_embeddingdir=self._ppi_embed_dir,
-                                           image_embeddingdir=self._image_embed_dir,
-                                           image_downloaddir=self._image_dir)
+                                           image_embeddingdir=self._image_embed_dir)
         else:
             gen = MuseCoEmbeddingGenerator(outdir=self._coembed_dir,
                                            ppi_embeddingdir=self._ppi_embed_dir,
-                                           image_embeddingdir=self._image_embed_dir,
-                                           image_downloaddir=self._image_dir)
+                                           image_embeddingdir=self._image_embed_dir)
         return CellmapsCoEmbedder(outdir=self._coembed_dir,
-                                  inputdirs=[self._image_embed_dir, self._ppi_embed_dir,
-                                             self._image_dir],
+                                  inputdirs=[self._image_embed_dir, self._ppi_embed_dir],
                                   embedding_generator=gen,
                                   input_data_dict=self._input_data_dict).run()
 
     def _embed_image(self):
         """
 
         :return:
@@ -174,15 +188,16 @@
             return 0
 
         if self._fake is True:
             gen = FakeEmbeddingGenerator(self._image_dir)
         else:
             gen = DensenetEmbeddingGenerator(self._image_dir,
                                              outdir=self._image_embed_dir,
-                                             model_path=self._model_path)
+                                             model_path=self._model_path,
+                                             fold=self._fold)
         return CellmapsImageEmbedder(outdir=self._image_embed_dir,
                                      inputdir=self._image_dir,
                                      embedding_generator=gen,
                                      input_data_dict=self._input_data_dict).run()
 
     def _embed_ppi(self):
         """
@@ -226,28 +241,35 @@
         :return: exit code of :py:meth:`~cellmaps_imagedownloader.runner.CellmapsImageDownloader.run`
         :rtype: int
         """
         if os.path.isdir(self._image_dir):
             warnings.warn('Found image dir, assuming we are good. skipping')
             return 0
         logger.info('Downloading images')
+
         imagegen = ImageGeneNodeAttributeGenerator(
             unique_list=ImageGeneNodeAttributeGenerator.get_unique_list_from_csvfile(self._unique),
             samples_list=ImageGeneNodeAttributeGenerator.get_samples_from_csvfile(self._samples))
 
+        proteinatlas_reader = ProteinAtlasReader(self._image_dir, proteinatlas=self._proteinatlasxml)
+        proteinatlas_urlreader = ProteinAtlasImageUrlReader(reader=proteinatlas_reader)
+        imageurlgen = ImageDownloadTupleGenerator(reader=proteinatlas_urlreader,
+                                                  samples_list=imagegen.get_samples_list())
+
         if self._fake is True:
             warnings.warn('FAKE IMAGES ARE BEING DOWNLOADED!!!!!')
             dloader = FakeImageDownloader()
         else:
             dloader = MultiProcessImageDownloader()
         # Todo: input_data_dict should NOT be required to run this
         #       https://github.com/idekerlab/cellmaps_imagedownloader/issues/2
         return CellmapsImageDownloader(outdir=self._image_dir,
                                        imagedownloader=dloader,
                                        imagegen=imagegen,
+                                       imageurlgen=imageurlgen,
                                        provenance=self._provenance,
                                        skip_failed=True,
                                        input_data_dict=self._input_data_dict).run()
 
 
 class CellmapsPipeline(object):
     """
```

### Comparing `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
-Author: Christopher Churas
-Author-email: cchuras@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ==============
         CM4AI Pipeline
         ==============
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_pipeline.svg
@@ -50,15 +50,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_pipeline
            cd cellmaps_pipeline
            make dist
-           pip install dist/cellmaps_pipelinecmd*whl
+           pip install dist/cellmaps_pipeline*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_pipeline-0.1.0a3/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/Makefile` & `cellmaps_pipeline-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a4/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/conf.py` & `cellmaps_pipeline-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/index.rst` & `cellmaps_pipeline-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/installation.rst` & `cellmaps_pipeline-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/make.bat` & `cellmaps_pipeline-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/usage.rst` & `cellmaps_pipeline-0.1.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/setup.py` & `cellmaps_pipeline-0.1.0a4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['cellmaps_utils',
-                'cellmaps_imagedownloader',
-                'cellmaps_ppidownloader',
-                'cellmaps_image_embedding',
-                'cellmaps_ppi_embedding',
-                'cellmaps_coembedding',
-                'cellmaps_generate_hierarchy',
-                'networkx']
+requirements = ['cellmaps_utils==0.1.0a13',
+                'cellmaps_imagedownloader==0.1.0a6',
+                'cellmaps_ppidownloader==0.1.0a3',
+                'cellmaps_image_embedding==0.1.0a7',
+                'cellmaps_ppi_embedding==0.1.0a4',
+                'cellmaps_coembedding==0.1.0a3',
+                'cellmaps_generate_hierarchy==0.1.0a6',
+                'networkx>=2.8,<2.9']
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     author=author,
```

### Comparing `cellmaps_pipeline-0.1.0a3/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a4/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a4/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a3/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a4/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

