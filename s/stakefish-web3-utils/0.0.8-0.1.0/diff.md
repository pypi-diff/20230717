# Comparing `tmp/stakefish-web3-utils-0.0.8.tar.gz` & `tmp/stakefish-web3-utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/stakefish/code/web3-utils/dist/.tmp-i31bkh4d/stakefish-web3-utils-0.0.8.tar", last modified: Thu Mar 30 11:49:34 2023, max compression
+gzip compressed data, was "/Users/stakefish/code/web3-utils/dist/.tmp-jwu7va52/stakefish-web3-utils-0.1.0.tar", last modified: Mon Jul 17 08:06:42 2023, max compression
```

## Comparing `stakefish-web3-utils-0.0.8.tar` & `stakefish-web3-utils-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-03-30 11:49:34.885697 stakefish-web3-utils-0.0.8/
--rw-r--r--   0 stakefish   (502) staff       (20)     1082 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.0.8/LICENSE.md
--rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-03-30 11:49:34.885893 stakefish-web3-utils-0.0.8/PKG-INFO
--rw-r--r--   0 stakefish   (502) staff       (20)      810 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.0.8/README.rst
--rw-r--r--   0 stakefish   (502) staff       (20)      187 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.0.8/pyproject.toml
--rw-r--r--   0 stakefish   (502) staff       (20)      796 2023-03-30 11:49:34.886924 stakefish-web3-utils-0.0.8/setup.cfg
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-03-30 11:49:34.872111 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/
--rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/PKG-INFO
--rw-r--r--   0 stakefish   (502) staff       (20)     1060 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/SOURCES.txt
--rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/dependency_links.txt
--rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/not-zip-safe
--rw-r--r--   0 stakefish   (502) staff       (20)       62 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/requires.txt
--rw-r--r--   0 stakefish   (502) staff       (20)       11 2023-03-30 11:49:34.000000 stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/top_level.txt
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-03-30 11:49:34.877477 stakefish-web3-utils-0.0.8/tests/
--rw-r--r--   0 stakefish   (502) staff       (20)     2799 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/tests/test_async_beacon.py
--rw-r--r--   0 stakefish   (502) staff       (20)      207 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.0.8/tests/test_compute_time_at_slot.py
--rw-r--r--   0 stakefish   (502) staff       (20)      269 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.0.8/tests/test_convert_to_standard_notation.py
--rw-r--r--   0 stakefish   (502) staff       (20)      635 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.0.8/tests/test_divide_chunks.py
--rw-r--r--   0 stakefish   (502) staff       (20)      320 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/tests/test_gwei_to_wei.py
--rw-r--r--   0 stakefish   (502) staff       (20)      228 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.0.8/tests/test_hash_event_param.py
--rw-r--r--   0 stakefish   (502) staff       (20)      256 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.0.8/tests/test_is_null_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)      289 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/tests/test_normalize_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3991 2023-03-30 11:06:22.000000 stakefish-web3-utils-0.0.8/tests/test_retryable_eth_module.py
--rw-r--r--   0 stakefish   (502) staff       (20)      628 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.0.8/tests/test_split_validator_pubkey_bytes.py
-drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-03-30 11:49:34.885129 stakefish-web3-utils-0.0.8/web3_utils/
--rw-r--r--   0 stakefish   (502) staff       (20)        0 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.0.8/web3_utils/__init__.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3660 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/async_beacon.py
--rw-r--r--   0 stakefish   (502) staff       (20)      343 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/calculate_max_fees.py
--rw-r--r--   0 stakefish   (502) staff       (20)      130 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/compute_time_at_slot.py
--rw-r--r--   0 stakefish   (502) staff       (20)      168 2023-03-30 10:43:41.000000 stakefish-web3-utils-0.0.8/web3_utils/convert_to_standard_notation.py
--rw-r--r--   0 stakefish   (502) staff       (20)      284 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/current_utc_timestamp.py
--rw-r--r--   0 stakefish   (502) staff       (20)      138 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.0.8/web3_utils/divide_chunks.py
--rw-r--r--   0 stakefish   (502) staff       (20)      111 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/gwei_to_wei.py
--rw-r--r--   0 stakefish   (502) staff       (20)      126 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/hash_event_param.py
--rw-r--r--   0 stakefish   (502) staff       (20)      241 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/is_null_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)      301 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/normalize_address.py
--rw-r--r--   0 stakefish   (502) staff       (20)     3050 2023-03-30 10:45:11.000000 stakefish-web3-utils-0.0.8/web3_utils/retryable_eth_module.py
--rw-r--r--   0 stakefish   (502) staff       (20)      336 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.0.8/web3_utils/split_validator_pubkey_bytes.py
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.705100 stakefish-web3-utils-0.1.0/
+-rw-r--r--   0 stakefish   (502) staff       (20)     1082 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.1.0/LICENSE.md
+-rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-07-17 08:06:42.705369 stakefish-web3-utils-0.1.0/PKG-INFO
+-rw-r--r--   0 stakefish   (502) staff       (20)      810 2023-01-12 15:11:34.000000 stakefish-web3-utils-0.1.0/README.rst
+-rw-r--r--   0 stakefish   (502) staff       (20)      187 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/pyproject.toml
+-rw-r--r--   0 stakefish   (502) staff       (20)      796 2023-07-17 08:06:42.706436 stakefish-web3-utils-0.1.0/setup.cfg
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.686877 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/
+-rw-r--r--   0 stakefish   (502) staff       (20)     1370 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/PKG-INFO
+-rw-r--r--   0 stakefish   (502) staff       (20)     1060 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)        1 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/not-zip-safe
+-rw-r--r--   0 stakefish   (502) staff       (20)       62 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/requires.txt
+-rw-r--r--   0 stakefish   (502) staff       (20)       11 2023-07-17 08:06:42.000000 stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/top_level.txt
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.695702 stakefish-web3-utils-0.1.0/tests/
+-rw-r--r--   0 stakefish   (502) staff       (20)     2799 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_async_beacon.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      207 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_compute_time_at_slot.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      269 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_convert_to_standard_notation.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      635 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/tests/test_divide_chunks.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      320 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_gwei_to_wei.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      228 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_hash_event_param.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      256 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_is_null_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      289 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/tests/test_normalize_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     3991 2023-03-30 11:06:22.000000 stakefish-web3-utils-0.1.0/tests/test_retryable_eth_module.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      628 2023-01-12 12:30:57.000000 stakefish-web3-utils-0.1.0/tests/test_split_validator_pubkey_bytes.py
+drwxr-xr-x   0 stakefish   (502) staff       (20)        0 2023-07-17 08:06:42.704613 stakefish-web3-utils-0.1.0/web3_utils/
+-rw-r--r--   0 stakefish   (502) staff       (20)        0 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/web3_utils/__init__.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     3779 2023-07-17 07:58:36.000000 stakefish-web3-utils-0.1.0/web3_utils/async_beacon.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      343 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/calculate_max_fees.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      130 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/compute_time_at_slot.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      168 2023-03-30 10:43:41.000000 stakefish-web3-utils-0.1.0/web3_utils/convert_to_standard_notation.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      284 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/current_utc_timestamp.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      138 2023-01-04 12:28:25.000000 stakefish-web3-utils-0.1.0/web3_utils/divide_chunks.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      111 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/gwei_to_wei.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      126 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/hash_event_param.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      241 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/is_null_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      301 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/normalize_address.py
+-rw-r--r--   0 stakefish   (502) staff       (20)     3050 2023-03-30 10:45:11.000000 stakefish-web3-utils-0.1.0/web3_utils/retryable_eth_module.py
+-rw-r--r--   0 stakefish   (502) staff       (20)      336 2023-01-06 17:01:52.000000 stakefish-web3-utils-0.1.0/web3_utils/split_validator_pubkey_bytes.py
```

### Comparing `stakefish-web3-utils-0.0.8/LICENSE.md` & `stakefish-web3-utils-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/PKG-INFO` & `stakefish-web3-utils-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.0.8
+Version: 0.1.0
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish-web3-utils-0.0.8/README.rst` & `stakefish-web3-utils-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/setup.cfg` & `stakefish-web3-utils-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stakefish-web3-utils
-version = 0.0.8
+version = 0.1.0
 description = Stakefish’s web3 utils for Python
 author = Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 url = https://github.com/stakefish/web3-utils
 long_description = file: README.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
```

### Comparing `stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/PKG-INFO` & `stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stakefish-web3-utils
-Version: 0.0.8
+Version: 0.1.0
 Summary: Stakefish’s web3 utils for Python
 Home-page: https://github.com/stakefish/web3-utils
 Author: Michal Baranowski <mbaranovski@stake.fish>, Mateusz Sokola <mateusz@stake.fish>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `stakefish-web3-utils-0.0.8/stakefish_web3_utils.egg-info/SOURCES.txt` & `stakefish-web3-utils-0.1.0/stakefish_web3_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/tests/test_async_beacon.py` & `stakefish-web3-utils-0.1.0/tests/test_async_beacon.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/tests/test_divide_chunks.py` & `stakefish-web3-utils-0.1.0/tests/test_divide_chunks.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/tests/test_retryable_eth_module.py` & `stakefish-web3-utils-0.1.0/tests/test_retryable_eth_module.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/tests/test_split_validator_pubkey_bytes.py` & `stakefish-web3-utils-0.1.0/tests/test_split_validator_pubkey_bytes.py`

 * *Files identical despite different names*

### Comparing `stakefish-web3-utils-0.0.8/web3_utils/async_beacon.py` & `stakefish-web3-utils-0.1.0/web3_utils/async_beacon.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,36 +41,39 @@
         genesis = await self._run_as_async(super().get_genesis)
         genesis_time = int(genesis["data"]["genesis_time"])
         return genesis_time
 
     async def get_validator(self, pubkey: str, state_id: str = "head"):
         return await self._run_as_async(self._get_validator, pubkey, state_id)
 
-    async def get_validators(self, state_id: str = "head", indexes: List[str] = None) -> Dict[str, Any]:
-        return await self._run_as_async(self._get_validators, state_id, indexes)
+    async def get_validators(
+        self, state_id: str = "head", indexes: List[str] = None, params: Dict[str, Any] = {}
+    ) -> Dict[str, Any]:
+        return await self._run_as_async(self._get_validators, state_id, indexes, params)
 
     async def get_validator_balances(self, state_id: str = "head", indexes: List[str] = None) -> Dict[str, Any]:
         return await self._run_as_async(self._get_validator_balances, state_id, indexes)
 
     def _get_validator(self, pubkey: str, state_id: str = "head"):
         try:
             return super().get_validator(pubkey, state_id)
         except HTTPError as e:
             if e.response.status_code == 404:
                 self.logger.info(f"BEACON CHAIN: Validator {pubkey} was not found, probably is not active yet | State: {state_id}")
                 return None
             else:
                 raise e
 
-    def _get_validators(self, state_id: str = "head", indexes: List[str] = None) -> Dict[str, Any]:
-        if indexes is None or len(indexes) > 50:
+    def _get_validators(self, state_id: str = "head", indexes: List[str] = None, params: Dict[str, Any] = {}) -> Dict[str, Any]:
+        if indexes is not None and len(indexes) > 50:
             raise Exception("Too many validators requested")
 
         endpoint = f"/eth/v1/beacon/states/{state_id}/validators"
-        params = {"id": indexes}
+        if indexes is not None:
+            params["id"] = indexes
 
         return self._make_get_request_with_params(endpoint, params)
 
     def _get_validator_balances(self, state_id: str = "head", indexes: List[str] = None) -> Dict[str, Any]:
         if indexes is None or len(indexes) > 250:
             raise Exception("Too many validators requested")
```

### Comparing `stakefish-web3-utils-0.0.8/web3_utils/retryable_eth_module.py` & `stakefish-web3-utils-0.1.0/web3_utils/retryable_eth_module.py`

 * *Files identical despite different names*

