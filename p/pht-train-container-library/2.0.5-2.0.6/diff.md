# Comparing `tmp/pht_train_container_library-2.0.5.tar.gz` & `tmp/pht_train_container_library-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht_train_container_library-2.0.5.tar", max compression
+gzip compressed data, was "pht_train_container_library-2.0.6.tar", max compression
```

## Comparing `pht_train_container_library-2.0.5.tar` & `pht_train_container_library-2.0.6.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1068 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/LICENSE.txt
--rw-r--r--   0        0        0     5852 2023-03-07 12:16:53.453164 pht_train_container_library-2.0.5/README.md
--rw-r--r--   0        0        0     1848 2023-04-17 18:07:22.070677 pht_train_container_library-2.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/__init__.py
--rw-r--r--   0        0        0       32 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/__init__.py
--rw-r--r--   0        0        0      107 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/__init__.py
--rw-r--r--   0        0        0    19926 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_client.py
--rw-r--r--   0        0        0     2509 2023-03-07 12:14:19.038419 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_k_anonymity.py
--rw-r--r--   0        0        0     3788 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_query_builder.py
--rw-r--r--   0        0        0      297 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/minimal_query.json
--rw-r--r--   0        0        0      758 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/query.json
--rw-r--r--   0        0        0       14 2023-04-12 10:34:43.891083 pht_train_container_library-2.0.5/train_lib/docker_util/__init__.py
--rw-r--r--   0        0        0     6213 2023-04-17 18:05:04.947429 pht_train_container_library-2.0.5/train_lib/docker_util/docker_ops.py
--rw-r--r--   0        0        0     6219 2023-03-30 14:41:16.691214 pht_train_container_library-2.0.5/train_lib/docker_util/validate_master_image.py
--rw-r--r--   0        0        0        1 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/__init__.py
--rw-r--r--   0        0        0      257 2023-04-12 13:21:36.885381 pht_train_container_library-2.0.5/train_lib/security/constants.py
--rw-r--r--   0        0        0     4436 2023-03-07 12:17:00.953436 pht_train_container_library-2.0.5/train_lib/security/encryption.py
--rw-r--r--   0        0        0      248 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/errors.py
--rw-r--r--   0        0        0     2543 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.5/train_lib/security/hashing.py
--rw-r--r--   0        0        0     1483 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/homomorphic_addition.py
--rw-r--r--   0        0        0     6336 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.5/train_lib/security/key_manager.py
--rw-r--r--   0        0        0     1772 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/primes.py
--rw-r--r--   0        0        0    32244 2023-04-12 12:11:47.497039 pht_train_container_library-2.0.5/train_lib/security/protocol.py
--rw-r--r--   0        0        0     2628 2023-03-07 12:41:46.414956 pht_train_container_library-2.0.5/train_lib/security/train_config.py
--rw-r--r--   0        0        0    11507 2023-03-30 14:41:16.301214 pht_train_container_library-2.0.5/train_lib/tests/conftest.py
--rw-r--r--   0        0        0    10607 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_fhir_functionality.py
--rw-r--r--   0        0        0     2425 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_homomorphic_addition.py
--rw-r--r--   0        0        0      116 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_key_manager.py
--rw-r--r--   0        0        0     5127 2023-03-07 12:17:04.923592 pht_train_container_library-2.0.5/train_lib/tests/test_security_functions.py
--rw-r--r--   0        0        0    23503 2023-03-07 12:17:05.793630 pht_train_container_library-2.0.5/train_lib/tests/test_security_protocol.py
--rw-r--r--   0        0        0     7602 2023-03-27 15:40:16.372314 pht_train_container_library-2.0.5/train_lib/tests/test_validate_master_image.py
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-19 10:45:16.949660 pht_train_container_library-2.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1953 2023-07-17 15:17:59.071683 pht_train_container_library-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5993 2023-03-07 13:34:10.507960 pht_train_container_library-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/__init__.py
+-rw-r--r--   0        0        0       33 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/__init__.py
+-rw-r--r--   0        0        0      109 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/__init__.py
+-rw-r--r--   0        0        0    20458 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_client.py
+-rw-r--r--   0        0        0     2582 2023-01-19 13:06:08.901080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_k_anonymity.py
+-rw-r--r--   0        0        0     3888 2023-01-19 13:06:08.902080 pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_query_builder.py
+-rw-r--r--   0        0        0      316 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/minimal_query.json
+-rw-r--r--   0        0        0      792 2023-01-19 10:45:16.961671 pht_train_container_library-2.0.6/train_lib/clients/fhir/query.json
+-rw-r--r--   0        0        0       16 2023-07-11 10:20:24.151603 pht_train_container_library-2.0.6/train_lib/docker_util/__init__.py
+-rw-r--r--   0        0        0     6389 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6/train_lib/docker_util/docker_ops.py
+-rw-r--r--   0        0        0     7974 2023-07-11 10:20:24.152601 pht_train_container_library-2.0.6/train_lib/docker_util/validate_master_image.py
+-rw-r--r--   0        0        0        2 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-29 07:40:07.173064 pht_train_container_library-2.0.6/train_lib/security/constants.py
+-rw-r--r--   0        0        0     4571 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/encryption.py
+-rw-r--r--   0        0        0      260 2023-01-19 13:06:08.903078 pht_train_container_library-2.0.6/train_lib/security/errors.py
+-rw-r--r--   0        0        0     2625 2023-03-07 13:34:10.513963 pht_train_container_library-2.0.6/train_lib/security/hashing.py
+-rw-r--r--   0        0        0     1549 2023-01-19 13:06:08.904079 pht_train_container_library-2.0.6/train_lib/security/homomorphic_addition.py
+-rw-r--r--   0        0        0     6510 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6/train_lib/security/key_manager.py
+-rw-r--r--   0        0        0     1864 2023-01-19 13:06:08.905079 pht_train_container_library-2.0.6/train_lib/security/primes.py
+-rw-r--r--   0        0        0    33074 2023-06-29 07:40:07.174064 pht_train_container_library-2.0.6/train_lib/security/protocol.py
+-rw-r--r--   0        0        0     2737 2023-03-07 13:34:10.514964 pht_train_container_library-2.0.6/train_lib/security/train_config.py
+-rw-r--r--   0        0        0    10240 2023-02-09 14:34:23.633115 pht_train_container_library-2.0.6/train_lib/tests/archive.tar
+-rw-r--r--   0        0        0    11881 2023-03-30 15:16:38.353625 pht_train_container_library-2.0.6/train_lib/tests/conftest.py
+-rw-r--r--   0        0        0    10976 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6/train_lib/tests/test_fhir_functionality.py
+-rw-r--r--   0        0        0     2522 2023-01-19 13:06:08.905584 pht_train_container_library-2.0.6/train_lib/tests/test_homomorphic_addition.py
+-rw-r--r--   0        0        0      119 2023-01-19 13:06:08.906589 pht_train_container_library-2.0.6/train_lib/tests/test_key_manager.py
+-rw-r--r--   0        0        0     5303 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6/train_lib/tests/test_security_functions.py
+-rw-r--r--   0        0        0    24163 2023-03-07 13:34:10.515970 pht_train_container_library-2.0.6/train_lib/tests/test_security_protocol.py
+-rw-r--r--   0        0        0     8373 2023-07-11 10:20:24.152601 pht_train_container_library-2.0.6/train_lib/tests/test_validate_master_image.py
+-rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6/setup.py
+-rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.6/PKG-INFO
```

### Comparing `pht_train_container_library-2.0.5/LICENSE.txt` & `pht_train_container_library-2.0.6/LICENSE.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2020] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [2020] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pht_train_container_library-2.0.5/README.md` & `pht_train_container_library-2.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pht-train-container-library
+Version: 2.0.6
+Summary: Python library for handling containerized PHT trains
+Author: Michael Graf
+Author-email: michael.graf@uni-tuebingen.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography
+Requires-Dist: docker
+Requires-Dist: fhir-kindling
+Requires-Dist: loguru
+Requires-Dist: pandas
+Requires-Dist: pendulum
+Requires-Dist: requests
+Requires-Dist: requests_oauthlib
+Description-Content-Type: text/markdown
+
 [![Documentation Status](https://readthedocs.org/projects/train-container-library/badge/?version=latest)](https://train-container-library.readthedocs.io/en/latest/?badge=latest)
 [![CodeQL](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml)
 [![main-ci](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml/badge.svg)](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/PHT-Medic/train-container-library/branch/master/graph/badge.svg?token=11RYRZK2FO)](https://codecov.io/gh/PHT-Medic/train-container-library)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pht-train-container-library)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/pht-train-container-library)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -135,7 +157,8 @@
 
 
 
 
 
 
 
+
```

### Comparing `pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_client.py` & `pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_client.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,532 +1,532 @@
-import collections
-import json
-import os
-from io import BytesIO
-from typing import List, Union
-
-import pandas as pd
-import requests
-import xmltodict
-from loguru import logger
-from oauthlib.oauth2 import BackendApplicationClient
-from requests.auth import HTTPBasicAuth
-from requests_oauthlib import OAuth2Session
-
-from .fhir_query_builder import build_query_string
-
-
-class PHTFhirClient:
-    def __init__(
-        self,
-        server_url: str = None,
-        username: str = None,
-        password: str = None,
-        token: str = None,
-        client_id: str = None,
-        client_secret: str = None,
-        oidc_provider_url: str = None,
-        fhir_server_type: str = None,
-        disable_auth: bool = False,
-        k_anon: int = 5,
-        disable_k_anon: bool = False,
-    ):
-        """
-        Fhir client for executing predefined queries contained in PHT trains. Supports IBM, Blaze, and HAPI FHIR servers
-
-        :param server_url: base url of the FHIR server to execute the query against
-        :param username: username for use in basic auth authentication against the fhir server
-        :param password: password for use in basic auth
-        :param token: token to use for authenticating against a FHIR server using a static bearer token
-        :param client_id: client id for OIDC authentication flow
-        :param client_secret: secret for OIDC authentication flow
-        :param oidc_provider_url: url where a token can be obtained using client_id and client_secret
-        :param fhir_server_type: the type of the server one of ["blaze", "hapi", "ibm"]
-        """
-        self.server_url = server_url if server_url else os.getenv("FHIR_SERVER_URL")
-        if not self.server_url[-1] == "/":
-            self.server_url = self.server_url + "/"
-        self.username = username
-        self.password = password
-        self.token = token
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.oidc_provider_url = oidc_provider_url
-
-        self.fhir_server_type = (
-            fhir_server_type if fhir_server_type else os.getenv("FHIR_SERVER_TYPE")
-        )
-        self.output_format = None
-        self.disable_auth = disable_auth
-        self.disable_k_anon = disable_k_anon
-        self.k_anon = k_anon
-
-        # Check for correct initialization based on env vars or constructor parameters
-        if (self.username and self.password) and self.token:
-            raise ValueError("Only one of username:pw or token auth can be selected")
-        if not ((self.username and self.password) or self.token) and disable_auth:
-            raise ValueError(
-                "Insufficient login information, either token or username and password need to be set."
-            )
-        if not self.server_url:
-            raise ValueError("No FHIR server address given.")
-
-    @classmethod
-    def from_dict(cls, fhir_config: dict):
-        # attempt to find the API address from the different options for environtment variables
-        api_url = fhir_config.get(
-            "FHIR_SERVER_URL", os.getenv("FHIR_ADDRESS", os.getenv("FHIR_API_URL"))
-        )
-        if not api_url:
-            raise EnvironmentError(
-                "No FHIR Address could be found in the clients environment variables."
-            )
-
-        server_type = fhir_config.get("FHIR_SERVER_TYPE", "blaze")
-
-        # attempt to load basic auth information
-        username = fhir_config.get("FHIR_USER")
-        if username:
-            password = fhir_config.get("FHIR_PW")
-            if not password:
-                raise EnvironmentError(
-                    "Username given but no password found in environment variables."
-                )
-
-            return cls(
-                server_url=api_url,
-                username=username,
-                password=password,
-                fhir_server_type=server_type,
-            )
-
-        token = fhir_config.get("FHIR_TOKEN")
-        if username and token:
-            raise EnvironmentError(
-                "Conflicting auth information: both username and token are set."
-            )
-
-        if token:
-            return cls(server_url=api_url, token=token, fhir_server_type=server_type)
-
-        client_id = fhir_config.get("CLIENT_ID")
-        client_secret = fhir_config.get("CLIENT_SECRET")
-        oidc_provider = fhir_config.get("OIDC_PROVIDER_URL")
-
-        if username and client_id:
-            raise EnvironmentError(
-                "Conflicting auth information: both username and client id are set."
-            )
-
-        if token and client_id:
-            raise EnvironmentError(
-                "Conflicting auth information: both token and client id are set."
-            )
-
-        if client_id:
-            if not client_secret:
-                raise EnvironmentError(
-                    "No client secret set for oauth2 authentication flow."
-                )
-            if not oidc_provider:
-                raise EnvironmentError(
-                    "No provider URL given for oauth2 authentication flow."
-                )
-
-            return cls(
-                server_url=api_url,
-                client_id=client_id,
-                client_secret=client_secret,
-                oidc_provider_url=oidc_provider,
-                fhir_server_type=server_type,
-            )
-
-        logger.info("No authentication info given, attempting access without it.")
-        return cls(server_url=api_url, fhir_server_type=server_type, disable_auth=True)
-
-    @classmethod
-    def from_env(cls):
-        """
-        Initialize a client instance from environment variables.
-
-        :return: an instance of the fhir client
-        """
-
-        # attempt to find the API address from the different options for environtment variables
-        api_url = os.getenv(
-            "FHIR_SERVER_URL", os.getenv("FHIR_ADDRESS", os.getenv("FHIR_API_URL"))
-        )
-        if not api_url:
-            raise EnvironmentError(
-                "No FHIR Address could be found in the clients environment variables."
-            )
-
-        server_type = os.getenv("FHIR_SERVER_TYPE", "blaze")
-
-        # attempt to load basic auth information
-        username = os.getenv("FHIR_USER")
-        if username:
-            password = os.getenv("FHIR_PW")
-            if not password:
-                raise EnvironmentError(
-                    "Username given but no password found in environment variables."
-                )
-
-            return cls(
-                server_url=api_url,
-                username=username,
-                password=password,
-                fhir_server_type=server_type,
-            )
-
-        token = os.getenv("FHIR_TOKEN")
-        if username and token:
-            raise EnvironmentError(
-                "Conflicting auth information: both username and token are set."
-            )
-
-        if token:
-            return cls(server_url=api_url, token=token, fhir_server_type=server_type)
-
-        client_id = os.getenv("CLIENT_ID")
-        client_secret = os.getenv("CLIENT_SECRET")
-        oidc_provider = os.getenv("OIDC_PROVIDER_URL")
-
-        if username and client_id:
-            raise EnvironmentError(
-                "Conflicting auth information: both username and client id are set."
-            )
-
-        if token and client_id:
-            raise EnvironmentError(
-                "Conflicting auth information: both token and client id are set."
-            )
-
-        if client_id:
-            if not client_secret:
-                raise EnvironmentError(
-                    "No client secret set for oauth2 authentication flow."
-                )
-            if not oidc_provider:
-                raise EnvironmentError(
-                    "No provider URL given for oauth2 authentication flow."
-                )
-
-            return cls(
-                server_url=api_url,
-                client_id=client_id,
-                client_secret=client_secret,
-                oidc_provider_url=oidc_provider,
-                fhir_server_type=server_type,
-            )
-
-        logger.info("No authentication info given, attempting access without it.")
-        return cls(server_url=api_url, fhir_server_type=server_type, disable_auth=True)
-
-    def execute_query(
-        self,
-        query_file: Union[str, os.PathLike, BytesIO] = None,
-        query: dict = None,
-        store_results: bool = False,
-    ) -> pd.DataFrame:
-        """
-        Asynchronously build the query string and execute it against the given fhir server either based on a query.json
-        file or based on a dictionary containing the query file content.
-        :param query_file: definition of the query given in json format either a string, a path to a file or in memory
-        file object
-        :param query: dictionary containing query definition
-        :param store_results: where to store the results to file
-        :return:
-        """
-        if query and query_file:
-            raise ValueError("Only specify one of query file or query dictionary")
-        if query and isinstance(query, dict):
-            query_file_content = query
-        else:
-            query_file_content = self.read_query_file(query_file)
-
-        # set the output format
-        self.output_format = query_file_content["data"]["output_format"]
-        # Generate url query string and generate auth (basic)
-        url = self._generate_url(query_file_content["query"])
-        auth = self._generate_auth()
-        selected_variables = query_file_content["data"].get("variables", None)
-
-        if self.output_format == "xml":
-            query_results = self._get_query_results_from_api_xml(url, auth)
-        else:
-            query_results = self._get_query_results_from_api_json(
-                url=url, auth=auth, selected_variables=selected_variables
-            )
-
-        filename = query_file_content["data"]["filename"]
-
-        if store_results:
-            self.store_query_results(query_results, filename=filename)
-
-        return query_results
-
-    def store_query_results(
-        self, query_results, filename: str, storage_dir: str = None
-    ) -> str:
-        """
-        Store the results from the query according to the output format specified in the query file
-
-        :param query_results: The parsed or raw response from a fhir server to the given query
-        :param filename: name for the results file (defined in query.json)
-        :param storage_dir: directory in which the data should be stored
-        :return:
-        """
-
-        storage_dir = storage_dir if storage_dir else os.getenv("TRAIN_DATA_DIR")
-        if not storage_dir:
-            logger.warning(
-                "No storage directory specified, saving results to current working directory."
-            )
-            results_path = filename
-        else:
-            results_path = os.path.join(storage_dir, filename)
-
-        if self.output_format in ["raw", "json"]:
-            with open(results_path, "w") as results_file:
-                results_file.write(json.dumps(query_results, indent=2))
-
-        # write xml string to file directly
-        elif self.output_format == "xml":
-            with open(results_path, "w") as results_file:
-                results_file.write(query_results)
-
-        else:
-            raise ValueError(f"Unsupported output format: {self.output_format}")
-
-        logger.info("Stored query results in {}", results_path)
-        return results_path
-
-    def _get_query_results_from_api_json(
-        self,
-        url: str,
-        auth: requests.auth.AuthBase = None,
-        selected_variables: List[str] = None,
-        k_anonymity: int = 5,
-    ):
-        """
-        Blocking version of the querying a fhir server with the given search url. Processes all next relations in the
-        response to get the full response in a single file.
-
-        :param url:
-        :param auth:
-        :param selected_variables:
-        :param k_anonymity:
-        :return:
-        """
-
-        r = requests.get(url, auth=auth)
-        r.raise_for_status()
-
-        initial_response = r.json()
-        response = r.json()
-        print(url)
-        print(response)
-        if response.get("entry"):
-            if (len(response["entry"]) < self.k_anon) and not self.disable_k_anon:
-                raise ValueError(
-                    "Too few results match the query. Response blocked by k-anonymity policy."
-                )
-        else:
-            raise ValueError("No results match the query.")
-        link = response.get("link", None)
-        if not link:
-            return response
-        else:
-            print("Resolving response pagination")
-            entries = []
-            entries.extend(response["entry"])
-
-            while response.get("link", None):
-
-                next_page = next(
-                    (
-                        link
-                        for link in response["link"]
-                        if link.get("relation", None) == "next"
-                    ),
-                    None,
-                )
-                if next_page:
-                    response = requests.get(next_page["url"], auth=auth).json()
-                    entries.extend(response["entry"])
-                else:
-                    break
-
-            initial_response["entry"] = entries
-            return initial_response
-
-    def _get_query_results_from_api_xml(
-        self, url: str, auth: requests.auth.AuthBase = None
-    ) -> str:
-        server_response = requests.get(url, auth=auth)
-        initial_response = xmltodict.parse(server_response.text)
-        entries = initial_response["Bundle"]["entry"]
-
-        if not entries:
-            print("No results found for query")
-            return server_response.text
-
-        response = initial_response
-        while True:
-            next_page = False
-            for link in response["Bundle"]["link"]:
-                if isinstance(link, collections.OrderedDict):
-                    relation_dict = dict(link["relation"])
-                else:
-                    break
-                if relation_dict.get("@value") == "next":
-                    print("Getting next")
-                    # get url and extend with xml format
-                    url = link["url"]["@value"]
-                    url = url + "&_format=xml"
-                    r = requests.get(url, auth=auth)
-                    r.raise_for_status()
-                    response = xmltodict.parse(r.text)
-                    added_entries = response["Bundle"]["entry"]
-                    entries.extend(added_entries)
-                    # Stop resolving the pagination when the limit is reached
-                    next_page = True
-
-            if not next_page:
-                print("All pages found")
-                break
-        # added the paginated resources to the initial response
-        initial_response["Bundle"]["entry"] = entries
-
-        if (len(entries) < self.k_anon) and not self.disable_k_anon:
-            raise ValueError(
-                "Too few results match the query. Response blocked by k-anonymity policy."
-            )
-        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
-        return full_response_xml
-
-    def health_check(self):
-
-        api_url = self.server_url + "metadata"
-        auth = self._generate_auth()
-
-        r = requests.get(api_url, auth=auth)
-        r.raise_for_status()
-
-    def _process_fhir_response(
-        self, response: dict, selected_variables: List[str] = None
-    ) -> Union[pd.DataFrame, List[dict], None]:
-        """
-        Parses the fhir response into a dataframe. If selected variables are given only these are parsed from the
-        response and returned
-
-        :param response: the response data to the query from a fhir server
-        :param selected_variables: list variable names to parse from the response
-        :return:
-        """
-        entries = []
-
-        if self.output_format == "df":
-            if response.get("entry", None):
-                for entry in response["entry"]:
-                    if selected_variables:
-                        series_entry = pd.Series(entry["resource"])[selected_variables]
-                    else:
-                        series_entry = pd.Series(entry["resource"])
-                    entries.append(series_entry)
-
-                df = pd.concat(entries, axis=1)
-                df = df.T
-
-                return df
-            else:
-                return None
-
-        else:
-            return response["entry"]
-
-    @staticmethod
-    def read_query_file(file: Union[str, os.PathLike, BytesIO]) -> dict:
-        """
-        Reads the content of a query.json file either given as a path or as in memory file object
-        :param file: path to file or in memory file object to parse
-        :return: dictionary representation of the query.json file
-        """
-        if isinstance(file, BytesIO):
-            query_file = file.read()
-        else:
-            with open(file, "r") as f:
-                query_file = f.read()
-        query_file = json.loads(query_file)
-        return query_file
-
-    def _generate_url(self, query: Union[dict, list, str], limit=1000):
-        """
-        Generates the fhir search url to request from the server based. Either based on a previously given query string
-        or based on a dictionary containing the query definition in the query.json file.
-
-        :param query: dictionary containing the content of the query definition in the query.json file
-        :param query_string: Predefined Fhir url query string to append to base server url
-        :param return_format: the format in which the server should return the data.
-        :param limit: the max number of entries in a paginated response
-        :return: url string to perform a request against a fhir server with
-        """
-
-        if self.server_url[-1] == "/":
-            url = self.server_url
-        else:
-            url = self.server_url + "/"
-
-        if isinstance(query, dict):
-            url += build_query_string(query_dict=query)
-        elif isinstance(query, list):
-            url += build_query_string(query_dict=query)
-        elif isinstance(query, str):
-            url += query
-        else:
-            raise ValueError("Either query dictionary or string need to be given")
-
-        # add formatting configuration
-
-        if url[-1] == "?":
-            url += f"_format={self.output_format}&_count={limit}"
-        else:
-            url += f"&_format={self.output_format}&_count={limit}"
-
-        return url
-
-    def _generate_auth(self) -> requests.auth.AuthBase:
-        """
-        Generate authentication for the request to be sent to server. Based on a given bearer token, basic
-        auth with username and password or by requesting a new token using oauth2.
-
-        :return: Auth object to pass to a requests call.
-        """
-        if self.username and self.password:
-            logger.info("Using basic auth")
-            return HTTPBasicAuth(username=self.username, password=self.password)
-        # TODO request token from id provider if configured
-        elif self.token:
-            logger.info("Using static token auth.")
-            return BearerAuth(token=self.token)
-
-        elif self.client_id and self.client_secret and self.oidc_provider_url:
-            logger.info("Requesting oauth2 token")
-            client = BackendApplicationClient(client_id=self.client_id)
-            oauth = OAuth2Session(client=client)
-            token = oauth.fetch_token(
-                token_url=self.oidc_provider_url,
-                client_secret=self.client_secret,
-                client_id=self.client_id,
-            )
-            self.token = token["access_token"]
-            return BearerAuth(token=self.token)
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
+import collections
+import json
+import os
+from io import BytesIO
+from typing import List, Union
+
+import pandas as pd
+import requests
+import xmltodict
+from loguru import logger
+from oauthlib.oauth2 import BackendApplicationClient
+from requests.auth import HTTPBasicAuth
+from requests_oauthlib import OAuth2Session
+
+from .fhir_query_builder import build_query_string
+
+
+class PHTFhirClient:
+    def __init__(
+        self,
+        server_url: str = None,
+        username: str = None,
+        password: str = None,
+        token: str = None,
+        client_id: str = None,
+        client_secret: str = None,
+        oidc_provider_url: str = None,
+        fhir_server_type: str = None,
+        disable_auth: bool = False,
+        k_anon: int = 5,
+        disable_k_anon: bool = False,
+    ):
+        """
+        Fhir client for executing predefined queries contained in PHT trains. Supports IBM, Blaze, and HAPI FHIR servers
+
+        :param server_url: base url of the FHIR server to execute the query against
+        :param username: username for use in basic auth authentication against the fhir server
+        :param password: password for use in basic auth
+        :param token: token to use for authenticating against a FHIR server using a static bearer token
+        :param client_id: client id for OIDC authentication flow
+        :param client_secret: secret for OIDC authentication flow
+        :param oidc_provider_url: url where a token can be obtained using client_id and client_secret
+        :param fhir_server_type: the type of the server one of ["blaze", "hapi", "ibm"]
+        """
+        self.server_url = server_url if server_url else os.getenv("FHIR_SERVER_URL")
+        if not self.server_url[-1] == "/":
+            self.server_url = self.server_url + "/"
+        self.username = username
+        self.password = password
+        self.token = token
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.oidc_provider_url = oidc_provider_url
+
+        self.fhir_server_type = (
+            fhir_server_type if fhir_server_type else os.getenv("FHIR_SERVER_TYPE")
+        )
+        self.output_format = None
+        self.disable_auth = disable_auth
+        self.disable_k_anon = disable_k_anon
+        self.k_anon = k_anon
+
+        # Check for correct initialization based on env vars or constructor parameters
+        if (self.username and self.password) and self.token:
+            raise ValueError("Only one of username:pw or token auth can be selected")
+        if not ((self.username and self.password) or self.token) and disable_auth:
+            raise ValueError(
+                "Insufficient login information, either token or username and password need to be set."
+            )
+        if not self.server_url:
+            raise ValueError("No FHIR server address given.")
+
+    @classmethod
+    def from_dict(cls, fhir_config: dict):
+        # attempt to find the API address from the different options for environtment variables
+        api_url = fhir_config.get(
+            "FHIR_SERVER_URL", os.getenv("FHIR_ADDRESS", os.getenv("FHIR_API_URL"))
+        )
+        if not api_url:
+            raise EnvironmentError(
+                "No FHIR Address could be found in the clients environment variables."
+            )
+
+        server_type = fhir_config.get("FHIR_SERVER_TYPE", "blaze")
+
+        # attempt to load basic auth information
+        username = fhir_config.get("FHIR_USER")
+        if username:
+            password = fhir_config.get("FHIR_PW")
+            if not password:
+                raise EnvironmentError(
+                    "Username given but no password found in environment variables."
+                )
+
+            return cls(
+                server_url=api_url,
+                username=username,
+                password=password,
+                fhir_server_type=server_type,
+            )
+
+        token = fhir_config.get("FHIR_TOKEN")
+        if username and token:
+            raise EnvironmentError(
+                "Conflicting auth information: both username and token are set."
+            )
+
+        if token:
+            return cls(server_url=api_url, token=token, fhir_server_type=server_type)
+
+        client_id = fhir_config.get("CLIENT_ID")
+        client_secret = fhir_config.get("CLIENT_SECRET")
+        oidc_provider = fhir_config.get("OIDC_PROVIDER_URL")
+
+        if username and client_id:
+            raise EnvironmentError(
+                "Conflicting auth information: both username and client id are set."
+            )
+
+        if token and client_id:
+            raise EnvironmentError(
+                "Conflicting auth information: both token and client id are set."
+            )
+
+        if client_id:
+            if not client_secret:
+                raise EnvironmentError(
+                    "No client secret set for oauth2 authentication flow."
+                )
+            if not oidc_provider:
+                raise EnvironmentError(
+                    "No provider URL given for oauth2 authentication flow."
+                )
+
+            return cls(
+                server_url=api_url,
+                client_id=client_id,
+                client_secret=client_secret,
+                oidc_provider_url=oidc_provider,
+                fhir_server_type=server_type,
+            )
+
+        logger.info("No authentication info given, attempting access without it.")
+        return cls(server_url=api_url, fhir_server_type=server_type, disable_auth=True)
+
+    @classmethod
+    def from_env(cls):
+        """
+        Initialize a client instance from environment variables.
+
+        :return: an instance of the fhir client
+        """
+
+        # attempt to find the API address from the different options for environtment variables
+        api_url = os.getenv(
+            "FHIR_SERVER_URL", os.getenv("FHIR_ADDRESS", os.getenv("FHIR_API_URL"))
+        )
+        if not api_url:
+            raise EnvironmentError(
+                "No FHIR Address could be found in the clients environment variables."
+            )
+
+        server_type = os.getenv("FHIR_SERVER_TYPE", "blaze")
+
+        # attempt to load basic auth information
+        username = os.getenv("FHIR_USER")
+        if username:
+            password = os.getenv("FHIR_PW")
+            if not password:
+                raise EnvironmentError(
+                    "Username given but no password found in environment variables."
+                )
+
+            return cls(
+                server_url=api_url,
+                username=username,
+                password=password,
+                fhir_server_type=server_type,
+            )
+
+        token = os.getenv("FHIR_TOKEN")
+        if username and token:
+            raise EnvironmentError(
+                "Conflicting auth information: both username and token are set."
+            )
+
+        if token:
+            return cls(server_url=api_url, token=token, fhir_server_type=server_type)
+
+        client_id = os.getenv("CLIENT_ID")
+        client_secret = os.getenv("CLIENT_SECRET")
+        oidc_provider = os.getenv("OIDC_PROVIDER_URL")
+
+        if username and client_id:
+            raise EnvironmentError(
+                "Conflicting auth information: both username and client id are set."
+            )
+
+        if token and client_id:
+            raise EnvironmentError(
+                "Conflicting auth information: both token and client id are set."
+            )
+
+        if client_id:
+            if not client_secret:
+                raise EnvironmentError(
+                    "No client secret set for oauth2 authentication flow."
+                )
+            if not oidc_provider:
+                raise EnvironmentError(
+                    "No provider URL given for oauth2 authentication flow."
+                )
+
+            return cls(
+                server_url=api_url,
+                client_id=client_id,
+                client_secret=client_secret,
+                oidc_provider_url=oidc_provider,
+                fhir_server_type=server_type,
+            )
+
+        logger.info("No authentication info given, attempting access without it.")
+        return cls(server_url=api_url, fhir_server_type=server_type, disable_auth=True)
+
+    def execute_query(
+        self,
+        query_file: Union[str, os.PathLike, BytesIO] = None,
+        query: dict = None,
+        store_results: bool = False,
+    ) -> pd.DataFrame:
+        """
+        Asynchronously build the query string and execute it against the given fhir server either based on a query.json
+        file or based on a dictionary containing the query file content.
+        :param query_file: definition of the query given in json format either a string, a path to a file or in memory
+        file object
+        :param query: dictionary containing query definition
+        :param store_results: where to store the results to file
+        :return:
+        """
+        if query and query_file:
+            raise ValueError("Only specify one of query file or query dictionary")
+        if query and isinstance(query, dict):
+            query_file_content = query
+        else:
+            query_file_content = self.read_query_file(query_file)
+
+        # set the output format
+        self.output_format = query_file_content["data"]["output_format"]
+        # Generate url query string and generate auth (basic)
+        url = self._generate_url(query_file_content["query"])
+        auth = self._generate_auth()
+        selected_variables = query_file_content["data"].get("variables", None)
+
+        if self.output_format == "xml":
+            query_results = self._get_query_results_from_api_xml(url, auth)
+        else:
+            query_results = self._get_query_results_from_api_json(
+                url=url, auth=auth, selected_variables=selected_variables
+            )
+
+        filename = query_file_content["data"]["filename"]
+
+        if store_results:
+            self.store_query_results(query_results, filename=filename)
+
+        return query_results
+
+    def store_query_results(
+        self, query_results, filename: str, storage_dir: str = None
+    ) -> str:
+        """
+        Store the results from the query according to the output format specified in the query file
+
+        :param query_results: The parsed or raw response from a fhir server to the given query
+        :param filename: name for the results file (defined in query.json)
+        :param storage_dir: directory in which the data should be stored
+        :return:
+        """
+
+        storage_dir = storage_dir if storage_dir else os.getenv("TRAIN_DATA_DIR")
+        if not storage_dir:
+            logger.warning(
+                "No storage directory specified, saving results to current working directory."
+            )
+            results_path = filename
+        else:
+            results_path = os.path.join(storage_dir, filename)
+
+        if self.output_format in ["raw", "json"]:
+            with open(results_path, "w") as results_file:
+                results_file.write(json.dumps(query_results, indent=2))
+
+        # write xml string to file directly
+        elif self.output_format == "xml":
+            with open(results_path, "w") as results_file:
+                results_file.write(query_results)
+
+        else:
+            raise ValueError(f"Unsupported output format: {self.output_format}")
+
+        logger.info("Stored query results in {}", results_path)
+        return results_path
+
+    def _get_query_results_from_api_json(
+        self,
+        url: str,
+        auth: requests.auth.AuthBase = None,
+        selected_variables: List[str] = None,
+        k_anonymity: int = 5,
+    ):
+        """
+        Blocking version of the querying a fhir server with the given search url. Processes all next relations in the
+        response to get the full response in a single file.
+
+        :param url:
+        :param auth:
+        :param selected_variables:
+        :param k_anonymity:
+        :return:
+        """
+
+        r = requests.get(url, auth=auth)
+        r.raise_for_status()
+
+        initial_response = r.json()
+        response = r.json()
+        print(url)
+        print(response)
+        if response.get("entry"):
+            if (len(response["entry"]) < self.k_anon) and not self.disable_k_anon:
+                raise ValueError(
+                    "Too few results match the query. Response blocked by k-anonymity policy."
+                )
+        else:
+            raise ValueError("No results match the query.")
+        link = response.get("link", None)
+        if not link:
+            return response
+        else:
+            print("Resolving response pagination")
+            entries = []
+            entries.extend(response["entry"])
+
+            while response.get("link", None):
+
+                next_page = next(
+                    (
+                        link
+                        for link in response["link"]
+                        if link.get("relation", None) == "next"
+                    ),
+                    None,
+                )
+                if next_page:
+                    response = requests.get(next_page["url"], auth=auth).json()
+                    entries.extend(response["entry"])
+                else:
+                    break
+
+            initial_response["entry"] = entries
+            return initial_response
+
+    def _get_query_results_from_api_xml(
+        self, url: str, auth: requests.auth.AuthBase = None
+    ) -> str:
+        server_response = requests.get(url, auth=auth)
+        initial_response = xmltodict.parse(server_response.text)
+        entries = initial_response["Bundle"]["entry"]
+
+        if not entries:
+            print("No results found for query")
+            return server_response.text
+
+        response = initial_response
+        while True:
+            next_page = False
+            for link in response["Bundle"]["link"]:
+                if isinstance(link, collections.OrderedDict):
+                    relation_dict = dict(link["relation"])
+                else:
+                    break
+                if relation_dict.get("@value") == "next":
+                    print("Getting next")
+                    # get url and extend with xml format
+                    url = link["url"]["@value"]
+                    url = url + "&_format=xml"
+                    r = requests.get(url, auth=auth)
+                    r.raise_for_status()
+                    response = xmltodict.parse(r.text)
+                    added_entries = response["Bundle"]["entry"]
+                    entries.extend(added_entries)
+                    # Stop resolving the pagination when the limit is reached
+                    next_page = True
+
+            if not next_page:
+                print("All pages found")
+                break
+        # added the paginated resources to the initial response
+        initial_response["Bundle"]["entry"] = entries
+
+        if (len(entries) < self.k_anon) and not self.disable_k_anon:
+            raise ValueError(
+                "Too few results match the query. Response blocked by k-anonymity policy."
+            )
+        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
+        return full_response_xml
+
+    def health_check(self):
+
+        api_url = self.server_url + "metadata"
+        auth = self._generate_auth()
+
+        r = requests.get(api_url, auth=auth)
+        r.raise_for_status()
+
+    def _process_fhir_response(
+        self, response: dict, selected_variables: List[str] = None
+    ) -> Union[pd.DataFrame, List[dict], None]:
+        """
+        Parses the fhir response into a dataframe. If selected variables are given only these are parsed from the
+        response and returned
+
+        :param response: the response data to the query from a fhir server
+        :param selected_variables: list variable names to parse from the response
+        :return:
+        """
+        entries = []
+
+        if self.output_format == "df":
+            if response.get("entry", None):
+                for entry in response["entry"]:
+                    if selected_variables:
+                        series_entry = pd.Series(entry["resource"])[selected_variables]
+                    else:
+                        series_entry = pd.Series(entry["resource"])
+                    entries.append(series_entry)
+
+                df = pd.concat(entries, axis=1)
+                df = df.T
+
+                return df
+            else:
+                return None
+
+        else:
+            return response["entry"]
+
+    @staticmethod
+    def read_query_file(file: Union[str, os.PathLike, BytesIO]) -> dict:
+        """
+        Reads the content of a query.json file either given as a path or as in memory file object
+        :param file: path to file or in memory file object to parse
+        :return: dictionary representation of the query.json file
+        """
+        if isinstance(file, BytesIO):
+            query_file = file.read()
+        else:
+            with open(file, "r") as f:
+                query_file = f.read()
+        query_file = json.loads(query_file)
+        return query_file
+
+    def _generate_url(self, query: Union[dict, list, str], limit=1000):
+        """
+        Generates the fhir search url to request from the server based. Either based on a previously given query string
+        or based on a dictionary containing the query definition in the query.json file.
+
+        :param query: dictionary containing the content of the query definition in the query.json file
+        :param query_string: Predefined Fhir url query string to append to base server url
+        :param return_format: the format in which the server should return the data.
+        :param limit: the max number of entries in a paginated response
+        :return: url string to perform a request against a fhir server with
+        """
+
+        if self.server_url[-1] == "/":
+            url = self.server_url
+        else:
+            url = self.server_url + "/"
+
+        if isinstance(query, dict):
+            url += build_query_string(query_dict=query)
+        elif isinstance(query, list):
+            url += build_query_string(query_dict=query)
+        elif isinstance(query, str):
+            url += query
+        else:
+            raise ValueError("Either query dictionary or string need to be given")
+
+        # add formatting configuration
+
+        if url[-1] == "?":
+            url += f"_format={self.output_format}&_count={limit}"
+        else:
+            url += f"&_format={self.output_format}&_count={limit}"
+
+        return url
+
+    def _generate_auth(self) -> requests.auth.AuthBase:
+        """
+        Generate authentication for the request to be sent to server. Based on a given bearer token, basic
+        auth with username and password or by requesting a new token using oauth2.
+
+        :return: Auth object to pass to a requests call.
+        """
+        if self.username and self.password:
+            logger.info("Using basic auth")
+            return HTTPBasicAuth(username=self.username, password=self.password)
+        # TODO request token from id provider if configured
+        elif self.token:
+            logger.info("Using static token auth.")
+            return BearerAuth(token=self.token)
+
+        elif self.client_id and self.client_secret and self.oidc_provider_url:
+            logger.info("Requesting oauth2 token")
+            client = BackendApplicationClient(client_id=self.client_id)
+            oauth = OAuth2Session(client=client)
+            token = oauth.fetch_token(
+                token_url=self.oidc_provider_url,
+                client_secret=self.client_secret,
+                client_id=self.client_id,
+            )
+            self.token = token["access_token"]
+            return BearerAuth(token=self.token)
+
+
+class BearerAuth(requests.auth.AuthBase):
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        r.headers["authorization"] = "Bearer " + self.token
+        return r
```

### Comparing `pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_query_builder.py` & `pht_train_container_library-2.0.6/train_lib/clients/fhir/fhir_query_builder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import json
-import os
-from typing import List, Union
-
-
-def build_query_string(query_dict: dict) -> str:
-    """
-    Builds a valid query string to perform a get request against a fhir server based on the given dictionary
-    containing the definition of a fhir query in json format.
-
-    :param query_dict: dictionary defining fhir search parameters
-    :return:
-    """
-    query_string = query_dict["resource"] + "?"
-
-    # check if there are search parameters given for the main resource
-    if query_dict.get("parameters", None):
-        # generate the url string for the main resources parameters
-        query_string += process_main_resource_parameters(query_dict["parameters"])
-
-    # check if there are reverse chain parameters specified and if so append them to the search url
-    if query_dict.get("has", None):
-        if query_dict.get("parameters", None):
-            query_string += "&"
-        query_string += process_reverse_chain_params(
-            query_dict["resource"], query_dict["has"]
-        )
-
-    return query_string
-
-
-def process_main_resource_parameters(resource_params: List[dict]) -> str:
-    """
-    Build the query parameters to be applied directly to queried fhir resource.
-    :param resource_params: List of dictionary containing the name of the parameter to search and the search condition
-    :return: part of
-    """
-    param_search_string = ""
-    for i, parameter in enumerate(resource_params):
-        if isinstance(parameter["condition"], list):
-            param_search_string += (
-                f"{parameter['variable']}={','.join(parameter['condition'])}"
-            )
-        else:
-            param_search_string += f"{parameter['variable']}={parameter['condition']}"
-        # dont add an additional & at the end
-        if i < len(resource_params) - 1:
-            param_search_string += "&"
-
-    return param_search_string
-
-
-def process_reverse_chain_params(resource: str, reverse_chains: List[dict]) -> str:
-    """
-    Creates a query string based on the given reverse chain parameters for the queried resource (querying based on
-    other resources that refer to the resource.
-    :param resource: the main resource on which to query references
-    :param reverse_chains: list of reverse chain resources and parameters
-    :return: query string to use in fhir search
-    """
-
-    resource_prop = resource.lower()
-    reverse_chain_string = ""
-    # add all the resources given as reverse chain parameters to the query url
-    for i, chain_resource in enumerate(reverse_chains):
-        reverse_chain_string += f"_has:{chain_resource['resource']}:{resource_prop}:{chain_resource['property']}="
-
-        # Check if there are multiple conditions given and if so join them with commas
-        if isinstance(chain_resource["params"], list):
-            reverse_chain_string += ",".join(chain_resource["params"])
-        else:
-            reverse_chain_string += chain_resource["params"]
-
-        if i < len(reverse_chains) - 1:
-            reverse_chain_string += "&"
-    return reverse_chain_string
-
-
-def load_query_file(query_json: Union[str, os.PathLike, bytes]) -> dict:
-    """
-    Load a give json file defining the fhir query into a dictionary
-    :param query_json:
-    :return:
-    """
-    if isinstance(query_json, str):
-        try:
-            query_dict = json.loads(query_json)
-        except json.decoder.JSONDecodeError:
-            with open(query_json) as f:
-                query_dict = json.load(fp=f)
-    elif isinstance(query_json, bytes):
-        query_dict = json.loads(query_json)
-
-    elif isinstance(query_json, os.PathLike):
-        with open(query_json) as f:
-            query_dict = json.load(fp=f)
-    else:
-        raise ValueError("Unsupported file type for query definition.")
-
-    return query_dict
+import json
+import os
+from typing import List, Union
+
+
+def build_query_string(query_dict: dict) -> str:
+    """
+    Builds a valid query string to perform a get request against a fhir server based on the given dictionary
+    containing the definition of a fhir query in json format.
+
+    :param query_dict: dictionary defining fhir search parameters
+    :return:
+    """
+    query_string = query_dict["resource"] + "?"
+
+    # check if there are search parameters given for the main resource
+    if query_dict.get("parameters", None):
+        # generate the url string for the main resources parameters
+        query_string += process_main_resource_parameters(query_dict["parameters"])
+
+    # check if there are reverse chain parameters specified and if so append them to the search url
+    if query_dict.get("has", None):
+        if query_dict.get("parameters", None):
+            query_string += "&"
+        query_string += process_reverse_chain_params(
+            query_dict["resource"], query_dict["has"]
+        )
+
+    return query_string
+
+
+def process_main_resource_parameters(resource_params: List[dict]) -> str:
+    """
+    Build the query parameters to be applied directly to queried fhir resource.
+    :param resource_params: List of dictionary containing the name of the parameter to search and the search condition
+    :return: part of
+    """
+    param_search_string = ""
+    for i, parameter in enumerate(resource_params):
+        if isinstance(parameter["condition"], list):
+            param_search_string += (
+                f"{parameter['variable']}={','.join(parameter['condition'])}"
+            )
+        else:
+            param_search_string += f"{parameter['variable']}={parameter['condition']}"
+        # dont add an additional & at the end
+        if i < len(resource_params) - 1:
+            param_search_string += "&"
+
+    return param_search_string
+
+
+def process_reverse_chain_params(resource: str, reverse_chains: List[dict]) -> str:
+    """
+    Creates a query string based on the given reverse chain parameters for the queried resource (querying based on
+    other resources that refer to the resource.
+    :param resource: the main resource on which to query references
+    :param reverse_chains: list of reverse chain resources and parameters
+    :return: query string to use in fhir search
+    """
+
+    resource_prop = resource.lower()
+    reverse_chain_string = ""
+    # add all the resources given as reverse chain parameters to the query url
+    for i, chain_resource in enumerate(reverse_chains):
+        reverse_chain_string += f"_has:{chain_resource['resource']}:{resource_prop}:{chain_resource['property']}="
+
+        # Check if there are multiple conditions given and if so join them with commas
+        if isinstance(chain_resource["params"], list):
+            reverse_chain_string += ",".join(chain_resource["params"])
+        else:
+            reverse_chain_string += chain_resource["params"]
+
+        if i < len(reverse_chains) - 1:
+            reverse_chain_string += "&"
+    return reverse_chain_string
+
+
+def load_query_file(query_json: Union[str, os.PathLike, bytes]) -> dict:
+    """
+    Load a give json file defining the fhir query into a dictionary
+    :param query_json:
+    :return:
+    """
+    if isinstance(query_json, str):
+        try:
+            query_dict = json.loads(query_json)
+        except json.decoder.JSONDecodeError:
+            with open(query_json) as f:
+                query_dict = json.load(fp=f)
+    elif isinstance(query_json, bytes):
+        query_dict = json.loads(query_json)
+
+    elif isinstance(query_json, os.PathLike):
+        with open(query_json) as f:
+            query_dict = json.load(fp=f)
+    else:
+        raise ValueError("Unsupported file type for query definition.")
+
+    return query_dict
```

### Comparing `pht_train_container_library-2.0.5/train_lib/clients/fhir/query.json` & `pht_train_container_library-2.0.6/train_lib/clients/fhir/query.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-00000000: 7b0a 2020 2271 7565 7279 223a 207b 0a20  {.  "query": {. 
-00000010: 2020 2022 7265 736f 7572 6365 223a 2022     "resource": "
-00000020: 5061 7469 656e 7422 2c0a 2020 2020 2270  Patient",.    "p
-00000030: 6172 616d 6574 6572 7322 3a20 5b0a 2020  arameters": [.  
-00000040: 2020 2020 7b0a 2020 2020 2020 2020 2276      {.        "v
-00000050: 6172 6961 626c 6522 3a20 2267 656e 6465  ariable": "gende
-00000060: 7222 2c0a 2020 2020 2020 2020 2263 6f6e  r",.        "con
-00000070: 6469 7469 6f6e 223a 2022 6d61 6c65 220a  dition": "male".
-00000080: 2020 2020 2020 7d2c 0a20 2020 2020 207b        },.      {
-00000090: 0a20 2020 2020 2020 2022 7661 7269 6162  .        "variab
-000000a0: 6c65 223a 2022 6269 7274 6864 6174 6522  le": "birthdate"
-000000b0: 2c0a 2020 2020 2020 2020 2263 6f6e 6469  ,.        "condi
-000000c0: 7469 6f6e 223a 2022 7361 3139 3830 2d30  tion": "sa1980-0
-000000d0: 382d 3132 220a 2020 2020 2020 7d0a 2020  8-12".      }.  
-000000e0: 2020 5d2c 0a20 2020 2022 6861 7322 3a20    ],.    "has": 
-000000f0: 5b0a 2020 2020 2020 7b0a 2020 2020 2020  [.      {.      
-00000100: 2020 2272 6573 6f75 7263 6522 3a20 224f    "resource": "O
-00000110: 6273 6572 7661 7469 6f6e 222c 0a20 2020  bservation",.   
-00000120: 2020 2020 2022 7072 6f70 6572 7479 223a       "property":
-00000130: 2022 636f 6465 222c 0a20 2020 2020 2020   "code",.       
-00000140: 2022 7061 7261 6d73 223a 205b 2249 3633   "params": ["I63
-00000150: 2e30 222c 2249 3633 2e31 222c 2249 3633  .0","I63.1","I63
-00000160: 2e32 222c 2249 3633 2e33 222c 2249 3633  .2","I63.3","I63
-00000170: 2e34 222c 2249 3633 2e35 222c 2249 3633  .4","I63.5","I63
-00000180: 2e36 222c 2249 3633 2e37 222c 2249 3633  .6","I63.7","I63
-00000190: 2e38 222c 2249 3633 2e39 225d 0a20 2020  .8","I63.9"].   
-000001a0: 2020 207d 2c0a 2020 2020 2020 7b0a 2020     },.      {.  
-000001b0: 2020 2020 2020 2272 6573 6f75 7263 6522        "resource"
-000001c0: 3a20 2243 6f6e 6469 7469 6f6e 222c 0a20  : "Condition",. 
-000001d0: 2020 2020 2020 2022 7072 6f70 6572 7479         "property
-000001e0: 223a 2022 636f 6465 222c 0a20 2020 2020  ": "code",.     
-000001f0: 2020 2022 7061 7261 6d73 223a 205b 2244     "params": ["D
-00000200: 3730 2e30 222c 2244 3730 2e31 3022 2c22  70.0","D70.10","
-00000210: 4437 302e 3131 222c 2244 3730 2e31 3122  D70.11","D70.11"
-00000220: 2c22 4437 302e 3132 222c 2244 3730 2e31  ,"D70.12","D70.1
-00000230: 3322 2c22 4437 302e 3134 222c 2244 3730  3","D70.14","D70
-00000240: 2e31 3822 2c22 4437 302e 3139 222c 2244  .18","D70.19","D
-00000250: 3730 2e33 222c 2244 3730 2e35 222c 2244  70.3","D70.5","D
-00000260: 3730 2e36 222c 2244 3730 2e37 225d 0a20  70.6","D70.7"]. 
-00000270: 2020 2020 207d 0a20 2020 205d 0a20 207d       }.    ].  }
-00000280: 2c0a 2020 2264 6174 6122 3a20 7b0a 2020  ,.  "data": {.  
-00000290: 2020 226f 7574 7075 745f 666f 726d 6174    "output_format
-000002a0: 223a 2022 6373 7622 2c0a 2020 2020 2276  ": "csv",.    "v
-000002b0: 6172 6961 626c 6573 223a 205b 0a20 2020  ariables": [.   
-000002c0: 2020 2022 6964 222c 0a20 2020 2020 2022     "id",.      "
-000002d0: 6269 7274 6844 6174 6522 2c0a 2020 2020  birthDate",.    
-000002e0: 2020 2267 656e 6465 7222 0a20 2020 205d    "gender".    ]
-000002f0: 0a20 207d 0a7d                           .  }.}
+00000000: 7b0d 0a20 2022 7175 6572 7922 3a20 7b0d  {..  "query": {.
+00000010: 0a20 2020 2022 7265 736f 7572 6365 223a  .    "resource":
+00000020: 2022 5061 7469 656e 7422 2c0d 0a20 2020   "Patient",..   
+00000030: 2022 7061 7261 6d65 7465 7273 223a 205b   "parameters": [
+00000040: 0d0a 2020 2020 2020 7b0d 0a20 2020 2020  ..      {..     
+00000050: 2020 2022 7661 7269 6162 6c65 223a 2022     "variable": "
+00000060: 6765 6e64 6572 222c 0d0a 2020 2020 2020  gender",..      
+00000070: 2020 2263 6f6e 6469 7469 6f6e 223a 2022    "condition": "
+00000080: 6d61 6c65 220d 0a20 2020 2020 207d 2c0d  male"..      },.
+00000090: 0a20 2020 2020 207b 0d0a 2020 2020 2020  .      {..      
+000000a0: 2020 2276 6172 6961 626c 6522 3a20 2262    "variable": "b
+000000b0: 6972 7468 6461 7465 222c 0d0a 2020 2020  irthdate",..    
+000000c0: 2020 2020 2263 6f6e 6469 7469 6f6e 223a      "condition":
+000000d0: 2022 7361 3139 3830 2d30 382d 3132 220d   "sa1980-08-12".
+000000e0: 0a20 2020 2020 207d 0d0a 2020 2020 5d2c  .      }..    ],
+000000f0: 0d0a 2020 2020 2268 6173 223a 205b 0d0a  ..    "has": [..
+00000100: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00000110: 2022 7265 736f 7572 6365 223a 2022 4f62   "resource": "Ob
+00000120: 7365 7276 6174 696f 6e22 2c0d 0a20 2020  servation",..   
+00000130: 2020 2020 2022 7072 6f70 6572 7479 223a       "property":
+00000140: 2022 636f 6465 222c 0d0a 2020 2020 2020   "code",..      
+00000150: 2020 2270 6172 616d 7322 3a20 5b22 4936    "params": ["I6
+00000160: 332e 3022 2c22 4936 332e 3122 2c22 4936  3.0","I63.1","I6
+00000170: 332e 3222 2c22 4936 332e 3322 2c22 4936  3.2","I63.3","I6
+00000180: 332e 3422 2c22 4936 332e 3522 2c22 4936  3.4","I63.5","I6
+00000190: 332e 3622 2c22 4936 332e 3722 2c22 4936  3.6","I63.7","I6
+000001a0: 332e 3822 2c22 4936 332e 3922 5d0d 0a20  3.8","I63.9"].. 
+000001b0: 2020 2020 207d 2c0d 0a20 2020 2020 207b       },..      {
+000001c0: 0d0a 2020 2020 2020 2020 2272 6573 6f75  ..        "resou
+000001d0: 7263 6522 3a20 2243 6f6e 6469 7469 6f6e  rce": "Condition
+000001e0: 222c 0d0a 2020 2020 2020 2020 2270 726f  ",..        "pro
+000001f0: 7065 7274 7922 3a20 2263 6f64 6522 2c0d  perty": "code",.
+00000200: 0a20 2020 2020 2020 2022 7061 7261 6d73  .        "params
+00000210: 223a 205b 2244 3730 2e30 222c 2244 3730  ": ["D70.0","D70
+00000220: 2e31 3022 2c22 4437 302e 3131 222c 2244  .10","D70.11","D
+00000230: 3730 2e31 3122 2c22 4437 302e 3132 222c  70.11","D70.12",
+00000240: 2244 3730 2e31 3322 2c22 4437 302e 3134  "D70.13","D70.14
+00000250: 222c 2244 3730 2e31 3822 2c22 4437 302e  ","D70.18","D70.
+00000260: 3139 222c 2244 3730 2e33 222c 2244 3730  19","D70.3","D70
+00000270: 2e35 222c 2244 3730 2e36 222c 2244 3730  .5","D70.6","D70
+00000280: 2e37 225d 0d0a 2020 2020 2020 7d0d 0a20  .7"]..      }.. 
+00000290: 2020 205d 0d0a 2020 7d2c 0d0a 2020 2264     ]..  },..  "d
+000002a0: 6174 6122 3a20 7b0d 0a20 2020 2022 6f75  ata": {..    "ou
+000002b0: 7470 7574 5f66 6f72 6d61 7422 3a20 2263  tput_format": "c
+000002c0: 7376 222c 0d0a 2020 2020 2276 6172 6961  sv",..    "varia
+000002d0: 626c 6573 223a 205b 0d0a 2020 2020 2020  bles": [..      
+000002e0: 2269 6422 2c0d 0a20 2020 2020 2022 6269  "id",..      "bi
+000002f0: 7274 6844 6174 6522 2c0d 0a20 2020 2020  rthDate",..     
+00000300: 2022 6765 6e64 6572 220d 0a20 2020 205d   "gender"..    ]
+00000310: 0d0a 2020 7d0d 0a7d                      ..  }..}
```

### Comparing `pht_train_container_library-2.0.5/train_lib/docker_util/validate_master_image.py` & `pht_train_container_library-2.0.6/train_lib/docker_util/validate_master_image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,190 @@
-import hashlib
-import tarfile
-from io import BytesIO
-
-import docker
-from train_lib.docker_util import TIMEOUT
-
-# statically define files and directories which shall be exempt from hash file comparison
-_DEFAULT_PATH_EXCEPTIONS = [
-    b"opt/pht_results",
-    b"opt/pht_train",
-    b"opt/train_config.json",
-    b"opt/user_sym_key.key",
-    b"opt/.wh.",
-]
-
-
-def _default_docker_client():
-    try:
-        client = docker.from_env(timeout=TIMEOUT)
-
-    except Exception:
-        client = docker.DockerClient(
-            base_url="unix://var/run/docker.sock", timeout=TIMEOUT
-        )
-
-    return client
-
-
-def validate_train_image(
-    master_image_name: str,
-    train_image_name: str,
-    path_exceptions=_DEFAULT_PATH_EXCEPTIONS,
-    docker_client=_default_docker_client(),
-):
-    """
-    Validates a train image against an official master image
-    :param master_image_name: string identifier of the master docker image to validate against
-    :param train_image_name: string identifier of the docker image defining a train
-    :param path_exceptions: list of byte strings containing paths that shall be exempt from file system comparison
-    :param docker_client: docker client able to apply for the master and train docker image
-    :return:
-    """
-
-    # extract docker images by name through client
-    master_image = docker_client.images.get(master_image_name)
-    train_image = docker_client.images.get(train_image_name)
-
-    # check if history entries indicate that train image stems from master image
-    if _do_history_test(master_image, train_image):
-        # extract file system hashes
-        master_hashes = _get_file_hashes(master_image, path_exceptions)
-        train_hashes = _get_file_hashes(train_image, path_exceptions)
-
-        # if comparison of hashed files systems turns out as False raise ValueError
-        if not dict(sorted(master_hashes.items())) == dict(
-            sorted(train_hashes.items())
-        ):
-            raise ValueError(
-                "File system of train image could not be validated. Hashed file system comparison "
-                "implicated error during validation."
-            )
-    # if train images does not stem from master image raise Value Error
-    else:
-        raise ValueError(
-            "File system of train image could not be validated. History entries implicated error during "
-            "validation."
-        )
-
-
-def _do_history_test(master_image, train_image) -> bool:
-    """
-    Compare history entries between images, to ensure that the given train image is a successor to the master image.
-    :param master_image: master image object whose history entries will be used as base
-    :param train_image: train image object whose history entries should contain the master image history entry's
-    :return: boolean fo whether all master image history entries are also in the train image history
-    """
-    # Extract history entry ids
-    master_img_entry_ids = [
-        {key: entry[key] for key in ["Created", "CreatedBy", "Size"]}
-        for entry in master_image.history()
-    ]
-    train_img_entry_ids = [
-        {key: entry[key] for key in ["Created", "CreatedBy", "Size"]}
-        for entry in train_image.history()
-    ]
-
-    # Check whether all entry ids of the master image history are also in the train image's
-    is_history_test_true = all(
-        [entry_dict in train_img_entry_ids for entry_dict in master_img_entry_ids]
-    )
-    return is_history_test_true
-
-
-def _get_file_hashes(
-    docker_image, path_exceptions: list[bytes]
-) -> dict[bytes : list[str]]:
-    """
-    Extracts file system of docker image and returns dictionary with byte paths as keys and list of hashed file
-    contents from layers
-    :param docker_image: docker image object whose file system is to be extracted and hashed
-    :param path_exceptions: list of byte strings for paths that, if they start with either of them, will be excluded
-                            from the returned hashed file system
-    :return: dictionary containing the hashed file system with byte paths as keys and list of associated
-             hashed file contents
-    """
-    # init dict which will collected hashes and be returned
-    image_hashes = {}
-
-    # extract file system form images as chunks collected into a bytearray
-    bytes_arr = bytearray()
-    for chunk in docker_image.save():
-        bytes_arr.extend(chunk)
-
-    # unzip chunk.tar from buffer
-    with tarfile.open(fileobj=BytesIO(bytes_arr)) as outer:
-        # isolate and extract layer.tar files
-        layers_tars = [n for n in outer.getnames() if n.endswith("/layer.tar")]
-        for i, layer_tar in enumerate(layers_tars):
-            layer_file = outer.extractfile(layer_tar)
-            if layer_file is None:
-                continue
-
-            # unzip layer.tar files
-            with tarfile.open(fileobj=layer_file, encoding="utf-8") as layer:
-                # collect paths in file system as keys and file contents as items in dictionary, if path does not start
-                # with any of the excepted paths
-                paths_in_layer = {
-                    x.encode("utf-8"): layer.getmember(x)
-                    for x in layer.getnames()
-                    if all(
-                        [not x.encode("utf-8").startswith(y) for y in path_exceptions]
-                    )
-                }
-
-                # collect hashes of file contents into lists using the paths as keys for all layer.tar files
-                for path, content in paths_in_layer.items():
-                    # path leads to anything but a file, set list with empty string (e.g. It is there. And that's it.)
-                    if not content.isfile():
-                        image_hashes[path] = [""]
-                    else:
-                        f = layer.extractfile(content)
-                        h = hashlib.sha256()
-                        h.update(f.read())
-                        if path in image_hashes.keys():
-                            image_hashes[path].append(h.hexdigest())
-                            image_hashes[path] = sorted(image_hashes[path])
-                        else:
-                            image_hashes[path] = [h.hexdigest()]
-    return image_hashes
+import hashlib
+import multiprocessing as mp
+import tarfile
+from io import BytesIO
+
+import docker
+from train_lib.docker_util import TIMEOUT
+
+# statically define files and directories which shall be exempt from hash file comparison
+_DEFAULT_PATH_EXCEPTIONS = [
+    b"opt/pht_results",
+    b"opt/pht_train",
+    b"opt/train_config.json",
+    b"opt/user_sym_key.key",
+    b"opt/.wh.",
+]
+
+
+def _default_docker_client():
+    try:
+        client = docker.from_env(timeout=TIMEOUT)
+
+    except Exception:
+        client = docker.DockerClient(
+            base_url="unix://var/run/docker.sock", timeout=TIMEOUT
+        )
+
+    return client
+
+
+def validate_train_image(
+    master_image_name: str,
+    train_image_name: str,
+    path_exceptions=_DEFAULT_PATH_EXCEPTIONS,
+    docker_client=_default_docker_client(),
+    num_cpus=4,
+):
+    """
+    Validates a train image against an official master image
+    :param master_image_name: string identifier of the master docker image to validate against
+    :param train_image_name: string identifier of the docker image defining a train
+    :param path_exceptions: list of byte strings containing paths that shall be exempt from file system comparison
+    :param docker_client: docker client able to apply for the master and train docker image
+    :param num_cpus: number of cpu cores used
+    :return:
+    """
+    # extract docker images by name through client
+    master_image = docker_client.images.get(master_image_name)
+    train_image = docker_client.images.get(train_image_name)
+
+    # check if history entries indicate that train image stems from master image
+    if _do_history_test(master_image, train_image):
+        # extract file system hashes
+        master_hashes = _get_file_hashes(master_image, path_exceptions, num_cpus)
+        train_hashes = _get_file_hashes(train_image, path_exceptions, num_cpus)
+
+        # if comparison of hashed files systems turns out as False raise ValueError
+        if not dict(sorted(master_hashes.items())) == dict(
+            sorted(train_hashes.items())
+        ):
+            raise ValueError(
+                "File system of train image could not be validated. Hashed file system comparison "
+                "implicated error during validation."
+            )
+    # if train images does not stem from master image raise Value Error
+    else:
+        raise ValueError(
+            "File system of train image could not be validated. History entries implicated error during "
+            "validation."
+        )
+
+
+def _do_history_test(master_image, train_image) -> bool:
+    """
+    Compare history entries between images, to ensure that the given train image is a successor to the master image.
+    :param master_image: master image object whose history entries will be used as base
+    :param train_image: train image object whose history entries should contain the master image history entry's
+    :return: boolean fo whether all master image history entries are also in the train image history
+    """
+    # Extract history entry ids
+    master_img_entry_ids = [
+        {key: entry[key] for key in ["Created", "CreatedBy", "Size"]}
+        for entry in master_image.history()
+    ]
+    train_img_entry_ids = [
+        {key: entry[key] for key in ["Created", "CreatedBy", "Size"]}
+        for entry in train_image.history()
+    ]
+
+    # Check whether all entry ids of the master image history are also in the train image's
+    is_history_test_true = all(
+        [entry_dict in train_img_entry_ids for entry_dict in master_img_entry_ids]
+    )
+    return is_history_test_true
+
+
+def _get_file_hashes(
+    docker_image, path_exceptions: list[bytes], num_cpus: int
+) -> dict[bytes : list[str]]:
+    """
+    Extracts file system of docker image and returns dictionary with byte paths as keys and list of hashed file
+    contents from layers
+    :param docker_image: docker image object whose file system is to be extracted and hashed
+    :param path_exceptions: list of byte strings for paths that, if they start with either of them, will be excluded
+                            from the returned hashed file system
+    :param num_cpus: number of cpu cores used
+    :return: dictionary containing the hashed file system with byte paths as keys and list of associated
+             hashed file contents
+    """
+    # init dict which will collect hashes and be returned
+    image_hashes = {}
+
+    # extract file system form images as chunks collected into a bytearray
+    bytes_arr = bytearray()
+    for chunk in docker_image.save():
+        bytes_arr.extend(chunk)
+
+    # unzip chunk.tar from buffer
+    with tarfile.open(fileobj=BytesIO(bytes_arr)) as outer:
+        # collect layer tarfiles and add them together with path exceptions to list of tuples
+        layer_tars = []
+        for n in outer.getnames():
+            if n.endswith("/layer.tar"):
+                layer_file = outer.extractfile(n)
+                if layer_file is not None:
+                    bytes_arr = bytearray()
+                    bytes_arr.extend(layer_file.read())
+                    layer_tars.append((bytes_arr, path_exceptions))
+
+        # init and execute (a)synchronous multiprocessing for hashing function
+        pool = mp.Pool(num_cpus) if num_cpus != -1 else mp.Pool(mp.cpu_count())
+        # results = []
+        # def collect_result(result):
+        #     global results
+        #     results.append(result)
+        # pool.map_async(_apply_hash_function_to_layers, layers, callback=collect_result)
+        results = pool.map(_apply_hash_function_to_layers, layer_tars)
+        pool.close()
+        # pool.join()
+
+        # aggregate multiprocessing results
+        for result in results:
+            # integrate hash results into full image hash
+            for path in result.keys():
+                hashes = [] if path not in image_hashes.keys() else image_hashes[path]
+                hashes.extend(result[path])
+                image_hashes[path] = sorted([h for h in hashes if h])
+
+    return image_hashes
+
+
+def _apply_hash_function_to_layers(
+    layer_tars: tuple[bytearray, list[bytes]]
+) -> dict[str:str]:
+    """
+    Apply hash function to layers in file system and return dictionary with hashed layer contents
+    :param layer_tars: tuple containing single layer tarfile as bytearray and list of filepath exceptions
+    :return: dictionary containing the hashed contents of the single layer
+    """
+    # init dict which will collect hashes and be returned
+    layer_hashes = {}
+
+    outer_layer_bytes_arr, path_exceptions = layer_tars
+
+    # open layer tarfile bytearray as tarfile
+    with tarfile.open(fileobj=BytesIO(outer_layer_bytes_arr)) as outer_layer:
+        # collect paths in file system as keys and file contents as items in dictionary, if path does not start
+        # with any of the excepted paths
+        paths_in_layer = {
+            x.encode("utf-8"): outer_layer.getmember(x)
+            for x in outer_layer.getnames()
+            if all([not x.encode("utf-8").startswith(y) for y in path_exceptions])
+        }
+
+        # collect hashes of file contents into lists using the paths as keys for all layer.tar files
+        for path, content in paths_in_layer.items():
+            # path leads to anything but a file, set list with empty string (e.g. It is there. And that's it.)
+            if not content.isfile():
+                layer_hashes[path] = [""]
+            else:
+                f = outer_layer.extractfile(content)
+                h = hashlib.sha256()
+                h.update(f.read())
+                if path in layer_hashes.keys():
+                    layer_hashes[path].append(h.hexdigest())
+                    layer_hashes[path] = layer_hashes[path]
+                else:
+                    layer_hashes[path] = [h.hexdigest()]
+
+    return layer_hashes
```

### Comparing `pht_train_container_library-2.0.5/train_lib/security/encryption.py` & `pht_train_container_library-2.0.6/train_lib/security/encryption.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import os
-from io import BytesIO
-from typing import BinaryIO, List, Union
-
-from cryptography.hazmat.primitives import padding
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from loguru import logger
-
-IV_LENGTH = 16
-
-PADDING_LENGTH = 128
-
-
-class FileEncryptor:
-    """
-    Performs symmetric encryption and decryption of sensitive files belonging to the train cargo
-    """
-
-    def __init__(self, key: bytes):
-        self.key = key
-        self.iv = os.urandom(IV_LENGTH)
-
-    def encrypt_files(
-        self, files: Union[List[str], List[BinaryIO]], binary_files=False
-    ) -> Union[List[BytesIO], None]:
-        """
-        Decrypt the given files using symmetric encryption
-        :return:
-        """
-        logger.info("Encrypting files..")
-        if binary_files:
-            encr_files = []
-            for i, file in enumerate(files):
-                logger.debug(f"file {i + 1}/{len(files)}...")
-                # Encrypt the files and convert them to bytes io file objects
-                file.seek(0)
-                data = file.read()
-                encr_files.append(BytesIO(self._encrypt_aes(data)))
-            logger.info("Done")
-            return encr_files
-
-        for i, file in enumerate(files):
-            logger.info(f"File {i + 1}/{len(files)}...")
-            with open(file, "rb") as f:
-                encr_file = self._encrypt_aes(f.read())
-            with open(file, "wb") as ef:
-                ef.write(encr_file)
-        logger.info("Done")
-
-    def decrypt_files(
-        self, files: Union[List[str], List[BinaryIO]], binary_files=False
-    ) -> Union[List[BytesIO], None]:
-        """
-        Decrypt the given files using symmetric encryption
-        :return:
-        """
-        logger.info("Decrypting files..")
-        if binary_files:
-            decr_files = []
-            for i, file in enumerate(files):
-                file.seek(0)
-                logger.debug(f"file {i + 1}/{len(files)}...")
-                data = self._decrypt_aes(file.read())
-                decr_files.append(BytesIO(data))
-            logger.info("Done")
-            return decr_files
-        for i, file in enumerate(files):
-            logger.info(f"File {i + 1}/{len(files)}...")
-            with open(file, "rb") as f:
-                decr_file = self._decrypt_aes(f.read())
-            with open(file, "wb") as ef:
-                ef.write(decr_file)
-            logger.info("Done")
-
-    def decrypt_file(self, file: BinaryIO) -> BytesIO:
-        """
-        Decrypt the given file using symmetric encryption
-        :return:
-        """
-        file.seek(0)
-        data = self._decrypt_aes(file.read())
-        return BytesIO(data)
-
-    def decrypt(self, data: bytes) -> bytes:
-        """
-        Decrypt the given data using symmetric encryption
-        :return:
-        """
-        return self._decrypt_aes(data)
-
-    def encrypt(self, data: bytes) -> bytes:
-        """
-        Encrypt the given data using symmetric encryption
-        :return:
-        """
-        return self._encrypt_aes(data)
-
-    def encrypt_file(self, file: BinaryIO) -> BytesIO:
-        """
-        Encrypt the given file using symmetric encryption
-        :return:
-        """
-        data = self._encrypt_aes(file.read())
-        return BytesIO(data)
-
-    def _encrypt_aes(self, data: bytes) -> bytes:
-
-        logger.debug("Encryption data preview: " + str(data[:100]))
-        padder = padding.PKCS7(PADDING_LENGTH).padder()
-        padded_data = padder.update(data)
-        padded_data += padder.finalize()
-
-        cipher = Cipher(algorithms.AES(self.key), modes.CBC(self.iv))
-        encryptor = cipher.encryptor()
-
-        encrypted = encryptor.update(padded_data) + encryptor.finalize()
-
-        logger.debug("Encrypted Data: " + str(encrypted[:100]))
-
-        return self.iv + encrypted
-
-    def _decrypt_aes(self, data: bytes) -> bytes:
-        iv = data[:IV_LENGTH]
-        data = data[IV_LENGTH:]
-        cipher = Cipher(algorithms.AES(self.key), modes.CBC(iv))
-        logger.debug("Encrypted data: " + str(data[:100]))
-        decryptor = cipher.decryptor()
-
-        decrypted = decryptor.update(data) + decryptor.finalize()
-        unpadder = padding.PKCS7(PADDING_LENGTH).unpadder()
-
-        unpadded_data = unpadder.update(decrypted)
-        unpadded_data += unpadder.finalize()
-        logger.debug("Decrypted data: " + str(unpadded_data[:100]))
-        return unpadded_data
+import os
+from io import BytesIO
+from typing import BinaryIO, List, Union
+
+from cryptography.hazmat.primitives import padding
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from loguru import logger
+
+IV_LENGTH = 16
+
+PADDING_LENGTH = 128
+
+
+class FileEncryptor:
+    """
+    Performs symmetric encryption and decryption of sensitive files belonging to the train cargo
+    """
+
+    def __init__(self, key: bytes):
+        self.key = key
+        self.iv = os.urandom(IV_LENGTH)
+
+    def encrypt_files(
+        self, files: Union[List[str], List[BinaryIO]], binary_files=False
+    ) -> Union[List[BytesIO], None]:
+        """
+        Decrypt the given files using symmetric encryption
+        :return:
+        """
+        logger.info("Encrypting files..")
+        if binary_files:
+            encr_files = []
+            for i, file in enumerate(files):
+                logger.debug(f"file {i + 1}/{len(files)}...")
+                # Encrypt the files and convert them to bytes io file objects
+                file.seek(0)
+                data = file.read()
+                encr_files.append(BytesIO(self._encrypt_aes(data)))
+            logger.info("Done")
+            return encr_files
+
+        for i, file in enumerate(files):
+            logger.info(f"File {i + 1}/{len(files)}...")
+            with open(file, "rb") as f:
+                encr_file = self._encrypt_aes(f.read())
+            with open(file, "wb") as ef:
+                ef.write(encr_file)
+        logger.info("Done")
+
+    def decrypt_files(
+        self, files: Union[List[str], List[BinaryIO]], binary_files=False
+    ) -> Union[List[BytesIO], None]:
+        """
+        Decrypt the given files using symmetric encryption
+        :return:
+        """
+        logger.info("Decrypting files..")
+        if binary_files:
+            decr_files = []
+            for i, file in enumerate(files):
+                file.seek(0)
+                logger.debug(f"file {i + 1}/{len(files)}...")
+                data = self._decrypt_aes(file.read())
+                decr_files.append(BytesIO(data))
+            logger.info("Done")
+            return decr_files
+        for i, file in enumerate(files):
+            logger.info(f"File {i + 1}/{len(files)}...")
+            with open(file, "rb") as f:
+                decr_file = self._decrypt_aes(f.read())
+            with open(file, "wb") as ef:
+                ef.write(decr_file)
+            logger.info("Done")
+
+    def decrypt_file(self, file: BinaryIO) -> BytesIO:
+        """
+        Decrypt the given file using symmetric encryption
+        :return:
+        """
+        file.seek(0)
+        data = self._decrypt_aes(file.read())
+        return BytesIO(data)
+
+    def decrypt(self, data: bytes) -> bytes:
+        """
+        Decrypt the given data using symmetric encryption
+        :return:
+        """
+        return self._decrypt_aes(data)
+
+    def encrypt(self, data: bytes) -> bytes:
+        """
+        Encrypt the given data using symmetric encryption
+        :return:
+        """
+        return self._encrypt_aes(data)
+
+    def encrypt_file(self, file: BinaryIO) -> BytesIO:
+        """
+        Encrypt the given file using symmetric encryption
+        :return:
+        """
+        data = self._encrypt_aes(file.read())
+        return BytesIO(data)
+
+    def _encrypt_aes(self, data: bytes) -> bytes:
+
+        logger.debug("Encryption data preview: " + str(data[:100]))
+        padder = padding.PKCS7(PADDING_LENGTH).padder()
+        padded_data = padder.update(data)
+        padded_data += padder.finalize()
+
+        cipher = Cipher(algorithms.AES(self.key), modes.CBC(self.iv))
+        encryptor = cipher.encryptor()
+
+        encrypted = encryptor.update(padded_data) + encryptor.finalize()
+
+        logger.debug("Encrypted Data: " + str(encrypted[:100]))
+
+        return self.iv + encrypted
+
+    def _decrypt_aes(self, data: bytes) -> bytes:
+        iv = data[:IV_LENGTH]
+        data = data[IV_LENGTH:]
+        cipher = Cipher(algorithms.AES(self.key), modes.CBC(iv))
+        logger.debug("Encrypted data: " + str(data[:100]))
+        decryptor = cipher.decryptor()
+
+        decrypted = decryptor.update(data) + decryptor.finalize()
+        unpadder = padding.PKCS7(PADDING_LENGTH).unpadder()
+
+        unpadded_data = unpadder.update(decrypted)
+        unpadded_data += unpadder.finalize()
+        logger.debug("Decrypted data: " + str(unpadded_data[:100]))
+        return unpadded_data
```

### Comparing `pht_train_container_library-2.0.5/train_lib/security/hashing.py` & `pht_train_container_library-2.0.6/train_lib/security/hashing.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import BinaryIO, List, Union
-
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
-from loguru import logger
-
-
-def hash_immutable_files(
-    immutable_files: Union[List[BinaryIO], List[str]],
-    user_id: str,
-    session_id: bytes,
-    binary_files=False,
-    ordered_file_list: list = None,
-    immutable_file_names: List[str] = None,
-    query: bytes = None,
-):
-    """
-    Calculates the hash of all immutable files in the train, A, R, Q as well as the
-    :param binary_files: boolean parameter indicating whether the files are binary files or file paths
-    :param user_id:
-    :param session_id:
-    :param immutable_files:
-    :return: byte object representing the hash of all files
-    """
-
-    digest = hashes.Hash(hashes.SHA512(), backend=default_backend())
-    digest.update(user_id.encode("utf-8"))
-    query_file = None
-    if binary_files:
-        if immutable_file_names:
-            for f in ordered_file_list:
-                logger.trace(f"Hashing file {f}")
-                # TODO ugly workaround fix this
-                if f.startswith("./"):
-                    f = f[2:]
-
-                index = immutable_file_names.index(f)
-                if f == "query.json":
-                    logger.debug("Found query file")
-                    query_file = immutable_files[index].read()
-                    continue
-                data = immutable_files[index].read()
-                digest.update(data)
-        else:
-            for file in immutable_files:
-                digest.update(file.read())
-    else:
-        for file in ordered_file_list:
-            with open(file, "rb") as f:
-                digest.update(f.read())
-
-    digest.update(session_id)
-    if query_file:
-        digest.update(query_file)
-    if query:
-        logger.debug("Adding query to hash")
-        digest.update(query)
-    return digest.finalize()
-
-
-def hash_results(
-    result_files: Union[List[str], List[BinaryIO]],
-    session_id: bytes,
-    binary_files=False,
-):
-    """
-    Creates a hash of the results of train execution
-    :param result_files: List
-    :param session_id:
-    :return:
-    """
-    digest = hashes.Hash(hashes.SHA512(), backend=default_backend())
-    if binary_files:
-        for file in result_files:
-            data = file.read()
-            digest.update(data)
-    else:
-        for file in result_files:
-            with open(file, "rb") as f:
-                digest.update(f.read())
-    digest.update(session_id)
-    return digest.finalize()
+from typing import BinaryIO, List, Union
+
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from loguru import logger
+
+
+def hash_immutable_files(
+    immutable_files: Union[List[BinaryIO], List[str]],
+    user_id: str,
+    session_id: bytes,
+    binary_files=False,
+    ordered_file_list: list = None,
+    immutable_file_names: List[str] = None,
+    query: bytes = None,
+):
+    """
+    Calculates the hash of all immutable files in the train, A, R, Q as well as the
+    :param binary_files: boolean parameter indicating whether the files are binary files or file paths
+    :param user_id:
+    :param session_id:
+    :param immutable_files:
+    :return: byte object representing the hash of all files
+    """
+
+    digest = hashes.Hash(hashes.SHA512(), backend=default_backend())
+    digest.update(user_id.encode("utf-8"))
+    query_file = None
+    if binary_files:
+        if immutable_file_names:
+            for f in ordered_file_list:
+                logger.trace(f"Hashing file {f}")
+                # TODO ugly workaround fix this
+                if f.startswith("./"):
+                    f = f[2:]
+
+                index = immutable_file_names.index(f)
+                if f == "query.json":
+                    logger.debug("Found query file")
+                    query_file = immutable_files[index].read()
+                    continue
+                data = immutable_files[index].read()
+                digest.update(data)
+        else:
+            for file in immutable_files:
+                digest.update(file.read())
+    else:
+        for file in ordered_file_list:
+            with open(file, "rb") as f:
+                digest.update(f.read())
+
+    digest.update(session_id)
+    if query_file:
+        digest.update(query_file)
+    if query:
+        logger.debug("Adding query to hash")
+        digest.update(query)
+    return digest.finalize()
+
+
+def hash_results(
+    result_files: Union[List[str], List[BinaryIO]],
+    session_id: bytes,
+    binary_files=False,
+):
+    """
+    Creates a hash of the results of train execution
+    :param result_files: List
+    :param session_id:
+    :return:
+    """
+    digest = hashes.Hash(hashes.SHA512(), backend=default_backend())
+    if binary_files:
+        for file in result_files:
+            data = file.read()
+            digest.update(data)
+    else:
+        for file in result_files:
+            with open(file, "rb") as f:
+                digest.update(f.read())
+    digest.update(session_id)
+    return digest.finalize()
```

### Comparing `pht_train_container_library-2.0.5/train_lib/security/homomorphic_addition.py` & `pht_train_container_library-2.0.6/train_lib/security/homomorphic_addition.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from random import SystemRandom
-
-
-class PublicKey(object):
-    @classmethod
-    def from_n(cls, n, g):
-        return cls(n, g)
-
-    def __init__(self, n, g):
-        self.n = n
-        self.n_sq = n * n
-        self.g = g
-
-    def __repr__(self):
-        return "<PublicKey: %s>" % self.n
-
-
-def invmod(a, p, maxiter=1000000):
-    """The multiplicitive inverse of a in the integers modulo p:
-      a * b == 1 mod p
-    Returns b.
-    (http://code.activestate.com/recipes/576737-inverse-modulo-p/)"""
-    if a == 0:
-        raise ValueError("0 has no inverse mod %d" % p)
-    r = a
-    d = 1
-    for i in range(min(p, maxiter)):
-        d = ((p // r + 1) * d) % p
-        r = (d * a) % p
-        if r == 1:
-            break
-    else:
-        raise ValueError("%d has no inverse mod %d" % (a, p))
-    return d
-
-
-def encrypt(pub, plain):
-    r = SystemRandom().randrange(1, pub.n)
-    x = pow(r, pub.n, pub.n_sq)
-
-    cipher = (pow(pub.g, plain, pub.n_sq) * x) % pub.n_sq
-    return cipher
-
-
-def enc_add(pub, a, b):
-    """Add one encrypted integer to another"""
-    return a * b % pub.n_sq
-
-
-def secure_addition(result_local, result_prev, n=None, g=None):
-    if not n or not g:
-        raise ValueError("Empty secure addition key")
-
-    pk = PublicKey.from_n(n, g)
-
-    if result_prev is None:
-        pt = 0
-        ct1 = encrypt(pk, pt)
-    else:
-        ct1 = result_prev
-
-    enc_local = encrypt(pk, result_local)
-
-    ct_added = enc_add(pk, ct1, enc_local)
-
-    return ct_added
+from random import SystemRandom
+
+
+class PublicKey(object):
+    @classmethod
+    def from_n(cls, n, g):
+        return cls(n, g)
+
+    def __init__(self, n, g):
+        self.n = n
+        self.n_sq = n * n
+        self.g = g
+
+    def __repr__(self):
+        return "<PublicKey: %s>" % self.n
+
+
+def invmod(a, p, maxiter=1000000):
+    """The multiplicitive inverse of a in the integers modulo p:
+      a * b == 1 mod p
+    Returns b.
+    (http://code.activestate.com/recipes/576737-inverse-modulo-p/)"""
+    if a == 0:
+        raise ValueError("0 has no inverse mod %d" % p)
+    r = a
+    d = 1
+    for i in range(min(p, maxiter)):
+        d = ((p // r + 1) * d) % p
+        r = (d * a) % p
+        if r == 1:
+            break
+    else:
+        raise ValueError("%d has no inverse mod %d" % (a, p))
+    return d
+
+
+def encrypt(pub, plain):
+    r = SystemRandom().randrange(1, pub.n)
+    x = pow(r, pub.n, pub.n_sq)
+
+    cipher = (pow(pub.g, plain, pub.n_sq) * x) % pub.n_sq
+    return cipher
+
+
+def enc_add(pub, a, b):
+    """Add one encrypted integer to another"""
+    return a * b % pub.n_sq
+
+
+def secure_addition(result_local, result_prev, n=None, g=None):
+    if not n or not g:
+        raise ValueError("Empty secure addition key")
+
+    pk = PublicKey.from_n(n, g)
+
+    if result_prev is None:
+        pt = 0
+        ct1 = encrypt(pk, pt)
+    else:
+        ct1 = result_prev
+
+    enc_local = encrypt(pk, result_local)
+
+    ct_added = enc_add(pk, ct1, enc_local)
+
+    return ct_added
```

### Comparing `pht_train_container_library-2.0.5/train_lib/security/key_manager.py` & `pht_train_container_library-2.0.6/train_lib/security/key_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import os
-from io import BytesIO
-
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
-
-from train_lib.security.train_config import TrainConfig
-
-SYMMETRIC_KEY_LENGTH = 32
-
-
-class KeyManager:
-    """
-    Class that creates, stores and if necessary updates all relevant keys for symmetric and asymmetric encryption
-    """
-
-    def __init__(self, train_config: TrainConfig):
-        """
-        Initialize a KeyManager instance that handles security relevant values based on a train configuration
-
-        :param train_config: either a path to a json file storing the configuration values or a dictionary with these
-            values
-        """
-        self.config = train_config
-
-    def save_config(self, path=None, binary_file=False):
-        """
-        Store the updated config file as a json at the same location
-
-        :return:
-        :rtype:
-        """
-        if binary_file:
-            return BytesIO(self.config.json(indent=2, by_alias=True).encode("utf-8"))
-
-        elif path:
-            with open(path, "w") as f:
-                f.write(self.config.json(indent=2, by_alias=True))
-        else:
-            raise ValueError("No path or binary file specified for saving the keyfile")
-
-    @staticmethod
-    def generate_symmetric_key():
-        """
-        Create a symmetric fernet key for encrypting sensitive files
-        :return:
-        """
-        key = os.urandom(SYMMETRIC_KEY_LENGTH)
-        return key
-
-    def decrypt_symmetric_key(
-        self,
-        encrypted_key: str,
-        private_key_path: str,
-        private_key_password: str = None,
-    ) -> bytes:
-        """
-        Decrypts the symmetric key using a stored private key
-        :arg encrypted_key: the encrypted symmetric key to decrypt in hex format
-        :arg private_key_path: path to the private key file
-        :arg private_key_password: optional password to decrypt the private key
-        :return: symmetric AES key used to encrypt and decrypt files
-        """
-        private_key = self.load_private_key(
-            key_path=private_key_path, password=private_key_password
-        )
-
-        symmetric_key = private_key.decrypt(
-            ciphertext=bytes.fromhex(encrypted_key),
-            padding=padding.OAEP(
-                mgf=padding.MGF1(algorithm=hashes.SHA512()),
-                algorithm=hashes.SHA512(),
-                label=None,
-            ),
-        )
-        return symmetric_key
-
-    def generate_encrypted_keys(self, symmetric_key: bytes):
-        """
-        Generates a dictionary containing the symmetric key used to encrypt files, encrypted with the public keys of all
-        stations on the route
-        :param symmetric_key: byte object containing the symmetric key used to encrypt the mutable files
-        :return: Dictionary consisting of  key = Station Id, value = Symmetric key encrypted with public key of station
-        """
-        enc_keys = {}
-        for station, pk in self.config["rsa_public_keys"]:
-            enc_keys[station] = self.encrypt_symmetric_key(symmetric_key, pk)
-        return enc_keys
-
-    def encrypt_symmetric_key(self, sym_key: bytes, public_key_hex: str) -> str:
-        """
-        Encrypt the symmetric key with all public keys provided in the train configuration file
-
-        :param sym_key: byte object containing the the symmetric key used to encrypt the mutable files
-        :return: dictionary containing the symmetric key encrypted with all available public keys, keys are the station
-        ids and values are the symmetric key encrypted with the RSA public key associated with the station id
-
-        :rtype: str
-        """
-
-        public_key = self.load_public_key(public_key_hex)
-
-        encrypted_key = public_key.encrypt(
-            sym_key,
-            padding.OAEP(
-                mgf=padding.MGF1(algorithm=hashes.SHA512()),
-                algorithm=hashes.SHA512(),
-                label=None,
-            ),
-        )
-        return encrypted_key.hex()
-
-    def _rsa_pk_encrypt(self, val, public_key):
-        encrypted = public_key.encrypt(
-            val,
-            padding.OAEP(
-                mgf=padding.MGF1(algorithm=hashes.SHA512()),
-                algorithm=hashes.SHA512(),
-                label=None,
-            ),
-        )
-        return encrypted.hex()
-
-    @staticmethod
-    def load_private_key(
-        env_key: str = None, key_path: str = None, password: str = None
-    ) -> RSAPrivateKey:
-        """
-        Loads the private key from the path provided provided in the environment variables of the currently
-        running image
-        :param key_path: path to a file containing the private key
-        :param env_key: environment variable containing a hex string representing the station private key
-        :return: a private key object either rsa or ec
-        """
-
-        if env_key and key_path:
-            raise ValueError(
-                f"Multiple private Key locations specified: \n {env_key} \n {key_path}"
-            )
-        # Load key from hex string stored in environment variable
-        if env_key:
-            private_key = serialization.load_pem_private_key(
-                bytes.fromhex(os.getenv(env_key)),
-                password=None,
-                backend=default_backend(),
-            )
-        # Load key from file
-        elif key_path:
-            with open(key_path, "rb") as sk_f:
-                private_key = serialization.load_pem_private_key(
-                    sk_f.read(),
-                    password=password.encode() if password else None,
-                    backend=default_backend(),
-                )
-        else:
-            raise ValueError(
-                "No environment variable or file containing a private key specified"
-            )
-
-        return private_key
-
-    @staticmethod
-    def load_public_key(key: str):
-        """
-        Loads a public key
-        :param key: string representation of a public key
-        :return: public key object for asymmetric encryption
-        """
-        public_key = serialization.load_pem_public_key(
-            bytes.fromhex(key), backend=default_backend()
-        )
-        return public_key
+import os
+from io import BytesIO
+
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+
+from train_lib.security.train_config import TrainConfig
+
+SYMMETRIC_KEY_LENGTH = 32
+
+
+class KeyManager:
+    """
+    Class that creates, stores and if necessary updates all relevant keys for symmetric and asymmetric encryption
+    """
+
+    def __init__(self, train_config: TrainConfig):
+        """
+        Initialize a KeyManager instance that handles security relevant values based on a train configuration
+
+        :param train_config: either a path to a json file storing the configuration values or a dictionary with these
+            values
+        """
+        self.config = train_config
+
+    def save_config(self, path=None, binary_file=False):
+        """
+        Store the updated config file as a json at the same location
+
+        :return:
+        :rtype:
+        """
+        if binary_file:
+            return BytesIO(self.config.json(indent=2, by_alias=True).encode("utf-8"))
+
+        elif path:
+            with open(path, "w") as f:
+                f.write(self.config.json(indent=2, by_alias=True))
+        else:
+            raise ValueError("No path or binary file specified for saving the keyfile")
+
+    @staticmethod
+    def generate_symmetric_key():
+        """
+        Create a symmetric fernet key for encrypting sensitive files
+        :return:
+        """
+        key = os.urandom(SYMMETRIC_KEY_LENGTH)
+        return key
+
+    def decrypt_symmetric_key(
+        self,
+        encrypted_key: str,
+        private_key_path: str,
+        private_key_password: str = None,
+    ) -> bytes:
+        """
+        Decrypts the symmetric key using a stored private key
+        :arg encrypted_key: the encrypted symmetric key to decrypt in hex format
+        :arg private_key_path: path to the private key file
+        :arg private_key_password: optional password to decrypt the private key
+        :return: symmetric AES key used to encrypt and decrypt files
+        """
+        private_key = self.load_private_key(
+            key_path=private_key_path, password=private_key_password
+        )
+
+        symmetric_key = private_key.decrypt(
+            ciphertext=bytes.fromhex(encrypted_key),
+            padding=padding.OAEP(
+                mgf=padding.MGF1(algorithm=hashes.SHA512()),
+                algorithm=hashes.SHA512(),
+                label=None,
+            ),
+        )
+        return symmetric_key
+
+    def generate_encrypted_keys(self, symmetric_key: bytes):
+        """
+        Generates a dictionary containing the symmetric key used to encrypt files, encrypted with the public keys of all
+        stations on the route
+        :param symmetric_key: byte object containing the symmetric key used to encrypt the mutable files
+        :return: Dictionary consisting of  key = Station Id, value = Symmetric key encrypted with public key of station
+        """
+        enc_keys = {}
+        for station, pk in self.config["rsa_public_keys"]:
+            enc_keys[station] = self.encrypt_symmetric_key(symmetric_key, pk)
+        return enc_keys
+
+    def encrypt_symmetric_key(self, sym_key: bytes, public_key_hex: str) -> str:
+        """
+        Encrypt the symmetric key with all public keys provided in the train configuration file
+
+        :param sym_key: byte object containing the the symmetric key used to encrypt the mutable files
+        :return: dictionary containing the symmetric key encrypted with all available public keys, keys are the station
+        ids and values are the symmetric key encrypted with the RSA public key associated with the station id
+
+        :rtype: str
+        """
+
+        public_key = self.load_public_key(public_key_hex)
+
+        encrypted_key = public_key.encrypt(
+            sym_key,
+            padding.OAEP(
+                mgf=padding.MGF1(algorithm=hashes.SHA512()),
+                algorithm=hashes.SHA512(),
+                label=None,
+            ),
+        )
+        return encrypted_key.hex()
+
+    def _rsa_pk_encrypt(self, val, public_key):
+        encrypted = public_key.encrypt(
+            val,
+            padding.OAEP(
+                mgf=padding.MGF1(algorithm=hashes.SHA512()),
+                algorithm=hashes.SHA512(),
+                label=None,
+            ),
+        )
+        return encrypted.hex()
+
+    @staticmethod
+    def load_private_key(
+        env_key: str = None, key_path: str = None, password: str = None
+    ) -> RSAPrivateKey:
+        """
+        Loads the private key from the path provided provided in the environment variables of the currently
+        running image
+        :param key_path: path to a file containing the private key
+        :param env_key: environment variable containing a hex string representing the station private key
+        :return: a private key object either rsa or ec
+        """
+
+        if env_key and key_path:
+            raise ValueError(
+                f"Multiple private Key locations specified: \n {env_key} \n {key_path}"
+            )
+        # Load key from hex string stored in environment variable
+        if env_key:
+            private_key = serialization.load_pem_private_key(
+                bytes.fromhex(os.getenv(env_key)),
+                password=None,
+                backend=default_backend(),
+            )
+        # Load key from file
+        elif key_path:
+            with open(key_path, "rb") as sk_f:
+                private_key = serialization.load_pem_private_key(
+                    sk_f.read(),
+                    password=password.encode() if password else None,
+                    backend=default_backend(),
+                )
+        else:
+            raise ValueError(
+                "No environment variable or file containing a private key specified"
+            )
+
+        return private_key
+
+    @staticmethod
+    def load_public_key(key: str):
+        """
+        Loads a public key
+        :param key: string representation of a public key
+        :return: public key object for asymmetric encryption
+        """
+        public_key = serialization.load_pem_public_key(
+            bytes.fromhex(key), backend=default_backend()
+        )
+        return public_key
```

### Comparing `pht_train_container_library-2.0.5/train_lib/security/protocol.py` & `pht_train_container_library-2.0.6/train_lib/security/protocol.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,830 +1,830 @@
-import os
-import tarfile
-import time
-from io import BytesIO
-from tarfile import TarInfo
-from typing import BinaryIO, List, Tuple, Union
-
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import padding, utils
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
-from loguru import logger
-
-import docker
-import docker.errors
-import docker.models
-from train_lib.docker_util import TIMEOUT
-from train_lib.docker_util.docker_ops import (
-    display_archive_content,
-    extract_archive,
-    extract_query_json,
-    files_from_archive,
-    rebase_train_image,
-    result_files_from_archive,
-)
-from train_lib.security.constants import TrainPaths
-from train_lib.security.encryption import FileEncryptor
-from train_lib.security.errors import ValidationError
-from train_lib.security.hashing import hash_immutable_files, hash_results
-from train_lib.security.key_manager import KeyManager
-from train_lib.security.train_config import RouteEntry, TrainConfig
-
-
-class SecurityProtocol:
-    """
-    Class that performs the security protocol outlined in the security concept
-
-    :param station_id: PID used to identify the station and to access the correct security values inside the
-        train_config.json
-
-    :type station_id: str
-    :param config: either a string containing a path to the train_config.json or a dictionary containing the values
-        parsed from said json file
-    :param results_dir: path to the directory containing the results
-    :param train_dir: path to the directory containing the immutable files defining a train
-    """
-
-    def __init__(
-        self,
-        station_id: str,
-        config: TrainConfig,
-        results_dir: str = None,
-        train_dir: str = None,
-        docker_client=None,
-    ):
-        self.station_id = station_id
-
-        self.config = config
-        self.route_stop = next(
-            (stop for stop in self.config.route if stop.station == self.station_id),
-            None,
-        )
-        if not self.route_stop:
-            raise ValidationError(f"Station {self.station_id} not found in route")
-        self.key_manager = KeyManager(train_config=config)
-        self.results_dir = results_dir
-        self.train_dir = train_dir
-        self.docker_client = docker_client
-        # self.redis = redis.Redis(decode_responses=True)
-
-    def pre_run_protocol(
-        self,
-        img: str = None,
-        private_key_path: str = None,
-        private_key_password: str = None,
-        immutable_dir: str = "/opt/pht_train",
-        mutable_dir: str = "/opt/pht_results",
-    ):
-        """
-        Decrypts the files contained in the train. And performs the steps necessary to validate a train before it is
-        being run
-
-        :param img: identifier of the image from which the security relevant files will be extracted
-        :param private_key_path:
-        :param private_key_password:
-        :param immutable_dir:
-        :param mutable_dir:
-        :return:
-        """
-        logger.info(
-            f"Executing pre-run protocol at station {self.station_id} for image: {img}"
-        )
-
-        # extract and decrypt symmetric key
-        key = self.key_manager.decrypt_symmetric_key(
-            encrypted_key=self.route_stop.encrypted_key,
-            private_key_path=private_key_path,
-            private_key_password=private_key_password,
-        )
-
-        # Get the content of the immutable files from the image as ByteObjects
-        try:
-            query = extract_query_json(img)
-            logger.info("Query json extracted from image")
-        except Exception as e:
-            logger.warning(f"Error extracting query json from image: {e}")
-            query = None
-
-        try:
-            immutable_files, file_names, query = self.extract_immutable_files(
-                img=img, directory=immutable_dir, symmetric_key=key, query=query
-            )
-        except Exception as e:
-            logger.error(f"Error extracting immutable files from image: {e}")
-            raise ValidationError("Error extracting immutable files from image")
-
-        # Check that no files have been added or removed
-        # assert len(immutable_files) == len(self.config.file_list)
-
-        self.validate_immutable_files(
-            files=immutable_files,
-            immutable_file_names=file_names,
-            ordered_file_list=self.config.file_list,
-            query=query,
-        )
-
-        # add the decrypted files back to the image
-        self._add_train_files(img, immutable_files, file_names, query=query)
-        results_archive = None
-        if not self._is_first_station_on_route():
-            self.verify_digital_signature()
-            file_encryptor = FileEncryptor(key)
-            # Decrypt all previously encrypted files
-            logger.info("Decrypting results files")
-            mutable_files, mf_members, mf_dir = result_files_from_archive(
-                extract_archive(img, mutable_dir)
-            )
-            decrypted_files = file_encryptor.decrypt_files(
-                mutable_files, binary_files=True
-            )
-            self.validate_previous_results(files=decrypted_files)
-            results_archive = self._make_results_archive(
-                mf_dir, mf_members, decrypted_files
-            )
-
-        self._update_image(
-            img,
-            results_archive=results_archive,
-            results_path="/opt",
-            train_files=immutable_files,
-            file_names=file_names,
-            query=query,
-            tag="latest-decrypted",
-        )
-
-        logger.info(f"Successfully executed pre run protocol on img: {img}")
-
-    def post_run_protocol(
-        self,
-        img: str = None,
-        private_key_path: str = None,
-        private_key_password: str = None,
-        rebase: bool = True,
-    ):
-        """
-        Updates the necessary values in the train_config.json and encrypts the updated files after a successful train
-        execution.
-
-        :param img: identifier of the image <repository>:<tag>
-        :param private_key_path: path to the private key associated with the current station and with the corresponding
-            public key registered in vault under the PID chosen by the station
-        :param private_key_password: optional password to decrypt the private key
-        :param rebase: if True the image will be rebased on the latest version of the base image
-        :return:
-        """
-        # execute the post run station side extracting the relevant files from the image
-        logger.info(
-            f"Executing post-run protocol at station {self.station_id} for image: {img}"
-        )
-        # Get the mutable files and tar archive structure
-        mutable_files, mf_members, mf_dir = result_files_from_archive(
-            extract_archive(img, TrainPaths.RESULT_DIR.value)
-        )
-        # Run the post run protocol
-        encrypted_mutable_files, symmetric_key = self._post_run_outside_container(
-            mutable_files, private_key_path, private_key_password
-        )
-        results_archive = self._make_results_archive(
-            mf_dir, mf_members, encrypted_mutable_files
-        )
-        results_archive.seek(0)
-
-        self.config = TrainConfig(**self.config.dict(by_alias=True))
-
-        # get immutable files and query from image
-        query = extract_query_json(img)
-        immutable_files, file_names, query = self.extract_immutable_files(
-            img, TrainPaths.IMMUTABLE_DIR.value, query=query, decrypt=False
-        )
-        # Encrypt the immutable files
-        encrypted_files, query = self.encrypt_immutable_files(
-            immutable_files, symmetric_key, query
-        )
-        # Add the encrypted files to the image
-        # self._add_train_files(img, encrypted_files, file_names, query)
-
-        # update the container with the encrypted files
-        self._update_image(
-            img,
-            results_archive=results_archive,
-            results_path="/opt",
-            config_path="/opt",
-            train_files=encrypted_files,
-            file_names=file_names,
-            query=query,
-        )
-
-        if rebase:
-            base_image = self._get_base_image(img)
-
-            # Rebase the image on the latest version of the base image
-            rebase_train_image(base_image=base_image, train_image=img)
-
-        logger.info(f"Successfully executed post run protocol on img: {img}")
-
-    def extract_immutable_files(
-        self,
-        img: str,
-        directory: str,
-        symmetric_key: bytes = None,
-        query: bytes = None,
-        decrypt: bool = True,
-    ):
-        """
-        Extracts the immutable files from the docker image and saves them to the specified directory
-        :param img: docker image to extract files from
-        :param directory: directory to save the files to
-        :return:
-        """
-        logger.info("Extracting immutable files from image...")
-        # Extract the files from the image
-        immutable_files, file_names = files_from_archive(
-            extract_archive(img, directory)
-        )
-
-        def drop_query_json(file_names, files):
-            query_index = file_names.index("query.json")
-            file_names.pop(query_index)
-            immutable_files.pop(query_index)
-
-        if decrypt:
-            if not symmetric_key:
-                raise ValueError("No symmetric key provided")
-            if query:
-                drop_query_json(file_names, immutable_files)
-            immutable_files, query = self.decrypt_immutable_files(
-                immutable_files, symmetric_key, query
-            )
-        else:
-            if query:
-                drop_query_json(file_names, immutable_files)
-
-        return immutable_files, file_names, query
-
-    def validate_immutable_files(
-        self,
-        train_dir: str = None,
-        files: list = None,
-        ordered_file_list: List[str] = None,
-        immutable_file_names: List[str] = None,
-        query: bytes = None,
-    ):
-        """
-        Checks if the hash of the immutable files is the same as the one stored at the creation of the train
-
-        :raises ValidationError: when the files to be executed do not match the agreed upon files
-
-        :return:
-        """
-        # check the signature of the stored hash value using ec signature verifying that it is created by the user
-        user_pk = self.key_manager.load_public_key(self.config.creator.rsa_public_key)
-        e_h = bytes.fromhex(self.config.hash)
-        e_h_sig = bytes.fromhex(self.config.signature)
-        # now check before the run that no immutable files have changed, based on stored hash
-        if train_dir:
-            immutable_files = self._parse_files(train_dir)
-            immutable_files = [
-                str(file)
-                for file in immutable_files
-                if "train_config.json" not in str(file)
-            ]
-
-            current_hash = hash_immutable_files(
-                immutable_files=immutable_files,
-                user_id=str(self.config.creator.id),
-                session_id=bytes.fromhex(self.config.session_id),
-                query=query,
-            )
-        elif files:
-            current_hash = hash_immutable_files(
-                immutable_files=files,
-                user_id=str(self.config.creator.id),
-                session_id=bytes.fromhex(self.config.session_id),
-                binary_files=True,
-                ordered_file_list=ordered_file_list,
-                immutable_file_names=immutable_file_names,
-                query=query,
-            )
-        else:
-            raise ValueError("Either train_dir or files must be provided")
-
-        logger.info(f"Stored hash: {e_h}")
-        logger.info(f"Current hash: {current_hash}")
-        if e_h != current_hash:
-            raise ValidationError("Immutable Files have changed")
-        # Verify that the hash value corresponds with the signature
-        user_pk.verify(e_h_sig, current_hash, padding.PKCS1v15(), hashes.SHA512())
-        # validate the build signature to ensure no tampering has occurred
-        self.validate_build_signature(current_hash.hex())
-
-    def validate_previous_results(self, files: List[BinaryIO]):
-        """
-        Verify that the results from the execution of the previous station did not change, by hashing the stored results
-        from the previous station and comparing it with the decrypted stored hash from the previous station
-        """
-        # Get public key of the previous station
-        prev_station = self._get_previous_station()
-        station_public_key = self.key_manager.load_public_key(
-            prev_station.rsa_public_key
-        )
-        results_hash = hash_results(
-            files, session_id=bytes.fromhex(self.config.session_id), binary_files=True
-        )
-        if results_hash != bytes.fromhex(self.config.result_hash):
-            raise ValidationError("Previous results have changed")
-        try:
-            station_public_key.verify(
-                signature=bytes.fromhex(self.config.result_signature),
-                data=results_hash,
-                padding=padding.PSS(
-                    mgf=padding.MGF1(hashes.SHA512()),
-                    salt_length=padding.PSS.MAX_LENGTH,
-                ),
-                algorithm=utils.Prehashed(hashes.SHA512()),
-            )
-        except Exception as e:
-            logger.error(f"Error verifying previous results: {e}")
-            raise ValidationError("Error validating previous results signature")
-
-    def sign_digital_signature(self, sk: RSAPrivateKey):
-        """
-        Update the digital signature of the train after successful execution of the train.
-        If there is no previous signature present creates a signature based on the session id, otherwise the
-        signature of the previous station is loaded, signed using the current stations private key and appended to
-        the list of signatures stored in the train.
-
-        :param sk: private key of the currently running station
-        """
-        # ds = self.key_manager.get_security_param("digital_signature")
-        # sort the route by index for signing the signature in order
-        sorted_route = sorted(self.config.route, key=lambda x: x.index)
-
-        hasher = hashes.Hash(hashes.SHA512(), default_backend())
-        # use the session id when first station on route
-        if self.route_stop.index == 0:
-            hasher.update(bytes.fromhex(self.config.session_id))
-        else:
-            for stop in sorted_route:
-                if stop.index < self.route_stop.index:
-                    hasher.update(bytes.fromhex(stop.signature.digest))
-                else:
-                    break
-
-        hasher.update(bytes.fromhex(self.config.result_hash))
-        digest = hasher.finalize()
-        sig = sk.sign(
-            data=digest,
-            padding=padding.PSS(
-                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
-            ),
-            algorithm=utils.Prehashed(hashes.SHA512()),
-        )
-        self.route_stop.signature = {"signature": sig.hex(), "digest": digest.hex()}
-
-        sorted_route[self.route_stop.index] = self.route_stop
-
-        self.config.route = sorted_route
-
-    def verify_digital_signature(self):
-        """
-        Verifies the digital signature of the train by iterating over the list of signatures and verifying each one
-        using the correct public key stored in the train configuration json
-
-        :raise: InvalidSignatureError if any of the signed values can not be validated using the provided public keys
-
-        """
-
-        sorted_route = sorted(self.config.route, key=lambda x: x.index)
-
-        for stop in sorted_route:
-            if stop.index >= self.route_stop.index:
-                break
-            else:
-                if not stop.signature:
-                    error = ValidationError(
-                        f"Missing digital signature for previous stop {stop}. \n"
-                        f" While currently at {self.route_stop}"
-                    )
-                    logger.error(error)
-                    raise error
-                pk = self.key_manager.load_public_key(stop.rsa_public_key)
-                pk.verify(
-                    signature=bytes.fromhex(stop.signature.signature),
-                    data=bytes.fromhex(stop.signature.digest),
-                    padding=padding.PSS(
-                        mgf=padding.MGF1(hashes.SHA512()),
-                        salt_length=padding.PSS.MAX_LENGTH,
-                    ),
-                    algorithm=utils.Prehashed(hashes.SHA512()),
-                )
-
-    def validate_build_signature(self, immutable_file_hash: str):
-        """
-        Validate that the hash of the locally available file corresponds to initial hash provided by the builder
-        in combination with the user signature
-        :param immutable_file_hash:
-        :return:
-        """
-
-        logger.info("Validating build signature... ", nl=False)
-        builder_pk = self.key_manager.load_public_key(self.config.build.rsa_public_key)
-
-        content = immutable_file_hash + self.config.signature
-        try:
-            builder_pk.verify(
-                bytes.fromhex(self.config.build.signature),
-                bytes.fromhex(content),
-                padding.PKCS1v15(),
-                hashes.SHA512(),
-            )
-            logger.info("OK")
-
-        except Exception as e:
-            logger.error(f"Error\n {e}")
-            raise ValidationError("Error validating build signature.")
-
-    def encrypt_immutable_files(
-        self, files: List[BytesIO], symmetric_key: bytes, query=None
-    ):
-        """
-        Encrypts the immutable files
-        :param files: dictionary containing the files to encrypt
-        :param symmetric_key: symmetric key to encrypt the files with
-        :return:
-        """
-        logger.info("Encrypting immutable files...")
-        file_encryptor = FileEncryptor(symmetric_key)
-        encrypted_files = file_encryptor.encrypt_files(files, binary_files=True)
-        if query:
-            encrypted_query = file_encryptor.encrypt(query)
-            return encrypted_files, encrypted_query
-        return encrypted_files, None
-
-    def decrypt_immutable_files(
-        self, immutable_files: List[BinaryIO], symmetric_key: bytes, query: bytes = None
-    ) -> Union[Tuple[List[BytesIO], bytes], Tuple[List[BytesIO], None]]:
-        """
-        Decrypts the immutable files of the train using the private key of the currently running station
-        :param query: optional bytes for query json
-        :param symmetric_key:
-        :param immutable_files: list of binary files to decrypt
-        :return: list of decrypted files
-        """
-
-        fe = FileEncryptor(key=symmetric_key)
-        decrypted_files = fe.decrypt_files(immutable_files, binary_files=True)
-        if query:
-            decrypted_query = fe.decrypt(query)
-            return decrypted_files, decrypted_query
-        return decrypted_files, None
-
-    def _post_run_outside_container(
-        self,
-        mutable_files: List[BytesIO],
-        private_key_path: str,
-        private_key_password: str = None,
-    ) -> Tuple[List[BytesIO], bytes]:
-        """
-        Performs the post run protocol on the mutable files contained in an image. Consisting of encrypting the
-        mutable files and updateing the train_config.json. The extracted mutable files are encrypted and the
-        train_config.json is updated to reflect the current state of the train.
-        The changed files are written to the base image and the resulting image is tagged as latest.
-
-        :param mutable_files: list of BytesIO objects containing the mutable files for a train
-        :param private_key_path: path to private key used to sign the results
-        :return:
-        """
-        logger.info(f"Previous results hash: {self.config.result_hash}")
-        # Update the hash value of the mutable files
-        e_d = hash_results(
-            result_files=mutable_files,
-            session_id=bytes.fromhex(self.config.session_id),
-            binary_files=True,
-        )
-        self.config.result_hash = e_d.hex()
-        logger.info(f"Updated results hash: {self.config.result_hash}")
-
-        # Load the local private key and sign the hash of the results files
-        sk = self.key_manager.load_private_key(
-            key_path=private_key_path, password=private_key_password
-        )
-        e_d_sig = sk.sign(
-            e_d,
-            padding.PSS(
-                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
-            ),
-            utils.Prehashed(hashes.SHA512()),
-        )
-        self.config.result_signature = e_d_sig.hex()
-
-        # Update the digital signature of the train
-        self.sign_digital_signature(sk)
-
-        for file in mutable_files:
-            file.seek(0)
-        # Encrypt the files
-        new_sym_key = self.key_manager.generate_symmetric_key()
-        file_encryptor = FileEncryptor(new_sym_key)
-        encrypted_results = file_encryptor.encrypt_files(
-            mutable_files, binary_files=True
-        )
-
-        # Encrypt the new symmetric key with the available public keys and store them in the image
-        self._update_symmetric_keys(new_sym_key)
-        # at the last station encrypt the symmetric key using the rsa public key of the user
-
-        return encrypted_results, new_sym_key
-
-    def _update_image(
-        self,
-        img: str,
-        results_archive: BytesIO = None,
-        results_path: str = "/opt",
-        config_path: str = None,
-        train_files: List[BytesIO] = None,
-        file_names: List[str] = None,
-        query: bytes = None,
-        tag: str = "latest",
-    ):
-        """
-        Update the base image with the encrypted results files and the updated train_config.json and tag it as
-        latest.
-
-        """
-        # If a config path is given update the train config inside the container
-        client = (
-            self.docker_client
-            if self.docker_client
-            else docker.from_env(timeout=TIMEOUT)
-        )
-        container = client.containers.create(img)
-
-        if config_path:
-            logger.info("Updating train config")
-            config_archive = self._make_train_config_archive()
-            config_archive.seek(0)
-            # add_archive(img, config_archive, config_path)
-            container.put_archive(config_path, config_archive)
-            container.wait()
-        # add the updated results archive
-        if results_archive:
-            logger.info("Adding encrypted result files")
-            results_archive.seek(0)
-            container.put_archive(results_path, results_archive)
-            container.wait()
-        # add_archive(img, results_archive, results_path)
-
-        if self.config.creator.encrypted_key:
-            logger.info("Updating user key file")
-            user_key = self._make_user_key()
-            # add user key to opt directory
-            # add_archive(img, user_key, "/opt")
-            user_key.seek(0)
-            container.put_archive("/opt", user_key)
-            container.wait()
-
-        if train_files:
-            if not file_names:
-                raise ValueError(
-                    "File names must be provided if train files are provided"
-                )
-            logger.info("Adding train archive")
-            train_archive = self._make_train_files_archive(
-                train_files, file_names, query
-            )
-            tar = tarfile.open(fileobj=train_archive, mode="r")
-            display_archive_content(tar)
-
-            train_archive.seek(0)
-            # add the train archive to the image
-            container.put_archive("/opt", train_archive)
-            container.wait()
-
-        # Tag container as latest
-        self._commit_to_image(container, img, tag)
-        container.remove()
-
-    @staticmethod
-    def _make_results_archive(archive_members, file_members, updated_files):
-        """
-        Creates a tar archive containing the updated results
-
-        :param archive_members: tar directory structure of the pht_results directory
-        :param file_members: the members of the archive representing actual files
-        :param updated_files: updated files associated with the file_members that will be written to the archive
-        :return: updated tar archive to be copied into the new image.
-        """
-        archive_obj = BytesIO()
-        tar = tarfile.open(fileobj=archive_obj, mode="w")
-
-        # Create directory structure
-        for member in archive_members:
-            if member not in file_members:
-                tar.addfile(member)
-        # Add the updated members to a new archive
-        for i, file_member in enumerate(file_members):
-            file_size = updated_files[i].getbuffer().nbytes
-            updated_files[i].seek(0)
-            file_member.size = file_size
-            file_member.mtime = time.time()
-            tar.addfile(file_member, fileobj=updated_files[i])
-
-        # Close tarfile and reset BytesIO
-        tar.close()
-        archive_obj.seek(0)
-
-        return archive_obj
-
-    def _add_train_files(
-        self, img: str, train_files: List[BytesIO], file_names: List[str], query=None
-    ):
-        """
-        Create in memory tar archive containing the train files and add it to the image
-        :param img: identifier of the image <repository>:<tag>
-        :param train_files: list of train files
-        :param file_names: names of the train files
-        :return:
-        """
-
-        if query:
-            if isinstance(query, bytes):
-                query = BytesIO(query)
-            elif isinstance(query, BytesIO):
-                pass
-            else:
-                raise TypeError("Query must be of type bytes or BytesIO")
-        train_file_archive = self._make_train_files_archive(
-            train_files=train_files, file_names=file_names, query=query
-        )
-
-        client = (
-            self.docker_client
-            if self.docker_client
-            else docker.from_env(timeout=TIMEOUT)
-        )
-        container = client.containers.create(img)
-        logger.info(f"Adding train files to container: {container.id}")
-        train_file_archive.seek(0)
-        container.put_archive("/opt", train_file_archive)
-        container.wait()
-        logger.info("Done")
-
-    def _commit_to_image(self, container, img, tag: str = "latest"):
-        """
-        Commit the container to the image and remove the container
-        :param container:
-        :param img:
-        :return:
-        """
-
-        # Tag container as latest
-        img_split = img.split(":")
-        if len(img_split) == 1:
-            repo = img_split[0]
-            docker_tag = "latest"
-        elif len(img_split) == 2:
-            repo, docker_tag = img_split
-        else:
-            repo = ":".join(img_split[:-1])
-            docker_tag = img_split[-1]
-
-        logger.debug(
-            f"Committing Container ({container.id}) to image ({repo}:{docker_tag})"
-        )
-        container.commit(repository=repo, tag=docker_tag)
-        container.wait()
-
-    @staticmethod
-    def _make_train_files_archive(
-        train_files: List[BytesIO], file_names: List[str], query: BytesIO = None
-    ) -> BytesIO:
-        """
-        Create a tar archive containing the train files and the query file
-        :param train_files: list of in memory file objects defining the algorithm of the train
-        :param file_names: names of the train files
-        :param query: optional query file
-        :return: Tar archive containing the train files and the query file
-        """
-        archive_obj = BytesIO()
-        tar = tarfile.open(fileobj=archive_obj, mode="w")
-
-        if query:
-            if isinstance(query, bytes):
-                query = BytesIO(query)
-            logger.debug("Adding query file to train archive")
-            query.seek(0)
-            info = TarInfo(name="pht_train/query.json")
-            info.size = query.getbuffer().nbytes
-            info.mtime = time.time()
-            tar.addfile(info, query)
-
-        for i, train_file in enumerate(train_files):
-            name = f"pht_train/{file_names[i]}"
-            train_file.seek(0)
-            logger.debug(f"Adding train file: {name} to archive")
-            train_file.seek(0)
-            info = TarInfo(name=name)
-            info.size = train_file.getbuffer().nbytes
-            info.mtime = time.time()
-            # add config data and reset the archive
-            tar.addfile(info, train_file)
-        tar.close()
-        archive_obj.seek(0)
-
-        return archive_obj
-
-    def _make_train_config_archive(self) -> BytesIO:
-        """
-        Create in memory tar archive containing the train configuration json file
-        :return:
-        """
-        archive_obj = BytesIO()
-        tar = tarfile.open(fileobj=archive_obj, mode="w")
-        data = BytesIO(self.config.json(indent=2, by_alias=True).encode("utf-8"))
-
-        # Create TarInfo Object based on the data
-        info = TarInfo(name="train_config.json")
-        info.size = data.getbuffer().nbytes
-        info.mtime = time.time()
-        # add config data and reset the archive
-        tar.addfile(info, data)
-        tar.close()
-        archive_obj.seek(0)
-        return archive_obj
-
-    def _make_user_key(self):
-        archive_obj = BytesIO()
-        tar = tarfile.open(fileobj=archive_obj, mode="w")
-        # Extract user key from config and convert it to bytesio
-        data = BytesIO(bytes.fromhex(self.config.creator.encrypted_key))
-        info = TarInfo(name="user_sym_key.key")
-        info.size = data.getbuffer().nbytes
-        info.mtime = time.time()
-        tar.addfile(info, data)
-        tar.close()
-        archive_obj.seek(0)
-        return archive_obj
-
-    def _is_first_station_on_route(self) -> bool:
-        """
-        Returns true if current station is the first station on the route
-        :return:
-        """
-        # Check if there are previous results if not station is first station on route
-        return self.config.result_hash is None
-
-    def _get_previous_station(self) -> RouteEntry:
-        for stop in self.config.route:
-            if stop.index == self.route_stop.index - 1:
-                return stop
-
-    @staticmethod
-    def _parse_files(target_dir):
-        """
-        Parses the exported files from a container and sorts them into relevant categories
-        :param target_dir: directory in which to find all files
-        :return: Tuple consisting of lists of paths for the different file types
-        """
-        files = list()
-        logger.info("Detecting files...")
-        for dir_path, dir_names, file_names in os.walk(target_dir):
-            files += [os.path.join(dir_path, file) for file in file_names]
-        logger.info(f"Found {len(files)} Files")
-        return files
-
-    def _update_symmetric_keys(self, new_sym_key: bytes):
-        """
-        Updates the symmetric key for the train creator and all stations on the route
-        :param new_sym_key:
-        :return:
-        """
-        for i, station in enumerate(self.config.route):
-            encrypted_key = self.key_manager.encrypt_symmetric_key(
-                new_sym_key, station.rsa_public_key
-            )
-            self.config.route[i].encrypted_key = encrypted_key
-
-        self.config.creator.encrypted_key = self.key_manager.encrypt_symmetric_key(
-            new_sym_key, self.config.creator.rsa_public_key
-        )
-
-    def _get_base_image(self, img: str) -> str:
-        """
-        Returns the base image of the given image
-        :param img:
-        :return:
-        """
-        client = (
-            self.docker_client
-            if self.docker_client
-            else docker.from_env(timeout=TIMEOUT)
-        )
-        base_image = ":".join(img.split(":")[:-1]) + ":base"
-        try:
-            client.images.get(base_image)
-            return base_image
-        except Exception as e:
-            logger.error(f"Base image {base_image} not found for image {img}")
-            logger.error(e)
-            raise ValueError(f"Base image {base_image} not found for image {img}")
+import os
+import tarfile
+import time
+from io import BytesIO
+from tarfile import TarInfo
+from typing import BinaryIO, List, Tuple, Union
+
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.asymmetric import padding, utils
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+from loguru import logger
+
+import docker
+import docker.errors
+import docker.models
+from train_lib.docker_util import TIMEOUT
+from train_lib.docker_util.docker_ops import (
+    display_archive_content,
+    extract_archive,
+    extract_query_json,
+    files_from_archive,
+    rebase_train_image,
+    result_files_from_archive,
+)
+from train_lib.security.constants import TrainPaths
+from train_lib.security.encryption import FileEncryptor
+from train_lib.security.errors import ValidationError
+from train_lib.security.hashing import hash_immutable_files, hash_results
+from train_lib.security.key_manager import KeyManager
+from train_lib.security.train_config import RouteEntry, TrainConfig
+
+
+class SecurityProtocol:
+    """
+    Class that performs the security protocol outlined in the security concept
+
+    :param station_id: PID used to identify the station and to access the correct security values inside the
+        train_config.json
+
+    :type station_id: str
+    :param config: either a string containing a path to the train_config.json or a dictionary containing the values
+        parsed from said json file
+    :param results_dir: path to the directory containing the results
+    :param train_dir: path to the directory containing the immutable files defining a train
+    """
+
+    def __init__(
+        self,
+        station_id: str,
+        config: TrainConfig,
+        results_dir: str = None,
+        train_dir: str = None,
+        docker_client=None,
+    ):
+        self.station_id = station_id
+
+        self.config = config
+        self.route_stop = next(
+            (stop for stop in self.config.route if stop.station == self.station_id),
+            None,
+        )
+        if not self.route_stop:
+            raise ValidationError(f"Station {self.station_id} not found in route")
+        self.key_manager = KeyManager(train_config=config)
+        self.results_dir = results_dir
+        self.train_dir = train_dir
+        self.docker_client = docker_client
+        # self.redis = redis.Redis(decode_responses=True)
+
+    def pre_run_protocol(
+        self,
+        img: str = None,
+        private_key_path: str = None,
+        private_key_password: str = None,
+        immutable_dir: str = "/opt/pht_train",
+        mutable_dir: str = "/opt/pht_results",
+    ):
+        """
+        Decrypts the files contained in the train. And performs the steps necessary to validate a train before it is
+        being run
+
+        :param img: identifier of the image from which the security relevant files will be extracted
+        :param private_key_path:
+        :param private_key_password:
+        :param immutable_dir:
+        :param mutable_dir:
+        :return:
+        """
+        logger.info(
+            f"Executing pre-run protocol at station {self.station_id} for image: {img}"
+        )
+
+        # extract and decrypt symmetric key
+        key = self.key_manager.decrypt_symmetric_key(
+            encrypted_key=self.route_stop.encrypted_key,
+            private_key_path=private_key_path,
+            private_key_password=private_key_password,
+        )
+
+        # Get the content of the immutable files from the image as ByteObjects
+        try:
+            query = extract_query_json(img)
+            logger.info("Query json extracted from image")
+        except Exception as e:
+            logger.warning(f"Error extracting query json from image: {e}")
+            query = None
+
+        try:
+            immutable_files, file_names, query = self.extract_immutable_files(
+                img=img, directory=immutable_dir, symmetric_key=key, query=query
+            )
+        except Exception as e:
+            logger.error(f"Error extracting immutable files from image: {e}")
+            raise ValidationError("Error extracting immutable files from image")
+
+        # Check that no files have been added or removed
+        # assert len(immutable_files) == len(self.config.file_list)
+
+        self.validate_immutable_files(
+            files=immutable_files,
+            immutable_file_names=file_names,
+            ordered_file_list=self.config.file_list,
+            query=query,
+        )
+
+        # add the decrypted files back to the image
+        self._add_train_files(img, immutable_files, file_names, query=query)
+        results_archive = None
+        if not self._is_first_station_on_route():
+            self.verify_digital_signature()
+            file_encryptor = FileEncryptor(key)
+            # Decrypt all previously encrypted files
+            logger.info("Decrypting results files")
+            mutable_files, mf_members, mf_dir = result_files_from_archive(
+                extract_archive(img, mutable_dir)
+            )
+            decrypted_files = file_encryptor.decrypt_files(
+                mutable_files, binary_files=True
+            )
+            self.validate_previous_results(files=decrypted_files)
+            results_archive = self._make_results_archive(
+                mf_dir, mf_members, decrypted_files
+            )
+
+        self._update_image(
+            img,
+            results_archive=results_archive,
+            results_path="/opt",
+            train_files=immutable_files,
+            file_names=file_names,
+            query=query,
+            tag="latest-decrypted",
+        )
+
+        logger.info(f"Successfully executed pre run protocol on img: {img}")
+
+    def post_run_protocol(
+        self,
+        img: str = None,
+        private_key_path: str = None,
+        private_key_password: str = None,
+        rebase: bool = True,
+    ):
+        """
+        Updates the necessary values in the train_config.json and encrypts the updated files after a successful train
+        execution.
+
+        :param img: identifier of the image <repository>:<tag>
+        :param private_key_path: path to the private key associated with the current station and with the corresponding
+            public key registered in vault under the PID chosen by the station
+        :param private_key_password: optional password to decrypt the private key
+        :param rebase: if True the image will be rebased on the latest version of the base image
+        :return:
+        """
+        # execute the post run station side extracting the relevant files from the image
+        logger.info(
+            f"Executing post-run protocol at station {self.station_id} for image: {img}"
+        )
+        # Get the mutable files and tar archive structure
+        mutable_files, mf_members, mf_dir = result_files_from_archive(
+            extract_archive(img, TrainPaths.RESULT_DIR.value)
+        )
+        # Run the post run protocol
+        encrypted_mutable_files, symmetric_key = self._post_run_outside_container(
+            mutable_files, private_key_path, private_key_password
+        )
+        results_archive = self._make_results_archive(
+            mf_dir, mf_members, encrypted_mutable_files
+        )
+        results_archive.seek(0)
+
+        self.config = TrainConfig(**self.config.dict(by_alias=True))
+
+        # get immutable files and query from image
+        query = extract_query_json(img)
+        immutable_files, file_names, query = self.extract_immutable_files(
+            img, TrainPaths.IMMUTABLE_DIR.value, query=query, decrypt=False
+        )
+        # Encrypt the immutable files
+        encrypted_files, query = self.encrypt_immutable_files(
+            immutable_files, symmetric_key, query
+        )
+        # Add the encrypted files to the image
+        # self._add_train_files(img, encrypted_files, file_names, query)
+
+        # update the container with the encrypted files
+        self._update_image(
+            img,
+            results_archive=results_archive,
+            results_path="/opt",
+            config_path="/opt",
+            train_files=encrypted_files,
+            file_names=file_names,
+            query=query,
+        )
+
+        if rebase:
+            base_image = self._get_base_image(img)
+
+            # Rebase the image on the latest version of the base image
+            rebase_train_image(base_image=base_image, train_image=img)
+
+        logger.info(f"Successfully executed post run protocol on img: {img}")
+
+    def extract_immutable_files(
+        self,
+        img: str,
+        directory: str,
+        symmetric_key: bytes = None,
+        query: bytes = None,
+        decrypt: bool = True,
+    ):
+        """
+        Extracts the immutable files from the docker image and saves them to the specified directory
+        :param img: docker image to extract files from
+        :param directory: directory to save the files to
+        :return:
+        """
+        logger.info("Extracting immutable files from image...")
+        # Extract the files from the image
+        immutable_files, file_names = files_from_archive(
+            extract_archive(img, directory)
+        )
+
+        def drop_query_json(file_names, files):
+            query_index = file_names.index("query.json")
+            file_names.pop(query_index)
+            immutable_files.pop(query_index)
+
+        if decrypt:
+            if not symmetric_key:
+                raise ValueError("No symmetric key provided")
+            if query:
+                drop_query_json(file_names, immutable_files)
+            immutable_files, query = self.decrypt_immutable_files(
+                immutable_files, symmetric_key, query
+            )
+        else:
+            if query:
+                drop_query_json(file_names, immutable_files)
+
+        return immutable_files, file_names, query
+
+    def validate_immutable_files(
+        self,
+        train_dir: str = None,
+        files: list = None,
+        ordered_file_list: List[str] = None,
+        immutable_file_names: List[str] = None,
+        query: bytes = None,
+    ):
+        """
+        Checks if the hash of the immutable files is the same as the one stored at the creation of the train
+
+        :raises ValidationError: when the files to be executed do not match the agreed upon files
+
+        :return:
+        """
+        # check the signature of the stored hash value using ec signature verifying that it is created by the user
+        user_pk = self.key_manager.load_public_key(self.config.creator.rsa_public_key)
+        e_h = bytes.fromhex(self.config.hash)
+        e_h_sig = bytes.fromhex(self.config.signature)
+        # now check before the run that no immutable files have changed, based on stored hash
+        if train_dir:
+            immutable_files = self._parse_files(train_dir)
+            immutable_files = [
+                str(file)
+                for file in immutable_files
+                if "train_config.json" not in str(file)
+            ]
+
+            current_hash = hash_immutable_files(
+                immutable_files=immutable_files,
+                user_id=str(self.config.creator.id),
+                session_id=bytes.fromhex(self.config.session_id),
+                query=query,
+            )
+        elif files:
+            current_hash = hash_immutable_files(
+                immutable_files=files,
+                user_id=str(self.config.creator.id),
+                session_id=bytes.fromhex(self.config.session_id),
+                binary_files=True,
+                ordered_file_list=ordered_file_list,
+                immutable_file_names=immutable_file_names,
+                query=query,
+            )
+        else:
+            raise ValueError("Either train_dir or files must be provided")
+
+        logger.info(f"Stored hash: {e_h}")
+        logger.info(f"Current hash: {current_hash}")
+        if e_h != current_hash:
+            raise ValidationError("Immutable Files have changed")
+        # Verify that the hash value corresponds with the signature
+        user_pk.verify(e_h_sig, current_hash, padding.PKCS1v15(), hashes.SHA512())
+        # validate the build signature to ensure no tampering has occurred
+        self.validate_build_signature(current_hash.hex())
+
+    def validate_previous_results(self, files: List[BinaryIO]):
+        """
+        Verify that the results from the execution of the previous station did not change, by hashing the stored results
+        from the previous station and comparing it with the decrypted stored hash from the previous station
+        """
+        # Get public key of the previous station
+        prev_station = self._get_previous_station()
+        station_public_key = self.key_manager.load_public_key(
+            prev_station.rsa_public_key
+        )
+        results_hash = hash_results(
+            files, session_id=bytes.fromhex(self.config.session_id), binary_files=True
+        )
+        if results_hash != bytes.fromhex(self.config.result_hash):
+            raise ValidationError("Previous results have changed")
+        try:
+            station_public_key.verify(
+                signature=bytes.fromhex(self.config.result_signature),
+                data=results_hash,
+                padding=padding.PSS(
+                    mgf=padding.MGF1(hashes.SHA512()),
+                    salt_length=padding.PSS.MAX_LENGTH,
+                ),
+                algorithm=utils.Prehashed(hashes.SHA512()),
+            )
+        except Exception as e:
+            logger.error(f"Error verifying previous results: {e}")
+            raise ValidationError("Error validating previous results signature")
+
+    def sign_digital_signature(self, sk: RSAPrivateKey):
+        """
+        Update the digital signature of the train after successful execution of the train.
+        If there is no previous signature present creates a signature based on the session id, otherwise the
+        signature of the previous station is loaded, signed using the current stations private key and appended to
+        the list of signatures stored in the train.
+
+        :param sk: private key of the currently running station
+        """
+        # ds = self.key_manager.get_security_param("digital_signature")
+        # sort the route by index for signing the signature in order
+        sorted_route = sorted(self.config.route, key=lambda x: x.index)
+
+        hasher = hashes.Hash(hashes.SHA512(), default_backend())
+        # use the session id when first station on route
+        if self.route_stop.index == 0:
+            hasher.update(bytes.fromhex(self.config.session_id))
+        else:
+            for stop in sorted_route:
+                if stop.index < self.route_stop.index:
+                    hasher.update(bytes.fromhex(stop.signature.digest))
+                else:
+                    break
+
+        hasher.update(bytes.fromhex(self.config.result_hash))
+        digest = hasher.finalize()
+        sig = sk.sign(
+            data=digest,
+            padding=padding.PSS(
+                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
+            ),
+            algorithm=utils.Prehashed(hashes.SHA512()),
+        )
+        self.route_stop.signature = {"signature": sig.hex(), "digest": digest.hex()}
+
+        sorted_route[self.route_stop.index] = self.route_stop
+
+        self.config.route = sorted_route
+
+    def verify_digital_signature(self):
+        """
+        Verifies the digital signature of the train by iterating over the list of signatures and verifying each one
+        using the correct public key stored in the train configuration json
+
+        :raise: InvalidSignatureError if any of the signed values can not be validated using the provided public keys
+
+        """
+
+        sorted_route = sorted(self.config.route, key=lambda x: x.index)
+
+        for stop in sorted_route:
+            if stop.index >= self.route_stop.index:
+                break
+            else:
+                if not stop.signature:
+                    error = ValidationError(
+                        f"Missing digital signature for previous stop {stop}. \n"
+                        f" While currently at {self.route_stop}"
+                    )
+                    logger.error(error)
+                    raise error
+                pk = self.key_manager.load_public_key(stop.rsa_public_key)
+                pk.verify(
+                    signature=bytes.fromhex(stop.signature.signature),
+                    data=bytes.fromhex(stop.signature.digest),
+                    padding=padding.PSS(
+                        mgf=padding.MGF1(hashes.SHA512()),
+                        salt_length=padding.PSS.MAX_LENGTH,
+                    ),
+                    algorithm=utils.Prehashed(hashes.SHA512()),
+                )
+
+    def validate_build_signature(self, immutable_file_hash: str):
+        """
+        Validate that the hash of the locally available file corresponds to initial hash provided by the builder
+        in combination with the user signature
+        :param immutable_file_hash:
+        :return:
+        """
+
+        logger.info("Validating build signature... ", nl=False)
+        builder_pk = self.key_manager.load_public_key(self.config.build.rsa_public_key)
+
+        content = immutable_file_hash + self.config.signature
+        try:
+            builder_pk.verify(
+                bytes.fromhex(self.config.build.signature),
+                bytes.fromhex(content),
+                padding.PKCS1v15(),
+                hashes.SHA512(),
+            )
+            logger.info("OK")
+
+        except Exception as e:
+            logger.error(f"Error\n {e}")
+            raise ValidationError("Error validating build signature.")
+
+    def encrypt_immutable_files(
+        self, files: List[BytesIO], symmetric_key: bytes, query=None
+    ):
+        """
+        Encrypts the immutable files
+        :param files: dictionary containing the files to encrypt
+        :param symmetric_key: symmetric key to encrypt the files with
+        :return:
+        """
+        logger.info("Encrypting immutable files...")
+        file_encryptor = FileEncryptor(symmetric_key)
+        encrypted_files = file_encryptor.encrypt_files(files, binary_files=True)
+        if query:
+            encrypted_query = file_encryptor.encrypt(query)
+            return encrypted_files, encrypted_query
+        return encrypted_files, None
+
+    def decrypt_immutable_files(
+        self, immutable_files: List[BinaryIO], symmetric_key: bytes, query: bytes = None
+    ) -> Union[Tuple[List[BytesIO], bytes], Tuple[List[BytesIO], None]]:
+        """
+        Decrypts the immutable files of the train using the private key of the currently running station
+        :param query: optional bytes for query json
+        :param symmetric_key:
+        :param immutable_files: list of binary files to decrypt
+        :return: list of decrypted files
+        """
+
+        fe = FileEncryptor(key=symmetric_key)
+        decrypted_files = fe.decrypt_files(immutable_files, binary_files=True)
+        if query:
+            decrypted_query = fe.decrypt(query)
+            return decrypted_files, decrypted_query
+        return decrypted_files, None
+
+    def _post_run_outside_container(
+        self,
+        mutable_files: List[BytesIO],
+        private_key_path: str,
+        private_key_password: str = None,
+    ) -> Tuple[List[BytesIO], bytes]:
+        """
+        Performs the post run protocol on the mutable files contained in an image. Consisting of encrypting the
+        mutable files and updateing the train_config.json. The extracted mutable files are encrypted and the
+        train_config.json is updated to reflect the current state of the train.
+        The changed files are written to the base image and the resulting image is tagged as latest.
+
+        :param mutable_files: list of BytesIO objects containing the mutable files for a train
+        :param private_key_path: path to private key used to sign the results
+        :return:
+        """
+        logger.info(f"Previous results hash: {self.config.result_hash}")
+        # Update the hash value of the mutable files
+        e_d = hash_results(
+            result_files=mutable_files,
+            session_id=bytes.fromhex(self.config.session_id),
+            binary_files=True,
+        )
+        self.config.result_hash = e_d.hex()
+        logger.info(f"Updated results hash: {self.config.result_hash}")
+
+        # Load the local private key and sign the hash of the results files
+        sk = self.key_manager.load_private_key(
+            key_path=private_key_path, password=private_key_password
+        )
+        e_d_sig = sk.sign(
+            e_d,
+            padding.PSS(
+                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
+            ),
+            utils.Prehashed(hashes.SHA512()),
+        )
+        self.config.result_signature = e_d_sig.hex()
+
+        # Update the digital signature of the train
+        self.sign_digital_signature(sk)
+
+        for file in mutable_files:
+            file.seek(0)
+        # Encrypt the files
+        new_sym_key = self.key_manager.generate_symmetric_key()
+        file_encryptor = FileEncryptor(new_sym_key)
+        encrypted_results = file_encryptor.encrypt_files(
+            mutable_files, binary_files=True
+        )
+
+        # Encrypt the new symmetric key with the available public keys and store them in the image
+        self._update_symmetric_keys(new_sym_key)
+        # at the last station encrypt the symmetric key using the rsa public key of the user
+
+        return encrypted_results, new_sym_key
+
+    def _update_image(
+        self,
+        img: str,
+        results_archive: BytesIO = None,
+        results_path: str = "/opt",
+        config_path: str = None,
+        train_files: List[BytesIO] = None,
+        file_names: List[str] = None,
+        query: bytes = None,
+        tag: str = "latest",
+    ):
+        """
+        Update the base image with the encrypted results files and the updated train_config.json and tag it as
+        latest.
+
+        """
+        # If a config path is given update the train config inside the container
+        client = (
+            self.docker_client
+            if self.docker_client
+            else docker.from_env(timeout=TIMEOUT)
+        )
+        container = client.containers.create(img)
+
+        if config_path:
+            logger.info("Updating train config")
+            config_archive = self._make_train_config_archive()
+            config_archive.seek(0)
+            # add_archive(img, config_archive, config_path)
+            container.put_archive(config_path, config_archive)
+            container.wait()
+        # add the updated results archive
+        if results_archive:
+            logger.info("Adding encrypted result files")
+            results_archive.seek(0)
+            container.put_archive(results_path, results_archive)
+            container.wait()
+        # add_archive(img, results_archive, results_path)
+
+        if self.config.creator.encrypted_key:
+            logger.info("Updating user key file")
+            user_key = self._make_user_key()
+            # add user key to opt directory
+            # add_archive(img, user_key, "/opt")
+            user_key.seek(0)
+            container.put_archive("/opt", user_key)
+            container.wait()
+
+        if train_files:
+            if not file_names:
+                raise ValueError(
+                    "File names must be provided if train files are provided"
+                )
+            logger.info("Adding train archive")
+            train_archive = self._make_train_files_archive(
+                train_files, file_names, query
+            )
+            tar = tarfile.open(fileobj=train_archive, mode="r")
+            display_archive_content(tar)
+
+            train_archive.seek(0)
+            # add the train archive to the image
+            container.put_archive("/opt", train_archive)
+            container.wait()
+
+        # Tag container as latest
+        self._commit_to_image(container, img, tag)
+        container.remove()
+
+    @staticmethod
+    def _make_results_archive(archive_members, file_members, updated_files):
+        """
+        Creates a tar archive containing the updated results
+
+        :param archive_members: tar directory structure of the pht_results directory
+        :param file_members: the members of the archive representing actual files
+        :param updated_files: updated files associated with the file_members that will be written to the archive
+        :return: updated tar archive to be copied into the new image.
+        """
+        archive_obj = BytesIO()
+        tar = tarfile.open(fileobj=archive_obj, mode="w")
+
+        # Create directory structure
+        for member in archive_members:
+            if member not in file_members:
+                tar.addfile(member)
+        # Add the updated members to a new archive
+        for i, file_member in enumerate(file_members):
+            file_size = updated_files[i].getbuffer().nbytes
+            updated_files[i].seek(0)
+            file_member.size = file_size
+            file_member.mtime = time.time()
+            tar.addfile(file_member, fileobj=updated_files[i])
+
+        # Close tarfile and reset BytesIO
+        tar.close()
+        archive_obj.seek(0)
+
+        return archive_obj
+
+    def _add_train_files(
+        self, img: str, train_files: List[BytesIO], file_names: List[str], query=None
+    ):
+        """
+        Create in memory tar archive containing the train files and add it to the image
+        :param img: identifier of the image <repository>:<tag>
+        :param train_files: list of train files
+        :param file_names: names of the train files
+        :return:
+        """
+
+        if query:
+            if isinstance(query, bytes):
+                query = BytesIO(query)
+            elif isinstance(query, BytesIO):
+                pass
+            else:
+                raise TypeError("Query must be of type bytes or BytesIO")
+        train_file_archive = self._make_train_files_archive(
+            train_files=train_files, file_names=file_names, query=query
+        )
+
+        client = (
+            self.docker_client
+            if self.docker_client
+            else docker.from_env(timeout=TIMEOUT)
+        )
+        container = client.containers.create(img)
+        logger.info(f"Adding train files to container: {container.id}")
+        train_file_archive.seek(0)
+        container.put_archive("/opt", train_file_archive)
+        container.wait()
+        logger.info("Done")
+
+    def _commit_to_image(self, container, img, tag: str = "latest"):
+        """
+        Commit the container to the image and remove the container
+        :param container:
+        :param img:
+        :return:
+        """
+
+        # Tag container as latest
+        img_split = img.split(":")
+        if len(img_split) == 1:
+            repo = img_split[0]
+            docker_tag = "latest"
+        elif len(img_split) == 2:
+            repo, docker_tag = img_split
+        else:
+            repo = ":".join(img_split[:-1])
+            docker_tag = img_split[-1]
+
+        logger.debug(
+            f"Committing Container ({container.id}) to image ({repo}:{docker_tag})"
+        )
+        container.commit(repository=repo, tag=docker_tag)
+        container.wait()
+
+    @staticmethod
+    def _make_train_files_archive(
+        train_files: List[BytesIO], file_names: List[str], query: BytesIO = None
+    ) -> BytesIO:
+        """
+        Create a tar archive containing the train files and the query file
+        :param train_files: list of in memory file objects defining the algorithm of the train
+        :param file_names: names of the train files
+        :param query: optional query file
+        :return: Tar archive containing the train files and the query file
+        """
+        archive_obj = BytesIO()
+        tar = tarfile.open(fileobj=archive_obj, mode="w")
+
+        if query:
+            if isinstance(query, bytes):
+                query = BytesIO(query)
+            logger.debug("Adding query file to train archive")
+            query.seek(0)
+            info = TarInfo(name="pht_train/query.json")
+            info.size = query.getbuffer().nbytes
+            info.mtime = time.time()
+            tar.addfile(info, query)
+
+        for i, train_file in enumerate(train_files):
+            name = f"pht_train/{file_names[i]}"
+            train_file.seek(0)
+            logger.debug(f"Adding train file: {name} to archive")
+            train_file.seek(0)
+            info = TarInfo(name=name)
+            info.size = train_file.getbuffer().nbytes
+            info.mtime = time.time()
+            # add config data and reset the archive
+            tar.addfile(info, train_file)
+        tar.close()
+        archive_obj.seek(0)
+
+        return archive_obj
+
+    def _make_train_config_archive(self) -> BytesIO:
+        """
+        Create in memory tar archive containing the train configuration json file
+        :return:
+        """
+        archive_obj = BytesIO()
+        tar = tarfile.open(fileobj=archive_obj, mode="w")
+        data = BytesIO(self.config.json(indent=2, by_alias=True).encode("utf-8"))
+
+        # Create TarInfo Object based on the data
+        info = TarInfo(name="train_config.json")
+        info.size = data.getbuffer().nbytes
+        info.mtime = time.time()
+        # add config data and reset the archive
+        tar.addfile(info, data)
+        tar.close()
+        archive_obj.seek(0)
+        return archive_obj
+
+    def _make_user_key(self):
+        archive_obj = BytesIO()
+        tar = tarfile.open(fileobj=archive_obj, mode="w")
+        # Extract user key from config and convert it to bytesio
+        data = BytesIO(bytes.fromhex(self.config.creator.encrypted_key))
+        info = TarInfo(name="user_sym_key.key")
+        info.size = data.getbuffer().nbytes
+        info.mtime = time.time()
+        tar.addfile(info, data)
+        tar.close()
+        archive_obj.seek(0)
+        return archive_obj
+
+    def _is_first_station_on_route(self) -> bool:
+        """
+        Returns true if current station is the first station on the route
+        :return:
+        """
+        # Check if there are previous results if not station is first station on route
+        return self.config.result_hash is None
+
+    def _get_previous_station(self) -> RouteEntry:
+        for stop in self.config.route:
+            if stop.index == self.route_stop.index - 1:
+                return stop
+
+    @staticmethod
+    def _parse_files(target_dir):
+        """
+        Parses the exported files from a container and sorts them into relevant categories
+        :param target_dir: directory in which to find all files
+        :return: Tuple consisting of lists of paths for the different file types
+        """
+        files = list()
+        logger.info("Detecting files...")
+        for dir_path, dir_names, file_names in os.walk(target_dir):
+            files += [os.path.join(dir_path, file) for file in file_names]
+        logger.info(f"Found {len(files)} Files")
+        return files
+
+    def _update_symmetric_keys(self, new_sym_key: bytes):
+        """
+        Updates the symmetric key for the train creator and all stations on the route
+        :param new_sym_key:
+        :return:
+        """
+        for i, station in enumerate(self.config.route):
+            encrypted_key = self.key_manager.encrypt_symmetric_key(
+                new_sym_key, station.rsa_public_key
+            )
+            self.config.route[i].encrypted_key = encrypted_key
+
+        self.config.creator.encrypted_key = self.key_manager.encrypt_symmetric_key(
+            new_sym_key, self.config.creator.rsa_public_key
+        )
+
+    def _get_base_image(self, img: str) -> str:
+        """
+        Returns the base image of the given image
+        :param img:
+        :return:
+        """
+        client = (
+            self.docker_client
+            if self.docker_client
+            else docker.from_env(timeout=TIMEOUT)
+        )
+        base_image = ":".join(img.split(":")[:-1]) + ":base"
+        try:
+            client.images.get(base_image)
+            return base_image
+        except Exception as e:
+            logger.error(f"Base image {base_image} not found for image {img}")
+            logger.error(e)
+            raise ValueError(f"Base image {base_image} not found for image {img}")
```

### Comparing `pht_train_container_library-2.0.5/train_lib/tests/conftest.py` & `pht_train_container_library-2.0.6/train_lib/tests/conftest.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-import json
-import os
-import random
-import tarfile
-import time
-from io import BytesIO
-
-import pytest
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding, rsa
-
-import docker
-from train_lib.docker_util import TIMEOUT
-from train_lib.security.encryption import FileEncryptor
-from train_lib.security.hashing import hash_immutable_files
-from train_lib.security.train_config import TrainConfig
-
-
-@pytest.fixture
-def docker_client():
-    try:
-        client = docker.from_env(timeout=TIMEOUT)
-
-    except Exception:
-        client = docker.DockerClient(base_url="unix://var/run/docker.sock")
-
-    return client
-
-
-@pytest.fixture
-def key_pairs():
-    # Create private keys
-    station_1_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-    station_2_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-    station_3_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-    user_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-
-    builder_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-
-    # Create public keys
-
-    station_1_pk = station_1_sk.public_key()
-    station_2_pk = station_2_sk.public_key()
-    station_3_pk = station_3_sk.public_key()
-    user_pk = user_sk.public_key()
-    builder_pk = builder_sk.public_key()
-
-    # serialize the keys to bytes
-
-    station_1_sk = station_1_sk.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-    station_2_sk = station_2_sk.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-    station_3_sk = station_3_sk.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-
-    station_1_pk = station_1_pk.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-    station_2_pk = station_2_pk.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-    station_3_pk = station_3_pk.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-
-    user_sk = user_sk.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-
-    user_pk = user_pk.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-
-    builder_sk = builder_sk.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-
-    builder_pk = builder_pk.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
-
-    key_pairs = {
-        "station_1": {
-            "private_key": station_1_sk.hex(),
-            "public_key": station_1_pk.hex(),
-        },
-        "station_2": {
-            "private_key": station_2_sk.hex(),
-            "public_key": station_2_pk.hex(),
-        },
-        "station_3": {
-            "private_key": station_3_sk.hex(),
-            "public_key": station_3_pk.hex(),
-        },
-        "user": {"private_key": user_sk.hex(), "public_key": user_pk.hex()},
-        "builder": {"private_key": builder_sk.hex(), "public_key": builder_pk.hex()},
-    }
-
-    return key_pairs
-
-
-@pytest.fixture
-def train_files(query_json):
-    entrypoint_file_string = """
-import os
-import random
-import string
-
-
-def generate_random_text_file(filename, size):
-    print("Generating file...")
-    chars = ''.join([random.choice(string.ascii_letters) for i in range(size)])
-    with open("/opt/pht_results/test_result.txt", 'w') as file:
-        file.write(chars)
-
-
-if __name__ == '__main__':
-    # 20 mb
-    FILE_SIZE = 1024 * 1024
-    RESULTS_DIR = "/opt/pht_results"
-    FILE_NAME = "test_result.txt"
-    print(f"Generating a new random file: Size={FILE_SIZE}b")
-
-    generate_random_text_file(os.path.abspath(os.path.join(RESULTS_DIR, FILE_NAME)), FILE_SIZE)
-    with open(os.path.join(RESULTS_DIR, FILE_NAME), "r") as f:
-        print(f.read(200))
-    print("File Generated Successfully")
-    """
-    entrypoint_file = BytesIO(entrypoint_file_string.encode("utf-8"))
-
-    filenames = ["entrypoint.py", "file_1_test.py", "r_script.r", "query.json"]
-    files = [
-        BytesIO(os.urandom(random.randint(100, 500))) for _ in range(len(filenames) - 2)
-    ]
-    files.insert(0, entrypoint_file)
-    files.append(query_json)
-    return filenames, files
-
-
-@pytest.fixture
-def symmetric_key():
-    return b"\xcc\xd3\xd7V\xa5J\x15a-\xa0\xa2+\x88_=X\xb1\xd2=\x9f{!\x95\x07\x14\xf2z\x83WL\x8f\xe4"
-
-
-@pytest.fixture
-def encrypted_symmetric_key(key_pairs, symmetric_key):
-    station_1_pk = serialization.load_pem_public_key(
-        bytes.fromhex(key_pairs["station_1"]["public_key"]),
-        backend=default_backend(),
-    )
-
-    encrypted_key = station_1_pk.encrypt(
-        symmetric_key,
-        padding.OAEP(
-            mgf=padding.MGF1(algorithm=hashes.SHA512()),
-            algorithm=hashes.SHA512(),
-            label=None,
-        ),
-    )
-
-    return encrypted_key
-
-
-@pytest.fixture
-def query_json():
-    minimal_query = {
-        "query": {
-            "resource": "Patient",
-            "parameters": [{"variable": "gender", "condition": "male"}],
-        },
-        "data": {
-            "output_format": "json",
-            "filename": "patients.json",
-            "variables": ["id", "birthDate", "gender"],
-        },
-    }
-    # transform  to BytesIo containing binary json data
-    query = BytesIO(json.dumps(minimal_query, indent=2).encode("utf-8"))
-
-    return query
-
-
-@pytest.fixture
-def train_config(key_pairs, train_files, encrypted_symmetric_key):
-    filenames, files = train_files
-    session_id = os.urandom(64)
-
-    station_public_keys = {
-        "station_1": key_pairs["station_1"]["public_key"],
-        "station_2": key_pairs["station_2"]["public_key"],
-        "station_3": key_pairs["station_3"]["public_key"],
-    }
-
-    user_id = "test-user-id"
-    print("filenames", filenames)
-    immutable_hash = hash_immutable_files(
-        immutable_files=files,
-        binary_files=True,
-        user_id=user_id,
-        session_id=session_id,
-        ordered_file_list=filenames,
-        immutable_file_names=filenames,
-    )
-
-    print("Immutable Hash: ", immutable_hash)
-    # create user signature
-    user_private_key = serialization.load_pem_private_key(
-        bytes.fromhex(key_pairs["user"]["private_key"]),
-        password=None,
-        backend=default_backend(),
-    )
-    user_signature = user_private_key.sign(
-        immutable_hash, padding.PKCS1v15(), hashes.SHA512()
-    )
-
-    # create builder signature
-    builder_private_key = serialization.load_pem_private_key(
-        bytes.fromhex(key_pairs["builder"]["private_key"]),
-        password=None,
-        backend=default_backend(),
-    )
-
-    # create hash of user signature and immutable hash
-
-    build_sig_data = immutable_hash.hex() + user_signature.hex()
-
-    # sign the hash with builder private key
-    builder_signature = builder_private_key.sign(
-        bytes.fromhex(build_sig_data), padding.PKCS1v15(), hashes.SHA512()
-    )
-    filenames_no_query = filenames[:-1]
-
-    config_dict = {
-        "@id": "test_train_id",
-        "session_id": session_id.hex(),
-        "proposal_id": "test_proposal_id",
-        "source": {
-            "type": "docker_repository",
-            "tag": "latest",
-            "address": "test_repository",
-        },
-        "creator": {
-            "id": user_id,
-            "rsa_public_key": key_pairs["user"]["public_key"],
-        },
-        "build": {
-            "signature": builder_signature.hex(),
-            "rsa_public_key": key_pairs["builder"]["public_key"],
-        },
-        "route": [
-            {
-                "station": "station_1",
-                "eco_system": "tue",
-                "rsa_public_key": station_public_keys["station_1"],
-                "index": 0,
-                "encrypted_key": encrypted_symmetric_key.hex(),
-            },
-            {
-                "station": "station_2",
-                "rsa_public_key": station_public_keys["station_2"],
-                "eco_system": "tue",
-                "index": 1,
-            },
-            {
-                "station": "station_3",
-                "rsa_public_key": station_public_keys["station_3"],
-                "eco_system": "tue",
-                "index": 2,
-            },
-        ],
-        "file_list": filenames_no_query,
-        "hash": immutable_hash.hex(),
-        "signature": user_signature.hex(),
-        "@context": {"link": "https://www.w3.org/2018/credentials/v1"},
-    }
-
-    return TrainConfig(**config_dict)
-
-
-@pytest.fixture
-def train_file_archive(train_files, symmetric_key):
-    archive = BytesIO()
-    tar = tarfile.open(fileobj=archive, mode="w")
-
-    file_names, files = train_files
-    # init encryptor with symmetric key
-    encryptor = FileEncryptor(symmetric_key)
-    # encrypt all the files
-    encrypted_files = encryptor.encrypt_files(files, binary_files=True)
-
-    for i, file in enumerate(encrypted_files):
-        file.seek(0)
-        f = tarfile.TarInfo(name=file_names[i])
-        f.size = file.getbuffer().nbytes
-        f.mtime = time.time()
-        # add config data and reset the archive
-        tar.addfile(f, file)
-
-    tar.close()
-    archive.seek(0)
-
-    return archive
-
-
-@pytest.fixture
-def master_image():
-    return "dev-harbor.personalhealthtrain.de/master/python/base:latest"
-
-
-@pytest.fixture
-def train_image(
-    train_config: TrainConfig, train_file_archive, docker_client, master_image
-):
-    docker_file_obj = BytesIO(
-        f"""
-        FROM {master_image}
-        RUN mkdir /opt/pht_results && mkdir /opt/pht_train
-        CMD ["python", "/opt/pht_train/entrypoint.py"]
-        """.encode(
-            "utf-8"
-        )
-    )
-
-    client = docker_client
-    image, build_logs = client.images.build(
-        fileobj=docker_file_obj, tag="sp-test", rm=True, pull=True
-    )
-
-    # Create the train_config archive
-
-    config_archive = BytesIO()
-    tar = tarfile.open(fileobj=config_archive, mode="w")
-    # transform  to bytesIo containing binary json data
-    config = BytesIO(train_config.json(indent=2, by_alias=True).encode("utf-8"))
-
-    # Create TarInfo Object based on the data
-    config_file = tarfile.TarInfo(name="train_config.json")
-    config_file.size = config.getbuffer().nbytes
-    config_file.mtime = time.time()
-    # add config data and reset the archive
-    tar.addfile(config_file, config)
-    tar.close()
-    config_archive.seek(0)
-
-    container = client.containers.create(image)
-    container.put_archive("/opt", config_archive)
-
-    # add train file archive
-    container.put_archive("/opt/pht_train", train_file_archive)
-
-    container.commit("sp-test", tag="latest")
-    container.commit("sp-test", tag="base")
-
-    return "sp-test"
+import json
+import os
+import random
+import tarfile
+import time
+from io import BytesIO
+
+import pytest
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
+
+import docker
+from train_lib.docker_util import TIMEOUT
+from train_lib.security.encryption import FileEncryptor
+from train_lib.security.hashing import hash_immutable_files
+from train_lib.security.train_config import TrainConfig
+
+
+@pytest.fixture
+def docker_client():
+    try:
+        client = docker.from_env(timeout=TIMEOUT)
+
+    except Exception:
+        client = docker.DockerClient(base_url="unix://var/run/docker.sock")
+
+    return client
+
+
+@pytest.fixture
+def key_pairs():
+    # Create private keys
+    station_1_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+    station_2_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+    station_3_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+    user_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+
+    builder_sk = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+
+    # Create public keys
+
+    station_1_pk = station_1_sk.public_key()
+    station_2_pk = station_2_sk.public_key()
+    station_3_pk = station_3_sk.public_key()
+    user_pk = user_sk.public_key()
+    builder_pk = builder_sk.public_key()
+
+    # serialize the keys to bytes
+
+    station_1_sk = station_1_sk.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+    station_2_sk = station_2_sk.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+    station_3_sk = station_3_sk.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+
+    station_1_pk = station_1_pk.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+    station_2_pk = station_2_pk.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+    station_3_pk = station_3_pk.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+
+    user_sk = user_sk.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+
+    user_pk = user_pk.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+
+    builder_sk = builder_sk.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+
+    builder_pk = builder_pk.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo,
+    )
+
+    key_pairs = {
+        "station_1": {
+            "private_key": station_1_sk.hex(),
+            "public_key": station_1_pk.hex(),
+        },
+        "station_2": {
+            "private_key": station_2_sk.hex(),
+            "public_key": station_2_pk.hex(),
+        },
+        "station_3": {
+            "private_key": station_3_sk.hex(),
+            "public_key": station_3_pk.hex(),
+        },
+        "user": {"private_key": user_sk.hex(), "public_key": user_pk.hex()},
+        "builder": {"private_key": builder_sk.hex(), "public_key": builder_pk.hex()},
+    }
+
+    return key_pairs
+
+
+@pytest.fixture
+def train_files(query_json):
+    entrypoint_file_string = """
+import os
+import random
+import string
+
+
+def generate_random_text_file(filename, size):
+    print("Generating file...")
+    chars = ''.join([random.choice(string.ascii_letters) for i in range(size)])
+    with open("/opt/pht_results/test_result.txt", 'w') as file:
+        file.write(chars)
+
+
+if __name__ == '__main__':
+    # 20 mb
+    FILE_SIZE = 1024 * 1024
+    RESULTS_DIR = "/opt/pht_results"
+    FILE_NAME = "test_result.txt"
+    print(f"Generating a new random file: Size={FILE_SIZE}b")
+
+    generate_random_text_file(os.path.abspath(os.path.join(RESULTS_DIR, FILE_NAME)), FILE_SIZE)
+    with open(os.path.join(RESULTS_DIR, FILE_NAME), "r") as f:
+        print(f.read(200))
+    print("File Generated Successfully")
+    """
+    entrypoint_file = BytesIO(entrypoint_file_string.encode("utf-8"))
+
+    filenames = ["entrypoint.py", "file_1_test.py", "r_script.r", "query.json"]
+    files = [
+        BytesIO(os.urandom(random.randint(100, 500))) for _ in range(len(filenames) - 2)
+    ]
+    files.insert(0, entrypoint_file)
+    files.append(query_json)
+    return filenames, files
+
+
+@pytest.fixture
+def symmetric_key():
+    return b"\xcc\xd3\xd7V\xa5J\x15a-\xa0\xa2+\x88_=X\xb1\xd2=\x9f{!\x95\x07\x14\xf2z\x83WL\x8f\xe4"
+
+
+@pytest.fixture
+def encrypted_symmetric_key(key_pairs, symmetric_key):
+    station_1_pk = serialization.load_pem_public_key(
+        bytes.fromhex(key_pairs["station_1"]["public_key"]),
+        backend=default_backend(),
+    )
+
+    encrypted_key = station_1_pk.encrypt(
+        symmetric_key,
+        padding.OAEP(
+            mgf=padding.MGF1(algorithm=hashes.SHA512()),
+            algorithm=hashes.SHA512(),
+            label=None,
+        ),
+    )
+
+    return encrypted_key
+
+
+@pytest.fixture
+def query_json():
+    minimal_query = {
+        "query": {
+            "resource": "Patient",
+            "parameters": [{"variable": "gender", "condition": "male"}],
+        },
+        "data": {
+            "output_format": "json",
+            "filename": "patients.json",
+            "variables": ["id", "birthDate", "gender"],
+        },
+    }
+    # transform  to BytesIo containing binary json data
+    query = BytesIO(json.dumps(minimal_query, indent=2).encode("utf-8"))
+
+    return query
+
+
+@pytest.fixture
+def train_config(key_pairs, train_files, encrypted_symmetric_key):
+    filenames, files = train_files
+    session_id = os.urandom(64)
+
+    station_public_keys = {
+        "station_1": key_pairs["station_1"]["public_key"],
+        "station_2": key_pairs["station_2"]["public_key"],
+        "station_3": key_pairs["station_3"]["public_key"],
+    }
+
+    user_id = "test-user-id"
+    print("filenames", filenames)
+    immutable_hash = hash_immutable_files(
+        immutable_files=files,
+        binary_files=True,
+        user_id=user_id,
+        session_id=session_id,
+        ordered_file_list=filenames,
+        immutable_file_names=filenames,
+    )
+
+    print("Immutable Hash: ", immutable_hash)
+    # create user signature
+    user_private_key = serialization.load_pem_private_key(
+        bytes.fromhex(key_pairs["user"]["private_key"]),
+        password=None,
+        backend=default_backend(),
+    )
+    user_signature = user_private_key.sign(
+        immutable_hash, padding.PKCS1v15(), hashes.SHA512()
+    )
+
+    # create builder signature
+    builder_private_key = serialization.load_pem_private_key(
+        bytes.fromhex(key_pairs["builder"]["private_key"]),
+        password=None,
+        backend=default_backend(),
+    )
+
+    # create hash of user signature and immutable hash
+
+    build_sig_data = immutable_hash.hex() + user_signature.hex()
+
+    # sign the hash with builder private key
+    builder_signature = builder_private_key.sign(
+        bytes.fromhex(build_sig_data), padding.PKCS1v15(), hashes.SHA512()
+    )
+    filenames_no_query = filenames[:-1]
+
+    config_dict = {
+        "@id": "test_train_id",
+        "session_id": session_id.hex(),
+        "proposal_id": "test_proposal_id",
+        "source": {
+            "type": "docker_repository",
+            "tag": "latest",
+            "address": "test_repository",
+        },
+        "creator": {
+            "id": user_id,
+            "rsa_public_key": key_pairs["user"]["public_key"],
+        },
+        "build": {
+            "signature": builder_signature.hex(),
+            "rsa_public_key": key_pairs["builder"]["public_key"],
+        },
+        "route": [
+            {
+                "station": "station_1",
+                "eco_system": "tue",
+                "rsa_public_key": station_public_keys["station_1"],
+                "index": 0,
+                "encrypted_key": encrypted_symmetric_key.hex(),
+            },
+            {
+                "station": "station_2",
+                "rsa_public_key": station_public_keys["station_2"],
+                "eco_system": "tue",
+                "index": 1,
+            },
+            {
+                "station": "station_3",
+                "rsa_public_key": station_public_keys["station_3"],
+                "eco_system": "tue",
+                "index": 2,
+            },
+        ],
+        "file_list": filenames_no_query,
+        "hash": immutable_hash.hex(),
+        "signature": user_signature.hex(),
+        "@context": {"link": "https://www.w3.org/2018/credentials/v1"},
+    }
+
+    return TrainConfig(**config_dict)
+
+
+@pytest.fixture
+def train_file_archive(train_files, symmetric_key):
+    archive = BytesIO()
+    tar = tarfile.open(fileobj=archive, mode="w")
+
+    file_names, files = train_files
+    # init encryptor with symmetric key
+    encryptor = FileEncryptor(symmetric_key)
+    # encrypt all the files
+    encrypted_files = encryptor.encrypt_files(files, binary_files=True)
+
+    for i, file in enumerate(encrypted_files):
+        file.seek(0)
+        f = tarfile.TarInfo(name=file_names[i])
+        f.size = file.getbuffer().nbytes
+        f.mtime = time.time()
+        # add config data and reset the archive
+        tar.addfile(f, file)
+
+    tar.close()
+    archive.seek(0)
+
+    return archive
+
+
+@pytest.fixture
+def master_image():
+    return "dev-harbor.personalhealthtrain.de/master/python/base:latest"
+
+
+@pytest.fixture
+def train_image(
+    train_config: TrainConfig, train_file_archive, docker_client, master_image
+):
+    docker_file_obj = BytesIO(
+        f"""
+        FROM {master_image}
+        RUN mkdir /opt/pht_results && mkdir /opt/pht_train
+        CMD ["python", "/opt/pht_train/entrypoint.py"]
+        """.encode(
+            "utf-8"
+        )
+    )
+
+    client = docker_client
+    image, build_logs = client.images.build(
+        fileobj=docker_file_obj, tag="sp-test", rm=True, pull=True
+    )
+
+    # Create the train_config archive
+
+    config_archive = BytesIO()
+    tar = tarfile.open(fileobj=config_archive, mode="w")
+    # transform  to bytesIo containing binary json data
+    config = BytesIO(train_config.json(indent=2, by_alias=True).encode("utf-8"))
+
+    # Create TarInfo Object based on the data
+    config_file = tarfile.TarInfo(name="train_config.json")
+    config_file.size = config.getbuffer().nbytes
+    config_file.mtime = time.time()
+    # add config data and reset the archive
+    tar.addfile(config_file, config)
+    tar.close()
+    config_archive.seek(0)
+
+    container = client.containers.create(image)
+    container.put_archive("/opt", config_archive)
+
+    # add train file archive
+    container.put_archive("/opt/pht_train", train_file_archive)
+
+    container.commit("sp-test", tag="latest")
+    container.commit("sp-test", tag="base")
+
+    return "sp-test"
```

### Comparing `pht_train_container_library-2.0.5/train_lib/tests/test_fhir_functionality.py` & `pht_train_container_library-2.0.6/train_lib/tests/test_fhir_functionality.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,369 +1,369 @@
-import json
-import os
-from io import BytesIO
-from unittest import mock
-
-import pytest
-from dotenv import find_dotenv, load_dotenv
-
-from train_lib.clients import PHTFhirClient
-from train_lib.clients.fhir import build_query_string, load_query_file
-
-
-@pytest.fixture
-def pht_fhir_client():
-    load_dotenv(find_dotenv())
-    client = PHTFhirClient(
-        server_url=os.getenv("FHIR_SERVER_URL"),
-        username=os.getenv("FHIR_USER"),
-        password=os.getenv("FHIR_PW"),
-        fhir_server_type=os.getenv("FHIR_SERVER_TYPE"),
-        disable_k_anon=True,
-    )
-    return client
-
-
-@pytest.fixture
-def minimal_query():
-    return {
-        "query": {
-            "resource": "Patient",
-            "parameters": [{"variable": "gender", "condition": "male"}],
-        },
-        "data": {
-            "output_format": "json",
-            "filename": "patients.json",
-        },
-    }
-
-
-@pytest.fixture
-def advanced_query():
-    return {
-        "query": {
-            "resource": "Patient",
-            "parameters": [
-                {"variable": "gender", "condition": ["male", "female"]},
-                {"variable": "birthdate", "condition": "gt1980-08-12"},
-            ],
-            "has": [
-                {
-                    "resource": "Observation",
-                    "property": "code",
-                    "params": [
-                        "I63.0",
-                        "I63.1",
-                        "I63.2",
-                        "I63.3",
-                        "I63.4",
-                        "I63.5",
-                        "I63.6",
-                        "I63.7",
-                        "I63.8",
-                        "I63.9",
-                    ],
-                },
-                {"resource": "Condition", "property": "code", "params": "D70.0"},
-            ],
-        },
-        "data": {"output_format": "json", "filename": "patients.json"},
-    }
-
-
-def test_client_from_env():
-    user = "test_user"
-    password = "test_password"
-    token = "test_token"
-    client_id = "test_client_id"
-    client_secret = "test_client_secret"
-    oidc_url = "test_oidc_url"
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": user,
-            "FHIR_PW": password,
-            "FHIR_TOKEN": "",
-        },
-    ):
-        client = PHTFhirClient.from_env()
-
-        assert client.username == user
-        assert client.password == password
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": user,
-            "FHIR_PW": "",
-            "FHIR_TOKEN": "",
-        },
-    ):
-        with pytest.raises(EnvironmentError):
-            client = PHTFhirClient.from_env()
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": "",
-            "FHIR_PW": "",
-            "FHIR_TOKEN": token,
-        },
-    ):
-        client = PHTFhirClient.from_env()
-        assert client.token == token
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": user,
-            "FHIR_PW": "",
-            "FHIR_TOKEN": token,
-        },
-    ):
-        with pytest.raises(EnvironmentError):
-            client = PHTFhirClient.from_env()
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": "",
-            "FHIR_PW": "",
-            "FHIR_TOKEN": "",
-            "CLIENT_ID": client_id,
-            "CLIENT_SECRET": client_secret,
-            "OIDC_PROVIDER_URL": oidc_url,
-        },
-    ):
-        client = PHTFhirClient.from_env()
-
-        assert client.client_id == client_id
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": "",
-            "FHIR_PW": "",
-            "FHIR_TOKEN": "",
-            "CLIENT_ID": client_id,
-            "CLIENT_SECRET": "",
-            "OIDC_PROVIDER_URL": oidc_url,
-        },
-    ):
-        with pytest.raises(EnvironmentError):
-            client = PHTFhirClient.from_env()
-
-    with mock.patch.dict(
-        os.environ,
-        {
-            "FHIR_SERVER_URL": "test_address",
-            "FHIR_USER": "hello",
-            "FHIR_PW": "",
-            "FHIR_TOKEN": "",
-            "CLIENT_ID": client_id,
-            "CLIENT_SECRET": client_secret,
-            "OIDC_PROVIDER_URL": oidc_url,
-        },
-    ):
-        with pytest.raises(EnvironmentError):
-            client = PHTFhirClient.from_env()
-
-
-def test_query_marius(pht_fhir_client: PHTFhirClient):
-    query = {
-        "query": {
-            "resource": "Patient",
-            "parameters": [
-                {"variable": "gender", "condition": "male"},
-                {"variable": "birthdate", "condition": "sa1980-08-12"},
-            ],
-            "has": [
-                {
-                    "resource": "Condition",
-                    "property": "code",
-                    "params": [
-                        "E70.0",
-                        "E70.1",
-                        "E84.0",
-                        "E84.1",
-                        "E84.8",
-                        "E84.80",
-                        "E84.87",
-                        "E84.88",
-                        "E84.9",
-                    ],
-                }
-            ],
-        },
-        "data": {"output_format": "xml", "filename": "patients.xml"},
-    }
-
-    query2 = {
-        "query": {
-            "resource": "Patient",
-            "parameters": [{"variable": "birthdate", "condition": "gt1960-08-12"}],
-            "has": [{"resource": "Condition", "property": "code", "params": ["E70.0"]}],
-        },
-        "data": {"output_format": "xml", "filename": "patients.xml"},
-    }
-    query_string = build_query_string(query["query"])
-    print(query_string)
-    query_string = build_query_string(query2["query"])
-    print(query_string)
-
-
-def test_server_connection(pht_fhir_client: PHTFhirClient):
-    pht_fhir_client.health_check()
-
-
-def test_load_query_json(pht_fhir_client: PHTFhirClient, minimal_query, advanced_query):
-    query_io = BytesIO(json.dumps(minimal_query).encode("utf-8"))
-    minimal_query_dict = pht_fhir_client.read_query_file(query_io)
-
-    assert isinstance(minimal_query_dict, dict)
-    assert minimal_query == minimal_query_dict
-
-    query_io = BytesIO(json.dumps(advanced_query).encode("utf-8"))
-    advanced_query_dict = pht_fhir_client.read_query_file(query_io)
-
-    assert isinstance(advanced_query_dict, dict)
-    assert advanced_query == advanced_query_dict
-
-
-def test_load_query_file(minimal_query, tmp_path):
-    query_str = json.dumps(minimal_query)
-    loaded_query = load_query_file(query_str)
-
-    assert loaded_query == minimal_query
-
-    query_bytes = query_str.encode("utf-8")
-
-    loaded_query = load_query_file(query_bytes)
-
-    assert loaded_query == minimal_query
-
-    p = tmp_path / "query.json"
-    p.write_text(query_str)
-
-    loaded_query = load_query_file(p)
-    assert loaded_query == minimal_query
-
-    loaded_query = load_query_file(str(p))
-
-    assert loaded_query == minimal_query
-
-    with pytest.raises(ValueError):
-        loaded_query = load_query_file(1234567)
-
-
-def test_build_query_string(
-    pht_fhir_client: PHTFhirClient, minimal_query, advanced_query
-):
-    string_query = "Patient?gender=male"
-
-    query_string = build_query_string(minimal_query["query"])
-
-    query_dict = {
-        "query": {
-            "resource": "Patient",
-            "parameters": [
-                {"variable": "gender", "condition": "male"},
-                {"variable": "birthdate", "condition": "sa1980-08-12"},
-            ],
-            "has": [
-                {
-                    "resource": "Observation",
-                    "property": "code",
-                    "params": [
-                        "I63.0",
-                        "I63.1",
-                        "I63.2",
-                        "I63.3",
-                        "I63.4",
-                        "I63.5",
-                        "I63.6",
-                        "I63.7",
-                        "I63.8",
-                        "I63.9",
-                    ],
-                },
-                {
-                    "resource": "Condition",
-                    "property": "code",
-                    "params": [
-                        "D70.0",
-                        "D70.10",
-                        "D70.11",
-                        "D70.11",
-                        "D70.12",
-                        "D70.13",
-                        "D70.14",
-                        "D70.18",
-                        "D70.19",
-                        "D70.3",
-                        "D70.5",
-                        "D70.6",
-                        "D70.7",
-                    ],
-                },
-            ],
-        },
-        "data": {"output_format": "json", "filename": "patients.json"},
-    }
-
-    print(build_query_string(query_dict["query"]))
-
-    assert string_query == query_string
-
-    advanced_query_string = (
-        "Patient?gender=male,female&birthdate=gt1980-08-12&_has:Observation:patient:code=I63.0,"
-        "I63.1,I63.2,I63.3,I63.4,I63.5,I63.6,I63.7,I63.8,I63.9&_has:Condition:patient:code=D70.0"
-    )
-
-    query_string = build_query_string(advanced_query["query"])
-
-    assert advanced_query_string == query_string
-
-
-def test_query_with_client(pht_fhir_client: PHTFhirClient, minimal_query):
-    query_result = pht_fhir_client.execute_query(query=minimal_query)
-    print(query_result)
-    assert query_result
-
-
-def test_query_xml(pht_fhir_client: PHTFhirClient):
-    xml_query = {
-        "query": {"resource": "Patient"},
-        "data": {"output_format": "xml", "filename": "conditions.xml"},
-    }
-    query_result = pht_fhir_client.execute_query(query=xml_query)
-    assert query_result
-    assert isinstance(query_result, str)
-
-    pht_fhir_client.store_query_results(query_result, filename="fhir_results.xml")
-
-    file_content = open("fhir_results.xml", "r").read()
-
-    assert file_content == query_result
-
-    # os.remove("fhir_results.xml")
-
-
-def test_query_json(pht_fhir_client: PHTFhirClient):
-    json_query = {
-        "query": {"resource": "Patient"},
-        "data": {
-            "output_format": "json",
-            "filename": "patients.json",
-        },
-    }
-    query_result = pht_fhir_client.execute_query(query=json_query)
-    assert len(query_result["entry"]) >= 1
-    pht_fhir_client.store_query_results(query_result, filename="patients.json")
-    os.remove("patients.json")
+import json
+import os
+from io import BytesIO
+from unittest import mock
+
+import pytest
+from dotenv import find_dotenv, load_dotenv
+
+from train_lib.clients import PHTFhirClient
+from train_lib.clients.fhir import build_query_string, load_query_file
+
+
+@pytest.fixture
+def pht_fhir_client():
+    load_dotenv(find_dotenv())
+    client = PHTFhirClient(
+        server_url=os.getenv("FHIR_SERVER_URL"),
+        username=os.getenv("FHIR_USER"),
+        password=os.getenv("FHIR_PW"),
+        fhir_server_type=os.getenv("FHIR_SERVER_TYPE"),
+        disable_k_anon=True,
+    )
+    return client
+
+
+@pytest.fixture
+def minimal_query():
+    return {
+        "query": {
+            "resource": "Patient",
+            "parameters": [{"variable": "gender", "condition": "male"}],
+        },
+        "data": {
+            "output_format": "json",
+            "filename": "patients.json",
+        },
+    }
+
+
+@pytest.fixture
+def advanced_query():
+    return {
+        "query": {
+            "resource": "Patient",
+            "parameters": [
+                {"variable": "gender", "condition": ["male", "female"]},
+                {"variable": "birthdate", "condition": "gt1980-08-12"},
+            ],
+            "has": [
+                {
+                    "resource": "Observation",
+                    "property": "code",
+                    "params": [
+                        "I63.0",
+                        "I63.1",
+                        "I63.2",
+                        "I63.3",
+                        "I63.4",
+                        "I63.5",
+                        "I63.6",
+                        "I63.7",
+                        "I63.8",
+                        "I63.9",
+                    ],
+                },
+                {"resource": "Condition", "property": "code", "params": "D70.0"},
+            ],
+        },
+        "data": {"output_format": "json", "filename": "patients.json"},
+    }
+
+
+def test_client_from_env():
+    user = "test_user"
+    password = "test_password"
+    token = "test_token"
+    client_id = "test_client_id"
+    client_secret = "test_client_secret"
+    oidc_url = "test_oidc_url"
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": user,
+            "FHIR_PW": password,
+            "FHIR_TOKEN": "",
+        },
+    ):
+        client = PHTFhirClient.from_env()
+
+        assert client.username == user
+        assert client.password == password
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": user,
+            "FHIR_PW": "",
+            "FHIR_TOKEN": "",
+        },
+    ):
+        with pytest.raises(EnvironmentError):
+            client = PHTFhirClient.from_env()
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": "",
+            "FHIR_PW": "",
+            "FHIR_TOKEN": token,
+        },
+    ):
+        client = PHTFhirClient.from_env()
+        assert client.token == token
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": user,
+            "FHIR_PW": "",
+            "FHIR_TOKEN": token,
+        },
+    ):
+        with pytest.raises(EnvironmentError):
+            client = PHTFhirClient.from_env()
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": "",
+            "FHIR_PW": "",
+            "FHIR_TOKEN": "",
+            "CLIENT_ID": client_id,
+            "CLIENT_SECRET": client_secret,
+            "OIDC_PROVIDER_URL": oidc_url,
+        },
+    ):
+        client = PHTFhirClient.from_env()
+
+        assert client.client_id == client_id
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": "",
+            "FHIR_PW": "",
+            "FHIR_TOKEN": "",
+            "CLIENT_ID": client_id,
+            "CLIENT_SECRET": "",
+            "OIDC_PROVIDER_URL": oidc_url,
+        },
+    ):
+        with pytest.raises(EnvironmentError):
+            client = PHTFhirClient.from_env()
+
+    with mock.patch.dict(
+        os.environ,
+        {
+            "FHIR_SERVER_URL": "test_address",
+            "FHIR_USER": "hello",
+            "FHIR_PW": "",
+            "FHIR_TOKEN": "",
+            "CLIENT_ID": client_id,
+            "CLIENT_SECRET": client_secret,
+            "OIDC_PROVIDER_URL": oidc_url,
+        },
+    ):
+        with pytest.raises(EnvironmentError):
+            client = PHTFhirClient.from_env()
+
+
+def test_query_marius(pht_fhir_client: PHTFhirClient):
+    query = {
+        "query": {
+            "resource": "Patient",
+            "parameters": [
+                {"variable": "gender", "condition": "male"},
+                {"variable": "birthdate", "condition": "sa1980-08-12"},
+            ],
+            "has": [
+                {
+                    "resource": "Condition",
+                    "property": "code",
+                    "params": [
+                        "E70.0",
+                        "E70.1",
+                        "E84.0",
+                        "E84.1",
+                        "E84.8",
+                        "E84.80",
+                        "E84.87",
+                        "E84.88",
+                        "E84.9",
+                    ],
+                }
+            ],
+        },
+        "data": {"output_format": "xml", "filename": "patients.xml"},
+    }
+
+    query2 = {
+        "query": {
+            "resource": "Patient",
+            "parameters": [{"variable": "birthdate", "condition": "gt1960-08-12"}],
+            "has": [{"resource": "Condition", "property": "code", "params": ["E70.0"]}],
+        },
+        "data": {"output_format": "xml", "filename": "patients.xml"},
+    }
+    query_string = build_query_string(query["query"])
+    print(query_string)
+    query_string = build_query_string(query2["query"])
+    print(query_string)
+
+
+def test_server_connection(pht_fhir_client: PHTFhirClient):
+    pht_fhir_client.health_check()
+
+
+def test_load_query_json(pht_fhir_client: PHTFhirClient, minimal_query, advanced_query):
+    query_io = BytesIO(json.dumps(minimal_query).encode("utf-8"))
+    minimal_query_dict = pht_fhir_client.read_query_file(query_io)
+
+    assert isinstance(minimal_query_dict, dict)
+    assert minimal_query == minimal_query_dict
+
+    query_io = BytesIO(json.dumps(advanced_query).encode("utf-8"))
+    advanced_query_dict = pht_fhir_client.read_query_file(query_io)
+
+    assert isinstance(advanced_query_dict, dict)
+    assert advanced_query == advanced_query_dict
+
+
+def test_load_query_file(minimal_query, tmp_path):
+    query_str = json.dumps(minimal_query)
+    loaded_query = load_query_file(query_str)
+
+    assert loaded_query == minimal_query
+
+    query_bytes = query_str.encode("utf-8")
+
+    loaded_query = load_query_file(query_bytes)
+
+    assert loaded_query == minimal_query
+
+    p = tmp_path / "query.json"
+    p.write_text(query_str)
+
+    loaded_query = load_query_file(p)
+    assert loaded_query == minimal_query
+
+    loaded_query = load_query_file(str(p))
+
+    assert loaded_query == minimal_query
+
+    with pytest.raises(ValueError):
+        loaded_query = load_query_file(1234567)
+
+
+def test_build_query_string(
+    pht_fhir_client: PHTFhirClient, minimal_query, advanced_query
+):
+    string_query = "Patient?gender=male"
+
+    query_string = build_query_string(minimal_query["query"])
+
+    query_dict = {
+        "query": {
+            "resource": "Patient",
+            "parameters": [
+                {"variable": "gender", "condition": "male"},
+                {"variable": "birthdate", "condition": "sa1980-08-12"},
+            ],
+            "has": [
+                {
+                    "resource": "Observation",
+                    "property": "code",
+                    "params": [
+                        "I63.0",
+                        "I63.1",
+                        "I63.2",
+                        "I63.3",
+                        "I63.4",
+                        "I63.5",
+                        "I63.6",
+                        "I63.7",
+                        "I63.8",
+                        "I63.9",
+                    ],
+                },
+                {
+                    "resource": "Condition",
+                    "property": "code",
+                    "params": [
+                        "D70.0",
+                        "D70.10",
+                        "D70.11",
+                        "D70.11",
+                        "D70.12",
+                        "D70.13",
+                        "D70.14",
+                        "D70.18",
+                        "D70.19",
+                        "D70.3",
+                        "D70.5",
+                        "D70.6",
+                        "D70.7",
+                    ],
+                },
+            ],
+        },
+        "data": {"output_format": "json", "filename": "patients.json"},
+    }
+
+    print(build_query_string(query_dict["query"]))
+
+    assert string_query == query_string
+
+    advanced_query_string = (
+        "Patient?gender=male,female&birthdate=gt1980-08-12&_has:Observation:patient:code=I63.0,"
+        "I63.1,I63.2,I63.3,I63.4,I63.5,I63.6,I63.7,I63.8,I63.9&_has:Condition:patient:code=D70.0"
+    )
+
+    query_string = build_query_string(advanced_query["query"])
+
+    assert advanced_query_string == query_string
+
+
+def test_query_with_client(pht_fhir_client: PHTFhirClient, minimal_query):
+    query_result = pht_fhir_client.execute_query(query=minimal_query)
+    print(query_result)
+    assert query_result
+
+
+def test_query_xml(pht_fhir_client: PHTFhirClient):
+    xml_query = {
+        "query": {"resource": "Patient"},
+        "data": {"output_format": "xml", "filename": "conditions.xml"},
+    }
+    query_result = pht_fhir_client.execute_query(query=xml_query)
+    assert query_result
+    assert isinstance(query_result, str)
+
+    pht_fhir_client.store_query_results(query_result, filename="fhir_results.xml")
+
+    file_content = open("fhir_results.xml", "r").read()
+
+    assert file_content == query_result
+
+    # os.remove("fhir_results.xml")
+
+
+def test_query_json(pht_fhir_client: PHTFhirClient):
+    json_query = {
+        "query": {"resource": "Patient"},
+        "data": {
+            "output_format": "json",
+            "filename": "patients.json",
+        },
+    }
+    query_result = pht_fhir_client.execute_query(query=json_query)
+    assert len(query_result["entry"]) >= 1
+    pht_fhir_client.store_query_results(query_result, filename="patients.json")
+    os.remove("patients.json")
```

### Comparing `pht_train_container_library-2.0.5/train_lib/tests/test_homomorphic_addition.py` & `pht_train_container_library-2.0.6/train_lib/tests/test_homomorphic_addition.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import random
-
-import pytest
-
-from train_lib.security import homomorphic_addition, primes
-
-
-def test_primes():
-    # small primes
-    assert primes.is_probably_prime(17)
-    assert primes.is_probably_prime(1)
-
-    assert not primes.is_probably_prime(20)
-
-    assert primes.is_probably_prime(46861, k=100)
-
-
-def test_generate_prime():
-    prime = primes.generate_prime(128)
-    assert primes.is_probably_prime(prime)
-
-    prime_with_k = primes.generate_prime(128, 20)
-
-    assert primes.is_probably_prime(prime_with_k)
-
-
-def test_create_public_key():
-    n = random.randint(100, 1000)
-    public_key = homomorphic_addition.PublicKey(n, 12345)
-    assert public_key
-
-    repr_string = f"<PublicKey: {n}>"
-
-    assert str(public_key) == repr_string
-
-
-def test_modulo_inverse():
-    inv_mod_1 = homomorphic_addition.invmod(3, 11)
-
-    assert inv_mod_1 == 4
-
-    with pytest.raises(ValueError):
-        homomorphic_addition.invmod(0, 21312)
-
-    with pytest.raises(ValueError):
-        homomorphic_addition.invmod(14, 12)
-
-
-def test_homomorphic_encrypt():
-    n = 327
-    public_key = homomorphic_addition.PublicKey(n, 12345)
-
-    encrypted = homomorphic_addition.encrypt(public_key, n)
-
-    assert encrypted
-
-    assert encrypted != n
-
-
-def test_encrypted_addition():
-    n = random.randint(5000, 3213123)
-    public_key = homomorphic_addition.PublicKey(n, 12345)
-    a = 32
-    b = 17
-    encrypted_a = homomorphic_addition.encrypt(public_key, a)
-    encrypted_b = homomorphic_addition.encrypt(public_key, b)
-
-    encrypted_add = homomorphic_addition.enc_add(public_key, encrypted_a, encrypted_b)
-
-    assert encrypted_add
-
-
-def test_secure_addition():
-    test_n = random.randint(1000, 100000)
-    test_g = random.randint(1000, 100000)
-    public_key = homomorphic_addition.PublicKey(test_n, test_g)
-    a = 32
-    b = 64
-    encrypted_a = homomorphic_addition.encrypt(public_key, a)
-    encrypted_b = homomorphic_addition.encrypt(public_key, b)
-
-    encrypted_add = homomorphic_addition.enc_add(public_key, encrypted_a, encrypted_b)
-
-    assert encrypted_add
-
-    with pytest.raises(ValueError):
-        added = homomorphic_addition.secure_addition(a, 0, test_n)
-
-    added = homomorphic_addition.secure_addition(a, b, test_n, test_g)
-
-    assert added
-
-    homomorphic_addition.secure_addition(a, b, test_n, test_g)
-
-    added_no_prev = homomorphic_addition.secure_addition(a, None, test_n, test_g)
-
-    assert added_no_prev
+import random
+
+import pytest
+
+from train_lib.security import homomorphic_addition, primes
+
+
+def test_primes():
+    # small primes
+    assert primes.is_probably_prime(17)
+    assert primes.is_probably_prime(1)
+
+    assert not primes.is_probably_prime(20)
+
+    assert primes.is_probably_prime(46861, k=100)
+
+
+def test_generate_prime():
+    prime = primes.generate_prime(128)
+    assert primes.is_probably_prime(prime)
+
+    prime_with_k = primes.generate_prime(128, 20)
+
+    assert primes.is_probably_prime(prime_with_k)
+
+
+def test_create_public_key():
+    n = random.randint(100, 1000)
+    public_key = homomorphic_addition.PublicKey(n, 12345)
+    assert public_key
+
+    repr_string = f"<PublicKey: {n}>"
+
+    assert str(public_key) == repr_string
+
+
+def test_modulo_inverse():
+    inv_mod_1 = homomorphic_addition.invmod(3, 11)
+
+    assert inv_mod_1 == 4
+
+    with pytest.raises(ValueError):
+        homomorphic_addition.invmod(0, 21312)
+
+    with pytest.raises(ValueError):
+        homomorphic_addition.invmod(14, 12)
+
+
+def test_homomorphic_encrypt():
+    n = 327
+    public_key = homomorphic_addition.PublicKey(n, 12345)
+
+    encrypted = homomorphic_addition.encrypt(public_key, n)
+
+    assert encrypted
+
+    assert encrypted != n
+
+
+def test_encrypted_addition():
+    n = random.randint(5000, 3213123)
+    public_key = homomorphic_addition.PublicKey(n, 12345)
+    a = 32
+    b = 17
+    encrypted_a = homomorphic_addition.encrypt(public_key, a)
+    encrypted_b = homomorphic_addition.encrypt(public_key, b)
+
+    encrypted_add = homomorphic_addition.enc_add(public_key, encrypted_a, encrypted_b)
+
+    assert encrypted_add
+
+
+def test_secure_addition():
+    test_n = random.randint(1000, 100000)
+    test_g = random.randint(1000, 100000)
+    public_key = homomorphic_addition.PublicKey(test_n, test_g)
+    a = 32
+    b = 64
+    encrypted_a = homomorphic_addition.encrypt(public_key, a)
+    encrypted_b = homomorphic_addition.encrypt(public_key, b)
+
+    encrypted_add = homomorphic_addition.enc_add(public_key, encrypted_a, encrypted_b)
+
+    assert encrypted_add
+
+    with pytest.raises(ValueError):
+        added = homomorphic_addition.secure_addition(a, 0, test_n)
+
+    added = homomorphic_addition.secure_addition(a, b, test_n, test_g)
+
+    assert added
+
+    homomorphic_addition.secure_addition(a, b, test_n, test_g)
+
+    added_no_prev = homomorphic_addition.secure_addition(a, None, test_n, test_g)
+
+    assert added_no_prev
```

### Comparing `pht_train_container_library-2.0.5/train_lib/tests/test_security_protocol.py` & `pht_train_container_library-2.0.6/train_lib/tests/test_security_protocol.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,660 +1,660 @@
-import os
-import random
-import tarfile
-import time
-from io import BytesIO
-from unittest import mock
-
-import cryptography
-import cryptography.exceptions
-import pytest
-from cryptography import fernet
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding, rsa, utils
-
-from train_lib.docker_util.docker_ops import (
-    extract_archive,
-    extract_train_config,
-    files_from_archive,
-)
-from train_lib.security.errors import ValidationError
-from train_lib.security.protocol import SecurityProtocol
-from train_lib.security.train_config import TrainConfig
-
-
-def test_extract_train_config(train_image, train_files):
-    file_names, files = train_files
-    config = extract_train_config(train_image)
-
-    assert config
-    assert isinstance(config, TrainConfig)
-
-    assert config.file_list == file_names[:-1]
-
-
-def test_get_previous_station(train_config):
-    sp = SecurityProtocol(station_id="station_2", config=train_config)
-    assert sp._get_previous_station().station == "station_1"
-
-
-def test_pre_run_protocol(train_image, tmpdir, key_pairs, docker_client):
-    config = extract_train_config(train_image)
-
-    # Check if any station can execute the pre run protocol on the raw image
-    p1 = tmpdir.join("station_1_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
-
-    # set up temporary env vars
-    environment_dict_station_1 = {
-        "STATION_ID": "station_1",
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-        sp.pre_run_protocol(
-            img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-        )
-
-        files, file_names = files_from_archive(
-            extract_archive(train_image, "/opt/pht_train")
-        )
-        print(f"Files after pre run: {files}")
-        for f in files:
-            print(f"File: {f}")
-            print(f"File content: {f.read()}")
-
-        print(f"File names: {file_names}")
-
-        # check that the session key cannot be changed
-        changed_config_session_key = config.copy()
-        changed_config_session_key.session_id = os.urandom(64).hex()
-
-        with pytest.raises(ValidationError):
-            wrong_sess_key_sp = SecurityProtocol(
-                os.getenv("STATION_ID"),
-                config=changed_config_session_key,
-                docker_client=docker_client,
-            )
-            wrong_sess_key_sp.pre_run_protocol(
-                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-        # check that you can not change the file list
-        changed_file_list_config = config.copy()
-        changed_file_list_config.file_list = [
-            "file_1_test.py",
-            "r_script.r",
-            "query.json",
-        ]
-
-        with pytest.raises(ValidationError):
-            changed_file_list_sp = SecurityProtocol(
-                os.getenv("STATION_ID"),
-                config=changed_file_list_config,
-                docker_client=docker_client,
-            )
-            changed_file_list_sp.pre_run_protocol(
-                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-
-def test_files_changed_pre_run(train_image, tmpdir, key_pairs, docker_client):
-    """
-    The pre-run protocol should fail, when the content of one the immutable files has changed
-    """
-
-    # sp.pre_run_protocol(img=test_train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
-
-    # Change the content of one the immutable files
-    # changed_files_image = docker_client.containers.create(test_train_image)
-    train_file_archive = extract_archive(train_image, "/opt/pht_train")
-    train_files, tf_names = files_from_archive(train_file_archive)
-
-    train_files = [BytesIO(f.read()) for f in train_files]
-    train_files[0] = BytesIO(os.urandom(random.randint(5000, 20000)))
-    # Create a new archive containing the old files and the one changed file
-    archive_obj = BytesIO()
-    tar = tarfile.open(fileobj=archive_obj, mode="w")
-    for i, file in enumerate(train_files):
-        info = tarfile.TarInfo(name=tf_names[i])
-        info.size = file.getbuffer().nbytes
-        info.mtime = time.time()
-        tar.addfile(info, fileobj=file)
-
-    tar.close()
-    archive_obj.seek(0)
-
-    train_container = docker_client.containers.create(train_image)
-    train_container.put_archive("/opt/pht_train", archive_obj)
-    train_container.commit(repository=train_image)
-    train_container.wait()
-    train_container.remove()
-
-    # Get config and initialize pre run protocol
-
-    config = extract_train_config(train_image)
-    p1 = tmpdir.join("station_1_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
-
-    # set up temporary env vars
-    environment_dict_station_1 = {
-        "STATION_ID": "station_1",
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-        # Security protocol should throw a validation error
-        with pytest.raises(ValidationError):
-            sp.pre_run_protocol(
-                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-
-def test_user_signature_verification_pre_run(
-    train_image, tmpdir, key_pairs, docker_client
-):
-    config = extract_train_config(train_image)
-    p1 = tmpdir.join("station_1_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
-
-    # set up temporary env vars
-    environment_dict_station_1 = {
-        "STATION_ID": "station_1",
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        # Generally invalid signature
-        config.signature = os.urandom(64).hex()
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-        with pytest.raises(cryptography.exceptions.InvalidSignature):
-            sp.pre_run_protocol(
-                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-        user_private_key = serialization.load_pem_private_key(
-            bytes.fromhex(key_pairs["user"]["private_key"]),
-            password=None,
-            backend=default_backend(),
-        )
-
-        # Valid signature but wrong underlying hash
-        wrong_hash = hashes.Hash(hashes.SHA512(), backend=default_backend())
-        wrong_hash.update(os.urandom(672))
-        wrong_hash = wrong_hash.finalize()
-        wrong_signature = user_private_key.sign(
-            wrong_hash,
-            padding.PSS(
-                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
-            ),
-            utils.Prehashed(hashes.SHA512()),
-        )
-        config.signature = wrong_signature.hex()
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-        with pytest.raises(cryptography.exceptions.InvalidSignature):
-            sp.pre_run_protocol(
-                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-
-def execute_image_and_post_run_protocol(
-    test_train_image, docker_client, tmpdir, key_pairs, station_id
-):
-    init_config = extract_train_config(test_train_image)
-    # Execute the image
-    client = docker_client
-
-    # Perform post run protocol
-    # if station_id == "station_1":
-    p1 = tmpdir.join("station_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs[station_id]["private_key"]))
-
-    environment_dict_station_1 = {
-        "STATION_ID": station_id,
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-    print(f"Executing train for station: {environment_dict_station_1}")
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=init_config, docker_client=docker_client
-        )
-        sp.pre_run_protocol(
-            img=test_train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-        )
-
-        container = client.containers.run(
-            image=test_train_image + ":latest", detach=True
-        )
-        exit_code = container.wait()["StatusCode"]
-        print(container.logs())
-        assert exit_code == 0
-
-        container.commit(test_train_image + ":latest")
-
-        sp.post_run_protocol(
-            img=test_train_image + ":latest",
-            private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-        )
-    # elif station_id == "station_2":
-    #     p2 = tmpdir.join("station_2_private_key.pem")
-    #     p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
-    #
-    #     environment_dict_station_2 = {
-    #         "STATION_ID": "station_2",
-    #         "STATION_PRIVATE_KEY_PATH": str(p2)
-    #     }
-    #     with mock.patch.dict(os.environ, environment_dict_station_2):
-    #         sp = SecurityProtocol(os.getenv("STATION_ID"), config=init_config, docker_client=docker_client)
-    #         sp.post_run_protocol(img=test_train_image + ":latest",
-    #                              private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
-    #
-    # elif station_id == "station_3":
-    #     p3 = tmpdir.join("station_3_private_key.pem")
-    #     p3.write(bytes.fromhex(key_pairs["station_3"]["private_key"]))
-    #
-    #     environment_dict_station_3 = {
-    #         "STATION_ID": "station_3",
-    #         "STATION_PRIVATE_KEY_PATH": str(p3)
-    #     }
-    #     with mock.patch.dict(os.environ, environment_dict_station_3):
-    #         sp = SecurityProtocol(os.getenv("STATION_ID"), config=init_config, docker_client=docker_client)
-    #         sp.post_run_protocol(img=test_train_image + ":latest",
-    #                              private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
-
-
-def test_digital_signature(train_image, tmpdir, key_pairs, docker_client):
-    image_name = train_image + "-signature"
-    # Create a new image with a different name
-    container = docker_client.containers.create(train_image)
-    container.commit(repository=image_name, tag="latest")
-    container.commit(repository=image_name, tag="base")
-    container.wait()
-    container.remove()
-    image_name += ":latest"
-
-    # pre run station 1
-    p1 = tmpdir.join("station_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
-    environment_dict_station_1 = {
-        "STATION_ID": "station_1",
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-
-    init_config = extract_train_config(image_name)
-
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=init_config, docker_client=docker_client
-        )
-        sp.pre_run_protocol(
-            img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-        )
-
-        container = docker_client.containers.run(image=image_name, detach=True)
-
-        exit_code = container.wait()["StatusCode"]
-        output = container.logs()
-
-        # extract the files from the container
-        # tar_stream, _ = container("/train")
-
-        files, file_names = files_from_archive(
-            extract_archive(train_image, "/opt/pht_train")
-        )
-        print(f"Files: {files}")
-        for f in files:
-            print(f"File: {f}")
-            print(f"File content: {f.read()}")
-
-        print(f"File names: {file_names}")
-
-    print(output.decode("utf-8"))
-    assert exit_code == 0
-
-    container.commit(image_name)
-
-    config = extract_train_config(image_name)
-
-    assert not config.route[0].signature
-
-    assert not config.result_hash
-
-    # # check that the previous stop has signed the image
-    # stop = next((stop for stop in config.route if stop.station == "station_1"), None)
-    # assert stop.signature
-    # pre run station 1
-    p1 = tmpdir.join("station_private_key.pem")
-    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
-    environment_dict_station_1 = {
-        "STATION_ID": "station_1",
-        "STATION_PRIVATE_KEY_PATH": str(p1),
-    }
-
-    with mock.patch.dict(os.environ, environment_dict_station_1):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), docker_client=docker_client, config=config
-        )
-        sp.post_run_protocol(
-            img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-        )
-
-    post_run_config = extract_train_config(image_name)
-
-    assert post_run_config.route[0].signature
-    assert config.result_hash
-
-
-def test_post_run_protocol(train_image, tmpdir, key_pairs, docker_client):
-    init_config = extract_train_config(train_image)
-    execute_image_and_post_run_protocol(
-        test_train_image=train_image,
-        docker_client=docker_client,
-        tmpdir=tmpdir,
-        key_pairs=key_pairs,
-        station_id="station_1",
-    )
-
-    config = extract_train_config(train_image)
-
-    # check that the config has changed as expected
-    assert config != init_config
-
-    # The digital signature changed
-    assert config.result_hash != init_config.result_hash
-
-    assert config.result_signature != init_config.result_signature
-    stop = next((stop for stop in config.route if stop.station == "station_1"), None)
-
-    assert stop.signature.signature
-    assert stop.signature.digest
-
-    # Check that the pre-run protocol works for the next station
-    p2 = tmpdir.join("station_1_private_key.pem")
-    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
-
-    # set up temporary env vars
-    environment_dict_station_2 = {
-        "STATION_ID": "station_2",
-        "STATION_PRIVATE_KEY_PATH": str(p2),
-    }
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-        sp.pre_run_protocol(
-            img=train_image + ":latest",
-            private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-        )
-
-    # Ensure that it does not work with a different private key
-
-    # generate a new private key
-    unregistered_sk = rsa.generate_private_key(
-        public_exponent=65537, key_size=2048
-    ).private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-    p_wrong_key = tmpdir.join("unregistered_private_key.pem")
-    p_wrong_key.write(unregistered_sk)
-
-    assert unregistered_sk not in [
-        bytes.fromhex(key_pairs[f"station_{s}"]["private_key"]) for s in range(1, 4)
-    ]
-
-    environment_dict_wrong_sk = {
-        "STATION_ID": "station_2",
-        "STATION_PRIVATE_KEY_PATH": str(p_wrong_key),
-    }
-    with mock.patch.dict(os.environ, environment_dict_wrong_sk):
-        sp = SecurityProtocol(
-            os.getenv("STATION_ID"), config=config, docker_client=docker_client
-        )
-
-        with pytest.raises(ValueError):
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-    # Change the results file to an unencrypted one and different one
-
-    train_container = docker_client.containers.create(train_image)
-    archive_obj = BytesIO()
-    tar = tarfile.open(fileobj=archive_obj, mode="w")
-    file = BytesIO(os.urandom(7634).hex().encode("utf-8"))
-    info = tarfile.TarInfo(name="test_result.txt")
-    info.size = file.getbuffer().nbytes
-    info.mtime = time.time()
-    tar.addfile(info, fileobj=file)
-
-    tar.close()
-    archive_obj.seek(0)
-
-    train_container.put_archive("/opt/pht_results", archive_obj)
-
-    train_container.commit(repository=train_image)
-    train_container.wait()
-
-    # Should throw error because the results file is not correctly encrypted
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        with pytest.raises(ValidationError):
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"), config=config, docker_client=docker_client
-            )
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-    train_container = docker_client.containers.create(train_image)
-    archive_obj = BytesIO()
-    tar = tarfile.open(fileobj=archive_obj, mode="w")
-
-    wrong_file_bytes = os.urandom(7634).hex().encode("utf-8")
-
-    file = BytesIO(wrong_file_bytes)
-
-    info = tarfile.TarInfo(name="test_result.txt")
-    info.size = file.getbuffer().nbytes
-    info.mtime = time.time()
-    tar.addfile(info, fileobj=file)
-
-    tar.close()
-    archive_obj.seek(0)
-
-    train_container.put_archive("/opt/pht_results", archive_obj)
-
-    train_container.commit(repository=train_image)
-    train_container.wait()
-
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        with pytest.raises(ValidationError):
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"), config=config, docker_client=docker_client
-            )
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-
-def test_post_run_protocol_wrong_symmetric_key(
-    train_image, tmpdir, key_pairs, docker_client
-):
-    execute_image_and_post_run_protocol(
-        test_train_image=train_image,
-        docker_client=docker_client,
-        tmpdir=tmpdir,
-        key_pairs=key_pairs,
-        station_id="station_1",
-    )
-
-    config = extract_train_config(train_image)
-
-    train_container = docker_client.containers.create(train_image)
-    archive_obj = BytesIO()
-    tar = tarfile.open(fileobj=archive_obj, mode="w")
-
-    wrong_file_bytes = os.urandom(7634)
-
-    # Encrypt the results file with a newly created symmetric key
-
-    wrong_fernet = fernet.Fernet(fernet.Fernet.generate_key())
-
-    wrong_file_bytes = wrong_fernet.encrypt(wrong_file_bytes)
-
-    file = BytesIO(wrong_file_bytes)
-
-    info = tarfile.TarInfo(name="test_result.txt")
-    info.size = file.getbuffer().nbytes
-    info.mtime = time.time()
-    tar.addfile(info, fileobj=file)
-
-    tar.close()
-    archive_obj.seek(0)
-
-    train_container.put_archive("/opt/pht_results", archive_obj)
-
-    train_container.commit(repository=train_image)
-    train_container.wait()
-
-    p2 = tmpdir.join("station_2_private_key.pem")
-    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
-    # set up temporary env vars
-    environment_dict_station_2 = {
-        "STATION_ID": "station_2",
-        "STATION_PRIVATE_KEY_PATH": str(p2),
-    }
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        with pytest.raises(ValueError):
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"), config=config, docker_client=docker_client
-            )
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-
-def test_pre_run_protocol_wrong_results_hash(
-    train_image, tmpdir, key_pairs, docker_client
-):
-    execute_image_and_post_run_protocol(
-        test_train_image=train_image,
-        docker_client=docker_client,
-        tmpdir=tmpdir,
-        key_pairs=key_pairs,
-        station_id="station_1",
-    )
-
-    config = extract_train_config(train_image)
-
-    # Change the results hash to a random byte value
-    wrong_hash_config = config.copy()
-    wrong_hash_config.result_hash = os.urandom(52).hex()
-    p2 = tmpdir.join("station_2_private_key.pem")
-    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
-    environment_dict_station_2 = {
-        "STATION_ID": "station_2",
-        "STATION_PRIVATE_KEY_PATH": str(p2),
-    }
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        with pytest.raises(ValidationError):
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"),
-                config=wrong_hash_config,
-                docker_client=docker_client,
-            )
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-    # wrong signature
-    wrong_signature_config = config.copy()
-    wrong_signature_config.result_signature = os.urandom(52).hex()
-    with mock.patch.dict(os.environ, environment_dict_station_2):
-        with pytest.raises(ValidationError):
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"),
-                config=wrong_signature_config,
-                docker_client=docker_client,
-            )
-            sp.pre_run_protocol(
-                img=train_image + ":latest",
-                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
-            )
-
-
-def test_multi_execution_protocol(train_image, tmpdir, key_pairs, docker_client):
-
-    # setup the separate images for the test
-    image_name = train_image + "-multi"
-    container = docker_client.containers.create(train_image)
-    container.commit(repository=image_name, tag="latest")
-    container.commit(repository=image_name, tag="base")
-    container.wait()
-    container.remove()
-    image_name += ":latest"
-
-    # repo, tag = base_image_name.split(":")
-    # container.commit(repository=repo, tag=tag)
-
-    ids = ["station_1", "station_2", "station_3"]
-
-    print("Running train image: " + image_name)
-    for i, station_id in enumerate(ids):
-        config = extract_train_config(image_name)
-        print("Running station: " + station_id)
-        p1 = tmpdir.join("station_private_key.pem")
-        p1.write(bytes.fromhex(key_pairs[station_id]["private_key"]))
-        environment_dict_station = {
-            "STATION_ID": station_id,
-            "STATION_PRIVATE_KEY_PATH": str(p1),
-        }
-        with mock.patch.dict(os.environ, environment_dict_station):
-
-            private_key_path = os.getenv("STATION_PRIVATE_KEY_PATH")
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"), docker_client=docker_client, config=config
-            )
-            sym_key = sp.key_manager.decrypt_symmetric_key(
-                sp.route_stop.encrypted_key, private_key_path=private_key_path
-            )
-            print("Symmetric key: ")
-            print(sym_key)
-            sp.pre_run_protocol(img=image_name, private_key_path=private_key_path)
-            container = docker_client.containers.run(image=image_name, detach=True)
-            exit_code = container.wait()["StatusCode"]
-
-            logs = container.logs()
-            print(logs)
-            assert exit_code == 0
-
-            container.commit(image_name)
-            container.wait()
-
-            # config = extract_train_config(image_name)
-
-            sp = SecurityProtocol(
-                os.getenv("STATION_ID"), docker_client=docker_client, config=config
-            )
-            sp.post_run_protocol(
-                img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
-            )
-
-            post_run_config = extract_train_config(image_name)
-
-            assert post_run_config.route[i].signature
+import os
+import random
+import tarfile
+import time
+from io import BytesIO
+from unittest import mock
+
+import cryptography
+import cryptography.exceptions
+import pytest
+from cryptography import fernet
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding, rsa, utils
+
+from train_lib.docker_util.docker_ops import (
+    extract_archive,
+    extract_train_config,
+    files_from_archive,
+)
+from train_lib.security.errors import ValidationError
+from train_lib.security.protocol import SecurityProtocol
+from train_lib.security.train_config import TrainConfig
+
+
+def test_extract_train_config(train_image, train_files):
+    file_names, files = train_files
+    config = extract_train_config(train_image)
+
+    assert config
+    assert isinstance(config, TrainConfig)
+
+    assert config.file_list == file_names[:-1]
+
+
+def test_get_previous_station(train_config):
+    sp = SecurityProtocol(station_id="station_2", config=train_config)
+    assert sp._get_previous_station().station == "station_1"
+
+
+def test_pre_run_protocol(train_image, tmpdir, key_pairs, docker_client):
+    config = extract_train_config(train_image)
+
+    # Check if any station can execute the pre run protocol on the raw image
+    p1 = tmpdir.join("station_1_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
+
+    # set up temporary env vars
+    environment_dict_station_1 = {
+        "STATION_ID": "station_1",
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+        sp.pre_run_protocol(
+            img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+        )
+
+        files, file_names = files_from_archive(
+            extract_archive(train_image, "/opt/pht_train")
+        )
+        print(f"Files after pre run: {files}")
+        for f in files:
+            print(f"File: {f}")
+            print(f"File content: {f.read()}")
+
+        print(f"File names: {file_names}")
+
+        # check that the session key cannot be changed
+        changed_config_session_key = config.copy()
+        changed_config_session_key.session_id = os.urandom(64).hex()
+
+        with pytest.raises(ValidationError):
+            wrong_sess_key_sp = SecurityProtocol(
+                os.getenv("STATION_ID"),
+                config=changed_config_session_key,
+                docker_client=docker_client,
+            )
+            wrong_sess_key_sp.pre_run_protocol(
+                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+        # check that you can not change the file list
+        changed_file_list_config = config.copy()
+        changed_file_list_config.file_list = [
+            "file_1_test.py",
+            "r_script.r",
+            "query.json",
+        ]
+
+        with pytest.raises(ValidationError):
+            changed_file_list_sp = SecurityProtocol(
+                os.getenv("STATION_ID"),
+                config=changed_file_list_config,
+                docker_client=docker_client,
+            )
+            changed_file_list_sp.pre_run_protocol(
+                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+
+def test_files_changed_pre_run(train_image, tmpdir, key_pairs, docker_client):
+    """
+    The pre-run protocol should fail, when the content of one the immutable files has changed
+    """
+
+    # sp.pre_run_protocol(img=test_train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
+
+    # Change the content of one the immutable files
+    # changed_files_image = docker_client.containers.create(test_train_image)
+    train_file_archive = extract_archive(train_image, "/opt/pht_train")
+    train_files, tf_names = files_from_archive(train_file_archive)
+
+    train_files = [BytesIO(f.read()) for f in train_files]
+    train_files[0] = BytesIO(os.urandom(random.randint(5000, 20000)))
+    # Create a new archive containing the old files and the one changed file
+    archive_obj = BytesIO()
+    tar = tarfile.open(fileobj=archive_obj, mode="w")
+    for i, file in enumerate(train_files):
+        info = tarfile.TarInfo(name=tf_names[i])
+        info.size = file.getbuffer().nbytes
+        info.mtime = time.time()
+        tar.addfile(info, fileobj=file)
+
+    tar.close()
+    archive_obj.seek(0)
+
+    train_container = docker_client.containers.create(train_image)
+    train_container.put_archive("/opt/pht_train", archive_obj)
+    train_container.commit(repository=train_image)
+    train_container.wait()
+    train_container.remove()
+
+    # Get config and initialize pre run protocol
+
+    config = extract_train_config(train_image)
+    p1 = tmpdir.join("station_1_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
+
+    # set up temporary env vars
+    environment_dict_station_1 = {
+        "STATION_ID": "station_1",
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+        # Security protocol should throw a validation error
+        with pytest.raises(ValidationError):
+            sp.pre_run_protocol(
+                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+
+def test_user_signature_verification_pre_run(
+    train_image, tmpdir, key_pairs, docker_client
+):
+    config = extract_train_config(train_image)
+    p1 = tmpdir.join("station_1_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
+
+    # set up temporary env vars
+    environment_dict_station_1 = {
+        "STATION_ID": "station_1",
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        # Generally invalid signature
+        config.signature = os.urandom(64).hex()
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+        with pytest.raises(cryptography.exceptions.InvalidSignature):
+            sp.pre_run_protocol(
+                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+        user_private_key = serialization.load_pem_private_key(
+            bytes.fromhex(key_pairs["user"]["private_key"]),
+            password=None,
+            backend=default_backend(),
+        )
+
+        # Valid signature but wrong underlying hash
+        wrong_hash = hashes.Hash(hashes.SHA512(), backend=default_backend())
+        wrong_hash.update(os.urandom(672))
+        wrong_hash = wrong_hash.finalize()
+        wrong_signature = user_private_key.sign(
+            wrong_hash,
+            padding.PSS(
+                mgf=padding.MGF1(hashes.SHA512()), salt_length=padding.PSS.MAX_LENGTH
+            ),
+            utils.Prehashed(hashes.SHA512()),
+        )
+        config.signature = wrong_signature.hex()
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+        with pytest.raises(cryptography.exceptions.InvalidSignature):
+            sp.pre_run_protocol(
+                img=train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+
+def execute_image_and_post_run_protocol(
+    test_train_image, docker_client, tmpdir, key_pairs, station_id
+):
+    init_config = extract_train_config(test_train_image)
+    # Execute the image
+    client = docker_client
+
+    # Perform post run protocol
+    # if station_id == "station_1":
+    p1 = tmpdir.join("station_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs[station_id]["private_key"]))
+
+    environment_dict_station_1 = {
+        "STATION_ID": station_id,
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+    print(f"Executing train for station: {environment_dict_station_1}")
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=init_config, docker_client=docker_client
+        )
+        sp.pre_run_protocol(
+            img=test_train_image, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+        )
+
+        container = client.containers.run(
+            image=test_train_image + ":latest", detach=True
+        )
+        exit_code = container.wait()["StatusCode"]
+        print(container.logs())
+        assert exit_code == 0
+
+        container.commit(test_train_image + ":latest")
+
+        sp.post_run_protocol(
+            img=test_train_image + ":latest",
+            private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+        )
+    # elif station_id == "station_2":
+    #     p2 = tmpdir.join("station_2_private_key.pem")
+    #     p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
+    #
+    #     environment_dict_station_2 = {
+    #         "STATION_ID": "station_2",
+    #         "STATION_PRIVATE_KEY_PATH": str(p2)
+    #     }
+    #     with mock.patch.dict(os.environ, environment_dict_station_2):
+    #         sp = SecurityProtocol(os.getenv("STATION_ID"), config=init_config, docker_client=docker_client)
+    #         sp.post_run_protocol(img=test_train_image + ":latest",
+    #                              private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
+    #
+    # elif station_id == "station_3":
+    #     p3 = tmpdir.join("station_3_private_key.pem")
+    #     p3.write(bytes.fromhex(key_pairs["station_3"]["private_key"]))
+    #
+    #     environment_dict_station_3 = {
+    #         "STATION_ID": "station_3",
+    #         "STATION_PRIVATE_KEY_PATH": str(p3)
+    #     }
+    #     with mock.patch.dict(os.environ, environment_dict_station_3):
+    #         sp = SecurityProtocol(os.getenv("STATION_ID"), config=init_config, docker_client=docker_client)
+    #         sp.post_run_protocol(img=test_train_image + ":latest",
+    #                              private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"))
+
+
+def test_digital_signature(train_image, tmpdir, key_pairs, docker_client):
+    image_name = train_image + "-signature"
+    # Create a new image with a different name
+    container = docker_client.containers.create(train_image)
+    container.commit(repository=image_name, tag="latest")
+    container.commit(repository=image_name, tag="base")
+    container.wait()
+    container.remove()
+    image_name += ":latest"
+
+    # pre run station 1
+    p1 = tmpdir.join("station_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
+    environment_dict_station_1 = {
+        "STATION_ID": "station_1",
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+
+    init_config = extract_train_config(image_name)
+
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=init_config, docker_client=docker_client
+        )
+        sp.pre_run_protocol(
+            img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+        )
+
+        container = docker_client.containers.run(image=image_name, detach=True)
+
+        exit_code = container.wait()["StatusCode"]
+        output = container.logs()
+
+        # extract the files from the container
+        # tar_stream, _ = container("/train")
+
+        files, file_names = files_from_archive(
+            extract_archive(train_image, "/opt/pht_train")
+        )
+        print(f"Files: {files}")
+        for f in files:
+            print(f"File: {f}")
+            print(f"File content: {f.read()}")
+
+        print(f"File names: {file_names}")
+
+    print(output.decode("utf-8"))
+    assert exit_code == 0
+
+    container.commit(image_name)
+
+    config = extract_train_config(image_name)
+
+    assert not config.route[0].signature
+
+    assert not config.result_hash
+
+    # # check that the previous stop has signed the image
+    # stop = next((stop for stop in config.route if stop.station == "station_1"), None)
+    # assert stop.signature
+    # pre run station 1
+    p1 = tmpdir.join("station_private_key.pem")
+    p1.write(bytes.fromhex(key_pairs["station_1"]["private_key"]))
+    environment_dict_station_1 = {
+        "STATION_ID": "station_1",
+        "STATION_PRIVATE_KEY_PATH": str(p1),
+    }
+
+    with mock.patch.dict(os.environ, environment_dict_station_1):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), docker_client=docker_client, config=config
+        )
+        sp.post_run_protocol(
+            img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+        )
+
+    post_run_config = extract_train_config(image_name)
+
+    assert post_run_config.route[0].signature
+    assert config.result_hash
+
+
+def test_post_run_protocol(train_image, tmpdir, key_pairs, docker_client):
+    init_config = extract_train_config(train_image)
+    execute_image_and_post_run_protocol(
+        test_train_image=train_image,
+        docker_client=docker_client,
+        tmpdir=tmpdir,
+        key_pairs=key_pairs,
+        station_id="station_1",
+    )
+
+    config = extract_train_config(train_image)
+
+    # check that the config has changed as expected
+    assert config != init_config
+
+    # The digital signature changed
+    assert config.result_hash != init_config.result_hash
+
+    assert config.result_signature != init_config.result_signature
+    stop = next((stop for stop in config.route if stop.station == "station_1"), None)
+
+    assert stop.signature.signature
+    assert stop.signature.digest
+
+    # Check that the pre-run protocol works for the next station
+    p2 = tmpdir.join("station_1_private_key.pem")
+    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
+
+    # set up temporary env vars
+    environment_dict_station_2 = {
+        "STATION_ID": "station_2",
+        "STATION_PRIVATE_KEY_PATH": str(p2),
+    }
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+        sp.pre_run_protocol(
+            img=train_image + ":latest",
+            private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+        )
+
+    # Ensure that it does not work with a different private key
+
+    # generate a new private key
+    unregistered_sk = rsa.generate_private_key(
+        public_exponent=65537, key_size=2048
+    ).private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.TraditionalOpenSSL,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+    p_wrong_key = tmpdir.join("unregistered_private_key.pem")
+    p_wrong_key.write(unregistered_sk)
+
+    assert unregistered_sk not in [
+        bytes.fromhex(key_pairs[f"station_{s}"]["private_key"]) for s in range(1, 4)
+    ]
+
+    environment_dict_wrong_sk = {
+        "STATION_ID": "station_2",
+        "STATION_PRIVATE_KEY_PATH": str(p_wrong_key),
+    }
+    with mock.patch.dict(os.environ, environment_dict_wrong_sk):
+        sp = SecurityProtocol(
+            os.getenv("STATION_ID"), config=config, docker_client=docker_client
+        )
+
+        with pytest.raises(ValueError):
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+    # Change the results file to an unencrypted one and different one
+
+    train_container = docker_client.containers.create(train_image)
+    archive_obj = BytesIO()
+    tar = tarfile.open(fileobj=archive_obj, mode="w")
+    file = BytesIO(os.urandom(7634).hex().encode("utf-8"))
+    info = tarfile.TarInfo(name="test_result.txt")
+    info.size = file.getbuffer().nbytes
+    info.mtime = time.time()
+    tar.addfile(info, fileobj=file)
+
+    tar.close()
+    archive_obj.seek(0)
+
+    train_container.put_archive("/opt/pht_results", archive_obj)
+
+    train_container.commit(repository=train_image)
+    train_container.wait()
+
+    # Should throw error because the results file is not correctly encrypted
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        with pytest.raises(ValidationError):
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"), config=config, docker_client=docker_client
+            )
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+    train_container = docker_client.containers.create(train_image)
+    archive_obj = BytesIO()
+    tar = tarfile.open(fileobj=archive_obj, mode="w")
+
+    wrong_file_bytes = os.urandom(7634).hex().encode("utf-8")
+
+    file = BytesIO(wrong_file_bytes)
+
+    info = tarfile.TarInfo(name="test_result.txt")
+    info.size = file.getbuffer().nbytes
+    info.mtime = time.time()
+    tar.addfile(info, fileobj=file)
+
+    tar.close()
+    archive_obj.seek(0)
+
+    train_container.put_archive("/opt/pht_results", archive_obj)
+
+    train_container.commit(repository=train_image)
+    train_container.wait()
+
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        with pytest.raises(ValidationError):
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"), config=config, docker_client=docker_client
+            )
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+
+def test_post_run_protocol_wrong_symmetric_key(
+    train_image, tmpdir, key_pairs, docker_client
+):
+    execute_image_and_post_run_protocol(
+        test_train_image=train_image,
+        docker_client=docker_client,
+        tmpdir=tmpdir,
+        key_pairs=key_pairs,
+        station_id="station_1",
+    )
+
+    config = extract_train_config(train_image)
+
+    train_container = docker_client.containers.create(train_image)
+    archive_obj = BytesIO()
+    tar = tarfile.open(fileobj=archive_obj, mode="w")
+
+    wrong_file_bytes = os.urandom(7634)
+
+    # Encrypt the results file with a newly created symmetric key
+
+    wrong_fernet = fernet.Fernet(fernet.Fernet.generate_key())
+
+    wrong_file_bytes = wrong_fernet.encrypt(wrong_file_bytes)
+
+    file = BytesIO(wrong_file_bytes)
+
+    info = tarfile.TarInfo(name="test_result.txt")
+    info.size = file.getbuffer().nbytes
+    info.mtime = time.time()
+    tar.addfile(info, fileobj=file)
+
+    tar.close()
+    archive_obj.seek(0)
+
+    train_container.put_archive("/opt/pht_results", archive_obj)
+
+    train_container.commit(repository=train_image)
+    train_container.wait()
+
+    p2 = tmpdir.join("station_2_private_key.pem")
+    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
+    # set up temporary env vars
+    environment_dict_station_2 = {
+        "STATION_ID": "station_2",
+        "STATION_PRIVATE_KEY_PATH": str(p2),
+    }
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        with pytest.raises(ValueError):
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"), config=config, docker_client=docker_client
+            )
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+
+def test_pre_run_protocol_wrong_results_hash(
+    train_image, tmpdir, key_pairs, docker_client
+):
+    execute_image_and_post_run_protocol(
+        test_train_image=train_image,
+        docker_client=docker_client,
+        tmpdir=tmpdir,
+        key_pairs=key_pairs,
+        station_id="station_1",
+    )
+
+    config = extract_train_config(train_image)
+
+    # Change the results hash to a random byte value
+    wrong_hash_config = config.copy()
+    wrong_hash_config.result_hash = os.urandom(52).hex()
+    p2 = tmpdir.join("station_2_private_key.pem")
+    p2.write(bytes.fromhex(key_pairs["station_2"]["private_key"]))
+    environment_dict_station_2 = {
+        "STATION_ID": "station_2",
+        "STATION_PRIVATE_KEY_PATH": str(p2),
+    }
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        with pytest.raises(ValidationError):
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"),
+                config=wrong_hash_config,
+                docker_client=docker_client,
+            )
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+    # wrong signature
+    wrong_signature_config = config.copy()
+    wrong_signature_config.result_signature = os.urandom(52).hex()
+    with mock.patch.dict(os.environ, environment_dict_station_2):
+        with pytest.raises(ValidationError):
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"),
+                config=wrong_signature_config,
+                docker_client=docker_client,
+            )
+            sp.pre_run_protocol(
+                img=train_image + ":latest",
+                private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH"),
+            )
+
+
+def test_multi_execution_protocol(train_image, tmpdir, key_pairs, docker_client):
+
+    # setup the separate images for the test
+    image_name = train_image + "-multi"
+    container = docker_client.containers.create(train_image)
+    container.commit(repository=image_name, tag="latest")
+    container.commit(repository=image_name, tag="base")
+    container.wait()
+    container.remove()
+    image_name += ":latest"
+
+    # repo, tag = base_image_name.split(":")
+    # container.commit(repository=repo, tag=tag)
+
+    ids = ["station_1", "station_2", "station_3"]
+
+    print("Running train image: " + image_name)
+    for i, station_id in enumerate(ids):
+        config = extract_train_config(image_name)
+        print("Running station: " + station_id)
+        p1 = tmpdir.join("station_private_key.pem")
+        p1.write(bytes.fromhex(key_pairs[station_id]["private_key"]))
+        environment_dict_station = {
+            "STATION_ID": station_id,
+            "STATION_PRIVATE_KEY_PATH": str(p1),
+        }
+        with mock.patch.dict(os.environ, environment_dict_station):
+
+            private_key_path = os.getenv("STATION_PRIVATE_KEY_PATH")
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"), docker_client=docker_client, config=config
+            )
+            sym_key = sp.key_manager.decrypt_symmetric_key(
+                sp.route_stop.encrypted_key, private_key_path=private_key_path
+            )
+            print("Symmetric key: ")
+            print(sym_key)
+            sp.pre_run_protocol(img=image_name, private_key_path=private_key_path)
+            container = docker_client.containers.run(image=image_name, detach=True)
+            exit_code = container.wait()["StatusCode"]
+
+            logs = container.logs()
+            print(logs)
+            assert exit_code == 0
+
+            container.commit(image_name)
+            container.wait()
+
+            # config = extract_train_config(image_name)
+
+            sp = SecurityProtocol(
+                os.getenv("STATION_ID"), docker_client=docker_client, config=config
+            )
+            sp.post_run_protocol(
+                img=image_name, private_key_path=os.getenv("STATION_PRIVATE_KEY_PATH")
+            )
+
+            post_run_config = extract_train_config(image_name)
+
+            assert post_run_config.route[i].signature
```

### Comparing `pht_train_container_library-2.0.5/train_lib/tests/test_validate_master_image.py` & `pht_train_container_library-2.0.6/train_lib/tests/test_validate_master_image.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,192 +1,217 @@
-import tarfile
-import time
-from io import BytesIO
-
-import pytest
-
-from train_lib.docker_util.validate_master_image import validate_train_image
-
-
-def test_validate_master_image(master_image: str, train_image: str, docker_client):
-    print("\nComparison: master_img vs. train_img (SUCCESS)", end="")
-    _file_system_change_test(master_image, train_image, docker_client, "none", True)
-
-    docker_client.images.pull("hello-world")
-    print("\nComparison: master_img vs. random_img (FAIL)", end="")
-    _file_system_change_test(master_image, "hello-world", docker_client, "none", False)
-
-    print("\nComparison: train_img vs. master_img (FAIL)", end="")
-    _file_system_change_test(train_image, master_image, docker_client, "none", False)
-
-    for change_type in ["add", "change", "delete"]:
-        for test_result in [True, False]:
-            print(
-                f"\nComparison: master_img vs. train_img_with_{change_type} ({'SUCCESS' if test_result else 'FAIL'})",
-                end="",
-            )
-            _file_system_change_test(
-                master_image, train_image, docker_client, change_type, test_result
-            )
-
-
-def _file_system_change_test(
-    master_img: str,
-    train_img: str,
-    docker_client,
-    change_type: str,
-    positive_test: bool,
-):
-    """
-    Changes file system in train image according to given change type, creates a copy in the docker_client, and performs
-    either positive or negative test validation against master image.
-    :param master_img: master image identifier for validation test
-    :param train_img: train image identifier onto which changes will be applied
-    :param docker_client: docker client associated with given docker image and where the new image will be created
-    :param change_type: either "add", "change", "delete" or "none" clarifying which kind of change should be applied to
-    the new train image. If no changes are applied the normal train image will be used for the validation test
-    :param positive_test: boolean value determining whether a positive or negative validation test will be performed
-    :return:
-    """
-    if change_type in ["add", "change", "delete", "none"]:
-        # Define name of new train image
-        new_train_img = (
-            f"{train_img}_{change_type}:{'not_' if positive_test else ''}faulty"
-        )
-
-        # Determine and apply change type
-        if change_type == "add":
-            if positive_test:
-                _add_img_file(
-                    train_img, new_train_img, docker_client, "opt/pht_results/file"
-                )
-            else:
-                _add_img_file(train_img, new_train_img, docker_client, "opt/file")
-        elif change_type == "change":
-            if positive_test:
-                _make_change_in_img_file(
-                    train_img,
-                    new_train_img,
-                    docker_client,
-                    "opt/train_config.json",
-                    ".",
-                )
-            else:
-                _make_change_in_img_file(
-                    train_img, new_train_img, docker_client, ".dockerenv", "."
-                )
-        elif change_type == "delete":
-            if positive_test:
-                _delete_img_file(
-                    train_img, new_train_img, docker_client, "opt/train_config.json"
-                )
-            else:
-                _delete_img_file(train_img, new_train_img, docker_client, ".dockerenv")
-        else:
-            new_train_img = train_img
-
-        # Perform validation test
-        start_t = time.time()
-        if positive_test:
-            validate_train_image(master_img, new_train_img, docker_client=docker_client)
-            print(" -> succeeds")
-        else:
-            with pytest.raises(ValueError):
-                validate_train_image(
-                    master_img, new_train_img, docker_client=docker_client
-                )
-            print(" -> fails")
-        print(f"{time.time() - start_t:.2f}s")
-    else:
-        raise ValueError("File system change test was given an invalid change type.")
-
-
-def _add_img_file(img: str, new_img: str, docker_client, path: str):
-    """
-    Adds a file to a given docker image at the specified path and creates new image from it
-    :param img: identifier of the image
-    :param new_img: identifier of newly created image <repository>:<tag>
-    :param docker_client: docker client associated with given docker image and where the new image will be created
-    :param path: filepath at which a new file will be added
-    :return:
-    """
-    # create and commit new copy of image
-    data = docker_client.containers.create(img)
-    repository, tag = new_img.split(":")
-    data.commit(repository=repository, tag=tag)
-    data.wait()
-    data.remove()
-
-    # run copy and add file.txt at given path, overwrite new image
-    data = docker_client.containers.run(new_img, command=f"touch {path}", detach=True)
-    data.wait()
-    data.commit(repository=repository, tag=tag)
-    data.wait()
-    data.remove()
-
-
-def _make_change_in_img_file(
-    img: str, new_img: str, docker_client, path: str, added_change: str
-):
-    """
-    Appends change to file at the specified path in given docker image and creates new image from it
-    :param img:  identifier of the image
-    :param new_img:  identifier of newly created image <repository>:<tag>
-    :param docker_client: docker client associated with given docker image and where the new image will be created
-    :param path: filepath at which the change will be appended to file
-    :param added_change: string that will be appended to the specified file in the docker image
-    :return:
-    """
-
-    data = docker_client.containers.create(img)
-    # extract specified file
-    bits, _ = data.get_archive(path, None)
-    data.wait()
-    bytes_arr = bytearray()
-    for chunk in bits:
-        bytes_arr.extend(chunk)
-    # add change to raw bitstream
-    bytes_arr.extend(added_change.encode("utf-8"))
-
-    # setup old archive around new file content
-    archive_obj = BytesIO()
-    tar = tarfile.open(fileobj=archive_obj, mode="w")
-    bytes_data = BytesIO(bytes_arr)
-    info = tarfile.TarInfo(name=path.split("/")[-1])
-    info.size = bytes_data.getbuffer().nbytes
-    info.mtime = time.time()
-    tar.addfile(info, bytes_data)
-    tar.close()
-    archive_obj.seek(0)
-
-    # overwrite old archive
-    data.put_archive(f"{'/'.join(path.split('/')[:-1])}/", archive_obj)
-    data.wait()
-    # get repository and tag for committing the container to an image
-    repository, tag = new_img.split(":")
-    data.commit(repository=repository, tag=tag)
-    data.wait()
-    data.remove()
-
-
-def _delete_img_file(img: str, new_img: str, docker_client, path: str):
-    """
-    Deletes file at the specified path in given docker image and creates new image from it
-    :param img:  identifier of the image
-    :param new_img:  identifier of newly created image <repository>:<tag>
-    :param docker_client: docker client associated with given docker image and where the new image will be created
-    :param path: filepath of file in docker image that will be deleted
-    :return:
-    """
-    # create and commit new copy of image
-    data = docker_client.containers.create(img)
-    repository, tag = new_img.split(":")
-    data.commit(repository=repository, tag=tag)
-    data.wait()
-    data.remove()
-
-    # run copy and remove specified file at given path, overwrite new image
-    data = docker_client.containers.run(new_img, command=f"rm {path}", detach=True)
-    data.wait()
-    data.commit(repository=repository, tag=tag)
-    data.wait()
-    data.remove()
+import tarfile
+import time
+from io import BytesIO
+
+import pytest
+
+from train_lib.docker_util.validate_master_image import validate_train_image
+
+
+def test_validate_master_image(
+    master_image: str, train_image: str, docker_client, num_cpus=4
+):
+    print("\nComparison: master_img vs. train_img (SUCCESS)", end="")
+    _file_system_change_test(
+        master_image, train_image, docker_client, num_cpus, "none", True
+    )
+
+    docker_client.images.pull("hello-world")
+    print("\nComparison: master_img vs. random_img (FAIL)", end="")
+    _file_system_change_test(
+        master_image, "hello-world", docker_client, num_cpus, "none", False
+    )
+
+    if master_image != train_image:
+        print("\nComparison: train_img vs. master_img (FAIL)", end="")
+        _file_system_change_test(
+            train_image, master_image, docker_client, num_cpus, "none", False
+        )
+
+    for change_type in ["add", "change", "delete"]:
+        for test_result in [True, False]:
+            print(
+                f"\nComparison: master_img vs. train_img_with_{change_type} ({'SUCCESS' if test_result else 'FAIL'})",
+                end="",
+            )
+            _file_system_change_test(
+                master_image,
+                train_image,
+                docker_client,
+                num_cpus,
+                change_type,
+                test_result,
+            )
+
+
+def _file_system_change_test(
+    master_img: str,
+    train_img: str,
+    docker_client,
+    num_cpus: int,
+    change_type: str,
+    positive_test: bool,
+):
+    """
+    Changes file system in train image according to given change type, creates a copy in the docker_client, and performs
+    either positive or negative test validation against master image.
+    :param master_img: master image identifier for validation test
+    :param train_img: train image identifier onto which changes will be applied
+    :param docker_client: docker client associated with given docker image and where the new image will be created
+    :param num_cpus: number of cpus used
+    :param change_type: either "add", "change", "delete" or "none" clarifying which kind of change should be applied to
+    the new train image. If no changes are applied the normal train image will be used for the validation test
+    :param positive_test: boolean value determining whether a positive or negative validation test will be performed
+    :return:
+    """
+    if change_type in ["add", "change", "delete", "none"]:
+        # Define name of new train image
+        train_img = train_img if ":" not in train_img else train_img.split(":")[0]
+        new_train_img = (
+            f"{train_img}_{change_type}:{'not_' if positive_test else ''}faulty"
+        )
+
+        # Determine and apply change type
+        if change_type == "add":
+            if positive_test:
+                _add_img_file(
+                    train_img, new_train_img, docker_client, "opt/pht_results/file"
+                )
+            else:
+                _add_img_file(train_img, new_train_img, docker_client, "opt/file")
+        elif change_type == "change":
+            if positive_test:
+                _make_change_in_img_file(
+                    train_img,
+                    new_train_img,
+                    docker_client,
+                    "opt/train_config.json",
+                    ".",
+                )
+            else:
+                _make_change_in_img_file(
+                    train_img, new_train_img, docker_client, ".dockerenv", "."
+                )
+        elif change_type == "delete":
+            if positive_test:
+                _delete_img_file(
+                    train_img, new_train_img, docker_client, "opt/train_config.json"
+                )
+            else:
+                _delete_img_file(train_img, new_train_img, docker_client, ".dockerenv")
+        else:
+            new_train_img = train_img
+
+        # Perform validation test
+        start_t = time.time()
+        if positive_test:
+            validate_train_image(
+                master_img,
+                new_train_img,
+                docker_client=docker_client,
+                num_cpus=num_cpus,
+            )
+            print(" -> succeeds")
+        else:
+            with pytest.raises(ValueError):
+                validate_train_image(
+                    master_img,
+                    new_train_img,
+                    docker_client=docker_client,
+                    num_cpus=num_cpus,
+                )
+            print(" -> fails")
+        print(f"{time.time() - start_t:.2f}s")
+    else:
+        raise ValueError("File system change test was given an invalid change type.")
+
+
+def _add_img_file(img: str, new_img: str, docker_client, path: str):
+    """
+    Adds a file to a given docker image at the specified path and creates new image from it
+    :param img: identifier of the image
+    :param new_img: identifier of newly created image <repository>:<tag>
+    :param docker_client: docker client associated with given docker image and where the new image will be created
+    :param path: filepath at which a new file will be added
+    :return:
+    """
+    # create and commit new copy of image
+    data = docker_client.containers.create(img)
+    repository, tag = new_img.split(":")
+    data.commit(repository=repository, tag=tag)
+    data.wait()
+    data.remove()
+
+    # run copy and add file.txt at given path, overwrite new image
+    data = docker_client.containers.run(new_img, command=f"touch {path}", detach=True)
+    data.wait()
+    data.commit(repository=repository, tag=tag)
+    data.wait()
+    data.remove()
+
+
+def _make_change_in_img_file(
+    img: str, new_img: str, docker_client, path: str, added_change: str
+):
+    """
+    Appends change to file at the specified path in given docker image and creates new image from it
+    :param img:  identifier of the image
+    :param new_img:  identifier of newly created image <repository>:<tag>
+    :param docker_client: docker client associated with given docker image and where the new image will be created
+    :param path: filepath at which the change will be appended to file
+    :param added_change: string that will be appended to the specified file in the docker image
+    :return:
+    """
+
+    data = docker_client.containers.create(img)
+    # extract specified file
+    bits, _ = data.get_archive(path, None)
+    data.wait()
+    bytes_arr = bytearray()
+    for chunk in bits:
+        bytes_arr.extend(chunk)
+    # add change to raw bitstream
+    bytes_arr.extend(added_change.encode("utf-8"))
+
+    # setup old archive around new file content
+    archive_obj = BytesIO()
+    tar = tarfile.open(fileobj=archive_obj, mode="w")
+    bytes_data = BytesIO(bytes_arr)
+    info = tarfile.TarInfo(name=path.split("/")[-1])
+    info.size = bytes_data.getbuffer().nbytes
+    info.mtime = time.time()
+    tar.addfile(info, bytes_data)
+    tar.close()
+    archive_obj.seek(0)
+
+    # overwrite old archive
+    data.put_archive(f"{'/'.join(path.split('/')[:-1])}/", archive_obj)
+    data.wait()
+    # get repository and tag for committing the container to an image
+    repository, tag = new_img.split(":")
+    data.commit(repository=repository, tag=tag)
+    data.wait()
+    data.remove()
+
+
+def _delete_img_file(img: str, new_img: str, docker_client, path: str):
+    """
+    Deletes file at the specified path in given docker image and creates new image from it
+    :param img:  identifier of the image
+    :param new_img:  identifier of newly created image <repository>:<tag>
+    :param docker_client: docker client associated with given docker image and where the new image will be created
+    :param path: filepath of file in docker image that will be deleted
+    :return:
+    """
+    # create and commit new copy of image
+    data = docker_client.containers.create(img)
+    repository, tag = new_img.split(":")
+    data.commit(repository=repository, tag=tag)
+    data.wait()
+    data.remove()
+
+    # run copy and remove specified file at given path, overwrite new image
+    data = docker_client.containers.run(new_img, command=f"rm {path}", detach=True)
+    data.wait()
+    data.commit(repository=repository, tag=tag)
+    data.wait()
+    data.remove()
```

### Comparing `pht_train_container_library-2.0.5/PKG-INFO` & `pht_train_container_library-2.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,42 @@
-Metadata-Version: 2.1
-Name: pht-train-container-library
-Version: 2.0.5
-Summary: Python library for handling containerized PHT trains
-Author: Michael Graf
-Author-email: michael.graf@uni-tuebingen.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography
-Requires-Dist: docker
-Requires-Dist: fhir-kindling
-Requires-Dist: loguru
-Requires-Dist: pandas
-Requires-Dist: pendulum
-Requires-Dist: requests
-Requires-Dist: requests_oauthlib
-Description-Content-Type: text/markdown
-
-[![Documentation Status](https://readthedocs.org/projects/train-container-library/badge/?version=latest)](https://train-container-library.readthedocs.io/en/latest/?badge=latest)
-[![CodeQL](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml)
-[![main-ci](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml/badge.svg)](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/PHT-Medic/train-container-library/branch/master/graph/badge.svg?token=11RYRZK2FO)](https://codecov.io/gh/PHT-Medic/train-container-library)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pht-train-container-library)
-![PyPI - Downloads](https://img.shields.io/pypi/dw/pht-train-container-library)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# &#128646; Train Container Library
-
-Python library for validating and interacting with pht-train images/containers.
-
-## Installation
-
-```shell
-pip install pht-train-container-library
-```
-
-
-## Setup development environment
-Make sure you have [poetry](https://python-poetry.org/docs/#installation) and [pre-commit](https://pre-commit.com/#install) installed.
-
-Install the dependencies and pre-commit hooks:
-```shell
-poetry install --with dev
-```
-
-```shell
-poetry run pre-commit install
-```
-
-### Run tests
-
-```shell
-poetry run pytest
-```
-
-### Linting and formatting
-
-These commands are also run as pre-commit hooks.
-
-Linting with ruff:
-```shell
-poetry run ruff . --fix
-```
-
-Formatting with black:
-```shell
-poetry run black .
-```
-
-## Security Protocol
-
-The pht security protocol adapted from `docs/Secure_PHT_latest__official.pdf` performs two main tasks:
-
-1. Before executing a train-image on the local machine, unless the station is the first station on the route, the
-   previous results need to be decrypted and the content of the image needs to be validated based on the configuration
-   of the individual train -> `pre-run`.
-2. After executing the train the updated results need to be encrypted and the train configuration needs to be updated to
-   reflect the current state ->`post-run`.
-
-### Train image structure
-
-To ensure the protocol is working correctly train docker images are required to keep the following structure:
-
-- `/opt/train_config.json`: Stores the configuration file of the train.
-- `/opt/pht_train/`: Stores all the files containing code or other things required for the train algorithm to run. The
-  contents of this directory can never change and is validated by the `pre-run` step.
-- `/opt/pht_results/`: Stores the results of the train. Which will be decrypted in the `pre-run` step and encrypted in
-  the `post-run` step.
-
-No files in the image outside the `/opt/pht_results/` directory should change during the execution of the algorithm.
-
-### Usage - Python Script
-
-To use the protocol in your own python application, after installing the library
-with `pip install pht-train-container-library` an instance of the protocol can be to validate docker images as follows:
-
-```python
-from train_lib.security.protocol import SecurityProtocol
-from train_lib.docker_util.docker_ops import extract_train_config
-
-image_name = '<image-repo>:<image-tag>'
-station_id = '<station-id>'
-
-# Get the train configuration from the image
-config = extract_train_config(image_name)
-# Initialize the protocol with the extracted config and station_id
-protocol = SecurityProtocol(station_id=station_id, config=config)
-
-# execute one of the protocol steps
-protocol.pre_run_protocol(image_name, private_key_path='<path-to-private-key>')
-# protocol.post_run_protocol(image_name, private_key_path='<path-to-private-key>')
-```
-
-### Usage - Container
-
-A containerized version of the protocol is also available it can be used with the following command:
-
-```shell
-docker run -e STATION_ID=<station_id> -e PRIVATE_KEY_PATH=/opt/private_key.pem -v /var/run/docker.sock:/var/run/docker.sock -v <path_to_your_key>:/opt/private_key.pem ghcr.io/pht-medic/protocol <pre-run/post-run> <image-repo>:<image-tag>
-```
-
-`STATION_ID` and `PRIVATE_KEY_PATH` are required to be set in the environment variables. As well as passing the docker
-socket `/var/run/docker.sock` to the container as a volume to enable docker-in-docker functionality.
-
-### Pre-run protocol
-
-The pre-run protocol consists of the following steps
-
-1. The hash of the immutable files (train definition) is verified making sure that the executable files did not change
-   during the the train definition.
-2. The digital signature is verified ensuring the correctness of the results at each stop of the train.
-3. The symmetric key is decrypted using the provided station private key
-4. The mutable files in `/opt/pht_results` are decrypted using the symmetric key obtained in the previous step
-5. The decrypted files are hashed and the hash is compared to the one stored in the train configuration file.
-
-Once these steps have been completed the image is ready to be executed.
-
-### Post-run protocol
-
-1. Calculate the hash of the newly generated results
-2. Sign the hash of the results using the provided `PRIVATE_KEY_PATH`
-3. Update the the train signature using the session id that is randomly generated at each execution step
-4. Encrypt the resulting files using a newly generated symmetric key
-5. Encrypt the generated symmetric key with the public keys of the train participants
-6. Update the train configuration file
-
-With the completion of these steps the train is ready to be pushed into the registry for further processing
-
-## Tests
-
-Run the tests to validate the security protocol is working as intended. From this projects root directory run
-`pytest train_lib`
-
-
-
-
-
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
+packages = \
+['train_lib',
+ 'train_lib.clients',
+ 'train_lib.clients.fhir',
+ 'train_lib.docker_util',
+ 'train_lib.security',
+ 'train_lib.tests']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['cryptography',
+ 'docker',
+ 'fhir-kindling',
+ 'loguru',
+ 'pandas',
+ 'pendulum',
+ 'requests',
+ 'requests_oauthlib']
+
+setup_kwargs = {
+    'name': 'pht-train-container-library',
+    'version': '2.0.6',
+    'description': 'Python library for handling containerized PHT trains',
+    'long_description': "[![Documentation Status](https://readthedocs.org/projects/train-container-library/badge/?version=latest)](https://train-container-library.readthedocs.io/en/latest/?badge=latest)\n[![CodeQL](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/PHT-Medic/train-container-library/actions/workflows/codeql-analysis.yml)\n[![main-ci](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml/badge.svg)](https://github.com/PHT-EU/train-container-library/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/PHT-Medic/train-container-library/branch/master/graph/badge.svg?token=11RYRZK2FO)](https://codecov.io/gh/PHT-Medic/train-container-library)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pht-train-container-library)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/pht-train-container-library)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# &#128646; Train Container Library\n\nPython library for validating and interacting with pht-train images/containers.\n\n## Installation\n\n```shell\npip install pht-train-container-library\n```\n\n\n## Setup development environment\nMake sure you have [poetry](https://python-poetry.org/docs/#installation) and [pre-commit](https://pre-commit.com/#install) installed.\n\nInstall the dependencies and pre-commit hooks:\n```shell\npoetry install --with dev\n```\n\n```shell\npoetry run pre-commit install\n```\n\n### Run tests\n\n```shell\npoetry run pytest\n```\n\n### Linting and formatting\n\nThese commands are also run as pre-commit hooks.\n\nLinting with ruff:\n```shell\npoetry run ruff . --fix\n```\n\nFormatting with black:\n```shell\npoetry run black .\n```\n\n## Security Protocol\n\nThe pht security protocol adapted from `docs/Secure_PHT_latest__official.pdf` performs two main tasks:\n\n1. Before executing a train-image on the local machine, unless the station is the first station on the route, the\n   previous results need to be decrypted and the content of the image needs to be validated based on the configuration\n   of the individual train -> `pre-run`.\n2. After executing the train the updated results need to be encrypted and the train configuration needs to be updated to\n   reflect the current state ->`post-run`.\n\n### Train image structure\n\nTo ensure the protocol is working correctly train docker images are required to keep the following structure:\n\n- `/opt/train_config.json`: Stores the configuration file of the train.\n- `/opt/pht_train/`: Stores all the files containing code or other things required for the train algorithm to run. The\n  contents of this directory can never change and is validated by the `pre-run` step.\n- `/opt/pht_results/`: Stores the results of the train. Which will be decrypted in the `pre-run` step and encrypted in\n  the `post-run` step.\n\nNo files in the image outside the `/opt/pht_results/` directory should change during the execution of the algorithm.\n\n### Usage - Python Script\n\nTo use the protocol in your own python application, after installing the library\nwith `pip install pht-train-container-library` an instance of the protocol can be to validate docker images as follows:\n\n```python\nfrom train_lib.security.protocol import SecurityProtocol\nfrom train_lib.docker_util.docker_ops import extract_train_config\n\nimage_name = '<image-repo>:<image-tag>'\nstation_id = '<station-id>'\n\n# Get the train configuration from the image\nconfig = extract_train_config(image_name)\n# Initialize the protocol with the extracted config and station_id\nprotocol = SecurityProtocol(station_id=station_id, config=config)\n\n# execute one of the protocol steps\nprotocol.pre_run_protocol(image_name, private_key_path='<path-to-private-key>')\n# protocol.post_run_protocol(image_name, private_key_path='<path-to-private-key>')\n```\n\n### Usage - Container\n\nA containerized version of the protocol is also available it can be used with the following command:\n\n```shell\ndocker run -e STATION_ID=<station_id> -e PRIVATE_KEY_PATH=/opt/private_key.pem -v /var/run/docker.sock:/var/run/docker.sock -v <path_to_your_key>:/opt/private_key.pem ghcr.io/pht-medic/protocol <pre-run/post-run> <image-repo>:<image-tag>\n```\n\n`STATION_ID` and `PRIVATE_KEY_PATH` are required to be set in the environment variables. As well as passing the docker\nsocket `/var/run/docker.sock` to the container as a volume to enable docker-in-docker functionality.\n\n### Pre-run protocol\n\nThe pre-run protocol consists of the following steps\n\n1. The hash of the immutable files (train definition) is verified making sure that the executable files did not change\n   during the the train definition.\n2. The digital signature is verified ensuring the correctness of the results at each stop of the train.\n3. The symmetric key is decrypted using the provided station private key\n4. The mutable files in `/opt/pht_results` are decrypted using the symmetric key obtained in the previous step\n5. The decrypted files are hashed and the hash is compared to the one stored in the train configuration file.\n\nOnce these steps have been completed the image is ready to be executed.\n\n### Post-run protocol\n\n1. Calculate the hash of the newly generated results\n2. Sign the hash of the results using the provided `PRIVATE_KEY_PATH`\n3. Update the the train signature using the session id that is randomly generated at each execution step\n4. Encrypt the resulting files using a newly generated symmetric key\n5. Encrypt the generated symmetric key with the public keys of the train participants\n6. Update the train configuration file\n\nWith the completion of these steps the train is ready to be pushed into the registry for further processing\n\n## Tests\n\nRun the tests to validate the security protocol is working as intended. From this projects root directory run\n`pytest train_lib`\n\n\n\n\n\n\n\n",
+    'author': 'Michael Graf',
+    'author_email': 'michael.graf@uni-tuebingen.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8,<4.0',
+}
 
 
+setup(**setup_kwargs)
```

