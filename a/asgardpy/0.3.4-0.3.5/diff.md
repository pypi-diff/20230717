# Comparing `tmp/asgardpy-0.3.4.tar.gz` & `tmp/asgardpy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.3.4.tar", last modified: Sun Jul  2 20:26:38 2023, max compression
+gzip compressed data, was "asgardpy-0.3.5.tar", last modified: Mon Jul 17 00:34:03 2023, max compression
```

## Comparing `asgardpy-0.3.4.tar` & `asgardpy-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-02 20:26:16.000000 asgardpy-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-02 20:26:38.115688 asgardpy-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-02 20:26:16.000000 asgardpy-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/config/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24791 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dataset_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dl4.py
--rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-02 20:26:16.000000 asgardpy-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-02 20:26:38.115688 asgardpy-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-02 20:26:16.000000 asgardpy-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-17 00:33:45.000000 asgardpy-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 00:34:03.164307 asgardpy-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-17 00:33:45.000000 asgardpy-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25065 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38087 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-17 00:33:45.000000 asgardpy-0.3.5/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 00:34:03.000000 asgardpy-0.3.5/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 00:33:45.000000 asgardpy-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 00:34:03.164307 asgardpy-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-17 00:33:45.000000 asgardpy-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:34:03.164307 asgardpy-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 00:33:45.000000 asgardpy-0.3.5/tests/test_basic.py
```

### Comparing `asgardpy-0.3.4/LICENSE` & `asgardpy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.4/PKG-INFO` & `asgardpy-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.4
+Version: 0.3.5
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
@@ -32,10 +32,13 @@
 
 The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
+# Cite
+If you use Asgardpy in a publication, please cite the exact version you used from Zenodo _Cite as_ https://doi.org/10.5281/zenodo.8106369
+
 # Pipeline Template
 
 Pipeline generated based on the template by [python-package-template](https://github.com/allenai/python-package-template).
```

### Comparing `asgardpy-0.3.4/README.md` & `asgardpy-0.3.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
@@ -13,10 +13,13 @@
 
 The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
+# Cite
+If you use Asgardpy in a publication, please cite the exact version you used from Zenodo _Cite as_ https://doi.org/10.5281/zenodo.8106369
+
 # Pipeline Template
 
 Pipeline generated based on the template by [python-package-template](https://github.com/allenai/python-package-template).
```

### Comparing `asgardpy-0.3.4/asgardpy/analysis/analysis.py` & `asgardpy-0.3.5/asgardpy/analysis/analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 from gammapy.datasets import Datasets
 from gammapy.modeling.models import Models
 
 from asgardpy.base import AnalysisStep
 from asgardpy.config import AsgardpyConfig
-from asgardpy.data import apply_selection_mask_to_models, set_models
+from asgardpy.data import set_models
 
 log = logging.getLogger(__name__)
 
 __all__ = ["AsgardpyAnalysis"]
 
 
 class AsgardpyAnalysis:
@@ -80,90 +80,79 @@
     def run(self, steps=None, overwrite=None, **kwargs):
         if steps is None:
             steps = self.config.general.steps
             overwrite = self.config.general.overwrite
         else:
             if overwrite is None:
                 overwrite = True
-        for step in steps:
-            if "datasets" in step:
+
+        dl3_dl4_steps = [step for step in steps if "datasets" in step]
+        dl4_dl5_steps = [step for step in steps if "datasets" not in step]
+
+        if len(dl3_dl4_steps) > 0:
+            self.log.info("Perform DL3 to DL4 process!")
+
+            for step in dl3_dl4_steps:
                 analysis_step = AnalysisStep.create(step, self.config, **kwargs)
+
                 datasets_list, models_list, instrument_spectral_info = analysis_step.run()
 
-                if step == "datasets-3d":
+                if models_list:
+                    # This step is only valid for 3D Datasets which have a list of models
                     target_source_model = models_list[self.config.target.source_name]
 
                     if target_source_model.spatial_model:
                         # If the target source has Spatial model included,
                         # only then (?) get all the models as final_model.
                         # Needs reconsideration.
                         for m in models_list:
                             self.final_model.append(m)
                     else:
                         self.log.info(
                             f"The target source only has spectral model:{target_source_model}"
                         )
 
-                    # To get all datasets_names from the target source model.
-                    if target_source_model.datasets_names:
-                        for names in target_source_model.datasets_names:
-                            # Only update the list if a new name is found.
-                            if names not in self.dataset_name_list:
-                                self.dataset_name_list.append(names)
-
-                    # Finally, simply update the final datasets list
-                    for data in datasets_list:
-                        self.datasets.append(data)
-
-                if step == "datasets-1d":
-                    for data in datasets_list:
-                        if data.name not in self.dataset_name_list:
-                            self.dataset_name_list.append(data.name)
-                        self.datasets.append(data)
+                # To get all datasets_names from the datasets and update the final datasets list
+                for data in datasets_list:
+                    if data.name not in self.dataset_name_list:
+                        self.dataset_name_list.append(data.name)
+                    self.datasets.append(data)
 
                 # Update the name and spectral energy ranges for each
                 # instrument Datasets, to be used for the FluxPointsAnalysisStep.
                 for name in instrument_spectral_info["name"]:
                     self.instrument_spectral_info["name"].append(name)
 
                 for edges in instrument_spectral_info["spectral_energy_ranges"]:
                     self.instrument_spectral_info["spectral_energy_ranges"].append(edges)
 
+        self.datasets, self.final_model = set_models(
+            self.config.target,
+            self.datasets,
+            self.dataset_name_list,
+            models=self.final_model,
+        )
+
+        # Evaluate the total degree of freedom for the model fitting to the data
+        en_bins = 0
+        for data in self.datasets:
+            if data.mask:
+                en_bins += data.mask.geom.axes["energy"].nbin
             else:
-                # Running DL5 functions on a given Datasets object.
-                if step == "fit":
-                    # Confirming the Final Models object for all the datasets
-                    # for the Fit function.
-
-                    # In case of only 1D dataset being selected, Model is read
-                    # from the config information, by passing None as value.
-                    # It should be reinitialized again with the DatasetModels.
-                    if len(self.final_model) == 0:
-                        self.final_model = None
-                    # Apply selection filter for the ROI if more than 1 models
-                    # are provided in the FoV, that are not the background models.
-                    elif len(self.final_model) > 1:
-                        self.final_model = apply_selection_mask_to_models(
-                            list_sources=self.final_model,
-                            target_source=self.config.target.source_name,
-                            roi_radius=self.config.target.roi_selection.roi_radius,
-                            free_sources=self.config.target.roi_selection.free_sources,
-                        )
+                en_bins += data.counts.geom.axes["energy"].nbin
+
+        dof = en_bins + len(list(self.final_model.parameters.free_parameters))
+        self.instrument_spectral_info["DoF"] = dof
 
-                    self.datasets = set_models(
-                        self.config.target,
-                        self.datasets,
-                        self.dataset_name_list,
-                        models=self.final_model,
-                        target_source_name=self.config.target.source_name,
-                    )
-                    if self.final_model is None:
-                        self.final_model = self.datasets.models
+        if len(dl4_dl5_steps) > 0:
+            self.log.info("Perform DL4 to DL5 processes!")
 
+            for step in dl4_dl5_steps:
                 analysis_step = AnalysisStep.create(step, self.config, **kwargs)
+
                 analysis_step.run(
                     datasets=self.datasets, instrument_spectral_info=self.instrument_spectral_info
                 )
 
                 # Update the final data product objects
                 for data_product in self.final_data_products:
                     if hasattr(analysis_step, data_product):
@@ -183,8 +172,9 @@
         self.run(steps=["fit"])
 
     def get_flux_points(self):
         """Calculate flux points for a specific model component."""
         self.run(steps=["flux-points"])
 
     def update_config(self, config):
+        """Update the primary config with another config."""
         self.config = self.config.update(config=config)
```

### Comparing `asgardpy-0.3.4/asgardpy/base/base.py` & `asgardpy-0.3.5/asgardpy/base/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -82,48 +82,61 @@
             if path_.exists():
                 return Path(v)
             else:
                 raise ValueError(f"Path {v} does not exist")
 
 
 class FrameEnum(str, Enum):
+    """Config section for list of frames on creating a SkyCoord object."""
+
     icrs = "icrs"
     galactic = "galactic"
 
 
 class TimeFormatEnum(str, Enum):
+    """Config section for list of formats for creating a Time object."""
+
     datetime = "datetime"
     fits = "fits"
     iso = "iso"
     isot = "isot"
     jd = "jd"
     mjd = "mjd"
     unix = "unix"
 
 
 class BaseConfig(BaseModel):
+    """
+    Base Config class for creating other Config sections with specific encoders.
+    """
+
     class Config:
         validate_all = True
         validate_assignment = True
         extra = "forbid"
         json_encoders = {
             Angle: lambda v: f"{v.value} {v.unit}",
             u.Quantity: lambda v: f"{v.value} {v.unit}",
             Time: lambda v: f"{v.value}",
             Path: lambda v: Path(v),
         }
 
 
 class AnalysisStepBase(abc.ABC):
+    """Config section for creating a basic AsgardpyAnalysis Step."""
+
     tag = "analysis-step"
 
     def __init__(self, config, log=None, overwrite=True):
         self.config = config
         self.overwrite = overwrite
 
+        self.datasets = None
+        self.instrument_spectral_info = None
+
         if log is None:
             log = logging.getLogger(__name__)
             self.log = log
 
     def run(self, datasets=None, instrument_spectral_info=None):
         """
         One can provide datasets and instrument_spectral_info to be used,
@@ -152,27 +165,44 @@
         from asgardpy.data import ANALYSIS_STEP_REGISTRY
 
         cls = ANALYSIS_STEP_REGISTRY.get_cls(tag)
         return cls(config, **kwargs)
 
 
 class AnalysisStepEnum(str, Enum):
+    """Config section for list of Analysis Steps."""
+
     datasets_1d = "datasets-1d"
     datasets_3d = "datasets-3d"
     fit = "fit"
     flux_points = "flux-points"
 
 
 # Basic Quantity ranges Type for building the Config
 class TimeRangeConfig(BaseConfig):
+    """
+    Config section for getting a time range information for creating a Time
+    object.
+    """
+
     start: TimeType = Time("0", format="mjd")
     stop: TimeType = Time("0", format="mjd")
 
 
 class TimeIntervalsConfig(BaseConfig):
+    """
+    Config section for getting main information for creating a Time Intervals
+    object.
+    """
+
     format: TimeFormatEnum = TimeFormatEnum.iso
     intervals: List[TimeRangeConfig] = [TimeRangeConfig()]
 
 
 class EnergyRangeConfig(BaseConfig):
+    """
+    Config section for getting a energy range information for creating an
+    Energy type Quantity object.
+    """
+
     min: EnergyType = 1 * u.GeV
     max: EnergyType = 1 * u.TeV
```

### Comparing `asgardpy-0.3.4/asgardpy/config/generator.py` & `asgardpy-0.3.5/asgardpy/config/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,33 @@
 CONFIG_PATH = Path(__file__).resolve().parent
 
 log = logging.getLogger(__name__)
 
 
 # Other general config params
 class LogConfig(BaseConfig):
+    """Config section for main logging information."""
+
     level: str = "info"
     filename: str = ""
     filemode: str = "w"
     format: str = ""
     datefmt: str = ""
 
 
 class ParallelBackendEnum(str, Enum):
+    """Config section for list of parallel processing backend methods."""
+
     multi = "multiprocessing"
     ray = "ray"
 
 
 class GeneralConfig(BaseConfig):
+    """Config section for general information for running AsgardpyAnalysis."""
+
     log: LogConfig = LogConfig()
     outdir: PathType = PathType(".")
     n_jobs: int = 1
     parallel_backend: ParallelBackendEnum = ParallelBackendEnum.multi
     steps: List[AnalysisStepEnum] = []
     overwrite: bool = True
     stacked_dataset: bool = False
```

### Comparing `asgardpy-0.3.4/asgardpy/data/__init__.py` & `asgardpy-0.3.5/asgardpy/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     apply_selection_mask_to_models,
     check_model_preference_aic,
     check_model_preference_lrt,
     config_to_dict,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
+    get_chi2_pval,
     set_models,
     xml_spatial_model_to_gammapy,
     xml_spectral_model_to_gammapy_params,
 )
 
 ANALYSIS_STEP_REGISTRY = Registry(
     [
@@ -38,33 +39,32 @@
         Datasets3DAnalysisStep,
         FitAnalysisStep,
         FluxPointsAnalysisStep,
     ]
 )
 
 __all__ = [
-    "Target",
     "BrokenPowerLaw2SpectralModel",
-    "ExpCutoffLogParabolaSpectralModel",
-    "set_models",
-    "apply_selection_mask_to_models",
-    "config_to_dict",
-    "xml_spectral_model_to_gammapy_params",
-    "xml_spatial_model_to_gammapy",
-    "check_model_preference_aic",
-    "check_model_preference_lrt",
-    "create_source_skymodel",
-    "create_iso_diffuse_skymodel",
-    "create_gal_diffuse_skymodel",
-    "SpatialCircleConfig",
-    "SpatialPointConfig",
     "Dataset1DConfig",
     "Dataset1DGeneration",
-    "Datasets1DAnalysisStep",
     "Dataset3DConfig",
     "Dataset3DGeneration",
+    "Datasets1DAnalysisStep",
     "Datasets3DAnalysisStep",
-    "FluxPointsConfig",
-    "FitConfig",
+    "ExpCutoffLogParabolaSpectralModel",
     "FitAnalysisStep",
+    "FitConfig",
     "FluxPointsAnalysisStep",
+    "FluxPointsConfig",
+    "Target",
+    "apply_selection_mask_to_models",
+    "check_model_preference_aic",
+    "check_model_preference_lrt",
+    "config_to_dict",
+    "create_gal_diffuse_skymodel",
+    "create_iso_diffuse_skymodel",
+    "create_source_skymodel",
+    "get_chi2_pval",
+    "set_models",
+    "xml_spatial_model_to_gammapy",
+    "xml_spectral_model_to_gammapy_params",
 ]
```

### Comparing `asgardpy-0.3.4/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.5/asgardpy/data/dataset_3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 """
 Main classes to define 3D Dataset Config, 3D Dataset Analysis Step and
 to generate 3D Datasets from given Instruments' DL3 data from the config.
 """
 
 import logging
-import re
 from typing import List
 
 import numpy as np
 import xmltodict
 from astropy import units as u
-from astropy.coordinates import SkyCoord
 from astropy.io import fits
 
 # from gammapy.analysis import Analysis, AnalysisConfig - no support for DL3 with RAD_MAX
+from gammapy.catalog import CATALOG_REGISTRY
 from gammapy.data import GTI, EventList
 from gammapy.datasets import Datasets, MapDataset
 from gammapy.irf import EDispKernel, EDispKernelMap, PSFMap
 from gammapy.makers import MapDatasetMaker
 from gammapy.maps import Map, MapAxis
 from gammapy.modeling.models import (
     Models,
     PowerLawNormSpectralModel,
     SkyModel,
     TemplateSpatialModel,
 )
-from regions import CircleAnnulusSkyRegion, CircleSkyRegion
 
 from asgardpy.base import (
     AnalysisStepBase,
     BackgroundConfig,
     BaseConfig,
     GeomConfig,
     MapAxesConfig,
     MapSelectionEnum,
+    ObservationsConfig,
     ReductionTypeEnum,
     SafeMaskConfig,
     SkyPositionConfig,
     get_energy_axis,
 )
+from asgardpy.base.geom import create_counts_map, generate_geom, get_source_position
+from asgardpy.base.reduction import (
+    generate_dl4_dataset,
+    get_bkg_maker,
+    get_dataset_maker,
+    get_dataset_reference,
+    get_exclusion_region_mask,
+    get_filtered_observations,
+    get_safe_mask_maker,
+)
 from asgardpy.data.target import (
     apply_selection_mask_to_models,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
+    read_models_from_asgardpy_config,
 )
 from asgardpy.io import DL3Files, InputConfig
 
 __all__ = [
     "Datasets3DAnalysisStep",
     "Dataset3DBaseConfig",
     "Dataset3DConfig",
@@ -56,32 +66,41 @@
 ]
 
 log = logging.getLogger(__name__)
 
 
 # Defining various components of 3D Dataset Config section
 class Dataset3DInfoConfig(BaseConfig):
+    """Config section for 3D DL3 Dataset Reduction for each instrument."""
+
     name: str = "dataset-name"
     key: List = []
+    observation: ObservationsConfig = ObservationsConfig()
     map_selection: List[MapSelectionEnum] = MapDatasetMaker.available_selection
     geom: GeomConfig = GeomConfig()
     background: BackgroundConfig = BackgroundConfig()
     safe_mask: SafeMaskConfig = SafeMaskConfig()
     on_region: SkyPositionConfig = SkyPositionConfig()
     containment_correction: bool = True
     spectral_energy_range: MapAxesConfig = MapAxesConfig()
 
 
 class Dataset3DBaseConfig(BaseConfig):
+    """
+    Config section for 3D DL3 Dataset base information for each instrument.
+    """
+
     name: str = "Instrument-name"
     io: List[InputConfig] = [InputConfig()]
     dataset_info: Dataset3DInfoConfig = Dataset3DInfoConfig()
 
 
 class Dataset3DConfig(BaseConfig):
+    """Config section for a list of all 3D DL3 Datasets information."""
+
     type: ReductionTypeEnum = ReductionTypeEnum.cube
     instruments: List[Dataset3DBaseConfig] = [Dataset3DBaseConfig()]
 
 
 # The main Analysis Step
 class Datasets3DAnalysisStep(AnalysisStepBase):
     """
@@ -119,38 +138,42 @@
             # Retrieving a single dataset for each instrument.
             for key in key_names:
                 generate_3d_dataset = Dataset3DGeneration(self.log, config_3d_dataset, self.config)
                 dataset, models = generate_3d_dataset.run(key)
 
                 # Assigning datasets_names and including them in the final
                 # model list
-                for model_ in models:
-                    if key:
-                        model_.datasets_names = [f"{config_3d_dataset.name}_{key}"]
-                    else:
-                        model_.datasets_names = [f"{config_3d_dataset.name}"]
-
-                    if model_.name in models_final.names:
-                        models_final[model_.name].datasets_names.append(model_.datasets_names[0])
-                    else:
-                        models_final.append(model_)
+
+                # When no associated list of models are provided, look for a
+                # separate model for target and an entry of catalog to fill in.
+                if len(models) > 0:
+                    for model_ in models:
+                        model_.datasets_names = [dataset.name]
+
+                        if model_.name in models_final.names:
+                            models_final[model_.name].datasets_names.append(dataset.name)
+                        else:
+                            models_final.append(model_)
 
                 dataset_instrument.append(dataset)
 
-            # Linking the spectral model of the diffuse model for each key
-            diffuse_models_names = []
-            for model_name in models_final.names:
-                if "diffuse-iso" in model_name:
-                    diffuse_models_names.append(model_name)
-
-            if len(diffuse_models_names) > 1:
-                for model_name in diffuse_models_names[1:]:
-                    models_final[diffuse_models_names[0]].spectral_model.model2 = models_final[
-                        model_name
-                    ].spectral_model.model2
+            if len(models_final) > 0:
+                # Linking the spectral model of the diffuse model for each key
+                diffuse_models_names = []
+                for model_name in models_final.names:
+                    if "diffuse-iso" in model_name:
+                        diffuse_models_names.append(model_name)
+
+                if len(diffuse_models_names) > 1:
+                    for model_name in diffuse_models_names[1:]:
+                        models_final[diffuse_models_names[0]].spectral_model.model2 = models_final[
+                            model_name
+                        ].spectral_model.model2
+            else:
+                models_final = None
 
             # Get the spectral energy information for each Instrument Dataset
             energy_axes = config_3d_dataset.dataset_info.spectral_energy_range
             if len(energy_axes.axis_custom.edges) > 0:
                 energy_bin_edges = get_energy_axis(energy_axes, only_edges=True, custom_range=True)
             else:
                 energy_bin_edges = get_energy_axis(
@@ -203,55 +226,164 @@
         self.config_full = config_full
         self.config_target = config_full.target
 
     def run(self, key_name):
         # First check for the given file list if they are readable or not.
         file_list = self.read_to_objects(key_name)
 
-        # Start preparing objects to create the counts map
-        self.set_energy_dispersion_matrix()
         self.load_events(file_list["events_file"])
+        exclusion_regions = []
+
+        if self.config_3d_dataset.io[0].type == "gadf-dl3":
+            observations = get_filtered_observations(
+                dl3_path=self.config_3d_dataset.io[0].input_dir,
+                obs_config=self.config_3d_dataset.dataset_info.observation,
+                log=self.log,
+            )
+            center_pos = get_source_position(config_target=self.config_target)
+            geom = generate_geom(
+                tag="3d",
+                geom_config=self.config_3d_dataset.dataset_info.geom,
+                center_pos=center_pos,
+            )
+            dataset_reference = get_dataset_reference(
+                tag="3d", geom=geom, geom_config=self.config_3d_dataset.dataset_info.geom
+            )
+
+            dataset_maker = get_dataset_maker(
+                tag="3d",
+                dataset_config=self.config_3d_dataset.dataset_info,
+            )
+
+            safe_maker = get_safe_mask_maker(
+                safe_config=self.config_3d_dataset.dataset_info.safe_mask
+            )
 
-        source_pos, evts_radius = self.get_source_skycoord()
+            # If there is no explicit list of models provided for the 3D data,
+            # one can use one of the several catalogs available in Gammapy.
+            # Reading them as Models will keep the procedure uniform.
+            if len(self.list_sources) == 0:
+                # Read the SkyModel info from AsgardpyConfig.target section
+                if len(self.config_target.components) > 0:
+                    spectral_model, spatial_model = read_models_from_asgardpy_config(
+                        self.config_target
+                    )
+                    self.list_sources.append(
+                        Models(
+                            SkyModel(
+                                spectral_model=spectral_model,
+                                spatial_model=spatial_model,
+                                name=self.config_target.source_name,
+                            )
+                        )
+                    )
 
-        # Create the Counts Map
-        self.create_counts_map(source_pos, evts_radius)
+                # If a catalog information is provided, use it to build up the list of models
+                # Check if a catalog data is given with selection radius
+                if self.config_target.use_catalog.selection_radius != 0 * u.deg:
+                    catalog = CATALOG_REGISTRY.get_cls(self.config_target.use_catalog.name)()
+
+                    # One can also provide a separate file, but one has to add
+                    # another config option for reading Catalog file paths.
+                    base_geom = self.events["counts_map"].geom.copy()
+                    inside_geom = base_geom.to_image().contains(catalog.positions)
+
+                    idx_list = np.nonzero(inside_geom)[0]
+                    for i in idx_list:
+                        self.list_sources.append(catalog[i].sky_model())
+
+            exclusion_mask = get_exclusion_region_mask(
+                exclusion_params=self.config_3d_dataset.dataset_info.background.exclusion,
+                exclusion_regions=exclusion_regions,
+                excluded_geom=None,
+                config_target=self.config_target,
+                geom_config=self.config_3d_dataset.dataset_info.geom,
+                log=self.log,
+            )
 
-        # Create any dataset reduction makers or mask
-        self.generate_diffuse_background_cutout()
+            bkg_maker = get_bkg_maker(
+                bkg_config=self.config_3d_dataset.dataset_info.background,
+                exclusion_mask=exclusion_mask,
+            )
 
-        self.set_edisp_interpolator()
-        self.set_exposure_interpolator()
+            dataset = generate_dl4_dataset(
+                tag="3d",
+                observations=observations,
+                dataset_reference=dataset_reference,
+                dataset_maker=dataset_maker,
+                bkg_maker=bkg_maker,
+                safe_maker=safe_maker,
+                n_jobs=self.config_full.general.n_jobs,
+                parallel_backend=self.config_full.general.parallel_backend,
+            )
 
-        self.create_exclusion_mask()
+        elif "lat" in self.config_3d_dataset.io[0].type:
+            # Start preparing objects to create the counts map
+            self.set_energy_dispersion_matrix()
+
+            center_pos = get_source_position(
+                config_target=self.config_target,
+                fits_header=self.events["event_fits"][1].header,
+            )
 
-        # Apply the same exclusion mask to the list of source models as applied
-        # to the Counts Map
-        self.list_sources = apply_selection_mask_to_models(
-            self.list_sources,
-            target_source=self.config_target.source_name,
-            selection_mask=self.exclusion_mask,
-        )
+            # Create the Counts Map
+            self.events["counts_map"] = create_counts_map(
+                geom_config=self.config_3d_dataset.dataset_info.geom,
+                center_pos=center_pos,
+            )
+            self.events["counts_map"].fill_by_coord(
+                {
+                    "skycoord": self.events["events"].radec,
+                    "energy": self.events["events"].energy,
+                    "time": self.events["events"].time,
+                }
+            )
+            # Create any dataset reduction makers or mask
+            self.generate_diffuse_background_cutout()
+
+            self.set_edisp_interpolator()
+            self.set_exposure_interpolator()
+
+            self.exclusion_mask = get_exclusion_region_mask(
+                exclusion_params=self.config_3d_dataset.dataset_info.background.exclusion,
+                excluded_geom=self.events["counts_map"].geom.copy(),
+                exclusion_regions=exclusion_regions,
+                config_target=self.config_target,
+                geom_config=self.config_3d_dataset.dataset_info.geom,
+                log=self.log,
+            )
+
+            # Generate the final dataset
+            dataset = self.generate_dataset(key_name)
 
-        # Generate the final dataset
-        dataset = self.generate_dataset(key_name)
+        if len(self.list_sources) != 0:
+            # Apply the same exclusion mask to the list of source models as applied
+            # to the Counts Map
+            self.list_sources = apply_selection_mask_to_models(
+                self.list_sources,
+                target_source=self.config_target.source_name,
+                selection_mask=self.exclusion_mask,
+            )
 
         return dataset, self.list_sources
 
     def read_to_objects(self, key_name):
         """
         For each key type of files, read the files to get the required
         Gammapy objects for further analyses.
         """
         file_list = {}
 
         # Read the first IO list for events, IRFs and XML files
 
         # Get the Diffuse models files list
         for io_ in self.config_3d_dataset.io:
+            if io_.type in ["gadf-dl3"]:
+                file_list, _ = self.get_base_objects(io_, key_name, file_list)
+
             if io_.type in ["lat"]:
                 file_list, [
                     self.irfs["exposure"],
                     self.irfs["psf"],
                     self.irfs["edisp"],
                 ] = self.get_base_objects(io_, key_name, file_list)
                 self.update_source_pos_from_3d_dataset()
@@ -305,30 +437,36 @@
         For a DL3 files type and tag of the 'mode of observations' or key
         (FRONT/00 and BACK/01 for Fermi-LAT in enrico/fermipy files),
         read the files to appropriate Object type for further analysis.
 
         If there are no distinct key types of files, the value is None.
         """
         dl3_info = DL3Files(dl3_dir_dict, file_list, log=self.log)
-        file_list = dl3_info.prepare_lat_files(key, file_list)
         object_list = []
 
-        if dl3_dir_dict.type.lower() in ["lat"]:
-            exposure = Map.read(file_list["expmap_file"])
-            psf = PSFMap.read(file_list["psf_file"], format="gtpsf")
-            drmap = fits.open(file_list["edrm_file"])
-            object_list = [exposure, psf, drmap]
-
-        if dl3_dir_dict.type.lower() in ["lat-aux"]:
-            diff_gal = Map.read(file_list["gal_diff_file"])
-            diff_gal.meta["filename"] = file_list["gal_diff_file"]
-            diff_iso = create_iso_diffuse_skymodel(file_list["iso_diff_file"], key)
-            object_list = [diff_gal, diff_iso]
+        if dl3_dir_dict.type.lower() in ["gadf-dl3"]:
+            file_list = dl3_info.list_dl3_files()
 
-        return file_list, object_list
+            return file_list, object_list
+        else:
+            file_list = dl3_info.prepare_lat_files(key, file_list)
+
+            if dl3_dir_dict.type.lower() in ["lat"]:
+                exposure = Map.read(file_list["expmap_file"])
+                psf = PSFMap.read(file_list["psf_file"], format="gtpsf")
+                drmap = fits.open(file_list["edrm_file"])
+                object_list = [exposure, psf, drmap]
+
+            if dl3_dir_dict.type.lower() in ["lat-aux"]:
+                diff_gal = Map.read(file_list["gal_diff_file"])
+                diff_gal.meta["filename"] = file_list["gal_diff_file"]
+                diff_iso = create_iso_diffuse_skymodel(file_list["iso_diff_file"], key)
+                object_list = [diff_gal, diff_iso]
+
+            return file_list, object_list
 
     def get_list_objects(self, aux_path, xml_file):
         """
         Read from the XML file to enlist the various objects and get their
         SkyModels
 
         Currently assuming this to be applicable only for Fermi-LAT data.
@@ -411,100 +549,31 @@
         Loading the events files for the specific "Key" into an EventList
         object and the GTI information into a GTI object.
         """
         self.events["event_fits"] = fits.open(events_file)
         self.events["events"] = EventList.read(events_file)
         self.events["gti"] = GTI.read(events_file)
 
-    def get_source_skycoord(self):
-        """
-        Get the source skycoord and the ROI radius from the events file.
-
-        Needs to be generalized for other possible file structures for other
-        instruments.
-        """
-        try:
-            dsval2 = self.events["event_fits"][1].header["DSVAL2"]
-            list_str_check = re.findall(r"[-+]?\d*\.\d+|\d+", dsval2)
-            ra_pos, dec_pos, evts_radius = [float(k) for k in list_str_check]
-        except IndexError:
-            history = str(self.events["event_fits"][1].header["HISTORY"])
-            str_ = history.split("angsep(RA,DEC,")[1]
-            list_str_check = re.findall(r"[-+]?\d*\.\d+|\d+", str_)[:3]
-            ra_pos, dec_pos, evts_radius = [float(k) for k in list_str_check]
-
-        source_pos = SkyCoord(ra_pos, dec_pos, unit="deg", frame="fk5")
-
-        return source_pos, evts_radius
-
-    def create_counts_map(self, source_pos, evts_radius):
-        """
-        Generate the counts Map object using the information provided in the
-        geom section of the Config and fill it with the events' RA-Dec
-        position, Energy and Time information.
-        """
-        geom_config = self.config_3d_dataset.dataset_info.geom
-
-        energy_axes = geom_config.axes[0]
-        energy_axis = get_energy_axis(energy_axes)
-        bin_size = geom_config.wcs.binsize.to_value(u.deg)
-
-        if geom_config.from_events_file:
-            self.events["counts_map"] = Map.create(
-                skydir=source_pos.galactic,
-                binsz=bin_size,
-                npix=(
-                    int(evts_radius * 2 / bin_size),
-                    int(evts_radius * 2 / bin_size),
-                ),  # Using the limits from the events fits file
-                proj=geom_config.wcs.proj,
-                frame="galactic",
-                axes=[energy_axis],
-                dtype=float,
-            )
-        else:
-            width_ = geom_config.wcs.map_frame_shape.width.to_value(u.deg)
-            width_in_pixel = int(width_ / bin_size)
-            height_ = geom_config.wcs.map_frame_shape.height.to_value(u.deg)
-            height_in_pixel = int(height_ / bin_size)
-
-            self.events["counts_map"] = Map.create(
-                skydir=source_pos.galactic,
-                binsz=bin_size,
-                npix=(width_in_pixel, height_in_pixel),
-                proj=geom_config.wcs.proj,
-                frame="galactic",
-                axes=[energy_axis],
-                dtype=float,
-            )
-        self.events["counts_map"].fill_by_coord(
-            {
-                "skycoord": self.events["events"].radec,
-                "energy": self.events["events"].energy,
-                "time": self.events["events"].time,
-            }
-        )
-
     def generate_diffuse_background_cutout(self):
         """
         Perform a cutout of the Diffuse background model with respect to the
         counts map geom (may improve fitting speed?) and update the main list
         of models.
 
-        The Template Spatial Model is without normalization currently.
+        The reference Spatial Model is without normalization currently.
         """
         diffuse_cutout = self.diffuse_models["gal_diffuse"].cutout(
             self.events["counts_map"].geom.center_skydir, self.events["counts_map"].geom.width[0]
         )
 
-        template_diffuse = TemplateSpatialModel(diffuse_cutout, normalize=False)
+        reference_diffuse = TemplateSpatialModel(diffuse_cutout, normalize=False)
 
         self.diffuse_models["gal_diffuse_cutout"] = SkyModel(
             spectral_model=PowerLawNormSpectralModel(),
-            spatial_model=template_diffuse,
+            spatial_model=reference_diffuse,
             name="diffuse-iem",
         )
         self.diffuse_models["gal_diffuse_cutout"].parameters["norm"].min = 0
         self.diffuse_models["gal_diffuse_cutout"].parameters["norm"].max = 10
         self.diffuse_models["gal_diffuse_cutout"].parameters["norm"].frozen = False
 
         # Update the model in self.list_sources
@@ -537,85 +606,14 @@
         """
         Set Exposure interpolated along energy axis of real counts.
         """
         self.irfs["exposure_interp"] = self.irfs["exposure"].interp_to_geom(
             self.events["counts_map"].geom.as_energy_true
         )
 
-    def create_exclusion_mask(self):
-        """
-        Generate an Exclusion Mask for the final MapDataset and also select
-        the region for the list of Models using the excluded regions.
-        """
-        exclusion_regions = []
-        excluded_geom = self.events["counts_map"].geom.copy()
-        exclusion_params = self.config_3d_dataset.dataset_info.background.exclusion
-
-        if len(exclusion_params.regions) != 0:
-            for region in exclusion_params.regions:
-                if region.name == "None":
-                    coord = region.position
-                    center_ex = SkyCoord(
-                        u.Quantity(coord.lon), u.Quantity(coord.lat), frame=coord.frame
-                    ).icrs
-                else:
-                    center_ex = SkyCoord.from_name(region.name)
-
-                if region.type == "CircleAnnulusSkyRegion":
-                    excluded_region = CircleAnnulusSkyRegion(
-                        center=center_ex,
-                        inner_radius=u.Quantity(region.parameters["rad_0"]),
-                        outer_radius=u.Quantity(region.parameters["rad_1"]),
-                    )
-                elif region.type == "CircleSkyRegion":
-                    excluded_region = CircleSkyRegion(
-                        center=center_ex, radius=u.Quantity(region.parameters["region_radius"])
-                    )
-                else:
-                    self.log.error(f"Unknown type of region passed {region.type}")
-                exclusion_regions.append(excluded_region)
-            self.exclusion_mask = ~excluded_geom.region_mask(exclusion_regions)
-
-        elif len(exclusion_regions) == 0:
-            self.log.info("Creating empty/dummy exclusion region")
-            pos = SkyCoord(0, 90, unit="deg")
-            exclusion_region = CircleSkyRegion(pos, 0.00001 * u.deg)
-
-            exclusion_regions.append(exclusion_region)
-            self.exclusion_mask = ~excluded_geom.region_mask(exclusion_regions)
-        else:
-            self.log.info("Creating exclusion region")
-            self.exclusion_mask = ~excluded_geom.region_mask(exclusion_regions)
-
-    def add_source_to_exclusion_region(
-        self, exclusion_regions, source_pos=None, radius=0.1 * u.deg
-    ):
-        """
-        Add to an existing exclusion_regions list, the source region.
-
-        Check if this function is necessary.
-        """
-        if source_pos is not None:
-            exclusion_region = CircleSkyRegion(
-                center=source_pos.galactic,
-                radius=radius,
-            )
-        else:
-            sky_pos = self.config_target.sky_position
-            source_pos = SkyCoord(
-                u.Quantity(sky_pos.lon), u.Quantity(sky_pos.lat), frame=sky_pos.frame
-            )
-            exclusion_region = CircleSkyRegion(
-                center=source_pos.galactic,
-                radius=radius,
-            )
-        exclusion_regions.append(exclusion_region)
-
-        return exclusion_regions
-
     def generate_dataset(self, key_name):
         """
         Generate MapDataset for the given Instrument files using the Counts Map,
         and IRFs objects.
         """
         try:
             mask_safe = self.exclusion_mask
```

### Comparing `asgardpy-0.3.4/asgardpy/data/dl4.py` & `asgardpy-0.3.5/asgardpy/data/dl4.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,39 +6,46 @@
 
 from astropy import units as u
 from gammapy.datasets import Datasets
 from gammapy.estimators import FluxPointsEstimator
 from gammapy.modeling import Fit
 
 from asgardpy.base import AnalysisStepBase, BaseConfig, EnergyRangeConfig
+from asgardpy.data.target import get_chi2_pval
 
 __all__ = [
     "FitAnalysisStep",
     "FitConfig",
     "FluxPointsAnalysisStep",
     "FluxPointsConfig",
 ]
 
 
 # Defining various components of High-level Analysis Config
 class BackendEnum(str, Enum):
+    """Config section for a list Fitting backend methods."""
+
     minuit = "minuit"
     scipy = "scipy"
 
 
 class FitConfig(BaseConfig):
+    """Config section for parameters to use for Fit function."""
+
     fit_range: EnergyRangeConfig = EnergyRangeConfig()
     backend: BackendEnum = BackendEnum.minuit
     optimize_opts: dict = {}
     covariance_opts: dict = {}
     confidence_opts: dict = {}
     store_trace: bool = True
 
 
 class FluxPointsConfig(BaseConfig):
+    """Config section for parameters to use for FluxPointsEstimator function."""
+
     parameters: dict = {"selection_optional": "all"}
     reoptimize: bool = False
 
 
 # The main Analysis Steps
 class FitAnalysisStep(AnalysisStepBase):
     """
@@ -51,15 +58,29 @@
     def _run(self):
         self.fit_params = self.config.fit_params
 
         self._setup_fit()
         final_dataset = self._set_datasets()
         self.fit_result = self.fit.run(datasets=final_dataset)
 
+        self.instrument_spectral_info["total_stat"] = self.fit_result.total_stat
+
+        chi2_, pval_ = get_chi2_pval(
+            self.instrument_spectral_info["total_stat"], self.instrument_spectral_info["DoF"]
+        )
+        self.instrument_spectral_info["chi2"] = chi2_
+        self.instrument_spectral_info["p-value"] = pval_
+
+        stat_message = (
+            f'The Chi2/dof value of the Fit is {chi2_:.2f}/{self.instrument_spectral_info["DoF"]}'
+        )
+        stat_message += f"\nand the p-value is {pval_:.3e}"
+
         self.log.info(self.fit_result)
+        self.log.info(stat_message)
 
     def _setup_fit(self):
         """
         Setup the Gammapy Fit function with all the provided parameters from
         the config.
         """
         self.fit = Fit(
@@ -97,34 +118,34 @@
     tag = "flux-points"
 
     def _run(self):
         self.flux_points = []
         datasets, energy_edges = self._sort_datasets_info()
 
         for dataset, energy_edges in zip(datasets, energy_edges):
-            self._set_fpe(dataset, energy_edges)
+            self._set_fpe(energy_edges)
             flux_points = self.fpe.run(datasets=dataset)
             flux_points.name = dataset.names
 
             self.flux_points.append(flux_points)
 
-    def _set_fpe(self, dataset, energy_bin_edges):
+    def _set_fpe(self, energy_bin_edges):
         """
         Setup the Gammapy FluxPointsEstimator function with all the
         provided parameters.
         """
         fpe_settings = self.config.flux_points_params.parameters
 
         self.fpe = FluxPointsEstimator(
             energy_edges=energy_bin_edges,
             source=self.config.target.source_name,
             n_jobs=self.config.general.n_jobs,
             parallel_backend=self.config.general.parallel_backend,
             reoptimize=self.config.flux_points_params.reoptimize,
-            **fpe_settings
+            **fpe_settings,
         )
 
     def _sort_datasets_info(self):
         """
         The given list of datasets may contain sub-instrument level datasets.
         With the help of the dict information for instrument specific name and
         spectral energy edges, this function, sorts the datasets and returns
```

### Comparing `asgardpy-0.3.4/asgardpy/data/target.py` & `asgardpy-0.3.5/asgardpy/data/target.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from gammapy.maps import Map
 from gammapy.modeling import Parameter, Parameters
 from gammapy.modeling.models import (
     SPATIAL_MODEL_REGISTRY,
     SPECTRAL_MODEL_REGISTRY,
     DatasetModels,
     EBLAbsorptionNormSpectralModel,
+    FoVBackgroundModel,
     Models,
     SkyModel,
     SpectralModel,
     create_fermi_isotropic_diffuse_model,
 )
 from scipy.stats import chi2, norm
 
@@ -35,82 +36,120 @@
     "apply_selection_mask_to_models",
     "check_model_preference_aic",
     "check_model_preference_lrt",
     "config_to_dict",
     "create_gal_diffuse_skymodel",
     "create_iso_diffuse_skymodel",
     "create_source_skymodel",
+    "get_chi2_pval",
     "params_renaming_to_gammapy",
     "params_rescale_to_gammapy",
     "read_models_from_asgardpy_config",
     "set_models",
     "xml_spatial_model_to_gammapy",
     "xml_spectral_model_to_gammapy_params",
 ]
 
 
 # Basic components to define the Target Config and any Models Config
 class EBLAbsorptionModel(BaseConfig):
+    """
+    Config section for parameters to use for EBLAbsorptionNormSpectralModel.
+    """
+
     filename: PathType = PathType(".")
     reference: str = "dominguez"
     type: str = "EBLAbsorptionNormSpectralModel"
     redshift: float = 0.4
     alpha_norm: float = 1.0
 
 
 class ModelParams(BaseConfig):
+    """Config section for parameters to use for a basic Parameter object."""
+
     name: str = ""
     value: float = 1
     unit: str = " "
     error: float = 0.1
     min: float = 0.1
     max: float = 10
     frozen: bool = True
 
 
 class SpectralModelConfig(BaseConfig):
+    """
+    Config section for parameters to use for creating a SpectralModel object.
+    """
+
     type: str = ""
     parameters: List[ModelParams] = [ModelParams()]
     ebl_abs: EBLAbsorptionModel = EBLAbsorptionModel()
 
 
 class SpatialModelConfig(BaseConfig):
+    """
+    Config section for parameters to use for creating a SpatialModel object.
+    """
+
     type: str = ""
     parameters: List[ModelParams] = [ModelParams()]
 
 
 class SkyModelComponent(BaseConfig):
+    """Config section for parameters to use for creating a SkyModel object."""
+
     name: str = ""
     type: str = "SkyModel"
     spectral: SpectralModelConfig = SpectralModelConfig()
     spatial: SpatialModelConfig = SpatialModelConfig()
 
 
 class RoISelectionConfig(BaseConfig):
+    """
+    Config section for parameters to perform some selection on FoV source
+    models.
+    """
+
     roi_radius: AngleType = 0 * u.deg
     free_sources: List[str] = []
 
 
+class CatalogConfig(BaseConfig):
+    """Config section for parameters to use information from Catalog."""
+
+    name: str = ""
+    selection_radius: AngleType = 0 * u.deg
+    exclusion_radius: AngleType = 0 * u.deg
+
+
 class Target(BaseConfig):
+    """Config section for main information on creating various Models."""
+
     source_name: str = ""
     sky_position: SkyPositionConfig = SkyPositionConfig()
     use_uniform_position: bool = True
     models_file: PathType = PathType(".")
-    extended: bool = False
+    add_fov_bkg_model: bool = False
+    use_catalog: CatalogConfig = CatalogConfig()
     components: List[SkyModelComponent] = [SkyModelComponent()]
     covariance: str = ""
     from_3d: bool = False
     roi_selection: RoISelectionConfig = RoISelectionConfig()
 
 
 class ExpCutoffLogParabolaSpectralModel(SpectralModel):
     r"""Spectral Exponential Cutoff Log Parabola model.
 
     Using a simple template from Gammapy.
 
+    .. math::
+        \phi(E) = \phi_0 \left( \frac{E}{E_0} \right) ^ {
+          - \alpha_1 - \beta \log{ \left( \frac{E}{E_0} \right) }} \cdot
+          \exp(- {(\lambda E})^{\alpha_2})
+
     Parameters
     ----------
     amplitude : `~astropy.units.Quantity`
         :math:`\phi_0`
     reference : `~astropy.units.Quantity`
         :math:`E_0`
     alpha_1 : `~astropy.units.Quantity`
@@ -136,36 +175,42 @@
     alpha_2 = Parameter("alpha_2", 1, frozen=True)
     beta = Parameter("beta", 1)
     lambda_ = Parameter("lambda_", "0.1 TeV-1")
 
     @staticmethod
     def evaluate(energy, amplitude, reference, alpha_1, beta, lambda_, alpha_2):
         """Evaluate the model (static function)."""
-        xx = energy / reference
-        exponent = -alpha_1 - beta * np.log(xx)
+        en_ref = energy / reference
+        exponent = -alpha_1 - beta * np.log(en_ref)
         cutoff = np.exp(-np.power(energy * lambda_, alpha_2))
 
-        return amplitude * np.power(xx, exponent) * cutoff
+        return amplitude * np.power(en_ref, exponent) * cutoff
 
 
 class BrokenPowerLaw2SpectralModel(SpectralModel):
     r"""Spectral broken power-law 2 model.
 
     In this slightly modified Broken Power Law, instead of having the second index
     as a distinct parameter, the difference in the spectral indices around the
     Break Energy is used, to try for some assumptions on the different physical
     processes that define the full spectrum, where the second process is dependent
     on the first process.
 
     For more information see :ref:`broken-powerlaw-spectral-model`.
 
+    .. math::
+        \phi(E) = \phi_0 \cdot \begin{cases}
+                \left( \frac{E}{E_{break}} \right)^{-\Gamma_1} & \text{if } E < E_{break} \\
+                \left( \frac{E}{E_{break}} \right)^{-(\Gamma_1 + \Delta\Gamma)} & \text{otherwise}
+            \end{cases}
+
     Parameters
     ----------
     index1 : `~astropy.units.Quantity`
-        :math:`\Gamma1`
+        :math:`\Gamma_1`
     index_diff : `~astropy.units.Quantity`
         :math:`\Delta\Gamma`
     amplitude : `~astropy.units.Quantity`
         :math:`\phi_0`
     ebreak : `~astropy.units.Quantity`
         :math:`E_{break}`
 
@@ -202,81 +247,92 @@
 
 SPECTRAL_MODEL_REGISTRY.append(ExpCutoffLogParabolaSpectralModel)
 SPECTRAL_MODEL_REGISTRY.append(BrokenPowerLaw2SpectralModel)
 
 
 # Function for Models assignment
 def set_models(
-    config, datasets, datasets_name_list=None, models=None, target_source_name=None, extend=False
+    config_target,
+    datasets,
+    datasets_name_list=None,
+    models=None,
 ):
     """
     Set models on given Datasets.
 
     Parameters
     ----------
-    config: `AsgardpyConfig` or others?
+    config_target: `AsgardpyConfig.target`
         AsgardpyConfig containing target information.
     datasets: `gammapy.datasets.Datasets`
         Datasets object
     dataset_name_list: List
         List of datasets_names to be used on the Models, before assigning them
         to the given datasets.
     models : `~gammapy.modeling.models.Models` or str
         Models object or YAML models string
-    target_source_name: str
-        Name of the Target source, to use to update only that Model's
-        datasets_names, when a list of more than 1 models are provided.
-    extend : bool
-        Extend the existing models on the datasets or replace them with
-        another model, maybe a Background Model. Not worked out currently.
 
     Returns
     -------
     datasets: `gammapy.datasets.Datasets`
         Datasets object with Models assigned.
     """
     # Have some checks on argument types
-    if isinstance(models, DatasetModels) or isinstance(models, list):
+    if isinstance(models, (DatasetModels, list)):
         models = Models(models)
     elif isinstance(models, PathType):
         models = Models.read(models)
-    elif len(config.components) > 0:
-        spectral_model, spatial_model = read_models_from_asgardpy_config(config)
-        models = Models(
-            SkyModel(
-                spectral_model=spectral_model,
-                spatial_model=spatial_model,
-                name=config.source_name,
-            )
-        )
     else:
         raise TypeError(f"Invalid type: {type(models)}")
 
-    # if extend:
-    # For extending a Background Model
-    #    Models(models).extend(self.bkg_models)
+    if len(models) == 0:
+        if len(config_target.components) > 0:
+            spectral_model, spatial_model = read_models_from_asgardpy_config(config_target)
+            models = Models(
+                SkyModel(
+                    spectral_model=spectral_model,
+                    spatial_model=spatial_model,
+                    name=config_target.source_name,
+                )
+            )
+        else:
+            raise Exception("No input for Models provided for the Target source!")
+    else:
+        models = apply_selection_mask_to_models(
+            list_sources=models,
+            target_source=config_target.source_name,
+            roi_radius=config_target.roi_selection.roi_radius,
+            free_sources=config_target.roi_selection.free_sources,
+        )
+
+    if config_target.add_fov_bkg_model:
+        # For extending a Background Model for each 3D dataset
+        bkg_models = []
+
+        for dataset in datasets:
+            if dataset.tag == "MapDataset" and dataset.background_model is None:
+                bkg_models.append(FoVBackgroundModel(dataset_name=dataset.name))
+
+        models.extend(bkg_models)
 
     if datasets_name_list is None:
         datasets_name_list = datasets.names
 
-    if target_source_name is None:
-        target_source_name = config.source_name
-
     if len(models) > 1:
-        models[target_source_name].datasets_names = datasets_name_list
+        models[config_target.source_name].datasets_names = datasets_name_list
     else:
         models.datasets_names = datasets_name_list
 
     datasets.models = models
 
-    return datasets
+    return datasets, models
 
 
 def apply_selection_mask_to_models(
-    list_sources, target_source=None, selection_mask=None, roi_radius=0 * u.deg, free_sources=[None]
+    list_sources, target_source=None, selection_mask=None, roi_radius=0 * u.deg, free_sources=[]
 ):
     """
     For a given list of source models, with a given target source, apply various
     selection masks on the Region of Interest in the sky. This will lead to
     complete exclusion of models or freezing some or all spectral parameters.
     These selections excludes the diffuse background models in the given list.
 
@@ -337,15 +393,15 @@
         for model_ in list_sources_excluded:
             model_pos = model_.spatial_model.position
             separation = target_source_pos.separation(model_pos).deg
             if separation >= roi_radius.deg:
                 model_.spectral_model.freeze()
     else:
         # For a given list of non free sources, unfreeze the spectral amplitude
-        if free_sources[0]:
+        if len(free_sources) > 0:
             for model_ in list_sources_excluded:
                 # Freeze all spectral parameters for other models
                 if model_.name != target_source:
                     model_.spectral_model.freeze()
                 # and now unfreeze the amplitude of selected models
                 if model_.name in free_sources:
                     model_.spectral_model.parameters["amplitude"].frozen = False
@@ -911,73 +967,90 @@
     source.parameters["norm"].min = 0
     source.parameters["norm"].max = 10
     source.parameters["norm"].frozen = False
 
     return source
 
 
-def check_model_preference_lrt(result1, result2, model1, model2):
+def get_chi2_pval(test_stat, ndof):
+    """
+    Using the log-likelihood value for a model fitting to data, along with the
+    total degrees of freedom, evaluate the chi2 value along with the p-value
+    for the fitting statistics.
+
+    In Gammapy, for 3D analysis, cash statistics is used, while for 1D analysis,
+    wstat statistics is used. Check the documentation for more details
+    https://docs.gammapy.org/1.1/user-guide/stats/index.html
+
+    Parameters
+    ----------
+    test_stat: float
+        The test statistic (-2 ln L) value of the fitting.
+    ndof: int
+        Total number of degrees of freedom.
+
+    Returns
+    -------
+    chi2_: float
+        significance (Chi2) of the likelihood of fit model estimated in
+        Gaussian distribution.
+    pval: float
+        p-value for the model fitting
+
+    """
+    pval = chi2.sf(np.sqrt(test_stat), ndof)
+    chi2_ = norm.isf(pval / 2)
+
+    if not np.isfinite(chi2_):
+        chi2_ = np.sqrt(test_stat)
+
+    return chi2_, pval
+
+
+def check_model_preference_lrt(test_stat_1, test_stat_2, ndof_1, ndof_2):
     """
     Log-likelihood ratio test. Checking the preference of a "nested" spectral
     model2 (observed), over a primary model1.
 
     Parameters
     ----------
-    result1: `gammapy.modeling.fit.FitResult`
-        Fit result of the primary spectral model.
-    result2: `gammapy.modeling.fit.FitResult`
-        Fit result of the nested spectral model.
-    model1: `gammapy.modeling.models.spectral.SpectralModel`
-        Primary spectral model
-    model2: `gammapy.modeling.models.spectral.SpectralModel`
-        Nested spectral model
+    test_stat_1: `gammapy.modeling.fit.FitResult.total_stat`
+        The test statistic (-2 ln L) of the Fit result of the primary spectral model.
+    test_stat_2: `gammapy.modeling.fit.FitResult.total_stat`
+        The test statistic (-2 ln L) of the Fit result of the nested spectral model.
+    ndof_1: 'int'
+        Number of energy bins used for spectral fit - number of free spectral parameters for the primary model
+    ndof_2: 'int'
+        Number of energy bins used for spectral fit - number of free spectral parameters for the nested model
 
     Returns
     -------
     p_value: float
         p-value for the ratio of the likelihoods
     gaussian_sigmas: float
         significance (Chi2) of the ratio of the likelihoods estimated in
         Gaussian distribution.
-    chi2_1: float
-        significance (Chi2) of the likelihood of primary fit model estimated in
-        Gaussian distribution.
-    chi2_2: float
-        significance (Chi2) of the likelihood of nested fit model estimated in
-        Gaussian distribution.
     n_dof: int
         number of degrees of freedom or free parameters between primary and
         nested model.
     """
-    Wstat_1 = result1.total_stat
-    Wstat_2 = result2.total_stat
-
-    pval_1 = chi2.sf(Wstat_1, len(list(model1.parameters.free_parameters)))
-    pval_2 = chi2.sf(Wstat_2, len(list(model2.parameters.free_parameters)))
-
-    chi2_1 = norm.isf(pval_1 / 2)
-    chi2_2 = norm.isf(pval_2 / 2)
+    n_dof = ndof_2 - ndof_1
 
-    n_dof = len(list(model2.parameters.free_parameters)) - len(
-        list(model1.parameters.free_parameters)
-    )
     if n_dof < 1:
-        print(
-            f"DoF is lower in {model2.spectral_model.model1.tag[0]} compared "
-            f"to {model1.spectral_model.model1.tag[0]}"
-        )
-        return np.nan, np.nan, chi2_1, chi2_2, n_dof
+        print(f"DoF is lower in {ndof_2} compared to {ndof_1}")
+
+        return np.nan, np.nan, n_dof
 
-    p_value = chi2.sf((Wstat_1 - Wstat_2), n_dof)
+    p_value = chi2.sf((test_stat_1 - test_stat_2), n_dof)
     gaussian_sigmas = norm.isf(p_value / 2)
 
     if not np.isfinite(gaussian_sigmas):
-        gaussian_sigmas = np.sqrt((Wstat_1 - Wstat_2))
+        gaussian_sigmas = np.sqrt((test_stat_1 - test_stat_2))
 
-    return p_value, gaussian_sigmas, chi2_1, chi2_2, n_dof
+    return p_value, gaussian_sigmas, n_dof
 
 
 def check_model_preference_aic(list_wstat, list_dof):
     """
     Akaike Information Criterion (AIC) preference over a list of wstat and DoF
     (degree of freedom) to get relative likelihood of a given list of best-fit
     models.
@@ -987,31 +1060,31 @@
     list_wstat: list
         List of wstat or -2 Log likelihood values for a list of models.
     list_dof: list
         List of degrees of freedom or list of free parameters, for a list of models.
 
     Returns
     -------
-    list_p: list
+    list_rel_p: list
         List of relative likelihood probabilities, for a list of models.
     """
-    list_aic = []
-    for w, d in zip(list_wstat, list_dof):
-        aic = 2 * w + 2 * d
-        list_aic.append(aic)
-    list_aic = np.array(list_aic)
-
-    aic_min = np.min(list_aic)
-
-    list_b = []
-    for a in list_aic:
-        b = np.exp((aic_min - a) / 2)
-        list_b.append(b)
-    list_b = np.array(list_b)
-
-    list_p = []
-    for bb in list_b:
-        bbb = bb / np.sum(list_b)
-        list_p.append(bbb)
-    list_p = np.array(list_p)
+    list_aic_stat = []
+    for wstat, dof in zip(list_wstat, list_dof):
+        aic_stat = wstat + 2 * dof
+        list_aic_stat.append(aic_stat)
+    list_aic_stat = np.array(list_aic_stat)
+
+    aic_stat_min = np.min(list_aic_stat)
+
+    list_b_stat = []
+    for aic in list_aic_stat:
+        b_stat = np.exp((aic_stat_min - aic) / 2)
+        list_b_stat.append(b_stat)
+    list_b_stat = np.array(list_b_stat)
+
+    list_rel_p = []
+    for b_stat in list_b_stat:
+        rel_p = b_stat / np.sum(list_b_stat)
+        list_rel_p.append(rel_p)
+    list_rel_p = np.array(list_rel_p)
 
-    return list_p
+    return list_rel_p
```

### Comparing `asgardpy-0.3.4/asgardpy/io/io.py` & `asgardpy-0.3.5/asgardpy/io/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,27 +15,36 @@
 __all__ = ["InputFilePatterns", "InputConfig", "DL3Files"]
 
 EXPECTED_DL3_RANGE = ["gadf-dl3", "lat", "lat-aux"]
 
 
 # Basic Components for the Input Config
 class InputFilePatterns(BaseConfig):
+    """
+    Config section for list of file patterns to use for fetching relevant DL3
+    files.
+    """
+
     events: str = "*events.fits*"
     edisp: str = "*DRM.fits*"
     exposure: str = "*BinnedMap.fits*"
     xml_model: str = "*out.xml"
     psf: str = "*psf.fits*"
 
     dl3: str = "dl3*fits"
 
     gal_diffuse: str = "gll_iem_v*.fits*"
     iso_diffuse: str = "iso_P8R3_SOURCE_V*_*.txt"
 
 
 class InputConfig(BaseConfig):
+    """
+    Config section for main information on getting the relevant DL3 files.
+    """
+
     type: str = "type"
     input_dir: PathType = PathType(".")
     glob_pattern: dict = {}
 
 
 # Main Classes for I/O
 class DL3Files:
@@ -132,23 +141,23 @@
             var_list = []
             if key:
                 if "0" not in key:  # For fermipy files, the diffuse files are already unique
                     var_list = [
                         "iso_diff_files",
                     ]
             if isinstance(self.iso_diff_files, list):
-                self.iso_gal_f = self.iso_diff_files[0]
+                setattr(self, "iso_gal_f", self.iso_diff_files[0])
             else:
-                self.iso_gal_f = self.iso_diff_files
+                setattr(self, "iso_gal_f", self.iso_diff_files)
             file_list["iso_diff_file"] = self.iso_gal_f
 
             if isinstance(self.gal_diff_files, list):
-                self.diff_gal_f = self.gal_diff_files[0]
+                setattr(self, "diff_gal_f", self.gal_diff_files[0])
             else:
-                self.diff_gal_f = self.gal_diff_files
+                setattr(self, "diff_gal_f", self.gal_diff_files)
             file_list["gal_diff_file"] = self.diff_gal_f
 
         if len(var_list) > 0:
             for _v in var_list:
                 try:
                     filtered = [K for K in getattr(self, _v) if key in str(K.name)]
                     assert len(filtered) == 1
```

### Comparing `asgardpy-0.3.4/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.5/asgardpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.4
+Version: 0.3.5
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106369.svg)](https://doi.org/10.5281/zenodo.8106369) ![PyPI](https://img.shields.io/pypi/v/asgardpy?label=pypi%20asgardpy) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
@@ -32,10 +32,13 @@
 
 The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
+# Cite
+If you use Asgardpy in a publication, please cite the exact version you used from Zenodo _Cite as_ https://doi.org/10.5281/zenodo.8106369
+
 # Pipeline Template
 
 Pipeline generated based on the template by [python-package-template](https://github.com/allenai/python-package-template).
```

### Comparing `asgardpy-0.3.4/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.5/asgardpy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 asgardpy/base/__init__.py
 asgardpy/base/base.py
 asgardpy/base/geom.py
 asgardpy/base/reduction.py
 asgardpy/config/__init__.py
 asgardpy/config/generator.py
 asgardpy/data/__init__.py
-asgardpy/data/base.py
 asgardpy/data/dataset_1d.py
 asgardpy/data/dataset_3d.py
 asgardpy/data/dl4.py
 asgardpy/data/target.py
 asgardpy/io/__init__.py
-asgardpy/io/io.py
+asgardpy/io/io.py
+tests/test_basic.py
```

### Comparing `asgardpy-0.3.4/setup.py` & `asgardpy-0.3.5/setup.py`

 * *Files identical despite different names*

