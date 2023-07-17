# Comparing `tmp/calcipy-1.4.1.tar.gz` & `tmp/calcipy-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.4.1.tar", max compression
+gzip compressed data, was "calcipy-1.4.2.tar", max compression
```

## Comparing `calcipy-1.4.1.tar` & `calcipy-1.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.4.1/LICENSE
--rw-r--r--   0        0        0      167 2023-07-07 10:08:33.703053 calcipy-1.4.1/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.4.1/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.4.1/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.4.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.4.1/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.4.1/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.4.1/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.4.1/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.4.1/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.4.1/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.4.1/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.4.1/calcipy/file_search.py
--rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.4.1/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.4.1/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.4.1/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.4.1/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6444 2023-07-07 09:54:44.784397 calcipy-1.4.1/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1418 2023-06-23 11:18:02.014243 calcipy-1.4.1/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.4.1/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.4.1/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.4.1/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.4.1/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.4.1/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.4.1/calcipy/tasks/executable_utils.py
--rw-r--r--   0        0        0     4191 2023-06-25 19:43:32.342494 calcipy-1.4.1/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.4.1/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.4.1/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.4.1/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.4.1/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.4.1/calcipy/tasks/test.py
--rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.4.1/calcipy/tasks/types.py
--rw-r--r--   0        0        0     7709 2023-07-07 10:08:16.231213 calcipy-1.4.1/docs/README.md
--rw-r--r--   0        0        0     6579 2023-07-07 10:08:33.742868 calcipy-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    12323 1970-01-01 00:00:00.000000 calcipy-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-17 03:05:20.222178 calcipy-1.4.2/LICENSE
+-rw-r--r--   0        0        0      167 2023-07-17 03:12:27.138003 calcipy-1.4.2/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.4.2/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.4.2/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8587 2023-07-17 03:06:34.200571 calcipy-1.4.2/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6435 2023-07-17 03:06:34.200957 calcipy-1.4.2/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.4.2/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11287 2023-07-17 03:06:34.201393 calcipy-1.4.2/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.4.2/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.4.2/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.4.2/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.4.2/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.4.2/calcipy/file_search.py
+-rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.4.2/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.4.2/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.4.2/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.4.2/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6444 2023-07-07 09:54:44.784397 calcipy-1.4.2/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1418 2023-07-17 03:05:43.263677 calcipy-1.4.2/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.4.2/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.4.2/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.4.2/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.4.2/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.4.2/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.4.2/calcipy/tasks/executable_utils.py
+-rw-r--r--   0        0        0     4334 2023-07-17 03:11:20.928724 calcipy-1.4.2/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.4.2/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.4.2/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.4.2/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.4.2/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.4.2/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.4.2/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     7709 2023-07-17 03:12:34.067702 calcipy-1.4.2/docs/README.md
+-rw-r--r--   0        0        0     6578 2023-07-17 03:12:27.177423 calcipy-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    12322 1970-01-01 00:00:00.000000 calcipy-1.4.2/PKG-INFO
```

### Comparing `calcipy-1.4.1/LICENSE` & `calcipy-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/can_skip.py` & `calcipy-1.4.2/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.4.2/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from arrow import Arrow
 from beartype import beartype
 from beartype.typing import Dict, List, Optional, Union
 from bidict import bidict
 from corallium.file_helpers import LOCK
 from corallium.log import logger
 from corallium.tomllib import tomllib
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, field_serializer, validator
 from pyrate_limiter import Duration, Limiter, RequestRate
 
 from .. import can_skip  # Required for mocking can_skip.can_skip
 
 CALCIPY_CACHE = Path('.calcipy_packaging.lock')
 """Path to the packaging lock file."""
 
@@ -32,15 +32,18 @@
     version: str
     datetime: Optional[Arrow] = Field(default=None)
     latest_version: str = Field(default='')
     latest_datetime: Optional[Arrow] = Field(default=None)  # noqa: CCE001
 
     class Config:
         arbitrary_types_allowed = True
-        json_encoders = {Arrow: str}
+
+    @field_serializer('datetime', 'latest_datetime')
+    def serialize_datetime(self, value: Optional[Arrow]) -> Optional[str]:  # noqa: RBT002
+        return str(value) if value else None
 
     @validator('datetime', 'latest_datetime', pre=True)
     def date_validator(cls, value: Union[str, Arrow]) -> Arrow:  # noqa: N805,RBT002
         return arrow.get(value)
 
 
 # Configure rate-limiter
@@ -130,15 +133,15 @@
         try:
             cached_package = old_cache.get(package.name)
             cached_version = '' if cached_package is None else cached_package.version
             if package.version != cached_version:
                 updated_packages.append(asyncio.run(_get_release_date(package)))
             elif cached_package:
                 updated_packages.append(cached_package)
-        except httpx.HTTPError as exc:
+        except httpx.HTTPError as exc:  # noqa: PERF203
             logger.warning('Could not lock package', package=package, error=str(exc))
     return updated_packages
 
 
 @beartype
 def _write_cache(updated_packages: List[_HostedPythonPackage], path_pack_lock: Path = CALCIPY_CACHE) -> None:
     """Read the cached packaging information.
```

### Comparing `calcipy-1.4.1/calcipy/cli.py` & `calcipy-1.4.2/calcipy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     working_dir: Path = Field(default_factory=Path.cwd)
     """Working directory for the program to use globally."""
 
     file_args: List[Path] = Field(default_factory=list)
     """List of Paths to modify."""
 
-    verbose: PositiveInt = Field(default=0, lte=3)
+    verbose: PositiveInt = Field(default=0, le=3)
     """Verbosity level."""
 
     keep_going: bool = False
     """Continue task execution regardless of failure."""
 
 
 class _CalcipyProgram(Program):
```

### Comparing `calcipy-1.4.1/calcipy/code_tag_collector/_collector.py` & `calcipy-1.4.2/calcipy/code_tag_collector/_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     """
     matches = []
     for path_source in paths_source:
         lines = []
         try:
             lines = read_lines(path_source)
-        except UnicodeDecodeError as err:
+        except UnicodeDecodeError as err:  # noqa: PERF203
             logger.text_debug('Could not parse', path_source=path_source, err=err)
 
         if comments := _search_lines(lines, regex_compiled):
             matches.append(_Tags(path_source=path_source, code_tags=comments))
 
     return matches
```

### Comparing `calcipy-1.4.1/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.4.2/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.4.2/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/file_search.py` & `calcipy-1.4.2/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/invoke_helpers.py` & `calcipy-1.4.2/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/md_writer/_writer.py` & `calcipy-1.4.2/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/noxfile/_noxfile.py` & `calcipy-1.4.2/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/scripts.py` & `calcipy-1.4.2/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/all_tasks.py` & `calcipy-1.4.2/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/cl.py` & `calcipy-1.4.2/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/defaults.py` & `calcipy-1.4.2/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/doc.py` & `calcipy-1.4.2/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/executable_utils.py` & `calcipy-1.4.2/calcipy/tasks/executable_utils.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/lint.py` & `calcipy-1.4.2/calcipy/tasks/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         '--config=r/contrib',
         '--config=r/fingerprints',
         '--config=r/generic',
         '--config=r/json',
         '--config=r/python',
         '--config=r/terraform',
         '--config=r/yaml',
+        '--exclude-rule=yaml.github-actions.security.third-party-action-not-pinned-to-commit-sha.third-party-action-not-pinned-to-commit-sha',
     ])
     logger.text('Note: Selectively override semgrep with "# nosem"', is_header=True)
     run(ctx, f'{python_dir()}/semgrep ci --autofix {semgrep_configs}')
 
 
 # ==============================================================================
 # Pre-Commit
```

### Comparing `calcipy-1.4.1/calcipy/tasks/pack.py` & `calcipy-1.4.2/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/stale.py` & `calcipy-1.4.2/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/tags.py` & `calcipy-1.4.2/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/test.py` & `calcipy-1.4.2/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/calcipy/tasks/types.py` & `calcipy-1.4.2/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/docs/README.md` & `calcipy-1.4.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.1/pyproject.toml` & `calcipy-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.4.1"
+version = "1.4.2"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,25 +26,25 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.4.1"
+version = "1.4.2"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # lint
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
 bidict = {optional = true, version = ">=0.22.1"} # stale
 commitizen = {optional = true, version = ">=2.42.0"} # doc
-corallium = ">=0.2.2"
+corallium = ">=0.3.0"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
 flake8-adjustable-complexity = {optional = true, version = ">=0.0.6"} # flake8
 flake8-annotations-complexity = {optional = true, version = ">=0.0.7"} # flake8
 flake8-executable = {optional = true, version = ">=2.1.3"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-functions = {optional = true, version = ">=0.0.7"} # flake8
@@ -71,15 +71,15 @@
 mkdocs-material = {optional = true, version = ">=8.2.16"} # doc
 mkdocs-section-index = {optional = true, version = ">=0.3.4"} # doc
 mkdocstrings = {extras = ["python"], optional = true, version = ">=0.21.1"} # doc
 mypy = {optional = true, version = ">=1.0.0"} # types
 nox-poetry = {optional = true, version = ">=1.0.2"} # test
 pandas = {optional = true, version = ">=1.5.3"} # docs,tags
 pip-check = {optional = true, version = ">=2.8.1"} # lint
-pydantic = ">=1.10.5"
+pydantic = ">=2.0.2"
 pylint = {optional = true, version = ">=2.16.2"} # doc,pylint
 pymdown-extensions = {optional = true, version = ">=10.0.1"} # docs
 pyrate_limiter = {optional = true, version = ">=2.4"} # stale
 pytest = {optional = true, version = ">=7.2.1"} # test
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
```

### Comparing `calcipy-1.4.1/PKG-INFO` & `calcipy-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -32,15 +32,15 @@
 Provides-Extra: types
 Requires-Dist: arrow (>=1.2.3) ; extra == "stale" or extra == "tags"
 Requires-Dist: autopep8 (>=2.0.1) ; extra == "lint"
 Requires-Dist: bandit (>=1.7.4) ; extra == "lint"
 Requires-Dist: beartype (>=0.12.0)
 Requires-Dist: bidict (>=0.22.1) ; extra == "stale"
 Requires-Dist: commitizen (>=2.42.0) ; extra == "doc"
-Requires-Dist: corallium (>=0.2.2)
+Requires-Dist: corallium (>=0.3.0)
 Requires-Dist: dlint (>=0.14.0) ; extra == "flake8"
 Requires-Dist: flake8 (>=6.0.0) ; extra == "flake8"
 Requires-Dist: flake8-adjustable-complexity (>=0.0.6) ; extra == "flake8"
 Requires-Dist: flake8-annotations-complexity (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-executable (>=2.1.3) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-functions (>=0.0.7) ; extra == "flake8"
@@ -67,15 +67,15 @@
 Requires-Dist: mkdocs-material (>=8.2.16) ; extra == "doc"
 Requires-Dist: mkdocs-section-index (>=0.3.4) ; extra == "doc"
 Requires-Dist: mkdocstrings[python] (>=0.21.1) ; extra == "doc"
 Requires-Dist: mypy (>=1.0.0) ; extra == "types"
 Requires-Dist: nox-poetry (>=1.0.2) ; extra == "nox"
 Requires-Dist: pandas (>=1.5.3) ; extra == "doc" or extra == "tags"
 Requires-Dist: pip-check (>=2.8.1) ; extra == "lint"
-Requires-Dist: pydantic (>=1.10.5)
+Requires-Dist: pydantic (>=2.0.2)
 Requires-Dist: pylint (>=2.16.2) ; extra == "doc" or extra == "pylint"
 Requires-Dist: pymdown-extensions (>=10.0.1) ; extra == "doc"
 Requires-Dist: pyrate_limiter (>=2.4) ; extra == "stale"
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
```

