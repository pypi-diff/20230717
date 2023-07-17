# Comparing `tmp/RACS-tools-2.1.5a0.tar.gz` & `tmp/RACS-tools-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RACS-tools-2.1.5a0.tar", last modified: Fri Mar 31 01:42:50 2023, max compression
+gzip compressed data, was "RACS-tools-2.2.2.tar", last modified: Mon Jul 17 01:11:09 2023, max compression
```

## Comparing `RACS-tools-2.1.5a0.tar` & `RACS-tools-2.2.2.tar`

### file list

```diff
@@ -1,31 +1,26 @@
-drwxr-xr-x   0 tho822   (728663)   286778        0 2023-03-31 01:42:50.155003 RACS-tools-2.1.5a0/
-drwxr-xr-x   0 tho822   (728663)   286778        0 2023-03-31 01:42:50.145871 RACS-tools-2.1.5a0/.github/
-drwxr-xr-x   0 tho822   (728663)   286778        0 2023-03-31 01:42:50.148965 RACS-tools-2.1.5a0/.github/workflows/
--rw-r--r--   0 tho822   (728663)   286778      238 2022-08-01 01:55:38.000000 RACS-tools-2.1.5a0/.github/workflows/black.yml
--rw-r--r--   0 tho822   (728663)   286778     1860 2023-03-31 01:37:12.000000 RACS-tools-2.1.5a0/.github/workflows/docker.yml
--rw-r--r--   0 tho822   (728663)   286778     1302 2022-12-21 05:04:31.000000 RACS-tools-2.1.5a0/.github/workflows/python-package.yml
--rw-r--r--   0 tho822   (728663)   286778     1907 2022-04-04 06:22:50.000000 RACS-tools-2.1.5a0/.gitignore
--rw-r--r--   0 tho822   (728663)   286778      539 2023-02-01 04:05:07.000000 RACS-tools-2.1.5a0/Dockerfile
--rw-r--r--   0 tho822   (728663)   286778     1520 2020-02-28 12:00:34.000000 RACS-tools-2.1.5a0/LICENSE
--rw-r--r--   0 tho822   (728663)   286778     9875 2023-03-31 01:42:50.154381 RACS-tools-2.1.5a0/PKG-INFO
-drwxr-xr-x   0 tho822   (728663)   286778        0 2023-03-31 01:42:50.151456 RACS-tools-2.1.5a0/RACS_tools.egg-info/
--rw-r--r--   0 tho822   (728663)   286778     9875 2023-03-31 01:42:49.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/PKG-INFO
--rw-------   0 tho822   (728663)   286778     6981 2021-01-06 02:54:45.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/PKG-INFO (1)
--rw-r--r--   0 tho822   (728663)   286778      600 2023-03-31 01:42:50.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/SOURCES.txt
--rw-r--r--   0 tho822   (728663)   286778        1 2023-03-31 01:42:49.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/dependency_links.txt
--rw-r--r--   0 tho822   (728663)   286778      141 2023-03-31 01:42:49.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/entry_points.txt
--rw-------   0 tho822   (728663)   286778       94 2020-09-04 02:42:47.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/requires (1).txt
--rw-r--r--   0 tho822   (728663)   286778       82 2023-03-31 01:42:49.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/requires.txt
--rw-r--r--   0 tho822   (728663)   286778       11 2023-03-31 01:42:49.000000 RACS-tools-2.1.5a0/RACS_tools.egg-info/top_level.txt
--rw-r--r--   0 tho822   (728663)   286778     9220 2023-03-31 01:42:26.000000 RACS-tools-2.1.5a0/README.md
--rw-r--r--   0 tho822   (728663)   286778      224 2022-04-20 01:48:43.000000 RACS-tools-2.1.5a0/environment.yml
-drwxr-xr-x   0 tho822   (728663)   286778        0 2023-03-31 01:42:50.153786 RACS-tools-2.1.5a0/racs_tools/
--rw-r--r--   0 tho822   (728663)   286778        0 2020-10-22 02:19:45.000000 RACS-tools-2.1.5a0/racs_tools/__init__.py
--rw-r--r--   0 tho822   (728663)   286778     5078 2022-12-08 07:12:39.000000 RACS-tools-2.1.5a0/racs_tools/au2.py
--rw-r--r--   0 tho822   (728663)   286778    24832 2023-03-31 01:40:23.000000 RACS-tools-2.1.5a0/racs_tools/beamcon_2D.py
--rw-r--r--   0 tho822   (728663)   286778    45772 2023-03-31 01:40:44.000000 RACS-tools-2.1.5a0/racs_tools/beamcon_3D.py
--rw-r--r--   0 tho822   (728663)   286778     5334 2023-02-01 04:05:28.000000 RACS-tools-2.1.5a0/racs_tools/convolve_uv.py
--rw-r--r--   0 tho822   (728663)   286778     4351 2020-10-22 03:16:56.000000 RACS-tools-2.1.5a0/racs_tools/gaussft.f
--rw-r--r--   0 tho822   (728663)   286778     7464 2022-12-08 07:12:39.000000 RACS-tools-2.1.5a0/racs_tools/getnoise_list.py
--rw-r--r--   0 tho822   (728663)   286778       38 2023-03-31 01:42:50.156227 RACS-tools-2.1.5a0/setup.cfg
--rw-r--r--   0 tho822   (728663)   286778     4284 2023-03-31 01:42:37.000000 RACS-tools-2.1.5a0/setup.py
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-17 01:11:09.925732 RACS-tools-2.2.2/
+-rw-------   0 tho822   (728663) staff       (20)     1520 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/LICENSE
+-rw-r--r--   0 tho822   (728663) staff       (20)    10024 2023-07-17 01:11:09.925549 RACS-tools-2.2.2/PKG-INFO
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-17 01:11:09.923469 RACS-tools-2.2.2/RACS_tools.egg-info/
+-rw-------   0 tho822   (728663) staff       (20)    10024 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/PKG-INFO
+-rw-------   0 tho822   (728663) staff       (20)      467 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/SOURCES.txt
+-rw-------   0 tho822   (728663) staff       (20)        1 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/dependency_links.txt
+-rw-------   0 tho822   (728663) staff       (20)      141 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/entry_points.txt
+-rw-------   0 tho822   (728663) staff       (20)       88 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/requires.txt
+-rw-------   0 tho822   (728663) staff       (20)       11 2023-07-17 01:11:09.000000 RACS-tools-2.2.2/RACS_tools.egg-info/top_level.txt
+-rw-------   0 tho822   (728663) staff       (20)     9371 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/README.md
+-rw-------   0 tho822   (728663) staff       (20)      116 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/pyproject.toml
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-17 01:11:09.924894 RACS-tools-2.2.2/racs_tools/
+-rw-------   0 tho822   (728663) staff       (20)        0 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/__init__.py
+-rw-------   0 tho822   (728663) staff       (20)     5078 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/au2.py
+-rw-------   0 tho822   (728663) staff       (20)    25109 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/beamcon_2D.py
+-rw-------   0 tho822   (728663) staff       (20)    46081 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/beamcon_3D.py
+-rw-------   0 tho822   (728663) staff       (20)     5334 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/convolve_uv.py
+-rw-------   0 tho822   (728663) staff       (20)     4351 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/gaussft.f
+-rw-------   0 tho822   (728663) staff       (20)     8308 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/racs_tools/getnoise_list.py
+-rw-r--r--   0 tho822   (728663) staff       (20)       38 2023-07-17 01:11:09.925769 RACS-tools-2.2.2/setup.cfg
+-rw-------   0 tho822   (728663) staff       (20)     4296 2023-07-17 01:10:25.000000 RACS-tools-2.2.2/setup.py
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-17 01:11:09.925322 RACS-tools-2.2.2/tests/
+-rw-------   0 tho822   (728663) staff       (20)     5831 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/tests/test_2d.py
+-rw-------   0 tho822   (728663) staff       (20)     6843 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/tests/test_3d.py
+-rw-------   0 tho822   (728663) staff       (20)     4349 2023-05-22 00:36:00.000000 RACS-tools-2.2.2/tests/test_noise.py
```

### Comparing `RACS-tools-2.1.5a0/LICENSE` & `RACS-tools-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.1.5a0/PKG-INFO` & `RACS-tools-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RACS-tools
-Version: 2.1.5a0
+Version: 2.2.2
 Summary: Useful scripts for RACS.
 Home-page: https://github.com/AlecThomson/RACS-tools
 Author: Alec Thomson
 Author-email: alec.thomson@csiro.au
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: mpi
 License-File: LICENSE
 
 
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
 The recommended way to install. First obtain `conda` from Anaconda or Miniconda. Clone this repo, build the environment, and activate:
@@ -188,24 +188,25 @@
                         epsilon for radio_beam.commonbeam.
   -n NSAMPS, --nsamps NSAMPS
                         nsamps for radio_beam.commonbeam.
 ```
 
 ```
 $ getnoise_list -h
-usage: getnoise_list [-h] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
+usage: getnoise_list [-h] [-s] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
 
  Find bad channels by checking statistics of each channel image.
 
 positional arguments:
   qfile                 Stokes Q fits file
   ufile                 Stokes U fits file
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -s, --save_noise      Save noise values to disk [default False]
   -b, --blank           Blank bad channels? [default False - just print out bad channels]
   -c CLIPLEV, --cliplev CLIPLEV
                         Clip level in sigma, make this number lower to be more aggressive [default 5]
   -i ITERATE, --iterate ITERATE
                         Iterate flagging check N times [dafult 1 -- one pass only]
   -f FILE, --file FILE  Filename to write bad channel indices to file [None --  do not write]
 ```
```

### Comparing `RACS-tools-2.1.5a0/RACS_tools.egg-info/PKG-INFO` & `RACS-tools-2.2.2/RACS_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RACS-tools
-Version: 2.1.5a0
+Version: 2.2.2
 Summary: Useful scripts for RACS.
 Home-page: https://github.com/AlecThomson/RACS-tools
 Author: Alec Thomson
 Author-email: alec.thomson@csiro.au
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: mpi
 License-File: LICENSE
 
 
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
 The recommended way to install. First obtain `conda` from Anaconda or Miniconda. Clone this repo, build the environment, and activate:
@@ -188,24 +188,25 @@
                         epsilon for radio_beam.commonbeam.
   -n NSAMPS, --nsamps NSAMPS
                         nsamps for radio_beam.commonbeam.
 ```
 
 ```
 $ getnoise_list -h
-usage: getnoise_list [-h] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
+usage: getnoise_list [-h] [-s] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
 
  Find bad channels by checking statistics of each channel image.
 
 positional arguments:
   qfile                 Stokes Q fits file
   ufile                 Stokes U fits file
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -s, --save_noise      Save noise values to disk [default False]
   -b, --blank           Blank bad channels? [default False - just print out bad channels]
   -c CLIPLEV, --cliplev CLIPLEV
                         Clip level in sigma, make this number lower to be more aggressive [default 5]
   -i ITERATE, --iterate ITERATE
                         Iterate flagging check N times [dafult 1 -- one pass only]
   -f FILE, --file FILE  Filename to write bad channel indices to file [None --  do not write]
 ```
```

### Comparing `RACS-tools-2.1.5a0/README.md` & `RACS-tools-2.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
 The recommended way to install. First obtain `conda` from Anaconda or Miniconda. Clone this repo, build the environment, and activate:
@@ -168,24 +168,25 @@
                         epsilon for radio_beam.commonbeam.
   -n NSAMPS, --nsamps NSAMPS
                         nsamps for radio_beam.commonbeam.
 ```
 
 ```
 $ getnoise_list -h
-usage: getnoise_list [-h] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
+usage: getnoise_list [-h] [-s] [-b] [-c CLIPLEV] [-i ITERATE] [-f FILE] qfile ufile
 
  Find bad channels by checking statistics of each channel image.
 
 positional arguments:
   qfile                 Stokes Q fits file
   ufile                 Stokes U fits file
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -s, --save_noise      Save noise values to disk [default False]
   -b, --blank           Blank bad channels? [default False - just print out bad channels]
   -c CLIPLEV, --cliplev CLIPLEV
                         Clip level in sigma, make this number lower to be more aggressive [default 5]
   -i ITERATE, --iterate ITERATE
                         Iterate flagging check N times [dafult 1 -- one pass only]
   -f FILE, --file FILE  Filename to write bad channel indices to file [None --  do not write]
 ```
```

### Comparing `RACS-tools-2.1.5a0/racs_tools/au2.py` & `RACS-tools-2.2.2/racs_tools/au2.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.1.5a0/racs_tools/beamcon_2D.py` & `RACS-tools-2.2.2/racs_tools/beamcon_2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 #!/usr/bin/env python
 """ Convolve ASKAP images to common resolution """
 __author__ = "Alec Thomson"
 
-import logging as logger
+import logging
 import os
 import sys
 from functools import partial
 from hashlib import new
 from typing import Dict, List, Tuple
 
 import astropy.wcs
 import numpy as np
 import psutil
 import schwimmbad
 from astropy import units as u
 from astropy.io import ascii, fits
 from astropy.table import Table
+from astropy.wcs import WCS
+from astropy.wcs.utils import proj_plane_pixel_scales
 from radio_beam import Beam, Beams
 from radio_beam.utils import BeamError
 from tqdm import tqdm
 
 from racs_tools import au2
 from racs_tools.convolve_uv import smooth
 
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+
+
 #############################################
 #### ADAPTED FROM SCRIPT BY T. VERNSTROM ####
 #############################################
 
 
 def round_up(n: float, decimals: int = 0) -> float:
     """Round to number of decimals
@@ -130,17 +136,16 @@
         cubenm (str): File name of image.
 
     Returns:
         dict: Data and metadata.
     """
     logger.info(f"Getting image data from {cubenm}")
     with fits.open(cubenm, memmap=True, mode="denywrite") as hdu:
-
         w = astropy.wcs.WCS(hdu[0])
-        pixelscales = astropy.wcs.utils.proj_plane_pixel_scales(w)
+        pixelscales = proj_plane_pixel_scales(w)
 
         dxas = pixelscales[0] * u.deg
         dyas = pixelscales[1] * u.deg
 
         if len(hdu[0].data.shape) == 4:
             # has spectral, polarization axes
             data = hdu[0].data[0, 0]
@@ -323,39 +328,46 @@
                 [np.nan for beam in beams_list] * u.deg,
                 [np.nan for beam in beams_list] * u.deg,
                 [np.nan for beam in beams_list] * u.deg,
             )
             return nan_beam, nan_beams
     else:
         flags = np.array([False for beam in beams])
-    try:
-        cmn_beam = beams[~flags].common_beam(
-            tolerance=tolerance, epsilon=epsilon, nsamps=nsamps
-        )
-    except BeamError:
-        logger.warning(
-            "Couldn't find common beam with defaults\nTrying again with smaller tolerance"
-        )
-        cmn_beam = beams[~flags].common_beam(
-            tolerance=tolerance * 0.1, epsilon=epsilon, nsamps=nsamps
+
+    if not target_beam:
+        # Find the common beam
+        try:
+            cmn_beam = beams[~flags].common_beam(
+                tolerance=tolerance, epsilon=epsilon, nsamps=nsamps
+            )
+        except BeamError:
+            logger.warning(
+                "Couldn't find common beam with defaults\nTrying again with smaller tolerance"
+            )
+            cmn_beam = beams[~flags].common_beam(
+                tolerance=tolerance * 0.1, epsilon=epsilon, nsamps=nsamps
+            )
+
+        # Round up values
+        cmn_beam = Beam(
+            major=my_ceil(cmn_beam.major.to(u.arcsec).value, precision=1) * u.arcsec,
+            minor=my_ceil(cmn_beam.minor.to(u.arcsec).value, precision=1) * u.arcsec,
+            pa=round_up(cmn_beam.pa.to(u.deg), decimals=2),
         )
 
-    # Round up values
-    cmn_beam = Beam(
-        major=my_ceil(cmn_beam.major.to(u.arcsec).value, precision=1) * u.arcsec,
-        minor=my_ceil(cmn_beam.minor.to(u.arcsec).value, precision=1) * u.arcsec,
-        pa=round_up(cmn_beam.pa.to(u.deg), decimals=2),
-    )
+    else:
+        cmn_beam = target_beam
+
     target_header = header
-    w = astropy.wcs.WCS(target_header)
-    pixelscales = astropy.wcs.utils.proj_plane_pixel_scales(w)
+    w = WCS(target_header)
+    pixelscales = proj_plane_pixel_scales(w)
 
     dx = pixelscales[0] * u.deg
     dy = pixelscales[1] * u.deg
-    if not dx == dy:
+    if not np.isclose(dx, dy):
         raise Exception("GRID MUST BE SAME IN X AND Y")
     grid = dy
     if conv_mode != "robust":
         # Get the minor axis of the convolving beams
         minorcons = []
         for beam in beams:
             minorcons += [cmn_beam.deconvolve(beam).minor.to(u.arcsec).value]
@@ -549,15 +561,15 @@
         mask_count = 0
         failed = []
         for i, (beam, file) in enumerate(
             tqdm(
                 zip(allbeams, files),
                 total=len(allbeams),
                 desc="Deconvolving",
-                disable=(logger.root.level > logger.INFO),
+                disable=(logger.level > logging.INFO),
             )
         ):
             try:
                 target_beam.deconvolve(beam)
             except ValueError:
                 mask_count += 1
                 failed.append(file)
@@ -797,22 +809,22 @@
         try:
             myPE = psutil.Process().cpu_num()
         except AttributeError:
             myPE = 0
     if args.verbosity == 1:
         logger.basicConfig(
             filename=args.logfile,
-            level=logger.INFO,
+            level=logging.INFO,
             format=f"[{myPE}] %(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
     elif args.verbosity >= 2:
         logger.basicConfig(
             filename=args.logfile,
-            level=logger.DEBUG,
+            level=logging.DEBUG,
             format=f"[{myPE}] %(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
     pool = schwimmbad.choose_pool(mpi=args.mpi, processes=args.n_cores)
     if args.mpi:
         if not pool.is_master():
             pool.wait()
```

### Comparing `RACS-tools-2.1.5a0/racs_tools/beamcon_3D.py` & `RACS-tools-2.2.2/racs_tools/beamcon_3D.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """ Convolve ASKAP cubes to common resolution """
 __author__ = "Alec Thomson"
 
-import logging as log
+import logging
 import os
 import stat
 import sys
 import warnings
 from typing import Dict, List, Tuple
 
 import numpy as np
@@ -23,14 +23,17 @@
 from spectral_cube.utils import SpectralCubeWarning
 from tqdm import tqdm, trange
 
 from racs_tools import au2
 from racs_tools.beamcon_2D import my_ceil, round_up
 from racs_tools.convolve_uv import smooth
 
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+
 mpiSwitch = False
 if (
     os.environ.get("OMPI_COMM_WORLD_SIZE") is not None
     or int(os.environ.get("SLURM_NTASKS") or 1) > 1
 ):
     mpiSwitch = True
 
@@ -124,15 +127,15 @@
 
 
 def copyfileobj(fsrc, fdst, length=16 * 1024):
     # copied = 0
     total = os.fstat(fsrc.fileno()).st_size
     with tqdm(
         total=total,
-        disable=(log.root.level > log.INFO),
+        disable=(logger.level > logging.INFO),
         unit_scale=True,
         desc="Copying file",
     ) as pbar:
         while True:
             buf = fsrc.read(length)
             if not buf:
                 break
@@ -160,25 +163,25 @@
 
     # First check for CASA beams
     try:
         headcheck = header["CASAMBM"]
     except KeyError:
         headcheck = False
     if headcheck:
-        log.info(
+        logger.info(
             "CASA beamtable found in header - will use this table for beam calculations"
         )
         with fits.open(file) as hdul:
             hdu = hdul.pop("BEAMS")
             beams = Table.read(hdu)
 
     # Otherwise use beamlog file
     else:
-        log.info("No CASA beamtable found in header - looking for beamlogs")
-        log.info(f"Getting beams from {beamlog}")
+        logger.info("No CASA beamtable found in header - looking for beamlogs")
+        logger.info(f"Getting beams from {beamlog}")
 
         beams = Table.read(beamlog, format="ascii.commented_header")
         # Header looks like:
         # colnames=['Channel', 'BMAJarcsec', 'BMINarcsec', 'BPAdeg']
         # But needs some fix up - astropy can't read the header properly
         for col in beams.colnames:
             idx = col.find("[")
@@ -278,15 +281,15 @@
     axis_names = [i["coordinate_type"] for i in axis_type_dict]
     spec_idx = axis_names.index("spectral")
     slicer = [slice(None)] * len(cube.unmasked_data.shape)
     slicer[spec_idx] = idx
     slicer = tuple(slicer)
 
     plane = cube.unmasked_data[slicer].value.astype(np.float32)
-    log.debug(f"Size of plane is {(plane.nbytes*u.byte).to(u.MB)}")
+    logger.debug(f"Size of plane is {(plane.nbytes*u.byte).to(u.MB)}")
     newim = smooth(image=plane, **kwargs)
     return newim
 
 
 def makedata(files: List[str], outdir: str) -> Dict[str, dict]:
     """Create data dictionary.
 
@@ -312,15 +315,15 @@
         pixelscales = proj_plane_pixel_scales(w)
 
         dxas = pixelscales[0] * u.deg
         dyas = pixelscales[1] * u.deg
 
         datadict[f"cube_{i}"]["dx"] = dxas
         datadict[f"cube_{i}"]["dy"] = dyas
-        if not dxas == dyas:
+        if not np.isclose(dxas, dyas):
             raise Exception("GRID MUST BE SAME IN X AND Y")
         # Get beam info
         beam, nchan, beamlog = getbeams(file=file, header=header)
         datadict[f"cube_{i}"]["beamlog"] = beamlog
         datadict[f"cube_{i}"]["beam"] = beam
         datadict[f"cube_{i}"]["nchan"] = nchan
     return datadict
@@ -335,15 +338,15 @@
     target_beam: Beam = None,
     circularise: bool = False,
     tolerance: float = 0.0001,
     nsamps: int = 200,
     epsilon: float = 0.0005,
 ) -> Dict[str, dict]:
     """Find common beam for all channels.
-    Computed beams will be written to convolving beam log.
+    Computed beams will be written to convolving beam logger.
 
     Args:
         datadict (Dict[str, dict]): Main data dictionary.
         nchans (int): Number of channels.
         conv_mode (str, optional): Convolution mode. Defaults to "robust".
         mode (str, optional): Frequency mode. Defaults to "natural".
         target_beam (Beam, optional): Target PSF. Defaults to None.
@@ -360,15 +363,17 @@
     """
     if suffix is None:
         suffix = mode
     ### Natural mode ###
     if mode == "natural":
         big_beams = []
         for n in trange(
-            nchans, desc="Constructing beams", disable=(log.root.level > log.INFO)
+            nchans,
+            desc="Constructing beams",
+            disable=(logger.level > logging.INFO),
         ):
             majors_list = []
             minors_list = []
             pas_list = []
             for key in datadict.keys():
                 major = datadict[key]["beams"][n].major
                 minor = datadict[key]["beams"][n].minor
@@ -393,31 +398,31 @@
         # Find common beams
         bmaj_common = []
         bmin_common = []
         bpa_common = []
         for beams in tqdm(
             big_beams,
             desc="Finding common beam per channel",
-            disable=(log.root.level > log.INFO),
+            disable=(logger.level > logging.INFO),
             total=nchans,
         ):
             if all(np.isnan(beams)):
                 commonbeam = Beam(
                     major=np.nan * u.deg, minor=np.nan * u.deg, pa=np.nan * u.deg
                 )
             else:
                 try:
                     commonbeam = beams[~np.isnan(beams)].common_beam(
                         tolerance=tolerance,
                         nsamps=nsamps,
                         epsilon=epsilon,
                     )
                 except BeamError:
-                    log.warn("Couldn't find common beam with defaults")
-                    log.warn("Trying again with smaller tolerance")
+                    logger.warn("Couldn't find common beam with defaults")
+                    logger.warn("Trying again with smaller tolerance")
 
                     commonbeam = beams[~np.isnan(beams)].common_beam(
                         tolerance=tolerance * 0.1,
                         nsamps=nsamps,
                         epsilon=epsilon,
                     )
                 # Round up values
@@ -455,20 +460,20 @@
                             * u.arcsec,
                             minor=my_ceil(
                                 nyq_beam.minor.to(u.arcsec).value, precision=1
                             )
                             * u.arcsec,
                             pa=round_up(nyq_beam.pa.to(u.deg), decimals=2),
                         )
-                        log.info(
+                        logger.info(
                             f"Smallest common Nyquist sampled beam is: {nyq_beam!r}"
                         )
 
-                        log.warn("COMMON BEAM WILL BE UNDERSAMPLED!")
-                        log.warn("SETTING COMMON BEAM TO NYQUIST BEAM")
+                        logger.warn("COMMON BEAM WILL BE UNDERSAMPLED!")
+                        logger.warn("SETTING COMMON BEAM TO NYQUIST BEAM")
                         commonbeam = nyq_beam
 
             bmaj_common.append(commonbeam.major.to(u.arcsec).value)
             bmin_common.append(commonbeam.minor.to(u.arcsec).value)
             bpa_common.append(commonbeam.pa.to(u.deg).value)
 
         bmaj_common *= u.arcsec
@@ -498,24 +503,24 @@
         pas = np.array(pas_list).ravel()
 
         majors *= u.arcsec
         minors *= u.arcsec
         pas *= u.deg
         big_beams = Beams(major=majors, minor=minors, pa=pas)
 
-        log.info("Finding common beam across all channels")
-        log.info("This may take some time...")
+        logger.info("Finding common beam across all channels")
+        logger.info("This may take some time...")
 
         try:
             commonbeam = big_beams[~np.isnan(big_beams)].common_beam(
                 tolerance=tolerance, nsamps=nsamps, epsilon=epsilon
             )
         except BeamError:
-            log.warn("Couldn't find common beam with defaults")
-            log.warn("Trying again with smaller tolerance")
+            logger.warn("Couldn't find common beam with defaults")
+            logger.warn("Trying again with smaller tolerance")
 
             commonbeam = big_beams[~np.isnan(big_beams)].common_beam(
                 tolerance=tolerance * 0.1, nsamps=nsamps, epsilon=epsilon
             )
         if target_beam is not None:
             commonbeam = target_beam
         else:
@@ -545,48 +550,48 @@
                 nyq_beam = Beam(
                     major=my_ceil(nyq_beam.major.to(u.arcsec).value, precision=1)
                     * u.arcsec,
                     minor=my_ceil(nyq_beam.minor.to(u.arcsec).value, precision=1)
                     * u.arcsec,
                     pa=round_up(nyq_beam.pa.to(u.deg), decimals=2),
                 )
-                log.info(f"Smallest common Nyquist sampled beam is: {nyq_beam!r}")
+                logger.info(f"Smallest common Nyquist sampled beam is: {nyq_beam!r}")
                 if target_beam is not None:
                     commonbeam = target_beam
                     if target_beam < nyq_beam:
-                        log.warn("TARGET BEAM WILL BE UNDERSAMPLED!")
+                        logger.warn("TARGET BEAM WILL BE UNDERSAMPLED!")
                         raise Exception("CAN'T UNDERSAMPLE BEAM - EXITING")
                 else:
-                    log.warn("COMMON BEAM WILL BE UNDERSAMPLED!")
-                    log.warn("SETTING COMMON BEAM TO NYQUIST BEAM")
+                    logger.warn("COMMON BEAM WILL BE UNDERSAMPLED!")
+                    logger.warn("SETTING COMMON BEAM TO NYQUIST BEAM")
                     commonbeam = nyq_beam
 
         # Make Beams object
         commonbeams = Beams(
             major=[commonbeam.major] * nchans * commonbeam.major.unit,
             minor=[commonbeam.minor] * nchans * commonbeam.minor.unit,
             pa=[commonbeam.pa] * nchans * commonbeam.pa.unit,
         )
 
     if circularise:
-        log.info("Circular beam requested, setting BMIN=BMAJ and BPA=0")
+        logger.info("Circular beam requested, setting BMIN=BMAJ and BPA=0")
         commonbeams = Beams(
             major=commonbeams.major,
             minor=commonbeams.major,
             pa=commonbeams.pa * 0,
         )
 
-    log.info("Final beams are:")
+    logger.info("Final beams are:")
     for i, commonbeam in enumerate(commonbeams):
-        log.info(f"Channel {i}: {commonbeam!r}")
+        logger.info(f"Channel {i}: {commonbeam!r}")
 
     for key in tqdm(
         datadict.keys(),
         desc="Getting convolution data",
-        disable=(log.root.level > log.INFO),
+        disable=(logger.level > logging.INFO),
     ):
         # Get convolving beams
         conv_bmaj = []
         conv_bmin = []
         conv_bpa = []
         old_beams = datadict[key]["beams"]
         masks = datadict[key]["mask"]
@@ -605,15 +610,15 @@
                 )
                 if commonbeam == old_beam_check:
                     convbeam = Beam(
                         major=0 * u.deg,
                         minor=0 * u.deg,
                         pa=0 * u.deg,
                     )
-                    log.warn(
+                    logger.warn(
                         f"New beam {commonbeam!r} and old beam {old_beam_check!r} are the same. Won't attempt convolution."
                     )
 
                 else:
                     convbeam = commonbeam.deconvolve(old_beam)
 
             conv_bmaj.append(convbeam.major.to(u.arcsec).value)
@@ -664,15 +669,15 @@
         commonbeam_tab.meta["comments"] = [units]
         ascii.write(
             commonbeam_tab,
             output=commonbeam_log,
             format="commented_header",
             overwrite=True,
         )
-        log.info(f"Convolving log written to {commonbeam_log}")
+        logger.info(f"Convolving log written to {commonbeam_log}")
 
     return datadict
 
 
 def masking(nchans: int, datadict: dict, cutoff: u.Quantity = None) -> dict:
     """Apply masking to data.
 
@@ -720,15 +725,15 @@
     Args:
         datadict (dict): Main data dict - indexed
         mode (str): 'total' or 'natural'
 
     Returns:
         datadict: Updated datadict
     """
-    log.debug(f"Reading {filename}")
+    logger.debug(f"Reading {filename}")
     with fits.open(filename, memmap=True, mode="denywrite") as hdulist:
         primary_hdu = hdulist[0]
         data = primary_hdu.data
         header = primary_hdu.header
         wcs = WCS(header)
 
     ## Header
@@ -755,26 +760,26 @@
     ref_psf = commonbeams[crindex]
     # Check the Stokes
     stokes_axis = wcs.sub(["stokes"])
     if stokes_axis.array_shape == ():
         raise ValueError("No Stokes axis found")
     nstokes = stokes_axis.array_shape[0]
     if nstokes > 1:
-        log.critical(
+        logger.critical(
             f"More than one Stokes parameter in header. Only the first one will be used."
         )
     pols = np.zeros_like(chans)  # Zeros because we take the first one
     if any(
         (
             np.isnan(ref_psf.major.value),
             np.isnan(ref_psf.minor.value),
             np.isnan(ref_psf.pa.value),
         )
     ):
-        log.warning("Reference PSF is NaN - replacing with 0 in the header")
+        logger.warning("Reference PSF is NaN - replacing with 0 in the header")
         ref_psf = Beam(major=0 * u.deg, minor=0 * u.deg, pa=0 * u.deg)
         header["COMMENT"] = "Reference PSF is NaN"
         header["COMMENT"] = "- This is likely because the reference channel is masked."
         header["COMMENT"] = "- It has been replaced with 0 to keep FITS happy."
     header = ref_psf.attach_to_header(header)
     primary_hdu = fits.PrimaryHDU(data=data, header=header)
     if mode == "natural":
@@ -816,15 +821,15 @@
         suffix = mode
     outname = os.path.basename(filename)
     outname = outname.replace(".fits", f".{suffix}.fits")
     if prefix is not None:
         outname = prefix + outname
 
     outfile = os.path.join(outdir, outname)
-    log.info(f"Initialising to {outfile}")
+    logger.info(f"Initialising to {outfile}")
     new_hdulist.writeto(outfile, overwrite=True)
 
     return outfile
 
 
 def readlogs(commonbeam_log: str) -> Tuple[Beams, Beams, np.ndarray]:
     """Read convolving log files
@@ -834,15 +839,15 @@
 
     Raises:
         Exception: If the log file is not found
 
     Returns:
         Tuple[Beams, Beams, np.ndarray]: Common beams, convolving beams, and scaling factors
     """
-    log.info(f"Reading from {commonbeam_log}")
+    logger.info(f"Reading from {commonbeam_log}")
     try:
         commonbeam_tab = Table.read(commonbeam_log, format="ascii.commented_header")
     except FileNotFoundError:
         raise Exception("beamlogConvolve must be co-located with image")
     # Convert to Beams
     commonbeams = Beams(
         major=commonbeam_tab["Target BMAJ"] * u.arcsec,
@@ -851,17 +856,17 @@
     )
     convbeams = Beams(
         major=commonbeam_tab["Convolving BMAJ"] * u.arcsec,
         minor=commonbeam_tab["Convolving BMIN"] * u.arcsec,
         pa=commonbeam_tab["Convolving BPA"] * u.deg,
     )
     facs = np.array(commonbeam_tab["Convolving factor"])
-    log.info("Final beams are:")
+    logger.info("Final beams are:")
     for i, commonbeam in enumerate(commonbeams):
-        log.info(f"Channel {i}: {commonbeam!r}")
+        logger.info(f"Channel {i}: {commonbeam!r}")
     return commonbeams, convbeams, facs
 
 
 def main(
     infile: list,
     uselogs: bool = False,
     mode: str = "natural",
@@ -884,65 +889,67 @@
 
     Args:
         args (args): Command line args
 
     """
 
     if myPE == 0:
-        log.info(f"Total number of MPI ranks = {nPE}")
+        logger.info(f"Total number of MPI ranks = {nPE}")
         # Parse args
         if dryrun:
-            log.info("Doing a dry run -- no files will be saved")
+            logger.info("Doing a dry run -- no files will be saved")
 
         # Check mode
-        log.info(f"Mode is {mode}")
+        logger.info(f"Mode is {mode}")
         if mode == "natural" and mode == "total":
             raise Exception("'mode' must be 'natural' or 'total'")
         if mode == "natural":
-            log.info("Smoothing each channel to a common resolution")
+            logger.info("Smoothing each channel to a common resolution")
         if mode == "total":
-            log.info("Smoothing all channels to a common resolution")
+            logger.info("Smoothing all channels to a common resolution")
 
         # Check cutoff
         if cutoff is not None:
             cutoff *= u.arcsec
-            log.info(f"Cutoff is: {cutoff}")
+            logger.info(f"Cutoff is: {cutoff}")
 
         # Check target
-        log.debug(conv_mode)
+        logger.debug(conv_mode)
         if (
             not conv_mode == "robust"
             and not conv_mode == "scipy"
             and not conv_mode == "astropy"
             and not conv_mode == "astropy_fft"
         ):
             raise Exception("Please select valid convolution method!")
 
-        log.info(f"Using convolution method {conv_mode}")
+        logger.info(f"Using convolution method {conv_mode}")
         if conv_mode == "robust":
-            log.info("This is the most robust method. And fast!")
+            logger.info("This is the most robust method. And fast!")
         elif conv_mode == "scipy":
-            log.info("This fast, but not robust to NaNs or small PSF changes")
+            logger.info("This fast, but not robust to NaNs or small PSF changes")
         else:
-            log.info("This is slower, but robust to NaNs, but not to small PSF changes")
+            logger.info(
+                "This is slower, but robust to NaNs, but not to small PSF changes"
+            )
 
         nonetest = [test is None for test in [bmaj, bmin, bpa]]
 
         if not all(nonetest) and mode != "total":
             raise Exception("Only specify a target beam in 'total' mode")
 
         if all(nonetest):
             target_beam = None
 
         elif not all(nonetest) and any(nonetest):
             raise Exception("Please specify all target beam params!")
 
         elif not all(nonetest) and not any(nonetest):
             target_beam = Beam(bmaj * u.arcsec, bmin * u.arcsec, bpa * u.deg)
-            log.info(f"Target beam is {target_beam!r}")
+            logger.info(f"Target beam is {target_beam!r}")
 
         files = sorted(infile)
         if files == []:
             raise Exception("No files found!")
 
         if outdir is not None:
             if outdir[-1] == "/":
@@ -994,15 +1001,15 @@
                 suffix=suffix,
                 circularise=circularise,
                 tolerance=tolerance,
                 nsamps=nsamps,
                 epsilon=epsilon,
             )
         else:
-            log.info("Reading from convolve beamlog files")
+            logger.info("Reading from convolve beamlog files")
             for key in datadict.keys():
                 commonbeam_log = datadict[key]["beamlog"].replace(
                     ".txt", f".{suffix}.txt"
                 )
                 commonbeams, convbeams, facs = readlogs(commonbeam_log)
                 # Save to datadict
                 datadict[key]["facs"] = facs
@@ -1017,15 +1024,15 @@
 
     if mpiSwitch:
         comm.Barrier()
 
     # Init the files in parallel
     if not dryrun:
         if myPE == 0:
-            log.info("Initialising output files")
+            logger.info("Initialising output files")
         if mpiSwitch:
             files = comm.bcast(files, root=0)
             datadict = comm.bcast(datadict, root=0)
             nchans = comm.bcast(nchans, root=0)
 
         inputs = list(datadict.keys())
         dims = len(inputs)
@@ -1044,16 +1051,16 @@
 
             else:
                 # The remaining 'size - remainder' ranks get 'count' task each
                 my_start = myPE * count + rem
                 my_end = my_start + (count - 1)
 
         if myPE == 0:
-            log.info(f"There are {dims} files to init")
-        log.debug(f"My start is {my_start}, my end is {my_end}")
+            logger.info(f"There are {dims} files to init")
+        logger.debug(f"My start is {my_start}, my end is {my_end}")
 
         # Init output files and retrieve file names
         outfile_dict = {}
         for inp in inputs[my_start : my_end + 1]:
             outfile = initfiles(
                 filename=datadict[inp]["filename"],
                 commonbeams=datadict[inp]["commonbeams"],
@@ -1072,15 +1079,14 @@
             outlist = [outfile_dict]
 
         if mpiSwitch:
             comm.Barrier()
 
         # Now do the convolution in parallel
         if myPE == 0:
-
             # Conver list to dict and save to main dict
             outlist_dict = {}
             for d in outlist:
                 outlist_dict.update(d)
             # Also make inputs list
             inputs = []
             for key in datadict.keys():
@@ -1107,21 +1113,21 @@
             my_end = my_start + count
 
         else:
             # The remaining 'size - remainder' ranks get 'count' task each
             my_start = myPE * count + rem
             my_end = my_start + (count - 1)
         if myPE == 0:
-            log.info(f"There are {nchans} channels, across {len(files)} files")
-        log.debug(f"My start is {my_start}, my end is {my_end}")
+            logger.info(f"There are {nchans} channels, across {len(files)} files")
+        logger.debug(f"My start is {my_start}, my end is {my_end}")
 
         for inp in inputs[my_start : my_end + 1]:
             key, chan = inp
             outfile = datadict[key]["outfile"]
-            log.debug(f"{outfile}  - channel {chan} - Started")
+            logger.debug(f"{outfile}  - channel {chan} - Started")
 
             cubedict = datadict[key]
             newim = worker(
                 filename=cubedict["filename"],
                 idx=chan,
                 dx=cubedict["dx"],
                 dy=cubedict["dy"],
@@ -1144,17 +1150,17 @@
                 slicer[stokes_idx] = 0  # only do single stokes
                 slicer = tuple(slicer)
 
                 outfh[0].data[slicer] = newim.astype(
                     np.float32
                 )  # make sure data is 32-bit
                 outfh.flush()
-            log.info(f"{outfile}  - channel {chan} - Done")
+            logger.info(f"{outfile}  - channel {chan} - Done")
 
-    log.info("Done!")
+    logger.info("Done!")
     return datadict
 
 
 def cli():
     """Command-line interface"""
     import argparse
 
@@ -1344,24 +1350,24 @@
         default=200,
         help="nsamps for radio_beam.commonbeam.",
     )
 
     args = parser.parse_args()
 
     if args.verbosity == 1:
-        log.basicConfig(
+        logger.basicConfig(
             filename=args.logfile,
-            level=log.INFO,
+            level=logging.INFO,
             format=f"[{myPE}] %(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
     elif args.verbosity >= 2:
-        log.basicConfig(
+        logger.basicConfig(
             filename=args.logfile,
-            level=log.DEBUG,
+            level=logger.DEBUG,
             format=f"[{myPE}] %(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
 
     arg_dict = vars(args)
     # Pop the verbosity argument
     _ = arg_dict.pop("verbosity")
```

### Comparing `RACS-tools-2.1.5a0/racs_tools/convolve_uv.py` & `RACS-tools-2.2.2/racs_tools/convolve_uv.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.1.5a0/racs_tools/gaussft.f` & `RACS-tools-2.2.2/racs_tools/gaussft.f`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.1.5a0/racs_tools/getnoise_list.py` & `RACS-tools-2.2.2/racs_tools/getnoise_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python
 """ Find bad channels by checking statistics of each channel image. """
 
 import argparse
+import logging
 import warnings
 from typing import List, Tuple, Union
 
 import astropy.units as u
 import numpy as np
 from astropy.stats import mad_std
 from spectral_cube import SpectralCube
 from spectral_cube.utils import SpectralCubeWarning
 
 warnings.filterwarnings(action="ignore", category=SpectralCubeWarning, append=True)
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
 
 #############################################
 ####### ADAPTED FROM SCRIPT BY G. HEALD #####
 #############################################
 def getcube(filename: str) -> SpectralCube:
     """Read FITS file as SpectralCube
     Masks out 0Jy/beam pixels
@@ -33,24 +37,24 @@
     return cube
 
 
 def getbadchans(
     qcube: SpectralCube,
     ucube: SpectralCube,
     cliplev: float = 5,
-) -> np.ndarray:
+) -> Tuple[np.ndarray, u.Quantity, u.Quantity]:
     """Find bad channels in Stokes Q and U cubes
 
     Args:
         qcube (SpectralCube): Stokes Q data
         ucube (SpectralCube): Stokes U data
         cliplev (float, optional): Number stddev above median to clip. Defaults to 5.
 
     Returns:
-        np.ndarray: Bad channel boolean array
+        Tuple[np.ndarray, u.Quantity, u.Quantity]: Bad channels in Q, U, and noise spectra
     """
     assert len(ucube.spectral_axis) == len(qcube.spectral_axis)
 
     qnoisevals = (
         qcube.apply_function_parallel_spatial(
             function=mad_std,
             parallel=False,
@@ -66,33 +70,34 @@
             use_memmap=True,
             ignore_nan=True,
         )[:, 0, 0].unitless_filled_data[:]
         * ucube.unit
     )
     qmeannoise = np.nanmedian(qnoisevals)
     qstdnoise = mad_std(qnoisevals, ignore_nan=True)
-    print(
+    logger.info(
         f"Median Q noise=({qmeannoise.value:0.3f}±{qstdnoise.value:0.3f}) / ({qmeannoise.unit})"
     )
     umeannoise = np.nanmedian(unoisevals)
     ustdnoise = mad_std(unoisevals, ignore_nan=True)
-    print(
+    logger.info(
         f"Median U noise=({umeannoise.value:0.3f}±{ustdnoise.value:0.3f}) / ({umeannoise.unit})"
     )
     qbadones = np.logical_or(
         qnoisevals > (qmeannoise + cliplev * qstdnoise), ~np.isfinite(qnoisevals)
     )
     ubadones = np.logical_or(
         unoisevals > (umeannoise + cliplev * ustdnoise), ~np.isfinite(unoisevals)
     )
-    print(f"{qbadones.sum()} of {len(qcube.spectral_axis)} are bad in Q")
-    print(f"{ubadones.sum()} of {len(ucube.spectral_axis)} are bad in U")
+    logger.info(f"{qbadones.sum()} of {len(qcube.spectral_axis)} are bad in Q")
+    logger.info(f"{ubadones.sum()} of {len(ucube.spectral_axis)} are bad in U")
     total_bad = np.logical_or(qbadones, ubadones)
-    print(f"{total_bad.sum()} of {len(qcube.spectral_axis)} are bad in Q -or- U")
-    return total_bad
+    logger.info(f"{total_bad.sum()} of {len(qcube.spectral_axis)} are bad in Q -or- U")
+
+    return total_bad, qnoisevals, unoisevals
 
 
 def blankchans(
     qcube: SpectralCube, ucube: SpectralCube, totalbad: np.ndarray, blank: bool = False
 ) -> Tuple[SpectralCube, SpectralCube]:
     """Mask out bad channels
 
@@ -105,19 +110,19 @@
     Returns:
         Tuple[SpectralCube, SpectralCube]: _description_
     """
     chans = np.arange(len(qcube.spectral_axis))
     badchans = chans[totalbad]
     badfreqs = qcube.spectral_axis[totalbad]
     if not blank:
-        print(
+        logger.info(
             "Nothing will be blanked, but these are the channels/frequencies that would be with the -b option activated:"
         )
-    print(f"Bad channels are {badchans}")
-    print(f"Bad frequencies are {badfreqs}")
+    logger.info(f"Bad channels are {badchans}")
+    logger.info(f"Bad frequencies are {badfreqs}")
     totalgood = ~totalbad
     q_msk = qcube.mask_channels(totalgood)
     u_msk = ucube.mask_channels(totalgood)
     return q_msk, u_msk
 
 
 def writefits(qcube: SpectralCube, ucube: SpectralCube, qfile: str, ufile: str) -> None:
@@ -126,28 +131,29 @@
     Args:
         qcube (SpectralCube): Stokes Q data
         ucube (SpectralCube): Stokes U data
         qfile (str): Original Q file
         ufile (str): Original U file
     """
     outfile = qfile.replace(".fits", ".blanked.fits")
-    print(f"Writing to {outfile}")
+    logger.info(f"Writing to {outfile}")
     qcube.write(outfile, format="fits", overwrite=True)
     outfile = ufile.replace(".fits", ".blanked.fits")
-    print(f"Writing to {outfile}")
+    logger.info(f"Writing to {outfile}")
     ucube.write(outfile, format="fits", overwrite=True)
 
 
 def main(
     qfile: str,
     ufile: str,
     blank: bool = False,
     cliplev: float = 5,
     iterate: int = 1,
-    outfile: str = None,
+    outfile: Union[str, None] = None,
+    save_noise: bool = False,
 ) -> None:
     """Flag bad channels in Stokes Q and U cubes
 
     Args:
         qfile (str): Stokes Q fits file
         ufile (str): Stokes U fits file
         blank (bool, optional): Flag bad data and save to disk. Defaults to False.
@@ -160,27 +166,35 @@
 
     assert len(ucube.spectral_axis) == len(
         qcube.spectral_axis
     ), "Cubes have different number of channels"
 
     # Iterate
     for i in range(iterate):
-        print(f"Flagging iteration {i+1} of {iterate}")
-        totalbad = getbadchans(
+        logger.info(f"Flagging iteration {i+1} of {iterate}")
+        totalbad, qnoisevals, unoisevals = getbadchans(
             qcube,
             ucube,
             cliplev=cliplev,
         )
-        qcube, ucube = blankchans(qcube, ucube, totalbad, blank=blank)
+        qcube, ucube = blankchans(
+            qcube=qcube, ucube=ucube, totalbad=totalbad, blank=blank
+        )
+
+    if save_noise:
+        logger.info("Saving noise values to disk")
+        np.savetxt(qfile.replace(".fits", ".noise.txt"), qnoisevals.value)
+        np.savetxt(ufile.replace(".fits", ".noise.txt"), unoisevals.value)
 
     if blank:
-        writefits(qcube, qcube, qfile, ufile)
+        logger.warning("Overwriting original files")
+        writefits(qcube=qcube, ucube=ucube, qfile=qfile, ufile=ufile)
 
-    if outfile is not None:
-        print(f"Saving bad files to {outfile}")
+    if outfile:
+        logger.info(f"Saving bad files to {outfile}")
         np.savetxt(outfile, totalbad)
 
 
 def cli() -> None:
     warnings.filterwarnings(
         "ignore",
         message="Cube is a Stokes cube, returning spectral cube for I component",
@@ -193,14 +207,20 @@
     # Parse the command line options
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument("qfile", type=str, help="Stokes Q fits file")
     parser.add_argument("ufile", type=str, help="Stokes U fits file")
     parser.add_argument(
+        "-s",
+        "--save_noise",
+        help="Save noise values to disk [default False]",
+        action="store_true",
+    )
+    parser.add_argument(
         "-b",
         "--blank",
         help="Blank bad channels? [default False - just print out bad channels]",
         action="store_true",
     )
     parser.add_argument(
         "-c",
@@ -231,12 +251,13 @@
     main(
         qfile=args.qfile,
         ufile=args.ufile,
         blank=args.blank,
         cliplev=args.cliplev,
         iterate=args.iterate,
         outfile=args.file,
+        save_noise=args.save_noise,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `RACS-tools-2.1.5a0/setup.py` & `RACS-tools-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # Package meta-data.
 NAME = "RACS-tools"
 DESCRIPTION = "Useful scripts for RACS."
 URL = "https://github.com/AlecThomson/RACS-tools"
 EMAIL = "alec.thomson@csiro.au"
 AUTHOR = "Alec Thomson"
 REQUIRES_PYTHON = ">=3.8.0"
-VERSION = "2.1.5a"
+VERSION = "2.2.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
+    "numpy",
     "astropy",
     "radio_beam",
     "schwimmbad",
     "psutil",
     "scipy",
     "numpy",
     "spectral_cube",
```

