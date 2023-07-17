# Comparing `tmp/dkist-header-validator-3.0.5.tar.gz` & `tmp/dkist-header-validator-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-header-validator-3.0.5.tar", last modified: Tue Feb 28 22:00:03 2023, max compression
+gzip compressed data, was "dkist-header-validator-4.0.0rc1.tar", last modified: Mon Jul 17 17:15:27 2023, max compression
```

## Comparing `dkist-header-validator-3.0.5.tar` & `dkist-header-validator-4.0.0rc1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1960 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/dkist_header_validator/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/dkist_header_validator/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/api/validate.py
--rw-rw-rw-   0 root         (0) root         (0)    26508 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/base_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/spec_validators.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/dkist_header_validator/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18885 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16213 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_base_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_translation.py
--rw-rw-rw-   0 root         (0) root         (0)     4981 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_validation+.py
--rw-rw-rw-   0 root         (0) root         (0)     3649 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_validation-.py
--rw-rw-rw-   0 root         (0) root         (0)    13832 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec214_validation+.py
--rw-rw-rw-   0 root         (0) root         (0)     5803 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec214_validation-.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/tests/test_translator.py
--rw-rw-rw-   0 root         (0) root         (0)     7451 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/translator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/dkist_header_validator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/dkist_header_validator/utils/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1324 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-02-28 22:00:03.000000 dkist-header-validator-3.0.5/dkist_header_validator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 22:00:03.422174 dkist-header-validator-3.0.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-02-28 22:00:03.426174 dkist-header-validator-3.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-02-28 21:59:58.000000 dkist-header-validator-3.0.5/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.350567 dkist-header-validator-4.0.0rc1/dkist_header_validator/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)    26463 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/base_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/spec_validators.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18856 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16213 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_base_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_translation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4981 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation+.py
+-rw-rw-rw-   0 root         (0) root         (0)     3649 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation-.py
+-rw-rw-rw-   0 root         (0) root         (0)    13832 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation+.py
+-rw-rw-rw-   0 root         (0) root         (0)     5803 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation-.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/translator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/tox.ini
```

### Comparing `dkist-header-validator-3.0.5/.gitignore` & `dkist-header-validator-4.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/.pre-commit-config.yaml` & `dkist-header-validator-4.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/PKG-INFO` & `dkist-header-validator-4.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: dkist-header-validator
-Version: 3.0.5
+Version: 4.0.0rc1
 Summary: DKIST data validator
 Home-page: https://bitbucket.org/dkistdc/dkist-header-validator/src/main/
 Author: NSO / AURA
 Author-email: "aderks@nso.edu"
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: cli
 Provides-Extra: docs
 
 DKIST Data Validator
 ====================
 
@@ -123,9 +121,7 @@
     >>> from dkist_header_validator import spec122_validator, Spec122ValidationException
     >>> from astropy.io import fits
     >>> hdus = fits.open('dkist_rosa0181200000_observation.fits')
     >>> spec122_validator.validate(hdus[0].header, return_type=dict)
 
 
 This project is Copyright (c) AURA/NSO.
-
-
```

### Comparing `dkist-header-validator-3.0.5/README.rst` & `dkist-header-validator-4.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/bitbucket-pipelines.yml` & `dkist-header-validator-4.0.0rc1/bitbucket-pipelines.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Build Configuration for python package deployment to pypi
-image: python:3.9
+image: python:3.11
 
 definitions:
   steps:
     - step: &lint
         caches:
           - pip
         name: Lint
@@ -11,17 +11,16 @@
           - pip install pre-commit
           - pre-commit install
           - pre-commit run --all-files
     - step: &test
         name: Test
         script:
           - pip install -U pip
-          - pip install tox codecov
-          - tox -e py39-test
-          - codecov
+          - pip install .[test]
+          - pytest -v -n auto --cov dkist_header_validator
     - step: &scan
         caches:
           - pip
         name: Scan
         script:
           - pip install -e .
           - pip freeze | grep -v @ > requirements.txt
```

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/api/validate.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/api/validate.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/base_validator.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/base_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from io import BytesIO
 from numbers import Integral
 from numbers import Real
 from pathlib import Path
 from typing import Any
 from typing import IO
 from typing import Type
-from typing import Union
 
 import astropy.time as t
 import astropy.units as u
 import numpy as np
 import voluptuous as vol
 from astropy.io import fits
 from astropy.io.fits.hdu.hdulist import HDUList
@@ -326,28 +325,28 @@
         SpecValidationException or subclass of SpecValidationException
             to raise if spec_validator validation fails
 
     """
 
     def __init__(
         self,
-        spec_schema: Union[schema_type_hint, SpecSchema],
+        spec_schema: schema_type_hint | SpecSchema,
         SchemaValidationException: Type[SpecValidationException] = SpecValidationException,
     ):
         # Callable for validating a dict against the defined spec_validator
         if isinstance(spec_schema, SpecSchema):
             self.spec_schema = spec_schema
         else:
             self.spec_schema = SpecSchema(spec_schema)
 
         # Exception raised when spec validation fails
         self.SchemaValidationException = SchemaValidationException
 
     @staticmethod
-    def _headers_to_dict(headers: Union[HDUList, dict, fits.header.Header, str, IO]) -> dict:
+    def _headers_to_dict(headers: HDUList | dict | fits.header.Header | str | IO) -> dict:
         """
         Convert headers from multiple types to a dict
         :param headers: Headers to convert to a dict
         :return: Dict of the headers
         """
         if isinstance(headers, dict):
             return headers
@@ -418,15 +417,15 @@
 
             raise self.SchemaValidationException(errors=validation_errors)
         logger.debug("Schema validation succeeded")
 
         return headers
 
     def _validate_headers(
-        self, input_headers: Union[HDUList, dict, fits.header.Header], extra
+        self, input_headers: HDUList | dict | fits.header.Header, extra
     ) -> tuple[dict, dict]:
         """
         Validates open input headers against the instance spec_schema
         :param input_headers: The input headers to validate in the following formats:
             - HDUList object
             - fits.header.Header object
             - Dictionary of header keys and values
@@ -439,15 +438,15 @@
                     "Too many HDUs in your HDUList! May only have two HDUs at most."
                 )
         headers = self._headers_to_dict(input_headers)
         fits_cards = self._capture_fits_cards(headers)
         verified_headers = self.verify_headers(headers, extra)
         return verified_headers, fits_cards
 
-    def _validate_file(self, input_headers: Union[str, IO], extra) -> tuple[dict, dict, np.ndarray]:
+    def _validate_file(self, input_headers: str | IO, extra) -> tuple[dict, dict, np.ndarray]:
         """
         Validates files against the astropy and then instance spec_schema
         :param input_headers: The input headers to validate in the following formats:
             - string file path
             - File like object
         :param extra: switch for validation to allow extra keys in schema
         :return: dictionary of verified headers to be used later
```

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/exceptions.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/spec_validators.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/spec_validators.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/conftest.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from typing import Union
 from uuid import uuid4
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.wcs import WCS
 from dkist_data_simulator.spec122 import Spec122Dataset
@@ -18,15 +17,15 @@
     "multiple_fits_cards_hdulist",
     "multiple_fits_cards_header",
 ]
 
 
 def get_fits_object(
     object_type: str, tmpdir: Path, ds, required_only: bool = False, expected_only: bool = False
-) -> Union[str, dict, fits.HDUList, fits.header.Header]:
+) -> str | dict | fits.HDUList | fits.header.Header:
     """
     Build up the required object type from the given simulated Dataset
 
     TYPES
     -----
     fits : a fits file on disk
     compressed : a compressed fits file on disk
```

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_base_validator.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_base_validator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_translation.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_translation.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_validation+.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation+.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec122_validation-.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation-.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec214_validation+.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation+.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_spec214_validation-.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation-.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/tests/test_translator.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/translator.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import logging
 from datetime import datetime
 from functools import reduce
 from typing import Any
-from typing import Dict
 from typing import IO
-from typing import List
-from typing import Optional
-from typing import Tuple
-from typing import Union
 
 from astropy.io import fits
 from astropy.io.fits.hdu.hdulist import HDUList
 from dkist_fits_specifications.spec214 import level0
 from dkist_fits_specifications.spec214 import load_expanded_spec214
 from dkist_fits_specifications.spec214 import load_spec214
 
@@ -26,16 +21,16 @@
     "remove_extra_axis_keys",
 ]
 
 type_map = {"int": int, "float": float, "str": str, "bool": bool}
 
 
 def translate_spec122_to_spec214_l0(
-    spec122_input: Union[HDUList, dict, fits.header.Header, str, IO, List]
-) -> Union[dict, HDUList]:
+    spec122_input: HDUList | dict | fits.header.Header | str | IO | list,
+) -> dict | HDUList:
     """
     Convert spec 122 headers to spec 214 l0 headers
 
     Parameters
     ----------
     spec122_input
         Spec 122 headers or headers + data to convert
@@ -51,16 +46,16 @@
     output_headers["DATE"] = datetime.now().isoformat()
     if input_data:  # return hdu list if the input had data
         return _format_output_hdu(output_headers, input_data)
     return output_headers  # return headers if only headers were given
 
 
 def sanitize_to_spec214_level1(
-    input_headers: Union[HDUList, dict, fits.header.Header, str, IO, List]
-) -> Union[dict, HDUList]:
+    input_headers: HDUList | dict | fits.header.Header | str | IO | list,
+) -> dict | HDUList:
     """
     Remove all non-214 compliant header values
 
     Parameters
     ----------
     input_headers
         Spec 214 headers or headers + data to convert
@@ -81,16 +76,16 @@
 
     if input_data is not None:  # return hdu list if the input had data
         return _format_output_hdu(header, input_data)
     return header  # return headers if only headers were given
 
 
 def remove_extra_axis_keys(
-    input_headers: Union[HDUList, dict, fits.header.Header, str, IO, List]
-) -> Union[dict, HDUList]:
+    input_headers: HDUList | dict | fits.header.Header | str | IO | list,
+) -> dict | HDUList:
     """
     Remove all keywords that refer to axes that don't exist in the data array
 
     Parameters
     ----------
     input_headers
         Spec 214 headers or headers + data
@@ -114,16 +109,16 @@
 
     if input_data is not None:  # return hdu list if the input had data
         return _format_output_hdu(header, input_data)
     return header  # return headers if only headers were given
 
 
 def _parse_fits_like_input(
-    spec122_input: Union[HDUList, dict, fits.header.Header, str, IO, List]
-) -> Tuple[fits.Header, Optional[bytes]]:
+    spec122_input: HDUList | dict | fits.header.Header | str | IO | list,
+) -> tuple[fits.Header, bytes | None]:
     """
     Parse out a header and optional data from the various types of input
     """
     if isinstance(spec122_input, dict):
         return fits.Header(spec122_input), None
     if isinstance(spec122_input, fits.header.Header):
         return spec122_input, None
@@ -148,15 +143,15 @@
     for key, value in hdr.items():
         hdu_list[0].header[key] = value
     return hdu_list
 
 
 def _create_spec214_schema_for_header(
     hdr: dict, generic_schema, naxis=None
-) -> Dict[str, Dict[str, Any]]:
+) -> dict[str, dict[str, Any]]:
     s = {key: schema for definition in generic_schema for (key, schema) in definition.items()}
     if naxis == None:
         return s
     else:
         hdr["DNAXIS"] = naxis
         return expand_index_d(expand_naxis(hdr["NAXIS"], s), DNAXIS=hdr["DNAXIS"])
```

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator/utils/expansions.py` & `dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator.egg-info/PKG-INFO` & `dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: dkist-header-validator
-Version: 3.0.5
+Version: 4.0.0rc1
 Summary: DKIST data validator
 Home-page: https://bitbucket.org/dkistdc/dkist-header-validator/src/main/
 Author: NSO / AURA
 Author-email: "aderks@nso.edu"
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: cli
 Provides-Extra: docs
 
 DKIST Data Validator
 ====================
 
@@ -123,9 +121,7 @@
     >>> from dkist_header_validator import spec122_validator, Spec122ValidationException
     >>> from astropy.io import fits
     >>> hdus = fits.open('dkist_rosa0181200000_observation.fits')
     >>> spec122_validator.validate(hdus[0].header, return_type=dict)
 
 
 This project is Copyright (c) AURA/NSO.
-
-
```

### Comparing `dkist-header-validator-3.0.5/dkist_header_validator.egg-info/SOURCES.txt` & `dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/docs/Makefile` & `dkist-header-validator-4.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/docs/conf.py` & `dkist-header-validator-4.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/docs/make.bat` & `dkist-header-validator-4.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/setup.cfg` & `dkist-header-validator-4.0.0rc1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -6,52 +6,46 @@
 author_email = "aderks@nso.edu"
 license = MIT
 url = https://bitbucket.org/dkistdc/dkist-header-validator/src/main/
 edit_on_github = False
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	astropy >= 5.0
 	voluptuous >=0.11.7, < 1.0.0
-	pyyaml >=5.3, < 6.0
+	pyyaml >=5.3
 	dkist-fits-specifications >= 2.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
+	pytest-xdist
 	deepdiff
 	tox
 	dkist-data-simulator
 cli = 
 	typer
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog
 	sphinx-autoapi
 	pytest
 	towncrier
 	dkist-sphinx-theme
 
-[pycodestyle]
-max_line_length = 100
-
-[flake8]
-max-line-length = 100
-
 [tool:pytest]
 minversion = 3.0
 testpaths = "dkist_header_validator/tests"
 norecursedirs = ".tox" "build" "docs[\/]_build" "docs[\/]generated" "*.egg-info" "examples"
 
 [coverage:run]
 source = dkist_header_validator/
```

### Comparing `dkist-header-validator-3.0.5/setup.py` & `dkist-header-validator-4.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-3.0.5/tox.ini` & `dkist-header-validator-4.0.0rc1/tox.ini`

 * *Files identical despite different names*

