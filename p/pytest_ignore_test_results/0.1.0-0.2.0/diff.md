# Comparing `tmp/pytest_ignore_test_results-0.1.0.tar.gz` & `tmp/pytest_ignore_test_results-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ignore_test_results-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_ignore_test_results-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_ignore_test_results-0.1.0.tar` & `pytest_ignore_test_results-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
--rw-r--r--   0        0        0      438 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     1165 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/.github/workflows/test-python.yml
--rw-r--r--   0        0        0     3077 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/.gitignore
--rw-r--r--   0        0        0      818 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/LICENSE
--rw-r--r--   0        0        0       70 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/README.md
--rw-r--r--   0        0        0      101 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/license_header.txt
--rw-r--r--   0        0        0     2530 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/__init__.py
--rw-r--r--   0        0        0      352 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/hooks.py
--rw-r--r--   0        0        0     5410 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/ignore_results.py
--rw-r--r--   0        0        0     1616 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/plugin.py
--rw-r--r--   0        0        0     1692 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/utils.py
--rw-r--r--   0        0        0     1712 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      657 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/tests/fixtures/script.py
--rw-r--r--   0        0        0     2945 2023-06-28 08:59:32.471658 pytest_ignore_test_results-0.1.0/tests/test_plugin.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 pytest_ignore_test_results-0.1.0/setup.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 pytest_ignore_test_results-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      438 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1165 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/.github/workflows/test-python.yml
+-rw-r--r--   0        0        0     3077 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/.gitignore
+-rw-r--r--   0        0        0      818 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      169 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/LICENSE
+-rw-r--r--   0        0        0       70 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/README.md
+-rw-r--r--   0        0        0      634 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      454 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     1354 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      440 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      101 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/license_header.txt
+-rw-r--r--   0        0        0     2921 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/hooks.py
+-rw-r--r--   0        0        0     5478 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/ignore_results.py
+-rw-r--r--   0        0        0     1616 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/plugin.py
+-rw-r--r--   0        0        0     1726 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/utils.py
+-rw-r--r--   0        0        0     1712 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      657 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/tests/fixtures/script.py
+-rw-r--r--   0        0        0     3925 2023-07-17 10:02:52.944842 pytest_ignore_test_results-0.2.0/tests/test_plugin.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 pytest_ignore_test_results-0.2.0/setup.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 pytest_ignore_test_results-0.2.0/PKG-INFO
```

### Comparing `pytest_ignore_test_results-0.1.0/.github/workflows/test-python.yml` & `pytest_ignore_test_results-0.2.0/.github/workflows/test-python.yml`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/.gitignore` & `pytest_ignore_test_results-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/.pre-commit-config.yaml` & `pytest_ignore_test_results-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/LICENSE` & `pytest_ignore_test_results-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/pyproject.toml` & `pytest_ignore_test_results-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -25,18 +25,35 @@
     "pytest>=7.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest-cov",
 ]
+doc = [
+    "sphinx",
+    # theme
+    "sphinx-rtd-theme",
+    # extensions
+    "sphinx_copybutton",        # copy button
+    "myst-parser",              # markdown support
+    "sphinxcontrib-mermaid",    # mermaid graph support
+]
 
 [project.entry-points."pytest11"]
 pytest_ignore_test_results = "pytest_ignore_test_results.plugin"
 
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "0.2.0"
+tag_format = "v$version"
+version_files = [
+    "pytest_ignore_test_results/__init__.py",
+]
+
 [tool.isort]
 profile = 'black'
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 skip-string-normalization = true
```

### Comparing `pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/ignore_results.py` & `pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/ignore_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,43 +92,46 @@
         Note:
             Remember that this function will be called three times (setup, call, teardown) for each item.
             We only care about the call phase of the test case.
         """
         if not report.failed:
             return
 
+        main_case_name = getattr(report, 'custom_test_case_name', report.nodeid)
+        main_case_ignored = self.is_ignored_result_case(report.nodeid)
         if report.when in ['setup', 'teardown']:
             # setup and teardown failures we only record them
-            custom_test_case_name = getattr(report, 'custom_test_case_name', report.nodeid)
-            self._failed_test_cases[custom_test_case_name] = self.is_ignored_result_case(custom_test_case_name)
+            self._failed_test_cases[main_case_name] = main_case_ignored
             return
 
         child_cases = self.config.stash[ChildCasesStashKey].get(report.nodeid, [])
         if not child_cases:
             # no child cases, we use the test case itself
-            custom_test_case_name = getattr(report, 'custom_test_case_name', report.nodeid)
-            self._failed_test_cases[custom_test_case_name] = self.is_ignored_result_case(custom_test_case_name)
-            if self._failed_test_cases[custom_test_case_name]:
+            self._failed_test_cases[main_case_name] = main_case_ignored
+            if main_case_ignored:
                 return 'ignored', 'I', 'IGNORED'
         else:
             # there are child cases, we use child cases instead
-            has_failed = False
-            has_ignored = False
+            # if the main case is ignored, we ignore all child cases as well
+            failed_child_cases = []
+            ignored_child_cases = []
             for child_case in child_cases:
                 if child_case.result == 'failed':
-                    has_failed = True
-                    self._failed_test_cases[child_case.name] = self.is_ignored_result_case(child_case.name)
-                    if self._failed_test_cases[child_case.name]:
-                        has_ignored = True
-
-            if has_failed:
-                if has_ignored:
-                    return 'ignored', 'I', 'IGNORED CHILD CASES'
-                else:
-                    return 'failed', 'F', 'FAILED CHILD CASES'
+                    child_case_ignored = main_case_ignored or self.is_ignored_result_case(child_case.name)
+                    self._failed_test_cases[child_case.name] = child_case_ignored
+                    if child_case_ignored:
+                        ignored_child_cases.append(child_case.name)
+                    else:
+                        failed_child_cases.append(child_case.name)
+
+            if failed_child_cases:
+                return 'failed', 'F', 'FAILED CHILD CASES'
+
+            if ignored_child_cases:
+                return 'ignored', 'I', 'IGNORED CHILD CASES'
 
     def pytest_terminal_summary(self, terminalreporter: TerminalReporter) -> None:
         if self.ignored_result_cases:
             terminalreporter.section('Ignored Result Cases', bold=True, yellow=True)
             terminalreporter.line('\n'.join(self.ignored_result_cases))
 
     def pytest_sessionfinish(self, session):
```

### Comparing `pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/plugin.py` & `pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/pytest_ignore_test_results/utils.py` & `pytest_ignore_test_results-0.2.0/pytest_ignore_test_results/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     INTERRUPTED = 2
     #: An internal error got in the way.
     INTERNAL_ERROR = 3
     #: pytest was misused.
     USAGE_ERROR = 4
     #: pytest couldn't find tests.
     NO_TESTS_COLLECTED = 5
-    #: Only ignore result cases failed, and the
+    #: Only ignore result cases failed, and the `--strict-exit-code` flag is set.
     ONLY_IGNORE_RESULT_CASES_FAILED = 6
```

### Comparing `pytest_ignore_test_results-0.1.0/tests/conftest.py` & `pytest_ignore_test_results-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/tests/fixtures/script.py` & `pytest_ignore_test_results-0.2.0/tests/fixtures/script.py`

 * *Files identical despite different names*

### Comparing `pytest_ignore_test_results-0.1.0/tests/test_plugin.py` & `pytest_ignore_test_results-0.2.0/tests/test_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from pytest_ignore_test_results.ignore_results import ChildCase, ChildCasesStashKey
 
 def pytest_runtest_makereport(item, call):
     if call.when == 'call':
         item.config.stash[ChildCasesStashKey] = {
             item.nodeid: [
                 ChildCase('child_case_1', 'passed'),
-                ChildCase('child_case_2', 'failed')
+                ChildCase('child_case_2', 'failed'),
             ]
         }
 """
     )
 
     result = pytester.runpytest(
         '-vv',
@@ -102,7 +102,41 @@
         '-vv',
         '-k',
         'test_failed_2',
         '--ignore-result-cases',
         'child_case_2',
     )
     assert_outcomes(result.parseoutcomes(), failed=0, passed=0, skipped=0, xfailed=0, ignored=1, deselected=7)
+
+
+def test_ignore_main_case_with_child_cases(pytester):
+    pytester.makeconftest(
+        """
+from pytest_ignore_test_results.ignore_results import ChildCase, ChildCasesStashKey
+
+def pytest_runtest_makereport(item, call):
+    if call.when == 'call':
+        item.config.stash[ChildCasesStashKey] = {
+            item.nodeid: [
+                ChildCase('child_case_1', 'passed'),
+                ChildCase('child_case_2', 'failed'),
+            ]
+        }
+"""
+    )
+
+    result = pytester.runpytest(
+        '-vv',
+        '-k',
+        'test_failed_2',
+    )
+    assert result.ret == 1
+    assert_outcomes(result.parseoutcomes(), failed=1, passed=0, skipped=0, xfailed=0, ignored=0, deselected=7)
+
+    result = pytester.runpytest(
+        '-vv',
+        '-k',
+        'test_failed_2',
+        '--ignore-result-cases',
+        'test_script.py::test_failed_2',
+    )
+    assert_outcomes(result.parseoutcomes(), failed=0, passed=0, skipped=0, xfailed=0, ignored=1, deselected=7)
```

### Comparing `pytest_ignore_test_results-0.1.0/PKG-INFO` & `pytest_ignore_test_results-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: pytest_ignore_test_results
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pytest plugin to ignore test results.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Pytest
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest>=7.0
+Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx-rtd-theme ; extra == "doc"
+Requires-Dist: sphinx_copybutton ; extra == "doc"
+Requires-Dist: myst-parser ; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid ; extra == "doc"
 Requires-Dist: pytest-cov ; extra == "test"
+Provides-Extra: doc
 Provides-Extra: test
 
 # pytest-ignore-test-results
 
 A pytest plugin to ignore test results.
```

