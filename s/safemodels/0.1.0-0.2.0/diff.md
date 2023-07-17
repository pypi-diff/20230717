# Comparing `tmp/safemodels-0.1.0.tar.gz` & `tmp/safemodels-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safemodels-0.1.0.tar", max compression
+gzip compressed data, was "safemodels-0.2.0.tar", max compression
```

## Comparing `safemodels-0.1.0.tar` & `safemodels-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2010 2023-07-15 08:05:19.810729 safemodels-0.1.0/README.md
--rw-r--r--   0        0        0      619 2023-07-11 22:00:41.410899 safemodels-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      445 2023-07-15 06:11:57.047800 safemodels-0.1.0/safemodels/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-14 06:29:42.861402 safemodels-0.1.0/safemodels/check.py
--rw-r--r--   0        0        0     1833 2023-07-14 05:39:48.854820 safemodels-0.1.0/safemodels/cosign.py
--rw-r--r--   0        0        0     1099 2023-07-11 22:01:31.589461 safemodels-0.1.0/safemodels/hash.py
--rw-r--r--   0        0        0     1950 2023-07-15 05:37:09.602146 safemodels-0.1.0/safemodels/model.py
--rw-r--r--   0        0        0      697 2023-07-11 03:13:15.717733 safemodels-0.1.0/safemodels/patch/__init__.py
--rw-r--r--   0        0        0      358 2023-07-15 06:38:05.901163 safemodels-0.1.0/safemodels/patch/huggingface_hub.py
--rw-r--r--   0        0        0      639 2023-07-14 05:56:29.386804 safemodels-0.1.0/safemodels/patch/safetensors.py
--rw-r--r--   0        0        0     2892 2023-07-14 06:32:22.210230 safemodels-0.1.0/safemodels/repo.py
--rw-r--r--   0        0        0     1001 2023-07-11 03:11:33.685025 safemodels-0.1.0/safemodels/utils/safetensors.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 safemodels-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2023-07-17 20:06:12.881650 safemodels-0.2.0/README.md
+-rw-r--r--   0        0        0      584 2023-07-17 20:07:07.293402 safemodels-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      445 2023-07-15 06:11:57.047800 safemodels-0.2.0/safemodels/__init__.py
+-rw-r--r--   0        0        0     1626 2023-07-17 20:01:27.945925 safemodels-0.2.0/safemodels/check.py
+-rw-r--r--   0        0        0     1833 2023-07-14 05:39:48.854820 safemodels-0.2.0/safemodels/cosign.py
+-rw-r--r--   0        0        0     1128 2023-07-17 20:05:29.079541 safemodels-0.2.0/safemodels/hash.py
+-rw-r--r--   0        0        0     1940 2023-07-17 20:01:13.013957 safemodels-0.2.0/safemodels/model.py
+-rw-r--r--   0        0        0      697 2023-07-11 03:13:15.717733 safemodels-0.2.0/safemodels/patch/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-15 06:38:05.901163 safemodels-0.2.0/safemodels/patch/huggingface_hub.py
+-rw-r--r--   0        0        0      639 2023-07-14 05:56:29.386804 safemodels-0.2.0/safemodels/patch/safetensors.py
+-rw-r--r--   0        0        0     2892 2023-07-14 06:32:22.210230 safemodels-0.2.0/safemodels/repo.py
+-rw-r--r--   0        0        0     1001 2023-07-11 03:11:33.685025 safemodels-0.2.0/safemodels/utils/safetensors.py
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 safemodels-0.2.0/PKG-INFO
```

### Comparing `safemodels-0.1.0/README.md` & `safemodels-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```python
 from safemodels import safe_hash
 from huggingface_hub import hf_hub_download as dl
 
 st = dl("gpt2", filename="model.safetensors")
 pt = dl("gpt2", filename="pytorch_model.bin")
 
-assert safe_hash(st) == safe_hash(pt) == 11799646609665420805
+assert safe_hash(st) == safe_hash(pt) == 'd6c60a3126ef088e5f8fdaa332da56d552da966a'
 ```
 
 ### Signing
 
 ```python
 from safemodels import SafeModel
 from huggingface_hub import hf_hub_download as dl
@@ -44,16 +44,15 @@
 >>> from huggingface_hub import hf_hub_download
 >>>
 >>> init(Issuer(identity="EleutherAI", issuer="https://auth.huggingface.com")
 >>>
 >>> hf_hub_download("EleuterAI/gpt-j-6B", filename="model.safetensors")
 Downloading model.safetensors: 100%|███| 548M/548M [00:14<00:00, 39.2MB/s]
 211it [00:00, 4785.46it/s]
-Error: none of the expected identities matched what was in the certificate,
-got subjects [EleuterAI] with issuer https://auth.huggingface.com
+Error: none of the expected identities matched what was in the certificate, got subjects [EleuterAI] with issuer https://auth.huggingface.com
 Traceback (most recent call last):
   ...
 safemodels.InvalidSignature: Loaded a safetensor with an invalid signature!
 ```
 
 ### `safetensor` Metadata
```

### Comparing `safemodels-0.1.0/pyproject.toml` & `safemodels-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [tool.poetry]
 name = "safemodels"
-version = "0.1.0"
+version = "0.2.0"
 description = "safetensors with model weight hashing"
 authors = ["Yasyf Mohamedali <yasyfm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.15"
 safetensors = "^0.3.1"
 numpy = "^1.25.1"
-xxhash = "^3.2.0"
 huggingface-hub = { version = "^0.16.4", optional = true }
 torch = { version = "^2.0.1", optional = true }
-tqdm = "^4.65.0"
 pydantic = "^2.0.2"
 pyyaml = "^6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
 pytest = "^7.4.0"
```

### Comparing `safemodels-0.1.0/safemodels/check.py` & `safemodels-0.2.0/safemodels/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,27 @@
 
 
 def _check(name: str, filename: str, version: str = "main"):
     hash = safe_hash(filename)
     meta = extract_metadata(filename)
     if "sig" not in meta:
         warnings.warn(f"Signature missing for {name} ({version})")
-    elif not HashRepo.check(
-        Hash(name=name, version=version, hash=str(hash)), meta["sig"]
-    ):
+    elif not HashRepo.check(Hash(name=name, version=version, hash=hash), meta["sig"]):
         warnings.warn(f"Signature mismatch for {name} ({version})")
         raise InvalidSignature()
 
     try:
         check = HashRepo.default.get(name, version)
     except NoHashInDatabase:
         HashRepo.default.set(name, hash, version)
         warnings.warn(
             f"Hash for {name} ({version}) not found in database. Adding for future."
         )
     else:
-        if str(hash) != check.hash:
+        if hash != check.hash:
             warnings.warn(f"Hash mismatch for {name} ({version})")
             raise HashMismatch()
 
 
 @try_
 def check(name: str, filename: str, version: str = "main"):
     _check(name, filename, version)
```

### Comparing `safemodels-0.1.0/safemodels/cosign.py` & `safemodels-0.2.0/safemodels/cosign.py`

 * *Files identical despite different names*

### Comparing `safemodels-0.1.0/safemodels/hash.py` & `safemodels-0.2.0/safemodels/hash.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from typing import Generator
 
-import torch, xxhash, os
+import os, hashlib
 import numpy as np
 from tqdm import tqdm
 
 from safetensors import safe_open
 
 
-def _hash(arrs: Generator[np.ndarray, None, None]) -> int:
-    x = xxhash.xxh64()
+def _hash(arrs: Generator[np.ndarray, None, None]) -> str:
+    x = hashlib.blake2b(digest_size=20)
     for arr in tqdm(arrs):
         for chunk in np.nditer(arr, flags=["buffered", "external_loop"]):
             x.update(memoryview(chunk))
-    return x.intdigest()
+    return x.hexdigest()
 
 
-def st_hash(filename) -> int:
+def st_hash(filename) -> str:
     with safe_open(filename, framework="np") as f:
         return _hash(f.get_tensor(k) for k in sorted(f.keys()))
 
 
-def pt_hash(filename) -> int:
+def pt_hash(filename) -> str:
+    import torch
+
     f = torch.load(filename)
     return _hash(f[k] for k in sorted(f.keys()))
 
 
-def np_hash(filename) -> int:
+def np_hash(filename) -> str:
     f = np.load(filename)
     return _hash(f[k] for k in sorted(f.keys()))
 
 
-def safe_hash(filename) -> int:
+def safe_hash(filename) -> str:
     ext = os.path.splitext(filename)[1]
     try:
         return {
             ".npz": np_hash,
             ".npy": np_hash,
             ".pt": pt_hash,
             ".bin": pt_hash,
```

### Comparing `safemodels-0.1.0/safemodels/model.py` & `safemodels-0.2.0/safemodels/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         return Cosign().verify(self.model_dump_json(), sig, **kwargs)
 
     @classmethod
     def from_safetensor(cls, filename: Union[str, Path]):
         meta = extract_metadata(filename)
         if "hash" not in meta:
             raise HashMissing()
-        if meta["hash"] != str(safe_hash(filename)):
+        if meta["hash"] != safe_hash(filename):
             raise HashMismatch()
         return cls(**meta)
 
     @classmethod
     def from_hf(cls, name: str, version: str, filename: str = "model.safetensors"):
         file = hf_hub_download(name, revision=version, filename=filename)
         return file, cls.from_tensor(name, version, file)
 
     @classmethod
     def from_tensor(cls, name: str, version: str, filename: Union[str, Path]):
-        return cls(name=name, version=version, hash=str(safe_hash(filename)))
+        return cls(name=name, version=version, hash=safe_hash(filename))
```

### Comparing `safemodels-0.1.0/safemodels/patch/__init__.py` & `safemodels-0.2.0/safemodels/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `safemodels-0.1.0/safemodels/patch/safetensors.py` & `safemodels-0.2.0/safemodels/patch/safetensors.py`

 * *Files identical despite different names*

### Comparing `safemodels-0.1.0/safemodels/repo.py` & `safemodels-0.2.0/safemodels/repo.py`

 * *Files identical despite different names*

### Comparing `safemodels-0.1.0/safemodels/utils/safetensors.py` & `safemodels-0.2.0/safemodels/utils/safetensors.py`

 * *Files identical despite different names*

### Comparing `safemodels-0.1.0/PKG-INFO` & `safemodels-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safemodels
-Version: 0.1.0
+Version: 0.2.0
 Summary: safetensors with model weight hashing
 License: MIT
 Author: Yasyf Mohamedali
 Author-email: yasyfm@gmail.com
 Requires-Python: >=3.9.15,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: huggingface-hub (>=0.16.4,<0.17.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: safetensors (>=0.3.1,<0.4.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # `safemodels`
 ### Cryptographically-secure proof-of-concept for verifying the provenance of ML models.
 
 This library is a thought experiment into what securing the supply chain of ML models could look like. It's built on top of `safetensors`. You should probably read [the blog post](https://musings.yasyf.com/on-llm-supply-chain-attacks/) for more context!
 
@@ -38,15 +36,15 @@
 ```python
 from safemodels import safe_hash
 from huggingface_hub import hf_hub_download as dl
 
 st = dl("gpt2", filename="model.safetensors")
 pt = dl("gpt2", filename="pytorch_model.bin")
 
-assert safe_hash(st) == safe_hash(pt) == 11799646609665420805
+assert safe_hash(st) == safe_hash(pt) == 'd6c60a3126ef088e5f8fdaa332da56d552da966a'
 ```
 
 ### Signing
 
 ```python
 from safemodels import SafeModel
 from huggingface_hub import hf_hub_download as dl
@@ -66,16 +64,15 @@
 >>> from huggingface_hub import hf_hub_download
 >>>
 >>> init(Issuer(identity="EleutherAI", issuer="https://auth.huggingface.com")
 >>>
 >>> hf_hub_download("EleuterAI/gpt-j-6B", filename="model.safetensors")
 Downloading model.safetensors: 100%|███| 548M/548M [00:14<00:00, 39.2MB/s]
 211it [00:00, 4785.46it/s]
-Error: none of the expected identities matched what was in the certificate,
-got subjects [EleuterAI] with issuer https://auth.huggingface.com
+Error: none of the expected identities matched what was in the certificate, got subjects [EleuterAI] with issuer https://auth.huggingface.com
 Traceback (most recent call last):
   ...
 safemodels.InvalidSignature: Loaded a safetensor with an invalid signature!
 ```
 
 ### `safetensor` Metadata
```

