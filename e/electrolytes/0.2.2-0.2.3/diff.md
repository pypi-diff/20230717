# Comparing `tmp/electrolytes-0.2.2.tar.gz` & `tmp/electrolytes-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.2.2.tar", last modified: Mon Jul 17 03:44:31 2023, max compression
+gzip compressed data, was "electrolytes-0.2.3.tar", last modified: Mon Jul 17 05:53:39 2023, max compression
```

## Comparing `electrolytes-0.2.2.tar` & `electrolytes-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.236967 electrolytes-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-17 03:44:18.000000 electrolytes-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    45957 2023-07-17 03:44:31.232967 electrolytes-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-17 03:44:18.000000 electrolytes-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-17 03:44:18.000000 electrolytes-0.2.2/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-17 03:44:18.000000 electrolytes-0.2.2/electrolytes/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45957 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 03:44:18.000000 electrolytes-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:44:31.236967 electrolytes-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 03:44:18.000000 electrolytes-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 03:44:18.000000 electrolytes-0.2.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 03:44:18.000000 electrolytes-0.2.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.449792 electrolytes-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-17 05:53:26.000000 electrolytes-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-17 05:53:39.449792 electrolytes-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-17 05:53:26.000000 electrolytes-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/db1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-17 05:53:26.000000 electrolytes-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 05:53:39.449792 electrolytes-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 05:53:26.000000 electrolytes-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 05:53:26.000000 electrolytes-0.2.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 05:53:26.000000 electrolytes-0.2.3/tests/test_cli.py
```

### Comparing `electrolytes-0.2.2/LICENSE.txt` & `electrolytes-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.2/README.md` & `electrolytes-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # electrolytes
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 
 
 **electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
-Developed for use with the [`electroMicroTransport`](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for simulation of electromigrative separations.
+## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
+
+**electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
 
 # Installation
 
 Install with [pip](https://pip.pypa.io/en/stable/):
 
 ```bash
 $ python3 -m pip install electrolytes
 ```
 
-**electrolytes** requires Python 3.6 or later, and a relatively recent version of pip (pip may be upgraded with ```python3 -m pip install --upgrade pip```).
+**electrolytes** currently requires Python 3.7 or later, and a relatively recent version of pip (pip may be upgraded with ```python3 -m pip install --upgrade pip```).
 
 # Command-line usage
 
 Invoke the `electrolytes` command-line application to search the database, find the details of a particular component, or to add/remove user-defined components. In your terminal, run:
 
 ```bash
 $ electrolytes
@@ -34,15 +38,15 @@
 $ python3 -m electrolytes
 ```
 
 Add the `--help` flag to learn what options are available.
 
 # Python API
 
-The Python API is provided for `electroMicroTransport` case setup scripts.
+The Python API is provided for _electroMicroTransport_ case initialization scripts.
 
 ```python
 from electrolytes import database, Properties
 ```
 
 You can look up components in the `database` as you would with `dict` (with component names as keys), and also add user-defined components with the `add` method (as if `database` were a set). Components are instances of the `Constituent` class. Extra methods are also defined for `database`:
 
@@ -75,10 +79,10 @@
     def diffusivity(self) -> float: ...  # SI units
 ```
 
 # Data credits
 
 Electrolyte data taken from the Simul 6 application[^simul6] ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa[^Hirokawa].
 
-[^simul6]: GAŠ, Bohuslav; BRAVENEC, Petr. Simul 6: A fast dynamic simulator of electromigration. Electrophoresis, 2021. DOI: [10.1002/elps.202100048](https://doi.org/10.1002/elps.202100048)
+[^simul6]: GAŠ, Bohuslav; BRAVENEC, Petr. Simul 6: A fast dynamic simulator of electromigration. Electrophoresis, 2021, vol. 42, no. 12-13, pp. 1291-1299. DOI: [10.1002/elps.202100048](https://doi.org/10.1002/elps.202100048)
 
-[^Hirokawa]: HIROKAWA, Takeshi, et al. Table of isotachophoretic indices: I. Simulated qualitative and quantitative indices of 287 anionic substances in the range ph 3–10. Journal of Chromatography A, 1983, vol. 271, no 2, p. D1-D106. DOI: [10.1016/S0021-9673(00)80225-3](https://doi.org/10.1016/S0021-9673(00)80225-3)
+[^Hirokawa]: HIROKAWA, Takeshi, et al. Table of isotachophoretic indices: I. Simulated qualitative and quantitative indices of 287 anionic substances in the range ph 3–10. Journal of Chromatography A, 1983, vol. 271, no. 2, pp. D1-D106. DOI: [10.1016/S0021-9673(00)80225-3](https://doi.org/10.1016/S0021-9673(00)80225-3)
```

### Comparing `electrolytes-0.2.2/electrolytes/__init__.py` & `electrolytes-0.2.3/electrolytes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from warnings import warn
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from typer import get_app_dir
 
 _APP_NAME = "electrolytes"
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 class Constituent(BaseModel):
     model_config = ConfigDict(populate_by_name=True, validate_default=True)
 
     id: int = -1
     name: str
@@ -109,15 +109,15 @@
     data = _StoredConstituents.dump_json({"constituents": list(components.values())})
     _USER_CONSTITUENTS_FILE.parent.mkdir(parents=True, exist_ok=True)
     with _USER_CONSTITUENTS_FILE.open("wb") as f:
         f.write(data)
 
 
 def _load_default_constituents() -> Dict[str, Constituent]:
-    data = pkgutil.get_data(__name__, "data/db1.json")
+    data = pkgutil.get_data(__name__, "db1.json")
     if data is None:
         raise RuntimeError("failed to load default constituents")
 
     constituents = _StoredConstituents.validate_json(data)["constituents"]
 
     for c in constituents:
         if " " in c.name:
```

### Comparing `electrolytes-0.2.2/electrolytes/__main__.py` & `electrolytes-0.2.3/electrolytes/__main__.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.2/pyproject.toml` & `electrolytes-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "electrolytes"
 description = "Electrolyte database manager"
 readme = "README.md"
 requires-python = ">=3.7"
-license = {file = "LICENSE.txt"}
 authors = [{name = "Gabriel S. Gerlero", email = "ggerlero@cimec.unl.edu.ar"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Pydantic :: 2",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
@@ -49,12 +48,18 @@
 [project.urls]
 Homepage = "https://github.com/microfluidica/electrolytes"
 Repository = "https://github.com/microfluidica/electrolytes"
 
 [project.scripts]
 electrolytes = "electrolytes.__main__:app"
 
+[tool.setuptools]
+packages = ["electrolytes"]
+
 [tool.setuptools.dynamic]
 version = {attr = "electrolytes.__version__"}
 
+[tool.setuptools.package-data]
+electrolytes = ["*.json"]
+
 [tool.mypy]
 plugins = ["pydantic.mypy"]
```

### Comparing `electrolytes-0.2.2/tests/test_api.py` & `electrolytes-0.2.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.2/tests/test_cli.py` & `electrolytes-0.2.3/tests/test_cli.py`

 * *Files identical despite different names*

