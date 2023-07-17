# Comparing `tmp/renkon-0.0.1.tar.gz` & `tmp/renkon-0.0.2.tar.gz`

## Comparing `renkon-0.0.1.tar` & `renkon-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,67 @@
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 renkon-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 renkon-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/1225e6dc6665bd76
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/24e4f3306f58915c
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/414f08e2ce2eb05f
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/43c75c27da25d38c
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/45830c16ca16c846
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/49162ebc47082fe9
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/4afb152263521118
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/4b44f7d6401e53f8
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/638fe78d4035d833
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/6dbf28747a60c29d
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/7013ceb7c56bd36e
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/71aa3be4ba56902d
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/734ca0838ec411ee
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/79f9b72d7672697d
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/7ee889019fcc2064
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/8336512dc0aec3c0
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/8b35e5f972a5c08e
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/95fd4589656370
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/a10edea17fbb562b
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/b1a626d037a5b0c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/b683cb70caae369b
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/e10c3fa5c2e36dae
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/e67db3bdff51f696
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/ea35371720a933cb
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/f417c530b9067139
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 renkon-0.0.1/.ruff_cache/content/f5b6b6946a1e9207
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 renkon-0.0.1/scripts/generate_coverage_summary.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 renkon-0.0.1/scripts/write_coverage_summary_report.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/__about__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/__main__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/py.typed
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/infer/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/infer/inference.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/infer/type.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/__init__.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/datastore.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/queries.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/registry.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/store.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/store/store.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/task/__init__.py
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/task/graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/task/misc.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/task/result.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/task/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/util/__init__.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/util/dag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/src/renkon/web/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/test_store.py
--rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/cars.csv
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/cereals-corrupt.csv
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/cereals.csv
--rw-r--r--   0        0        0    64856 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/factbook.csv
--rw-r--r--   0        0        0   159714 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/films.csv
--rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/gini.csv
--rw-r--r--   0        0        0    55507 2020-02-02 00:00:00.000000 renkon-0.0.1/tests/samples/smallwikipedia.csv
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 renkon-0.0.1/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 renkon-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 renkon-0.0.1/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 renkon-0.0.1/hatch.toml
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 renkon-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 renkon-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 renkon-0.0.2/TODO.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 renkon-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 renkon-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/cars.csv
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/cereals-corrupt.csv
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/cereals.csv
+-rw-r--r--   0        0        0    64856 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/factbook.csv
+-rw-r--r--   0        0        0   159714 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/films.csv
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/gini.csv
+-rw-r--r--   0        0        0    55507 2020-02-02 00:00:00.000000 renkon-0.0.2/etc/samples/smallwikipedia.csv
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 renkon-0.0.2/notebooks/RelativeEntropy.ipynb
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 renkon-0.0.2/scripts/generate_coverage_summary.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 renkon-0.0.2/scripts/write_coverage_summary_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/dummy.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/__init__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/__main__.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/cli.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/client.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/py.typed
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/core/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/core/derivation.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/core/inference.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/core/trait.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/info.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/queries.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/registry.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/registry.sql
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/repository.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/repo/storage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/task/__init__.py
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/task/graph.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/task/result.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/task/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/util/__init__.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/util/common.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/util/dag.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/util/ransac.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/util/stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/src/renkon/web/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/core/test_derivation.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/repo/test_registry.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/repo/test_repository.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/repo/test_storage.py
+-rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/cars.csv
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/cereals-corrupt.csv
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/cereals.csv
+-rw-r--r--   0        0        0    64856 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/factbook.csv
+-rw-r--r--   0        0        0   159714 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/films.csv
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/gini.csv
+-rw-r--r--   0        0        0    55507 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/samples/smallwikipedia.csv
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/task/test_graph.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/task/test_result.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/task/test_task.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 renkon-0.0.2/tests/util/test_dag.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 renkon-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 renkon-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 renkon-0.0.2/README.md
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 renkon-0.0.2/hatch.toml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 renkon-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 renkon-0.0.2/PKG-INFO
```

### Comparing `renkon-0.0.1/.github/workflows/publish.yml` & `renkon-0.0.2/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Publish Python Package
+name: publish
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
```

### Comparing `renkon-0.0.1/.github/workflows/test.yml` & `renkon-0.0.2/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Tests
+name: test
 
 on:
   push:
     branches: [ main, master ]
   pull_request:
     branches: [ main, master ]
 
@@ -19,15 +19,15 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ '3.10', '3.11' ]
+        python-version: [ '3.11' ]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -65,15 +65,15 @@
 
       - name: Set up Python ${{ env.STABLE_PYTHON_VERSION }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ env.STABLE_PYTHON_VERSION }}
 
       - name: Install Hatch
-        run: pip install hatch
+        run: pip install --upgrade hatch
 
       - name: Download coverage data
         uses: actions/download-artifact@v3
         with:
           name: coverage-data
 
       - name: Combine coverage data
@@ -99,14 +99,15 @@
       - name: Update coverage pull request comment
         if: github.event_name == 'pull_request' && !github.event.pull_request.head.repo.fork
         uses: marocchino/sticky-pull-request-comment@v2
         with:
           path: coverage-report.md
 
 
+
   # https://github.com/marketplace/actions/alls-green#why
   check: # This job does nothing and is only used for the branch protection
     name: "Check all green"
     if: always()
 
     needs:
       - coverage
```

### Comparing `renkon-0.0.1/scripts/generate_coverage_summary.py` & `renkon-0.0.2/scripts/generate_coverage_summary.py`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/scripts/write_coverage_summary_report.py` & `renkon-0.0.2/scripts/write_coverage_summary_report.py`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/src/renkon/task/graph.py` & `renkon-0.0.2/src/renkon/task/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-import time
 from collections import defaultdict
 from collections.abc import Callable
 from functools import partial
-from multiprocessing import Event, Pool, current_process
-from pprint import pformat
-from typing import Any, Generic, TypeAlias, TypeVar
+from multiprocessing import Event, Pool
+from typing import Generic, TypeAlias, TypeVar
 
 from loguru import logger
 
 from renkon.task.result import Err, Ok, Result, Unk
 from renkon.task.task import Task
 from renkon.util.dag import DAG
 
-# Return type of the tasks.
-_RT = TypeVar("_RT")
+_T = TypeVar("_T")
 
-TaskSpec: TypeAlias = tuple[str, Callable[..., _RT], list[str]]
+TaskSpec: TypeAlias = tuple[str, Callable[..., _T], list[str]]
 
 
-class TaskGraph(Generic[_RT]):
+class TaskGraph(Generic[_T]):
     """
     Implements a task graph with dependencies using python multiprocessing,
     generic in the return type of the tasks.
 
     The idea is that you instantiate one of these per frame of data, and it
     will run all the inference tasks in parallel, respecting dependencies.
 
     There is no special support for data sharing between tasks.
     """
 
-    task_dag: DAG[Task[_RT]]
+    __slots__ = ("task_dag", "task_id_to_name", "task_id_to_result", "task_name_to_id")
+
+    task_dag: DAG[Task[_T]]
 
     task_id_to_name: dict[int, str]
-    task_id_to_result: dict[int, Result[_RT]]
+    task_id_to_result: dict[int, Result[_T]]
     task_name_to_id: dict[str, int]
 
     def __init__(self) -> None:
-        self.task_dag = DAG[Task[_RT]]()
+        self.task_dag = DAG[Task[_T]]()
         self.task_id_to_name = {}
         self.task_id_to_result = defaultdict(Unk)
         self.task_name_to_id = {}
 
-    def add_task(self, name: str, func: Callable[..., Any], dependencies: list[int]) -> int:
+    def add_task(self, name: str, func: Callable[..., _T], dependencies: list[int]) -> int:
         """
         Add a single task to the graph to be run after the dependencies.
         """
         if name in self.task_name_to_id:
             msg = f"Task {name} already exists!"
             raise ValueError(msg)
 
@@ -55,15 +54,15 @@
 
         # Store the mapping from task id to name (and back).
         self.task_id_to_name[task_id] = name
         self.task_name_to_id[name] = task_id
 
         return task_id
 
-    def add_tasks(self, specs: list[TaskSpec[_RT]]) -> dict[str, int]:
+    def add_tasks(self, specs: list[TaskSpec[_T]]) -> dict[str, int]:
         """
         Add a batch of tasks to the graph. The task names are the keys of the
         dictionary, and the values are tuples of (name, func, dependencies).
 
         Dependencies should be expressed using task names.
 
         :returns: a mapping from task names to task ids.
@@ -74,34 +73,36 @@
         for name, func, dependency_names in specs:
             dep_ids = [self.task_name_to_id[name] for name in dependency_names]
             self.add_task(name, func, dep_ids)
             task_name_to_id[name] = self.task_name_to_id[name]
 
         return task_name_to_id
 
-    def get_task(self, task_id: int) -> Task[_RT]:
+    def get_task(self, task_id: int) -> Task[_T]:
         return self.task_dag.get_node(task_id)
 
-    def get_result(self, task_id: int) -> Any:
+    def get_result(self, task_id: int) -> object:
         return self.task_id_to_result[task_id]
 
     def run(self) -> None:
         tasks_remaining = set(range(len(self.task_dag)))
         all_done = Event()
 
         logger.info("Scanning dependency tree...")
         tasks_next = {}
         for task_id in range(len(self.task_dag)):
             deps = self.task_dag.get_dependencies(task_id)
             tasks_next[task_id] = deps
             logger.info(f"{task_id} <- {deps}.")
 
+        # todo: inject pool (allow for different pool implementations)
         with Pool() as pool:
+            # pool = MultiprocessingPoolExecutor(_pool)
 
-            def on_complete(task_id: int, result: Any) -> None:
+            def on_complete(task_id: int, result: _T) -> None:
                 nonlocal tasks_remaining
 
                 # Store the result
                 self.task_id_to_result[task_id] = Ok(result)
 
                 # First, check if we're all done.
                 tasks_remaining.remove(task_id)
@@ -110,30 +111,27 @@
                     return
 
                 # Otherwise, submit the tasks that were only waiting for this one.
                 for next_task_id in self.task_dag.get_dependents(task_id):
                     s = tasks_next[next_task_id]
                     s.remove(task_id)
                     if not s:
-                        if next_task_id not in tasks_remaining:
-                            logger.warning(f"Task {next_task_id} was pruned.")
-                            continue
                         logger.info(f"All dependencies finished for {next_task_id}.")
                         submit(next_task_id)
 
             def on_error(task_id: int, error: Exception) -> None:
                 nonlocal tasks_remaining
 
-                logger.error(f"Task {task_id} failed: {error}")
+                logger.info(f"Task {task_id} failed: {error}")
                 self.task_id_to_result[task_id] = Err(error)
 
                 # Compute the set of tasks that depend on this one.
                 pruned_tasks = self.task_dag.get_descendants(task_id)
                 pruned_task_names = [self.get_task(task_id).name for task_id in pruned_tasks]
-                logger.error(f"Pruning tasks: {pruned_task_names}")
+                logger.info(f"Pruning tasks: {pruned_task_names}")
 
                 # Remove the failed task and all of its descendants.
                 tasks_remaining.remove(task_id)
                 tasks_remaining = tasks_remaining.difference(pruned_tasks)
 
                 # Then, check if we're all done.
                 if not tasks_remaining:
@@ -151,43 +149,44 @@
 
             # Kick off the tasks that have no dependencies.
             for task_id in self.task_dag.get_roots():
                 submit(task_id)
             all_done.wait()
 
 
-def dummy_task(name: str) -> int:
-    proc = current_process()
-    logger.info(f"START {name}...")
-    time.sleep(0.1)
-    logger.info(f"DONE {name}...")
-    return proc.pid if proc.pid is not None else 0
-
-
-def fail_task(name: str) -> int:
-    current_process()
-    logger.info(f"START {name}...")
-    msg = "Uh oh, SNAFU!"
-    raise RuntimeError(msg)
-
-
-if __name__ == "__main__":
-    g = TaskGraph[int]()
-
-    name_to_tid = g.add_tasks(
-        [
-            ("Task-0", dummy_task, []),
-            ("Task-1", dummy_task, ["Task-0"]),
-            ("Task-2", dummy_task, []),
-            ("Task-3", dummy_task, ["Task-1", "Task-2"]),
-            ("Task-4", fail_task, ["Task-3"]),
-            ("Task-5", dummy_task, ["Task-4"]),
-            ("Task-6", dummy_task, ["Task-1", "Task-5"]),
-        ]
-    )
-
-    logger.info("Added tasks:\n" + pformat(name_to_tid))
-    g.run()
-
-    for name in sorted(name_to_tid.keys()):
-        task_id = name_to_tid[name]
-        logger.info(f"Task {name} has result {g.get_result(task_id)}.")
+#
+# def dummy_task(name: str) -> int:
+#     proc = current_process()
+#     logger.info(f"START {name}...")
+#     time.sleep(0.1)
+#     logger.info(f"DONE {name}...")
+#     return proc.pid if proc.pid is not None else 0
+#
+#
+# def fail_task(name: str) -> int:
+#     current_process()
+#     logger.info(f"START {name}...")
+#     msg = "Uh oh, SNAFU!"
+#     raise RuntimeError(msg)
+#
+#
+# if __name__ == "__main__":
+#     g = TaskGraph[int]()
+#
+#     name_to_tid = g.add_tasks(
+#         [
+#             ("Task-0", dummy_task, []),
+#             ("Task-1", dummy_task, ["Task-0"]),
+#             ("Task-2", dummy_task, []),
+#             ("Task-3", dummy_task, ["Task-1", "Task-2"]),
+#             ("Task-4", fail_task, ["Task-3"]),
+#             ("Task-5", dummy_task, ["Task-4"]),
+#             ("Task-6", dummy_task, ["Task-1", "Task-5"]),
+#         ]
+#     )
+#
+#     logger.info("Added tasks:\n" + pformat(name_to_tid))
+#     g.run()
+#
+#     for name in sorted(name_to_tid.keys()):
+#         task_id = name_to_tid[name]
+#         logger.info(f"Task {name} has result {g.get_result(task_id)}.")
```

### Comparing `renkon-0.0.1/src/renkon/task/result.py` & `renkon-0.0.2/src/renkon/task/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from dataclasses import dataclass
 from typing import Generic, TypeAlias, TypeVar
 
 _T = TypeVar("_T")
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Ok(Generic[_T]):
     """
     Represents a successful result, carrying the value.
     """
 
     value: _T
 
     def __repr__(self) -> str:
         return f"Ok({self.value!r})"
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Err:
     """
     Represents an error result, carrying the responsible exception.
     """
 
     cause: Exception
```

### Comparing `renkon-0.0.1/tests/samples/cars.csv` & `renkon-0.0.2/etc/samples/cars.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/cereals-corrupt.csv` & `renkon-0.0.2/etc/samples/cereals-corrupt.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/cereals.csv` & `renkon-0.0.2/etc/samples/cereals.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/factbook.csv` & `renkon-0.0.2/etc/samples/factbook.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/films.csv` & `renkon-0.0.2/etc/samples/films.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/gini.csv` & `renkon-0.0.2/etc/samples/gini.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/tests/samples/smallwikipedia.csv` & `renkon-0.0.2/etc/samples/smallwikipedia.csv`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/.gitignore` & `renkon-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/LICENSE.txt` & `renkon-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `renkon-0.0.1/hatch.toml` & `renkon-0.0.2/hatch.toml`

 * *Files 5% similar despite different names*

```diff
@@ -48,62 +48,67 @@
 000002f0: 7920 3320 2d72 2061 5220 7b61 7267 733a  y 3 -r aR {args:
 00000300: 7465 7374 737d 220a 0a23 2054 6573 7420  tests}"..# Test 
 00000310: 456e 7669 726f 6e6d 656e 7420 4d61 7472  Environment Matr
 00000320: 6978 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ix.# -----------
 00000330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5b5b  ------------..[[
 00000340: 656e 7673 2e74 6573 742e 6d61 7472 6978  envs.test.matrix
 00000350: 5d5d 0a70 7974 686f 6e20 3d20 5b22 332e  ]].python = ["3.
-00000360: 3130 222c 2022 332e 3131 225d 0a0a 2320  10", "3.11"]..# 
-00000370: 436f 7665 7261 6765 2045 6e76 6972 6f6e  Coverage Environ
-00000380: 656d 6e74 0a23 202d 2d2d 2d2d 2d2d 2d2d  emnt.# ---------
-00000390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a5b 656e  -----------..[en
-000003a0: 7673 2e63 6f76 6572 6167 655d 0a64 6574  vs.coverage].det
-000003b0: 6163 6865 6420 3d20 7472 7565 0a64 6570  ached = true.dep
-000003c0: 656e 6465 6e63 6965 7320 3d20 5b0a 2020  endencies = [.  
-000003d0: 2020 2263 6f76 6572 6167 655b 746f 6d6c    "coverage[toml
-000003e0: 5d3e 3d36 2e35 222c 0a20 2020 2022 6c78  ]>=6.5",.    "lx
-000003f0: 6d6c 222c 0a5d 0a0a 5b65 6e76 732e 636f  ml",.]..[envs.co
-00000400: 7665 7261 6765 2e73 6372 6970 7473 5d0a  verage.scripts].
-00000410: 636f 6d62 696e 6520 3d20 2263 6f76 6572  combine = "cover
-00000420: 6167 6520 636f 6d62 696e 6520 7b61 7267  age combine {arg
-00000430: 737d 220a 7265 706f 7274 2d78 6d6c 203d  s}".report-xml =
-00000440: 2022 636f 7665 7261 6765 2078 6d6c 220a   "coverage xml".
-00000450: 7265 706f 7274 2d75 6e63 6f76 6572 6564  report-uncovered
-00000460: 2d68 746d 6c20 3d20 2263 6f76 6572 6167  -html = "coverag
-00000470: 6520 6874 6d6c 202d 2d73 6b69 702d 636f  e html --skip-co
-00000480: 7665 7265 6420 2d2d 736b 6970 2d65 6d70  vered --skip-emp
-00000490: 7479 220a 6765 6e65 7261 7465 2d73 756d  ty".generate-sum
-000004a0: 6d61 7279 203d 2022 7079 7468 6f6e 2073  mary = "python s
-000004b0: 6372 6970 7473 2f67 656e 6572 6174 655f  cripts/generate_
-000004c0: 636f 7665 7261 6765 5f73 756d 6d61 7279  coverage_summary
-000004d0: 2e70 7922 0a77 7269 7465 2d73 756d 6d61  .py".write-summa
-000004e0: 7279 2d72 6570 6f72 7420 3d20 2270 7974  ry-report = "pyt
-000004f0: 686f 6e20 7363 7269 7074 732f 7772 6974  hon scripts/writ
-00000500: 655f 636f 7665 7261 6765 5f73 756d 6d61  e_coverage_summa
-00000510: 7279 5f72 6570 6f72 742e 7079 220a 0a23  ry_report.py"..#
-00000520: 204c 696e 7469 6e67 2045 6e76 6972 6f6e   Linting Environ
-00000530: 6d65 6e74 0a23 202d 2d2d 2d2d 2d2d 2d2d  ment.# ---------
-00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5b65 6e76  ----------..[env
-00000550: 732e 6c69 6e74 5d0a 6465 7461 6368 6564  s.lint].detached
-00000560: 203d 2074 7275 650a 6465 7065 6e64 656e   = true.dependen
-00000570: 6369 6573 203d 205b 0a20 2020 2022 626c  cies = [.    "bl
-00000580: 6163 6b3e 3d32 332e 312e 3022 2c0a 2020  ack>=23.1.0",.  
-00000590: 2020 226d 7970 793e 3d31 2e30 2e30 222c    "mypy>=1.0.0",
-000005a0: 0a20 2020 2022 7275 6666 3e3d 302e 302e  .    "ruff>=0.0.
-000005b0: 3234 3322 2c0a 5d0a 0a5b 656e 7673 2e6c  243",.]..[envs.l
-000005c0: 696e 742e 7363 7269 7074 735d 0a74 7970  int.scripts].typ
-000005d0: 696e 6720 3d20 226d 7970 7920 2d2d 696e  ing = "mypy --in
-000005e0: 7374 616c 6c2d 7479 7065 7320 2d2d 6e6f  stall-types --no
-000005f0: 6e2d 696e 7465 7261 6374 6976 6520 7b61  n-interactive {a
-00000600: 7267 733a 7372 632f 7265 6e6b 6f6e 2074  rgs:src/renkon t
-00000610: 6573 7473 7d22 0a73 7479 6c65 203d 205b  ests}".style = [
-00000620: 0a20 2020 2022 7275 6666 207b 6172 6773  .    "ruff {args
-00000630: 3a2e 7d22 2c0a 2020 2020 2262 6c61 636b  :.}",.    "black
-00000640: 202d 2d63 6865 636b 202d 2d64 6966 6620   --check --diff 
-00000650: 7b61 7267 733a 2e7d 222c 0a5d 0a66 6d74  {args:.}",.].fmt
-00000660: 203d 205b 0a20 2020 2022 626c 6163 6b20   = [.    "black 
-00000670: 7b61 7267 733a 2e7d 222c 0a20 2020 2022  {args:.}",.    "
-00000680: 7275 6666 202d 2d66 6978 207b 6172 6773  ruff --fix {args
-00000690: 3a2e 7d22 2c0a 2020 2020 2273 7479 6c65  :.}",.    "style
-000006a0: 222c 0a5d 0a61 6c6c 203d 205b 0a20 2020  ",.].all = [.   
-000006b0: 2022 7374 796c 6522 2c0a 2020 2020 2274   "style",.    "t
-000006c0: 7970 696e 6722 2c0a 5d                   yping",.]
+00000360: 3131 225d 0a0a 2320 436f 7665 7261 6765  11"]..# Coverage
+00000370: 2045 6e76 6972 6f6e 656d 6e74 0a23 202d   Environemnt.# -
+00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000390: 2d2d 2d0a 0a5b 656e 7673 2e63 6f76 6572  ---..[envs.cover
+000003a0: 6167 655d 0a64 6574 6163 6865 6420 3d20  age].detached = 
+000003b0: 7472 7565 0a64 6570 656e 6465 6e63 6965  true.dependencie
+000003c0: 7320 3d20 5b0a 2020 2020 2263 6f76 6572  s = [.    "cover
+000003d0: 6167 655b 746f 6d6c 5d3e 3d36 2e35 222c  age[toml]>=6.5",
+000003e0: 0a20 2020 2022 6c78 6d6c 222c 0a5d 0a0a  .    "lxml",.]..
+000003f0: 5b65 6e76 732e 636f 7665 7261 6765 2e73  [envs.coverage.s
+00000400: 6372 6970 7473 5d0a 636f 6d62 696e 6520  cripts].combine 
+00000410: 3d20 2263 6f76 6572 6167 6520 636f 6d62  = "coverage comb
+00000420: 696e 6520 7b61 7267 737d 220a 7265 706f  ine {args}".repo
+00000430: 7274 2d78 6d6c 203d 2022 636f 7665 7261  rt-xml = "covera
+00000440: 6765 2078 6d6c 220a 7265 706f 7274 2d75  ge xml".report-u
+00000450: 6e63 6f76 6572 6564 2d68 746d 6c20 3d20  ncovered-html = 
+00000460: 2263 6f76 6572 6167 6520 6874 6d6c 202d  "coverage html -
+00000470: 2d73 6b69 702d 636f 7665 7265 6420 2d2d  -skip-covered --
+00000480: 736b 6970 2d65 6d70 7479 220a 6765 6e65  skip-empty".gene
+00000490: 7261 7465 2d73 756d 6d61 7279 203d 2022  rate-summary = "
+000004a0: 7079 7468 6f6e 2073 6372 6970 7473 2f67  python scripts/g
+000004b0: 656e 6572 6174 655f 636f 7665 7261 6765  enerate_coverage
+000004c0: 5f73 756d 6d61 7279 2e70 7922 0a77 7269  _summary.py".wri
+000004d0: 7465 2d73 756d 6d61 7279 2d72 6570 6f72  te-summary-repor
+000004e0: 7420 3d20 2270 7974 686f 6e20 7363 7269  t = "python scri
+000004f0: 7074 732f 7772 6974 655f 636f 7665 7261  pts/write_covera
+00000500: 6765 5f73 756d 6d61 7279 5f72 6570 6f72  ge_summary_repor
+00000510: 742e 7079 220a 0a23 204c 696e 7469 6e67  t.py"..# Linting
+00000520: 2045 6e76 6972 6f6e 6d65 6e74 0a23 202d   Environment.# -
+00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000540: 2d2d 0a0a 5b65 6e76 732e 6c69 6e74 5d0a  --..[envs.lint].
+00000550: 6465 7461 6368 6564 203d 2074 7275 650a  detached = true.
+00000560: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
+00000570: 0a20 2020 2022 626c 6163 6b3e 3d32 332e  .    "black>=23.
+00000580: 312e 3022 2c0a 2020 2020 226d 7970 793e  1.0",.    "mypy>
+00000590: 3d31 2e30 2e30 222c 0a20 2020 2022 7275  =1.0.0",.    "ru
+000005a0: 6666 3e3d 302e 302e 3234 3322 2c0a 2020  ff>=0.0.243",.  
+000005b0: 2020 2263 6c69 636b 3d3d 382e 312e 3322    "click==8.1.3"
+000005c0: 2c20 2320 666f 7220 7479 7065 730a 2020  , # for types.  
+000005d0: 2020 2264 6163 6974 6522 2c20 2320 666f    "dacite", # fo
+000005e0: 7220 7479 7065 730a 2020 2020 2270 6f6c  r types.    "pol
+000005f0: 6172 7322 2c20 2023 2066 6f72 2074 7970  ars",  # for typ
+00000600: 6573 0a5d 0a0a 5b65 6e76 732e 6c69 6e74  es.]..[envs.lint
+00000610: 2e73 6372 6970 7473 5d0a 7479 7069 6e67  .scripts].typing
+00000620: 203d 2022 6d79 7079 202d 2d69 6e73 7461   = "mypy --insta
+00000630: 6c6c 2d74 7970 6573 202d 2d6e 6f6e 2d69  ll-types --non-i
+00000640: 6e74 6572 6163 7469 7665 207b 6172 6773  nteractive {args
+00000650: 3a73 7263 2f72 656e 6b6f 6e20 7465 7374  :src/renkon test
+00000660: 737d 220a 7374 796c 6520 3d20 5b0a 2020  s}".style = [.  
+00000670: 2020 2272 7566 6620 7b61 7267 733a 2e7d    "ruff {args:.}
+00000680: 222c 0a20 2020 2022 626c 6163 6b20 2d2d  ",.    "black --
+00000690: 6368 6563 6b20 2d2d 6469 6666 207b 6172  check --diff {ar
+000006a0: 6773 3a2e 7d22 2c0a 5d0a 666d 7420 3d20  gs:.}",.].fmt = 
+000006b0: 5b0a 2020 2020 2262 6c61 636b 207b 6172  [.    "black {ar
+000006c0: 6773 3a2e 7d22 2c0a 2020 2020 2272 7566  gs:.}",.    "ruf
+000006d0: 6620 2d2d 6669 7820 7b61 7267 733a 2e7d  f --fix {args:.}
+000006e0: 222c 0a20 2020 2022 7374 796c 6522 2c0a  ",.    "style",.
+000006f0: 5d0a 616c 6c20 3d20 5b0a 2020 2020 2273  ].all = [.    "s
+00000700: 7479 6c65 222c 0a20 2020 2022 7479 7069  tyle",.    "typi
+00000710: 6e67 222c 0a5d                           ng",.]
```

### Comparing `renkon-0.0.1/pyproject.toml` & `renkon-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,86 +3,90 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "renkon"
 dynamic = ["version"]
 description = 'Robust likely invariant analysis over columnar data'
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 license = "BSD-3-Clause"
 keywords = []
 authors = [
     { name = "Dylan Lukes", email = "lukes.dylan@gmail.com" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
     "aiosql",
     "click",
+    "dacite",
     "loguru",
-    "pyarrow"
+    "pyarrow",
+    "polars",
+    "rich",
+    "toolz"
 ]
 
 [project.urls]
 Documentation = "https://github.com/DylanLukes/renkon#readme"
 Issues = "https://github.com/DylanLukes/renkon/issues"
 Source = "https://github.com/DylanLukes/renkon"
 
 [project.scripts]
-renkon = "renkon.cli:renkon"
+renkon = "renkon.cli:cli"
 
 # Tool Configurations
 # ===================
 
 # Mypy
 # ----
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 strict = true
+mypy_path = "$MYPY_CONFIG_FILE_DIR/stubs"
 
 [[tool.mypy.overrides]]
 module = [
     "aiosql.*",
     "loguru.*",
     "pyarrow.*",
-    "pytest.*"
+    "pytest.*",
+    "rich.*",
+    "toolz.*"
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disable_error_code = ["misc"]
 
 # Pytest
 # ------
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+
 
 # Black
 # -----
 
 [tool.black]
-target-version = ["py310"]
+target-version = ["py311"]
 line-length = 120
 skip-string-normalization = true
 
 # Ruff
 # ----
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py311"
 line-length = 120
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
```

