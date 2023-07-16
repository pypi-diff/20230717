# Comparing `tmp/solarannotator-0.3.1.tar.gz` & `tmp/solarannotator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarannotator-0.3.1.tar", last modified: Fri Feb  3 15:16:51 2023, max compression
+gzip compressed data, was "solarannotator-1.0.0.tar", last modified: Sun Jul 16 22:34:33 2023, max compression
```

## Comparing `solarannotator-0.3.1.tar` & `solarannotator-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-03 15:16:51.959216 solarannotator-0.3.1/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2180 2023-02-03 15:16:51.958709 solarannotator-0.3.1/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1915 2021-12-22 15:39:28.000000 solarannotator-0.3.1/README.md
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-03 15:16:51.945809 solarannotator-0.3.1/cfg/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      596 2021-12-22 15:39:28.000000 solarannotator-0.3.1/cfg/default.json
--rw-r--r--   0 jhughes  (1624782681) 1567826318       38 2023-02-03 15:16:51.959380 solarannotator-0.3.1/setup.cfg
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1171 2023-02-03 15:14:27.000000 solarannotator-0.3.1/setup.py
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-03 15:16:51.952111 solarannotator-0.3.1/solarannotator/
--rw-r--r--   0 jhughes  (1624782681) 1567826318        0 2021-12-22 15:39:28.000000 solarannotator-0.3.1/solarannotator/__init__.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1233 2021-12-22 15:39:28.000000 solarannotator-0.3.1/solarannotator/config.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318    32270 2023-02-03 15:12:44.000000 solarannotator-0.3.1/solarannotator/gui.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318     6867 2023-02-03 14:58:46.000000 solarannotator-0.3.1/solarannotator/io.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318      796 2021-12-22 15:39:28.000000 solarannotator-0.3.1/solarannotator/main.py
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-02-03 15:16:51.957872 solarannotator-0.3.1/solarannotator.egg-info/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2180 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318      383 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/SOURCES.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/dependency_links.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       61 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/entry_points.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318      109 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/requires.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       15 2023-02-03 15:16:51.000000 solarannotator-0.3.1/solarannotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 22:34:33.427623 solarannotator-1.0.0/
+-rw-rw-rw-   0        0        0     2812 2023-07-16 22:34:33.426626 solarannotator-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-07-16 21:47:49.000000 solarannotator-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 22:34:33.416652 solarannotator-1.0.0/cfg/
+-rw-rw-rw-   0        0        0      628 2023-07-16 21:47:49.000000 solarannotator-1.0.0/cfg/default.json
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:34:33.427623 solarannotator-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-07-16 21:55:55.000000 solarannotator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:34:33.420642 solarannotator-1.0.0/solarannotator/
+-rw-rw-rw-   0        0        0        0 2023-07-16 21:47:49.000000 solarannotator-1.0.0/solarannotator/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-07-16 22:28:29.000000 solarannotator-1.0.0/solarannotator/config.py
+-rw-rw-rw-   0        0        0    33338 2023-07-16 21:58:50.000000 solarannotator-1.0.0/solarannotator/gui.py
+-rw-rw-rw-   0        0        0     9567 2023-07-16 22:28:29.000000 solarannotator-1.0.0/solarannotator/io.py
+-rw-rw-rw-   0        0        0      826 2023-07-16 21:47:49.000000 solarannotator-1.0.0/solarannotator/main.py
+-rw-rw-rw-   0        0        0     2727 2023-07-16 22:28:29.000000 solarannotator-1.0.0/solarannotator/template.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:34:33.425628 solarannotator-1.0.0/solarannotator.egg-info/
+-rw-rw-rw-   0        0        0     2812 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 22:34:33.000000 solarannotator-1.0.0/solarannotator.egg-info/top_level.txt
```

### Comparing `solarannotator-0.3.1/cfg/default.json` & `solarannotator-1.0.0/cfg/default.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 7b0a 2263 6c61 7373 6573 223a 7b0a 2020  {."classes":{.  
-00000010: 2020 226f 7574 6572 5f73 7061 6365 223a    "outer_space":
-00000020: 312c 0a20 2020 2022 6272 6967 6874 5f72  1,.    "bright_r
-00000030: 6567 696f 6e22 3a33 2c0a 2020 2020 2266  egion":3,.    "f
-00000040: 696c 616d 656e 7422 3a34 2c0a 2020 2020  ilament":4,.    
-00000050: 2270 726f 6d69 6e65 6e63 6522 3a35 2c0a  "prominence":5,.
-00000060: 2020 2020 2263 6f72 6f6e 616c 5f68 6f6c      "coronal_hol
-00000070: 6522 3a36 2c0a 2020 2020 2271 7569 6574  e":6,.    "quiet
-00000080: 5f73 756e 223a 372c 0a20 2020 2022 6c69  _sun":7,.    "li
-00000090: 6d62 223a 382c 0a20 2020 2022 666c 6172  mb":8,.    "flar
-000000a0: 6522 3a39 0a20 207d 2c0a 0a20 2022 6469  e":9.  },..  "di
-000000b0: 7370 6c61 7922 3a7b 0a20 2020 2022 636f  splay":{.    "co
-000000c0: 6c6f 7273 223a 7b0a 2020 2020 2020 226f  lors":{.      "o
-000000d0: 7574 6572 5f73 7061 6365 223a 2022 2330  uter_space": "#0
-000000e0: 3030 3030 3022 2c0a 2020 2020 2020 2262  00000",.      "b
-000000f0: 7269 6768 745f 7265 6769 6f6e 223a 2022  right_region": "
-00000100: 2346 3045 3434 3222 2c0a 2020 2020 2020  #F0E442",.      
-00000110: 2266 696c 616d 656e 7422 3a20 2223 4435  "filament": "#D5
-00000120: 3545 3030 222c 0a20 2020 2020 2022 7072  5E00",.      "pr
-00000130: 6f6d 696e 656e 6365 223a 2022 2345 3639  ominence": "#E69
-00000140: 4630 3022 2c0a 2020 2020 2020 2263 6f72  F00",.      "cor
-00000150: 6f6e 616c 5f68 6f6c 6522 3a20 2223 3030  onal_hole": "#00
-00000160: 3945 3733 222c 0a20 2020 2020 2022 7175  9E73",.      "qu
-00000170: 6965 745f 7375 6e22 3a20 2223 3030 3732  iet_sun": "#0072
-00000180: 4232 222c 0a20 2020 2020 2022 6c69 6d62  B2",.      "limb
-00000190: 223a 2022 2335 3642 3445 3922 2c0a 2020  ": "#56B4E9",.  
-000001a0: 2020 2020 2266 6c61 7265 223a 2022 2343      "flare": "#C
-000001b0: 4337 3941 3722 0a20 2020 207d 2c0a 0a20  C79A7".    },.. 
-000001c0: 2020 2022 6368 616e 6e65 6c73 223a 7b0a     "channels":{.
-000001d0: 2020 2020 2020 2272 6564 223a 2022 7375        "red": "su
-000001e0: 7669 2d6c 3162 2d66 6531 3731 222c 0a20  vi-l1b-fe171",. 
-000001f0: 2020 2020 2022 6772 6565 6e22 3a20 2273       "green": "s
-00000200: 7576 692d 6c31 622d 6665 3139 3522 2c0a  uvi-l1b-fe195",.
-00000210: 2020 2020 2020 2262 6c75 6522 3a20 2273        "blue": "s
-00000220: 7576 692d 6c31 622d 6665 3238 3422 2c0a  uvi-l1b-fe284",.
-00000230: 2020 2020 2020 2273 696e 676c 6522 3a22        "single":"
-00000240: 6861 6c70 6861 220a 2020 2020 7d0a 2020  halpha".    }.  
-00000250: 7d0a 7d0a                                }.}.
+00000000: 7b0d 0a22 636c 6173 7365 7322 3a7b 0d0a  {.."classes":{..
+00000010: 2020 2020 226f 7574 6572 5f73 7061 6365      "outer_space
+00000020: 223a 312c 0d0a 2020 2020 2262 7269 6768  ":1,..    "brigh
+00000030: 745f 7265 6769 6f6e 223a 332c 0d0a 2020  t_region":3,..  
+00000040: 2020 2266 696c 616d 656e 7422 3a34 2c0d    "filament":4,.
+00000050: 0a20 2020 2022 7072 6f6d 696e 656e 6365  .    "prominence
+00000060: 223a 352c 0d0a 2020 2020 2263 6f72 6f6e  ":5,..    "coron
+00000070: 616c 5f68 6f6c 6522 3a36 2c0d 0a20 2020  al_hole":6,..   
+00000080: 2022 7175 6965 745f 7375 6e22 3a37 2c0d   "quiet_sun":7,.
+00000090: 0a20 2020 2022 6c69 6d62 223a 382c 0d0a  .    "limb":8,..
+000000a0: 2020 2020 2266 6c61 7265 223a 390d 0a20      "flare":9.. 
+000000b0: 207d 2c0d 0a0d 0a20 2022 6469 7370 6c61   },....  "displa
+000000c0: 7922 3a7b 0d0a 2020 2020 2263 6f6c 6f72  y":{..    "color
+000000d0: 7322 3a7b 0d0a 2020 2020 2020 226f 7574  s":{..      "out
+000000e0: 6572 5f73 7061 6365 223a 2022 2330 3030  er_space": "#000
+000000f0: 3030 3022 2c0d 0a20 2020 2020 2022 6272  000",..      "br
+00000100: 6967 6874 5f72 6567 696f 6e22 3a20 2223  ight_region": "#
+00000110: 4630 4534 3432 222c 0d0a 2020 2020 2020  F0E442",..      
+00000120: 2266 696c 616d 656e 7422 3a20 2223 4435  "filament": "#D5
+00000130: 3545 3030 222c 0d0a 2020 2020 2020 2270  5E00",..      "p
+00000140: 726f 6d69 6e65 6e63 6522 3a20 2223 4536  rominence": "#E6
+00000150: 3946 3030 222c 0d0a 2020 2020 2020 2263  9F00",..      "c
+00000160: 6f72 6f6e 616c 5f68 6f6c 6522 3a20 2223  oronal_hole": "#
+00000170: 3030 3945 3733 222c 0d0a 2020 2020 2020  009E73",..      
+00000180: 2271 7569 6574 5f73 756e 223a 2022 2330  "quiet_sun": "#0
+00000190: 3037 3242 3222 2c0d 0a20 2020 2020 2022  072B2",..      "
+000001a0: 6c69 6d62 223a 2022 2335 3642 3445 3922  limb": "#56B4E9"
+000001b0: 2c0d 0a20 2020 2020 2022 666c 6172 6522  ,..      "flare"
+000001c0: 3a20 2223 4343 3739 4137 220d 0a20 2020  : "#CC79A7"..   
+000001d0: 207d 2c0d 0a0d 0a20 2020 2022 6368 616e   },....    "chan
+000001e0: 6e65 6c73 223a 7b0d 0a20 2020 2020 2022  nels":{..      "
+000001f0: 7265 6422 3a20 2273 7576 692d 6c31 622d  red": "suvi-l1b-
+00000200: 6665 3137 3122 2c0d 0a20 2020 2020 2022  fe171",..      "
+00000210: 6772 6565 6e22 3a20 2273 7576 692d 6c31  green": "suvi-l1
+00000220: 622d 6665 3139 3522 2c0d 0a20 2020 2020  b-fe195",..     
+00000230: 2022 626c 7565 223a 2022 7375 7669 2d6c   "blue": "suvi-l
+00000240: 3162 2d66 6532 3834 222c 0d0a 2020 2020  1b-fe284",..    
+00000250: 2020 2273 696e 676c 6522 3a22 6861 6c70    "single":"halp
+00000260: 6861 220d 0a20 2020 207d 0d0a 2020 7d0d  ha"..    }..  }.
+00000270: 0a7d 0d0a                                .}..
```

### Comparing `solarannotator-0.3.1/setup.py` & `solarannotator-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup
-
-# read the contents of your README file
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-
-setup(
-    name='solarannotator',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    version='0.3.1',
-    packages=['solarannotator'],
-    url='',
-    license='',
-    author='J. Marcus Hughes',
-    author_email='j-marcus.hughes@noaa.gov',
-    description='A tool to annotate images of the Sun',
-    install_requires=["PyQt5",
-                      "matplotlib",
-                      "astropy",
-                      "numpy",
-                      "goes-solar-retriever",
-                      "scipy",
-                      "scikit-image",
-                      "pillow",
-                      "sunpy",
-                      "lxml",
-                      "reproject",
-                      "zeep",
-                      "drms"],
-    data_files=[('solarannotator', ['cfg/default.json'])],
-    entry_points={"console_scripts": ["SolarAnnotator = solarannotator.main:main"]}
-
-)
+from setuptools import setup
+
+# read the contents of your README file
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+
+setup(
+    name='solarannotator',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    version='1.0.0',
+    packages=['solarannotator'],
+    url='',
+    license='',
+    author='J. Marcus Hughes',
+    author_email='j-marcus.hughes@noaa.gov',
+    description='A tool to annotate images of the Sun',
+    install_requires=["PyQt5",
+                      "matplotlib",
+                      "astropy",
+                      "numpy",
+                      "goes-solar-retriever",
+                      "scipy",
+                      "scikit-image",
+                      "pillow",
+                      "sunpy",
+                      "lxml",
+                      "reproject",
+                      "zeep",
+                      "drms"],
+    data_files=[('solarannotator', ['cfg/default.json'])],
+    entry_points={"console_scripts": ["SolarAnnotator = solarannotator.main:main"]}
+
+)
```

### Comparing `solarannotator-0.3.1/solarannotator/config.py` & `solarannotator-1.0.0/solarannotator/config.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import json
-import matplotlib
-
-
-class Config:
-    def __init__(self, config_file_path):
-        """
-        Handles configuring the annotation tool
-        :param config_file_path: string path to configuration file
-        """
-        with open(config_file_path) as f:
-            config = json.load(f)
-
-        if not self.is_valid():
-            raise RuntimeError("The configuration file provided is invalid")
-
-        self.solar_classes = [(c, int(n)) for c, n in config['classes'].items()]
-        self.solar_class_index = {c: n for c, n in self.solar_classes}
-        self.solar_class_name = {n: c for c, n in config['classes'].items()}
-        self.solar_colors = config['display']['colors']
-        self.color_table = [self.solar_colors[self.solar_class_name[i]] if i in self.solar_class_name else '#FFFFFF'
-                            for i in range(max(list(self.solar_class_name.keys()))+1)]
-        self.solar_cmap = matplotlib.colors.ListedColormap(self.color_table)
-        self.max_index = max(list(self.solar_class_name.keys()))
-
-    def is_valid(self):
-        """
-        Check that the configuration file is valid
-        :return: boolean indicating validity
-        """
-        # TODO : write
-        return True
+import json
+import matplotlib
+
+
+class Config:
+    def __init__(self, config_file_path):
+        """
+        Handles configuring the annotation tool
+        :param config_file_path: string path to configuration file
+        """
+        with open(config_file_path) as f:
+            config = json.load(f)
+
+        if not self.is_valid():
+            raise RuntimeError("The configuration file provided is invalid")
+
+        self.solar_classes = [(c, int(n)) for c, n in config['classes'].items()]
+        self.solar_class_index = {c: n for c, n in self.solar_classes}
+        self.solar_class_name = {n: c for c, n in config['classes'].items()}
+        self.solar_colors = config['display']['colors']
+        self.color_table = [self.solar_colors[self.solar_class_name[i]] if i in self.solar_class_name else '#FFFFFF'
+                            for i in range(max(list(self.solar_class_name.keys()))+1)]
+        self.solar_cmap = matplotlib.colors.ListedColormap(self.color_table)
+        self.max_index = max(list(self.solar_class_name.keys()))
+
+    def is_valid(self):
+        """
+        Check that the configuration file is valid
+        :return: boolean indicating validity
+        """
+        # TODO : write
+        return True
```

### Comparing `solarannotator-0.3.1/solarannotator/gui.py` & `solarannotator-1.0.0/solarannotator/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,698 +1,705 @@
-import sys
-import PyQt5
-from PyQt5 import QtCore, QtWidgets
-from PyQt5.QtWidgets import QWidget, QLabel, QAction, QTabWidget, QPushButton, QFileDialog, QRadioButton, QMessageBox, \
-    QComboBox, QLineEdit, QSizePolicy
-from PyQt5.QtCore import QDateTime
-from PyQt5.QtGui import QIcon, QDoubleValidator
-from datetime import datetime, timedelta
-from matplotlib import path
-from matplotlib.collections import PatchCollection
-from matplotlib.patches import Polygon
-from skimage.morphology import binary_erosion
-import scipy
-import numpy as np
-from matplotlib.widgets import LassoSelector
-from matplotlib.backends.qt_compat import QtCore, QtWidgets
-from PIL import ImageColor
-from matplotlib.backends.backend_qt5agg import FigureCanvas, NavigationToolbar2QT as NavigationToolbar
-from matplotlib.figure import Figure
-
-if hasattr(QtCore.Qt, 'AA_EnableHighDpiScaling'):
-    PyQt5.QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)
-
-if hasattr(QtCore.Qt, 'AA_UseHighDpiPixmaps'):
-    PyQt5.QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps, True)
-
-from .config import Config
-from .io import ThematicMap, ImageSet
-
-
-class AnnotationWidget(QtWidgets.QWidget):
-    def __init__(self, config):
-        super().__init__()
-        self.composites = ImageSet.create_empty()
-        self.current_theme_index = 0
-
-        self.preview_data = self.composites['94'].data.copy()
-        self.thmap_data = np.zeros((1280, 1280))
-        self.thmap = ThematicMap(self.thmap_data, {'DATE-OBS': str(datetime.today())}, config.solar_class_name)
-
-        self.history = []
-
-        layout = QtWidgets.QVBoxLayout()
-
-        self.fig = Figure(figsize=(15, 10))
-        canvas = FigureCanvas(self.fig)
-        canvas.mpl_connect('button_press_event', self.onclick)
-
-        layout.addWidget(canvas)
-
-        self.region_patches = []
-        self.axs = canvas.figure.subplots(ncols=2, sharex=True, sharey=True)
-        self.preview_axesimage = self.axs[0].imshow(self.preview_data, vmin=0, vmax=1, cmap='gray', origin='lower')
-        self.thmap_axesimage = self.axs[1].imshow(self.thmap_data, origin='lower', interpolation='none',
-                                                  vmin=0, vmax=config.max_index, cmap=config.solar_cmap)
-        self.axs[0].set_axis_off()
-        self.axs[1].set_axis_off()
-        self.axs[0].set_title("Preview")
-        self.axs[1].set_title("Thematic Map")
-
-        self.toolbar = NavigationToolbar(canvas, self)
-        layout.addWidget(self.toolbar)
-        self.setLayout(layout)
-
-        # add selection layer for lasso
-        self.shape = (1280, 1280)  # TODO: replace with dynamic detection
-        self.pix = np.arange(self.shape[0])  # assumes square image
-        xv, yv = np.meshgrid(self.pix, self.pix)
-        self.pix = np.vstack((xv.flatten(), yv.flatten())).T
-
-        lineprops = dict(color="red", linewidth=2)
-        self.lasso = LassoSelector(self.axs[0], self.onlasso, lineprops=lineprops)
-        self.fig.tight_layout()
-
-    def onlasso(self, verts):
-        """
-        Main function to control the action of the lasso, allows user to draw on data image and adjust thematic map
-        :param verts: the vertices selected by the lasso
-        :return: nothin, but update the selection array so lassoed region now has the selected theme, redraws canvas
-        """
-        p = path.Path(verts)
-        ind = p.contains_points(self.pix, radius=1)
-        self.history.append(self.thmap_data.copy())
-        self.thmap_data = self.updateArray(self.thmap_data,
-                                                ind,
-                                                self.current_theme_index)
-        self.thmap_axesimage.set_data(self.thmap_data)
-        self.fig.canvas.draw_idle()
-        self.thmap.data = self.thmap_data
-
-    def rename_region(self, event):
-        # draw patches
-        y, x = int(event.xdata), int(event.ydata)
-        self.history.append(self.thmap_data.copy())
-        label = self.thmap_data[x, y]
-        contiguous_regions = scipy.ndimage.label(self.thmap_data == label)[0]
-        this_region = contiguous_regions == (contiguous_regions[x, y])
-        self.thmap_data[this_region] = self.current_theme_index
-        self.thmap_axesimage.set_data(self.thmap_data)
-        self.thmap.data = self.thmap_data
-        self.fig.canvas.draw_idle()
-
-    def draw_event_region_boundary(self, event):
-        """
-        Draw a patch around the contiguous region in the preview image
-        :param event:
-        :return:
-        """
-        # draw patches
-        y, x = int(event.xdata), int(event.ydata)
-        label = self.thmap_data[x, y]
-        contiguous_regions = scipy.ndimage.label(self.thmap_data == label)[0]
-        this_region = contiguous_regions == (contiguous_regions[x, y])
-
-        # remove the boundaries so any region touching the edge isn't drawn odd
-        this_region[0, :] = 0
-        this_region[:, 0] = 0
-        this_region[this_region.shape[0] - 1, :] = 0
-        this_region[:, this_region.shape[1] - 1] = 0
-
-        # convert the region mask into just a true/false array of its boundary pixels
-        edges = binary_erosion(this_region) ^ this_region
-
-        # convert the boundary pixels into a path, moving around instead of just where
-        x, y = np.where(edges)
-        coords = np.dstack([x, y])[0]
-        path = [coords[0]]
-        coords = coords[1:]
-
-        while len(coords):
-            dist = np.sum(np.abs(path[-1] - coords), axis=1)
-            neighbor_index = np.argmin(dist)
-
-            if dist[neighbor_index] < 5:
-                path.append(coords[neighbor_index].copy())
-                coords[neighbor_index:-1] = coords[neighbor_index + 1:]
-                coords = coords[:-1]
-            else:
-                break
-
-        path = np.array(path)
-
-        clips = []
-        while len(coords) > 5:
-            dist = np.sum(np.abs(path[-1] - coords), axis=1)
-            neighbor_index = np.argmin(dist)
-            clip = [coords[neighbor_index].copy()]
-            coords[neighbor_index:-1] = coords[neighbor_index + 1:]
-            coords = coords[:-1]
-            while len(coords):
-                dist = np.sum(np.abs(clip[-1] - coords), axis=1)
-                neighbor_index = np.argmin(dist)
-                if dist[neighbor_index] < 5:
-                    clip.append(coords[neighbor_index].copy())
-                    coords[neighbor_index:-1] = coords[neighbor_index + 1:]
-                    coords = coords[:-1]
-                else:
-                    break
-            clips.append(np.array(clip))
-
-        # draw the continguous  on the selection area
-        self.region_patches.append(PatchCollection(
-            [Polygon(np.dstack([path[:, 1], path[:, 0]])[0], False,
-                     fill=False, facecolor=None,
-                     edgecolor="black", alpha=1, lw=2.5)] +
-            [Polygon(np.dstack([clip[:, 1], clip[:, 0]])[0], False,
-                     fill=False, facecolor=None,
-                     edgecolor="black", alpha=1, lw=2.0) for clip in clips],
-            match_original=True))
-        self.axs[0].add_collection(self.region_patches[-1])
-        self.fig.canvas.draw_idle()
-
-    def undo_action(self):
-        """ when undo is clicked, revert the thematic map to the previous state"""
-        if len(self.history) > 1:
-            old = self.history.pop(-1)
-            self.thmap_data = old
-            self.thmap.data = self.thmap_data
-            self.thmap_axesimage.set_data(old)
-            self.fig.canvas.draw_idle()
-
-    def onclick(self, event):
-        """
-        Draw contours on the data for a click in the thematic map
-        :param event: mouse click on thematic map preview
-        """
-        if event.inaxes == self.axs[1]:
-            if event.button == 3:  # right click feature
-                self.draw_event_region_boundary(event)
-            if event.button == 1 and self.toolbar.mode == "":
-                self.rename_region(event)
-
-    def updateArray(self, array, indices, value):
-        """
-        updates array so that pixels at indices take on value
-        :param array: (m,n) array to adjust
-        :param indices: flattened image indices to change value
-        :param value: new value to assign
-        :return: the changed (m,n) array
-        """
-        lin = np.arange(array.size)
-        new_array = array.flatten()
-        new_array[lin[indices]] = value
-        return new_array.reshape(array.shape)
-
-    def clearBoundaries(self):
-        for patch in self.region_patches:
-            patch.remove()
-        self.region_patches = []
-        self.fig.canvas.draw_idle()
-
-    def loadThematicMap(self, thmap):
-        try:
-            download_message = QMessageBox.information(self,
-                                                       'Downloading',
-                                                       "Downloads may take a few moments. Click 'ok' to proceed.",
-                                                       QMessageBox.Ok)
-            self.composites = ImageSet.retrieve(thmap.date_obs)
-        except RuntimeError:
-            self.data_does_not_exist_popup()
-        else:
-            self.thmap = thmap
-            self.thmap.copy_195_metadata(self.composites)
-            self.history = [thmap.data.copy()]
-            self.thmap_data = thmap.data
-            self.thmap_axesimage.set_data(self.thmap_data)
-            self.preview_axesimage.set_data(self.composites['94'].data)
-            self.fig.canvas.draw_idle()
-
-    def updateSingleColorImage(self, channel, lower_percentile, upper_percentile, scale):
-        self.preview_data = self.composites[channel].data.copy()
-        self.preview_data = np.power(np.abs(self.preview_data), scale) * np.sign(self.preview_data)
-        lower = np.nanpercentile(self.preview_data, lower_percentile)
-        upper = np.nanpercentile(self.preview_data, upper_percentile)
-        self.preview_data[self.preview_data < lower] = lower
-        self.preview_data[self.preview_data > upper] = upper
-        self.preview_data = (self.preview_data - np.nanmin(self.preview_data)) \
-                            / (np.nanmax(self.preview_data) - np.nanmin(self.preview_data))
-        # self.preview_data /= np.nanmax(self.preview_data)
-        self.preview_axesimage.set_data(self.preview_data)
-        self.fig.canvas.draw_idle()
-
-    def updateThreeColorImage(self, red_channel, green_channel, blue_channel,
-                              red_min, green_min, blue_min,
-                              red_max, green_max, blue_max,
-                              red_scale, green_scale, blue_scale):
-        self.preview_data = np.stack([self.composites[red_channel].data.copy(),
-                                     self.composites[green_channel].data.copy(),
-                                     self.composites[blue_channel].data.copy()], axis=2)
-        self.preview_data[:, :, 0] = np.power(self.preview_data[:, :, 0], red_scale)
-        self.preview_data[:, :, 1] = np.power(self.preview_data[:, :, 1], green_scale)
-        self.preview_data[:, :, 2] = np.power(self.preview_data[:, :, 2], blue_scale)
-
-        red_lower = np.nanpercentile(self.preview_data[:, :, 0], red_min)
-        green_lower = np.nanpercentile(self.preview_data[:, :, 1], green_min)
-        blue_lower = np.nanpercentile(self.preview_data[:, :, 2], blue_min)
-
-        red_upper = np.nanpercentile(self.preview_data[:, :, 0], red_max)
-        green_upper = np.nanpercentile(self.preview_data[:, :, 1], green_max)
-        blue_upper = np.nanpercentile(self.preview_data[:, :, ], blue_max)
-
-        self.preview_data[self.preview_data[:, :, 0] < red_lower] = red_lower
-        self.preview_data[self.preview_data[:, :, 0] > red_upper] = red_upper
-        self.preview_data[self.preview_data[:, :, 1] < green_lower] = green_lower
-        self.preview_data[self.preview_data[:, :, 1] > green_upper] = green_upper
-        self.preview_data[self.preview_data[:, :, 2] < blue_lower] = blue_lower
-        self.preview_data[self.preview_data[:, :, 2] > blue_upper] = blue_upper
-        
-        for index in [0, 1, 2]:
-            # self.preview_data[:, :, index] /= np.nanmax(self.preview_data[:, :, index])
-            self.preview_data[:, :, index] = (self.preview_data[:, :, index] - np.nanmin(self.preview_data[:, :, index])) \
-                                / (np.nanmax(self.preview_data[:, :, index]) - np.nanmin(self.preview_data[:, :, index]))
-        self.preview_axesimage.set_data(self.preview_data)
-        self.fig.canvas.draw_idle()
-
-    def data_does_not_exist_popup(self):
-        QMessageBox.critical(self,
-                             'Error: Could not open',
-                             'Composite data does not exist for that date.',
-                             QMessageBox.Close)
-
-
-class ControlWidget(QtWidgets.QWidget):
-    def __init__(self, annotator):
-        super().__init__()
-        self.annotator = annotator
-
-        layout = QtWidgets.QHBoxLayout()
-        self.tabs = QTabWidget()
-        self.one_color_tab = QWidget()
-        self.three_color_tab = QWidget()
-
-        # Add tabs
-        self.tabs.addTab(self.one_color_tab, "Single")
-        self.tabs.addTab(self.three_color_tab, "Three-color")
-        self.tabs.currentChanged.connect(self.onTabChange)
-
-        self.initSingleColorUI()
-        self.initThreeColorUI()
-
-        layout.addWidget(self.tabs)
-        self.setLayout(layout)
-
-    def initSingleColorUI(self):
-        # Create single color tab
-        self.one_color_tab.layout = QtWidgets.QGridLayout(self)
-
-        self.single_color_label = QLabel()
-        self.single_color_label.setText("Channel")
-        self.one_color_tab.layout.addWidget(self.single_color_label)
-        self.single_color_combo_box = QComboBox()
-        self.single_color_combo_box.addItems(self.annotator.composites.channels())
-        self.single_color_combo_box.currentTextChanged.connect(self.onSingleColorChange)
-
-        self.one_color_min_editor = QLineEdit()
-        self.one_color_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.one_color_min_editor.setText("3.0")
-        self.one_color_min_editor.editingFinished.connect(self.onSingleColorChange)
-
-        self.one_color_max_editor = QLineEdit()
-        self.one_color_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.one_color_max_editor.setText("99.9")
-        self.one_color_max_editor.editingFinished.connect(self.onSingleColorChange)
-
-        self.one_color_scale_editor = QLineEdit()
-        self.one_color_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.one_color_scale_editor.setText("0.25")
-        self.one_color_scale_editor.editingFinished.connect(self.onSingleColorChange)
-
-        channel_label = QLabel("Channel", self)
-        channel_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        min_label = QLabel("Min", self)
-        min_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        max_label = QLabel("Max", self)
-        max_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        scale_label = QLabel("Scale", self)
-        scale_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-
-        self.one_color_tab.setLayout(self.one_color_tab.layout)
-        self.one_color_tab.layout.addWidget(channel_label, 0, 1)
-        self.one_color_tab.layout.addWidget(min_label, 0, 2)
-        self.one_color_tab.layout.addWidget(max_label, 0, 3)
-        self.one_color_tab.layout.addWidget(scale_label, 0, 4)
-        self.one_color_tab.layout.addWidget(self.single_color_label, 1, 0)
-        self.one_color_tab.layout.addWidget(self.single_color_combo_box, 1, 1)
-        self.one_color_tab.layout.addWidget(self.one_color_min_editor, 1, 2)
-        self.one_color_tab.layout.addWidget(self.one_color_max_editor, 1, 3)
-        self.one_color_tab.layout.addWidget(self.one_color_scale_editor, 1, 4)
-
-
-    def initThreeColorUI(self):
-        self.three_color_tab.layout = QtWidgets.QGridLayout(self)
-
-        channel_label = QLabel("Channel")
-        channel_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        min_label = QLabel("Min")
-        min_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        max_label = QLabel("Max")
-        max_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-        scale_label = QLabel("Scale")
-        scale_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
-
-        self.red_label = QLabel()
-        self.red_label.setText("Red Channel")
-        self.red_label.setAlignment(QtCore.Qt.AlignRight)
-        self.red_combo_box = QComboBox()
-        self.red_combo_box.addItems(self.annotator.composites.channels())
-        self.red_combo_box.setCurrentIndex(2)
-        self.red_combo_box.currentTextChanged.connect(self.onThreeColorChange)
-        self.red_min_editor = QLineEdit()
-        self.red_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.red_min_editor.setText("3.0")
-        self.red_min_editor.editingFinished.connect(self.onThreeColorChange)
-        self.red_max_editor = QLineEdit()
-        self.red_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.red_max_editor.setText("99.9")
-        self.red_max_editor.editingFinished.connect(self.onThreeColorChange)
-        self.red_scale_editor = QLineEdit()
-        self.red_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.red_scale_editor.setText("0.25")
-        self.red_scale_editor.editingFinished.connect(self.onThreeColorChange)
-
-        self.green_label = QLabel()
-        self.green_label.setText("Green Channel")
-        self.green_label.setAlignment(QtCore.Qt.AlignRight)
-        self.green_combo_box = QComboBox()
-        self.green_combo_box.addItems(self.annotator.composites.channels())
-        self.green_combo_box.setCurrentIndex(3)
-        self.green_combo_box.currentTextChanged.connect(self.onThreeColorChange)
-        self.green_min_editor = QLineEdit()
-        self.green_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.green_min_editor.setText("3.0")
-        self.green_min_editor.editingFinished.connect(self.onThreeColorChange)
-        self.green_max_editor = QLineEdit()
-        self.green_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.green_max_editor.setText("99.9")
-        self.green_max_editor.editingFinished.connect(self.onThreeColorChange)
-        self.green_scale_editor = QLineEdit()
-        self.green_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.green_scale_editor.setText("0.25")
-        self.green_scale_editor.editingFinished.connect(self.onThreeColorChange)
-
-        self.blue_label = QLabel()
-        self.blue_label.setText("Blue Channel")
-        self.blue_label.setAlignment(QtCore.Qt.AlignRight)
-        self.blue_combo_box = QComboBox()
-        self.blue_combo_box.addItems(self.annotator.composites.channels())
-        self.blue_combo_box.setCurrentIndex(4)
-        self.blue_combo_box.currentTextChanged.connect(self.onThreeColorChange)
-        self.blue_min_editor = QLineEdit()
-        self.blue_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.blue_min_editor.setText("3.0")
-        self.blue_min_editor.editingFinished.connect(self.onThreeColorChange)
-        self.blue_max_editor = QLineEdit()
-        self.blue_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.blue_max_editor.setText("99.9")
-        self.blue_max_editor.editingFinished.connect(self.onThreeColorChange)
-        self.blue_scale_editor = QLineEdit()
-        self.blue_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
-        self.blue_scale_editor.setText("0.25")
-        self.blue_scale_editor.editingFinished.connect(self.onThreeColorChange)
-
-        self.three_color_tab.setLayout(self.three_color_tab.layout)
-        self.three_color_tab.layout.addWidget(self.red_label, 1, 0)
-        self.three_color_tab.layout.addWidget(self.green_label, 2, 0)
-        self.three_color_tab.layout.addWidget(self.blue_label, 3, 0)
-        self.three_color_tab.layout.addWidget(channel_label, 0, 1)
-        self.three_color_tab.layout.addWidget(self.red_combo_box, 1, 1)
-        self.three_color_tab.layout.addWidget(self.green_combo_box, 2, 1)
-        self.three_color_tab.layout.addWidget(self.blue_combo_box, 3, 1)
-        self.three_color_tab.layout.addWidget(min_label, 0, 2)
-        self.three_color_tab.layout.addWidget(self.red_min_editor, 1, 2)
-        self.three_color_tab.layout.addWidget(self.green_min_editor, 2, 2)
-        self.three_color_tab.layout.addWidget(self.blue_min_editor, 3, 2)
-        self.three_color_tab.layout.addWidget(max_label, 0, 3)
-        self.three_color_tab.layout.addWidget(self.red_max_editor, 1, 3)
-        self.three_color_tab.layout.addWidget(self.green_max_editor, 2, 3)
-        self.three_color_tab.layout.addWidget(self.blue_max_editor, 3, 3)
-        self.three_color_tab.layout.addWidget(scale_label, 0, 4)
-        self.three_color_tab.layout.addWidget(self.red_scale_editor, 1, 4)
-        self.three_color_tab.layout.addWidget(self.green_scale_editor, 2, 4)
-        self.three_color_tab.layout.addWidget(self.blue_scale_editor, 3, 4)
-
-    def onTabChange(self):
-        if self.tabs.currentIndex() == 0:
-            self.onSingleColorChange()
-        elif self.tabs.currentIndex() == 1:
-            self.onThreeColorChange()
-
-    def onSingleColorChange(self):
-        self.annotator.updateSingleColorImage(self.single_color_combo_box.currentText(),
-                                              float(self.one_color_min_editor.text()),
-                                              float(self.one_color_max_editor.text()),
-                                              float(self.one_color_scale_editor.text()))
-
-    def onThreeColorChange(self):
-        red_channel = self.red_combo_box.currentText()
-        green_channel = self.green_combo_box.currentText()
-        blue_channel = self.blue_combo_box.currentText()
-        self.annotator.updateThreeColorImage(red_channel, green_channel, blue_channel,
-                                             float(self.red_min_editor.text()),
-                                             float(self.green_min_editor.text()),
-                                             float(self.blue_min_editor.text()),
-                                             float(self.red_max_editor.text()),
-                                             float(self.green_max_editor.text()),
-                                             float(self.blue_max_editor.text()),
-                                             float(self.red_scale_editor.text()),
-                                             float(self.green_scale_editor.text()),
-                                             float(self.blue_scale_editor.text()))
-
-
-class NewFilePopup(QWidget):
-    def __init__(self, parent):
-        super().__init__()
-        self.parent = parent
-        self.initUI()
-
-    def initUI(self):
-        layout = QtWidgets.QHBoxLayout()
-        instructions = QLabel("Please select a time for the new file.", self)
-        self.dateEdit = QtWidgets.QDateTimeEdit(QDateTime.currentDateTime())
-        submit_button = QPushButton("Submit")
-        layout.addWidget(instructions)
-        layout.addWidget(self.dateEdit)
-        layout.addWidget(submit_button)
-        self.setLayout(layout)
-        submit_button.clicked.connect(self.onSubmit)
-
-    def onSubmit(self):
-        # set the date in the application and close
-        self.parent.date = self.dateEdit.dateTime().toPyDateTime()
-        new_thmap = ThematicMap(np.zeros((1280, 1280)),
-                                {'DATE-OBS': str(self.parent.date),
-                                 'DATE': str(datetime.today())},
-                                self.parent.config.solar_class_name)
-        self.parent.annotator.loadThematicMap(new_thmap)
-        self.parent.controls.onTabChange()  # Us
-        self.close()
-        self.parent.setWindowTitle("SolarAnnotator: {}".format(new_thmap.date_obs))
-
-
-class ApplicationWindow(QtWidgets.QMainWindow):
-    def __init__(self, config_path):
-        super().__init__()
-        self.config = Config(config_path)
-        self.output_fn = None
-        self.initialized = False
-        self.initUI()
-        self.setWindowFlags(
-            QtCore.Qt.Window |
-            QtCore.Qt.CustomizeWindowHint |
-            QtCore.Qt.WindowTitleHint |
-            QtCore.Qt.WindowMinimizeButtonHint |
-            QtCore.Qt.WindowMaximizeButtonHint |
-            QtCore.Qt.WindowCloseButtonHint
-        )
-        self.setWindowTitle("SolarAnnotator")
-
-    def initUI(self):
-        self._main = QtWidgets.QWidget()
-        self.setCentralWidget(self._main)
-        layout = QtWidgets.QVBoxLayout(self._main)
-        self.annotator = AnnotationWidget(self.config)
-        layout.addWidget(self.annotator)
-
-        self._setup_control_layout()
-        layout.addLayout(self.control_layout)
-        self._setup_menubar()
-
-    def _setup_control_layout(self):
-        self.control_layout = QtWidgets.QHBoxLayout()
-        self.controls = ControlWidget(self.annotator)
-        self.control_layout.addWidget(self.controls)
-        self._setup_theme_radio_buttons()
-
-    def _setup_theme_radio_buttons(self):
-        def radio_button_font_color(background_color_hex):
-            """
-            Select white for dark color backgrounds and black for light colored backgrounds
-            """
-            background_color_rgb = ImageColor.getcolor(background_color_hex, "RGB")
-            if any([c < 50 for c in background_color_rgb]):
-                return "#FFFFFF"
-            else:
-                return "#000000"
-
-        theme_selection_layout = QtWidgets.QVBoxLayout()
-        radiobuttons = dict()
-
-        # add unlabelled button
-        radiobuttons['unlabeled'] = QRadioButton("unlabeled")
-        radiobuttons['unlabeled'].index = 0
-        radiobuttons['unlabeled'].setChecked(True)
-        radiobuttons['unlabeled'].toggled.connect(self.onClickedRadioButton)
-        background_color = '#FFFFFF'
-        font_color = radio_button_font_color(background_color)
-        radiobuttons['unlabeled'].setStyleSheet("QRadioButton"
-                                          "{"
-                                          "background-color : " + background_color + ";"
-                                          "color :" + font_color + ""
-                                           "}")
-        theme_selection_layout.addWidget(radiobuttons['unlabeled'])
-
-        # add rest of theme buttons
-        for theme, index in self.config.solar_class_index.items():
-            radiobuttons[theme] = QRadioButton(theme)
-            radiobuttons[theme].index = index
-            radiobuttons[theme].toggled.connect(self.onClickedRadioButton)
-            background_color = self.config.solar_colors[theme]
-            font_color = radio_button_font_color(background_color)
-            radiobuttons[theme].setStyleSheet("QRadioButton"
-                                       "{"
-                                       "background-color : " + background_color + ";"
-                                       "color :" + font_color + ""                                       
-                                       "}")
-
-            theme_selection_layout.addWidget(radiobuttons[theme])
-        self.control_layout.addLayout(theme_selection_layout)
-
-    def onClickedRadioButton(self):
-        radioButton = self.sender()
-        if radioButton.isChecked():
-            self.annotator.current_theme_index = radioButton.index
-
-    def _setup_menubar(self):
-        self.mainMenu = self.menuBar()
-        self.fileMenu = self.mainMenu.addMenu('File')
-
-        # File Menu
-        newButton = QAction("New", self)
-        newButton.setShortcut('Ctrl+N')
-        newButton.setStatusTip('Create new thematic map')
-        newButton.triggered.connect(self.new_file)
-        self.fileMenu.addAction(newButton)
-
-        openFile = QAction("&Open File", self)
-        openFile.setShortcut("Ctrl+O")
-        openFile.setStatusTip('Open File')
-        openFile.triggered.connect(self.file_open)
-        self.fileMenu.addAction(openFile)
-
-        saveFile = QAction("&Save", self)
-        saveFile.setShortcut("Ctrl+S")
-        saveFile.setStatusTip('Save File')
-        saveFile.triggered.connect(self.file_save)
-        self.fileMenu.addAction(saveFile)
-        self.fileMenu.addSeparator()
-
-        saveAsFile = QAction("&Save As...", self)
-        saveAsFile.setStatusTip('Save As...')
-        saveAsFile.triggered.connect(self.file_save_as)
-        self.fileMenu.addAction(saveAsFile)
-        self.fileMenu.addSeparator()
-
-        exitButton = QAction('Exit', self)
-        exitButton.setShortcut('Ctrl+Q')
-        exitButton.setStatusTip('Exit application')
-        exitButton.triggered.connect(self.exit)
-        self.fileMenu.addAction(exitButton)
-
-        # Edit Menu
-        self.editMenu = self.mainMenu.addMenu("Edit")
-        undoEdit = QAction("&Undo Edit", self)
-        undoEdit.setShortcut("Ctrl+Z")
-        undoEdit.setStatusTip('Undo a change on the thematic map')
-        undoEdit.triggered.connect(self.annotator.undo_action)
-        self.editMenu.addAction(undoEdit)
-        self.editMenu.addSeparator()
-
-        eraseBoundaries = QAction("&Erase boundaries", self)
-        eraseBoundaries.setShortcut("Ctrl+E")
-        eraseBoundaries.setStatusTip("Remove all the boundaries drawn on a map")
-        eraseBoundaries.triggered.connect(self.annotator.clearBoundaries)
-        self.editMenu.addAction(eraseBoundaries)
-
-    def exit(self):
-        if self.initialized:
-            answer = QMessageBox.question(self, '', "Would you like to save?",
-                                          QMessageBox.Yes | QMessageBox.No)
-            if answer == QMessageBox.Yes:
-                self.file_save_as()
-        sys.exit()
-
-    def closeEvent(self, *args, **kwargs):
-        self.exit()
-
-    def new_file(self):
-        self.new_file_popup = NewFilePopup(self)
-        self.new_file_popup.setGeometry(100, 200, 100, 100)
-        self.new_file_popup.show()
-        self.annotator.clearBoundaries()
-        self.initialized = True
-        self.output_fn = None
-
-    def file_open(self):
-        dlg = QFileDialog()
-        fname = dlg.getOpenFileName(None, "Open Thematic Map", "", "FITS files (*.fits)")
-        if fname != ('', ''):
-            thmap = ThematicMap.load(fname[0])
-            if thmap.complies_with_mapping(self.config.solar_class_name):
-                self.annotator.loadThematicMap(thmap)
-                self.controls.onTabChange()  # Use the tab change to automatically load the right image
-                self.annotator.clearBoundaries()
-                self.initialized = True
-                self.setWindowTitle("SolarAnnotator: {}".format(thmap.date_obs))
-                self.output_fn = None
-            else:
-                QMessageBox.critical(self,
-                                    'Error: Could not open',
-                                     'Thematic map could not open because theme mapping differs from configuration',
-                                     QMessageBox.Close)
-
-    def prompt_not_initialized(self):
-        QMessageBox.critical(self,
-                            "Error: Could not save",
-                            "You must create a new thematic map or load one before saving.",
-                            QMessageBox.Close)
-
-    def file_save(self):
-        if self.initialized:
-            if self.output_fn is None:
-                self.file_save_as()
-            else:
-                self.annotator.thmap.metadata['DATE'] = str(datetime.today())
-                self.annotator.thmap.save(self.output_fn)
-        else:
-            self.prompt_not_initialized()
-
-    def file_save_as(self):
-        if self.initialized:
-            dlg = QFileDialog()
-            fname = dlg.getSaveFileName(None, "Save Thematic Map", "", "FITS files (*.fits)")
-            if fname != ('', ''):
-                self.annotator.thmap.metadata['DATE'] = str(datetime.today())
-                self.annotator.thmap.save(fname[0])
-                self.output_fn = fname[0]
-        else:
-            self.prompt_not_initialized()
+import sys
+import PyQt5
+from PyQt5 import QtCore, QtWidgets
+from PyQt5.QtWidgets import QWidget, QLabel, QAction, QTabWidget, QPushButton, QFileDialog, QRadioButton, QMessageBox, \
+    QComboBox, QLineEdit, QSizePolicy, QCheckBox
+from PyQt5.QtCore import QDateTime
+from PyQt5.QtGui import QIcon, QDoubleValidator
+from datetime import datetime, timedelta
+from matplotlib import path
+from matplotlib.collections import PatchCollection
+from matplotlib.patches import Polygon
+from skimage.morphology import binary_erosion
+import scipy
+import numpy as np
+from matplotlib.widgets import LassoSelector
+from matplotlib.backends.qt_compat import QtCore, QtWidgets
+from PIL import ImageColor
+from matplotlib.backends.backend_qt5agg import FigureCanvas, NavigationToolbar2QT as NavigationToolbar
+from matplotlib.figure import Figure
+
+from solarannotator.template import create_thmap_template
+
+if hasattr(QtCore.Qt, 'AA_EnableHighDpiScaling'):
+    PyQt5.QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)
+
+if hasattr(QtCore.Qt, 'AA_UseHighDpiPixmaps'):
+    PyQt5.QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps, True)
+
+from .config import Config
+from .io import ThematicMap, ImageSet
+
+
+class AnnotationWidget(QtWidgets.QWidget):
+    def __init__(self, config):
+        super().__init__()
+        self.composites = ImageSet.create_empty()
+        self.current_theme_index = 0
+
+        self.preview_data = self.composites['94'].data.copy()
+        self.thmap_data = np.zeros((1280, 1280))
+        self.thmap = ThematicMap(self.thmap_data, {'DATE-OBS': str(datetime.today())}, config.solar_class_name)
+
+        self.history = []
+
+        layout = QtWidgets.QVBoxLayout()
+
+        self.fig = Figure(figsize=(15, 10))
+        canvas = FigureCanvas(self.fig)
+        canvas.mpl_connect('button_press_event', self.onclick)
+
+        layout.addWidget(canvas)
+
+        self.region_patches = []
+        self.axs = canvas.figure.subplots(ncols=2, sharex=True, sharey=True)
+        self.preview_axesimage = self.axs[0].imshow(self.preview_data, vmin=0, vmax=1, cmap='gray', origin='lower')
+        self.thmap_axesimage = self.axs[1].imshow(self.thmap_data, origin='lower', interpolation='none',
+                                                  vmin=0, vmax=config.max_index, cmap=config.solar_cmap)
+        self.axs[0].set_axis_off()
+        self.axs[1].set_axis_off()
+        self.axs[0].set_title("Preview")
+        self.axs[1].set_title("Thematic Map")
+
+        self.toolbar = NavigationToolbar(canvas, self)
+        layout.addWidget(self.toolbar)
+        self.setLayout(layout)
+
+        # add selection layer for lasso
+        self.shape = (1280, 1280)  # TODO: replace with dynamic detection
+        self.pix = np.arange(self.shape[0])  # assumes square image
+        xv, yv = np.meshgrid(self.pix, self.pix)
+        self.pix = np.vstack((xv.flatten(), yv.flatten())).T
+
+        lineprops = dict(color="red", linewidth=2)
+        self.lasso = LassoSelector(self.axs[0], self.onlasso, props=lineprops)
+        self.fig.tight_layout()
+
+    def onlasso(self, verts):
+        """
+        Main function to control the action of the lasso, allows user to draw on data image and adjust thematic map
+        :param verts: the vertices selected by the lasso
+        :return: nothin, but update the selection array so lassoed region now has the selected theme, redraws canvas
+        """
+        p = path.Path(verts)
+        ind = p.contains_points(self.pix, radius=1)
+        self.history.append(self.thmap_data.copy())
+        self.thmap_data = self.updateArray(self.thmap_data,
+                                                ind,
+                                                self.current_theme_index)
+        self.thmap_axesimage.set_data(self.thmap_data)
+        self.fig.canvas.draw_idle()
+        self.thmap.data = self.thmap_data
+
+    def rename_region(self, event):
+        # draw patches
+        y, x = int(event.xdata), int(event.ydata)
+        self.history.append(self.thmap_data.copy())
+        label = self.thmap_data[x, y]
+        contiguous_regions = scipy.ndimage.label(self.thmap_data == label)[0]
+        this_region = contiguous_regions == (contiguous_regions[x, y])
+        self.thmap_data[this_region] = self.current_theme_index
+        self.thmap_axesimage.set_data(self.thmap_data)
+        self.thmap.data = self.thmap_data
+        self.fig.canvas.draw_idle()
+
+    def draw_event_region_boundary(self, event):
+        """
+        Draw a patch around the contiguous region in the preview image
+        :param event:
+        :return:
+        """
+        # draw patches
+        y, x = int(event.xdata), int(event.ydata)
+        label = self.thmap_data[x, y]
+        contiguous_regions = scipy.ndimage.label(self.thmap_data == label)[0]
+        this_region = contiguous_regions == (contiguous_regions[x, y])
+
+        # remove the boundaries so any region touching the edge isn't drawn odd
+        this_region[0, :] = 0
+        this_region[:, 0] = 0
+        this_region[this_region.shape[0] - 1, :] = 0
+        this_region[:, this_region.shape[1] - 1] = 0
+
+        # convert the region mask into just a true/false array of its boundary pixels
+        edges = binary_erosion(this_region) ^ this_region
+
+        # convert the boundary pixels into a path, moving around instead of just where
+        x, y = np.where(edges)
+        coords = np.dstack([x, y])[0]
+        path = [coords[0]]
+        coords = coords[1:]
+
+        while len(coords):
+            dist = np.sum(np.abs(path[-1] - coords), axis=1)
+            neighbor_index = np.argmin(dist)
+
+            if dist[neighbor_index] < 5:
+                path.append(coords[neighbor_index].copy())
+                coords[neighbor_index:-1] = coords[neighbor_index + 1:]
+                coords = coords[:-1]
+            else:
+                break
+
+        path = np.array(path)
+
+        clips = []
+        while len(coords) > 5:
+            dist = np.sum(np.abs(path[-1] - coords), axis=1)
+            neighbor_index = np.argmin(dist)
+            clip = [coords[neighbor_index].copy()]
+            coords[neighbor_index:-1] = coords[neighbor_index + 1:]
+            coords = coords[:-1]
+            while len(coords):
+                dist = np.sum(np.abs(clip[-1] - coords), axis=1)
+                neighbor_index = np.argmin(dist)
+                if dist[neighbor_index] < 5:
+                    clip.append(coords[neighbor_index].copy())
+                    coords[neighbor_index:-1] = coords[neighbor_index + 1:]
+                    coords = coords[:-1]
+                else:
+                    break
+            clips.append(np.array(clip))
+
+        # draw the continguous  on the selection area
+        self.region_patches.append(PatchCollection(
+            [Polygon(np.dstack([path[:, 1], path[:, 0]])[0], False,
+                     fill=False, facecolor=None,
+                     edgecolor="black", alpha=1, lw=2.5)] +
+            [Polygon(np.dstack([clip[:, 1], clip[:, 0]])[0], False,
+                     fill=False, facecolor=None,
+                     edgecolor="black", alpha=1, lw=2.0) for clip in clips],
+            match_original=True))
+        self.axs[0].add_collection(self.region_patches[-1])
+        self.fig.canvas.draw_idle()
+
+    def undo_action(self):
+        """ when undo is clicked, revert the thematic map to the previous state"""
+        if len(self.history) > 1:
+            old = self.history.pop(-1)
+            self.thmap_data = old
+            self.thmap.data = self.thmap_data
+            self.thmap_axesimage.set_data(old)
+            self.fig.canvas.draw_idle()
+
+    def onclick(self, event):
+        """
+        Draw contours on the data for a click in the thematic map
+        :param event: mouse click on thematic map preview
+        """
+        if event.inaxes == self.axs[1]:
+            if event.button == 3:  # right click feature
+                self.draw_event_region_boundary(event)
+            if event.button == 1 and self.toolbar.mode == "":
+                self.rename_region(event)
+
+    def updateArray(self, array, indices, value):
+        """
+        updates array so that pixels at indices take on value
+        :param array: (m,n) array to adjust
+        :param indices: flattened image indices to change value
+        :param value: new value to assign
+        :return: the changed (m,n) array
+        """
+        lin = np.arange(array.size)
+        new_array = array.flatten()
+        new_array[lin[indices]] = value
+        return new_array.reshape(array.shape)
+
+    def clearBoundaries(self):
+        for patch in self.region_patches:
+            patch.remove()
+        self.region_patches = []
+        self.fig.canvas.draw_idle()
+
+    def loadThematicMap(self, thmap, template=True):
+        try:
+            download_message = QMessageBox.information(self,
+                                                       'Downloading',
+                                                       "Downloads may take a few moments. Click 'ok' to proceed.",
+                                                       QMessageBox.Ok)
+            self.composites = ImageSet.retrieve(thmap.date_obs)
+        except RuntimeError:
+            self.data_does_not_exist_popup()
+        else:
+            self.thmap = thmap
+            if template:
+                self.thmap = create_thmap_template(self.composites)
+            self.thmap.copy_195_metadata(self.composites)
+            self.history = [thmap.data.copy()]
+            self.thmap_data = self.thmap.data
+            self.thmap_axesimage.set_data(self.thmap_data)
+            self.preview_axesimage.set_data(self.composites['94'].data)
+            self.fig.canvas.draw_idle()
+
+    def updateSingleColorImage(self, channel, lower_percentile, upper_percentile, scale):
+        self.preview_data = self.composites[channel].data.copy()
+        self.preview_data = np.power(np.abs(self.preview_data), scale) * np.sign(self.preview_data)
+        lower = np.nanpercentile(self.preview_data, lower_percentile)
+        upper = np.nanpercentile(self.preview_data, upper_percentile)
+        self.preview_data[self.preview_data < lower] = lower
+        self.preview_data[self.preview_data > upper] = upper
+        self.preview_data = (self.preview_data - np.nanmin(self.preview_data)) \
+                            / (np.nanmax(self.preview_data) - np.nanmin(self.preview_data))
+        # self.preview_data /= np.nanmax(self.preview_data)
+        self.preview_axesimage.set_data(self.preview_data)
+        self.fig.canvas.draw_idle()
+
+    def updateThreeColorImage(self, red_channel, green_channel, blue_channel,
+                              red_min, green_min, blue_min,
+                              red_max, green_max, blue_max,
+                              red_scale, green_scale, blue_scale):
+        self.preview_data = np.stack([self.composites[red_channel].data.copy(),
+                                     self.composites[green_channel].data.copy(),
+                                     self.composites[blue_channel].data.copy()], axis=2)
+        self.preview_data[:, :, 0] = np.power(self.preview_data[:, :, 0], red_scale)
+        self.preview_data[:, :, 1] = np.power(self.preview_data[:, :, 1], green_scale)
+        self.preview_data[:, :, 2] = np.power(self.preview_data[:, :, 2], blue_scale)
+
+        red_lower = np.nanpercentile(self.preview_data[:, :, 0], red_min)
+        green_lower = np.nanpercentile(self.preview_data[:, :, 1], green_min)
+        blue_lower = np.nanpercentile(self.preview_data[:, :, 2], blue_min)
+
+        red_upper = np.nanpercentile(self.preview_data[:, :, 0], red_max)
+        green_upper = np.nanpercentile(self.preview_data[:, :, 1], green_max)
+        blue_upper = np.nanpercentile(self.preview_data[:, :, ], blue_max)
+
+        self.preview_data[self.preview_data[:, :, 0] < red_lower] = red_lower
+        self.preview_data[self.preview_data[:, :, 0] > red_upper] = red_upper
+        self.preview_data[self.preview_data[:, :, 1] < green_lower] = green_lower
+        self.preview_data[self.preview_data[:, :, 1] > green_upper] = green_upper
+        self.preview_data[self.preview_data[:, :, 2] < blue_lower] = blue_lower
+        self.preview_data[self.preview_data[:, :, 2] > blue_upper] = blue_upper
+        
+        for index in [0, 1, 2]:
+            # self.preview_data[:, :, index] /= np.nanmax(self.preview_data[:, :, index])
+            self.preview_data[:, :, index] = (self.preview_data[:, :, index] - np.nanmin(self.preview_data[:, :, index])) \
+                                / (np.nanmax(self.preview_data[:, :, index]) - np.nanmin(self.preview_data[:, :, index]))
+        self.preview_axesimage.set_data(self.preview_data)
+        self.fig.canvas.draw_idle()
+
+    def data_does_not_exist_popup(self):
+        QMessageBox.critical(self,
+                             'Error: Could not open',
+                             'Composite data does not exist for that date.',
+                             QMessageBox.Close)
+
+
+class ControlWidget(QtWidgets.QWidget):
+    def __init__(self, annotator):
+        super().__init__()
+        self.annotator = annotator
+
+        layout = QtWidgets.QHBoxLayout()
+        self.tabs = QTabWidget()
+        self.one_color_tab = QWidget()
+        self.three_color_tab = QWidget()
+
+        # Add tabs
+        self.tabs.addTab(self.one_color_tab, "Single")
+        self.tabs.addTab(self.three_color_tab, "Three-color")
+        self.tabs.currentChanged.connect(self.onTabChange)
+
+        self.initSingleColorUI()
+        self.initThreeColorUI()
+
+        layout.addWidget(self.tabs)
+        self.setLayout(layout)
+
+    def initSingleColorUI(self):
+        # Create single color tab
+        self.one_color_tab.layout = QtWidgets.QGridLayout(self)
+
+        self.single_color_label = QLabel()
+        self.single_color_label.setText("Channel")
+        self.one_color_tab.layout.addWidget(self.single_color_label)
+        self.single_color_combo_box = QComboBox()
+        self.single_color_combo_box.addItems(self.annotator.composites.channels())
+        self.single_color_combo_box.currentTextChanged.connect(self.onSingleColorChange)
+
+        self.one_color_min_editor = QLineEdit()
+        self.one_color_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.one_color_min_editor.setText("3.0")
+        self.one_color_min_editor.editingFinished.connect(self.onSingleColorChange)
+
+        self.one_color_max_editor = QLineEdit()
+        self.one_color_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.one_color_max_editor.setText("99.9")
+        self.one_color_max_editor.editingFinished.connect(self.onSingleColorChange)
+
+        self.one_color_scale_editor = QLineEdit()
+        self.one_color_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.one_color_scale_editor.setText("0.25")
+        self.one_color_scale_editor.editingFinished.connect(self.onSingleColorChange)
+
+        channel_label = QLabel("Channel", self)
+        channel_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        min_label = QLabel("Min", self)
+        min_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        max_label = QLabel("Max", self)
+        max_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        scale_label = QLabel("Scale", self)
+        scale_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+
+        self.one_color_tab.setLayout(self.one_color_tab.layout)
+        self.one_color_tab.layout.addWidget(channel_label, 0, 1)
+        self.one_color_tab.layout.addWidget(min_label, 0, 2)
+        self.one_color_tab.layout.addWidget(max_label, 0, 3)
+        self.one_color_tab.layout.addWidget(scale_label, 0, 4)
+        self.one_color_tab.layout.addWidget(self.single_color_label, 1, 0)
+        self.one_color_tab.layout.addWidget(self.single_color_combo_box, 1, 1)
+        self.one_color_tab.layout.addWidget(self.one_color_min_editor, 1, 2)
+        self.one_color_tab.layout.addWidget(self.one_color_max_editor, 1, 3)
+        self.one_color_tab.layout.addWidget(self.one_color_scale_editor, 1, 4)
+
+
+    def initThreeColorUI(self):
+        self.three_color_tab.layout = QtWidgets.QGridLayout(self)
+
+        channel_label = QLabel("Channel")
+        channel_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        min_label = QLabel("Min")
+        min_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        max_label = QLabel("Max")
+        max_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+        scale_label = QLabel("Scale")
+        scale_label.setAlignment(QtCore.Qt.AlignHCenter | QtCore.Qt.AlignBottom)
+
+        self.red_label = QLabel()
+        self.red_label.setText("Red Channel")
+        self.red_label.setAlignment(QtCore.Qt.AlignRight)
+        self.red_combo_box = QComboBox()
+        self.red_combo_box.addItems(self.annotator.composites.channels())
+        self.red_combo_box.setCurrentIndex(2)
+        self.red_combo_box.currentTextChanged.connect(self.onThreeColorChange)
+        self.red_min_editor = QLineEdit()
+        self.red_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.red_min_editor.setText("3.0")
+        self.red_min_editor.editingFinished.connect(self.onThreeColorChange)
+        self.red_max_editor = QLineEdit()
+        self.red_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.red_max_editor.setText("99.9")
+        self.red_max_editor.editingFinished.connect(self.onThreeColorChange)
+        self.red_scale_editor = QLineEdit()
+        self.red_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.red_scale_editor.setText("0.25")
+        self.red_scale_editor.editingFinished.connect(self.onThreeColorChange)
+
+        self.green_label = QLabel()
+        self.green_label.setText("Green Channel")
+        self.green_label.setAlignment(QtCore.Qt.AlignRight)
+        self.green_combo_box = QComboBox()
+        self.green_combo_box.addItems(self.annotator.composites.channels())
+        self.green_combo_box.setCurrentIndex(3)
+        self.green_combo_box.currentTextChanged.connect(self.onThreeColorChange)
+        self.green_min_editor = QLineEdit()
+        self.green_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.green_min_editor.setText("3.0")
+        self.green_min_editor.editingFinished.connect(self.onThreeColorChange)
+        self.green_max_editor = QLineEdit()
+        self.green_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.green_max_editor.setText("99.9")
+        self.green_max_editor.editingFinished.connect(self.onThreeColorChange)
+        self.green_scale_editor = QLineEdit()
+        self.green_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.green_scale_editor.setText("0.25")
+        self.green_scale_editor.editingFinished.connect(self.onThreeColorChange)
+
+        self.blue_label = QLabel()
+        self.blue_label.setText("Blue Channel")
+        self.blue_label.setAlignment(QtCore.Qt.AlignRight)
+        self.blue_combo_box = QComboBox()
+        self.blue_combo_box.addItems(self.annotator.composites.channels())
+        self.blue_combo_box.setCurrentIndex(4)
+        self.blue_combo_box.currentTextChanged.connect(self.onThreeColorChange)
+        self.blue_min_editor = QLineEdit()
+        self.blue_min_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.blue_min_editor.setText("3.0")
+        self.blue_min_editor.editingFinished.connect(self.onThreeColorChange)
+        self.blue_max_editor = QLineEdit()
+        self.blue_max_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.blue_max_editor.setText("99.9")
+        self.blue_max_editor.editingFinished.connect(self.onThreeColorChange)
+        self.blue_scale_editor = QLineEdit()
+        self.blue_scale_editor.setValidator(QDoubleValidator(0.0, 100.0, 3))
+        self.blue_scale_editor.setText("0.25")
+        self.blue_scale_editor.editingFinished.connect(self.onThreeColorChange)
+
+        self.three_color_tab.setLayout(self.three_color_tab.layout)
+        self.three_color_tab.layout.addWidget(self.red_label, 1, 0)
+        self.three_color_tab.layout.addWidget(self.green_label, 2, 0)
+        self.three_color_tab.layout.addWidget(self.blue_label, 3, 0)
+        self.three_color_tab.layout.addWidget(channel_label, 0, 1)
+        self.three_color_tab.layout.addWidget(self.red_combo_box, 1, 1)
+        self.three_color_tab.layout.addWidget(self.green_combo_box, 2, 1)
+        self.three_color_tab.layout.addWidget(self.blue_combo_box, 3, 1)
+        self.three_color_tab.layout.addWidget(min_label, 0, 2)
+        self.three_color_tab.layout.addWidget(self.red_min_editor, 1, 2)
+        self.three_color_tab.layout.addWidget(self.green_min_editor, 2, 2)
+        self.three_color_tab.layout.addWidget(self.blue_min_editor, 3, 2)
+        self.three_color_tab.layout.addWidget(max_label, 0, 3)
+        self.three_color_tab.layout.addWidget(self.red_max_editor, 1, 3)
+        self.three_color_tab.layout.addWidget(self.green_max_editor, 2, 3)
+        self.three_color_tab.layout.addWidget(self.blue_max_editor, 3, 3)
+        self.three_color_tab.layout.addWidget(scale_label, 0, 4)
+        self.three_color_tab.layout.addWidget(self.red_scale_editor, 1, 4)
+        self.three_color_tab.layout.addWidget(self.green_scale_editor, 2, 4)
+        self.three_color_tab.layout.addWidget(self.blue_scale_editor, 3, 4)
+
+    def onTabChange(self):
+        if self.tabs.currentIndex() == 0:
+            self.onSingleColorChange()
+        elif self.tabs.currentIndex() == 1:
+            self.onThreeColorChange()
+
+    def onSingleColorChange(self):
+        self.annotator.updateSingleColorImage(self.single_color_combo_box.currentText(),
+                                              float(self.one_color_min_editor.text()),
+                                              float(self.one_color_max_editor.text()),
+                                              float(self.one_color_scale_editor.text()))
+
+    def onThreeColorChange(self):
+        red_channel = self.red_combo_box.currentText()
+        green_channel = self.green_combo_box.currentText()
+        blue_channel = self.blue_combo_box.currentText()
+        self.annotator.updateThreeColorImage(red_channel, green_channel, blue_channel,
+                                             float(self.red_min_editor.text()),
+                                             float(self.green_min_editor.text()),
+                                             float(self.blue_min_editor.text()),
+                                             float(self.red_max_editor.text()),
+                                             float(self.green_max_editor.text()),
+                                             float(self.blue_max_editor.text()),
+                                             float(self.red_scale_editor.text()),
+                                             float(self.green_scale_editor.text()),
+                                             float(self.blue_scale_editor.text()))
+
+
+class NewFilePopup(QWidget):
+    def __init__(self, parent):
+        super().__init__()
+        self.parent = parent
+        self.initUI()
+
+    def initUI(self):
+        layout = QtWidgets.QHBoxLayout()
+        instructions = QLabel("Please select a time for the new file.", self)
+        self.dateEdit = QtWidgets.QDateTimeEdit(QDateTime.currentDateTime())
+        self.template_option = QCheckBox("Use template")
+        self.template_option.setChecked(True)
+        submit_button = QPushButton("Submit")
+        layout.addWidget(instructions)
+        layout.addWidget(self.dateEdit)
+        layout.addWidget(self.template_option)
+        layout.addWidget(submit_button)
+        self.setLayout(layout)
+        submit_button.clicked.connect(self.onSubmit)
+
+    def onSubmit(self):
+        # set the date in the application and close
+        self.parent.date = self.dateEdit.dateTime().toPyDateTime()
+        new_thmap = ThematicMap(np.zeros((1280, 1280)),
+                                {'DATE-OBS': str(self.parent.date),
+                                 'DATE': str(datetime.today())},
+                                self.parent.config.solar_class_name)
+        self.parent.annotator.loadThematicMap(new_thmap, self.template_option.isChecked())
+        self.parent.controls.onTabChange()  # Us
+        self.close()
+        self.parent.setWindowTitle("SolarAnnotator: {}".format(new_thmap.date_obs))
+
+
+class ApplicationWindow(QtWidgets.QMainWindow):
+    def __init__(self, config_path):
+        super().__init__()
+        self.config = Config(config_path)
+        self.output_fn = None
+        self.initialized = False
+        self.initUI()
+        self.setWindowFlags(
+            QtCore.Qt.Window |
+            QtCore.Qt.CustomizeWindowHint |
+            QtCore.Qt.WindowTitleHint |
+            QtCore.Qt.WindowMinimizeButtonHint |
+            QtCore.Qt.WindowMaximizeButtonHint |
+            QtCore.Qt.WindowCloseButtonHint
+        )
+        self.setWindowTitle("SolarAnnotator")
+
+    def initUI(self):
+        self._main = QtWidgets.QWidget()
+        self.setCentralWidget(self._main)
+        layout = QtWidgets.QVBoxLayout(self._main)
+        self.annotator = AnnotationWidget(self.config)
+        layout.addWidget(self.annotator)
+
+        self._setup_control_layout()
+        layout.addLayout(self.control_layout)
+        self._setup_menubar()
+
+    def _setup_control_layout(self):
+        self.control_layout = QtWidgets.QHBoxLayout()
+        self.controls = ControlWidget(self.annotator)
+        self.control_layout.addWidget(self.controls)
+        self._setup_theme_radio_buttons()
+
+    def _setup_theme_radio_buttons(self):
+        def radio_button_font_color(background_color_hex):
+            """
+            Select white for dark color backgrounds and black for light colored backgrounds
+            """
+            background_color_rgb = ImageColor.getcolor(background_color_hex, "RGB")
+            if any([c < 50 for c in background_color_rgb]):
+                return "#FFFFFF"
+            else:
+                return "#000000"
+
+        theme_selection_layout = QtWidgets.QVBoxLayout()
+        radiobuttons = dict()
+
+        # add unlabelled button
+        radiobuttons['unlabeled'] = QRadioButton("unlabeled")
+        radiobuttons['unlabeled'].index = 0
+        radiobuttons['unlabeled'].setChecked(True)
+        radiobuttons['unlabeled'].toggled.connect(self.onClickedRadioButton)
+        background_color = '#FFFFFF'
+        font_color = radio_button_font_color(background_color)
+        radiobuttons['unlabeled'].setStyleSheet("QRadioButton"
+                                          "{"
+                                          "background-color : " + background_color + ";"
+                                          "color :" + font_color + ""
+                                           "}")
+        theme_selection_layout.addWidget(radiobuttons['unlabeled'])
+
+        # add rest of theme buttons
+        for theme, index in self.config.solar_class_index.items():
+            radiobuttons[theme] = QRadioButton(theme)
+            radiobuttons[theme].index = index
+            radiobuttons[theme].toggled.connect(self.onClickedRadioButton)
+            background_color = self.config.solar_colors[theme]
+            font_color = radio_button_font_color(background_color)
+            radiobuttons[theme].setStyleSheet("QRadioButton"
+                                       "{"
+                                       "background-color : " + background_color + ";"
+                                       "color :" + font_color + ""                                       
+                                       "}")
+
+            theme_selection_layout.addWidget(radiobuttons[theme])
+        self.control_layout.addLayout(theme_selection_layout)
+
+    def onClickedRadioButton(self):
+        radioButton = self.sender()
+        if radioButton.isChecked():
+            self.annotator.current_theme_index = radioButton.index
+
+    def _setup_menubar(self):
+        self.mainMenu = self.menuBar()
+        self.fileMenu = self.mainMenu.addMenu('File')
+
+        # File Menu
+        newButton = QAction("New", self)
+        newButton.setShortcut('Ctrl+N')
+        newButton.setStatusTip('Create new thematic map')
+        newButton.triggered.connect(self.new_file)
+        self.fileMenu.addAction(newButton)
+
+        openFile = QAction("&Open File", self)
+        openFile.setShortcut("Ctrl+O")
+        openFile.setStatusTip('Open File')
+        openFile.triggered.connect(self.file_open)
+        self.fileMenu.addAction(openFile)
+
+        saveFile = QAction("&Save", self)
+        saveFile.setShortcut("Ctrl+S")
+        saveFile.setStatusTip('Save File')
+        saveFile.triggered.connect(self.file_save)
+        self.fileMenu.addAction(saveFile)
+        self.fileMenu.addSeparator()
+
+        saveAsFile = QAction("&Save As...", self)
+        saveAsFile.setStatusTip('Save As...')
+        saveAsFile.triggered.connect(self.file_save_as)
+        self.fileMenu.addAction(saveAsFile)
+        self.fileMenu.addSeparator()
+
+        exitButton = QAction('Exit', self)
+        exitButton.setShortcut('Ctrl+Q')
+        exitButton.setStatusTip('Exit application')
+        exitButton.triggered.connect(self.exit)
+        self.fileMenu.addAction(exitButton)
+
+        # Edit Menu
+        self.editMenu = self.mainMenu.addMenu("Edit")
+        undoEdit = QAction("&Undo Edit", self)
+        undoEdit.setShortcut("Ctrl+Z")
+        undoEdit.setStatusTip('Undo a change on the thematic map')
+        undoEdit.triggered.connect(self.annotator.undo_action)
+        self.editMenu.addAction(undoEdit)
+        self.editMenu.addSeparator()
+
+        eraseBoundaries = QAction("&Erase boundaries", self)
+        eraseBoundaries.setShortcut("Ctrl+E")
+        eraseBoundaries.setStatusTip("Remove all the boundaries drawn on a map")
+        eraseBoundaries.triggered.connect(self.annotator.clearBoundaries)
+        self.editMenu.addAction(eraseBoundaries)
+
+    def exit(self):
+        if self.initialized:
+            answer = QMessageBox.question(self, '', "Would you like to save?",
+                                          QMessageBox.Yes | QMessageBox.No)
+            if answer == QMessageBox.Yes:
+                self.file_save_as()
+        sys.exit()
+
+    def closeEvent(self, *args, **kwargs):
+        self.exit()
+
+    def new_file(self):
+        self.new_file_popup = NewFilePopup(self)
+        self.new_file_popup.setGeometry(100, 200, 100, 100)
+        self.new_file_popup.show()
+        self.annotator.clearBoundaries()
+        self.initialized = True
+        self.output_fn = None
+
+    def file_open(self):
+        dlg = QFileDialog()
+        fname = dlg.getOpenFileName(None, "Open Thematic Map", "", "FITS files (*.fits)")
+        if fname != ('', ''):
+            thmap = ThematicMap.load(fname[0])
+            if thmap.complies_with_mapping(self.config.solar_class_name):
+                self.annotator.loadThematicMap(thmap)
+                self.controls.onTabChange()  # Use the tab change to automatically load the right image
+                self.annotator.clearBoundaries()
+                self.initialized = True
+                self.setWindowTitle("SolarAnnotator: {}".format(thmap.date_obs))
+                self.output_fn = None
+            else:
+                QMessageBox.critical(self,
+                                    'Error: Could not open',
+                                     'Thematic map could not open because theme mapping differs from configuration',
+                                     QMessageBox.Close)
+
+    def prompt_not_initialized(self):
+        QMessageBox.critical(self,
+                            "Error: Could not save",
+                            "You must create a new thematic map or load one before saving.",
+                            QMessageBox.Close)
+
+    def file_save(self):
+        if self.initialized:
+            if self.output_fn is None:
+                self.file_save_as()
+            else:
+                self.annotator.thmap.metadata['DATE'] = str(datetime.today())
+                self.annotator.thmap.save(self.output_fn)
+        else:
+            self.prompt_not_initialized()
+
+    def file_save_as(self):
+        if self.initialized:
+            dlg = QFileDialog()
+            fname = dlg.getSaveFileName(None, "Save Thematic Map", "", "FITS files (*.fits)")
+            if fname != ('', ''):
+                self.annotator.thmap.metadata['DATE'] = str(datetime.today())
+                self.annotator.thmap.save(fname[0])
+                self.output_fn = fname[0]
+        else:
+            self.prompt_not_initialized()
```

### Comparing `solarannotator-0.3.1/solarannotator/main.py` & `solarannotator-1.0.0/solarannotator/main.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/env python3
-
-from solarannotator.gui import ApplicationWindow
-from PyQt5 import QtWidgets
-import argparse
-import os
-import sys
-
-
-def main():
-    parser = argparse.ArgumentParser(description='Annotate solar images with labels')
-    parser.add_argument('--config', help='a configuration file to load',
-                        default=os.path.join(sys.prefix, 'solarannotator/default.json'))
-    args = parser.parse_args()
-
-    # Check whether there is already a running QApplication (e.g., if running
-    # from an IDE).
-    qapp = QtWidgets.QApplication.instance()
-    if not qapp:
-        qapp = QtWidgets.QApplication(sys.argv)
-
-    app = ApplicationWindow(args.config)
-    app.show()
-    app.activateWindow()
-    app.raise_()
-    qapp.exec_()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python3
+
+from solarannotator.gui import ApplicationWindow
+from PyQt5 import QtWidgets
+import argparse
+import os
+import sys
+
+
+def main():
+    parser = argparse.ArgumentParser(description='Annotate solar images with labels')
+    parser.add_argument('--config', help='a configuration file to load',
+                        default=os.path.join(sys.prefix, 'solarannotator/default.json'))
+    args = parser.parse_args()
+
+    # Check whether there is already a running QApplication (e.g., if running
+    # from an IDE).
+    qapp = QtWidgets.QApplication.instance()
+    if not qapp:
+        qapp = QtWidgets.QApplication(sys.argv)
+
+    app = ApplicationWindow(args.config)
+    app.show()
+    app.activateWindow()
+    app.raise_()
+    qapp.exec_()
+
+
+if __name__ == "__main__":
+    main()
```

