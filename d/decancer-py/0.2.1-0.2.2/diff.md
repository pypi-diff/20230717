# Comparing `tmp/decancer_py-0.2.1.tar.gz` & `tmp/decancer_py-0.2.2.tar.gz`

## Comparing `decancer_py-0.2.1.tar` & `decancer_py-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 decancer_py-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     4207 2022-12-27 02:32:35.000000 decancer_py-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      123      697 2022-12-27 02:32:35.000000 decancer_py-0.2.1/.gitignore
--rw-r--r--   0     1001      123     1066 2022-12-27 02:32:35.000000 decancer_py-0.2.1/LICENSE
--rw-r--r--   0     1001      123      961 2022-12-27 02:32:35.000000 decancer_py-0.2.1/README.md
--rw-r--r--   0     1001      123      155 2022-12-27 02:32:35.000000 decancer_py-0.2.1/decancer_py/__init__.py
--rw-r--r--   0     1001      123     1561 2022-12-27 02:32:35.000000 decancer_py-0.2.1/decancer_py/decancer_py.pyi
--rw-r--r--   0     1001      123        0 2022-12-27 02:32:35.000000 decancer_py-0.2.1/decancer_py/py.typed
--rw-r--r--   0     1001      123      219 2022-12-27 02:32:35.000000 decancer_py-0.2.1/noxfile.py
--rw-r--r--   0     1001      123    22753 2022-12-27 02:32:35.000000 decancer_py-0.2.1/poetry.lock
--rw-r--r--   0     1001      123     1055 2022-12-27 02:32:35.000000 decancer_py-0.2.1/pyproject.toml
--rwxr-xr-x   0     1001      123      995 2022-12-27 02:33:05.000000 decancer_py-0.2.1/run-maturin-action.sh
--rw-r--r--   0     1001      123       32 2022-12-27 02:32:35.000000 decancer_py-0.2.1/rustfmt.toml
--rw-r--r--   0     1001      123     1974 2022-12-27 02:32:35.000000 decancer_py-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123     1163 2022-12-27 02:32:35.000000 decancer_py-0.2.1/tests/test_decancer.py
--rw-r--r--   0        0        0     7383 2022-12-27 02:33:39.000000 decancer_py-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 decancer_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 decancer_py-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123      192 2023-07-17 04:46:10.000000 decancer_py-0.2.2/.github/dependabot.yml
+-rw-r--r--   0     1001      123     4227 2023-07-17 04:46:10.000000 decancer_py-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      697 2023-07-17 04:46:10.000000 decancer_py-0.2.2/.gitignore
+-rw-r--r--   0     1001      123     1066 2023-07-17 04:46:10.000000 decancer_py-0.2.2/LICENSE
+-rw-r--r--   0     1001      123       85 2023-07-17 04:46:10.000000 decancer_py-0.2.2/MANIFEST.in
+-rw-r--r--   0     1001      123      961 2023-07-17 04:46:10.000000 decancer_py-0.2.2/README.md
+-rw-r--r--   0     1001      123      155 2023-07-17 04:46:10.000000 decancer_py-0.2.2/decancer_py/__init__.py
+-rw-r--r--   0     1001      123     1561 2023-07-17 04:46:10.000000 decancer_py-0.2.2/decancer_py/decancer_py.pyi
+-rw-r--r--   0     1001      123        0 2023-07-17 04:46:10.000000 decancer_py-0.2.2/decancer_py/py.typed
+-rw-r--r--   0     1001      123      219 2023-07-17 04:46:10.000000 decancer_py-0.2.2/noxfile.py
+-rw-r--r--   0     1001      123    18830 2023-07-17 04:46:10.000000 decancer_py-0.2.2/poetry.lock
+-rw-r--r--   0     1001      123     1080 2023-07-17 04:46:10.000000 decancer_py-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123       17 2023-07-17 04:46:10.000000 decancer_py-0.2.2/rustfmt.toml
+-rw-r--r--   0     1001      123     1938 2023-07-17 04:46:10.000000 decancer_py-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     1042 2023-07-17 04:46:10.000000 decancer_py-0.2.2/tests/test_decancer.py
+-rw-r--r--   0        0        0     7392 2023-07-17 04:46:59.000000 decancer_py-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 decancer_py-0.2.2/PKG-INFO
```

### Comparing `decancer_py-0.2.1/Cargo.toml` & `decancer_py-0.2.2/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "decancer_py"
 description = "Python bindings for decancer."
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/decancer_py"
 repository = "https://github.com/Jonxslays/decancer_py"
 documentation = "https://github.com/Jonxslays/decancer_py"
@@ -14,11 +14,11 @@
 
 [lib]
 name = "decancer_py"
 crate-type = ["cdylib"]
 
 [dependencies]
 # Sweet lib that does all the work for us
-decancer = "1.5.2"
+decancer = "1.6.4"
 
 # The most beautiful bindings in existence
 pyo3 = { version = "0.16.5", features = ["extension-module"] }
```

### Comparing `decancer_py-0.2.1/.github/workflows/ci.yml` & `decancer_py-0.2.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
       - name: Checkout code
         uses: actions/checkout@v3
 
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           command: build
-          args: "--release -i 3.7 3.8 3.9 3.10 3.11 -o dist --universal2"
+          args: "--release -i 3.7 3.8 3.9 3.10 3.11 -o dist --target universal2-apple-darwin"
 
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
```

### Comparing `decancer_py-0.2.1/.gitignore` & `decancer_py-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `decancer_py-0.2.1/LICENSE` & `decancer_py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decancer_py-0.2.1/README.md` & `decancer_py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `decancer_py-0.2.1/decancer_py/decancer_py.pyi` & `decancer_py-0.2.2/decancer_py/decancer_py.pyi`

 * *Files identical despite different names*

### Comparing `decancer_py-0.2.1/poetry.lock` & `decancer_py-0.2.2/poetry.lock`

 * *Files 17% similar despite different names*

```diff
@@ -1,116 +1,101 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
 name = "argcomplete"
-version = "2.0.0"
+version = "3.1.1"
 description = "Bash tab completion for argparse"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "argcomplete-2.0.0-py2.py3-none-any.whl", hash = "sha256:cffa11ea77999bb0dd27bb25ff6dc142a6796142f68d45b1a26b11f58724561e"},
-    {file = "argcomplete-2.0.0.tar.gz", hash = "sha256:6372ad78c89d662035101418ae253668445b391755cfe94ea52f1b9d22425b20"},
+    {file = "argcomplete-3.1.1-py3-none-any.whl", hash = "sha256:35fa893a88deea85ea7b20d241100e64516d6af6d7b0ae2bed1d263d26f70948"},
+    {file = "argcomplete-3.1.1.tar.gz", hash = "sha256:6c4c563f14f01440aaffa3eae13441c5db2357b5eec639abe7c0b15334627dff"},
 ]
 
 [package.dependencies]
-importlib-metadata = {version = ">=0.23,<5", markers = "python_version == \"3.7\""}
-
-[package.extras]
-test = ["coverage", "flake8", "pexpect", "wheel"]
-
-[[package]]
-name = "attrs"
-version = "22.2.0"
-description = "Classes Without Boilerplate"
-category = "dev"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
-    {file = "attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
-]
+importlib-metadata = {version = ">=0.23,<7", markers = "python_version < \"3.8\""}
 
 [package.extras]
-cov = ["attrs[tests]", "coverage-enable-subprocess", "coverage[toml] (>=5.3)"]
-dev = ["attrs[docs,tests]"]
-docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope.interface"]
-tests = ["attrs[tests-no-zope]", "zope.interface"]
-tests-no-zope = ["cloudpickle", "cloudpickle", "hypothesis", "hypothesis", "mypy (>=0.971,<0.990)", "mypy (>=0.971,<0.990)", "pympler", "pympler", "pytest (>=4.3.0)", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-mypy-plugins", "pytest-xdist[psutil]", "pytest-xdist[psutil]"]
+test = ["coverage", "mypy", "pexpect", "ruff", "wheel"]
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "23.7.0"
 description = "The uncompromising code formatter."
-category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
-    {file = "black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
-    {file = "black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
-    {file = "black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
-    {file = "black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
-    {file = "black-22.12.0-cp37-cp37m-win_amd64.whl", hash = "sha256:1f58cbe16dfe8c12b7434e50ff889fa479072096d79f0a7f25e4ab8e94cd8350"},
-    {file = "black-22.12.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77d86c9f3db9b1bf6761244bc0b3572a546f5fe37917a044e02f3166d5aafa7d"},
-    {file = "black-22.12.0-cp38-cp38-win_amd64.whl", hash = "sha256:82d9fe8fee3401e02e79767016b4907820a7dc28d70d137eb397b92ef3cc5bfc"},
-    {file = "black-22.12.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101c69b23df9b44247bd88e1d7e90154336ac4992502d4197bdac35dd7ee3320"},
-    {file = "black-22.12.0-cp39-cp39-win_amd64.whl", hash = "sha256:559c7a1ba9a006226f09e4916060982fd27334ae1998e7a38b3f33a37f7a2148"},
-    {file = "black-22.12.0-py3-none-any.whl", hash = "sha256:436cc9167dd28040ad90d3b404aec22cedf24a6e4d7de221bec2730ec0c97bcf"},
-    {file = "black-22.12.0.tar.gz", hash = "sha256:229351e5a18ca30f447bf724d007f890f97e13af070bb6ad4c0a441cd7596a2f"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be"},
+    {file = "black-23.7.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc"},
+    {file = "black-23.7.0-cp310-cp310-win_amd64.whl", hash = "sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a"},
+    {file = "black-23.7.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926"},
+    {file = "black-23.7.0-cp311-cp311-win_amd64.whl", hash = "sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6"},
+    {file = "black-23.7.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a"},
+    {file = "black-23.7.0-cp38-cp38-win_amd64.whl", hash = "sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087"},
+    {file = "black-23.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91"},
+    {file = "black-23.7.0-cp39-cp39-win_amd64.whl", hash = "sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491"},
+    {file = "black-23.7.0-py3-none-any.whl", hash = "sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96"},
+    {file = "black-23.7.0.tar.gz", hash = "sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
+packaging = ">=22.0"
 pathspec = ">=0.9.0"
 platformdirs = ">=2"
-tomli = {version = ">=1.1.0", markers = "python_full_version < \"3.11.0a7\""}
-typed-ast = {version = ">=1.4.2", markers = "python_version < \"3.8\" and implementation_name == \"cpython\""}
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typing-extensions = {version = ">=3.10.0.0", markers = "python_version < \"3.10\""}
 
 [package.extras]
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "click"
-version = "8.1.3"
+version = "8.1.5"
 description = "Composable command line interface toolkit"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
+    {file = "click-8.1.5-py3-none-any.whl", hash = "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"},
+    {file = "click-8.1.5.tar.gz", hash = "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
-importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
-category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "colorlog"
 version = "6.7.0"
 description = "Add colours to the output of Python's logging module."
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "colorlog-6.7.0-py2.py3-none-any.whl", hash = "sha256:0d33ca236784a1ba3ff9c532d4964126d8a2c44f1f0cb1d2b0728196f512f662"},
     {file = "colorlog-6.7.0.tar.gz", hash = "sha256:bd94bd21c1e13fac7bd3153f4bc3a7dc0eb0974b8bc2fdf1a989e474f6e582e5"},
 ]
 
@@ -120,328 +105,279 @@
 [package.extras]
 development = ["black", "flake8", "mypy", "pytest", "types-colorama"]
 
 [[package]]
 name = "distlib"
 version = "0.3.6"
 description = "Distribution utilities"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
     {file = "distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.0"
+version = "1.1.2"
 description = "Backport of PEP 654 (exception groups)"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.1.0-py3-none-any.whl", hash = "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e"},
-    {file = "exceptiongroup-1.1.0.tar.gz", hash = "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"},
+    {file = "exceptiongroup-1.1.2-py3-none-any.whl", hash = "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"},
+    {file = "exceptiongroup-1.1.2.tar.gz", hash = "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "filelock"
-version = "3.8.2"
+version = "3.12.2"
 description = "A platform independent file lock."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "filelock-3.8.2-py3-none-any.whl", hash = "sha256:8df285554452285f79c035efb0c861eb33a4bcfa5b7a137016e32e6a90f9792c"},
-    {file = "filelock-3.8.2.tar.gz", hash = "sha256:7565f628ea56bfcd8e54e42bdc55da899c85c1abfe1b5bcfd147e9188cebb3b2"},
+    {file = "filelock-3.12.2-py3-none-any.whl", hash = "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"},
+    {file = "filelock-3.12.2.tar.gz", hash = "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81"},
 ]
 
 [package.extras]
-docs = ["furo (>=2022.9.29)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-testing = ["covdefaults (>=2.2.2)", "coverage (>=6.5)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+testing = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "diff-cover (>=7.5)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)", "pytest-timeout (>=2.1)"]
 
 [[package]]
 name = "importlib-metadata"
-version = "4.13.0"
+version = "6.7.0"
 description = "Read metadata from Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-4.13.0-py3-none-any.whl", hash = "sha256:8a8a81bcf996e74fee46f0d16bd3eaa382a7eb20fd82445c3ad11f4090334116"},
-    {file = "importlib_metadata-4.13.0.tar.gz", hash = "sha256:dd0173e8f150d6815e098fd354f6414b0f079af4644ddfe90c71e2fc6174346d"},
+    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
+    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
 zipp = ">=0.5"
 
 [package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 perf = ["ipython"]
-testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
 name = "iniconfig"
-version = "1.1.1"
-description = "iniconfig: brain-dead simple config-ini parsing"
-category = "dev"
+version = "2.0.0"
+description = "brain-dead simple config-ini parsing"
 optional = false
-python-versions = "*"
+python-versions = ">=3.7"
 files = [
-    {file = "iniconfig-1.1.1-py2.py3-none-any.whl", hash = "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3"},
-    {file = "iniconfig-1.1.1.tar.gz", hash = "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"},
+    {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
+    {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "maturin"
-version = "0.14.7"
+version = "1.1.0"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "maturin-0.14.7-py3-none-linux_armv6l.whl", hash = "sha256:6c8fbbe4ddc41ca6a6cbc994e51d920dc907d20e3676b3403485f07945c4067a"},
-    {file = "maturin-0.14.7-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:dbdafb191475cfe3c29789deeb5330923dae4e620776e8b84fe7fa2fc5da3047"},
-    {file = "maturin-0.14.7-py3-none-macosx_10_9_x86_64.macosx_10_9_arm64.macosx_10_9_universal2.whl", hash = "sha256:8f4602fa53f606ed39e33f0150e4d2c13ce1d75161bda31f1783c62d49f5df7d"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:799d582f25ac2fce6a2aedf28ac34e7872ddafa8f995dfae73d7f9906754269d"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:6bb39a7e696d0a916eeadb5c6bce087e1b759fb528e180a894875669d3b86bd4"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:cc90a505c359e5cb3c7b69582b0cda2a2d67943b34188537b487c9425fd5cf86"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:ee04493dda88b4eda2334238a1981ecbb517c820807b3f8c3d58832bf58a4e9f"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.musllinux_1_1_ppc64le.whl", hash = "sha256:74c547b936c074d4fb555087d0910422f86fdfafe2ec953d3ed308ef7b0d1844"},
-    {file = "maturin-0.14.7-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5ae45fca0618ea29c177aa3c3d3c6a88f6676e2d69c24e82e7a31372cf2a2ee6"},
-    {file = "maturin-0.14.7-py3-none-win32.whl", hash = "sha256:4f5aa10540a1aeffd61552e567f9967572e9070e869d5110e0f3d5f3f7f90b1a"},
-    {file = "maturin-0.14.7-py3-none-win_amd64.whl", hash = "sha256:274913158beff0a7028f235c881eb4521fa38e7547feea957d6e6a5dfe6930cd"},
-    {file = "maturin-0.14.7-py3-none-win_arm64.whl", hash = "sha256:a33a61d64161bf4ab75b32a6054e4c786779cad1370bd44c6e28e4857029390a"},
-    {file = "maturin-0.14.7.tar.gz", hash = "sha256:87a8f894e828d64bfba34c507e11da7fb50ade7de46959685d7e4ca3251c443f"},
+    {file = "maturin-1.1.0-py3-none-linux_armv6l.whl", hash = "sha256:eb04f3473b9f283eba51a5dc20dc0bab6f8741048c1bbc5e45f39cc29ad69aa6"},
+    {file = "maturin-1.1.0-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:eee3c9b2cd80adee6938ea1828882795e261a7fc6b5ebaed15003ed4d713adaa"},
+    {file = "maturin-1.1.0-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:9042ea6538529e22954c0a4eefbe55026a9eba45484423882dd8eb97854b29dd"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:4252241c196abf0ede0088e38bc3c181fe0bf073a974d6594493f3ae7232545c"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:6f63dc6f9dba2081346f0ff40019e67a72eb20af7ee4847dc21174dd3636a981"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:c0fecd5ae4f8bad703ee648873d837e3bd6eb846f48ff8607bfb0556a2010adc"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:19332aa0830f23813e461f61e4d2b7d0c6f8ec84c335040232aafea3f068ac31"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.musllinux_1_1_ppc64le.whl", hash = "sha256:3f6f1e8e970f7728c26eeb55b4c38103f2c5d830b9df4c12fd00903eef7a4114"},
+    {file = "maturin-1.1.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7a2398df2d2f5ba4970ac7f670108e7c7e2da39185caf9b9f9e67d14ae4315e2"},
+    {file = "maturin-1.1.0-py3-none-win32.whl", hash = "sha256:32e95212e6b334caf68d278bcc5137dde020a8e84095c2728d9b08d2311e5d64"},
+    {file = "maturin-1.1.0-py3-none-win_amd64.whl", hash = "sha256:47705b6c5b5ec9d883f6b4fb6ae2480a07a77aabbfbc658d6327c9d6cd74c7cf"},
+    {file = "maturin-1.1.0-py3-none-win_arm64.whl", hash = "sha256:a36efcca897b356deee56c7a3c399c595201518a892ec0f20f0f20abb3064ccb"},
+    {file = "maturin-1.1.0.tar.gz", hash = "sha256:4650aeaa8debd004b55aae7afb75248cbd4d61cd7da2dcf4ead8b22b58cecae0"},
 ]
 
 [package.dependencies]
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "mypy-extensions"
-version = "0.4.3"
-description = "Experimental type system extensions for programs checked with the mypy typechecker."
-category = "dev"
+version = "1.0.0"
+description = "Type system extensions for programs checked with the mypy type checker."
 optional = false
-python-versions = "*"
+python-versions = ">=3.5"
 files = [
-    {file = "mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
-    {file = "mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
+    {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
+    {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "nox"
-version = "2022.11.21"
+version = "2023.4.22"
 description = "Flexible test automation."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "nox-2022.11.21-py3-none-any.whl", hash = "sha256:0e41a990e290e274cb205a976c4c97ee3c5234441a8132c8c3fd9ea3c22149eb"},
-    {file = "nox-2022.11.21.tar.gz", hash = "sha256:e21c31de0711d1274ca585a2c5fde36b1aa962005ba8e9322bf5eeed16dcd684"},
+    {file = "nox-2023.4.22-py3-none-any.whl", hash = "sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891"},
+    {file = "nox-2023.4.22.tar.gz", hash = "sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f"},
 ]
 
 [package.dependencies]
-argcomplete = ">=1.9.4,<3.0"
+argcomplete = ">=1.9.4,<4.0"
 colorlog = ">=2.6.1,<7.0.0"
 importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 packaging = ">=20.9"
 typing-extensions = {version = ">=3.7.4", markers = "python_version < \"3.8\""}
 virtualenv = ">=14"
 
 [package.extras]
-tox-to-nox = ["jinja2", "tox"]
+tox-to-nox = ["jinja2", "tox (<4)"]
 
 [[package]]
 name = "packaging"
-version = "22.0"
+version = "23.1"
 description = "Core utilities for Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-22.0-py3-none-any.whl", hash = "sha256:957e2148ba0e1a3b282772e791ef1d8083648bc131c8ab0c1feba110ce1146c3"},
-    {file = "packaging-22.0.tar.gz", hash = "sha256:2198ec20bd4c017b8f9717e00f0c8714076fc2fd93816750ab48e2c41de2cfd3"},
+    {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "pathspec"
-version = "0.10.3"
+version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pathspec-0.10.3-py3-none-any.whl", hash = "sha256:3c95343af8b756205e2aba76e843ba9520a24dd84f68c22b9f93251507509dd6"},
-    {file = "pathspec-0.10.3.tar.gz", hash = "sha256:56200de4077d9d0791465aa9095a01d421861e405b5096955051deefd697d6f6"},
+    {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
+    {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "2.6.0"
+version = "3.9.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-2.6.0-py3-none-any.whl", hash = "sha256:1a89a12377800c81983db6be069ec068eee989748799b946cce2a6e80dcc54ca"},
-    {file = "platformdirs-2.6.0.tar.gz", hash = "sha256:b46ffafa316e6b83b47489d240ce17173f123a9b9c83282141c3daf26ad9ac2e"},
+    {file = "platformdirs-3.9.1-py3-none-any.whl", hash = "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"},
+    {file = "platformdirs-3.9.1.tar.gz", hash = "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421"},
 ]
 
+[package.dependencies]
+typing-extensions = {version = ">=4.6.3", markers = "python_version < \"3.8\""}
+
 [package.extras]
-docs = ["furo (>=2022.9.29)", "proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.4)"]
-test = ["appdirs (==1.4.4)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
-version = "1.0.0"
+version = "1.2.0"
 description = "plugin and hook calling mechanisms for python"
-category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
-    {file = "pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
+    {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
+    {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 
 [package.dependencies]
 importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "pytest"
-version = "7.2.0"
+version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.2.0-py3-none-any.whl", hash = "sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71"},
-    {file = "pytest-7.2.0.tar.gz", hash = "sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59"},
+    {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [package.dependencies]
-attrs = ">=19.2.0"
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 iniconfig = "*"
 packaging = "*"
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
-name = "typed-ast"
-version = "1.5.4"
-description = "a fork of Python 2 and 3 ast modules with type comment support"
-category = "dev"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe"},
-    {file = "typed_ast-1.5.4-cp310-cp310-win_amd64.whl", hash = "sha256:a9916d2bb8865f973824fb47436fa45e1ebf2efd920f2b9f99342cb7fab93f72"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:79b1e0869db7c830ba6a981d58711c88b6677506e648496b1f64ac7d15633aec"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a94d55d142c9265f4ea46fab70977a1944ecae359ae867397757d836ea5a3f47"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-win_amd64.whl", hash = "sha256:639c5f0b21776605dd6c9dbe592d5228f021404dafd377e2b7ac046b0349b1a1"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:cf4afcfac006ece570e32d6fa90ab74a17245b83dfd6655a6f68568098345ff6"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:6778e1b2f81dfc7bc58e4b259363b83d2e509a65198e85d5700dfae4c6c8ff1c"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-win_amd64.whl", hash = "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2efae9db7a8c05ad5547d522e7dbe62c83d838d3906a3716d1478b6c1d61388d"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7d5d014b7daa8b0bf2eaef684295acae12b036d79f54178b92a2b6a56f92278f"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:370788a63915e82fd6f212865a596a0fefcbb7d408bbbb13dea723d971ed8bdc"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:4e964b4ff86550a7a7d56345c7864b18f403f5bd7380edf44a3c1fb4ee7ac6c6"},
-    {file = "typed_ast-1.5.4-cp38-cp38-win_amd64.whl", hash = "sha256:683407d92dc953c8a7347119596f0b0e6c55eb98ebebd9b23437501b28dcbb8e"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4879da6c9b73443f97e731b617184a596ac1235fe91f98d279a7af36c796da35"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3e123d878ba170397916557d31c8f589951e353cc95fb7f24f6bb69adc1a8a97"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebd9d7f80ccf7a82ac5f88c521115cc55d84e35bf8b446fcd7836eb6b98929a3"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
-    {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
-    {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
-]
-
-[[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {file = "typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.17.1"
+version = "20.24.0"
 description = "Virtual Python Environment builder"
-category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "virtualenv-20.17.1-py3-none-any.whl", hash = "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4"},
-    {file = "virtualenv-20.17.1.tar.gz", hash = "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"},
+    {file = "virtualenv-20.24.0-py3-none-any.whl", hash = "sha256:18d1b37fc75cc2670625702d76849a91ebd383768b4e91382a8d51be3246049e"},
+    {file = "virtualenv-20.24.0.tar.gz", hash = "sha256:e2a7cef9da880d693b933db7654367754f14e20650dc60e8ee7385571f8593a3"},
 ]
 
 [package.dependencies]
 distlib = ">=0.3.6,<1"
-filelock = ">=3.4.1,<4"
-importlib-metadata = {version = ">=4.8.3", markers = "python_version < \"3.8\""}
-platformdirs = ">=2.4,<3"
+filelock = ">=3.12,<4"
+importlib-metadata = {version = ">=6.6", markers = "python_version < \"3.8\""}
+platformdirs = ">=3.5.1,<4"
 
 [package.extras]
-docs = ["proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-argparse (>=0.3.2)", "sphinx-rtd-theme (>=1)", "towncrier (>=22.8)"]
-testing = ["coverage (>=6.2)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=21.3)", "pytest (>=7.0.1)", "pytest-env (>=0.6.2)", "pytest-freezegun (>=0.4.2)", "pytest-mock (>=3.6.1)", "pytest-randomly (>=3.10.3)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+test = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23.1)", "pytest (>=7.3.1)", "pytest-env (>=0.8.1)", "pytest-freezer (>=0.4.6)", "pytest-mock (>=3.10)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)", "setuptools (>=67.8)", "time-machine (>=2.9)"]
 
 [[package]]
 name = "zipp"
-version = "3.11.0"
+version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "zipp-3.11.0-py3-none-any.whl", hash = "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa"},
-    {file = "zipp-3.11.0.tar.gz", hash = "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"},
+    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
+    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
 [package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
-testing = ["flake8 (<5)", "func-timeout", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.7,<3.12"
-content-hash = "5022329b6b3a56a1044b6e348e4a80be6f4eff62e9e4c6b7a6df3ce2f383062d"
+content-hash = "86eef5b819efee81add2325073aecec7757798ff564af0a1eeb62bda8297c5a6"
```

### Comparing `decancer_py-0.2.1/pyproject.toml` & `decancer_py-0.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "decancer_py"
 requires-python = ">=3.7,<3.12"
 description = "Python bindings for decancer."
 authors = [{ name = "Jonxslays" }]
 license = { file = "LICENSE" }
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
@@ -20,23 +20,23 @@
 documentation = "https://github.com/Jonxslays/decancer_py"
 
 [tool.maturin]
 strip = true
 
 [tool.poetry]
 name = "decancer_py"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["Jonxslays"]
 description = "Python bindings for decancer."
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 
 [tool.poetry.group.dev.dependencies]
-black = "~=22.12.0"
-maturin = "0.14.7"
-nox = "~=2022.11.21"
-pytest = "~=7.2.0"
+black = { version = "~=23.7.0", python = ">=3.8"}
+maturin = "~=1.1.0"
+nox = "~=2023.4.22"
+pytest = "~=7.4.0"
 
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin~=1.1.0"]
 build-backend = "maturin"
```

### Comparing `decancer_py-0.2.1/src/lib.rs` & `decancer_py-0.2.2/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -23,35 +23,35 @@
     /// Checks if this string similarly contains another string.
     #[pyo3(text_signature = "($self, other: str) -> bool")]
     fn contains(&self, other: &str) -> bool {
         self.0.contains(other)
     }
 
     fn __richcmp__(&self, other: &str, op: CompareOp) -> PyResult<bool> {
-        match op {
-            CompareOp::Eq => Ok(self.0 == other),
-            CompareOp::Ne => Ok(self.0 != other),
-            _ => Ok(false),
-        }
+        Ok(match op {
+            CompareOp::Eq => self.0 == other,
+            CompareOp::Ne => self.0 != other,
+            _ => false,
+        })
     }
 
     fn __contains__(&self, other: &str) -> PyResult<bool> {
         Ok(self.contains(other))
     }
 
     fn __bool__(&self) -> PyResult<bool> {
-        Ok(self.0.len() > 0)
+        Ok(!self.0.is_empty())
     }
 
     fn __str__(&self) -> PyResult<&str> {
         Ok(&self.0)
     }
 
     fn __repr__(&self) -> PyResult<String> {
-        Ok(format!("CuredString(\"{}\")", &self.0))
+        Ok(format!("{:?}", self.0))
     }
 }
 
 /// Parses a jank string into a less toxic lowercase string wrapped in CuredString object.
 #[pyfunction]
 #[pyo3(text_signature = "(text: str) -> CuredString")]
 pub fn parse(text: String) -> CuredString {
@@ -60,11 +60,9 @@
 
 /// The module we export to python
 #[pymodule]
 fn decancer_py(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__version__", std::env!("CARGO_PKG_VERSION"))?;
 
     m.add_class::<CuredString>()?;
-    m.add_function(wrap_pyfunction!(parse, m)?)?;
-
-    Ok(())
+    m.add_function(wrap_pyfunction!(parse, m)?)
 }
```

### Comparing `decancer_py-0.2.1/tests/test_decancer.py` & `decancer_py-0.2.2/tests/test_decancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 YEET = parse("𝔂ＥＥ𝓣")
 
 
 def test_contains() -> None:
     assert YEET.contains("ee")
     assert not YEET.contains("no")
 
-
-def est_contains_invalid_type() -> None:
-    with pytest.raises(TypeError):
-        YEET.contains(69)  # type: ignore
-
-
 def test_starts_with() -> None:
     assert YEET.starts_with("ye")
     assert not YEET.starts_with("et")
 
 
 def test_starts_with_invalid_type() -> None:
     with pytest.raises(TypeError):
```

### Comparing `decancer_py-0.2.1/Cargo.lock` & `decancer_py-0.2.2/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -18,82 +18,82 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "decancer"
-version = "1.5.2"
+version = "1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d876a8402fe9e32ebfecb37e0d63285a44793d12a4843afc5a2048f41ad5b0d0"
+checksum = "a611be39729cfd30b9c2d3e4102b05a0c640125e8477996948d4d64570cb9e2b"
 
 [[package]]
 name = "decancer_py"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "decancer",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.16.6"
@@ -151,120 +151,120 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `decancer_py-0.2.1/PKG-INFO` & `decancer_py-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: decancer_py
-Version: 0.2.1
+Version: 0.2.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 License-File: LICENSE
 Summary: Python bindings for decancer.
 Keywords: decancer,ffi,string,parsing,unicode
 Home-Page: https://github.com/Jonxslays/decancer_py
 Author: Jonxslays
 License: MIT
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/Jonxslays/decancer_py
 Project-URL: repository, https://github.com/Jonxslays/decancer_py
 Project-URL: documentation, https://github.com/Jonxslays/decancer_py
-Project-URL: homepage, https://github.com/Jonxslays/decancer_py
 
 # decancer_py
 
 Python bindings for [decancer](https://github.com/null8626/decancer).
 
 ## Installation
```

