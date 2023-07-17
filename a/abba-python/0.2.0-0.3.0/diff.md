# Comparing `tmp/abba_python-0.2.0.tar.gz` & `tmp/abba_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-2ftz5zrf\abba_python-0.2.0.tar", last modified: Mon May 22 14:31:52 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-5ke3u64a\abba_python-0.3.0.tar", last modified: Mon Jul 17 15:19:09 2023, max compression
```

## Comparing `abba_python-0.2.0.tar` & `abba_python-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     2385 2023-05-03 06:42:55.000000 abba_python-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      157 2023-05-03 11:04:48.000000 abba_python-0.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2819 2023-05-22 14:31:52.000000 abba_python-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2023-05-22 14:29:44.000000 abba_python-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/usage.rst
--rw-rw-rw-   0        0        0      640 2023-05-22 14:31:52.000000 abba_python-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1406 2023-05-22 14:29:57.000000 abba_python-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/
--rw-rw-rw-   0        0        0      331 2023-05-22 14:29:57.000000 abba_python-0.2.0/src/abba_python/__init__.py
--rw-rw-rw-   0        0        0    42230 2023-05-22 14:25:41.000000 abba_python-0.2.0/src/abba_python/abba.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.2.0/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.2.0/src/abba_python/abba_private/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.2.0/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.2.0/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.2.0/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.2.0/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     2819 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.2.0/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.2.0/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     2385 2023-05-03 06:42:55.000000 abba_python-0.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      157 2023-05-03 11:04:48.000000 abba_python-0.3.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3191 2023-07-17 15:19:09.000000 abba_python-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2340 2023-07-17 15:00:52.000000 abba_python-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.3.0/docs/usage.rst
+-rw-rw-rw-   0        0        0      640 2023-07-17 15:19:09.000000 abba_python-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-07-17 15:18:42.000000 abba_python-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:11:13.000000 abba_python-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python/
+-rw-rw-rw-   0        0        0      331 2023-07-17 15:10:56.000000 abba_python-0.3.0/src/abba_python/__init__.py
+-rw-rw-rw-   0        0        0    42361 2023-07-14 07:36:32.000000 abba_python-0.3.0/src/abba_python/abba.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.3.0/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.3.0/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.3.0/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.3.0/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.3.0/src/abba_python/abba_private/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.3.0/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.3.0/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.3.0/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.3.0/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.3.0/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.3.0/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.3.0/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.3.0/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     3191 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.3.0/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 15:19:09.000000 abba_python-0.3.0/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 15:19:09.000000 abba_python-0.3.0/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.3.0/tests/test_abba_python.py
```

### Comparing `abba_python-0.2.0/CONTRIBUTING.rst` & `abba_python-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/LICENSE` & `abba_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/PKG-INFO` & `abba_python-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-===========
-ABBA Python
-===========
-
-
-.. image:: https://img.shields.io/pypi/v/abba_python.svg
-        :target: https://pypi.python.org/pypi/abba_python
-
-.. image:: https://img.shields.io/travis/nicoKiaru/abba_python.svg
-        :target: https://travis-ci.com/nicoKiaru/abba_python
 
+# ABBA Python
 
+[![](https://img.shields.io/pypi/v/abba_python.svg)](https://pypi.python.org/pypi/abba_python)
 
+[![](https://img.shields.io/travis/nicoKiaru/abba_python.svg)](https://travis-ci.com/nicoKiaru/abba_python)
 
 Aligning Big Brains and Atlases, controlled from Python.
 
-
 * Free software: GNU General Public License v3
 * Documentation: https://biop.github.io/ijp-imagetoatlas/
 
-
-ABBA in short
--------------
+# ABBA in short
 
 Aligning Big Brains & Atlases or ABBA for short, allows to register thin serial sections to several atlases, in coronal, sagittal and horizontal orientations.
 
-With ABBA Python, you have access to the 3D mouse Allen Brain atlas, and the Waxholm Space Atlas of the Sprague Dawley Rat Brain and all other BrainGlobe (https://docs.brainglobe.info/) atlases.
+With ABBA Python, you have access to the 3D mouse Allen Brain atlas, and the Waxholm Space Atlas of the Sprague Dawley Rat Brain and all [other BrainGlobe atlases](https://brainglobe.info/documentation/bg-atlasapi/usage/atlas-details.html).
 
-ABBA Python allows to use DeepSlice (https://pypi.org/project/DeepSlice/) for automated registration of mouse coronal sections (rat not implemented yet).
+ABBA Python allows to use [DeepSlice](https://pypi.org/project/DeepSlice/) for automated registration of mouse coronal sections (rat not implemented yet).
+
+# Getting started
 
 To get started with a GUI:
 - install miniconda
 - create a conda env with python 3.7 and openjdk 8:
 
-conda create -n myenv python=3.8 openjdk=8
+```
+conda create -c conda-forge -n myenv python=3.7 openjdk=8
 
 conda activate myenv
 
+pip install abba_python
+
 python
 
 >> from abba_python import abba
 
 >> abba.start_imagej()
+```
 
 You can then use ABBA in Fiji, see https://biop.github.io/ijp-imagetoatlas/
 
 ABBA is typically used in conjunction with QuPath (https://qupath.github.io/): a QuPath project can serve as an input for ABBA, and the registration results can be imported back into QuPath for downstream processing.
 
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+# Note on versions
 
+`abba_python` do not support python version above 3.7 because DeepSlice depends on tensorflow 1.15, which is not supported for later versions of python (https://github.com/PolarBean/DeepSlice/issues/41).
 
-=======
-History
-=======
+Openjdk version can work for version above 8, but it has been less used, so there may be unexpected bugs. You need to have openjdk installed from conda-forge, if you want to avoid [certificate issues](https://pyimagej.readthedocs.io/en/latest/Troubleshooting.html#unable-to-find-valid-certification-path).
 
-0.1.12 (2023-05-02)
--------------------
+# Credits
 
-* First working release on PyPI.
+This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
-0.1.13 (2023-05-03)
--------------------
+[Cookiecutter](https://github.com/audreyr/cookiecutter)
 
-* Documentation
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `abba_python-0.2.0/docs/Makefile` & `abba_python-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/docs/conf.py` & `abba_python-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/docs/installation.rst` & `abba_python-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/docs/make.bat` & `abba_python-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/setup.cfg` & `abba_python-0.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `abba_python-0.2.0/setup.py` & `abba_python-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['numpy', 'pandas', 'pyimagej', 'bg-atlasapi', 'DeepSlice==1.1.2']
 
@@ -21,24 +21,25 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.7'
     ],
     description="Aligning Big Brains and Atlases, controlled from Python.",
     install_requires=requirements,
     license="GNU General Public License v3",
-    long_description=readme + '\n\n' + history,
+    #long_description=readme + '\n\n' + history,
+    long_description=readme,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.2.0/src/abba_python/abba.py` & `abba_python-0.3.0/src/abba_python/abba.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 def get_java_dependencies():
     """
     Returns the jar files that need to be included into the classpath
     of an imagej object in order to have a functional ABBA app
     these jars should be available in https://maven.scijava.org/
     :return:
     """
-    imagej_core_dep = 'net.imagej:imagej:2.9.0'
-    imagej_legacy_dep = 'net.imagej:imagej-legacy:0.39.3'
-    abba_dep = 'ch.epfl.biop:ImageToAtlasRegister:0.5.4'
+    imagej_core_dep = 'net.imagej:imagej:2.14.0'
+    imagej_legacy_dep = 'net.imagej:imagej-legacy:1.2.0'
+    abba_dep = 'ch.epfl.biop:ImageToAtlasRegister:0.6.0'
     return [imagej_core_dep, imagej_legacy_dep, abba_dep]
 
 
 def add_brainglobe_atlases(ij):
     # TODO : check connection available or not
     try:
         check_internet_connection()
@@ -285,23 +285,25 @@
         # in java TODO
 
         # or in python
         if atlas_name not in Abba.opened_atlases:
             if atlas_name == 'Adult Mouse Brain - Allen Brain Atlas V3':
                 atlas_name = 'Adult Mouse Brain - Allen Brain Atlas V3p1'
             if atlas_name == 'Rat - Waxholm Sprague Dawley V4':
-                atlas_name = 'Rat - Waxholm Sprague Dawley V4p1'
+                atlas_name = 'Rat - Waxholm Sprague Dawley V4p2'
+            if atlas_name == 'Rat - Waxholm Sprague Dawley V4p1':
+                atlas_name = 'Rat - Waxholm Sprague Dawley V4p2'
             if atlas_name == 'Adult Mouse Brain - Allen Brain Atlas V3p1':
                 AllenBrainAdultMouseAtlasCCF2017Command = jimport(
                     'ch.epfl.biop.atlas.mouse.allen.ccfv3p1.command.AllenBrainAdultMouseAtlasCCF2017v3p1Command')
                 atlas = ij.command().run(AllenBrainAdultMouseAtlasCCF2017Command, True).get().getOutput("ba")
                 Abba.opened_atlases[atlas_name] = atlas
-            elif atlas_name == 'Rat - Waxholm Sprague Dawley V4p1':
+            elif atlas_name == 'Rat - Waxholm Sprague Dawley V4p2':
                 WaxholmSpragueDawleyRatV4Command = jimport(
-                    'ch.epfl.biop.atlas.rat.waxholm.spraguedawley.v4p1.command.WaxholmSpragueDawleyRatV4p1Command')
+                    'ch.epfl.biop.atlas.rat.waxholm.spraguedawley.v4p2.command.WaxholmSpragueDawleyRatV4p2Command')
                 atlas = ij.command().run(WaxholmSpragueDawleyRatV4Command, True).get().getOutput("ba")
                 Abba.opened_atlases[atlas_name] = atlas
             else:
                 bg_atlas = BrainGlobeAtlas(atlas_name)
 
                 try:
                     from abba_python.abba_private.AbbaAtlas import \
```

### Comparing `abba_python-0.2.0/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.3.0/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.3.0/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.3.0/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/abba_private/DeepSliceProcessor.py` & `abba_python-0.3.0/src/abba_python/abba_private/DeepSliceProcessor.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/itk/abba_itk.py` & `abba_python-0.3.0/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.3.0/src/abba_python/run-abba-local-fiji.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/run-abba.py` & `abba_python-0.3.0/src/abba_python/run-abba.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/scijava_python_command/command.py` & `abba_python-0.3.0/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.3.0/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.3.0/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.2.0/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.3.0/src/abba_python.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-===========
-ABBA Python
-===========
-
-
-.. image:: https://img.shields.io/pypi/v/abba_python.svg
-        :target: https://pypi.python.org/pypi/abba_python
-
-.. image:: https://img.shields.io/travis/nicoKiaru/abba_python.svg
-        :target: https://travis-ci.com/nicoKiaru/abba_python
 
+# ABBA Python
 
+[![](https://img.shields.io/pypi/v/abba_python.svg)](https://pypi.python.org/pypi/abba_python)
 
+[![](https://img.shields.io/travis/nicoKiaru/abba_python.svg)](https://travis-ci.com/nicoKiaru/abba_python)
 
 Aligning Big Brains and Atlases, controlled from Python.
 
-
 * Free software: GNU General Public License v3
 * Documentation: https://biop.github.io/ijp-imagetoatlas/
 
-
-ABBA in short
--------------
+# ABBA in short
 
 Aligning Big Brains & Atlases or ABBA for short, allows to register thin serial sections to several atlases, in coronal, sagittal and horizontal orientations.
 
-With ABBA Python, you have access to the 3D mouse Allen Brain atlas, and the Waxholm Space Atlas of the Sprague Dawley Rat Brain and all other BrainGlobe (https://docs.brainglobe.info/) atlases.
+With ABBA Python, you have access to the 3D mouse Allen Brain atlas, and the Waxholm Space Atlas of the Sprague Dawley Rat Brain and all [other BrainGlobe atlases](https://brainglobe.info/documentation/bg-atlasapi/usage/atlas-details.html).
 
-ABBA Python allows to use DeepSlice (https://pypi.org/project/DeepSlice/) for automated registration of mouse coronal sections (rat not implemented yet).
+ABBA Python allows to use [DeepSlice](https://pypi.org/project/DeepSlice/) for automated registration of mouse coronal sections (rat not implemented yet).
+
+# Getting started
 
 To get started with a GUI:
 - install miniconda
 - create a conda env with python 3.7 and openjdk 8:
 
-conda create -n myenv python=3.8 openjdk=8
+```
+conda create -c conda-forge -n myenv python=3.7 openjdk=8
 
 conda activate myenv
 
+pip install abba_python
+
 python
 
 >> from abba_python import abba
 
 >> abba.start_imagej()
+```
 
 You can then use ABBA in Fiji, see https://biop.github.io/ijp-imagetoatlas/
 
 ABBA is typically used in conjunction with QuPath (https://qupath.github.io/): a QuPath project can serve as an input for ABBA, and the registration results can be imported back into QuPath for downstream processing.
 
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+# Note on versions
 
+`abba_python` do not support python version above 3.7 because DeepSlice depends on tensorflow 1.15, which is not supported for later versions of python (https://github.com/PolarBean/DeepSlice/issues/41).
 
-=======
-History
-=======
+Openjdk version can work for version above 8, but it has been less used, so there may be unexpected bugs. You need to have openjdk installed from conda-forge, if you want to avoid [certificate issues](https://pyimagej.readthedocs.io/en/latest/Troubleshooting.html#unable-to-find-valid-certification-path).
 
-0.1.12 (2023-05-02)
--------------------
+# Credits
 
-* First working release on PyPI.
+This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
 
-0.1.13 (2023-05-03)
--------------------
+[Cookiecutter](https://github.com/audreyr/cookiecutter)
 
-* Documentation
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `abba_python-0.2.0/src/abba_python.egg-info/SOURCES.txt` & `abba_python-0.3.0/src/abba_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

