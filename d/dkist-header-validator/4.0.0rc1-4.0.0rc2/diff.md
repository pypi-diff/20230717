# Comparing `tmp/dkist-header-validator-4.0.0rc1.tar.gz` & `tmp/dkist-header-validator-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-header-validator-4.0.0rc1.tar", last modified: Mon Jul 17 17:15:27 2023, max compression
+gzip compressed data, was "dkist-header-validator-4.0.0rc2.tar", last modified: Mon Jul 17 17:33:23 2023, max compression
```

## Comparing `dkist-header-validator-4.0.0rc1.tar` & `dkist-header-validator-4.0.0rc2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     1960 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.350567 dkist-header-validator-4.0.0rc1/dkist_header_validator/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/api/validate.py
--rw-rw-rw-   0 root         (0) root         (0)    26463 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/base_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/spec_validators.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18856 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16213 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_base_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_translation.py
--rw-rw-rw-   0 root         (0) root         (0)     4981 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation+.py
--rw-rw-rw-   0 root         (0) root         (0)     3649 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation-.py
--rw-rw-rw-   0 root         (0) root         (0)    13832 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation+.py
--rw-rw-rw-   0 root         (0) root         (0)     5803 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation-.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_translator.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/translator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-17 17:15:27.000000 dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-17 17:15:27.354568 dkist-header-validator-4.0.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-17 17:15:22.000000 dkist-header-validator-4.0.0rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.382390 dkist-header-validator-4.0.0rc2/dkist_header_validator/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/dkist_header_validator/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/api/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)    26463 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/base_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/spec_validators.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18856 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16213 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_base_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_translation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4981 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_validation+.py
+-rw-rw-rw-   0 root         (0) root         (0)     3649 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_validation-.py
+-rw-rw-rw-   0 root         (0) root         (0)    13832 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec214_validation+.py
+-rw-rw-rw-   0 root         (0) root         (0)     5803 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec214_validation-.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/translator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/dkist_header_validator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/utils/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-17 17:33:23.000000 dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-17 17:33:23.386390 dkist-header-validator-4.0.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-17 17:33:17.000000 dkist-header-validator-4.0.0rc2/tox.ini
```

### Comparing `dkist-header-validator-4.0.0rc1/.gitignore` & `dkist-header-validator-4.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/.pre-commit-config.yaml` & `dkist-header-validator-4.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/PKG-INFO` & `dkist-header-validator-4.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-header-validator
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: DKIST data validator
 Home-page: https://bitbucket.org/dkistdc/dkist-header-validator/src/main/
 Author: NSO / AURA
 Author-email: "aderks@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-header-validator-4.0.0rc1/README.rst` & `dkist-header-validator-4.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/bitbucket-pipelines.yml` & `dkist-header-validator-4.0.0rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/api/validate.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/api/validate.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/base_validator.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/base_validator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/exceptions.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/spec_validators.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/spec_validators.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/conftest.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_base_validator.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_base_validator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_translation.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_translation.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation+.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_validation+.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec122_validation-.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec122_validation-.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation+.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec214_validation+.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_spec214_validation-.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_spec214_validation-.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/tests/test_translator.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/translator.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/translator.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator/utils/expansions.py` & `dkist-header-validator-4.0.0rc2/dkist_header_validator/utils/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/PKG-INFO` & `dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-header-validator
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: DKIST data validator
 Home-page: https://bitbucket.org/dkistdc/dkist-header-validator/src/main/
 Author: NSO / AURA
 Author-email: "aderks@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-header-validator-4.0.0rc1/dkist_header_validator.egg-info/SOURCES.txt` & `dkist-header-validator-4.0.0rc2/dkist_header_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/docs/Makefile` & `dkist-header-validator-4.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/docs/conf.py` & `dkist-header-validator-4.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/docs/make.bat` & `dkist-header-validator-4.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/setup.cfg` & `dkist-header-validator-4.0.0rc2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	astropy >= 5.0
 	voluptuous >=0.11.7, < 1.0.0
-	pyyaml >=5.3
+	pyyaml >=6.0
 	dkist-fits-specifications >= 2.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-xdist
```

### Comparing `dkist-header-validator-4.0.0rc1/setup.py` & `dkist-header-validator-4.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `dkist-header-validator-4.0.0rc1/tox.ini` & `dkist-header-validator-4.0.0rc2/tox.ini`

 * *Files identical despite different names*

