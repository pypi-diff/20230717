# Comparing `tmp/pyote-5.3.2.tar.gz` & `tmp/pyote-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.3.2.tar", last modified: Sun Jul 16 03:15:08 2023, max compression
+gzip compressed data, was "pyote-5.3.3.tar", last modified: Mon Jul 17 17:41:02 2023, max compression
```

## Comparing `pyote-5.3.2.tar` & `pyote-5.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.833435 pyote-5.3.2/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.2/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-16 03:15:08.833435 pyote-5.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.2/README.rst
--rw-rw-rw-   0        0        0       80 2023-07-16 03:15:08.834467 pyote-5.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-06-06 20:30:01.000000 pyote-5.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.648538 pyote-5.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.659622 pyote-5.3.2/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.2/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      257 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.795839 pyote-5.3.2/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.2/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.2/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.2/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.2/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.2/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.2/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.2/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.2/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.2/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.2/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.2/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.2/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.2/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.2/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.2/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.2/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.2/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.2/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.833435 pyote-5.3.2/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.2/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
--rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.2/src/pyoteapp/model-examples/LCP_penumbral.p
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.2/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.2/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   459582 2023-07-16 02:51:18.000000 pyote-5.3.2/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   449634 2023-07-16 02:45:25.000000 pyote-5.3.2/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.2/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.2/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.2/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.2/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.2/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.2/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.2/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-07-14 17:15:17.000000 pyote-5.3.2/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.651254 pyote-5.3.3/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.3/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-07-17 17:41:02.651254 pyote-5.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.3/README.rst
+-rw-rw-rw-   0        0        0       80 2023-07-17 17:41:02.652254 pyote-5.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-06-06 20:30:01.000000 pyote-5.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.455457 pyote-5.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.471068 pyote-5.3.3/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.3/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      257 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.605894 pyote-5.3.3/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.3/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.3/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.3/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.3/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.3/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.3/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.3/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.3/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.3/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.3/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.3/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.3/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.3/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.3/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.3/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.3/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.3/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.3/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.650254 pyote-5.3.3/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.3/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
+-rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.3/src/pyoteapp/model-examples/LCP_penumbral.p
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.3/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.3/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   459673 2023-07-17 17:39:18.000000 pyote-5.3.3/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   449791 2023-07-17 17:31:01.000000 pyote-5.3.3/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.3/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.3/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.3/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.3/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.3/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.3/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.3/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-07-17 17:37:34.000000 pyote-5.3.3/src/pyoteapp/version.py
```

### Comparing `pyote-5.3.2/LICENSE` & `pyote-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/PKG-INFO` & `pyote-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.2
+Version: 5.3.3
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.2/setup.py` & `pyote-5.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyote.egg-info/PKG-INFO` & `pyote-5.3.3/src/pyote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.2
+Version: 5.3.3
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.2/src/pyote.egg-info/SOURCES.txt` & `pyote-5.3.3/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/SER.py` & `pyote-5.3.3/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/autocorrtools.py` & `pyote-5.3.3/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.3.3/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.3.3/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/csvreader.py` & `pyote-5.3.3/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/diffraction-table.p` & `pyote-5.3.3/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/errorBarUtils.py` & `pyote-5.3.3/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/example-penumbral.csv` & `pyote-5.3.3/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.3.3/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/false_positive.py` & `pyote-5.3.3/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/fixedPrecision.py` & `pyote-5.3.3/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/genDiffraction.py` & `pyote-5.3.3/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/gui.py` & `pyote-5.3.3/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/helpDialog.py` & `pyote-5.3.3/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.3.3/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/likelihood_calculations.py` & `pyote-5.3.3/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p` & `pyote-5.3.3/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/LCP_penumbral.p` & `pyote-5.3.3/src/pyoteapp/model-examples/LCP_penumbral.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/model-help.pdf` & `pyote-5.3.3/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/noiseUtils.py` & `pyote-5.3.3/src/pyoteapp/noiseUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/pyote-info.pdf` & `pyote-5.3.3/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,11 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.3.3
+17 July 2023
+• Fixes a bug in the fit-metric.txt file duration calculation
 Version 5.3.2
 15 July 2023
 • Fixes a bug in the calculation of the duration fit metric when an already integrated csv
 file is in use.
 •
 
 Added specialized folders inside an observation folder to reduce clutter. There are new
@@ -36,21 +39,21 @@
 The user will need to edit the csv file to resolve the name duplication.
 •
 
 Added a warning message that will only appear if a user manually calculates baseline
 statistics and then does a find event. Sometimes that is exactly what is wanted, but
 those statistics become fixed and will be used for all subsequent find event clicks.
 That would be very wrong if the user is stepping through multiple light-curves in search
-of the “best” as they would all use the same baseline numbers (B and sigmaB).
 
+of the “best” as they would all use the same baseline numbers (B and sigmaB).
 •
 
 Added false-positive metric to fit-metrics and rearranged output order.
 
-Version 5.2.7
+Version 5.2.7
 24 June 2023
 • Minor change: corrected titles in fit-metric file from D frame to D reading num and R
 frame to R reading num
 Version 5.2.6
 17 June 2023
 • Changed order of buttons on Noise analysis/Detectability tab to better reflect work flow
 •
@@ -99,20 +102,25 @@
 
 Fixes a bug in the calculation of flash edge times that was discovered when very high
 SNR recording was attempted
 
 Version 5.2.2
 13 April 2023
 • Adds diffraction modelling of an elliptical asteroid shape
-Version 5.2.1 27 March 2023
-• Fixed problem with VizieR loading from North American .xlsx caused by Occult
-sometimes putting a string in the asteroid field and sometimes an integer.
+Version 5.2.1
+
+27 March 2023
 
 •
 
+Fixed problem with VizieR loading from North American .xlsx caused by Occult
+sometimes putting a string in the asteroid field and sometimes an integer.
+
+•
+
 SER files with colorCode other than mono are now accepted.
 
 Version 5.2.0 17 March 2023
 • Fixes a bug in code introduced in version 5.1.0 where dropped frames are detected –
 that code did not handle an observation that passed through midnight (23:59:59)
 Version 5.1.9 10 March 2023
 • Fixes issues involving Tangra light curve names
@@ -149,21 +157,22 @@
 reading PyMovie csv files (such as ‘signal’ or ‘appsum’), it was not possible to mix-andmatch data sets with different prefixes. With this version, that now becomes possible.
 With this feature, it now becomes possible to demonstrate for yourself that there is no
 reason to process a target lightcurve in ‘aperture sum’ mode (no background
 subtraction) versus the regular ‘signal’ mode (where background subtraction is
 performed). Simply display the ‘signal’ and ‘appsum’ versions of a target lightcurve and
 use the y position spinBox on one of the curves until they overlap. This should show
 that during the event, the points almost exactly overlap, so event timing will be the
-same.
+
+same.
 •
 
 Added a button to the VizieR tab that will fill most of the entry boxes in the VizieR form
-
-from a North American .xlsx file for that event (derived from OW/Occult 4), if one is
+from a North American .xlsx file for that event (derived from OW/Occult 4), if one is
 available.
+
 Version 5.0.8 1 February 2023
 • Changed the VizieR form filling requirements to allow for all star catalog entries to
 remain unfilled.
 Version 5.0.7 22 January 2023
 • Fixed insidious and dangerous bug in VizieR tab that caused site coordinates to be
 saved and restored incorrectly.
 Version 5.0.6 19 January 2023
@@ -198,22 +207,23 @@
 Made D and R edge time calculations work properly even when there are dropped
 readings in the observation
 
 Version 5.0.0 6 January 2023
 • Added ability to specify a block size to be used during automatic block integration.
 When a block size is entered, the program will determine the best offset value to use
 for the integration.
-•
+
+•
 
 Added a comprehensive set of lightcurve models together with tools to help automate
 the fitting of the new models to observation data. Models included:
 o Diffraction (including central spot for low rho events) using physical optics
-
-o Disk on disk (geometrical optics) for large stars
+o Disk on disk (geometrical optics) for large stars
 o Edge on disk (geometrical optics) for large stars and limb angles on asteroid
+
 Version 4.9.2 14 August 2022
 • Added various tests involving the penumbral fit process to gently lead the user back to
 the path of rightness should that user try to do a ‘fit’ without loading a light-curve and/or
 not marking D and R regions.
 Version 4.9.1 10 August 2022
 • In the diffraction tab, added a selection box so that asteroid distance can be entered
 either in parallax (arcseconds) or AU. Also reviewed and added to the context help on
@@ -238,22 +248,19 @@
 that appear after the program has closed are harmless artifacts of the order in which
 QUI elements are closed.
 Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
 two programs can share a virtual environment, thus saving much space.
 Version 4.8.6 23 July 2022
 • added instructions telling the user how to install a new version when one is found.
-There are instructions for pip based installations and pipenv installations
-Version 4.8.4
-
-•
 
-there are no changes. This is a new version just to test the change introduced in 4.8.3
+There are instructions for pip based installations and pipenv installations
+Version 4.8.4
+• there are no changes. This is a new version just to test the change introduced in 4.8.3
 about version detection and handling thereof.
-
 Version 4.8.3
 • this version removes the offer to update to a newer version when one is found. This
 has been done primarily to allow an easy transition to a distribution method that does
 not require the installation of Anaconda3, but it also gives the user more control. When
 a newer version is available, a message to that effect will be shown but otherwise the
 user’s workflow is not interrupted by a ‘nag’ about ‘do you want to download the newer
 version?’.
@@ -287,18 +294,17 @@
 version 4.6.4
 • made the 'camera response' checkbox (in the Settings/misc tab) sticky
 •
 
 corrected the log messaging about Donly, Ronly, DandR, and min/max directions to the
 solver consistent
 
-version 4.6.3
+version 4.6.3
 • in detectability: logged new 'drop message' to the detectability.log
-
-version 4.6.2
+version 4.6.2
 • in detectability: when event duration is or becomes less than the camera exposure
 time, the observed drop is reduced proportionately
 version 4.6.1
 • in detectability: changed calculation of number of event points from
 ceiling(dur/rdgTime) to round(dur/rdgTime)
 •
 
@@ -329,18 +335,18 @@
 have been caused by baseline noise alone.
 version 4.5.2
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
 too large error bars for magDrop
 version 4.5.0
 • fixes a bug introduced with the NE3 code changes that inhibited sub-frame timing
-adjustments.
-version 4.4.9
 
-• fixed yet another manisfestation of the bug introduced in version 4.2.1
+adjustments.
+version 4.4.9
+• fixed yet another manisfestation of the bug introduced in version 4.2.1
 version 4.4.8
 • fixed another manifestation of the bug introduced in version 4.2.1
 version 4.4.7
 • fixes a bug introduced in version 4.2.1 (February 8, 2022) that caused D values to be
 calculated as occurring 1 reading early
 version 4.4.5
 • added a checkbox to enable selection of whether or not the camera response curve is
@@ -369,19 +375,19 @@
 the less bumpy the normalized target curve is.
 When normalization is active, at each change, a pair of metrics are printed in the log
 panel.
 The red metric is the Pearson R value of the correlation between the target lightcurve
 and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
-The green metric is the standard deviation of the target lightcurve – it is lowered when
+
+The green metric is the standard deviation of the target lightcurve – it is lowered when
 the target lightcurve has a minimum slope and the fewest and shallowest bumps. Use
 the spinbox for the number of readings in the smoothing interval to minimize this
-
-number.
+number.
 version 4.3.5
 • made the 'step-by' buttons radio buttons so that it is clear what the current step size is.
 •
 
 removed the automatic switch to the Lightcurve panel
 
 version 4.3.3
@@ -416,19 +422,19 @@
 •
 
 adds 'step by' buttons that change the smoothing interval spinbox step size.
 
 version 4.2.6
 • tidies up the lightcurve panel a bit and changes color samples for target and reference
 curves.
-version 4.2.5
+
+version 4.2.5
 • completes implementation of the time shift (left/right shift) of the reference curve for
 normalization.
-
-•
+•
 
 adds dot color samples next to the lightcurve titles.
 
 version 4.2.4
 • makes tab/panel order sticky
 •
 
@@ -467,19 +473,19 @@
 row has a unique color other than blue or green.
 Lightcurves can be displaced up or down using the Y offset spinner to control the
 displacement. This affects the display position only; the underlying values are not
 affected. This facility was added to allow the separation of lightcurves that would
 otherwise overlap in a confusing manner.
 There can only be one lightcurve selected as target.
 There can be either 0 or 1 lightcurve selected as a reference for normalization.
-Normalization is applied whenever the normalization reference curve smoothing
+
+Normalization is applied whenever the normalization reference curve smoothing
 interval spinbox is changed from 0. Whenever this number is changed, a new
 normalization will result. If this number is returned to zero, all normalization is removed
-
-and the original values restored.
+and the original values restored.
 The X offset spinbox is not yet implemented. Its (future) purpose is to allow the
 reference curve used for normalization to be 'time shifted' for those cases where a
 drifting cloud affects lightcurves at slightly different times.
 •
 
 the normalization itself has been simplified so that no user input is needed other than
 the number of readings to be used in the smoothing procedure. The smoothing
@@ -519,18 +525,18 @@
 •
 
 Adds test to detectability routine so that the user cannot give an event duration that
 requires more points than are available in the observation.
 
 version 4.1.5
 • changed error bar calculation reporting so that the the value reported in the
-containment interval report matches that reported in the Excel final report when there is
-no asymmetry present.
 
-version 4.1.4
+containment interval report matches that reported in the Excel final report when there is
+no asymmetry present.
+version 4.1.4
 • This version adds tools needed to make best use of the Night Eagle 3 camera, the
 successor to the Night Eagle Astro camera (which is no longer in production). They are
 all grouped on a new tab page titled Night Eagle 3.
 •
 
 The Night Eagle 3 is a rolling shutter CMOS camera. As a result, with this camera, the
 timing of an occultation depends on which row the occulted star is at when the
@@ -585,18 +591,18 @@
 goodness of a 'fit'.
 
 •
 
 You will probably want to use the most aggressive noise reduction in most cases, but
 make sure that your expected event duration is long enough that the D transition
 exponential curve has time to settle to the bottom event plus some time to allow a good
-determination of the event bottom intensity. At DNR:HIGH, your expected event time
-should be greater than 30 frames (1 second) to use this setting.
 
-•
+determination of the event bottom intensity. At DNR:HIGH, your expected event time
+should be greater than 30 frames (1 second) to use this setting.
+•
 
 I suggest the following rules-of-thumb: can use DNR:HIGH for events 2 seconds and
 longer; can use DNR:MIDDLE for events 1 second and longer; can use DNR:LOW for
 events 0.5 seconds and longer.
 
 version 4.1.2
 • fixes bug when D only search has been selected
@@ -625,20 +631,21 @@
 curve can be used to extrat event times).
 Note: this only applies to csv files generated by PyMovie.
 version 4.0.6
 • minor GUI changes
 version 4.0.5
 • if you click outside the light-curve, the closest point will be toggled (so you don't have
 to zoom in to select the leftmost or rightmost point in a light-curve.
-•
+
+•
 
 When baseline statistics are calculated, they are reported as baseline mean and
 baseline snr (instead of just snr, which is the term we use when a drop is present).
 
-version 4.0.4
+version 4.0.4
 • a few GUI changes
 •
 
 removed the Use as secondary check box. Now if secondary curve is selected (spinner
 is non-zero), it will be used automatically.
 
 version 4.0.3
@@ -672,18 +679,18 @@
 lightCurveDirectory\DetectibilityPlots\
 In addition, if you supply a duration step size, which is the way to ask the detectibilty
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
 plotted.
 All of the above is just to cut down on clutter in the light-curve directory and to only plot
 meaningful graphics generated during the minimum duration search.
-version 3.9.9
-• whew! 3.9.8 did solve the sizing issue. So it is safe to get back in the water so...
 
-This version just improves the right-click context help for buttons in the new
+version 3.9.9
+• whew! 3.9.8 did solve the sizing issue. So it is safe to get back in the water so...
+This version just improves the right-click context help for buttons in the new
 Detectibility calculator.
 version 3.9.8
 • one more attempt to solve the gui sizing issue.
 •
 
 'sticky' settings are back but are now stored in pyote.ini instead of the
 obscure simple-ote.ini
@@ -710,18 +717,18 @@
 series of 'detectibility' calculations will be made at decreasing durations until the falsepositive probability becomes non-zero. A unique .png (incorporates duration and
 magDrop in the file name) will be written to the directory of the light-curve and the final
 plot where detection failed will be left on-screen.
 If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
 version 3.9.4
 • attempts to fix over-size initial gui.
-version 3.9.3
-• makes various improvements to the 'detectability' calculator to make it easier to use.
 
-version 3.9.2
+version 3.9.3
+• makes various improvements to the 'detectability' calculator to make it easier to use.
+version 3.9.2
 • adds a 'detectability' calculator for use in pre-planning event observation.
 •
 
 'scrunched' the left panel buttons together to make more room for the user to move the
 horizontal splitter up (which gives more room to view the lower right panel where the
 report gets printed).
 I think that this is kind of ugly, and it can be easily returned to the more spacious format
@@ -751,18 +758,18 @@
 version 3.8.5
 • changed the way QGridLayout was referenced.
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
 accommodate the latest Anaconda version, which has reorganized where those
 modules are stored. A similar change was made in version 3.7.6 and I do not know
 how this has gone uncorrected for so long – I hope that I have not missed something.
-version 3.8.3
-• adds display of light-curve name (if available in the csv file) to the curve-to-be-analyzed
 
-and the normalization curve next to their selection spinners.
+version 3.8.3
+• adds display of light-curve name (if available in the csv file) to the curve-to-be-analyzed
+and the normalization curve next to their selection spinners.
 version 3.8.2
 • 3.7.5 introduced a scrollable GUI for small screens. Unfortunately, that caused resizing
 problem for all users. The version reverts back to the original GUI design.
 •
 
 Added a print to the command window of the version number for diagnostic purposes.
 It will help clarify the situation when an installation has somehow managed to have
@@ -792,19 +799,19 @@
 • if timestamps are available in the csv file, they are used as x axis labels in the main
 plot.
 version 3.7.6
 • changed the way QMainWindow and Qapplication were referenced to accommodate
 the latest Anaconda version, which has reorganized where those modules are stored.
 This was causing a fatal startup error.
 version 3.7.5
-• changes the routine that looks for the latest version of PyOTE to one provided by Kia
+
+• changes the routine that looks for the latest version of PyOTE to one provided by Kia
 Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
-
-a special feature of pip (the loader that get programs from the PyPI repository) that was
+a special feature of pip (the loader that get programs from the PyPI repository) that was
 marked as 'unsupported'. That worked for many years until the pip programmers
 removed the 'special feature' as was their right (and the implicit promise/warning, I
 guess). This caused several users to always get a message that they were not running
 the most recent version of PyOTE, even though they were. Again: thanks to Kia
 Getrost for researching the problem and even supplying correct code (worked first
 time!) for me to use.
 • The GUI has been changed so that scroll bars will appear when the standard GUI size
@@ -834,19 +841,19 @@
 
 version 3.6.8
 • adds modeling of off centerline observations to lightcurve calibration curve
 generation
 version 3.6.7
 • clarified the location of the Enable Manual Timestamp Entry checkbox in the
 pop-up message appears when there are no timestamps in the csv file.
-version 3.6.6
+
+version 3.6.6
 • modified the lightcurve demo to show more clearly the camera exposure
 function and the star intensity function that are convolved with the diffraction
-
-lightcurve to produce the lightcurve as seen by the camera.
+lightcurve to produce the lightcurve as seen by the camera.
 The right-click help connected to the Demo button has been expanded to
 include a discussion of the convolution operation and hopefully provide some
 context to aid in understanding the star and camera function plots.
 version 3.6.5
 • added advisory message when False Positive probability plot appears in hopes
 of stemming in-discriminant use of this number as a 'decider' between a 'miss'
 and a 'positive' for an observation.
@@ -869,18 +876,18 @@
 help associated with the … fill Excel report button
 version 3.6.0
 • provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
 the … write report button
-NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
-requested) during your report to OccultWatcher ...
 
-… MUST BE CONVERTED to .xlsx for use by PyOTE!
+NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
+requested) during your report to OccultWatcher ...
+… MUST BE CONVERTED to .xlsx for use by PyOTE!
 … For Windows users, Excel will read an .xls file and save it as .xlsx
 … For Mac/Linux users, LibreOffice will read an .xls file and save it as .xlsx
 Sorry about this extra step, but it was necessary. The downstream tools used by area
 coordinators work equally well with the .xls and .xlsx forms of the spreadsheet, so there is no
 problem sending in the .xlsx version.
 What gets filled in for you is:
 ...D/R uncorrected times
@@ -905,24 +912,21 @@
 version 3.5.6
 • fixed a bug that kept a user from selecting a new file to read if PyOTE had been
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
 • fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
-through the event finder because they were a different type (coding error)
-version 3.5.4
 
-•
-
-made the 'get newest version' code identical to that in PyMovie in hopes that
+through the event finder because they were a different type (coding error)
+version 3.5.4
+• made the 'get newest version' code identical to that in PyMovie in hopes that
 that will resolve the issue that some people experience with pip (or python)
 installing downloaded pyote in a directory where it subsequently cannot be
 discovered. The change is minute, so I'm not optimistic, but it's worth a shot.
-
 version 3.5.3
 • removed the blank lines between header lines extracted from the csv file and
 placed in the log file --- this makes it easier to look at the newly added aperture
 settings (so just a tiny cosmetic change).
 version 3.5.2
 • Changed the 'smooth reference star procedure' to no longer display the points at
 the left and right ends; such points are actually extrapolated points with all the
@@ -954,20 +958,20 @@
 values and produce a 'trimmed' output file.
 
 •
 
 NEW: when a light curve has been 'normalized', the changed values are written
 to the data table where, once again, a 'write csv' process will capture the results.
 
-•
+•
 
 Added additional reminders that the start-of-exposure timestamp/timing
 convention is employed.
 
-version 3.4.9
+version 3.4.9
 • Added some explanatory language to the “Excel report” section regarding the
 proper interpretation of the 'false positive probability' number.
 version 3.4.8
 • This version deals more realistically with high magDrop lightcurves by defining a
 'limiting magDrop' as:
 limMagDrop = 2.5 * log10( B / std(A) )
 std(A) is the noise level of A.
@@ -991,27 +995,29 @@
 version 3.4.6
 • Adds AAV Version 2 file as a type that can be read (important when Do OCR
 check is enabled)
 version 3.4.5
 • Fixes block integration which was failing when more than 4 lightcurves were
 being processed.
 •
+version 3.4.4
 
 Made use diff and Do OCR checkboxes sticky.
 
-version 3.4.4
-• PyMovie files can have lightcurves extracted from more than 4 apertures (with
+•
+
+PyMovie files can have lightcurves extracted from more than 4 apertures (with
 user supplied names). This version allows all lightcurves from PyMovie files to
 be read and made available for processing. Prior to this change, only the first 4
-
-lightcurves were read.
+lightcurves were read.
 Note: when you change the lightcurve to be analyzed (with the spinner), the log
 panel will show the aperture name for that lightcurve. That happens when the
 reference lightcurve is changed as well.
 These changes are to PyMovie file treatment ONLY.
+
 version 3.4.3
 • Fixed bug that required an entry in dist(AU) and speed(km/sec) edit boxes for a
 solution to be found (the empty entries were causing an uncaught exception).
 The intention is that PyOTE should work as it always did if a user ignores the
 new lightcurve parameter panel and makes no entries. This 'fix' was required to
 make that happen.
 version 3.4.2
@@ -1040,19 +1046,17 @@
 installation. Find where it is by searching for example-penumbral.csv When
 you find it, copy or move it to some other folder because if you process it where
 it resides, other files will get added in your installation directory --- we really don't
 want extraneous non-program files floating around in your installation directory.
 To learn how to use the new procedure (which is a bit 'fiddly'), right-click on the
 penumbral fit checkbox --- be patient; play around.
 
-version 3.4.0
+version 3.4.0
 • Adds the ability to specify a diffraction lightcurve for use in timing the event. A
-new panel with edit boxes for asteroid/occulting body distance (in AU ---
-
-astronomical units) and asteroid/shadow speed (in km per second) has been
+new panel with edit boxes for asteroid/occulting body distance (in AU --astronomical units) and asteroid/shadow speed (in km per second) has been
 added. These values are needed in order to calculate a diffraction light curve.
 In addition to modeling diffraction effects, one can add the effect of a finite star
 disk to produce a penumbral curve. NOTE: PyOTE does not yet have the ability
 to correctly analyze a penumbral curve where it takes more than 1 or 2 readings
 for the transition. That project is under way and will be in the next version.
 version 3.3.9
 • Automatically installs cv2 if not already present. This package is needed for the
@@ -1082,19 +1086,19 @@
 best practice is to enter the D frame value in the spin box and visually confirm that the
 timestamp that you can see is the same as that extracted by the OCR procedure.
 Repeat for R.
 Another use for this feature is to handle the case where there is a visual timestamp, but
 either OCR was not activated during the .csv preparation, or the timestamp overlay
 came from an unsupported VTI type. The workflow would be to let PyOTE find the D
 and R frame values, but before pressing ... write report, do a Manual timestamp
-entry for the D and R frame entries found by viewing the relevant frames and entering
+
+entry for the D and R frame entries found by viewing the relevant frames and entering
 the correct times in the Manual timestamp dialog.
 It should be noted that the manual timestamp entry can be performed even when
-
-timestamps were already present in the file --- your manual entries will cause all the
+timestamps were already present in the file --- your manual entries will cause all the
 timestamps to be recalculated.
 version 3.3.5:
 • Changed usage of max([a, b ,c]) to max(a, b, c) to see if this allows the Numba
 JIT compiler to work for one user that found version 3.3.4 failed to load/compile.
 This should have no effect on users that already have version 3.3.4 working.
 version 3.3.4:
 • To shorten the time to find 'solutions', I used the Numba JIT (just-in-time)
@@ -1121,34 +1125,27 @@
 • Changed font size in help files --- it was fine for Mac but too big for Win10
 version 3.2.7
 • Removed the 'hover-for-help' and replaced it with a 'right-click-on-item' to get
 help. This scheme was introduced in PyMovie and I found it easier to use than
 the 'hover' scheme. In practice, the 'hover' popped up when it was not needed,
 so most users eventually disabled it. As a result, it became so tedious to look at
 help --- enable hover; hover; read; disable hover --- that the help system was
-used less and less. The right-click-for-help is always available and easily
+
+used less and less. The right-click-for-help is always available and easily
 invoked --- hopefully this will encourage more frequent reference to it.
 version 3.2.6
-
-•
-•
-•
-
-•
-
-This is a 'cosmetic' release --- there should be NO detectable differences from
+• This is a 'cosmetic' release --- there should be NO detectable differences from
 version 3.2.5 in terms of functionality.
-All python files were brought into compliance with PEP 8 coding standards.
+• All python files were brought into compliance with PEP 8 coding standards.
 Only I care about that.
-More significantly, I removed the dependency on C code by using Numba as a
+• More significantly, I removed the dependency on C code by using Numba as a
 code accelerator instead of Cython. As a result, I no longer need to compile
 separate code versions for Mac, Windows, and Linux. That makes my life
 easier, but you should experience no operational changes.
-All this 'cosmetic' work is in preparation for working on PyOTE issues again.
-
+• All this 'cosmetic' work is in preparation for working on PyOTE issues again.
 version 3.2.5
 • Added special test for Tangra files to detect the empty fields (which MUST be
 fixed) that Tangra outputs whenever it has trouble extracted a value from an
 aperture. It prints a message and stops all further processing, forcing the user
 to attend to and deal with the missing values.
 version 3.2.4
 • Modified the test for newer version to accommodate the different strings
@@ -1174,18 +1171,18 @@
 header/comment row --- the spreadsheet program did this to satisfy its internal
 requirement that every row have an equal number of columns. The result is
 superfluous commas at the end of data lines (that Tangra did NOT put there).
 Until this version, that 'butchered' file could not be read. This version adds code
 to parse data lines only up to the first non-empty column. Hopefully this will not
 have ramifications in the future (like a format change that has empty fields
 followed by non-empty fields --- not a likely expectation).
-version 3.2.0
-• Changed GUI to better align text on min max edit boxes to avoid confusion.
 
-version 3.1.9
+version 3.2.0
+• Changed GUI to better align text on min max edit boxes to avoid confusion.
+version 3.1.9
 • Fixed a bug in the test for a min/max solution search being constrained by a too
 large min value.
 version 3.1.8
 • version 3.1.7 was released without an updated version history. Here is what
 was changed in 3.1.7:
 •
 
@@ -1218,19 +1215,18 @@
 version 3.1.4:
 • Fixed error in new dropped reading detection logic when light curve was
 processed in field mode.
 •
 
 Cleaned up some language in tooltips.
 
-version 3.1.3:
+version 3.1.3:
 • Expanded manual timestamp preset time deltas to include NTSC and PAL field
 times. Also added ability to evaluate numeric expressions entered in the
-
-'Custom time' box: now you can type 1.001/60.0 in that box if you wish.
+'Custom time' box: now you can type 1.001/60.0 in that box if you wish.
 •
 
 Eliminated the 'entry num' column in the data matrix at the lower left of the GUI.
 The 'entry num' is unused and a possible source of confusion with the frame or
 field number for the unwary.
 
 •
@@ -1270,25 +1266,28 @@
 'report' button to the right in order to complete the process.
 
 version 3.1.0:
 • Added a Mac version of a pyote startup file. It is automatically placed on the
 Desktop the first time pyote is run. Double-clicking on that Desktop file icon will
 start pyote thereafter.
 version 3.0.8:
-• Added a Windows batch file to the distribution that, when executed, will startup
+
+•
+
+Added a Windows batch file to the distribution that, when executed, will startup
 pyote. The file is called PYOTE.bat and is automatically copied to
 C:\Anaconda3 (if it is not already there) when pyote is first run. Now, to create a
 clickable desktop icon for starting up pyote, a user need only go to the
-
-C:\Anaconda3 directory, locate the PYOTE.bat file, create a shortcut to it, and
+C:\Anaconda3 directory, locate the PYOTE.bat file, create a shortcut to it, and
 drag the shortcut to the desktop. Remember, that file does not appear until the
 first run of pyote.
 The ‘skipped’ version numbers were caused by the need for repeated testing of
 this new feature, each test requiring a new version, even though functionality did
 not change,
+
 version 3.0.1:
 • Restored the vertical splitter between the command/plot area and the
 table/report area. Somewhere along the line this capability was accidentally
 removed, and the lack of the splitter was not noticed. Now it’s back.
 version 3.0.0:
 • No code changes. This version is the same as 2.1.6 except that it is built on
 python 3.7. The previous versions used python 3.6. This allows new users to
@@ -1311,19 +1310,19 @@
 integration feature is employed. The edges now appear between data points so
 the bands are easier to see, particularly for 2 point block sizes.
 version 2.1.2:
 • To ease usage of the automatic block integration feature, accepting the
 automatically determined block integration parameters no longer uses a modal
 query box, which interfered with the ability to explore/expand the light curve plot.
 Now there is separate button which gets enabled after an automatic block
-integration completes.
+
+integration completes.
 version 2.1.1
 • Added progress bar tracking of block integration analysis because it can take an
-
-extended amount of time to complete the analysis when the light curve has
+extended amount of time to complete the analysis when the light curve has
 many points.
 version 2.1.0
 • Added automatic determination of 'correct' block size and offset for block
 integration when user clicks Block integrate button without selecting the two
 points normally required to specify integration block beginning and end. The
 user can choose to accept or reject pyote's opinion of the correct parameters to
 use when the automation determination is invoked.
@@ -1361,20 +1360,19 @@
 useful in general, but was particularly needed to support LED flash timing.
 Adds a checkbox to force manual entry of timestamp info. This is useful when
 OCR on a VTI timed light curve has catastrophic errors. It is always employed
 when using LED flash timing.
 During the error bar calculation, it is possible for the Cholesky decomposition
 needed for treating correlated noise to fail. Previous versions treated this as a
 fatal error and would not produce a final report. This version instead treats the
-noise as uncorrelated and continues processing to produce a final report.
 
+noise as uncorrelated and continues processing to produce a final report.
 version 2.0.6
 • Added additional instruction in the popup that appears when no timestamps are
-
-found in the csv file. This will give casual users additional guidance and
+found in the csv file. This will give casual users additional guidance and
 clarification for the manual timestamp entry process.
 version 2.0.5
 • files generated by pyote now contain PYOTE in the filename.
 •
 
 Timestamps can be corrupted to the point that a timeDelta of 0.0 can result.
 This version traps that event and reports it clearly --- 2.0.4 failed silently with a
@@ -1410,21 +1408,21 @@
 •
 
 removes unneeded 'analyze noise' buttons and rearranged other buttons to be
 in-line rather than one above the other to allow the vertical splitter between the
 plot area and report area more room to change (a help to those using screens
 with relatively low pixel densities).
 
-version 1.47
+version 1.47
 • adds bold red highlighting to message:
 ! There is something wrong with timestamps at D and/or R or frames have been dropped !
 
 so that it is harder to miss.
 
-version 1.46
+version 1.46
 • adds automatic recalculation of baseline and event noise parameters utilizing all
 available data points during a second solution pass; this removes the variability
 in calculated error bars due to user selection of a necessarily less complete set
 of data points for noise analysis during the first solution pass.
 •
 
 adds bold blue text in the 'Excel' portion of the final report to indicate whether or
```

### Comparing `pyote-5.3.2/src/pyoteapp/pyote.py` & `pyote-5.3.3/src/pyoteapp/pyote.py`

 * *Files 0% similar despite different names*

```diff
@@ -7227,40 +7227,44 @@
 
         if os.path.exists(metric_file_path):
             # self.showInfo('We will append to an existing fit_metric.csv file')
             pass
         else:
             # self.showInfo('We fill create a new fit_metric.csv file')
             with open(metric_file_path, 'w') as fileObject:
-                fileObject.writelines('aperture name,time err +/-secs,DNR,magDrop,'
+                fileObject.writelines('aperture name,time err +/-secs,DNR,FP metric,magDrop,'
                                       'percent drop,duration (secs),D time,'
                                       'R time,D frame,R frame,B,A,sigmaB,sigmaA,'
-                                      'observed drop,false positive drop,false positive margin,false positive metric\n')
+                                      'observed drop,FP drop,FP margin\n')
 
         with open(metric_file_path, 'a') as fileObject:
             # Start with the aperture name
             if self.targetKey == '':
                 self.targetKey = self.lightcurveTitles[0].text()
             new_data = self.targetKey
 
             margin = self.observedDrop - self.maxNoiseInducedDrop
             false_positive_metric = self.observedDrop / self.maxNoiseInducedDrop - 1.0
 
 
             # This works even for an Ronly event
             time_uncertainty = (self.deltaDhi95 - self.deltaDlo95) / 2.0 * self.timeDelta
-            new_data += f',{time_uncertainty:0.4f}'    # add time error bar
-            new_data += f',{self.snrB:0.2f}'           # add DNR
+            new_data += f',{time_uncertainty:0.4f}'       # add time error bar
+            new_data += f',{self.snrB:0.2f}'              # add DNR
+            new_data += f',{false_positive_metric:0.3f}'  # add false positive metric
+
 
             # add magDrop data
             new_data += f',{self.unvettedMagDrop:0.4f}'  # This gets displayed even if magDrop report would have suppressed it.
             new_data += f',{self.percentMagDrop:0.1f}'
 
             if self.eventType == 'DandR':
-                duration = (self.Rframe - self.Dframe) * (self.timeDelta / self.blockSize)
+                time_at_R = convertTimeStringToTime(self.Rtimestring)
+                time_at_D = convertTimeStringToTime(self.Dtimestring)
+                duration = time_at_R - time_at_D
             else:
                 duration = 0.0
             new_data += f',{duration:0.4f}'            # add duration
 
             # add D and R timestamps
             if self.eventType == 'Donly' or self.eventType == 'DandR':
                 new_data += f',{self.Dtimestring}'
@@ -7289,15 +7293,15 @@
             new_data += f',{self.sigmaB:0.2f}'
             new_data += f',{self.sigmaA:0.2f}'
 
             # add false positive data details
             new_data += f',{self.observedDrop:0.1f}'
             new_data += f',{self.maxNoiseInducedDrop:0.1f}'
             new_data += f',{margin:0.1f}'
-            new_data += f',{false_positive_metric:0.3f}'  # add false positive metric
+            # new_data += f',{false_positive_metric:0.3f}'  # add false positive metric
 
             self.showMsg("")
 
             fileObject.writelines(f'{new_data}\n')
 
         return
```

### Comparing `pyote-5.3.2/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.3.3/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/showVideoFrames.py` & `pyote-5.3.3/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/solverUtils.py` & `pyote-5.3.3/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.3.3/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/timestampDialog.py` & `pyote-5.3.3/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.2/src/pyoteapp/timestampUtils.py` & `pyote-5.3.3/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

