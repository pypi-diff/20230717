# Comparing `tmp/sotai-0.1.0.tar.gz` & `tmp/sotai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.1.0.tar", last modified: Tue Jul  4 21:17:51 2023, max compression
+gzip compressed data, was "sotai-0.2.0.tar", last modified: Mon Jul 17 21:08:28 2023, max compression
```

## Comparing `sotai-0.1.0.tar` & `sotai-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.031257 sotai-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 21:17:39.000000 sotai-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-04 21:17:51.031257 sotai-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-04 21:17:39.000000 sotai-0.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-04 21:17:39.000000 sotai-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:17:51.031257 sotai-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/trained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-04 21:17:39.000000 sotai-0.1.0/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.027257 sotai-0.1.0/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 21:17:51.000000 sotai-0.1.0/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:17:51.031257 sotai-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-04 21:17:39.000000 sotai-0.1.0/tests/test_trained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 21:08:14.000000 sotai-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 21:08:28.106196 sotai-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.102196 sotai-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-17 21:08:14.000000 sotai-0.2.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-17 21:08:14.000000 sotai-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:08:28.106196 sotai-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.102196 sotai-0.2.0/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19907 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-07-17 21:08:14.000000 sotai-0.2.0/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 21:08:28.000000 sotai-0.2.0/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:08:28.106196 sotai-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-17 21:08:14.000000 sotai-0.2.0/tests/test_trained_model.py
```

### Comparing `sotai-0.1.0/LICENSE` & `sotai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.1.0/PKG-INFO` & `sotai-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
@@ -22,41 +22,45 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">SOTAI</h1>
 
-<p align='center'>
-<a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
+<p align="center">
+  <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
+  <a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml"><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
-Installling the package:
+Installing the package:
 
 ```shell
 pip install sotai
 ```
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
+## SOTAI SDK Documentation
+
+You can find documentation for this SDK at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk) or in the repo [docs folder](./).
+
 ## SOTAI Web-App User Documentation
 
 You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
 For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+[MIT](../LICENSE/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sotai Version: 0.1.0 Summary: A Python Library For
+Metadata-Version: 2.1 Name: sotai Version: 0.2.0 Summary: A Python Library For
 Calibrated Modeling Built With PyTorch Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: MIT Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-
 calibrated/issues Project-URL: Bug Reports, https://github.com/SOTAI-Labs/
 pytorch-calibrated/issues Classifier: Development Status :: 5 - Production/
@@ -17,17 +17,18 @@
 markdown License-File: LICENSE
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
               actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
-243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
-find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
-app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
-[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
-CONTRIBUTING.md) for full details on how to contribute to the library. For any
-feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
-sotai/issues). ## Examples For detailed examples on how to use the library, see
-[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
-License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+243.pdf). Installing the package: ```shell pip install sotai ``` Importing the
+package: ```python import sotai ``` ## SOTAI SDK Documentation You can find
+documentation for this SDK at [https://docs.sotai.ai/sdk](https://
+docs.sotai.ai/sdk) or in the repo [docs folder](./). ## SOTAI Web-App User
+Documentation You can find documentation for how to use the hosted web-app at
+[https://docs.sotai.ai/app](https://docs.sotai.ai/app) ## Contribution
+Guidelines See the guide on [contributing](CONTRIBUTING.md) for full details on
+how to contribute to the library. For any feature and/or bug requests, visit
+our [Issues](https://github.com/SOTAI-Labs/sotai/issues). ## Examples For
+detailed examples on how to use the library, see [examples](https://github.com/
+SOTAI-Labs/sotai/tree/main/docs/examples). ## License [MIT](../LICENSE/)
```

### Comparing `sotai-0.1.0/docs/README.md` & `sotai-0.2.0/docs/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 <h1 align="center">SOTAI</h1>
 
-<p align='center'>
-<a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
+<p align="center">
+  <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
+  <a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml"><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
-Installling the package:
+Installing the package:
 
 ```shell
 pip install sotai
 ```
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
+## SOTAI SDK Documentation
+
+You can find documentation for this SDK at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk) or in the repo [docs folder](./).
+
 ## SOTAI Web-App User Documentation
 
 You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
 For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+[MIT](../LICENSE/)
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
               actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
-243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
-find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
-app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
-[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
-CONTRIBUTING.md) for full details on how to contribute to the library. For any
-feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
-sotai/issues). ## Examples For detailed examples on how to use the library, see
-[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
-License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+243.pdf). Installing the package: ```shell pip install sotai ``` Importing the
+package: ```python import sotai ``` ## SOTAI SDK Documentation You can find
+documentation for this SDK at [https://docs.sotai.ai/sdk](https://
+docs.sotai.ai/sdk) or in the repo [docs folder](./). ## SOTAI Web-App User
+Documentation You can find documentation for how to use the hosted web-app at
+[https://docs.sotai.ai/app](https://docs.sotai.ai/app) ## Contribution
+Guidelines See the guide on [contributing](CONTRIBUTING.md) for full details on
+how to contribute to the library. For any feature and/or bug requests, visit
+our [Issues](https://github.com/SOTAI-Labs/sotai/issues). ## Examples For
+detailed examples on how to use the library, see [examples](https://github.com/
+SOTAI-Labs/sotai/tree/main/docs/examples). ## License [MIT](../LICENSE/)
```

### Comparing `sotai-0.1.0/pyproject.toml` & `sotai-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
-#
-# NOTE: as part of the release flow, update this version immediately after release.
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `sotai-0.1.0/sotai/data.py` & `sotai-0.2.0/sotai/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,23 @@
 from .types import CategoricalFeatureConfig, NumericalFeatureConfig
 
 
 def replace_missing_values(
     data: pd.DataFrame,
     feature_configs: Dict[str, Union[CategoricalFeatureConfig, NumericalFeatureConfig]],
 ) -> pd.DataFrame:
-    """Replaces empty values or unspecified categories with a constant value."""
+    """Replaces empty values or unspecified categories with a constant value.
+
+    Args:
+        - data: The dataset in which to replace missing values.
+        - feature_configs: A dictionary mapping feature names to feature configurations.
+
+    Returns:
+        The dataset with missing values replaced.
+    """
     for feature_name, feature_config in feature_configs.items():
         if feature_config.type == FeatureType.CATEGORICAL:
             unspecified_categories = list(
                 set(data[feature_name].unique().tolist())
                 - set(feature_config.categories)
             )
             if unspecified_categories:
@@ -62,15 +70,14 @@
         data: A pandas `DataFrame` containing the loaded CSV data.
         headers: The list of headers available from the loaded data.
         num_examples: The number of examples in the dataset.
         prepared_data: The prepared data. This will be `None` if `prepare(...)` has not
             been called.
 
     Example:
-
     ```python
     csv_data = CSVData("path/to/data.csv")
     feature_configs = [
         NumericalFeatureConfig(
             feature_name="numerical_feature"
             data=csv_data("numerical_feature")  # must match feature column header
         ),
```

### Comparing `sotai-0.1.0/sotai/features.py` & `sotai-0.2.0/sotai/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Feature objects for use in models.
 
 To construct a calibrated model, create the calibrated model configuration and pass it
 in to the corresponding calibrated model constructor.
 
 Example:
-
 ```python
 feature_configs = [...]
 linear_config = CalibratedLinearConfig(feature_configs, ...)
 linear_model = CalibratedLinear(linear_config)
 ```
 """
 import logging
@@ -49,14 +48,15 @@
         self,
         feature_name: str,
         data: np.ndarray,
         num_keypoints: int = 10,
         input_keypoints_init: InputKeypointsInit = InputKeypointsInit.QUANTILES,
         missing_input_value: Optional[float] = None,
         monotonicity: Monotonicity = Monotonicity.NONE,
+        projection_iterations: int = 8,
     ) -> None:
         """Initializes a `NumericalFeatureConfig` instance.
 
         Args:
             feature_name: The name of the feature. This should match the header for the
                 column in the dataset representing this feature.
             data: Numpy array of float-valued data used for calculating keypoint inputs
@@ -65,14 +65,16 @@
                 linear function of a NumericalCalibrator. There will be
                 `num_keypoints - 1` total segments.
             input_keypoints_init: The scheme to use for initializing the input
                 keypoints. See `InputKeypointsInit` for more details.
             missing_input_value: If provided, this feature's calibrator will learn to
                 map all instances of this missing input value to a learned output value.
             monotonicity: Monotonicity constraint for this feature, if any.
+            projection_iterations: Number of times to run Dykstra's projection
+                algorithm when applying constraints.
 
         Raises:
             ValueError: If `data` contains NaN values.
             ValueError: If `input_keypoints_init` is invalid.
         """
         super().__init__(feature_name, FeatureType.NUMERICAL)
 
@@ -80,14 +82,15 @@
             raise ValueError("Data contains NaN values.")
 
         self.data = data
         self.num_keypoints = num_keypoints
         self.input_keypoints_init = input_keypoints_init
         self.missing_input_value = missing_input_value
         self.monotonicity = monotonicity
+        self.projection_iterations = projection_iterations
 
         sorted_unique_values = np.unique(data)
 
         if input_keypoints_init == InputKeypointsInit.QUANTILES:
             if sorted_unique_values.size < num_keypoints:
                 logging.info(
                     "Observed fewer unique values for feature %s than %d desired "
@@ -122,15 +125,15 @@
             categories to category indices. Only available if `monotonicity_pairs` are
             provided.
     """
 
     def __init__(
         self,
         feature_name: str,
-        categories: Union[List[str], List[int]],
+        categories: Union[List[int], List[str]],
         missing_input_value: Optional[float] = None,
         monotonicity_pairs: Optional[List[Tuple[str, str]]] = None,
     ) -> None:
         """Initializes a `CategoricalFeatureConfig` instance.
 
         Args:
             feature_name: The name of the feature. This should match the header for the
```

### Comparing `sotai-0.1.0/sotai/layers/categorical_calibrator.py` & `sotai-0.2.0/sotai/layers/categorical_calibrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     the input.
 
     Attributes:
         - All `__init__` arguments.
         kernel: `torch.nn.Parameter` that stores the categorical mapping weights.
 
     Example:
-
     ```python
     inputs = torch.tensor(...)  # shape: (batch_size, 1)
     calibrator = CategoricalCalibrator(
         num_categories=5,
         missing_input_value=-1,
         output_min=0.0
         output_max=1.0,
@@ -174,15 +173,15 @@
         return torch.squeeze(self.kernel.data, -1)
 
     ################################################################################
     ############################## PRIVATE METHODS #################################
     ################################################################################
 
     def _approximately_project_monotonicity_pairs(self, kernel_data) -> torch.Tensor:
-        """Projects kernel such that
+        """Projects kernel such that the monotonicity pairs are satisfied.
 
         The kernel will be projected such that `kernel_data[i] <= kernel_data[j]`. This
         results in calibrated outputs that adhere to the desired constraints.
 
         Args:
             kernel_data: The tensor of shape `(self.num_categories, 1)` to be projected
                 into the constraints specified by `self.monotonicity pairs`.
```

### Comparing `sotai-0.1.0/sotai/layers/linear.py` & `sotai-0.2.0/sotai/layers/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     Attributes:
       - All `__init__` arguments.
       kernel: `torch.nn.Parameter` that stores the linear combination weighting.
       bias: `torch.nn.Parameter` that stores the bias term. Only available is `use_bias`
         is true.
 
     Example:
-
     ```python
     input_dim = 3
     inputs = torch.tensor(...)  # shape: (batch_size, input_dim)
     linear = Linear(
       input_dim,
       monotonicities=[
         Monotonicity.NONE,
```

### Comparing `sotai-0.1.0/sotai/layers/numerical_calibrator.py` & `sotai-0.2.0/sotai/layers/numerical_calibrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     Attributes:
         - All `__init__` arguments.
         kernel: `torch.nn.Parameter` that stores the piece-wise linear function weights.
         missing_output: `torch.nn.Parameter` that stores the output learned for any
             missing inputs. Only available if `missing_input_value` is provided.
 
     Example:
-
     ```python
     inputs = torch.tensor(...)  # shape: (batch_size, 1)
     calibrator = NumericalCalibrator(
         input_keypoints=np.linspace(1., 5., num=5),
         output_min=0.0,
         output_max=1.0,
         monotonicity=Monotonicity.INCREASING,
```

### Comparing `sotai-0.1.0/sotai/models.py` & `sotai-0.2.0/sotai/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 self.calibrators[feature.feature_name] = NumericalCalibrator(
                     input_keypoints=feature.input_keypoints,
                     missing_input_value=feature.missing_input_value,
                     output_min=output_min,
                     output_max=output_max,
                     monotonicity=feature.monotonicity,
                     kernel_init=NumericalCalibratorInit.EQUAL_SLOPES,
+                    projection_iterations=feature.projection_iterations,
                 )
                 if feature.monotonicity == Monotonicity.NONE:
                     linear_monotonicities.append(Monotonicity.NONE)
                 else:
                     linear_monotonicities.append(Monotonicity.INCREASING)
             elif feature.feature_type == FeatureType.CATEGORICAL:
                 self.calibrators[feature.feature_name] = CategoricalCalibrator(
```

### Comparing `sotai-0.1.0/sotai/trained_model.py` & `sotai-0.2.0/sotai/trained_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A Trained Model created for a pipeline."""
 from __future__ import annotations
 
 import os
 import pickle
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
 from pydantic import BaseModel, Field
 
 from .data import CSVData, replace_missing_values
@@ -20,58 +20,59 @@
     """A trained calibrated model.
 
     This model is a container for a trained calibrated model that provides useful
     methods for using the model. The trained calibrated model is the result of running
     the `train` method of a `Pipeline` instance.
 
     Example:
-
     ```python
     data = pd.read_csv("data.csv")
     predictions = trained_model.predict(data)
     trained_model.analyze()
     ```
     """
 
     dataset_id: int = Field(...)
     pipeline_uuid: Optional[str] = None
     pipeline_config: PipelineConfig = Field(...)
     model_config: LinearConfig = Field(...)
     training_config: TrainingConfig = Field(...)
     training_results: TrainingResults = Field(...)
     model: CalibratedLinear = Field(...)
-    trained_model_uuid: Optional[str] = None
+    uuid: Optional[str] = None
     analysis_url: Optional[str] = None
 
     class Config:  # pylint: disable=missing-class-docstring,too-few-public-methods
+        """Standard Pydantic BaseModel Config."""
+
         arbitrary_types_allowed = True
 
-    def predict(self, data: pd.DataFrame) -> np.ndarray:
+    def predict(self, data: pd.DataFrame) -> Tuple[np.ndarray, Optional[np.ndarray]]:
         """Returns predictions for the given data.
 
         Args:
             data: The data to be used for prediction. Must have all columns used for
                 training the model to be used.
 
         Returns:
-            If the target type is regression, a numpy array of predictions. If the
-            target type is classification, a tuple containing a numpy array of
-            predictions (logits) and a numpy array of probabilities.
+            A tuple containing an array of predictions and an array of probabilities.
+            If the target type is regression, then logits will be `None`. If the target
+            type is classification, then the predictions will be logits.
         """
         data = data.loc[:, list(self.pipeline_config.feature_configs.keys())]
         data = replace_missing_values(data, self.pipeline_config.feature_configs)
 
         csv_data = CSVData(data)
         csv_data.prepare(self.model.features, None)
         inputs = list(csv_data.batch(csv_data.num_examples))[0]
         with torch.no_grad():
             predictions = self.model(inputs).numpy()
 
         if self.pipeline_config.target_type == TargetType.REGRESSION:
-            return predictions
+            return predictions, None
 
         return predictions, 1.0 / (1.0 + np.exp(-predictions))
 
     def save(self, filepath: str):
         """Saves the trained model to the specified directory.
 
         Args:
```

### Comparing `sotai-0.1.0/sotai/training.py` & `sotai-0.2.0/sotai/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,22 +55,23 @@
                 NumericalFeature(
                     feature_name=feature_name,
                     data=train_csv_data(feature_name),
                     num_keypoints=feature_config.num_keypoints,
                     input_keypoints_init=feature_config.input_keypoints_init,
                     missing_input_value=MISSING_NUMERICAL_VALUE,
                     monotonicity=feature_config.monotonicity,
+                    projection_iterations=feature_config.projection_iterations,
                 )
             )
 
     return features
 
 
 def create_loss(loss_type: LossType) -> torch.nn.Module:
-    """returns a Torch loss function from the given `LossType`."""
+    """Returns a Torch loss function from the given `LossType`."""
     if loss_type == LossType.BINARY_CROSSENTROPY:
         return torch.nn.BCEWithLogitsLoss()
     if loss_type == LossType.HINGE:
         return torch.nn.HingeEmbeddingLoss()
     if loss_type == LossType.HUBER:
         return torch.nn.HuberLoss()
     if loss_type == LossType.MAE:
@@ -176,15 +177,15 @@
     model: CalibratedLinear,
     feature_configs: Dict[str, Union[CategoricalFeatureConfig, NumericalFeatureConfig]],
     data: pd.DataFrame,
 ) -> Dict[str, FeatureAnalysis]:
     """Extracts feature statistics and calibration weights for each feature.
 
     Args:
-        ptcm_model: A PyTorch Calibrated model.
+        model: A (pytorch) calibrated model.
         feature_configs: A mapping from feature name to feature config.
         data: The training + validation data for this model.
 
     Returns:
         A dictionary mapping feature name to `FeatureAnalysis` instance.
     """
     feature_analyses = {}
@@ -198,26 +199,34 @@
             ]
             keypoints_inputs_categorical = []
         else:
             keypoints_inputs_numerical = []
             keypoints_inputs = feature_config.categories + [MISSING_CATEGORY_VALUE]
             keypoints_inputs_categorical = [str(ki) for ki in keypoints_inputs]
 
-        feature_analyses[feature_name] = FeatureAnalysis(
-            feature_name=feature_name,
-            feature_type=feature_config.type,
-            min=float(np.min(data[feature_name].values)),
-            max=float(np.max(data[feature_name].values)),
-            mean=float(np.mean(data[feature_name].values)),
-            median=float(np.median(data[feature_name].values)),
-            std=float(np.std(data[feature_name].values)),
-            keypoints_inputs_numerical=keypoints_inputs_numerical,
-            keypoints_inputs_categorical=keypoints_inputs_categorical,
-            keypoints_outputs=[float(x) for x in calibrator.keypoints_outputs()],
-        )
+        fa_dict = {
+            "feature_name": feature_name,
+            "feature_type": feature_config.type,
+            "keypoints_inputs_numerical": keypoints_inputs_numerical,
+            "keypoints_inputs_categorical": keypoints_inputs_categorical,
+            "keypoints_outputs": [float(x) for x in calibrator.keypoints_outputs()],
+        }
+
+        if feature_config.type == FeatureType.NUMERICAL:
+            fa_dict.update(
+                {
+                    "min": float(np.min(data[feature_name].values)),
+                    "max": float(np.max(data[feature_name].values)),
+                    "mean": float(np.mean(data[feature_name].values)),
+                    "median": float(np.median(data[feature_name].values)),
+                    "std": float(np.std(data[feature_name].values)),
+                }
+            )
+
+        feature_analyses[feature_name] = FeatureAnalysis(**fa_dict)
 
     return feature_analyses
 
 
 def extract_linear_coefficients(
     linear_model: CalibratedLinear,
     features: List[str],
```

### Comparing `sotai-0.1.0/sotai/types.py` & `sotai-0.2.0/sotai/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,30 +48,35 @@
     """
 
     train: pd.DataFrame = Field(...)
     val: pd.DataFrame = Field(...)
     test: pd.DataFrame = Field(...)
 
     class Config:  # pylint: disable=missing-class-docstring,too-few-public-methods
+        """Standard Pydantic BaseModel Config."""
+
         arbitrary_types_allowed = True
 
 
 class Dataset(BaseModel):
     """A class for managing data.
 
     Attributes:
+        id: The ID of the dataset used by the pipeline that prepared it.
         pipeline_config_id: The ID of the pipeline config used to create this dataset.
         prepared_data: The prepared data ready for training.
     """
 
     id: int = Field(...)
     pipeline_config_id: int = Field(...)
     prepared_data: PreparedData = Field(...)
 
     class Config:  # pylint: disable=missing-class-docstring,too-few-public-methods
+        """Standard Pydantic BaseModel Config."""
+
         arbitrary_types_allowed = True
 
 
 class _BaseModelConfig(BaseModel):
     """Configuration for a calibrated model.
 
     Attributes:
@@ -82,15 +87,14 @@
         output_calibration: Whether to calibrate the output.
         output_calibration_num_keypoints: The number of keypoints to use for the output
             calibrator.
         output_initialization: The method for initializing the output calibrator input
             keypoints.
         output_calibration_input_keypoints_type: The type of output calibrator input
             keypoints.
-        advanced_options: Advanced options for the model.
     """
 
     output_min: Optional[float] = None
     output_max: Optional[float] = None
     output_calibration: bool = False
     output_calibration_num_keypoints: int = 10
     output_initialization: InputKeypointsInit = InputKeypointsInit.QUANTILES
@@ -133,27 +137,27 @@
         feature_type: The type of the feature.
         min: The minimum value of the feature.
         max: The maximum value of the feature.
         mean: The mean value of the feature.
         median: The median value of the feature.
         std: The standard deviation of the feature.
         keypoints_inputs_numerical: The input keypoints for the feature if the feature
-            is numerical.
+            is numerical. Otherwise this should be `None`.
         keypoints_inputs_categorical: The input keypoints for the feature if the feature
-            is categorical.
+            is categorical. Otherwise this should be `None`.
         keypoints_outputs: The output keypoints for each input keypoint.
     """
 
     feature_name: str = Field(...)
     feature_type: FeatureType = Field(...)
-    min: float = Field(...)
-    max: float = Field(...)
-    mean: float = Field(...)
-    median: float = Field(...)
-    std: float = Field(...)
+    min: Optional[float] = None
+    max: Optional[float] = None
+    mean: Optional[float] = None
+    median: Optional[float] = None
+    std: Optional[float] = None
     # One of the keypoint inputs must exist, which one depends on feature_type.
     keypoints_inputs_numerical: Optional[List[float]] = Field(...)
     keypoints_inputs_categorical: Optional[List[str]] = Field(...)
     keypoints_outputs: List[float] = Field(...)
 
 
 class TrainingResults(BaseModel):
@@ -196,63 +200,67 @@
     Attributes:
         name: The name of the feature.
         type: The type of the feature. Always `FeatureType.NUMERICAL`.
         num_keypoints: The number of keypoints to use for the calibrator.
         input_keypoints_init: The method for initializing the input keypoints.
         input_keypoints_type: The type of input keypoints.
         monotonicity: The monotonicity constraint, if any.
+        projection_iterations: Number of times to run Dykstra's projection algorithm
+            when applying constraints.
     """
 
     name: str = Field(...)
     type: FeatureType = Field(FeatureType.NUMERICAL, const=True)
     num_keypoints: int = 10
     input_keypoints_init: InputKeypointsInit = InputKeypointsInit.QUANTILES
     input_keypoints_type: InputKeypointsType = InputKeypointsType.FIXED
     monotonicity: Monotonicity = Monotonicity.NONE
+    projection_iterations: int = 8
 
 
 class CategoricalFeatureConfig(BaseModel):
     """Configuration for a categorical feature.
 
     Attributes:
         name: The name of the feature.
         type: The type of the feature. Always `FeatureType.CATEGORICAL`.
         categories: The categories for the feature.
     """
 
     name: str = Field(...)
     type: FeatureType = Field(FeatureType.CATEGORICAL, const=True)
-    categories: Union[List[str], List[int]] = Field(...)
+    categories: Union[List[int], List[str]] = Field(...)
     # TODO (will): add support for categorical monotonicity.
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
 class PipelineConfig(BaseModel):
     """A configuration object for a `Pipeline`.
 
     Attributes:
-        id: The ID of the pipeline config.
-        pipeline_uuid: The UUID of the pipeline.
+        id: The ID of the pipeline config. This will be set by the Pipeline when it
+            versions this config during preparation.
+        uuid: The UUID of the pipeline.
         target: The column name for the target.
         target_type: The type of the target.
         primary_metric: The primary metric to use for training and evaluation.
         feature_configs: A dictionary mapping the column name for a feature to its
             config.
         shuffle_data: Whether to shuffle the data before splitting it into train,
             validation, and test sets.
         drop_empty_percentage: Rows will be dropped if they are this percentage empty.
         dataset_split: The split of the dataset into train, validation, and test sets.
     """
 
-    id: int = Field(...)
-    pipeline_config_uuid: Optional[str] = None
+    id: Optional[int] = None
+    uuid: Optional[str] = None
     target: str = Field(...)
     target_type: TargetType = Field(...)
     primary_metric: Metric = Field(...)
     feature_configs: Dict[
-        str, Union[NumericalFeatureConfig, CategoricalFeatureConfig]
+        str, Union[CategoricalFeatureConfig, NumericalFeatureConfig]
     ] = Field(...)
     shuffle_data: bool = Field(...)
     drop_empty_percentage: int = Field(...)
     dataset_split: DatasetSplit = Field(...)
```

### Comparing `sotai-0.1.0/sotai.egg-info/PKG-INFO` & `sotai-0.2.0/sotai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
@@ -22,41 +22,45 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">SOTAI</h1>
 
-<p align='center'>
-<a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
-<a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml" ><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
+<p align="center">
+  <a href="https://pypi.org/project/sotai/"><img src="https://img.shields.io/pypi/v/sotai" /></a>
+  <a href="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml"><img src="https://github.com/SOTAI-Labs/sotai/actions/workflows/tests.yml/badge.svg?branch=main" /></a>
 </p>
 
 A Library For Interpretable Machine Learning. This library is a PyTorch implementation of modeling techniques found in [Monotonic Calibrated Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-243.pdf).
 
-Installling the package:
+Installing the package:
 
 ```shell
 pip install sotai
 ```
 
 Importing the package:
 
 ```python
 import sotai
 ```
 
+## SOTAI SDK Documentation
+
+You can find documentation for this SDK at [https://docs.sotai.ai/sdk](https://docs.sotai.ai/sdk) or in the repo [docs folder](./).
+
 ## SOTAI Web-App User Documentation
 
 You can find documentation for how to use the hosted web-app at [https://docs.sotai.ai/app](https://docs.sotai.ai/app)
 
 ## Contribution Guidelines
 
-See the guide on [contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
+See the guide on [contributing](CONTRIBUTING.md) for full details on how to contribute to the library. For any feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/sotai/issues).
 
 ## Examples
 
 For detailed examples on how to use the library, see [examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples).
 
 ## License
 
-[MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+[MIT](../LICENSE/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sotai Version: 0.1.0 Summary: A Python Library For
+Metadata-Version: 2.1 Name: sotai Version: 0.2.0 Summary: A Python Library For
 Calibrated Modeling Built With PyTorch Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: MIT Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-
 calibrated/issues Project-URL: Bug Reports, https://github.com/SOTAI-Labs/
 pytorch-calibrated/issues Classifier: Development Status :: 5 - Production/
@@ -17,17 +17,18 @@
 markdown License-File: LICENSE
                               ****** SOTAI ******
   [https://img.shields.io/pypi/v/sotai] [https://github.com/SOTAI-Labs/sotai/
               actions/workflows/tests.yml/badge.svg?branch=main]
 A Library For Interpretable Machine Learning. This library is a PyTorch
 implementation of modeling techniques found in [Monotonic Calibrated
 Interpolated Look-Up Tables](https://jmlr.org/papers/volume17/15-243/15-
-243.pdf). Installling the package: ```shell pip install sotai ``` Importing the
-package: ```python import sotai ``` ## SOTAI Web-App User Documentation You can
-find documentation for how to use the hosted web-app at [https://docs.sotai.ai/
-app](https://docs.sotai.ai/app) ## Contribution Guidelines See the guide on
-[contributing](https://github.com/SOTAI-Labs/sotai/blob/main/docs/
-CONTRIBUTING.md) for full details on how to contribute to the library. For any
-feature and/or bug requests, visit our [Issues](https://github.com/SOTAI-Labs/
-sotai/issues). ## Examples For detailed examples on how to use the library, see
-[examples](https://github.com/SOTAI-Labs/sotai/tree/main/docs/examples). ##
-License [MIT](https://github.com/SOTAI-Labs/sotai/blob/main/LICENSE)
+243.pdf). Installing the package: ```shell pip install sotai ``` Importing the
+package: ```python import sotai ``` ## SOTAI SDK Documentation You can find
+documentation for this SDK at [https://docs.sotai.ai/sdk](https://
+docs.sotai.ai/sdk) or in the repo [docs folder](./). ## SOTAI Web-App User
+Documentation You can find documentation for how to use the hosted web-app at
+[https://docs.sotai.ai/app](https://docs.sotai.ai/app) ## Contribution
+Guidelines See the guide on [contributing](CONTRIBUTING.md) for full details on
+how to contribute to the library. For any feature and/or bug requests, visit
+our [Issues](https://github.com/SOTAI-Labs/sotai/issues). ## Examples For
+detailed examples on how to use the library, see [examples](https://github.com/
+SOTAI-Labs/sotai/tree/main/docs/examples). ## License [MIT](../LICENSE/)
```

### Comparing `sotai-0.1.0/sotai.egg-info/SOURCES.txt` & `sotai-0.2.0/sotai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sotai-0.1.0/tests/test_data.py` & `sotai-0.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.1.0/tests/test_features.py` & `sotai-0.2.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.1.0/tests/test_models.py` & `sotai-0.2.0/tests/test_models.py`

 * *Files identical despite different names*

