# Comparing `tmp/fileformats_medimage-0.3.5.tar.gz` & `tmp/fileformats_medimage-0.4.0.tar.gz`

## Comparing `fileformats_medimage-0.3.5.tar` & `fileformats_medimage-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/base.py
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/converters.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/mrtrix.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/raw.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/fileformats/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/LICENSE
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/README.rst
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    19496 2020-02-02 00:00:00.000000 fileformats_medimage-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/base.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/mrtrix.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/raw.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/README.rst
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    19004 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/PKG-INFO
```

### Comparing `fileformats_medimage-0.3.5/.pre-commit-config.yaml` & `fileformats_medimage-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/conftest.py` & `fileformats_medimage-0.4.0/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import logging
 import tempfile
 from pathlib import Path
 import pytest
-from pydra import set_input_validator
-
-# set_input_validator(True)
+try:
+    from pydra import set_input_validator
+except ImportError:
+    pass
+else:
+    set_input_validator(True)
 from fileformats.medimage.dicom import DicomDir
 
 
 # Set DEBUG logging for unittests
 
 log_level = logging.WARNING
 
@@ -47,14 +50,20 @@
 @pytest.fixture(scope="session")
 def dummy_mixedfmap_dicom():
     import medimages4tests.dummy.dicom.mri.fmap.ge.discovery_mr888.dv26_0_r05_2008a as module
 
     return DicomDir(module.get_image())
 
 
+@pytest.fixture(scope="session")
+def dummy_dwi_dicom():
+    import medimages4tests.dummy.dicom.mri.dwi.siemens.skyra.syngo_d13c as module
+
+    return DicomDir(module.get_image())
+
 # For debugging in IDE's don't catch raised exceptions and let the IDE
 # break at it
 if os.getenv("_PYTEST_RAISE", "0") != "0":
 
     @pytest.hookimpl(tryfirst=True)
     def pytest_exception_interact(call):
         raise call.excinfo.value
```

### Comparing `fileformats_medimage-0.3.5/.github/workflows/publish.yml` & `fileformats_medimage-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/.github/workflows/tests.yml` & `fileformats_medimage-0.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/__init__.py` & `fileformats_medimage-0.4.0/fileformats/medimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from ._version import __version__
 from .base import MedicalImage
 from .misc import (  # noqa: F401
     Analyze,
 )
 from .nifti import (
     Nifti,
+    Nifti1,
+    Nifti2,
     NiftiGz,
     NiftiX,
     NiftiGzX,
 )
 from .mrtrix import MrtrixImage, MrtrixImageHeader
 from .diffusion import (
     DwiEncoding,
```

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/base.py` & `fileformats_medimage-0.4.0/fileformats/medimage/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import math
 from fileformats.generic import FileSet
 
 
 # =====================================================================
 # Custom loader functions for different image types
 # =====================================================================
 
@@ -99,8 +100,8 @@
                     diff.append(key)
         return diff
 
     def rms_diff(self, other_image):
         """
         Return the RMS difference between the image arrays
         """
-        return np.sqrt(np.sum((self.get_array() - other_image.get_array()) ** 2))
+        return math.sqrt(sum((self.get_array() - other_image.get_array()) ** 2))
```

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/dicom.py` & `fileformats_medimage-0.4.0/fileformats/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.4.0/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/mrtrix.py` & `fileformats_medimage-0.4.0/fileformats/medimage/mrtrix.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/nifti.py` & `fileformats_medimage-0.4.0/fileformats/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/fileformats/medimage/raw.py` & `fileformats_medimage-0.4.0/fileformats/medimage/raw.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/LICENSE` & `fileformats_medimage-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.3.5/README.rst` & `fileformats_medimage-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-FileFormats Extension - Medimage
-================================
+FileFormats - Medimage
+======================
 .. image:: https://github.com/ArcanaFramework/fileformats-medimage/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/ArcanaFramework/fileformats-medimage/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/ArcanaFramework/fileformats-medimage/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/ArcanaFramework/fileformats-medimage
 .. image:: https://img.shields.io/pypi/pyversions/fileformats-medimage.svg
    :target: https://pypi.python.org/pypi/fileformats-medimage/
    :alt: Supported Python versions
```

### Comparing `fileformats_medimage-0.3.5/pyproject.toml` & `fileformats_medimage-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fileformats-medimage"
 description = "Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "numpy >= 1.24",
     "fileformats >=0.4.0",
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
@@ -26,15 +26,14 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
@@ -50,24 +49,14 @@
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
     "medimages4tests >=0.3",
 ]
 
-extended = [
-    "pydra >= 0.20.0",
-    "pydra-dcm2niix",
-    "pydra-mrtrix3",
-    "numpy >=1.20",    
-    "attrs >=22.1.0",
-    "jq >=1.4.0",
-    "nibabel >=5.0.0",
-    "pydicom >=2.3.1",
-]
 
 [project.urls]
 repository = "https://github.com/ArcanaFramework/fileformats-medimage"
 
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `fileformats_medimage-0.3.5/PKG-INFO` & `fileformats_medimage-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage
-Version: 0.3.5
+Version: 0.4.0
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -101,47 +101,37 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: fileformats>=0.4.0
 Requires-Dist: numpy>=1.24
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Provides-Extra: extended
-Requires-Dist: attrs>=22.1.0; extra == 'extended'
-Requires-Dist: jq>=1.4.0; extra == 'extended'
-Requires-Dist: nibabel>=5.0.0; extra == 'extended'
-Requires-Dist: numpy>=1.20; extra == 'extended'
-Requires-Dist: pydicom>=2.3.1; extra == 'extended'
-Requires-Dist: pydra-dcm2niix; extra == 'extended'
-Requires-Dist: pydra-mrtrix3; extra == 'extended'
-Requires-Dist: pydra>=0.20.0; extra == 'extended'
 Provides-Extra: test
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
-FileFormats Extension - Medimage
-================================
+FileFormats - Medimage
+======================
 .. image:: https://github.com/ArcanaFramework/fileformats-medimage/actions/workflows/tests.yml/badge.svg
    :target: https://github.com/ArcanaFramework/fileformats-medimage/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/ArcanaFramework/fileformats-medimage/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/ArcanaFramework/fileformats-medimage
 .. image:: https://img.shields.io/pypi/pyversions/fileformats-medimage.svg
    :target: https://pypi.python.org/pypi/fileformats-medimage/
    :alt: Supported Python versions
```

