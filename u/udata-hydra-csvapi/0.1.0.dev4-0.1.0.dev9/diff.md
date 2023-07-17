# Comparing `tmp/udata_hydra_csvapi-0.1.0.dev4.tar.gz` & `tmp/udata_hydra_csvapi-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udata_hydra_csvapi-0.1.0.dev4.tar", max compression
+gzip compressed data, was "udata_hydra_csvapi-0.1.0.dev9.tar", max compression
```

## Comparing `udata_hydra_csvapi-0.1.0.dev4.tar` & `udata_hydra_csvapi-0.1.0.dev9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2758 2023-02-12 18:21:04.000000 udata_hydra_csvapi-0.1.0.dev4/README.md
--rw-r--r--   0        0        0      590 2023-02-12 18:21:56.607411 udata_hydra_csvapi-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     1064 2023-02-12 18:21:04.000000 udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/__init__.py
--rw-r--r--   0        0        0     2318 2023-02-12 18:21:04.000000 udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/app.py
--rw-r--r--   0        0        0       37 2023-02-12 18:21:04.000000 udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/config_default.toml
--rw-r--r--   0        0        0     1181 2023-02-12 18:21:04.000000 udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/query.py
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 udata_hydra_csvapi-0.1.0.dev4/setup.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 udata_hydra_csvapi-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     2758 2023-02-12 19:02:59.000000 udata_hydra_csvapi-0.1.0.dev9/README.md
+-rw-r--r--   0        0        0      590 2023-02-12 19:03:28.304486 udata_hydra_csvapi-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1064 2023-02-12 19:02:59.000000 udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/__init__.py
+-rw-r--r--   0        0        0     2318 2023-02-12 19:02:59.000000 udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/app.py
+-rw-r--r--   0        0        0       37 2023-02-12 19:02:59.000000 udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/config_default.toml
+-rw-r--r--   0        0        0     1181 2023-02-12 19:02:59.000000 udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/query.py
+-rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 udata_hydra_csvapi-0.1.0.dev9/setup.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 udata_hydra_csvapi-0.1.0.dev9/PKG-INFO
```

### Comparing `udata_hydra_csvapi-0.1.0.dev4/README.md` & `udata_hydra_csvapi-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `udata_hydra_csvapi-0.1.0.dev4/pyproject.toml` & `udata_hydra_csvapi-0.1.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "udata-hydra-csvapi"
-version = "0.1.0.dev4"
+version = "0.1.0.dev9"
 description = "API for CSV converted by udata-hydra"
 authors = ["Etalab <opendatateam@data.gouv.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "udata_hydra_csvapi"}]
 
 [tool.poetry.dependencies]
```

### Comparing `udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/__init__.py` & `udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/__init__.py`

 * *Files identical despite different names*

### Comparing `udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/app.py` & `udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/app.py`

 * *Files identical despite different names*

### Comparing `udata_hydra_csvapi-0.1.0.dev4/udata_hydra_csvapi/query.py` & `udata_hydra_csvapi-0.1.0.dev9/udata_hydra_csvapi/query.py`

 * *Files identical despite different names*

### Comparing `udata_hydra_csvapi-0.1.0.dev4/setup.py` & `udata_hydra_csvapi-0.1.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0', 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'udata-hydra-csvapi',
-    'version': '0.1.0.dev4',
+    'version': '0.1.0.dev9',
     'description': 'API for CSV converted by udata-hydra',
     'long_description': '# udata-hydra-csvapi\n\nThis connects to [udata-hydra](https://github.com/etalab/udata-hydra) and serves the converted CSVs as an API.\n\n## Run locally\n\nStart [udata-hydra](https://github.com/etalab/udata-hydra) via `docker compose`.\n\nLaunch this project:\n\n```shell\ndocker compose up\n```\n\nYou can now access the raw postgrest API on http://localhost:8080.\n\nNow you can launch the proxy (ie the app):\n\n```\npoetry install\npoetry run adev runserver -p8005 udata_hydra_csvapi/app.py\n```\n\nAnd query postgrest via the proxy using a `resource_id`, cf below.\n\n## API\n\n### Meta informations on resource\n\n```shell\ncurl http://localhost:8005/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/\n```\n\n```json\n{\n  "created_at": "2023-02-11T11:44:03.875615+00:00",\n  "url": "https://data.toulouse-metropole.fr//explore/dataset/boulodromes/download?format=csv&timezone=Europe/Berlin&use_labels_for_header=false",\n  "links": [\n    {\n      "href": "/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/profile/",\n      "type": "GET",\n      "rel": "profile"\n    },\n    {\n      "href": "/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/data/",\n      "type": "GET",\n      "rel": "data"\n    }\n  ]\n}\n```\n\n### Profile (csv-detective output) for a resource\n\n```shell\ncurl http://localhost:8005/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/profile/\n```\n\n```json\n{\n  "profile": {\n    "header": [\n        "geo_point_2d",\n        "geo_shape",\n        "ins_nom",\n        "ins_complexe_nom_cplmt",\n        "ins_codepostal",\n        "secteur",\n        "..."\n    ]\n  },\n  "...": "..."\n}\n```\n\n### Data for a resource (ie resource API)\n\n```shell\ncurl http://localhost:8005/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/data/?limit=1\n```\n\n```json\n[\n  {\n    "__id": 1,\n    "geo_point_2d": "43.58061543292057,1.401751073689455",\n    "geo_shape": {\n      "coordinates": [\n        [\n          1.401751073689455,\n          43.58061543292057\n        ]\n      ],\n      "type": "MultiPoint"\n    },\n    "ins_nom": "BOULODROME LOU BOSC",\n    "ins_complexe_nom_cplmt": "COMPLEXE SPORTIF DU MIRAIL",\n    "ins_codepostal": 31100,\n    "secteur": "Toulouse Ouest",\n    "quartier": 6.3,\n    "acces_libre": null,\n    "ins_nb_equ": 1,\n    "ins_detail_equ": "",\n    "ins_complexe_nom": "",\n    "ins_adresse": "",\n    "ins_commune": "",\n    "acces_public_horaires": null,\n    "acces_club_scol": null,\n    "ins_nom_cplmt": "",\n    "ins_id_install": ""\n  }\n]\n```\n\nOn this endpoint you can use every neat stuff postgrest provides. Here we only want the `ins_nom` column where it icontains "maurice":\n\n```shell\ncurl "http://localhost:8005/api/resources/60963939-6ada-46bc-9a29-b288b16d969b/data/?select=ins_nom&ins_nom=ilike.*maurice*"\n```\n\n```json\n[\n  {\n    "ins_nom": "BOULODROME MAURICE BECANNE"\n  }\n]\n```\n',
     'author': 'Etalab',
     'author_email': 'opendatateam@data.gouv.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `udata_hydra_csvapi-0.1.0.dev4/PKG-INFO` & `udata_hydra_csvapi-0.1.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-hydra-csvapi
-Version: 0.1.0.dev4
+Version: 0.1.0.dev9
 Summary: API for CSV converted by udata-hydra
 License: MIT
 Author: Etalab
 Author-email: opendatateam@data.gouv.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

