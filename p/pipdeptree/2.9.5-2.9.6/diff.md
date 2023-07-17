# Comparing `tmp/pipdeptree-2.9.5.tar.gz` & `tmp/pipdeptree-2.9.6.tar.gz`

## Comparing `pipdeptree-2.9.5.tar` & `pipdeptree-2.9.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/CHANGES.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tox.ini
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/release.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/workflows/check.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/workflows/release.yml
--rw-r--r--   0        0        0    43408 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/version.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    42899 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/LICENSE
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/README.md
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/pyproject.toml
--rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/CHANGES.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/tox.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/release.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0    43359 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/src/pipdeptree/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    42906 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/LICENSE
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/README.md
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 pipdeptree-2.9.6/PKG-INFO
```

### Comparing `pipdeptree-2.9.5/.pre-commit-config.yaml` & `pipdeptree-2.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/CHANGES.md` & `pipdeptree-2.9.6/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/tox.ini` & `pipdeptree-2.9.6/tox.ini`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/.github/workflows/check.yml` & `pipdeptree-2.9.6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/.github/workflows/release.yml` & `pipdeptree-2.9.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/src/pipdeptree/__init__.py` & `pipdeptree-2.9.6/src/pipdeptree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 from collections import defaultdict, deque
 from importlib import import_module
 from itertools import chain
 from pathlib import Path
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Iterator, List, Mapping, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Iterator, List, Mapping, cast
 
 from pip._vendor.pkg_resources import Distribution, Requirement
 
 from .version import version as __version__
 
 try:
     from pip._internal.operations.freeze import FrozenRequirement
@@ -251,18 +251,14 @@
             "key": self.key,
             "package_name": self.project_name,
             "installed_version": self.installed_version,
             "required_version": self.version_spec,
         }
 
 
-_T = TypeVar("_T")
-_V = TypeVar("_V")
-
-
 class PackageDAG(Mapping[DistPackage, List[ReqPackage]]):
     """
     Representation of Package dependencies as directed acyclic graph using a dict (Mapping) as the underlying
     datastructure.
 
     The nodes and their relationships (edges) are internally stored using a map as follows,
```

### Comparing `pipdeptree-2.9.5/tests/test_pipdeptree.py` & `pipdeptree-2.9.6/tests/test_pipdeptree.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,15 +770,15 @@
 def randomized_dag_copy(raw: PackageDAG) -> PackageDAG:
     """Returns a copy of the package tree fixture with dependencies in randomized order."""
     # Extract the dependency graph from the package tree and randomize it.
     randomized_graph = {}
     randomized_nodes = list(raw._obj.keys())  # noqa: SLF001
     random.shuffle(randomized_nodes)
     for node in randomized_nodes:
-        edges = raw._obj[node]  # noqa: SLF001
+        edges = raw._obj[node].copy()  # noqa: SLF001
         random.shuffle(edges)
         randomized_graph[node] = edges
     assert set(randomized_graph) == set(raw._obj)  # noqa: SLF001
 
     # Create a randomized package tree.
     randomized_dag = PackageDAG(randomized_graph)
     assert len(raw) == len(randomized_dag)
```

### Comparing `pipdeptree-2.9.5/LICENSE` & `pipdeptree-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/README.md` & `pipdeptree-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/pyproject.toml` & `pipdeptree-2.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.5/PKG-INFO` & `pipdeptree-2.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.9.5
+Version: 2.9.6
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
```

