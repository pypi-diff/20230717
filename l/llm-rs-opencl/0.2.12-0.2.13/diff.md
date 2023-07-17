# Comparing `tmp/llm_rs_opencl-0.2.12.tar.gz` & `tmp/llm_rs_opencl-0.2.13.tar.gz`

## Comparing `llm_rs_opencl-0.2.12.tar` & `llm_rs_opencl-0.2.13.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 llm_rs_opencl-0.2.12/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     3317 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/CI-CuBLAS.yml
--rw-r--r--   0     1001      123     2136 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/CI-Metal.yml
--rw-r--r--   0     1001      123     3124 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/CI-OpenCL.yml
--rw-r--r--   0     1001      123     6258 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3477 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.gitignore
--rw-r--r--   0     1001      123       72 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/LICENSE
--rw-r--r--   0     1001      123     7164 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/README.md
--rw-r--r--   0     1001      123      702 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/build_scripts/pyproject_patcher.py
--rw-r--r--   0     1001      123     1016 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/build_scripts/repair_windows_wheels.py
--rw-r--r--   0     1001      123       16 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/build_scripts/requirements.txt
--rw-r--r--   0     1001      123     4799 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/docs/requirements.txt
--rw-r--r--   0     1001      123      424 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/examples/haystack_example.py
--rw-r--r--   0     1001      123      764 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/examples/langchain_example.py
--rw-r--r--   0     1001      123      334 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/__init__.py
--rw-r--r--   0     1001      123    17102 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/auto.py
--rw-r--r--   0     1001      123     2129 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1728 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2305 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5820 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123       48 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/haystack/__init__.py
--rw-r--r--   0     1001      123     4878 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/haystack/haystack.py
--rw-r--r--   0     1001      123       37 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/langchain/__init__.py
--rw-r--r--   0     1001      123     4268 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/langchain/langchain.py
--rw-r--r--   0     1001      123        0 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/py.typed
--rw-r--r--   0     1001      123     2915 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/repository.py
--rw-r--r--   0     1001      123      697 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/llm_rs/results.pyi
--rw-r--r--   0     1001      123     1031 2023-06-27 13:32:11.000000 llm_rs_opencl-0.2.12/pyproject.toml
--rw-r--r--   0     1001      123     7863 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/configs.rs
--rw-r--r--   0     1001      123     1700 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/lib.rs
--rw-r--r--   0     1001      123    17963 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/models.rs
--rw-r--r--   0     1001      123     3190 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/results.rs
--rw-r--r--   0     1001      123     1821 2023-06-27 13:32:09.000000 llm_rs_opencl-0.2.12/src/stopwords.rs
--rw-r--r--   0     1001      123    62531 2023-06-27 13:32:17.000000 llm_rs_opencl-0.2.12/Cargo.lock
--rw-r--r--   0        0        0     8434 1970-01-01 00:00:00.000000 llm_rs_opencl-0.2.12/PKG-INFO
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 llm_rs_opencl-0.2.13/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     3796 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/CI-CuBLAS.yml
+-rw-r--r--   0     1001      123     2136 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/CI-Metal.yml
+-rw-r--r--   0     1001      123     4173 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/CI-OpenCL.yml
+-rw-r--r--   0     1001      123     6258 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3477 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.gitignore
+-rw-r--r--   0     1001      123       72 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/LICENSE
+-rw-r--r--   0     1001      123     7034 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/README.md
+-rw-r--r--   0     1001      123      702 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/build_scripts/pyproject_patcher.py
+-rw-r--r--   0     1001      123     1016 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/build_scripts/repair_windows_wheels.py
+-rw-r--r--   0     1001      123       16 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/build_scripts/requirements.txt
+-rw-r--r--   0     1001      123     4799 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/docs/requirements.txt
+-rw-r--r--   0     1001      123      424 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/examples/haystack_example.py
+-rw-r--r--   0     1001      123      764 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/examples/langchain_example.py
+-rw-r--r--   0     1001      123     1121 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    17102 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/auto.py
+-rw-r--r--   0     1001      123     2129 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1728 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2305 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5820 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123       48 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/haystack/__init__.py
+-rw-r--r--   0     1001      123     4878 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/haystack/haystack.py
+-rw-r--r--   0     1001      123       37 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/langchain/__init__.py
+-rw-r--r--   0     1001      123     4268 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/langchain/langchain.py
+-rw-r--r--   0     1001      123      170 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/llm_rs/results.pyi
+-rw-r--r--   0     1001      123     1031 2023-07-17 15:33:40.000000 llm_rs_opencl-0.2.13/pyproject.toml
+-rw-r--r--   0     1001      123     7824 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/configs.rs
+-rw-r--r--   0     1001      123     2164 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/lib.rs
+-rw-r--r--   0     1001      123    17704 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/models.rs
+-rw-r--r--   0     1001      123     3192 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/results.rs
+-rw-r--r--   0     1001      123     1820 2023-07-17 15:33:34.000000 llm_rs_opencl-0.2.13/src/stopwords.rs
+-rw-r--r--   0     1001      123    59466 2023-07-17 15:33:50.000000 llm_rs_opencl-0.2.13/Cargo.lock
+-rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 llm_rs_opencl-0.2.13/PKG-INFO
```

### Comparing `llm_rs_opencl-0.2.12/Cargo.toml` & `llm_rs_opencl-0.2.13/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
 name = "llm-rs"
-version = "0.2.12"
+version = "0.2.13"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "llm_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 rand = "0.8.5"
 rand_chacha = "0.3.1"
 log  =  "0.4.17"
 serde = "1.0.163"
 serde_json = "1.0"
 
-llm = { git = "https://github.com/LLukas22/llm.git", branch = "feat/cuda-opencl-acceleration"  }
-llm-base = { git = "https://github.com/LLukas22/llm.git", branch = "feat/cuda-opencl-acceleration" }
+llm = { git = "https://github.com/rustformers/llm.git", rev = "5d09eed"}
+llm-base = { git = "https://github.com/rustformers/llm.git", rev = "5d09eed"}
 
 [dependencies.pyo3]
-version = "0.19.0"
+version = "0.19.1"
 # "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with
 # Python 3.7 or later.
 features = ["abi3-py37","extension-module", "generate-import-lib"]
 
 [features]
 cublas = ["llm/cublas", "llm-base/cublas"]
 clblast = ["llm/clblast", "llm-base/clblast"]
```

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/BuildDoc.yml` & `llm_rs_opencl-0.2.13/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/CI-CuBLAS.yml` & `llm_rs_opencl-0.2.13/.github/workflows/CI-CuBLAS.yml`

 * *Files 12% similar despite different names*

```diff
@@ -32,20 +32,23 @@
         run: pip install -r ./build_scripts/requirements.txt
       - name: Set package name
         run: python ./build_scripts/pyproject_patcher.py
 
       - name: Install libssl-dev
         run: sudo apt-get install libssl-dev
 
-      - uses: Jimver/cuda-toolkit@v0.2.10
-        id: cuda-toolkit
-        with:
-          cuda: '12.1.0'
-          method: 'local'
-          linux-local-args: '["--toolkit"]'
+      - uses: Jimver/cuda-toolkit@v0.2.11
+        name: Install CUDA toolkit on Linux
+        id: cuda-toolkit-linux
+        with:
+          cuda: "12.2.0"
+          method: "network"
+          #See e.g. https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/
+          non-cuda-sub-packages: '["libcublas","libcublas-dev"]'
+          sub-packages: '["nvcc","compiler","libraries","libraries-dev","cudart","cudart-dev"]'
 
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter --features cublas
@@ -72,18 +75,22 @@
           architecture: ${{ matrix.target }}
 
       - name: Install build dependencies
         run: pip install -r ./build_scripts/requirements.txt
       - name: Set package name
         run: python ./build_scripts/pyproject_patcher.py
 
-      - uses: Jimver/cuda-toolkit@v0.2.10
-        id: cuda-toolkit
-        with:
-          cuda: '12.1.0'
+      - uses: Jimver/cuda-toolkit@v0.2.11
+        name: Install CUDA toolkit on Windows
+        id: cuda-toolkit-windows
+        with:
+          cuda: "12.2.0"
+          #See https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html#install-the-cuda-software
+          method: "local"
+          
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter --features cublas
           sccache: 'true'
```

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/CI-Metal.yml` & `llm_rs_opencl-0.2.13/.github/workflows/CI-Metal.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/CI.yml` & `llm_rs_opencl-0.2.13/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/Clippy.yml` & `llm_rs_opencl-0.2.13/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/.github/workflows/PublishDocs.yml` & `llm_rs_opencl-0.2.13/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/.gitignore` & `llm_rs_opencl-0.2.13/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/LICENSE` & `llm_rs_opencl-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/README.md` & `llm_rs_opencl-0.2.13/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,54 +2,54 @@
 
 [![PyPI](https://img.shields.io/pypi/v/llm-rs)](https://pypi.org/project/llm-rs/)
 [![PyPI - License](https://img.shields.io/pypi/l/llm-rs)](https://pypi.org/project/llm-rs/)
 [![Downloads](https://static.pepy.tech/badge/llm-rs)](https://pepy.tech/project/llm-rs)
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
-With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU. 
+With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU or GPU. 
 
 For a detailed overview of all the supported architectures, visit the [llm](https://github.com/rustformers/llm) project page. 
 
 ### Integrations:
 * 🦜️🔗 [LangChain](https://github.com/hwchase17/langchain)
 * 🌾🔱 [Haystack](https://github.com/deepset-ai/haystack)
 
 ## Installation
 
 Simply install it via pip: `pip install llm-rs`
 
-### Installation with GPU Acceleration Support
-> ⚠️ Please note that GPU Acceleration support is currently in its experimental phase.
+<details>
+<summary>Installation with GPU Acceleration Support</summary>
+<br>
 
 `llm-rs` incorporates support for various GPU-accelerated backends to facilitate enhanced inference times. To enable GPU-acceleration the `use_gpu` parameter of your `SessionConfig` must be set to `True`. We distribute prebuilt binaries for the following operating systems and graphics APIs:
 
-#### MacOS (Using Metal)
+### MacOS (Using Metal)
 For MacOS users, the Metal-supported version of `llm-rs` can be easily installed via pip:
 
 `
 pip install llm-rs-metal
 `
 
-#### Windows/Linux (Using CUDA for Nvidia GPUs)
+### Windows/Linux (Using CUDA for Nvidia GPUs)
 Due to the significant file size, CUDA-supported packages cannot be directly uploaded to `pip`. To install them, download the appropriate `*.whl` file from the latest [Release](https://github.com/LLukas22/llm-rs-python/releases/latest) and install it using pip as follows:
 
 `
 pip install [wheelname].whl
 `
 
-#### Windows/Linux (Using OpenCL for All GPUs)
-> ⚠️ OpenCL support is highly experimental and may not provide stable results.
+### Windows/Linux (Using OpenCL for All GPUs)
 
 For universal GPU support on Windows and Linux, we offer an OpenCL-supported version. It can be installed via pip:
 
 `
 pip install llm-rs-opencl
 `
-
+</details>
 
 
 ## Usage
 ### Running local GGML models:
 Models can be loaded via the `AutoModel` interface.
 
 ```python
```

### Comparing `llm_rs_opencl-0.2.12/build_scripts/pyproject_patcher.py` & `llm_rs_opencl-0.2.13/build_scripts/pyproject_patcher.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/build_scripts/repair_windows_wheels.py` & `llm_rs_opencl-0.2.13/build_scripts/repair_windows_wheels.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/docs/docs/conversion.md` & `llm_rs_opencl-0.2.13/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/docs/docs/index.md` & `llm_rs_opencl-0.2.13/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/docs/mkdocs.yml` & `llm_rs_opencl-0.2.13/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/examples/langchain_example.py` & `llm_rs_opencl-0.2.13/examples/langchain_example.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/auto.py` & `llm_rs_opencl-0.2.13/llm_rs/auto.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/base_model.py` & `llm_rs_opencl-0.2.13/llm_rs/base_model.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/config.pyi` & `llm_rs_opencl-0.2.13/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/auto_converter.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/_base.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/_base.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/bloom.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/gpt2.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/gptj.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/gptneox.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/llama.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/convert/models/mpt.py` & `llm_rs_opencl-0.2.13/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/haystack/haystack.py` & `llm_rs_opencl-0.2.13/llm_rs/haystack/haystack.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/langchain/langchain.py` & `llm_rs_opencl-0.2.13/llm_rs/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/models.pyi` & `llm_rs_opencl-0.2.13/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/repository.py` & `llm_rs_opencl-0.2.13/llm_rs/repository.py`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/llm_rs/results.pyi` & `llm_rs_opencl-0.2.13/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/pyproject.toml` & `llm_rs_opencl-0.2.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/src/configs.rs` & `llm_rs_opencl-0.2.13/src/configs.rs`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,16 @@
             self.max_new_tokens,
             self.stop_words.clone(),
         ))
     }
 }
 
 impl GenerationConfig {
-    pub fn to_llm_params(&self, n_threads: usize) -> InferenceParameters {
+    pub fn to_llm_params(&self) -> InferenceParameters {
         InferenceParameters {
-            n_threads,
             sampler: std::sync::Arc::new(llm::samplers::TopPTopK {
                 top_k: self.top_k,
                 top_p: self.top_p,
                 temperature: self.temperature,
                 repeat_penalty: self.repetition_penalty,
                 repetition_penalty_last_n: self.repetition_penalty_last_n,
                 bias_tokens: TokenBias::default(),
@@ -264,11 +263,11 @@
 
 impl SessionConfig {
     pub fn to_llm_params(self) -> InferenceSessionConfig {
         InferenceSessionConfig {
             memory_k_type: self.keys_memory_type.to_llama_rs_memory_type(),
             memory_v_type: self.values_memory_type.to_llama_rs_memory_type(),
             n_batch: self.batch_size,
-            use_gpu: self.use_gpu,
+            n_threads: self.threads,
         }
     }
 }
```

### Comparing `llm_rs_opencl-0.2.12/src/model_base.rs` & `llm_rs_opencl-0.2.13/src/model_base.rs`

 * *Files 5% similar despite different names*

```diff
@@ -87,23 +87,23 @@
             }
         }
     }
 }
 
 pub fn _tokenize(model: &dyn llm::Model, text: &str) -> Result<Vec<u32>, InferenceError> {
     Ok(model
-        .vocabulary()
+        .tokenizer()
         .tokenize(text, false)?
         .iter()
         .map(|(_, token)| *token)
         .collect())
 }
 
 pub fn _decode(model: &dyn llm::Model, tokens: Vec<u32>) -> Result<String, std::str::Utf8Error> {
-    let vocab = model.vocabulary();
+    let vocab = model.tokenizer();
     let characters: Vec<u8> = vocab.decode(tokens, false);
 
     match std::str::from_utf8(&characters) {
         Ok(text) => Ok(text.to_string()),
         Err(e) => Err(e),
     }
 }
@@ -120,15 +120,15 @@
     Prompt<'a>,
     InferenceSession,
 ) {
     let session_params = session_config.to_llm_params();
     //Build the correct generation parameters
     let mut config_to_use = generation_config.unwrap_or(configs::GenerationConfig::default());
 
-    let generation_params = config_to_use.to_llm_params(session_config.threads);
+    let generation_params = config_to_use.to_llm_params();
 
     let rng = ChaCha8Rng::seed_from_u64(config_to_use.seed);
     let prompt = Prompt::from(prompt);
 
     config_to_use.init_stop_words(model);
 
     let session = model.start_session(session_params);
@@ -189,21 +189,17 @@
 
     let feed_start_at = std::time::SystemTime::now();
     //Feed the prompt
 
     let mut output_request_feeding = OutputRequest::default();
     _py.allow_threads(|| {
         session
-            .feed_prompt::<Infallible, _>(
-                model,
-                &inference_params,
-                prompt,
-                &mut output_request_feeding,
-                |_| Ok(InferenceFeedback::Continue),
-            )
+            .feed_prompt::<Infallible, _>(model, prompt, &mut output_request_feeding, |_| {
+                Ok(InferenceFeedback::Continue)
+            })
             .unwrap()
     });
     let feed_prompt_duration = feed_start_at.elapsed().unwrap();
 
     //Start the inference loop
     let mut tokens_processed = 0;
     let mut token_utf8_buf = TokenUtf8Buffer::new();
@@ -279,31 +275,26 @@
 
 pub fn _embed(
     _py: Python,
     model: &dyn llm::Model,
     session_config: &configs::SessionConfig,
     prompt: String,
 ) -> Result<Vec<f32>, PyErr> {
-    let (_, inference_params, _, prompt, mut session) =
-        _start_session(model, session_config, &prompt, None);
+    let (_, _, _, prompt, mut session) = _start_session(model, session_config, &prompt, None);
 
     //Feed the prompt
     let mut output_request_feeding = OutputRequest {
         all_logits: None,
         embeddings: Some(Vec::new()),
     };
     _py.allow_threads(|| {
         session
-            .feed_prompt::<Infallible, _>(
-                model,
-                &inference_params,
-                prompt,
-                &mut output_request_feeding,
-                |_| Ok(InferenceFeedback::Continue),
-            )
+            .feed_prompt::<Infallible, _>(model, prompt, &mut output_request_feeding, |_| {
+                Ok(InferenceFeedback::Continue)
+            })
             .unwrap()
     });
     Ok(output_request_feeding.embeddings.unwrap())
 }
 
 macro_rules! wrap_model {
     ($name:ident,$llm_model:ty) => {
@@ -344,30 +335,30 @@
                     context_size: config_to_use.context_length,
                     prefer_mmap: config_to_use.prefer_mmap,
                     lora_adapters: lora_paths.clone(),
                     use_gpu: config_to_use.use_gpu,
                     gpu_layers: config_to_use.gpu_layers,
                 };
 
-                let vocabulary_source: llm_base::VocabularySource;
+                let vocabulary_source: llm_base::TokenizerSource;
 
                 if let Some(name_or_path) = tokenizer_name_or_path {
                     let tokenizer_path = std::path::Path::new(&name_or_path);
                     if tokenizer_path.is_file() && tokenizer_path.exists() {
                         // Load tokenizer from file
-                        vocabulary_source = llm_base::VocabularySource::HuggingFaceTokenizerFile(
+                        vocabulary_source = llm_base::TokenizerSource::HuggingFaceTokenizerFile(
                             tokenizer_path.to_owned(),
                         );
                     } else {
                         // Load tokenizer from HuggingFace
                         vocabulary_source =
-                            llm_base::VocabularySource::HuggingFaceRemote(name_or_path);
+                            llm_base::TokenizerSource::HuggingFaceRemote(name_or_path);
                     }
                 } else {
-                    vocabulary_source = llm_base::VocabularySource::Model;
+                    vocabulary_source = llm_base::TokenizerSource::Embedded;
                 }
 
                 let llm_model: $llm_model =
                     llm_base::load(&path, vocabulary_source, model_params, |load_progress| {
                         if should_log {
                             llm_base::load_progress_callback_stdout(load_progress)
                         }
@@ -430,15 +421,14 @@
 
                 //feed the session
                 let mut output_request_feeding = llm_base::OutputRequest::default();
                 _py.allow_threads(|| {
                     session
                         .feed_prompt::<std::convert::Infallible, _>(
                             self.llm_model.as_ref(),
-                            &inference_params,
                             prompt,
                             &mut output_request_feeding,
                             |_| Ok(llm_base::InferenceFeedback::Continue),
                         )
                         .unwrap()
                 });
```

### Comparing `llm_rs_opencl-0.2.12/src/quantize.rs` & `llm_rs_opencl-0.2.13/src/quantize.rs`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
             element_type: llm_base::ggml::Type::F16,
         }),
     }?;
 
     let mut source_reader = BufReader::new(std::fs::File::open(&source)?);
     let mut destination_reader = BufWriter::new(std::fs::File::create(destination)?);
-    let vocabulary = llm::VocabularySource::Model.retrieve(&source).unwrap();
+    let vocabulary = llm::TokenizerSource::Embedded.retrieve(&source).unwrap();
 
     quantize::<M, _, _>(
         &mut source_reader,
         &mut destination_reader,
         vocabulary,
         container,
         quantization,
```

### Comparing `llm_rs_opencl-0.2.12/src/results.rs` & `llm_rs_opencl-0.2.13/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_opencl-0.2.12/src/stopwords.rs` & `llm_rs_opencl-0.2.13/src/stopwords.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 impl StopWordHandler {
     pub fn new(model: &dyn llm::Model, stop_words: &[String]) -> StopWordHandler {
         let tokenized_stop_words: HashSet<Vec<u8>> = stop_words
             .iter()
             .map(|word| {
                 model
-                    .vocabulary()
+                    .tokenizer()
                     .tokenize(word, false)
                     .unwrap()
                     .iter()
                     .flat_map(|(encoding, _)| encoding.to_owned())
                     .collect::<Vec<u8>>()
             })
             .collect();
```

### Comparing `llm_rs_opencl-0.2.12/Cargo.lock` & `llm_rs_opencl-0.2.13/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aes"
@@ -34,69 +43,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "anstream"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
-dependencies = [
- "anstyle",
- "anstyle-parse",
- "anstyle-query",
- "anstyle-wincon",
- "colorchoice",
- "is-terminal",
- "utf8parse",
-]
-
-[[package]]
-name = "anstyle"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
-
-[[package]]
-name = "anstyle-parse"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
-dependencies = [
- "utf8parse",
-]
-
-[[package]]
-name = "anstyle-query"
-version = "1.0.0"
+name = "autocfg"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
-dependencies = [
- "windows-sys 0.48.0",
-]
+checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
-name = "anstyle-wincon"
-version = "1.0.1"
+name = "backtrace"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
 dependencies = [
- "anstyle",
- "windows-sys 0.48.0",
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
 ]
 
 [[package]]
-name = "autocfg"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
-
-[[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
@@ -175,15 +150,15 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "097968e38f1319207f057d0f4d76452e4f4f847a5de61c5215379f297fa034f3"
 dependencies = [
  "flate2",
  "fs2",
  "glob",
- "indicatif 0.16.2",
+ "indicatif",
  "log",
  "rand",
  "reqwest",
  "serde",
  "serde_json",
  "sha2",
  "tar",
@@ -214,71 +189,22 @@
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
-name = "clap"
-version = "4.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9394150f5b4273a1763355bd1c2ec54cc5a2593f790587bcd6b2c947cfa9211"
-dependencies = [
- "clap_builder",
- "clap_derive",
- "once_cell",
-]
-
-[[package]]
-name = "clap_builder"
-version = "4.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a78fbdd3cc2914ddf37ba444114bc7765bbdcb55ec9cbe6fa054f0137400717"
-dependencies = [
- "anstream",
- "anstyle",
- "bitflags",
- "clap_lex",
- "strsim",
-]
-
-[[package]]
-name = "clap_derive"
-version = "4.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
-dependencies = [
- "heck",
- "proc-macro2",
- "quote",
- "syn 2.0.22",
-]
-
-[[package]]
-name = "clap_lex"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
-
-[[package]]
-name = "colorchoice"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
-
-[[package]]
 name = "console"
 version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
- "unicode-width",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "constant_time_eq"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -298,17 +224,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -517,17 +443,14 @@
 ]
 
 [[package]]
 name = "esaxx-rs"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f748b253ceca9fed5f42f8b5ceb3851e93102199bc25b64b65369f76e5c0a35"
-dependencies = [
- "cc",
-]
 
 [[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
@@ -664,30 +587,36 @@
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "ggml-sys",
  "memmap2",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
@@ -706,48 +635,32 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
 dependencies = [
- "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
-name = "heck"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
-
-[[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
@@ -849,33 +762,21 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indicatif"
-version = "0.15.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7baab56125e25686df467fe470785512329883aab42696d661247aca2a2896e4"
-dependencies = [
- "console",
- "lazy_static",
- "number_prefix 0.3.0",
- "regex",
-]
-
-[[package]]
-name = "indicatif"
 version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d207dc617c7a380ab07ff572a6e52fa202a2a8f355860ac9c38e23f8196be1b"
 dependencies = [
  "console",
  "lazy_static",
- "number_prefix 0.4.0",
+ "number_prefix",
  "regex",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -901,38 +802,26 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnet"
 version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
-name = "is-terminal"
-version = "0.4.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
-dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.48.0",
-]
-
-[[package]]
 name = "itertools"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f56a2d0bc861f9165be4eb3442afd3c236d8a98afd426f65d92324ae1091a484"
 dependencies = [
  "either",
 ]
@@ -944,17 +833,17 @@
 checksum = "284f18f85651fe11e8a991b2adb42cb078325c996ed026d994719efcfca1d54b"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
@@ -987,104 +876,99 @@
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "llm"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
  "llm-gptneox",
  "llm-llama",
  "llm-mpt",
  "serde",
+ "tracing",
 ]
 
 [[package]]
 name = "llm-base"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
  "regex",
  "serde",
  "serde_bytes",
  "thiserror",
  "tokenizers",
+ "tracing",
 ]
 
 [[package]]
 name = "llm-bloom"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
- "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
- "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptneox"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
- "bytemuck",
  "llm-base",
- "serde",
 ]
 
 [[package]]
 name = "llm-llama"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
- "bytemuck",
  "llm-base",
- "rand",
- "thiserror",
+ "tracing",
 ]
 
 [[package]]
 name = "llm-mpt"
 version = "0.2.0-dev"
-source = "git+https://github.com/LLukas22/llm.git?branch=feat/cuda-opencl-acceleration#a1f61b46a4e6f5c465928a0e21e0fff0b5eb9fc6"
+source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
- "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.12"
+version = "0.2.13"
 dependencies = [
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
@@ -1178,31 +1062,31 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "monostate"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0230b703f1ac35df1e24f6d0d2255472bcccaf657ecdfa4f1fcbcad1ad5bb98a"
+checksum = "3f3f57a8802842f648026a33c3d2e3bb41bb309a35b1609bd7ef2b060b8b6b1b"
 dependencies = [
  "monostate-impl",
  "serde",
 ]
 
 [[package]]
 name = "monostate-impl"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8795add3e14028f11f8e848bd3294898a8294767b3776b6f733560d33bd2530b"
+checksum = "e72f4d2e10fde62a0f2fcb4b44ccbf4f9899dcc30c9193449f8dfb9123d71377"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -1227,33 +1111,36 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "number_prefix"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17b02fc0ff9a9e4b35b3342880f48e896ebf69f2967921fe8646bf5b7125956a"
+checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
-name = "number_prefix"
-version = "0.4.0"
+name = "object"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
@@ -1298,15 +1185,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1339,15 +1226,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "partial_sort"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7924d1d0ad836f665c9065e26d016c673ece3993f30d340068b16f282afc1156"
@@ -1361,17 +1248,17 @@
  "base64ct",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pbkdf2"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
 dependencies = [
@@ -1385,17 +1272,17 @@
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1409,96 +1296,96 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python3-dll-a"
-version = "0.2.7"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "212d74540270e3a22eed5f0d4bbc0765dff20958d694e9d4f5ebe6e22778c422"
+checksum = "d5f07cd4412be8fa09a721d40007c483981bbe072cd6a21f2e83e04ec8f8343f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1589,34 +1476,46 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick 1.0.2",
+ "memchr",
+ "regex-automata",
+ "regex-syntax 0.7.4",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick 1.0.2",
  "memchr",
- "regex-syntax 0.7.2",
+ "regex-syntax 0.7.4",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
@@ -1648,47 +1547,53 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
 version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
@@ -1707,46 +1612,46 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.9"
+version = "0.11.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
+checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1790,17 +1695,17 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "socket2"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
@@ -1841,39 +1746,39 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.22"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tar"
-version = "0.4.38"
+version = "0.4.39"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b55807c0344e1e6c04d7c965f5289c39a8d94ae23ed5c0b57aabac549f871c6"
+checksum = "ec96d2ffad078296368d46ff1cb309be1c23c513b4ab0e22a45de0185275ac96"
 dependencies = [
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "tempfile"
 version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
@@ -1883,37 +1788,37 @@
  "redox_syscall 0.3.5",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
 dependencies = [
  "serde",
  "time-core",
 ]
 
 [[package]]
 name = "time-core"
@@ -1940,20 +1845,18 @@
 name = "tokenizers"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cf49017523bf0bc01c9966f172c5f120bbb7b96cccd1708772dd42e767fb9f5"
 dependencies = [
  "aho-corasick 0.7.20",
  "cached-path",
- "clap",
  "derive_builder",
  "dirs",
  "esaxx-rs",
  "getrandom",
- "indicatif 0.15.0",
  "itertools 0.9.0",
  "lazy_static",
  "log",
  "macro_rules_attribute",
  "monostate",
  "onig",
  "paste",
@@ -1970,19 +1873,20 @@
  "unicode-normalization-alignments",
  "unicode-segmentation",
  "unicode_categories",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
@@ -2021,19 +1925,32 @@
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
+ "log",
  "pin-project-lite",
+ "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
+name = "tracing-attributes"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
@@ -2054,17 +1971,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -2083,20 +2000,14 @@
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "unicode_categories"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39ec24b3121d976906ece63c9daad25b85969647682eee313cb5779fdd69e14e"
 
 [[package]]
 name = "unindent"
@@ -2112,20 +2023,14 @@
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
-name = "utf8parse"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
-
-[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "version_check"
@@ -2165,15 +2070,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2199,15 +2104,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.26",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2244,43 +2149,28 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -2292,17 +2182,17 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.0",
  "windows_aarch64_msvc 0.48.0",
  "windows_i686_gnu 0.48.0",
  "windows_i686_msvc 0.48.0",
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
```

### Comparing `llm_rs_opencl-0.2.12/PKG-INFO` & `llm_rs_opencl-0.2.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-rs-opencl
-Version: 0.2.12
+Version: 0.2.13
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
@@ -32,54 +32,54 @@
 
 [![PyPI](https://img.shields.io/pypi/v/llm-rs)](https://pypi.org/project/llm-rs/)
 [![PyPI - License](https://img.shields.io/pypi/l/llm-rs)](https://pypi.org/project/llm-rs/)
 [![Downloads](https://static.pepy.tech/badge/llm-rs)](https://pepy.tech/project/llm-rs)
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
-With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU. 
+With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU or GPU. 
 
 For a detailed overview of all the supported architectures, visit the [llm](https://github.com/rustformers/llm) project page. 
 
 ### Integrations:
 * 🦜️🔗 [LangChain](https://github.com/hwchase17/langchain)
 * 🌾🔱 [Haystack](https://github.com/deepset-ai/haystack)
 
 ## Installation
 
 Simply install it via pip: `pip install llm-rs`
 
-### Installation with GPU Acceleration Support
-> ⚠️ Please note that GPU Acceleration support is currently in its experimental phase.
+<details>
+<summary>Installation with GPU Acceleration Support</summary>
+<br>
 
 `llm-rs` incorporates support for various GPU-accelerated backends to facilitate enhanced inference times. To enable GPU-acceleration the `use_gpu` parameter of your `SessionConfig` must be set to `True`. We distribute prebuilt binaries for the following operating systems and graphics APIs:
 
-#### MacOS (Using Metal)
+### MacOS (Using Metal)
 For MacOS users, the Metal-supported version of `llm-rs` can be easily installed via pip:
 
 `
 pip install llm-rs-metal
 `
 
-#### Windows/Linux (Using CUDA for Nvidia GPUs)
+### Windows/Linux (Using CUDA for Nvidia GPUs)
 Due to the significant file size, CUDA-supported packages cannot be directly uploaded to `pip`. To install them, download the appropriate `*.whl` file from the latest [Release](https://github.com/LLukas22/llm-rs-python/releases/latest) and install it using pip as follows:
 
 `
 pip install [wheelname].whl
 `
 
-#### Windows/Linux (Using OpenCL for All GPUs)
-> ⚠️ OpenCL support is highly experimental and may not provide stable results.
+### Windows/Linux (Using OpenCL for All GPUs)
 
 For universal GPU support on Windows and Linux, we offer an OpenCL-supported version. It can be installed via pip:
 
 `
 pip install llm-rs-opencl
 `
-
+</details>
 
 
 ## Usage
 ### Running local GGML models:
 Models can be loaded via the `AutoModel` interface.
 
 ```python
```

