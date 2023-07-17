# Comparing `tmp/lowatt-grdf-2.1.2.tar.gz` & `tmp/lowatt-grdf-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lowatt-grdf-2.1.2.tar", last modified: Wed Mar  1 08:54:43 2023, max compression
+gzip compressed data, was "dist/lowatt-grdf-2.1.3.tar", last modified: Mon Jul 17 09:48:16 2023, max compression
```

## Comparing `lowatt-grdf-2.1.2.tar` & `lowatt-grdf-2.1.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/lowatt_grdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/lowatt_grdf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/lowatt_grdf/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/lowatt_grdf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/lowatt_grdf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/lowatt_grdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:43.000000 lowatt-grdf-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-01 08:54:37.000000 lowatt-grdf-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/lowatt_grdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/lowatt_grdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/lowatt_grdf/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/lowatt_grdf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/lowatt_grdf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/lowatt_grdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:16.000000 lowatt-grdf-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 09:48:09.000000 lowatt-grdf-2.1.3/tox.ini
```

### Comparing `lowatt-grdf-2.1.2/.github/workflows/tox.yml` & `lowatt-grdf-2.1.3/.github/workflows/tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       - uses: actions/checkout@v2
       - name: Find python version
         id: py_ver
         shell: python
         if: ${{ contains(matrix.tox_env, 'py') }}
         run: |
           v = '${{ matrix.tox_env }}'.split('-')[0].lstrip('py')
-          print('::set-output name=version::{0}.{1}'.format(v[0],v[1:]))
+          print('::set-output name=version::{}.{}'.format(v[0],v[1:]))
       - name: Install a default Python
         uses: actions/setup-python@v2
         if: ${{ ! contains(matrix.tox_env, 'py') }}
       - name: Set up Python version
         uses: actions/setup-python@v2
         if: ${{ contains(matrix.tox_env, 'py') }}
         with:
```

### Comparing `lowatt-grdf-2.1.2/LICENSE` & `lowatt-grdf-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lowatt-grdf-2.1.2/PKG-INFO` & `lowatt-grdf-2.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-grdf
-Version: 2.1.2
+Version: 2.1.3
 Summary: Client for the GRDF ADICT API
 Home-page: https://github.com/lowatt/lowatt-grdf
 Author: Lowatt
 Author-email: info@lowatt.fr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lowatt-grdf-2.1.2/README.md` & `lowatt-grdf-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lowatt-grdf-2.1.2/lowatt_grdf/__init__.py` & `lowatt-grdf-2.1.3/lowatt_grdf/__init__.py`

 * *Files identical despite different names*

### Comparing `lowatt-grdf-2.1.2/lowatt_grdf/api.py` & `lowatt-grdf-2.1.3/lowatt_grdf/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,27 +39,14 @@
             data = resp.json()
         except requests.exceptions.JSONDecodeError:
             data = resp.text
         LOGGER.error(data)
         raise
 
 
-def parse_grdf_bool(data: dict[str, Any]) -> dict[str, Any]:
-    """Turn 'Vrai' and 'Faux' items from input dict into regular booleans
-
-    >>> parse_grdf_bool({"foo": "Vrai", "bar": "Faux"})
-    {'foo': True, 'bar': False}
-    """
-    data = dict(data)
-    for key, value in data.items():
-        if isinstance(value, str) and value.lower() in ("vrai", "faux"):
-            data[key] = True if value.lower() == "vrai" else False
-    return data
-
-
 class BaseAPI(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def scope(self) -> str:
         raise NotImplementedError()
 
     @property
@@ -161,15 +148,15 @@
             items = resp[0]["liste_acces"]
         else:
             items = resp
         droits: dict[str, list[models.Access]] = {}
         for item in items:
             if "code_statut_traitement" in item:
                 continue
-            access = models.Access(**parse_grdf_bool(item))
+            access = models.converter.structure(item, models.Access)
             droits.setdefault(access.pce, []).append(access)
         errors = []
         for _, accesses in sorted(
             droits.items(), key=lambda x: (x[1][0].courriel_titulaire, x[0])
         ):
             for access in accesses:
                 if not access.check_consent():
@@ -180,15 +167,15 @@
             else:
                 for access in accesses:
                     access.is_active(log=True)
         if errors:
             raise RuntimeError(f"Theses consents have validation issues: {errors!r}")
 
     def declare_acces(self, access: models.DeclareAccess) -> None:
-        data = access.json(exclude={"pce"}, exclude_none=True)
+        data = models.converter.dumps(access)
         self.put(
             f"{self.api}/pce/{access.pce}/droit_acces",
             headers={"Content-Type": "application/json"},
             data=data,
         )
         LOGGER.info("Successfully declared access to %s", access.pce)
```

### Comparing `lowatt-grdf-2.1.2/lowatt_grdf/main.py` & `lowatt-grdf-2.1.3/lowatt_grdf/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import logging
 import os
 import sys
-from typing import Any, Callable, Type
+from typing import Any, Callable, Union
 
+import attrs
 import click
-import pydantic
 import requests
 import rich
 
 from . import LOGGER, api, models
 
 Callback = Callable[..., None]
 
@@ -52,31 +52,30 @@
         is_flag=True,
         help="Use staging (bac à sable) environment",
     )(func)
     return func
 
 
 def options_from_model(
-    model: Type[pydantic.BaseModel],
+    model: Any,
 ) -> Callable[[Callback], Callback]:
     def decorator(func: Callback) -> Callback:
-        for field in reversed(list(model.__fields__.values())):
+        for field in reversed(attrs.fields(model)):
             opt = field.alias.replace("_", "-")
             opt = f"--{opt}"
-            kwargs = {
-                "required": field.required,
-                "default": field.default,
-            }
-            if field.field_info.description is not None:
-                kwargs["help"] = field.field_info.description
-            if field.type_ == bool:
+            kwargs: dict[str, Union[str, bool]] = {}
+            if field.default == attrs.NOTHING:
+                kwargs["required"] = True
+            else:
+                kwargs.update(required=False, default=field.default)
+            if field.type == bool:
                 kwargs["is_flag"] = True
             if field.alias.startswith("date_"):
                 kwargs["metavar"] = "YYYY-MM-DD"
-            click.option(opt, **kwargs)(func)
+            click.option(opt, **kwargs)(func)  # type: ignore[arg-type]
         return func
 
     return decorator
 
 
 class ExceptionHandler(click.Group):
     def __call__(self, *args: Any, **kwargs: Any) -> None:
```

### Comparing `lowatt-grdf-2.1.2/lowatt_grdf/models.py` & `lowatt-grdf-2.1.3/lowatt_grdf/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,106 +14,81 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import json
 import time
 from typing import Any, Optional
 
-import pydantic
+import attrs
+import cattrs
+import cattrs.gen
+import cattrs.preconf.json
 
 from . import LOGGER
 
 
-def grdf_json_dumps(v: dict[str, Any], *, default: Any) -> Any:
-    for key, value in v.items():
-        if isinstance(value, bool):
-            v[key] = "Vrai" if value else "Faux"
-    return json.dumps(v, default=default)
+def validate_date_format(
+    instance: Any, attribute: "attrs.Attribute[str]", value: Any
+) -> None:
+    assert isinstance(value, str), type(value)
+    try:
+        time.strptime(value, "%Y-%m-%d")
+    except ValueError as exc:
+        raise ValueError(
+            f"format of {attribute} must be 'YYYY-MM-DD', got {value}"
+        ) from exc
+
 
+class BaseModel:
+    pass
 
-class DeclareAccess(pydantic.BaseModel):
+
+@attrs.frozen
+class DeclareAccess(BaseModel):
     pce: str
-    role_tiers: str = "AUTORISE_CONTRAT_FOURNITURE"
-    raison_sociale: Optional[str]
-    nom_titulaire: Optional[str]
     code_postal: str
     courriel_titulaire: str
-    date_consentement_declaree: str
+    date_consentement_declaree: str = attrs.field(validator=validate_date_format)
+    date_debut_droit_acces: str = attrs.field(validator=validate_date_format)
+    date_fin_droit_acces: str = attrs.field(validator=validate_date_format)
+    perim_donnees_conso_debut: str = attrs.field(validator=validate_date_format)
+    perim_donnees_conso_fin: str = attrs.field(validator=validate_date_format)
+    raison_sociale: Optional[str] = None
+    nom_titulaire: Optional[str] = None
+    role_tiers: str = "AUTORISE_CONTRAT_FOURNITURE"
     numero_telephone_titulaire: Optional[str] = None
-    date_debut_droit_acces: str
-    date_fin_droit_acces: str
-    perim_donnees_conso_debut: str
-    perim_donnees_conso_fin: str
     perim_donnees_contractuelles: bool = False
     perim_donnees_techniques: bool = False
     perim_donnees_informatives: bool = False
     perim_donnees_publiees: bool = False
 
-    class Config:
-        json_dumps = grdf_json_dumps
-        extra = "forbid"
-
-    @pydantic.root_validator()
-    def check_oneof_nom_or_raison_sociale(
-        cls,  # noqa: B902 (Invalid first argument 'cls' used for instance method.)
-        values: dict[str, str],
-    ) -> dict[str, str]:
-        if not any(values.get(k) for k in ("raison_sociale", "nom_titulaire")):
-            raise ValueError(
-                "One of raison-sociale or nom-titulaire should be specified"
-            )
-        return values
-
-    @pydantic.root_validator()
-    def check_date_format(
-        cls,  # noqa: B902 (Invalid first argument 'cls' used for instance method.)
-        values: dict[str, str],
-    ) -> dict[str, str]:
-        for param in [
-            "date_consentement_declaree",
-            "date_debut_droit_acces",
-            "date_fin_droit_acces",
-            "perim_donnees_conso_debut",
-            "perim_donnees_conso_fin",
-        ]:
-            _validate_date_format(param, values[param])
-        # Expect a datetime while it seems more consistent to use a simple date.
-        values["date_consentement_declaree"] += " 00:00:00"
-        return values
+    def __attrs_post_init__(self) -> None:
+        if not self.raison_sociale and not self.nom_titulaire:
+            raise ValueError("One of raison-sociale or nom-titulaire must be specified")
 
 
-def _validate_date_format(param: str, value: str) -> None:
-    assert isinstance(value, str), type(value)
-    try:
-        time.strptime(value, "%Y-%m-%d")
-    except ValueError as exc:
-        raise ValueError(
-            f"format of {param} must be 'YYYY-MM-DD', got {value}"
-        ) from exc
-
-
-class Access(pydantic.BaseModel):
-    pce: str = pydantic.Field(alias="id_pce")
+@attrs.frozen
+class Access(BaseModel):
+    pce: str
     etat_droit_acces: str
     perim_donnees_publiees: bool
     perim_donnees_informatives: bool
     courriel_titulaire: str
     raison_sociale_du_titulaire: Optional[str]
     nom_titulaire: Optional[str]
     statut_controle_preuve: Optional[str]
-    date_consentement_declaree: Optional[str] = None
-    numero_telephone_titulaire: Optional[str] = None
     date_debut_droit_acces: str
     date_fin_droit_acces: str
     perim_donnees_conso_debut: str
     perim_donnees_conso_fin: str
+    date_consentement_declaree: Optional[str] = None
+    numero_telephone_titulaire: Optional[str] = None
     perim_donnees_contractuelles: bool = False
     perim_donnees_techniques: bool = False
 
     def __str__(self) -> str:
         name = self.raison_sociale_du_titulaire or self.nom_titulaire
         return f"<PCE {self.pce} from {name} ({self.courriel_titulaire})>"
 
@@ -143,7 +118,54 @@
             LOGGER.error(
                 "statut_controle_preuve of %s is %r",
                 self,
                 self.statut_controle_preuve,
             )
             return False
         return True
+
+
+def structure_grdf_bool(value: Any, type_: Any) -> bool:
+    if not isinstance(value, str):
+        raise ValueError(f"Unhandled type {type(value)} for {value!r}")
+    if value.lower() == "vrai":
+        return True
+    if value.lower() == "faux":
+        return False
+    else:
+        raise ValueError(f"Unhandled value {value!r}")
+
+
+def unstructure_grdf_bool(value: bool) -> str:
+    return "Vrai" if value else "Faux"
+
+
+converter = cattrs.preconf.json.make_converter()
+converter.register_structure_hook(
+    Access,
+    cattrs.gen.make_dict_structure_fn(
+        Access,
+        cattrs.global_converter,
+        pce=cattrs.gen.override(rename="id_pce"),
+        **{
+            f.name: cattrs.gen.override(struct_hook=structure_grdf_bool)
+            for f in attrs.fields(Access)
+            if f.type == bool
+        },
+    ),
+)
+converter.register_unstructure_hook(
+    DeclareAccess,
+    cattrs.gen.make_dict_unstructure_fn(
+        DeclareAccess,
+        converter,
+        pce=cattrs.gen.override(omit=True),
+        date_consentement_declaree=cattrs.gen.override(
+            unstruct_hook=lambda v: v + " 00:00:00"
+        ),
+        **{
+            f.name: cattrs.gen.override(unstruct_hook=unstructure_grdf_bool)
+            for f in attrs.fields(Access)
+            if f.type == bool
+        },
+    ),
+)
```

### Comparing `lowatt-grdf-2.1.2/lowatt_grdf.egg-info/PKG-INFO` & `lowatt-grdf-2.1.3/lowatt_grdf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-grdf
-Version: 2.1.2
+Version: 2.1.3
 Summary: Client for the GRDF ADICT API
 Home-page: https://github.com/lowatt/lowatt-grdf
 Author: Lowatt
 Author-email: info@lowatt.fr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lowatt-grdf-2.1.2/setup.cfg` & `lowatt-grdf-2.1.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 [options]
 setup_requires = 
 	setuptools_scm
 python_requires = >=3.9
 packages = find:
 include_package_data = True
 install_requires = 
+	attrs
+	cattrs
 	click
 	ndjson
-	pydantic
 	requests
 	rich
 zip_safe = False
 
 [options.packages.find]
 exclude = 
 	tests
```

### Comparing `lowatt-grdf-2.1.2/setup.py` & `lowatt-grdf-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `lowatt-grdf-2.1.2/tests/test_api.py` & `lowatt-grdf-2.1.3/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
+import json
 import logging
 
 import ndjson
 import pytest
 import responses
 
 from lowatt_grdf import api, models
@@ -350,14 +351,18 @@
     )
     assert (
         grdf.donnees_consos_publiees(
             "23000000000000", from_date="2021-01-01", to_date="2021-01-23"
         )
         == payload
     )
+    assert (
+        responses.calls[-1].request.url
+        == "https://api.grdf.fr/adict/v2/pce/23000000000000/donnees_consos_publiees?date_debut=2021-01-01&date_fin=2021-01-23"
+    )
 
 
 @responses.activate
 def test_donnees_consos_informatives(grdf: api.API) -> None:
     payload = [
         {
             "pce": {"id_pce": "23000000000000"},
@@ -408,14 +413,18 @@
     )
     assert (
         grdf.donnees_consos_informatives(
             "23000000000000", from_date="2021-08-16", to_date="2021-08-17"
         )
         == payload
     )
+    assert (
+        responses.calls[-1].request.url
+        == "https://api.grdf.fr/adict/v2/pce/23000000000000/donnees_consos_informatives?date_debut=2021-08-16&date_fin=2021-08-17"
+    )
 
 
 @responses.activate
 def test_declare_acces(grdf: api.API, caplog: pytest.LogCaptureFixture) -> None:
     access = models.DeclareAccess(
         pce="23000000000000",
         nom_titulaire="jdoe",
@@ -429,10 +438,27 @@
         raison_sociale="dummy",
         date_consentement_declaree="2020-01-01",
     )
     # XXX: use a real life response
     responses.add(responses.PUT, f"{grdf.api}/pce/23000000000000/droit_acces", json={})
     with caplog.at_level(logging.INFO, logger="lowatt.grdf"):
         grdf.declare_acces(access)
+    assert json.loads(responses.calls[-1].request.body) == {
+        "code_postal": "99099",
+        "courriel_titulaire": "jdoe@example.com",
+        "date_consentement_declaree": "2020-01-01 00:00:00",
+        "date_debut_droit_acces": "2020-01-01",
+        "date_fin_droit_acces": "2025-12-31",
+        "nom_titulaire": "jdoe",
+        "numero_telephone_titulaire": "0600000000",
+        "perim_donnees_conso_debut": "2020-01-01",
+        "perim_donnees_conso_fin": "2020-01-01",
+        "perim_donnees_contractuelles": "Faux",
+        "perim_donnees_informatives": "Faux",
+        "perim_donnees_publiees": "Faux",
+        "perim_donnees_techniques": "Faux",
+        "raison_sociale": "dummy",
+        "role_tiers": "AUTORISE_CONTRAT_FOURNITURE",
+    }
     assert [r.message for r in caplog.records] == [
         "Successfully declared access to 23000000000000",
     ]
```

### Comparing `lowatt-grdf-2.1.2/tests/test_main.py` & `lowatt-grdf-2.1.3/tests/test_main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,29 +57,29 @@
         == """Usage: main declare-acces [OPTIONS]
 
 Options:
   --bas                           Use staging (bac à sable) environment
   --client-secret TEXT            openid client secret  [required]
   --client-id TEXT                openid client id  [required]
   --pce TEXT                      [required]
-  --role-tiers TEXT
-  --raison-sociale TEXT
-  --nom-titulaire TEXT
   --code-postal TEXT              [required]
   --courriel-titulaire TEXT       [required]
   --date-consentement-declaree YYYY-MM-DD
                                   [required]
-  --numero-telephone-titulaire TEXT
   --date-debut-droit-acces YYYY-MM-DD
                                   [required]
   --date-fin-droit-acces YYYY-MM-DD
                                   [required]
   --perim-donnees-conso-debut TEXT
                                   [required]
   --perim-donnees-conso-fin TEXT  [required]
+  --raison-sociale TEXT
+  --nom-titulaire TEXT
+  --role-tiers TEXT
+  --numero-telephone-titulaire TEXT
   --perim-donnees-contractuelles
   --perim-donnees-techniques
   --perim-donnees-informatives
   --perim-donnees-publiees
   -h, --help                      Show this message and exit.
 """
     )
```

