# Comparing `tmp/pht_train_container_library-2.0.6.tar.gz` & `tmp/pht_train_container_library-2.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht_train_container_library-2.0.6.tar", max compression
+gzip compressed data, was "pht_train_container_library-2.0.6a0.tar", max compression
```

## Comparing `pht_train_container_library-2.0.6.tar` & `pht_train_container_library-2.0.6a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1088 2023-01-19 10:45:16.949660 pht_train_container_library-2.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1953 2023-07-17 15:17:59.071683 pht_train_container_library-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     5993 2023-03-07 13:34:10.507960 pht_train_container_library-2.0.6/README.md
--rw-r--r--   0        0        0        0 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/__init__.py
--rw-r--r--   0        0        0       33 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/__init__.py
--rw-r--r--   0        0        0      109 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/__init__.py
--rw-r--r--   0        0        0    20458 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_client.py
--rw-r--r--   0        0        0     2582 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_k_anonymity.py
--rw-r--r--   0        0        0     3888 2023-01-19 13:06:08.902080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_query_builder.py
--rw-r--r--   0        0        0      316 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/minimal_query.json
--rw-r--r--   0        0        0      792 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/query.json
--rw-r--r--   0        0        0       16 2023-07-11 10:20:24.151603 pht_train_container_library-2.0.6/train_lib/docker_util/__init__.py
--rw-r--r--   0        0        0     6389 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6/train_lib/docker_util/docker_ops.py
--rw-r--r--   0        0        0     7974 2023-07-11 10:20:24.152601 pht_train_container_library-2.0.6/train_lib/docker_util/validate_master_image.py
--rw-r--r--   0        0        0        2 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/__init__.py
--rw-r--r--   0        0        0      270 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6/train_lib/security/constants.py
--rw-r--r--   0        0        0     4571 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/encryption.py
--rw-r--r--   0        0        0      260 2023-01-19 13:06:08.903078 pht_train_container_library-2.0.6/train_lib/security/errors.py
--rw-r--r--   0        0        0     2625 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/hashing.py
--rw-r--r--   0        0        0     1549 2023-01-19 13:06:08.904079 pht_train_container_library-2.0.6/train_lib/security/homomorphic_addition.py
--rw-r--r--   0        0        0     6510 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6/train_lib/security/key_manager.py
--rw-r--r--   0        0        0     1864 2023-01-19 13:06:08.905079 pht_train_container_library-2.0.6/train_lib/security/primes.py
--rw-r--r--   0        0        0    33074 2023-06-29 07:40:07.174064 pht_train_container_library-2.0.6/train_lib/security/protocol.py
--rw-r--r--   0        0        0     2737 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6/train_lib/security/train_config.py
--rw-r--r--   0        0        0    10240 2023-02-09 14:34:23.633115 pht_train_container_library-2.0.6/train_lib/tests/archive.tar
--rw-r--r--   0        0        0    11881 2023-03-30 15:16:38.353625 pht_train_container_library-2.0.6/train_lib/tests/conftest.py
--rw-r--r--   0        0        0    10976 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6/train_lib/tests/test_fhir_functionality.py
--rw-r--r--   0        0        0     2522 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6/train_lib/tests/test_homomorphic_addition.py
--rw-r--r--   0        0        0      119 2023-01-19 13:06:08.906589 pht_train_container_library-2.0.6/train_lib/tests/test_key_manager.py
--rw-r--r--   0        0        0     5303 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6/train_lib/tests/test_security_functions.py
--rw-r--r--   0        0        0    24163 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6/train_lib/tests/test_security_protocol.py
--rw-r--r--   0        0        0     8373 2023-07-11 10:20:24.152601 pht_train_container_library-2.0.6/train_lib/tests/test_validate_master_image.py
--rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6/setup.py
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-19 10:45:16.949660 pht_train_container_library-2.0.6a0/LICENSE.txt
+-rw-r--r--   0        0        0     1955 2023-07-17 18:01:39.294063 pht_train_container_library-2.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0     5993 2023-03-07 13:34:10.507960 pht_train_container_library-2.0.6a0/README.md
+-rw-r--r--   0        0        0        0 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6a0/train_lib/__init__.py
+-rw-r--r--   0        0        0       33 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6a0/train_lib/clients/__init__.py
+-rw-r--r--   0        0        0      109 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/__init__.py
+-rw-r--r--   0        0        0    20458 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_client.py
+-rw-r--r--   0        0        0     2582 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_k_anonymity.py
+-rw-r--r--   0        0        0     3888 2023-01-19 13:06:08.902080 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_query_builder.py
+-rw-r--r--   0        0        0      316 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/minimal_query.json
+-rw-r--r--   0        0        0      792 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6a0/train_lib/clients/fhir/query.json
+-rw-r--r--   0        0        0       16 2023-07-11 10:20:24.151603 pht_train_container_library-2.0.6a0/train_lib/docker_util/__init__.py
+-rw-r--r--   0        0        0     6389 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6a0/train_lib/docker_util/docker_ops.py
+-rw-r--r--   0        0        0     8085 2023-07-17 17:58:27.385896 pht_train_container_library-2.0.6a0/train_lib/docker_util/validate_master_image.py
+-rw-r--r--   0        0        0        2 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6a0/train_lib/security/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6a0/train_lib/security/constants.py
+-rw-r--r--   0        0        0     4571 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6a0/train_lib/security/encryption.py
+-rw-r--r--   0        0        0      260 2023-01-19 13:06:08.903078 pht_train_container_library-2.0.6a0/train_lib/security/errors.py
+-rw-r--r--   0        0        0     2625 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6a0/train_lib/security/hashing.py
+-rw-r--r--   0        0        0     1549 2023-01-19 13:06:08.904079 pht_train_container_library-2.0.6a0/train_lib/security/homomorphic_addition.py
+-rw-r--r--   0        0        0     6510 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6a0/train_lib/security/key_manager.py
+-rw-r--r--   0        0        0     1864 2023-01-19 13:06:08.905079 pht_train_container_library-2.0.6a0/train_lib/security/primes.py
+-rw-r--r--   0        0        0    33074 2023-06-29 07:40:07.174064 pht_train_container_library-2.0.6a0/train_lib/security/protocol.py
+-rw-r--r--   0        0        0     2737 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6a0/train_lib/security/train_config.py
+-rw-r--r--   0        0        0    10240 2023-02-09 14:34:23.633115 pht_train_container_library-2.0.6a0/train_lib/tests/archive.tar
+-rw-r--r--   0        0        0    11881 2023-03-30 15:16:38.353625 pht_train_container_library-2.0.6a0/train_lib/tests/conftest.py
+-rw-r--r--   0        0        0    10976 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6a0/train_lib/tests/test_fhir_functionality.py
+-rw-r--r--   0        0        0     2522 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6a0/train_lib/tests/test_homomorphic_addition.py
+-rw-r--r--   0        0        0      119 2023-01-19 13:06:08.906589 pht_train_container_library-2.0.6a0/train_lib/tests/test_key_manager.py
+-rw-r--r--   0        0        0     5303 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6a0/train_lib/tests/test_security_functions.py
+-rw-r--r--   0        0        0    24163 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6a0/train_lib/tests/test_security_protocol.py
+-rw-r--r--   0        0        0     8373 2023-07-11 10:20:24.152601 pht_train_container_library-2.0.6a0/train_lib/tests/test_validate_master_image.py
+-rw-r--r--   0        0        0     6876 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6a0/setup.py
+-rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6a0/PKG-INFO
```

### Comparing `pht_train_container_library-2.0.6/LICENSE.txt` & `pht_train_container_library-2.0.6a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/pyproject.toml` & `pht_train_container_library-2.0.6a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pht-train-container-library"
-version = "2.0.6"
+version = "2.0.6a0"
 description = "Python library for handling containerized PHT trains"
 authors = ["Michael Graf <michael.graf@uni-tuebingen.com>"]
 readme = "README.md"
 packages = [{include = "train_lib"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pht_train_container_library-2.0.6/README.md` & `pht_train_container_library-2.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_client.py` & `pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_client.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_k_anonymity.py` & `pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_query_builder.py` & `pht_train_container_library-2.0.6a0/train_lib/clients/fhir/fhir_query_builder.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/clients/fhir/query.json` & `pht_train_container_library-2.0.6a0/train_lib/clients/fhir/query.json`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/docker_util/docker_ops.py` & `pht_train_container_library-2.0.6a0/train_lib/docker_util/docker_ops.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/docker_util/validate_master_image.py` & `pht_train_container_library-2.0.6a0/train_lib/docker_util/validate_master_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import hashlib
-import multiprocessing as mp
 import tarfile
 from io import BytesIO
 
 import docker
 from train_lib.docker_util import TIMEOUT
 
 # statically define files and directories which shall be exempt from hash file comparison
@@ -123,25 +122,29 @@
             if n.endswith("/layer.tar"):
                 layer_file = outer.extractfile(n)
                 if layer_file is not None:
                     bytes_arr = bytearray()
                     bytes_arr.extend(layer_file.read())
                     layer_tars.append((bytes_arr, path_exceptions))
 
-        # init and execute (a)synchronous multiprocessing for hashing function
-        pool = mp.Pool(num_cpus) if num_cpus != -1 else mp.Pool(mp.cpu_count())
-        # results = []
-        # def collect_result(result):
-        #     global results
-        #     results.append(result)
-        # pool.map_async(_apply_hash_function_to_layers, layers, callback=collect_result)
-        results = pool.map(_apply_hash_function_to_layers, layer_tars)
-        pool.close()
+        # # init and execute (a)synchronous multiprocessing for hashing function #TODO
+        # pool = mp.Pool(num_cpus) if num_cpus != -1 else mp.Pool(mp.cpu_count())
+        # # results = []
+        # # def collect_result(result):
+        # #     global results
+        # #     results.append(result)
+        # # pool.map_async(_apply_hash_function_to_layers, layers, callback=collect_result)
+        # results = pool.map(_apply_hash_function_to_layers, layer_tars)
+        # pool.close()
         # pool.join()
 
+        results = [
+            _apply_hash_function_to_layers(layer_tar) for layer_tar in layer_tars
+        ]
+
         # aggregate multiprocessing results
         for result in results:
             # integrate hash results into full image hash
             for path in result.keys():
                 hashes = [] if path not in image_hashes.keys() else image_hashes[path]
                 hashes.extend(result[path])
                 image_hashes[path] = sorted([h for h in hashes if h])
```

### Comparing `pht_train_container_library-2.0.6/train_lib/security/encryption.py` & `pht_train_container_library-2.0.6a0/train_lib/security/encryption.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/hashing.py` & `pht_train_container_library-2.0.6a0/train_lib/security/hashing.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/homomorphic_addition.py` & `pht_train_container_library-2.0.6a0/train_lib/security/homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/key_manager.py` & `pht_train_container_library-2.0.6a0/train_lib/security/key_manager.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/primes.py` & `pht_train_container_library-2.0.6a0/train_lib/security/primes.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/protocol.py` & `pht_train_container_library-2.0.6a0/train_lib/security/protocol.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/security/train_config.py` & `pht_train_container_library-2.0.6a0/train_lib/security/train_config.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/archive.tar` & `pht_train_container_library-2.0.6a0/train_lib/tests/archive.tar`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/conftest.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/test_fhir_functionality.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/test_fhir_functionality.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/test_homomorphic_addition.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/test_homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/test_security_functions.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/test_security_functions.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/test_security_protocol.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/test_security_protocol.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/train_lib/tests/test_validate_master_image.py` & `pht_train_container_library-2.0.6a0/train_lib/tests/test_validate_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.6/setup.py` & `pht_train_container_library-2.0.6a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pandas',
  'pendulum',
  'requests',
  'requests_oauthlib']
 
 setup_kwargs = {
     'name': 'pht-train-container-library',
-    'version': '2.0.6',
+    'version': '2.0.6a0',
     'description': 'Python library for handling containerized PHT trains',
     'long_description': "[![Documentation Status](https://readthedocs.org/projects/train-container-library/badge/?version=latest)](https://train-container-library.readthedocs.io/en/latest/?badge=latest)\n[![CodeQL](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml)\n[![main-ci](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml/badge.svg)](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/PHT-Medic/train-container-library/branch/master/graph/badge.svg?token=11RYRZK2FO)](https://codecov.io/gh/PHT-Medic/train-container-library)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pht-train-container-library)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/pht-train-container-library)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# &#128646; Train Container Library\n\nPython library for validating and interacting with pht-train images/containers.\n\n## Installation\n\n```shell\npip install pht-train-container-library\n```\n\n\n## Setup development environment\nMake sure you have [poetry](https://python-poetry.org/docs/#installation) and [pre-commit](https://pre-commit.com/#install) installed.\n\nInstall the dependencies and pre-commit hooks:\n```shell\npoetry install --with dev\n```\n\n```shell\npoetry run pre-commit install\n```\n\n### Run tests\n\n```shell\npoetry run pytest\n```\n\n### Linting and formatting\n\nThese commands are also run as pre-commit hooks.\n\nLinting with ruff:\n```shell\npoetry run ruff . --fix\n```\n\nFormatting with black:\n```shell\npoetry run black .\n```\n\n## Security Protocol\n\nThe pht security protocol adapted from `docs/Secure_PHT_latest__official.pdf` performs two main tasks:\n\n1. Before executing a train-image on the local machine, unless the station is the first station on the route, the\n   previous results need to be decrypted and the content of the image needs to be validated based on the configuration\n   of the individual train -> `pre-run`.\n2. After executing the train the updated results need to be encrypted and the train configuration needs to be updated to\n   reflect the current state ->`post-run`.\n\n### Train image structure\n\nTo ensure the protocol is working correctly train docker images are required to keep the following structure:\n\n- `/opt/train_config.json`: Stores the configuration file of the train.\n- `/opt/pht_train/`: Stores all the files containing code or other things required for the train algorithm to run. The\n  contents of this directory can never change and is validated by the `pre-run` step.\n- `/opt/pht_results/`: Stores the results of the train. Which will be decrypted in the `pre-run` step and encrypted in\n  the `post-run` step.\n\nNo files in the image outside the `/opt/pht_results/` directory should change during the execution of the algorithm.\n\n### Usage - Python Script\n\nTo use the protocol in your own python application, after installing the library\nwith `pip install pht-train-container-library` an instance of the protocol can be to validate docker images as follows:\n\n```python\nfrom train_lib.security.protocol import SecurityProtocol\nfrom train_lib.docker_util.docker_ops import extract_train_config\n\nimage_name = '<image-repo>:<image-tag>'\nstation_id = '<station-id>'\n\n# Get the train configuration from the image\nconfig = extract_train_config(image_name)\n# Initialize the protocol with the extracted config and station_id\nprotocol = SecurityProtocol(station_id=station_id, config=config)\n\n# execute one of the protocol steps\nprotocol.pre_run_protocol(image_name, private_key_path='<path-to-private-key>')\n# protocol.post_run_protocol(image_name, private_key_path='<path-to-private-key>')\n```\n\n### Usage - Container\n\nA containerized version of the protocol is also available it can be used with the following command:\n\n```shell\ndocker run -e STATION_ID=<station_id> -e PRIVATE_KEY_PATH=/opt/private_key.pem -v /var/run/docker.sock:/var/run/docker.sock -v <path_to_your_key>:/opt/private_key.pem ghcr.io/pht-medic/protocol <pre-run/post-run> <image-repo>:<image-tag>\n```\n\n`STATION_ID` and `PRIVATE_KEY_PATH` are required to be set in the environment variables. As well as passing the docker\nsocket `/var/run/docker.sock` to the container as a volume to enable docker-in-docker functionality.\n\n### Pre-run protocol\n\nThe pre-run protocol consists of the following steps\n\n1. The hash of the immutable files (train definition) is verified making sure that the executable files did not change\n   during the the train definition.\n2. The digital signature is verified ensuring the correctness of the results at each stop of the train.\n3. The symmetric key is decrypted using the provided station private key\n4. The mutable files in `/opt/pht_results` are decrypted using the symmetric key obtained in the previous step\n5. The decrypted files are hashed and the hash is compared to the one stored in the train configuration file.\n\nOnce these steps have been completed the image is ready to be executed.\n\n### Post-run protocol\n\n1. Calculate the hash of the newly generated results\n2. Sign the hash of the results using the provided `PRIVATE_KEY_PATH`\n3. Update the the train signature using the session id that is randomly generated at each execution step\n4. Encrypt the resulting files using a newly generated symmetric key\n5. Encrypt the generated symmetric key with the public keys of the train participants\n6. Update the train configuration file\n\nWith the completion of these steps the train is ready to be pushed into the registry for further processing\n\n## Tests\n\nRun the tests to validate the security protocol is working as intended. From this projects root directory run\n`pytest train_lib`\n\n\n\n\n\n\n\n",
     'author': 'Michael Graf',
     'author_email': 'michael.graf@uni-tuebingen.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pht_train_container_library-2.0.6/PKG-INFO` & `pht_train_container_library-2.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pht-train-container-library
-Version: 2.0.6
+Version: 2.0.6a0
 Summary: Python library for handling containerized PHT trains
 Author: Michael Graf
 Author-email: michael.graf@uni-tuebingen.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

