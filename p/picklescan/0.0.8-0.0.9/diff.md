# Comparing `tmp/picklescan-0.0.8.tar.gz` & `tmp/picklescan-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/picklescan/picklescan/dist/.tmp-o0m8_isn/picklescan-0.0.8.tar", last modified: Sun Feb 26 20:52:55 2023, max compression
+gzip compressed data, was "/home/runner/work/picklescan/picklescan/dist/.tmp-bd_feqf5/picklescan-0.0.9.tar", last modified: Tue Apr 25 14:29:55 2023, max compression
```

## Comparing `picklescan-0.0.8.tar` & `picklescan-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:52:55.000000 picklescan-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-26 20:52:41.000000 picklescan-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-26 20:52:55.000000 picklescan-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-02-26 20:52:41.000000 picklescan-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-26 20:52:41.000000 picklescan-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-26 20:52:55.000000 picklescan-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-26 20:52:41.000000 picklescan-0.0.8/src/picklescan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-26 20:52:41.000000 picklescan-0.0.8/src/picklescan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-02-26 20:52:41.000000 picklescan-0.0.8/src/picklescan/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-02-26 20:52:41.000000 picklescan-0.0.8/src/picklescan/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-26 20:52:41.000000 picklescan-0.0.8/src/picklescan/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-26 20:52:55.000000 picklescan-0.0.8/src/picklescan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 20:52:55.000000 picklescan-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-02-26 20:52:41.000000 picklescan-0.0.8/tests/test_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:29:55.000000 picklescan-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 14:29:44.000000 picklescan-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-25 14:29:55.000000 picklescan-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-25 14:29:44.000000 picklescan-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 14:29:44.000000 picklescan-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 14:29:55.000000 picklescan-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 14:29:44.000000 picklescan-0.0.9/src/picklescan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 14:29:44.000000 picklescan-0.0.9/src/picklescan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-25 14:29:44.000000 picklescan-0.0.9/src/picklescan/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-25 14:29:44.000000 picklescan-0.0.9/src/picklescan/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-25 14:29:44.000000 picklescan-0.0.9/src/picklescan/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:29:55.000000 picklescan-0.0.9/src/picklescan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:29:55.000000 picklescan-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-25 14:29:44.000000 picklescan-0.0.9/tests/test_scanner.py
```

### Comparing `picklescan-0.0.8/LICENSE` & `picklescan-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `picklescan-0.0.8/PKG-INFO` & `picklescan-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: picklescan
-Version: 0.0.8
+Version: 0.0.9
 Summary: Security scanner detecting Python Pickle files performing suspicious actions
 Home-page: https://github.com/mmaitre314/picklescan
 Author: Matthieu Maitre
 Author-email: mmaitre314@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mmaitre314/picklescan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Pickle Malware Scanner
 
 [![PyPI](https://badge.fury.io/py/picklescan.svg)](https://pypi.org/project/picklescan/)
 [![Test](https://github.com/mmaitre314/picklescan/workflows/Test/badge.svg)](https://github.com/mmaitre314/picklescan/actions/workflows/test.yml)
@@ -39,14 +39,16 @@
 The scanner can also load Pickles from local files, directories, URLs, and zip archives (a-la [PyTorch](https://pytorch.org/)):
 ```bash
 picklescan --path downloads/pytorch_model.bin
 picklescan --path downloads
 picklescan --url https://huggingface.co/sshleifer/tiny-distilbert-base-cased-distilled-squad/resolve/main/pytorch_model.bin
 ```
 
+To scan Numpy's `.npy` files, pip install the `numpy` package first.
+
 The scanner exit status codes are (a-la [ClamAV](https://www.clamav.net/)):
 - `0`: scan did not find malware
 - `1`: scan found malware
 - `2`: scan failed
 
 ## Develop
```

### Comparing `picklescan-0.0.8/README.md` & `picklescan-0.0.9/src/picklescan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: picklescan
+Version: 0.0.9
+Summary: Security scanner detecting Python Pickle files performing suspicious actions
+Home-page: https://github.com/mmaitre314/picklescan
+Author: Matthieu Maitre
+Author-email: mmaitre314@users.noreply.github.com
+Project-URL: Bug Tracker, https://github.com/mmaitre314/picklescan/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python Pickle Malware Scanner
 
 [![PyPI](https://badge.fury.io/py/picklescan.svg)](https://pypi.org/project/picklescan/)
 [![Test](https://github.com/mmaitre314/picklescan/workflows/Test/badge.svg)](https://github.com/mmaitre314/picklescan/actions/workflows/test.yml)
 
 Security scanner detecting Python Pickle files performing suspicious actions.
 
@@ -24,14 +39,16 @@
 The scanner can also load Pickles from local files, directories, URLs, and zip archives (a-la [PyTorch](https://pytorch.org/)):
 ```bash
 picklescan --path downloads/pytorch_model.bin
 picklescan --path downloads
 picklescan --url https://huggingface.co/sshleifer/tiny-distilbert-base-cased-distilled-squad/resolve/main/pytorch_model.bin
 ```
 
+To scan Numpy's `.npy` files, pip install the `numpy` package first.
+
 The scanner exit status codes are (a-la [ClamAV](https://www.clamav.net/)):
 - `0`: scan did not find malware
 - `1`: scan found malware
 - `2`: scan failed
 
 ## Develop
```

### Comparing `picklescan-0.0.8/setup.cfg` & `picklescan-0.0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = picklescan
-version = 0.0.8
+version = 0.0.9
 author = Matthieu Maitre
 author_email = mmaitre314@users.noreply.github.com
 description = Security scanner detecting Python Pickle files performing suspicious actions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mmaitre314/picklescan
 project_urls = 
@@ -14,15 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.9
 install_requires = 
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts =
```

### Comparing `picklescan-0.0.8/src/picklescan/cli.py` & `picklescan-0.0.9/src/picklescan/cli.py`

 * *Files identical despite different names*

### Comparing `picklescan-0.0.8/src/picklescan/scanner.py` & `picklescan-0.0.9/src/picklescan/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,16 +132,18 @@
 # https://joblib.readthedocs.io/en/latest/generated/joblib.load.html
 # torch.load()
 # https://pytorch.org/docs/stable/generated/torch.load.html
 # tf.keras.models.load_model()
 # https://www.tensorflow.org/api_docs/python/tf/keras/models/load_model
 #
 
+# TODO: support .npz files
+_numpy_file_extensions = {".npy"}
 _pytorch_file_extensions = {".bin", ".pt", ".pth", ".ckpt"}
-_pickle_file_extensions = {".pkl", ".pickle", ".joblib", ".dat", ".data", ".npy"}
+_pickle_file_extensions = {".pkl", ".pickle", ".joblib", ".dat", ".data"}
 _zip_file_extensions = {".zip", ".npz"}
 
 
 def _http_get(url) -> bytes:
     _log.debug(f"Request: GET {url}")
 
     parsed_url = urllib.parse.urlparse(url)
@@ -275,14 +277,45 @@
                 _log.debug("Scanning file %s in zip archive %s", file_name, file_id)
                 with zip.open(file_name, "r") as file:
                     result.merge(scan_pickle_bytes(file, f"{file_id}:{file_name}"))
 
     return result
 
 
+def scan_numpy(data: IO[bytes], file_id) -> ScanResult:
+
+    # Delay import to avoid dependency on NumPy
+    import numpy as np
+
+    # Code to distinguish from NumPy binary files and pickles.
+    _ZIP_PREFIX = b"PK\x03\x04"
+    _ZIP_SUFFIX = b"PK\x05\x06"  # empty zip files start with this
+    N = len(np.lib.format.MAGIC_PREFIX)
+    magic = data.read(N)
+    # If the file size is less than N, we need to make sure not
+    # to seek past the beginning of the file
+    data.seek(-min(N, len(magic)), 1)  # back-up
+    if magic.startswith(_ZIP_PREFIX) or magic.startswith(_ZIP_SUFFIX):
+        # .npz file
+        raise NotImplementedError("Scanning of .npz files is not implemented yet")
+    elif magic == np.lib.format.MAGIC_PREFIX:
+        # .npy file
+
+        version = np.lib.format.read_magic(data)
+        np.lib.format._check_version(version)
+        _, _, dtype = np.lib.format._read_array_header(data, version)
+
+        if dtype.hasobject:
+            return scan_pickle_bytes(data, file_id)
+        else:
+            return ScanResult([], 1)
+    else:
+        return scan_pickle_bytes(data, file_id)
+
+
 def scan_pytorch(data: IO[bytes], file_id) -> ScanResult:
     # new pytorch format
     if _is_zipfile(data):
         return scan_zip_bytes(data, file_id)
     # old pytorch format
     else:
         scan_result = ScanResult([])
@@ -308,14 +341,16 @@
 def scan_bytes(data: IO[bytes], file_id, file_ext: Optional[str] = None) -> ScanResult:
     if file_ext is not None and file_ext in _pytorch_file_extensions:
         try:
             return scan_pytorch(data, file_id)
         except InvalidMagicError as e:
             _log.error(f"ERROR: Invalid magic number for file {e}")
             return ScanResult([], scan_err=True)
+    elif file_ext is not None and file_ext in _numpy_file_extensions:
+        return scan_numpy(data, file_id)
     else:
         is_zip = zipfile.is_zipfile(data)
         data.seek(0)
         return (
             scan_zip_bytes(data, file_id)
             if is_zip
             else scan_pickle_bytes(data, file_id)
```

### Comparing `picklescan-0.0.8/src/picklescan/torch.py` & `picklescan-0.0.9/src/picklescan/torch.py`

 * *Files identical despite different names*

### Comparing `picklescan-0.0.8/src/picklescan.egg-info/PKG-INFO` & `picklescan-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: picklescan
-Version: 0.0.8
-Summary: Security scanner detecting Python Pickle files performing suspicious actions
-Home-page: https://github.com/mmaitre314/picklescan
-Author: Matthieu Maitre
-Author-email: mmaitre314@users.noreply.github.com
-Project-URL: Bug Tracker, https://github.com/mmaitre314/picklescan/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Pickle Malware Scanner
 
 [![PyPI](https://badge.fury.io/py/picklescan.svg)](https://pypi.org/project/picklescan/)
 [![Test](https://github.com/mmaitre314/picklescan/workflows/Test/badge.svg)](https://github.com/mmaitre314/picklescan/actions/workflows/test.yml)
 
 Security scanner detecting Python Pickle files performing suspicious actions.
 
@@ -39,14 +24,16 @@
 The scanner can also load Pickles from local files, directories, URLs, and zip archives (a-la [PyTorch](https://pytorch.org/)):
 ```bash
 picklescan --path downloads/pytorch_model.bin
 picklescan --path downloads
 picklescan --url https://huggingface.co/sshleifer/tiny-distilbert-base-cased-distilled-squad/resolve/main/pytorch_model.bin
 ```
 
+To scan Numpy's `.npy` files, pip install the `numpy` package first.
+
 The scanner exit status codes are (a-la [ClamAV](https://www.clamav.net/)):
 - `0`: scan did not find malware
 - `1`: scan found malware
 - `2`: scan failed
 
 ## Develop
```

### Comparing `picklescan-0.0.8/tests/test_scanner.py` & `picklescan-0.0.9/tests/test_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     _list_globals,
     scan_pickle_bytes,
     scan_zip_bytes,
     scan_directory_path,
     scan_file_path,
     scan_url,
     scan_huggingface_model,
+    scan_numpy,
     scan_pytorch,
 )
 
 
 _root_path = os.path.dirname(__file__)
 
 
@@ -157,14 +158,25 @@
 
 def initialize_zip_file(path, file_name, data):
     if not os.path.exists(path):
         with zipfile.ZipFile(path, "w") as zip:
             zip.writestr(file_name, data)
 
 
+def initialize_numpy_file(path):
+    import numpy as np
+
+    # create numpy object array
+    with open(path, "wb") as f:
+        data = [(1, 2), (3, 4)]
+        x = np.empty((2, 2), dtype=object)
+        x[:] = data
+        np.save(f, x)
+
+
 def initialize_pickle_files():
     os.makedirs(f"{_root_path}/data", exist_ok=True)
 
     # Test with Pickle versions 0, 3, and 4:
     # - Pickle versions 0, 1, 2 have built-in functions under '__builtin__' while versions 3 and 4 have them under 'builtins'
     # - Pickle versions 0, 1, 2, 3 use 'GLOBAL' opcode while 4 uses 'STACK_GLOBAL' opcode
     for version in (0, 3, 4):
@@ -199,14 +211,16 @@
 
     initialize_zip_file(
         f"{_root_path}/data/malicious1.zip",
         "data.pkl",
         pickle.dumps(Malicious1(), protocol=4),
     )
 
+    initialize_numpy_file(f"{_root_path}/data/object_array.npy")
+
 
 initialize_pickle_files()
 
 
 def compare_scan_results(sr1: ScanResult, sr2: ScanResult):
     test_case = TestCase()
     assert sr1.scanned_files == sr2.scanned_files
@@ -241,14 +255,31 @@
         zip.writestr("data.pkl", pickle.dumps(Malicious1()))
 
     assert scan_zip_bytes(io.BytesIO(buffer.getbuffer()), "test.zip") == ScanResult(
         [Global("builtins", "eval", SafetyLevel.Dangerous)], 1, 1, 1
     )
 
 
+def test_scan_numpy():
+    scan_result = ScanResult(
+        [
+            Global("numpy.core.multiarray", "_reconstruct", SafetyLevel.Suspicious),
+            Global("numpy", "ndarray", SafetyLevel.Suspicious),
+            Global("numpy", "dtype", SafetyLevel.Suspicious),
+        ],
+        1,
+        0,
+        0,
+    )
+    with open(f"{_root_path}/data/object_array.npy", "rb") as f:
+        compare_scan_results(
+            scan_numpy(io.BytesIO(f.read()), "object_array.npy"), scan_result
+        )
+
+
 def test_scan_pytorch():
     scan_result = ScanResult(
         [
             Global("torch", "FloatStorage", SafetyLevel.Innocuous),
             Global("collections", "OrderedDict", SafetyLevel.Innocuous),
             Global("torch._utils", "_rebuild_tensor_v2", SafetyLevel.Innocuous),
         ],
```

