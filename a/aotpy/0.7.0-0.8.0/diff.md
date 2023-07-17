# Comparing `tmp/aotpy-0.7.0.tar.gz` & `tmp/aotpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.7.0.tar", last modified: Mon Jun 19 17:04:13 2023, max compression
+gzip compressed data, was "aotpy-0.8.0.tar", last modified: Mon Jul 17 15:39:51 2023, max compression
```

## Comparing `aotpy-0.7.0.tar` & `aotpy-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.298122 aotpy-0.7.0/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     2997 2023-06-19 17:04:13.298122 aotpy-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.210634 aotpy-0.7.0/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.7.0/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.245322 aotpy-0.7.0/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.7.0/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.7.0/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     3897 2023-06-05 13:40:11.000000 aotpy-0.7.0/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.7.0/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0      616 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1831 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.7.0/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.7.0/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.7.0/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3552 2023-06-19 16:50:55.000000 aotpy-0.7.0/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.246299 aotpy-0.7.0/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.254674 aotpy-0.7.0/aotpy/data/AOF/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.7.0/aotpy/data/AOF/subap.fits
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.257576 aotpy-0.7.0/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.7.0/aotpy/data/ERIS/ho_subap.fits
--rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.7.0/aotpy/data/ERIS/lo_subap.fits
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.263952 aotpy-0.7.0/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.7.0/aotpy/data/NAOMI/zernike_control_modes.fits
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.276639 aotpy-0.7.0/aotpy/data/PAPYRUS/
--rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.7.0/aotpy/data/PAPYRUS/T152_pupil.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.7.0/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.280545 aotpy-0.7.0/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.7.0/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.7.0/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.288359 aotpy-0.7.0/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.7.0/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26710 2023-06-19 16:49:27.000000 aotpy-0.7.0/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    42034 2023-06-19 16:49:27.000000 aotpy-0.7.0/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     9252 2023-06-19 16:19:02.000000 aotpy-0.7.0/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.7.0/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.297145 aotpy-0.7.0/aotpy/translators/
--rw-rw-rw-   0        0        0      432 2023-06-19 16:00:06.000000 aotpy-0.7.0/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0    11304 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     6993 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    18293 2023-06-19 16:47:44.000000 aotpy-0.7.0/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0    10438 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0     7412 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0     3642 2023-06-19 16:46:11.000000 aotpy-0.7.0/aotpy/translators/papyrus.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:04:13.232117 aotpy-0.7.0/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2997 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 17:04:13.000000 aotpy-0.7.0/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0     1029 2023-06-19 17:04:13.302035 aotpy-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.578629 aotpy-0.8.0/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2997 2023-07-17 15:39:51.578629 aotpy-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.527659 aotpy-0.8.0/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.0/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.545372 aotpy-0.8.0/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     5304 2023-07-17 15:34:04.000000 aotpy-0.8.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0     1162 2023-07-17 10:40:27.000000 aotpy-0.8.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1338 2023-07-17 12:24:43.000000 aotpy-0.8.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.546372 aotpy-0.8.0/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.548372 aotpy-0.8.0/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.0/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.0/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.549372 aotpy-0.8.0/aotpy/data/GALACSI/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.0/aotpy/data/GALACSI/subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.550372 aotpy-0.8.0/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.0/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.559459 aotpy-0.8.0/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.0/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.0/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.563459 aotpy-0.8.0/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.568543 aotpy-0.8.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26755 2023-07-17 08:56:36.000000 aotpy-0.8.0/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    41933 2023-07-06 15:43:11.000000 aotpy-0.8.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9284 2023-06-28 16:40:48.000000 aotpy-0.8.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31367 2023-07-17 09:16:43.000000 aotpy-0.8.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.577633 aotpy-0.8.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-0.8.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7087 2023-07-06 15:43:34.000000 aotpy-0.8.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18377 2023-07-06 15:47:56.000000 aotpy-0.8.0/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    10376 2023-06-28 16:36:06.000000 aotpy-0.8.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0    11408 2023-07-06 15:45:27.000000 aotpy-0.8.0/aotpy/translators/galacsi.py
+-rw-rw-rw-   0        0        0     7494 2023-07-06 15:45:40.000000 aotpy-0.8.0/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0     3658 2023-07-17 15:15:43.000000 aotpy-0.8.0/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.532658 aotpy-0.8.0/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2997 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1029 2023-07-17 15:39:51.579630 aotpy-0.8.0/setup.cfg
```

### Comparing `aotpy-0.7.0/LICENSE` & `aotpy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/PKG-INFO` & `aotpy-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.7.0/README.md` & `aotpy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/__init__.py` & `aotpy-0.8.0/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/__init__.py` & `aotpy-0.8.0/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/aberration.py` & `aotpy-0.8.0/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/atmosphere.py` & `aotpy-0.8.0/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/image.py` & `aotpy-0.8.0/aotpy/core/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,18 @@
 """
 
 from dataclasses import dataclass, field
 from typing import Any
 
 import numpy as np
 
+from .base import Metadatum
 from .time import Time
 
-__all__ = ['Image', 'Metadatum']
-
-
-@dataclass
-class Metadatum:
-    """Contains a set of key, value and (optionally) comment which describe the Image data in some aspect."""
-    key: str
-    "Identifier of the value."
-
-    value: Any
-    "Information that describes the Image data."
-
-    comment: str = None
-    "Optional description of the metadatum."
-
-    def to_tuple(self) -> tuple:
-        """ Return the `Metadatum` object expressed as a tuple (key, value, comment)."""
-        return self.key, self.value, self.comment
+__all__ = ['Image']
 
 
 @dataclass
 class Image:
     """Contains multidimensional data and the metadata related to it."""
 
     name: str
```

### Comparing `aotpy-0.7.0/aotpy/core/loop.py` & `aotpy-0.8.0/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/optical_sensor.py` & `aotpy-0.8.0/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/source.py` & `aotpy-0.8.0/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/telescope.py` & `aotpy-0.8.0/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/time.py` & `aotpy-0.8.0/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/core/wavefront_corrector.py` & `aotpy-0.8.0/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/data/AOF/subap.fits` & `aotpy-0.8.0/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/data/ERIS/ho_subap.fits` & `aotpy-0.8.0/aotpy/data/GALACSI/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/data/ERIS/lo_subap.fits` & `aotpy-0.8.0/aotpy/data/ERIS/lo_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-0.8.0/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/data/PAPYRUS/T152_pupil.fits` & `aotpy-0.8.0/aotpy/data/PAPYRUS/T152_pupil.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/io/base.py` & `aotpy-0.8.0/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/io/fits/_keywords.py` & `aotpy-0.8.0/aotpy/io/fits/_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,18 @@
 AOT_AO_MODE = 'AO-MODE'
 AOT_AO_MODE_SET = {'SCAO', 'SLAO', 'GLAO', 'MOAO', 'LTAO', 'MCAO'}
 AOT_TIMESYS = 'TIMESYS'
 AOT_TIMESYS_UTC = 'UTC'
 AOT_DATE_BEG = 'DATE-BEG'
 AOT_DATE_END = 'DATE-END'
 AOT_STREHL_RATIO = 'STREHL-R'
+AOT_SYSTEM_NAME = 'SYS-NAME'
 AOT_TEMPORAL_ERROR = 'TEMP-ERR'
 AOT_CONFIG = 'CONFIG'
-AOT_HEADER_SET = {AOT_VERSION, AOT_AO_MODE, AOT_TIMESYS, AOT_DATE_BEG, AOT_DATE_END, AOT_STREHL_RATIO,
+AOT_HEADER_SET = {AOT_VERSION, AOT_AO_MODE, AOT_TIMESYS, AOT_DATE_BEG, AOT_DATE_END, AOT_STREHL_RATIO, AOT_SYSTEM_NAME,
                   AOT_TEMPORAL_ERROR, AOT_CONFIG}
 
 REFERENCE_UID = 'UID'
 TIME_REFERENCE = 'TIME_UID'
 ABERRATION_REFERENCE = 'ABERRATION_UID'
 LASER_LAUNCH_TELESCOPE_REFERENCE = 'LLT_UID'
 DETECTOR_REFERENCE = 'DETECTOR_UID'
@@ -304,16 +305,16 @@
     AOTField(name=DETECTOR_TRANSMISSION, format=LIST_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_SKY_BACKGROUND, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_GAIN, format=FLOAT_FORMAT, unit=UNIT_ELECTRONS),
     AOTField(name=DETECTOR_EXCESS_NOISE, format=FLOAT_FORMAT, unit=UNIT_ELECTRONS),
     AOTField(name=DETECTOR_FILTER, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_BAD_PIXEL_MAP, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_DYNAMIC_RANGE, format=FLOAT_FORMAT, unit=UNIT_DECIBELS),
-    AOTField(name=DETECTOR_READOUT_RATE, format=STRING_FORMAT, unit=f'{UNIT_PIXELS}*{UNIT_SECONDS}^-1'),
-    AOTField(name=DETECTOR_FRAME_RATE, format=STRING_FORMAT, unit=f'{UNIT_FRAME}*{UNIT_SECONDS}^-1'),
+    AOTField(name=DETECTOR_READOUT_RATE, format=FLOAT_FORMAT, unit=f'{UNIT_PIXELS}*{UNIT_SECONDS}^-1'),
+    AOTField(name=DETECTOR_FRAME_RATE, format=FLOAT_FORMAT, unit=f'{UNIT_FRAME}*{UNIT_SECONDS}^-1'),
     AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[DETECTORS_TABLE] = DETECTOR_FIELDS
 
 # AOT_SCORING_CAMERAS fields
 SCORING_CAMERA_PUPIL_MASK = 'PUPIL_MASK'
 SCORING_CAMERA_WAVELENGTH = 'WAVELENGTH'
```

### Comparing `aotpy-0.7.0/aotpy/io/fits/reader.py` & `aotpy-0.8.0/aotpy/io/fits/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from . import _keywords as kw
-from .utils import FITSURLImage, FITSFileImage, image_from_hdu, keyword_is_relevant
+from .utils import FITSURLImage, FITSFileImage, image_from_hdu, keyword_is_relevant, metadatum_from_card
 from ..base import SystemReader
 
 _reference_pattern = re.compile(r'([^<]+)<(.+)>(\d+)?')
 
 
 def _type_matches(aot_format: str, fits_type: str) -> bool:
     try:
@@ -95,15 +95,14 @@
             kw.TELESCOPES_TABLE: self._telescopes,
             kw.SOURCES_TABLE: self._sources,
             kw.DETECTORS_TABLE: self._detectors,
             kw.WAVEFRONT_SENSORS_TABLE: self._wfss,
             kw.WAVEFRONT_CORRECTORS_TABLE: self._wfcs
         }
 
-        self._extra_header: list[fits.Card] = []
         self._extra_hdus: fits.HDUList = fits.HDUList()
         self._extra_columns: dict[str, list[fits.Column]] = {}
         self._extra_objects: list[aotpy.Referenceable] = []
 
     def _read(self, **kwargs) -> tuple[aotpy.AOSystem, list]:
         with fits.open(self._filename, **kwargs) as hdus:
             self._primary_header: fits.Header = hdus[0].header
@@ -157,15 +156,15 @@
             self._handle_detectors(hdus)
             self._handle_scoring_cameras(hdus)
             self._handle_wavefront_sensors(hdus)
             self._handle_wavefront_correctors(hdus)
             self._handle_loops(hdus)
 
             self._check_usage()
-            aux = [self._extra_header, self._extra_hdus, self._extra_columns, self._extra_objects]
+            aux = [self._extra_hdus, self._extra_columns, self._extra_objects]
             extra = aux if [x for x in aux if x] else None  # extra is None if everything is empty
             return self._system, extra
 
     def _check_header(self) -> aotpy.AOSystem:
         if kw.AOT_VERSION not in self._primary_header:
             raise ValueError(f"File is not in the AOT format or the mandatory '{kw.AOT_VERSION}' keyword is missing")
             # TODO do something with the version
@@ -205,37 +204,40 @@
                     end = datetime.fromisoformat(aux)
                 except (ValueError, TypeError):
                     warnings.warn(f"'{kw.AOT_DATE_END}' keyword not properly formatted.")
         except KeyError:
             pass
 
         try:
+            name = self._primary_header[kw.AOT_SYSTEM_NAME]
+        except KeyError:
+            name = None
+
+        try:
             strehl_ratio = self._primary_header[kw.AOT_STREHL_RATIO]
         except KeyError:
             strehl_ratio = None
 
         try:
             temporal_error = self._primary_header[kw.AOT_TEMPORAL_ERROR]
         except KeyError:
             temporal_error = None
 
         try:
             config = self._primary_header[kw.AOT_CONFIG]
         except KeyError:
             config = None
 
+        metadata = []
         for card in self._primary_header.cards:
             if card.keyword not in kw.AOT_HEADER_SET and keyword_is_relevant(card.keyword):
-                self._extra_header.append(card)
-        if self._extra_header and not self._extra_data_flag:
-            warnings.warn(f"""Header contains non-AOT keywords that were ignored: """
-                          f"""{', '.join([f"'{x.keyword}'" for x in self._extra_header])}""")
+                metadata.append(metadatum_from_card(card))
 
-        return aotpy.AOSystem(ao_mode=ao_mode, date_beginning=beg, date_end=end, strehl_ratio=strehl_ratio,
-                              temporal_error=temporal_error, config=config)
+        return aotpy.AOSystem(ao_mode=ao_mode, date_beginning=beg, date_end=end, name=name, strehl_ratio=strehl_ratio,
+                              temporal_error=temporal_error, config=config, metadata=metadata)
 
     def _check_bintable(self, hdus: fits.HDUList, table_name: str):
         fields = kw.TABLE_FIELDS[table_name]
         table = hdus[table_name]
         if not isinstance(table, fits.BinTableHDU):
             raise ValueError(f"HDU '{table.name}' must be a binary table")
```

### Comparing `aotpy-0.7.0/aotpy/io/fits/utils.py` & `aotpy-0.8.0/aotpy/io/fits/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     Get `Metadatum` from `Card`.
 
     Parameters
     ----------
     card
         `Card` to convert to `Metadatum`.
     """
-    return aotpy.Metadatum(card.keyword, card.value, card.comment)
+    return aotpy.Metadatum(card.keyword, card.value, card.comment if card.comment != '' else None)
 
 
 def metadata_from_hdu(hdu: fits.ImageHDU) -> list[aotpy.Metadatum]:
     """
     Get metadata (list of `Metadatum`) from HDU. Only relevant keywords are extracted.
 
     Parameters
```

### Comparing `aotpy-0.7.0/aotpy/io/fits/writer.py` & `aotpy-0.8.0/aotpy/io/fits/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,16 @@
     @staticmethod
     def _create_row_reference(uid: str) -> str:
         return f'{kw.ROW_REFERENCE}<{uid}>'
 
     def _handle_time(self, time: aotpy.Time) -> str | None:
         if time is None:
             return None
-        if time.timestamps and time.frame_numbers and len(time.timestamps) != len(time.frame_numbers):
+        if time.timestamps is not None and time.frame_numbers is not None \
+                and len(time.timestamps) != len(time.frame_numbers):
             raise ValueError(f"Error in Time '{time.uid}': If both 'timestamps' and 'frame_numbers' are non-null, they"
                              f"must have the same length.")
         row = {
             kw.REFERENCE_UID: time.uid,
             kw.TIME_TIMESTAMPS: time.timestamps,
             kw.TIME_FRAME_NUMBERS: time.frame_numbers
         }
@@ -513,34 +514,37 @@
             kw.LOOPS_DELAY: loop.delay,
             kw.LOOPS_TIME_FILTER_NUM: self._handle_image(loop.time_filter_num),
             kw.LOOPS_TIME_FILTER_DEN: self._handle_image(loop.time_filter_den)
         }
         self._add_to_table(kw.LOOPS_TABLE, loop, row)
 
     def _create_primary_hdu(self) -> fits.PrimaryHDU:
-        cards = {
-            kw.AOT_VERSION: kw.CURRENT_AOT_VERSION,
-            kw.AOT_TIMESYS: kw.AOT_TIMESYS_UTC,
-        }
+        hdr = fits.Header([(f'HIERARCH {md.key}' if len(md.key) > 8 else md.key,
+                            md.value,
+                            md.comment) for md in self._system.metadata])
+        hdr[kw.AOT_VERSION] = kw.CURRENT_AOT_VERSION
+        hdr[kw.AOT_TIMESYS] = kw.AOT_TIMESYS_UTC
 
         if self._system.ao_mode not in kw.AOT_AO_MODE_SET:
             raise ValueError(f"'AOSystem.ao_mode' must be one of: {str(kw.AOT_AO_MODE_SET)[1:-1]}")
-        cards[kw.AOT_AO_MODE] = self._system.ao_mode
+        hdr[kw.AOT_AO_MODE] = self._system.ao_mode
 
-        cards[kw.AOT_DATE_BEG] = datetime_to_iso(self._system.date_beginning)
-        cards[kw.AOT_DATE_END] = datetime_to_iso(self._system.date_end)
+        hdr[kw.AOT_DATE_BEG] = datetime_to_iso(self._system.date_beginning)
+        hdr[kw.AOT_DATE_END] = datetime_to_iso(self._system.date_end)
 
+        if self._system.name is not None:
+            hdr[kw.AOT_SYSTEM_NAME] = self._system.name
         if self._system.strehl_ratio is not None:
-            cards[kw.AOT_STREHL_RATIO] = self._system.strehl_ratio
+            hdr[kw.AOT_STREHL_RATIO] = self._system.strehl_ratio
         if self._system.temporal_error is not None:
-            cards[kw.AOT_TEMPORAL_ERROR] = self._system.temporal_error
+            hdr[kw.AOT_TEMPORAL_ERROR] = self._system.temporal_error
         if self._system.config is not None:
-            cards[kw.AOT_CONFIG] = self._system.config
+            hdr[kw.AOT_CONFIG] = self._system.config
 
-        return fits.PrimaryHDU(header=fits.Header(cards))
+        return fits.PrimaryHDU(header=hdr)
 
     def _create_bintable_hdus(self) -> list[fits.BinTableHDU]:
         hdus = []
         for table_name in kw.TABLE_SEQUENCE:
             try:
                 table = self._tables[table_name]
             except KeyError:
```

### Comparing `aotpy-0.7.0/aotpy/translators/aof.py` & `aotpy-0.8.0/aotpy/translators/galacsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains a class for translating data produced by ESO's AOF system.
+This module contains a class for translating data produced by ESO's GALACSI system.
 """
 
 import importlib.resources
 import warnings
 from datetime import datetime
 from pathlib import Path
 
@@ -14,29 +14,29 @@
 from aotpy.io import image_from_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
-class AOFTranslator(ESOTranslator):
-    """Contains functions for translating telemetry data produced by ESO's AOF system.
+class GALACSITranslator(ESOTranslator):
+    """Contains functions for translating telemetry data produced by ESO's GALACSI system.
 
     Parameters
     ----------
     path_lgs
         Path to folder containing LGS data (LGSAcq, LGSCtr, LGSRecn, JitCtr, JitRecnOptimiser, RTC).
     path_ir
         Path to folder containing IR data (IRAcq, IRCtr, IRLoopMonitor).
     path_pix
         Path to folder containing pixel data.
     """
 
     def __init__(self, path_lgs: str, path_ir: str, path_pix: str):
-        self.system = aotpy.AOSystem(ao_mode='LTAO')
+        self.system = aotpy.AOSystem(ao_mode='LTAO', name='GALACSI')
         self.system.main_telescope = aotpy.MainTelescope(
             uid='ESO VLT UT4',
             enclosing_diameter=8.2,
             inscribed_diameter=8.2
         )
 
         self._handle_lgs_data(path_lgs)
@@ -59,15 +59,15 @@
         lgs_timestamps = lgs_loop_frame['Seconds'] + lgs_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(lgs_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(lgs_timestamps[-1])
         lgs_frame_numbers = lgs_loop_frame['FrameCounter']
         lgs_time = aotpy.Time('LGS Loop Time', timestamps=lgs_timestamps.tolist(),
                               frame_numbers=lgs_frame_numbers.tolist())
 
-        aof_data_path = importlib.resources.files('aotpy.data') / 'AOF'
+        aof_data_path = importlib.resources.files('aotpy.data') / 'GALACSI'
         with importlib.resources.as_file(aof_data_path / 'subap.fits') as p:
             subaperture_mask = image_from_file(p)
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         dsm_positions = aotpy.Image('DSM_positions', lgs_loop_frame['DSM_Positions'][:, self.dsm_valid])
         m2c = image_from_file(path_lgs / 'LGSCtr.ACT_POS_MODAL_PROJECTION.fits')
         lgs_tfz_num = aotpy.Image('LGSCtr.A_TERMS', fits.getdata(path_lgs / 'LGSCtr.A_TERMS.fits').T)
@@ -226,8 +226,11 @@
             time_filter_den=aotpy.Image('IRCtr.B_TERMS', fits.getdata(path_ir / 'IRCtr.B_TERMS.fits').T)
         ))
 
     def _get_eso_telescope_name(self) -> str:
         return 'ESO-VLT-U4'
 
     def _get_eso_ao_name(self) -> str:
-        return 'AOF'
+        return 'GALACSI'
+
+    def _get_run_id(self) -> str:
+        return '60.A-9278(B)'
```

### Comparing `aotpy-0.7.0/aotpy/translators/base.py` & `aotpy-0.8.0/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.7.0/aotpy/translators/ciao.py` & `aotpy-0.8.0/aotpy/translators/ciao.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
         with fits.open(path / 'CIAO_LOOP_0001.fits', extname='LoopFrame') as hdus:
             main_hdr = hdus[0].header
             main_loop_frame = hdus['LoopFrame'].data
 
         self.system = aotpy.AOSystem(
             ao_mode='SCAO',
+            name='CIAO',
             strehl_ratio=main_hdr['ESO AOS ATM SR'],
             temporal_error=main_hdr['ESO AOS ATM TERR']
         )
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
             azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
@@ -154,7 +155,10 @@
         #   ESO-VLTI-Amnop
         #   ESO-VLTI-Uijkl-Amnop
         # as long as mnop contains the correct number
         return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'CIAO'
+
+    def _get_run_id(self) -> str:
+        return '60.A-9278(C)'
```

### Comparing `aotpy-0.7.0/aotpy/translators/eris.py` & `aotpy-0.8.0/aotpy/translators/eris.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains a class for translating data produced by ESO's AOF system.
+This module contains a class for translating data produced by ESO's ERIS system.
 """
 
 import importlib.resources
 import warnings
 from datetime import datetime
 from pathlib import Path
 
@@ -25,15 +25,15 @@
     ----------
     path
         Path to folder containing all system data.
     """
 
     def __init__(self, path):
         self._path = Path(path)
-        self.system = aotpy.AOSystem()
+        self.system = aotpy.AOSystem(name='ERIS AO')
         self.system.main_telescope = aotpy.MainTelescope(
             uid='ESO VLT UT4',
             enclosing_diameter=8.2,
             inscribed_diameter=8.2
         )
         self.dsm = aotpy.DeformableMirror(
             uid='DSM',
@@ -358,8 +358,11 @@
             modes_to_measurements=aotpy.Image('CLMatrixOptimiser.M2S', m2s),
         ))
 
     def _get_eso_telescope_name(self) -> str:
         return 'ESO-VLT-U4'
 
     def _get_eso_ao_name(self) -> str:
-        return 'ERIS'
+        return 'ERIAO'
+
+    def _get_run_id(self) -> str:
+        return '60.A-9278(E)'
```

### Comparing `aotpy-0.7.0/aotpy/translators/eso.py` & `aotpy-0.8.0/aotpy/translators/eso.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from astropy.time import Time
 
 try:
     from pyvo.dal import tap
 except (ImportError, ModuleNotFoundError):
     tap = None
 
-from aotpy.io.fits import FITSWriter
+from ..core.base import Metadatum
 from .base import BaseTranslator
 
 ESO_TAP_OBS = "https://archive.eso.org/tap_obs"
 
 
 class ESOTranslator(BaseTranslator):
     """Abstract class for translators for ESO systems.
@@ -80,37 +80,39 @@
         =====================   =============================================================================
         """
         pass
 
     @abstractmethod
     def _get_eso_ao_name(self) -> str:
         """
-        Get abbreviation of the adaptive optics system's name (e.g. 'AOF', 'NAOMI', 'CIAO', ...).
+        Get abbreviation of the adaptive optics system's name, as defined by ESO.
         """
         pass
 
-    def to_archive_ready_file(self, filename: str, query_archive: bool = True, **kwargs) -> None:
+    @abstractmethod
+    def _get_run_id(self) -> str:
+        """
+        Get the run ID (prog ID) that refers to the data, as defined by ESO.
         """
-        Writes translated system into an AOT FITS file with the necessary metadata for ESO Archive.
+        pass
 
-        Requires pyvo.
+    def add_archive_metadata(self, query_archive: bool = False) -> None:
+        """
+        Adds necessary metadata for ESO Archive to AOSystem.
 
         Parameters
         ----------
-        filename
-            Path to the file that will be written.
-        query_archive : default = True
-            Whether the ESO archive should be queried to find relevant metadata already in the archive.
-        **kwargs
-            Keyword arguments passed on as options to the file handling function.
-
+        query_archive : default = False
+            Whether the ESO archive should be queried to find relevant metadata already in the archive. Requires pyvo.
         """
         telescope = self._get_eso_telescope_name()
         metadata = {
             'ORIGIN': 'ESO-PARANAL',
+            'INSTRUME': self._get_eso_ao_name(),
+            'HIERARCH ESO OBS PROG ID': self._get_run_id(),
             'TELESCOP': telescope.replace('%', ''),
             'DATE': datetime.now().isoformat(timespec='milliseconds'),
             'OBJECT': 'AO-TELEM',
             'OBSERVER': 'I, Condor',
             'DATE-OBS': self.system.date_beginning.astimezone(timezone.utc).replace(tzinfo=None).isoformat(
                 timespec='milliseconds'),
             'MJD-OBS': Time(self.system.date_beginning, scale='utc').mjd,
@@ -160,19 +162,15 @@
                 if 'HIERARCH ESO TEL AZ' not in metadata:
                     metadata['HIERARCH ESO TEL AZ'] = res['tel_az']
                 if 'HIERARCH ESO TEL ALT' not in metadata:
                     metadata['HIERARCH ESO TEL ALT'] = res['tel_alt']
             else:
                 warnings.warn(f"Could not find data from telescope '{telescope}' near mjd_obs {beg.mjd} at the "
                               f"ESO Archive")
-
-        hdul = FITSWriter(self.system).get_hdus()
-        hdr: fits.Header = hdul[0].header
-        hdr.extend(metadata)
-        hdul.writeto(filename, **kwargs)
+        self.system.metadata.extend([Metadatum(k, v) for k, v in metadata.items()])
 
     def get_atmospheric_parameters_from_archive(self) -> astropy.table.Table:
         """
         Get atmospheric data from ESO's Science Archive within the recording period.
 
         Requires pyvo.
         """
```

### Comparing `aotpy-0.7.0/aotpy/translators/naomi.py` & `aotpy-0.8.0/aotpy/translators/naomi.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         path = Path(path)
         self._at_number = at_number
 
         with fits.open(path / 'NAOMI_LOOP_0001.fits', extname='LoopFrame') as hdus:
             main_hdr = hdus[0].header
             main_loop_frame: fits.FITS_rec = hdus['LoopFrame'].data
 
-        self.system = aotpy.AOSystem(ao_mode='SCAO')
+        self.system = aotpy.AOSystem(ao_mode='SCAO', name='NAOMI')
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
             azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
             parallactic=main_hdr['ESO TEL PRLTIC'],
             enclosing_diameter=1.82,
             inscribed_diameter=1.82
@@ -154,7 +154,10 @@
         #   ESO-VLTI-Amnop
         #   ESO-VLTI-Uijkl-Amnop
         # as long as mnop contains the correct number
         return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'NAOMI'
+
+    def _get_run_id(self) -> str:
+        return '60.A-9278(D)'
```

### Comparing `aotpy-0.7.0/aotpy/translators/papyrus.py` & `aotpy-0.8.0/aotpy/translators/papyrus.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class PAPYRUSTranslator(BaseTranslator):
     def __init__(self, file) -> None:
         if loadmat is None:
             raise ImportError("Translating PAPYRUS data requires the scipy module.")
         data = loadmat(file, simplify_cells=True)['data']
 
-        self.system = aotpy.AOSystem(ao_mode='SCAO')
+        self.system = aotpy.AOSystem(ao_mode='SCAO', name='PAPYRUS')
 
         self.system.sources = [aotpy.NaturalGuideStar(uid=data['source'])]
 
         papyrus_data_path = importlib.resources.files('aotpy.data') / 'PAPYRUS'
         with importlib.resources.as_file(papyrus_data_path / 'T152_pupil.fits') as p:
             pupil_mask = image_from_file(p, name='T152 PUPIL')
```

### Comparing `aotpy-0.7.0/aotpy.egg-info/PKG-INFO` & `aotpy-0.8.0/aotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.7.0/aotpy.egg-info/SOURCES.txt` & `aotpy-0.8.0/aotpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 aotpy/core/loop.py
 aotpy/core/optical_sensor.py
 aotpy/core/source.py
 aotpy/core/telescope.py
 aotpy/core/time.py
 aotpy/core/wavefront_corrector.py
 aotpy/data/__init__.py
-aotpy/data/AOF/subap.fits
 aotpy/data/ERIS/ho_subap.fits
 aotpy/data/ERIS/lo_subap.fits
+aotpy/data/GALACSI/subap.fits
 aotpy/data/NAOMI/zernike_control_modes.fits
 aotpy/data/PAPYRUS/T152_pupil.fits
 aotpy/io/__init__.py
 aotpy/io/base.py
 aotpy/io/fits/__init__.py
 aotpy/io/fits/_keywords.py
 aotpy/io/fits/reader.py
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
 aotpy/translators/__init__.py
-aotpy/translators/aof.py
 aotpy/translators/base.py
 aotpy/translators/ciao.py
 aotpy/translators/eris.py
 aotpy/translators/eso.py
+aotpy/translators/galacsi.py
 aotpy/translators/naomi.py
 aotpy/translators/papyrus.py
```

### Comparing `aotpy-0.7.0/setup.cfg` & `aotpy-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 372e 300d 0a61 7574 686f  n = 0.7.0..autho
+00000020: 6e20 3d20 302e 382e 300d 0a61 7574 686f  n = 0.8.0..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
```

