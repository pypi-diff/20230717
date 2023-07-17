# Comparing `tmp/electrolytes-0.2.1.tar.gz` & `tmp/electrolytes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.2.1.tar", last modified: Tue Jun 13 16:59:56 2023, max compression
+gzip compressed data, was "electrolytes-0.2.2.tar", last modified: Mon Jul 17 03:44:31 2023, max compression
```

## Comparing `electrolytes-0.2.1.tar` & `electrolytes-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.571194 electrolytes-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-06-13 16:59:39.000000 electrolytes-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 16:59:39.000000 electrolytes-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-13 16:59:56.571194 electrolytes-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-13 16:59:39.000000 electrolytes-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes/data/
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/data/db1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 16:59:39.000000 electrolytes-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 16:59:56.571194 electrolytes-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 16:59:39.000000 electrolytes-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.236967 electrolytes-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-17 03:44:18.000000 electrolytes-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    45957 2023-07-17 03:44:31.232967 electrolytes-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-17 03:44:18.000000 electrolytes-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-17 03:44:18.000000 electrolytes-0.2.2/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-17 03:44:18.000000 electrolytes-0.2.2/electrolytes/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45957 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 03:44:31.000000 electrolytes-0.2.2/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 03:44:18.000000 electrolytes-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:44:31.236967 electrolytes-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 03:44:18.000000 electrolytes-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:44:31.232967 electrolytes-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 03:44:18.000000 electrolytes-0.2.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 03:44:18.000000 electrolytes-0.2.2/tests/test_cli.py
```

### Comparing `electrolytes-0.2.1/LICENSE.txt` & `electrolytes-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.1/PKG-INFO` & `electrolytes-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: electrolytes
-Version: 0.2.1
-Summary: Electrolyte database manager
-Home-page: https://github.com/microfluidica/electrolytes
-Author: Gabriel S. Gerlero
-Author-email: ggerlero@cimec.unl.edu.ar
-Project-URL: Source Code, https://github.com/microfluidica/electrolytes
-Project-URL: Bug Tracker, https://github.com/microfluidica/electrolytes/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: lint
-License-File: LICENSE.txt
-
 # electrolytes
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 
@@ -101,12 +73,12 @@
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
 
 # Data credits
 
-Electrolyte data taken from the Simul 6 [1] application ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa [2].
+Electrolyte data taken from the Simul 6 application[^simul6] ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa[^Hirokawa].
 
-[1]: GAŠ, Bohuslav; BRAVENEC, Petr. Simul 6: A fast dynamic simulator of electromigration. Electrophoresis, 2021. DOI: [10.1002/elps.202100048](https://doi.org/10.1002/elps.202100048)
+[^simul6]: GAŠ, Bohuslav; BRAVENEC, Petr. Simul 6: A fast dynamic simulator of electromigration. Electrophoresis, 2021. DOI: [10.1002/elps.202100048](https://doi.org/10.1002/elps.202100048)
 
-[2]: HIROKAWA, Takeshi, et al. Table of isotachophoretic indices: I. Simulated qualitative and quantitative indices of 287 anionic substances in the range ph 3–10. Journal of Chromatography A, 1983, vol. 271, no 2, p. D1-D106. DOI: [10.1016/S0021-9673(00)80225-3](https://doi.org/10.1016/S0021-9673(00)80225-3)
+[^Hirokawa]: HIROKAWA, Takeshi, et al. Table of isotachophoretic indices: I. Simulated qualitative and quantitative indices of 287 anionic substances in the range ph 3–10. Journal of Chromatography A, 1983, vol. 271, no 2, p. D1-D106. DOI: [10.1016/S0021-9673(00)80225-3](https://doi.org/10.1016/S0021-9673(00)80225-3)
```

### Comparing `electrolytes-0.2.1/electrolytes/__init__.py` & `electrolytes-0.2.2/electrolytes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pkgutil
-import json
 from pathlib import Path
-from typing import Iterable, Iterator, List, Sequence, Dict, Optional
+from typing import Iterable, Iterator, List, Sequence, Dict
+from warnings import warn
 
-from pydantic import BaseModel, Field, validator, root_validator, parse_file_as, parse_raw_as
+from pydantic import BaseModel, ConfigDict, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from typer import get_app_dir
 
 _APP_NAME = "electrolytes"
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 class Constituent(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, validate_default=True)
+
     id: int = -1
     name: str
     u_neg: List[float] = Field([], alias="uNeg") # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     u_pos: List[float] = Field([], alias="uPos") # [+1, +2, +3, ..., +pos_count]
     pkas_neg: List[float] = Field([], alias="pKaNeg") # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     pkas_pos: List[float] = Field([], alias="pKaPos") # [+1, +2, +3, ..., +pos_count]
     neg_count: int = Field(-1, alias="negCount")
@@ -58,62 +60,68 @@
     def _default_pka(charge: int) -> float:
         assert charge != 0
         if charge < 0:
             return 14 - charge
         else:
             return -charge
 
-    class Config:
-        allow_population_by_field_name = True
-
-    @validator("pkas_neg", "pkas_pos")
-    def pka_lengths(cls, v, values, field):
-        if len(v) != len(values[f"u_{field.name[5:]}"]):
-            raise ValueError(f"len({field.name}) != len(u_{field.name[5:]})")
+    @field_validator("pkas_neg", "pkas_pos")
+    def pka_lengths(cls, v: List[float], info: FieldValidationInfo) -> List[float]:
+        if len(v) != len(info.data[f"u_{info.field_name[5:]}"]):
+            raise ValueError(f"len({info.field_name}) != len(u_{info.field_name[5:]})")
         return v
  
-    @validator("neg_count", "pos_count", always=True)
-    def counts(cls, v, values, field):
+    @field_validator("neg_count", "pos_count")
+    def counts(cls, v: int, info: FieldValidationInfo) -> int:
         if v == -1:
-            v = len(values[f"u_{field.name[:3]}"])
-        elif v != len(values[f"u_{field.name[:3]}"]):
-            raise ValueError(f"{field.name} != len(u_{field.name[:3]})")
+            v = len(info.data[f"u_{info.field_name[:3]}"])
+        elif v != len(info.data[f"u_{info.field_name[:3]}"]):
+            raise ValueError(f"{info.field_name} != len(u_{info.field_name[:3]})")
         return v
 
-    @root_validator
-    def pkas_not_increasing(cls, values):
-        pkas = [*values["pkas_neg"], *values["pkas_pos"]]
+    @model_validator(mode="after")
+    def pkas_not_increasing(self):
+        pkas = [*self.pkas_neg, *self.pkas_pos]
 
         if not all(x>=y for x, y in zip(pkas, pkas[1:])):
             raise ValueError("pKa values must not increase with charge")
 
-        return values
+        return self
+
 
+_StoredConstituents = TypeAdapter(Dict[str, List[Constituent]])
 
 _USER_CONSTITUENTS_FILE = Path(get_app_dir(_APP_NAME), "user_constituents.json")
 
 def _load_user_constituents() -> Dict[str, Constituent]:
     try:
-        constituents = parse_file_as(Dict[str, List[Constituent]], _USER_CONSTITUENTS_FILE)["constituents"]
-        return {c.name: c for c in constituents}
-    except (FileNotFoundError, json.decoder.JSONDecodeError):
+        with _USER_CONSTITUENTS_FILE.open("rb") as f:
+            data = f.read()
+    except FileNotFoundError:
+        return {}
+    try:
+        constituents = _StoredConstituents.validate_json(data)["constituents"]
+    except Exception as e:
+        warn(f"failed to load user constituents from {_USER_CONSTITUENTS_FILE}: {type(e).__name__}", RuntimeWarning)
         return {}
+    return {c.name: c for c in constituents}
 
 def _save_user_constituents(components: Dict[str, Constituent]) -> None:
+    data = _StoredConstituents.dump_json({"constituents": list(components.values())})
     _USER_CONSTITUENTS_FILE.parent.mkdir(parents=True, exist_ok=True)
-    with _USER_CONSTITUENTS_FILE.open("w") as f:
-        json.dump({"constituents": [c.dict() for c in components.values()]}, f)
+    with _USER_CONSTITUENTS_FILE.open("wb") as f:
+        f.write(data)
 
 
 def _load_default_constituents() -> Dict[str, Constituent]:
     data = pkgutil.get_data(__name__, "data/db1.json")
     if data is None:
         raise RuntimeError("failed to load default constituents")
 
-    constituents = parse_raw_as(Dict[str, List[Constituent]], data)["constituents"]
+    constituents = _StoredConstituents.validate_json(data)["constituents"]
 
     for c in constituents:
         if " " in c.name:
             c.name = c.name.replace(" ", "_")
         if "Cl-" in c.name:
             c.name = c.name.replace("Cl-", "CHLORO")
```

### Comparing `electrolytes-0.2.1/electrolytes/__main__.py` & `electrolytes-0.2.2/electrolytes/__main__.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.1/tests/test_api.py` & `electrolytes-0.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.1/tests/test_cli.py` & `electrolytes-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

