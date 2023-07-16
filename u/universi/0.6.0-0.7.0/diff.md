# Comparing `tmp/universi-0.6.0.tar.gz` & `tmp/universi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.6.0.tar", max compression
+gzip compressed data, was "universi-0.7.0.tar", max compression
```

## Comparing `universi-0.6.0.tar` & `universi-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.6.0/LICENSE
--rw-r--r--   0        0        0    10672 2023-07-16 08:12:54.529999 universi-0.6.0/README.md
--rw-r--r--   0        0        0     4136 2023-07-16 13:59:35.396666 universi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.6.0/universi/__init__.py
--rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.6.0/universi/_utils.py
--rw-r--r--   0        0        0    22168 2023-07-16 13:24:36.323327 universi-0.6.0/universi/codegen.py
--rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.6.0/universi/exceptions.py
--rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.6.0/universi/fields.py
--rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.6.0/universi/header.py
--rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.6.0/universi/py.typed
--rw-r--r--   0        0        0    12077 2023-07-16 13:58:23.713333 universi-0.6.0/universi/routing.py
--rw-r--r--   0        0        0      426 2023-07-16 13:09:25.456661 universi-0.6.0/universi/structure/__init__.py
--rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.6.0/universi/structure/common.py
--rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.6.0/universi/structure/endpoints.py
--rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.6.0/universi/structure/enums.py
--rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.6.0/universi/structure/responses.py
--rw-r--r--   0        0        0     6058 2023-07-16 13:58:29.106666 universi-0.6.0/universi/structure/schemas.py
--rw-r--r--   0        0        0     9545 2023-07-16 13:09:26.053328 universi-0.6.0/universi/structure/versions.py
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 universi-0.6.0/setup.py
--rw-r--r--   0        0        0    11332 1970-01-01 00:00:00.000000 universi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.7.0/LICENSE
+-rw-r--r--   0        0        0    10813 2023-07-16 21:30:00.123318 universi-0.7.0/README.md
+-rw-r--r--   0        0        0     4072 2023-07-16 22:36:50.423332 universi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.7.0/universi/__init__.py
+-rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.7.0/universi/_utils.py
+-rw-r--r--   0        0        0    22168 2023-07-16 13:24:36.323327 universi-0.7.0/universi/codegen.py
+-rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.7.0/universi/exceptions.py
+-rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.7.0/universi/fields.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.7.0/universi/header.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.7.0/universi/py.typed
+-rw-r--r--   0        0        0    12077 2023-07-16 13:58:23.713333 universi-0.7.0/universi/routing.py
+-rw-r--r--   0        0        0      426 2023-07-16 13:09:25.456661 universi-0.7.0/universi/structure/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.7.0/universi/structure/common.py
+-rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.7.0/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.7.0/universi/structure/enums.py
+-rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.7.0/universi/structure/responses.py
+-rw-r--r--   0        0        0     6058 2023-07-16 13:58:29.106666 universi-0.7.0/universi/structure/schemas.py
+-rw-r--r--   0        0        0     9545 2023-07-16 13:09:26.053328 universi-0.7.0/universi/structure/versions.py
+-rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 universi-0.7.0/setup.py
+-rw-r--r--   0        0        0    11400 1970-01-01 00:00:00.000000 universi-0.7.0/PKG-INFO
```

### Comparing `universi-0.6.0/LICENSE` & `universi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/README.md` & `universi-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,28 @@
+Metadata-Version: 2.1
+Name: universi
+Version: 0.7.0
+Summary: 
+Home-page: https://github.com/ovsyanka83/universi
+License: MIT
+Author: Stanislav Zmiev
+Author-email: szmiev2000@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.96.1)
+Requires-Dist: typing-extensions
+Project-URL: Repository, https://github.com/ovsyanka83/universi
+Description-Content-Type: text/markdown
+
 # universi
 
-Modern Stripe-like API versioning for FastAPI
+Modern [Stripe-like](https://stripe.com/blog/api-versioning) API versioning for FastAPI
 
 ---
 
 <p align="center">
 <a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
@@ -28,15 +46,22 @@
 <!---
 # TODO: Note that we don't handle "from .schemas import Schema as OtherSchema" case
 # TODO: Need to validate that the user doesn't use versioned schemas instead of the latest ones
 -->
 
 ## Who is this for?
 
-Universi and its approach will be useful if you want to support many API versions for a long time and backport features and bugfixes back to all of your versions easily like Stripe does. It is made possible by moving all "versioning" logic away from your business code and encapsulating it in small "migration modules" which are then combined to create a full blown versioning infrastructure.
+Universi allows you to support a single version of your code, auto-generating the code/routes for older versions. You keep versioning encapsulated in small and independent "version change" modules while your business logic knows nothing about versioning.
+
+Its approach will be useful if you want to:
+
+1. Support many API versions for a long time
+2. Effortlessly backport features and bugfixes to all of your versions
+
+Otherwise, more conventional methods of API versioning may be preferable.
 
 ## Tutorial
 
 This guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User's address.
 
 ### A dummy setup
 
@@ -200,7 +225,8 @@
 Note that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.
 
 Obviously, this was just a simple example and universi has a lot more features so if you're interested -- take a look at the reference
 
 ## Reference
 
 TBD
+
```

### Comparing `universi-0.6.0/pyproject.toml` & `universi-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [tool.poetry]
 name = "universi"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "*"
-typer = {version="*", extras=["all"]}
 fastapi = ">=0.96.1"
-type-inspector = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ruff = "*"
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
 httpx = ">=0.23.0"
```

### Comparing `universi-0.6.0/universi/_utils.py` & `universi-0.7.0/universi/_utils.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/codegen.py` & `universi-0.7.0/universi/codegen.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/fields.py` & `universi-0.7.0/universi/fields.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/header.py` & `universi-0.7.0/universi/header.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/routing.py` & `universi-0.7.0/universi/routing.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/structure/endpoints.py` & `universi-0.7.0/universi/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/structure/enums.py` & `universi-0.7.0/universi/structure/enums.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/structure/responses.py` & `universi-0.7.0/universi/structure/responses.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/structure/schemas.py` & `universi-0.7.0/universi/structure/schemas.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/universi/structure/versions.py` & `universi-0.7.0/universi/structure/versions.py`

 * *Files identical despite different names*

### Comparing `universi-0.6.0/setup.py` & `universi-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 packages = \
 ['universi', 'universi.structure']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.96.1',
- 'type-inspector>=1.2.2,<2.0.0',
- 'typer[all]',
- 'typing-extensions']
+['fastapi>=0.96.1', 'typing-extensions']
 
 setup_kwargs = {
     'name': 'universi',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': '',
-    'long_description': '# universi\n\nModern Stripe-like API versioning for FastAPI\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n\n<!---\n# TODO: Note that we don\'t handle "from .schemas import Schema as OtherSchema" case\n# TODO: Need to validate that the user doesn\'t use versioned schemas instead of the latest ones\n-->\n\n## Who is this for?\n\nUniversi and its approach will be useful if you want to support many API versions for a long time and backport features and bugfixes back to all of your versions easily like Stripe does. It is made possible by moving all "versioning" logic away from your business code and encapsulating it in small "migration modules" which are then combined to create a full blown versioning infrastructure.\n\n## Tutorial\n\nThis guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User\'s address.\n\n### A dummy setup\n\nHere is an initial API setup where the User has a single address. We will be implementing two routes - one for creating a user and another for retrieving user details. We\'ll be using "int" for ID for simplicity.\n\nThe first API you come up with usually doesn\'t require more than one address -- why bother?\n\nSo we create our file with schemas:\n\n```python\nfrom pydantic import BaseModel\n\n\nclass UserCreateRequest(BaseModel):\n    address: str\n\nclass UserResource(BaseModel):\n    id: int\n    address: str\n```\n\nAnd we create our file with routes:\n\n```python\nfrom versions.latest.users import UserCreateRequest, UserResource\nfrom universi import VersionedAPIRouter\n\nrouter = VersionedAPIRouter()\n\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "address": payload.address,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "address": "123 Example St",\n    }\n```\n\n### Turning address into a list\n\nDuring our development, we have realized that the initial API design was wrong and that addresses should have always been a list because the user wants to have multiple addresses to choose from so now we have to change the type of the "address" field to the list of strings.\n\n```python\nfrom pydantic import BaseModel\nfrom universi import Field\n\n\nclass UserCreateRequest(BaseModel):\n    addresses: list[str] = Field(min_items=1)\n\nclass UserResource(BaseModel):\n    id: int\n    addresses: list[str]\n```\n\n```python\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "addresses": payload.addresses,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "addresses": ["123 Example St", "456 Main St"],\n    }\n\n```\n\nBut every user of ours will now have their API integration broken. To prevent that, we have to introduce API versioning. There aren\'t many methods of doing that. Most of them force you to either duplicate your schemas, your endpoints, or your entire app instance. And it makes sense, really: duplication is the only way to make sure that you will not break old versions with your new versions; the bigger the piece you duplicating -- the safer. Of course, the safest being duplicating the entire app instance and even having a separate database. But that is expensive and makes it either impossible to make breaking changes often or to support many versions. As a result, either you need infinite resources, very long development cycles, or your users will need to often migrate from version to version.\n\nStripe has come up [with a solution](https://stripe.com/blog/api-versioning): let\'s have one latest app version whose responses get migrated to older versions and let\'s describe changes between these versions using migrations. This approach allows them to keep versions for **years** without dropping them. Obviously, each breaking change is still bad and each version still makes our system more complex and expensive, but their approach gives us a chance to minimize that. Additionally, it allows us backport features and bugfixes to older versions. However, you will also be backporting bugs, which is a sad consequence of eliminating duplication.\n\nUniversi is heavily inspired by this approach so let\'s continue our tutorial and now try to combine the two versions we created using versioning.\n\n### Creating the Migration\n\nWe need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.\n\n```python\nfrom universi import Field\nfrom universi.structure import (\n    schema,\n    AbstractVersionChange,\n    convert_response_to_previous_version_for,\n)\n\nclass ChangeAddressToList(AbstractVersionChange):\n    description = (\n        "Change user address to a list of strings to "\n        "allow the user to specify multiple addresses"\n    )\n    instructions_to_migrate_to_previous_version = (\n        # You should use schema inheritance if you don\'t want to repeat yourself in such cases\n        schema(UserCreateRequest).field("addresses").didnt_exist,\n        schema(UserCreateRequest).field("address").existed_with(type=str, info=Field()),\n        schema(UserResource).field("addresses").didnt_exist,\n        schema(UserResource).field("address").existed_with(type=str, info=Field()),\n    )\n\n    @convert_response_to_previous_version_for(get_user, create_user)\n    def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:\n        data["address"] = data.pop("addresses")[0]\n    \n    @schema(UserCreateRequest).had_property("addresses")\n    def addresses_property(parsed_schema):\n        return [parsed_schema.address]\n\n```\n\ns\nSee how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn\'t, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn\'t have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.\n\nSee how we added the `addresses` property? This simple instruction will allow us to use `addresses` even from the old schema, which means that our api route will not need to know anything about versioning. The main goal of universi is to shift the logic of versioning away from your business logic and api endpoints which makes your project easier to navigate and which makes deleting versions a breeze.\n\n### Grouping Version Changes\n\nFinally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let\'s use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002\'s version.\n\n```python\nfrom universi.structure import Version, Versions\nfrom datetime import date\n\nversions = Versions(\n    Version(date(2002, 1, 1), ChangeAddressToList),\n    Version(date(2001, 1, 1)),\n)\n```\n\nThat\'s it. You\'re done with describing things. Now you just gotta ask universi to do the rest for you. We\'ll need the VersionedAPIRouter we used previously, our API versions, and the module representing the latest versions of our schemas.\n\n```python\nfrom versions import latest\nfrom universi import regenerate_dir_to_all_versions, api_version_var\n\nregenerate_dir_to_all_versions(latest, versions)\nrouter_versions = router.create_versioned_copies(\n    versions,\n    latest_schemas_module=latest,\n)\napi_version_var.set(date(2002, 1, 1))\nuvicorn.run(router_versions[date(2002, 1, 1)])\n```\n\nUniversi has generated multiple things in this code:\n\n* Three versions of our schemas: one for each API version and one that includes definitions of unions of all versions for each schema which will be useful when you want to type check that you are using requests of different versions correctly. For example, we\'ll have `UserCreateRequestUnion` defined there which is a `TypeAlias` pointing to the union of 2002 version and 2001 version of `UserCreateRequest`.\n* Two versions of our API router: one for each API version\n\nYou can now just pick a router by its version and run it separately or use a parent router/app to specify the logic by which you\'d like to pick a version. I recommend using a header-based router with version dates as headers. And yes, that\'s how Stripe does it.\n\nNote that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.\n\nObviously, this was just a simple example and universi has a lot more features so if you\'re interested -- take a look at the reference\n\n## Reference\n\nTBD\n',
+    'long_description': '# universi\n\nModern [Stripe-like](https://stripe.com/blog/api-versioning) API versioning for FastAPI\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n\n<!---\n# TODO: Note that we don\'t handle "from .schemas import Schema as OtherSchema" case\n# TODO: Need to validate that the user doesn\'t use versioned schemas instead of the latest ones\n-->\n\n## Who is this for?\n\nUniversi allows you to support a single version of your code, auto-generating the code/routes for older versions. You keep versioning encapsulated in small and independent "version change" modules while your business logic knows nothing about versioning.\n\nIts approach will be useful if you want to:\n\n1. Support many API versions for a long time\n2. Effortlessly backport features and bugfixes to all of your versions\n\nOtherwise, more conventional methods of API versioning may be preferable.\n\n## Tutorial\n\nThis guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User\'s address.\n\n### A dummy setup\n\nHere is an initial API setup where the User has a single address. We will be implementing two routes - one for creating a user and another for retrieving user details. We\'ll be using "int" for ID for simplicity.\n\nThe first API you come up with usually doesn\'t require more than one address -- why bother?\n\nSo we create our file with schemas:\n\n```python\nfrom pydantic import BaseModel\n\n\nclass UserCreateRequest(BaseModel):\n    address: str\n\nclass UserResource(BaseModel):\n    id: int\n    address: str\n```\n\nAnd we create our file with routes:\n\n```python\nfrom versions.latest.users import UserCreateRequest, UserResource\nfrom universi import VersionedAPIRouter\n\nrouter = VersionedAPIRouter()\n\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "address": payload.address,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "address": "123 Example St",\n    }\n```\n\n### Turning address into a list\n\nDuring our development, we have realized that the initial API design was wrong and that addresses should have always been a list because the user wants to have multiple addresses to choose from so now we have to change the type of the "address" field to the list of strings.\n\n```python\nfrom pydantic import BaseModel\nfrom universi import Field\n\n\nclass UserCreateRequest(BaseModel):\n    addresses: list[str] = Field(min_items=1)\n\nclass UserResource(BaseModel):\n    id: int\n    addresses: list[str]\n```\n\n```python\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "addresses": payload.addresses,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "addresses": ["123 Example St", "456 Main St"],\n    }\n\n```\n\nBut every user of ours will now have their API integration broken. To prevent that, we have to introduce API versioning. There aren\'t many methods of doing that. Most of them force you to either duplicate your schemas, your endpoints, or your entire app instance. And it makes sense, really: duplication is the only way to make sure that you will not break old versions with your new versions; the bigger the piece you duplicating -- the safer. Of course, the safest being duplicating the entire app instance and even having a separate database. But that is expensive and makes it either impossible to make breaking changes often or to support many versions. As a result, either you need infinite resources, very long development cycles, or your users will need to often migrate from version to version.\n\nStripe has come up [with a solution](https://stripe.com/blog/api-versioning): let\'s have one latest app version whose responses get migrated to older versions and let\'s describe changes between these versions using migrations. This approach allows them to keep versions for **years** without dropping them. Obviously, each breaking change is still bad and each version still makes our system more complex and expensive, but their approach gives us a chance to minimize that. Additionally, it allows us backport features and bugfixes to older versions. However, you will also be backporting bugs, which is a sad consequence of eliminating duplication.\n\nUniversi is heavily inspired by this approach so let\'s continue our tutorial and now try to combine the two versions we created using versioning.\n\n### Creating the Migration\n\nWe need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.\n\n```python\nfrom universi import Field\nfrom universi.structure import (\n    schema,\n    AbstractVersionChange,\n    convert_response_to_previous_version_for,\n)\n\nclass ChangeAddressToList(AbstractVersionChange):\n    description = (\n        "Change user address to a list of strings to "\n        "allow the user to specify multiple addresses"\n    )\n    instructions_to_migrate_to_previous_version = (\n        # You should use schema inheritance if you don\'t want to repeat yourself in such cases\n        schema(UserCreateRequest).field("addresses").didnt_exist,\n        schema(UserCreateRequest).field("address").existed_with(type=str, info=Field()),\n        schema(UserResource).field("addresses").didnt_exist,\n        schema(UserResource).field("address").existed_with(type=str, info=Field()),\n    )\n\n    @convert_response_to_previous_version_for(get_user, create_user)\n    def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:\n        data["address"] = data.pop("addresses")[0]\n    \n    @schema(UserCreateRequest).had_property("addresses")\n    def addresses_property(parsed_schema):\n        return [parsed_schema.address]\n\n```\n\ns\nSee how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn\'t, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn\'t have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.\n\nSee how we added the `addresses` property? This simple instruction will allow us to use `addresses` even from the old schema, which means that our api route will not need to know anything about versioning. The main goal of universi is to shift the logic of versioning away from your business logic and api endpoints which makes your project easier to navigate and which makes deleting versions a breeze.\n\n### Grouping Version Changes\n\nFinally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let\'s use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002\'s version.\n\n```python\nfrom universi.structure import Version, Versions\nfrom datetime import date\n\nversions = Versions(\n    Version(date(2002, 1, 1), ChangeAddressToList),\n    Version(date(2001, 1, 1)),\n)\n```\n\nThat\'s it. You\'re done with describing things. Now you just gotta ask universi to do the rest for you. We\'ll need the VersionedAPIRouter we used previously, our API versions, and the module representing the latest versions of our schemas.\n\n```python\nfrom versions import latest\nfrom universi import regenerate_dir_to_all_versions, api_version_var\n\nregenerate_dir_to_all_versions(latest, versions)\nrouter_versions = router.create_versioned_copies(\n    versions,\n    latest_schemas_module=latest,\n)\napi_version_var.set(date(2002, 1, 1))\nuvicorn.run(router_versions[date(2002, 1, 1)])\n```\n\nUniversi has generated multiple things in this code:\n\n* Three versions of our schemas: one for each API version and one that includes definitions of unions of all versions for each schema which will be useful when you want to type check that you are using requests of different versions correctly. For example, we\'ll have `UserCreateRequestUnion` defined there which is a `TypeAlias` pointing to the union of 2002 version and 2001 version of `UserCreateRequest`.\n* Two versions of our API router: one for each API version\n\nYou can now just pick a router by its version and run it separately or use a parent router/app to specify the logic by which you\'d like to pick a version. I recommend using a header-based router with version dates as headers. And yes, that\'s how Stripe does it.\n\nNote that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.\n\nObviously, this was just a simple example and universi has a lot more features so if you\'re interested -- take a look at the reference\n\n## Reference\n\nTBD\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/universi',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['universi',
 'universi.structure'] package_data = \ {'': ['*']} install_requires = \
-['fastapi>=0.96.1', 'type-inspector>=1.2.2,<2.0.0', 'typer[all]', 'typing-
-extensions'] setup_kwargs = { 'name': 'universi', 'version': '0.6.0',
-'description': '', 'long_description': '# universi\n\nModern Stripe-like API
+['fastapi>=0.96.1', 'typing-extensions'] setup_kwargs = { 'name': 'universi',
+'version': '0.7.0', 'description': '', 'long_description': '#
+universi\n\nModern [Stripe-like](https://stripe.com/blog/api-versioning) API
 versioning for FastAPI\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install universi\n```\n\n\n\n## Who is this
-for?\n\nUniversi and its approach will be useful if you want to support many
-API versions for a long time and backport features and bugfixes back to all of
-your versions easily like Stripe does. It is made possible by moving all
-"versioning" logic away from your business code and encapsulating it in small
-"migration modules" which are then combined to create a full blown versioning
-infrastructure.\n\n## Tutorial\n\nThis guide provides a step-by-step tutorial
-for setting up automatic API versioning using Universi library. I will
-illustrate this with an example of a User API, where we will be implementing
-changes to a User\'s address.\n\n### A dummy setup\n\nHere is an initial API
-setup where the User has a single address. We will be implementing two routes -
-one for creating a user and another for retrieving user details. We\'ll be
-using "int" for ID for simplicity.\n\nThe first API you come up with usually
-doesn\'t require more than one address -- why bother?\n\nSo we create our file
-with schemas:\n\n```python\nfrom pydantic import BaseModel\n\n\nclass
-UserCreateRequest(BaseModel):\n address: str\n\nclass UserResource(BaseModel):
-\n id: int\n address: str\n```\n\nAnd we create our file with routes:
-\n\n```python\nfrom versions.latest.users import UserCreateRequest,
-UserResource\nfrom universi import VersionedAPIRouter\n\nrouter =
-VersionedAPIRouter()\n\n@router.post("/users",
+for?\n\nUniversi allows you to support a single version of your code, auto-
+generating the code/routes for older versions. You keep versioning encapsulated
+in small and independent "version change" modules while your business logic
+knows nothing about versioning.\n\nIts approach will be useful if you want to:
+\n\n1. Support many API versions for a long time\n2. Effortlessly backport
+features and bugfixes to all of your versions\n\nOtherwise, more conventional
+methods of API versioning may be preferable.\n\n## Tutorial\n\nThis guide
+provides a step-by-step tutorial for setting up automatic API versioning using
+Universi library. I will illustrate this with an example of a User API, where
+we will be implementing changes to a User\'s address.\n\n### A dummy
+setup\n\nHere is an initial API setup where the User has a single address. We
+will be implementing two routes - one for creating a user and another for
+retrieving user details. We\'ll be using "int" for ID for simplicity.\n\nThe
+first API you come up with usually doesn\'t require more than one address -
+- why bother?\n\nSo we create our file with schemas:\n\n```python\nfrom
+pydantic import BaseModel\n\n\nclass UserCreateRequest(BaseModel):\n address:
+str\n\nclass UserResource(BaseModel):\n id: int\n address: str\n```\n\nAnd we
+create our file with routes:\n\n```python\nfrom versions.latest.users import
+UserCreateRequest, UserResource\nfrom universi import
+VersionedAPIRouter\n\nrouter = VersionedAPIRouter()\n\n@router.post("/users",
 response_model=UserResource)\nasync def create_user(payload:
 UserCreateRequest):\n return {\n "id": 83,\n "address": payload.address,\n
 }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def
 get_user(user_id: int):\n return {\n "id": user_id,\n "address": "123 Example
 St",\n }\n```\n\n### Turning address into a list\n\nDuring our development, we
 have realized that the initial API design was wrong and that addresses should
 have always been a list because the user wants to have multiple addresses to
```

### Comparing `universi-0.6.0/PKG-INFO` & `universi-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: universi
-Version: 0.6.0
-Summary: 
-Home-page: https://github.com/ovsyanka83/universi
-License: MIT
-Author: Stanislav Zmiev
-Author-email: szmiev2000@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.96.1)
-Requires-Dist: type-inspector (>=1.2.2,<2.0.0)
-Requires-Dist: typer[all]
-Requires-Dist: typing-extensions
-Project-URL: Repository, https://github.com/ovsyanka83/universi
-Description-Content-Type: text/markdown
-
 # universi
 
-Modern Stripe-like API versioning for FastAPI
+Modern [Stripe-like](https://stripe.com/blog/api-versioning) API versioning for FastAPI
 
 ---
 
 <p align="center">
 <a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
@@ -48,15 +28,22 @@
 <!---
 # TODO: Note that we don't handle "from .schemas import Schema as OtherSchema" case
 # TODO: Need to validate that the user doesn't use versioned schemas instead of the latest ones
 -->
 
 ## Who is this for?
 
-Universi and its approach will be useful if you want to support many API versions for a long time and backport features and bugfixes back to all of your versions easily like Stripe does. It is made possible by moving all "versioning" logic away from your business code and encapsulating it in small "migration modules" which are then combined to create a full blown versioning infrastructure.
+Universi allows you to support a single version of your code, auto-generating the code/routes for older versions. You keep versioning encapsulated in small and independent "version change" modules while your business logic knows nothing about versioning.
+
+Its approach will be useful if you want to:
+
+1. Support many API versions for a long time
+2. Effortlessly backport features and bugfixes to all of your versions
+
+Otherwise, more conventional methods of API versioning may be preferable.
 
 ## Tutorial
 
 This guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User's address.
 
 ### A dummy setup
 
@@ -220,8 +207,7 @@
 Note that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.
 
 Obviously, this was just a simple example and universi has a lot more features so if you're interested -- take a look at the reference
 
 ## Reference
 
 TBD
-
```

