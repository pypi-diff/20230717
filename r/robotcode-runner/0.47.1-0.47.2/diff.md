# Comparing `tmp/robotcode_runner-0.47.1.tar.gz` & `tmp/robotcode_runner-0.47.2.tar.gz`

## Comparing `robotcode_runner-0.47.1.tar` & `robotcode_runner-0.47.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    23760 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.47.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    23850 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/PKG-INFO
```

### Comparing `robotcode_runner-0.47.1/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.47.2/src/robotcode/runner/cli/libdoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
         return super().main(arguments, **options)
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
-
-
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see the `libdoc` help.',
```

### Comparing `robotcode_runner-0.47.1/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.47.2/src/robotcode/runner/cli/rebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
         return super().main(arguments, **options)
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
-
-
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `rebot` help.',
```

### Comparing `robotcode_runner-0.47.1/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.47.2/src/robotcode/runner/cli/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 f"Would execute robot with the following options and arguments:\n"
                 f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
+# mypy: disable-error-code="arg-type"
 
 ROBOT_OPTIONS: Set[click.Command] = {
     click.option("--by-longname", type=str, multiple=True, help="Select tests/tasks or suites by longname."),
     click.option(
         "--exclude-by-longname",
         type=str,
         multiple=True,
```

### Comparing `robotcode_runner-0.47.1/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.47.2/src/robotcode/runner/cli/testdoc.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
         return super().main(arguments, **options)
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
-
-
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `testdoc` help.',
```

### Comparing `robotcode_runner-0.47.1/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,17 +277,14 @@
 
         self.tests.append(item)
         self._current.children.append(item)
 
         self.statistics.tests += 1
 
 
-# mypy: disable-error-code="misc, arg-type, attr-defined"
-
-
 @click.group(invoke_without_command=False)
 @click.option(
     "--read-from-stdin", is_flag=True, help="Read file contents from stdin. This is an internal option.", hidden=True
 )
 @pass_application
 def discover(app: Application, read_from_stdin: bool) -> None:
     """\
@@ -428,15 +425,15 @@
     except DataError as err:
         LOGGER.error(err)
         app.exit(DATA_ERROR)
 
     raise UnknownError("Unexpected error happened.")
 
 
-@discover.command(
+@discover.command(  # type: ignore[attr-defined]
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -488,15 +485,15 @@
 
             app.echo_via_pager(print(collector.all.children[0]))
 
         else:
             app.print_data(ResultItem([collector.all], diagnostics), remove_defaults=True)
 
 
-@discover.command(
+@discover.command(  # type: ignore[attr-defined]
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -535,15 +532,15 @@
             if collector.tests:
                 app.echo_via_pager(print(collector.tests))
 
         else:
             app.print_data(ResultItem(collector.tests, diagnostics), remove_defaults=True)
 
 
-@discover.command(
+@discover.command(  # type: ignore[attr-defined]
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -587,15 +584,15 @@
 
 
 @dataclass
 class TagsResult:
     tags: Dict[str, List[TestItem]]
 
 
-@discover.command(
+@discover.command(  # type: ignore[attr-defined]
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -669,15 +666,15 @@
     machine: str
     processor: str
     platform: str
     system: str
     system_version: str
 
 
-@discover.command(
+@discover.command(  # type: ignore[attr-defined]
     add_help_option=True,
 )
 @pass_application
 def info(
     app: Application,
 ) -> None:
     """\
```

### Comparing `robotcode_runner-0.47.1/.gitignore` & `robotcode_runner-0.47.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.1/LICENSE.txt` & `robotcode_runner-0.47.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.1/README.md` & `robotcode_runner-0.47.2/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.1/pyproject.toml` & `robotcode_runner-0.47.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.47.1",
-  "robotcode-modifiers==0.47.1",
-  "robotcode==0.47.1",
+  "robotcode-robot==0.47.2",
+  "robotcode-modifiers==0.47.2",
+  "robotcode==0.47.2",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.47.1/PKG-INFO` & `robotcode_runner-0.47.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.47.1
+Version: 0.47.2
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.47.1
-Requires-Dist: robotcode-robot==0.47.1
-Requires-Dist: robotcode==0.47.1
+Requires-Dist: robotcode-modifiers==0.47.2
+Requires-Dist: robotcode-robot==0.47.2
+Requires-Dist: robotcode==0.47.2
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

