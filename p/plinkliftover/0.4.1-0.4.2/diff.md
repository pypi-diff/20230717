# Comparing `tmp/plinkliftover-0.4.1.tar.gz` & `tmp/plinkliftover-0.4.2.tar.gz`

## Comparing `plinkliftover-0.4.1.tar` & `plinkliftover-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.dockerignore
--rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.editorconfig
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.flake8
--rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     2346 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CHANGELOG.md
--rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/Makefile
--rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/SECURITY.md
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/cookiecutter-config-file.yml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/renovate.json
--rwxr-xr-x   0        0        0     1265 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/setup.cfg
--rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/.stale.yml
--rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/dependabot.yml
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/release-drafter.yml
--rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/config.yml
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/greetings.yml
--rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/release-drafter.yml
--rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.vscode/launch.json
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/docker/Dockerfile
--rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/docker/README.md
--rwxr-xr-x   0        0        0     1292 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/__init__.py
--rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/__main__.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/bed2map.py
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/liftover.py
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/logger.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/map2bed.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/py.typed
--rwxr-xr-x   0        0        0    10552 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.gitignore
--rwxr-xr-x   0        0        0    34902 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/LICENSE.md
--rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/README.md
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.dockerignore
+-rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.editorconfig
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.flake8
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     2819 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/Makefile
+-rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/SECURITY.md
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/cookiecutter-config-file.yml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/renovate.json
+-rwxr-xr-x   0        0        0     1265 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/setup.cfg
+-rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/.stale.yml
+-rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/release-drafter.yml
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/greetings.yml
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.github/workflows/release-drafter.yml
+-rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.vscode/launch.json
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/docker/Dockerfile
+-rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/docker/README.md
+-rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/__init__.py
+-rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/__main__.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/bed2map.py
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/liftover.py
+-rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/logger.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/map2bed.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/src/plinkliftover/py.typed
+-rwxr-xr-x   0        0        0    10552 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/.gitignore
+-rwxr-xr-x   0        0        0    34902 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/LICENSE.md
+-rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/README.md
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 plinkliftover-0.4.2/PKG-INFO
```

### Comparing `plinkliftover-0.4.1/.pre-commit-config.yaml` & `plinkliftover-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/CHANGELOG.md` & `plinkliftover-0.4.2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+** [0.4.2] - 2023-07-17
+
+*** Fix
+
+- Minimum python version
+- running `plinkliftover` with no arguments now shows the help
+
+
+** [0.4.1]
+
+*** Added
+
+- Updated gitignore
+
+
 ## [0.4.0] - 2023-07-13
 
 ### Change
 
 - Update dependencies
 - Adjust functions to use updated `typer` syntax
 - Increase required python version to 3.10
@@ -77,14 +92,18 @@
 
 ## [0.1.6] - 2021-02-22
 
 ### Fixed
 
 - replace `set` and `tuple` in type hints with their `typing.Set` and `typing.Tuple` counterparts
 
+[0.4.2]: https://github.com/milescsmith/PLINKLiftOver/compare/0.4.1...0.4.2
+[0.4.1]: https://github.com/milescsmith/PLINKLiftOver/compare/0.4.0...0.4.1
+[0.4.0]: https://github.com/milescsmith/PLINKLiftOver/compare/0.3.0...0.4.0
+[0.3.0]: https://github.com/milescsmith/PLINKLiftOver/compare/0.2.0...0.3.0
 [0.2.0]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.11...0.2.0
 [0.1.11]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.10...0.1.11
 [0.1.10]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.9...0.1.10
 [0.1.9]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.8...0.1.9
 [0.1.8]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.7...0.1.8
 [0.1.7]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.6...0.1.7
 [0.1.6]: https://github.com/milescsmith/PLINKLiftOver/compare/0.1.6...0.1.6
```

### Comparing `plinkliftover-0.4.1/CODE_OF_CONDUCT.md` & `plinkliftover-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/CONTRIBUTING.md` & `plinkliftover-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/Makefile` & `plinkliftover-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/SECURITY.md` & `plinkliftover-0.4.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/setup.cfg` & `plinkliftover-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/.stale.yml` & `plinkliftover-0.4.2/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/PULL_REQUEST_TEMPLATE.md` & `plinkliftover-0.4.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/dependabot.yml` & `plinkliftover-0.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/release-drafter.yml` & `plinkliftover-0.4.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `plinkliftover-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.github/workflows/build.yml` & `plinkliftover-0.4.2/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     strategy:
       matrix:
         python-version: ["3.10"]
 
     steps:
     - uses: actions/checkout@v3.3.0
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install poetry
       run: make download-poetry
 
     - name: Set up cache
```

### Comparing `plinkliftover-0.4.1/.github/workflows/greetings.yml` & `plinkliftover-0.4.2/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.vscode/launch.json` & `plinkliftover-0.4.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/docker/Dockerfile` & `plinkliftover-0.4.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/docker/README.md` & `plinkliftover-0.4.2/docker/README.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/src/plinkliftover/__init__.py` & `plinkliftover-0.4.2/src/plinkliftover/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 console = Console()
 logger.disable("readcounts")
 
 app = typer.Typer(
     name="plinkliftover",
     help="Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver",
     add_completion=False,
+    no_args_is_help=True
 )
 
 verbosity_level = 0
 
 
 def version_callback(value: bool) -> None:  # noqa FBT001
     """Prints the version of the package."""
```

### Comparing `plinkliftover-0.4.1/src/plinkliftover/__main__.py` & `plinkliftover-0.4.2/src/plinkliftover/__main__.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/src/plinkliftover/bed2map.py` & `plinkliftover-0.4.2/src/plinkliftover/bed2map.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/src/plinkliftover/liftover.py` & `plinkliftover-0.4.2/src/plinkliftover/liftover.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/src/plinkliftover/logger.py` & `plinkliftover-0.4.2/src/plinkliftover/logger.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/src/plinkliftover/map2bed.py` & `plinkliftover-0.4.2/src/plinkliftover/map2bed.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/.gitignore` & `plinkliftover-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/LICENSE.md` & `plinkliftover-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/README.md` & `plinkliftover-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.4.1/pyproject.toml` & `plinkliftover-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "plinkliftover"
-version = "0.4.1"
+version = "0.4.2"
 description = "Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver"
 readme = "README.md"
 keywords = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+requires-python = ">=3.10"
 dependencies = [
     "psutil ==5.9.5",
     "rich ==13.4.2",
     "typer ==0.9.0",
     "loguru ==0.7.0",
 ]
```

### Comparing `plinkliftover-0.4.1/PKG-INFO` & `plinkliftover-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: plinkliftover
-Version: 0.4.1
+Version: 0.4.2
 Summary: Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver
 Project-URL: repository, https://github.com/milescsmith/plinkliftover
 Project-URL: homepage, https://github.com/milescsmith/plinkliftover
 Author-email: Miles Smith <miles-smith@omrf.org>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
 Requires-Dist: loguru==0.7.0
 Requires-Dist: psutil==5.9.5
 Requires-Dist: rich==13.4.2
 Requires-Dist: typer==0.9.0
 Provides-Extra: dev
 Requires-Dist: bandit==1.7.5; extra == 'dev'
 Requires-Dist: black==23.7.0; extra == 'dev'
```

