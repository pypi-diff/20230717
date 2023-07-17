# Comparing `tmp/adafruit-circuitpython-portalbase-1.9.3.tar.gz` & `tmp/adafruit-circuitpython-portalbase-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-portalbase-1.9.3.tar", last modified: Tue Oct  5 20:24:11 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-portalbase-1.9.4.tar", last modified: Mon Nov 15 18:59:12 2021, max compression
```

## Comparing `adafruit-circuitpython-portalbase-1.9.3.tar` & `adafruit-circuitpython-portalbase-1.9.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.120016 adafruit-circuitpython-portalbase-1.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.120016 adafruit-circuitpython-portalbase-1.9.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.120016 adafruit-circuitpython-portalbase-1.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16240 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-10-05 20:24:10.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      977 2021-10-05 20:24:10.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 20:24:10.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-10-05 20:24:10.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-10-05 20:24:10.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/
--rw-r--r--   0 runner    (1001) docker     (121)    17226 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)    22672 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/wifi_coprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/wifi_esp32s2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5644 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-05 20:24:11.124016 adafruit-circuitpython-portalbase-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-10-05 20:23:57.000000 adafruit-circuitpython-portalbase-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.606430 adafruit-circuitpython-portalbase-1.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.594430 adafruit-circuitpython-portalbase-1.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.598430 adafruit-circuitpython-portalbase-1.9.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.598430 adafruit-circuitpython-portalbase-1.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16260 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.602430 adafruit-circuitpython-portalbase-1.9.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3349 2021-11-15 18:59:12.606430 adafruit-circuitpython-portalbase-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.602430 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3349 2021-11-15 18:59:12.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-11-15 18:59:12.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:59:12.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-11-15 18:59:12.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-15 18:59:12.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.602430 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/
+-rw-r--r--   0 runner    (1001) docker     (121)    17270 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5889 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22714 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/wifi_coprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/wifi_esp32s2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.602430 adafruit-circuitpython-portalbase-1.9.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:59:12.606430 adafruit-circuitpython-portalbase-1.9.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5644 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:59:12.606430 adafruit-circuitpython-portalbase-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-11-15 18:58:57.000000 adafruit-circuitpython-portalbase-1.9.4/setup.py
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-portalbase-1.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/.github/workflows/build.yml` & `adafruit-circuitpython-portalbase-1.9.4/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,17 @@
       with:
         repository: adafruit/actions-ci-circuitpython-libs
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
-    - name: Pip install pylint, Sphinx, pre-commit
+    - name: Pip install Sphinx, pre-commit
       run: |
-        pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit
+        pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/.github/workflows/release.yml` & `adafruit-circuitpython-portalbase-1.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/.pre-commit-config.yaml` & `adafruit-circuitpython-portalbase-1.9.4/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.3.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+    rev: v2.11.1
     hooks:
     -   id: pylint
         name: pylint (library code)
         types: [python]
-        exclude: "^(docs/|examples/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+        args:
+          - --disable=consider-using-f-string,duplicate-code
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
+    -   id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name,consider-using-f-string $example; done)']
-        language: system
+        types: [python]
+        files: "^examples/"
+        args:
+        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+    -   id: pylint
+        name: pylint (test code)
+        description: Run pylint rules on "tests/*.py" files
+        types: [python]
+        files: "^tests/"
+        args:
+        - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/.pylintrc` & `adafruit-circuitpython-portalbase-1.9.4/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=12
+min-similarity-lines=4
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-portalbase-1.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/LICENSE` & `adafruit-circuitpython-portalbase-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-portalbase-1.9.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/LICENSES/MIT.txt` & `adafruit-circuitpython-portalbase-1.9.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-portalbase-1.9.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/PKG-INFO` & `adafruit-circuitpython-portalbase-1.9.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-portalbase
-Version: 1.9.3
+Version: 1.9.4
 Summary: Base Library for the Portal-style libraries.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PortalBase
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython portalbase PyPortal MatrixPortal MagTag Portal base
 Platform: UNKNOWN
@@ -73,14 +73,19 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .env
     source .env/bin/activate
     pip3 install adafruit-circuitpython-portalbase
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/portalbase/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_PortalBase/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/README.rst` & `adafruit-circuitpython-portalbase-1.9.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .env
     source .env/bin/activate
     pip3 install adafruit-circuitpython-portalbase
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/portalbase/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_PortalBase/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/PKG-INFO` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-portalbase
-Version: 1.9.3
+Version: 1.9.4
 Summary: Base Library for the Portal-style libraries.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PortalBase
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython portalbase PyPortal MatrixPortal MagTag Portal base
 Platform: UNKNOWN
@@ -73,14 +73,19 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .env
     source .env/bin/activate
     pip3 install adafruit-circuitpython-portalbase
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/portalbase/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_PortalBase/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_circuitpython_portalbase.egg-info/SOURCES.txt` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_circuitpython_portalbase.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 pyproject.toml
 requirements.txt
 setup.py
@@ -27,9 +27,10 @@
 adafruit_portalbase/wifi_coprocessor.py
 adafruit_portalbase/wifi_esp32s2.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/__init__.py` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
             return values[0]
         return values
 
     def _fill_text_labels(self, values):
         # fill out all the text blocks
         if self._text:
             value_index = 0  # In case values and text is not the same
-            for i in range(len(self._text)):
+            for i in range(len(self._text)):  # pylint: disable=consider-using-enumerate
                 if (not self._text[i]["is_data"]) or (value_index > (len(values) - 1)):
                     continue
                 string = None
                 if self._text[i]["transform"]:
                     func = self._text[i]["transform"]
                     string = func(values[value_index])
                 else:
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/graphics.py` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
             position = (0, 0)  # default in top corner
 
         if not file_or_color:
             return  # we're done, no background desired
         if self._bg_file:
             self._bg_file.close()
         if isinstance(file_or_color, str):  # its a filenme:
-            self._bg_file = open(file_or_color, "rb")
-            background = displayio.OnDiskBitmap(self._bg_file)
+            with open(file_or_color, "rb") as self._bg_file:
+                background = displayio.OnDiskBitmap(self._bg_file)
             self._bg_sprite = displayio.TileGrid(
                 background,
                 pixel_shader=getattr(
                     background, "pixel_shader", displayio.ColorConverter()
                 ),
                 # TODO: Once CP6 is no longer supported, replace the above line with below
                 # pixel_shader=background.pixel_shader,
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/network.py` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,30 +286,29 @@
         if "content-length" in headers:
             content_length = int(headers["content-length"])
         else:
             raise RuntimeError("Content-Length missing from headers")
         remaining = content_length
         print("Saving data to ", filename)
         stamp = time.monotonic()
-        file = open(filename, "wb")
-        for i in response.iter_content(min(remaining, chunk_size)):  # huge chunks!
-            self.neo_status(STATUS_DOWNLOADING)
-            remaining -= len(i)
-            file.write(i)
-            if self._debug:
-                print(
-                    "Read %d bytes, %d remaining"
-                    % (content_length - remaining, remaining)
-                )
-            else:
-                print(".", end="")
-            if not remaining:
-                break
-            self.neo_status(STATUS_FETCHING)
-        file.close()
+        with open(filename, "wb") as file:
+            for i in response.iter_content(min(remaining, chunk_size)):  # huge chunks!
+                self.neo_status(STATUS_DOWNLOADING)
+                remaining -= len(i)
+                file.write(i)
+                if self._debug:
+                    print(
+                        "Read %d bytes, %d remaining"
+                        % (content_length - remaining, remaining)
+                    )
+                else:
+                    print(".", end="")
+                if not remaining:
+                    break
+                self.neo_status(STATUS_FETCHING)
 
         response.close()
         stamp = time.monotonic() - stamp
         print(
             "Created file of %d bytes in %0.1f seconds" % (os.stat(filename)[6], stamp)
         )
         self.neo_status(STATUS_OFF)
```

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/wifi_coprocessor.py` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/wifi_coprocessor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/adafruit_portalbase/wifi_esp32s2.py` & `adafruit-circuitpython-portalbase-1.9.4/adafruit_portalbase/wifi_esp32s2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/docs/_static/favicon.ico` & `adafruit-circuitpython-portalbase-1.9.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/docs/conf.py` & `adafruit-circuitpython-portalbase-1.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/docs/index.rst` & `adafruit-circuitpython-portalbase-1.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/requirements.txt` & `adafruit-circuitpython-portalbase-1.9.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-portalbase-1.9.3/setup.py` & `adafruit-circuitpython-portalbase-1.9.4/setup.py`

 * *Files identical despite different names*

