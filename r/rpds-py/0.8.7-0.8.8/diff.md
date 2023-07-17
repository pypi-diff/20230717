# Comparing `tmp/rpds_py-0.8.7.tar.gz` & `tmp/rpds_py-0.8.8.tar.gz`

## Comparing `rpds_py-0.8.7.tar` & `rpds_py-0.8.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.7/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/release.yml
--rw-r--r--   0        0        0     5075 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.gitignore
--rw-r--r--   0        0        0     1050 2023-07-06 13:57:08.000000 rpds_py-0.8.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-06 13:57:08.000000 rpds_py-0.8.7/LICENSE
--rw-r--r--   0        0        0     1739 2023-07-06 13:57:08.000000 rpds_py-0.8.7/README.rst
--rw-r--r--   0        0        0     1043 2023-07-06 13:57:08.000000 rpds_py-0.8.7/noxfile.py
--rw-r--r--   0        0        0     1406 2023-07-06 13:57:08.000000 rpds_py-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-07-06 13:57:08.000000 rpds_py-0.8.7/rpds.pyi
--rw-r--r--   0        0        0    17578 2023-07-06 13:57:08.000000 rpds_py-0.8.7/src/lib.rs
--rw-r--r--   0        0        0       20 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/requirements.txt
--rw-r--r--   0        0        0     8653 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5098 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3533 2023-07-06 13:57:08.000000 rpds_py-0.8.7/tests/test_list.py
--rw-r--r--   0        0        0     8633 2023-07-06 13:57:08.000000 rpds_py-0.8.7/Cargo.lock
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 rpds_py-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.8/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/release.yml
+-rw-r--r--   0        0        0     5106 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-06 14:59:52.000000 rpds_py-0.8.8/LICENSE
+-rw-r--r--   0        0        0     2522 2023-07-06 14:59:52.000000 rpds_py-0.8.8/README.rst
+-rw-r--r--   0        0        0     1043 2023-07-06 14:59:52.000000 rpds_py-0.8.8/noxfile.py
+-rw-r--r--   0        0        0     1406 2023-07-06 14:59:52.000000 rpds_py-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-06 14:59:52.000000 rpds_py-0.8.8/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-06 14:59:52.000000 rpds_py-0.8.8/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_list.py
+-rw-r--r--   0        0        0     8633 2023-07-06 14:59:52.000000 rpds_py-0.8.8/Cargo.lock
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 rpds_py-0.8.8/PKG-INFO
```

### Comparing `rpds_py-0.8.7/.github/workflows/CI.yml` & `rpds_py-0.8.8/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   release:
```

### Comparing `rpds_py-0.8.7/.gitignore` & `rpds_py-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/.pre-commit-config.yaml` & `rpds_py-0.8.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/LICENSE` & `rpds_py-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/README.rst` & `rpds_py-0.8.8/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,31 @@
 
 
 Python bindings to the Rust ``rpds`` crate.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
 
+Installation
+------------
+
+The distribution on PyPI is named ``rpds.py`` (equivalently ``rpds-py``), and thus can be installed via e.g.:
+
+.. code:: sh
+
+    $ pip install rpds-py
+
+Note that if you install ``rpds-py`` from source, you will need a Rust toolchain installed, as it is a build-time dependency.
+An example of how to do so in a ``Dockerfile`` can be found `here <https://github.com/bowtie-json-schema/bowtie/blob/e77fd93598cb6e7dc1b8b1f53c00e5aa410c201a/implementations/python-jsonschema/Dockerfile#L1-L8>`_.
+
+If you believe you are on a common platform which should have wheels built (i.e. and not need to compile from source), feel free to file an issue or pull request modifying the GitHub action used here to build wheels via ``maturin``.
+
+Usage
+-----
+
 Methods in general are named similarly to their ``rpds`` counterparts (rather than ``pyrsistent``\ 's conventions, though probably a full drop-in ``pyrsistent``\ -compatible wrapper module is a good addition at some point).
 
 .. code:: python
 
     >>> from rpds import HashTrieMap, HashTrieSet, List
 
     >>> m = HashTrieMap({"foo": "bar", "baz": "quux"})
```

### Comparing `rpds_py-0.8.7/noxfile.py` & `rpds_py-0.8.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/pyproject.toml` & `rpds_py-0.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/rpds.pyi` & `rpds_py-0.8.8/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/src/lib.rs` & `rpds_py-0.8.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/tests/test_hash_trie_map.py` & `rpds_py-0.8.8/tests/test_hash_trie_map.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/tests/test_hash_trie_set.py` & `rpds_py-0.8.8/tests/test_hash_trie_set.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/tests/test_list.py` & `rpds_py-0.8.8/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.7/Cargo.lock` & `rpds_py-0.8.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
 dependencies = [
  "archery",
 ]
 
 [[package]]
 name = "rpds-py"
-version = "0.8.7"
+version = "0.8.8"
 dependencies = [
  "archery",
  "pyo3",
  "rpds",
 ]
 
 [[package]]
```

### Comparing `rpds_py-0.8.7/PKG-INFO` & `rpds_py-0.8.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.8.7
+Version: 0.8.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -46,14 +46,31 @@
 
 
 Python bindings to the Rust ``rpds`` crate.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
 
+Installation
+------------
+
+The distribution on PyPI is named ``rpds.py`` (equivalently ``rpds-py``), and thus can be installed via e.g.:
+
+.. code:: sh
+
+    $ pip install rpds-py
+
+Note that if you install ``rpds-py`` from source, you will need a Rust toolchain installed, as it is a build-time dependency.
+An example of how to do so in a ``Dockerfile`` can be found `here <https://github.com/bowtie-json-schema/bowtie/blob/e77fd93598cb6e7dc1b8b1f53c00e5aa410c201a/implementations/python-jsonschema/Dockerfile#L1-L8>`_.
+
+If you believe you are on a common platform which should have wheels built (i.e. and not need to compile from source), feel free to file an issue or pull request modifying the GitHub action used here to build wheels via ``maturin``.
+
+Usage
+-----
+
 Methods in general are named similarly to their ``rpds`` counterparts (rather than ``pyrsistent``\ 's conventions, though probably a full drop-in ``pyrsistent``\ -compatible wrapper module is a good addition at some point).
 
 .. code:: python
 
     >>> from rpds import HashTrieMap, HashTrieSet, List
 
     >>> m = HashTrieMap({"foo": "bar", "baz": "quux"})
```

