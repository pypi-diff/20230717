# Comparing `tmp/tap_pulumi_cloud-0.0.2.tar.gz` & `tmp/tap_pulumi_cloud-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_pulumi_cloud-0.0.2.tar", max compression
+gzip compressed data, was "tap_pulumi_cloud-0.0.2a1.tar", max compression
```

## Comparing `tap_pulumi_cloud-0.0.2.tar` & `tap_pulumi_cloud-0.0.2a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/LICENSE
--rw-r--r--   0        0        0     3087 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/README.md
--rw-r--r--   0        0        0     2307 2023-07-17 15:03:09.240629 tap_pulumi_cloud-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/__init__.py
--rw-r--r--   0        0        0      129 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/__main__.py
--rw-r--r--   0        0        0     2027 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/client.py
--rw-r--r--   0        0        0     7958 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/streams.py
--rw-r--r--   0        0        0     2496 2023-07-17 15:02:49.246880 tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/tap.py
--rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 tap_pulumi_cloud-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0     3087 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/README.md
+-rw-r--r--   0        0        0     2131 2023-05-12 18:12:36.079154 tap_pulumi_cloud-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/__main__.py
+-rw-r--r--   0        0        0     2027 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/client.py
+-rw-r--r--   0        0        0     7957 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/streams.py
+-rw-r--r--   0        0        0     2496 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/tap.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 tap_pulumi_cloud-0.0.2a1/PKG-INFO
```

### Comparing `tap_pulumi_cloud-0.0.2/LICENSE` & `tap_pulumi_cloud-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.2/README.md` & `tap_pulumi_cloud-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.2/pyproject.toml` & `tap_pulumi_cloud-0.0.2a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [build-system]
-build-backend = "poetry_dynamic_versioning.backend"
-requires = [
-  "poetry-core==1.6",
-  "poetry-dynamic-versioning",
-]
+requires = ["poetry-core>=1,<2"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tap-pulumi-cloud"
-version = "0.0.2"
+version = "0.0.2a1"
 description = "`tap-pulumi-cloud` is a Singer tap for Pulumi Cloud, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Pulumi Cloud",
 ]
@@ -21,72 +18,68 @@
 repository = "https://github.com/edgarrmondragon/tap-pulumi-cloud"
 documentation = "https://github.com/edgarrmondragon/tap-pulumi-cloud#readme"
 
 [tool.poetry.dependencies]
 pyhumps = "^3.8.0"
 python = "<3.12,>=3.7.1"
 requests-cache = "^1.0.1"
-singer-sdk = "0.30.0"
+singer-sdk = "0.27.0"
 
 [tool.poetry.group.dev.dependencies]
-singer-sdk = { version = "0.30.0", extras = ["testing"] }
+singer-sdk = { version = "0.27.0", extras = ["testing"] }
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-pulumi-cloud" = "tap_pulumi_cloud.tap:TapPulumiCloud.cli"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+format-jinja = """
+    {%- if distance == 0 -%}
+        {{ serialize_pep440(base, stage, revision) }}
+    {%- elif revision is not none -%}
+        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
+    {%- else -%}
+        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
+    {%- endif -%}
+"""
+metadata = true
+style = "pep440"
+vcs = "git"
+
+[tool.pytest.ini_options]
+addopts = "-vvv"
+
+[tool.mypy]
+python_version = "3.10"
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = ["backoff.*"]
+
 [tool.ruff]
 ignore = [
   "ANN101", # missing-type-self
   "DJ",     # flake8-django
 ]
 line-length = 88
 select = ["ALL"]
 src = ["tap_pulumi_cloud", "tests"]
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
 "noxfile.py" = ["ANN"]
-"tap_pulumi_cloud/streams.py" = [
-    "RUF012",  # mutable-class-default
-]
 "tests/*" = [
   "ANN201",  # missing-return-type-public-function
   "S101",    # assert
   "SLF001",  # private-member-access
 ]
 
 [tool.ruff.flake8-annotations]
 allow-star-arg-any = true
 
 [tool.ruff.isort]
 known-first-party = ["tap_pulumi_cloud"]
-required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
-
-[tool.pytest.ini_options]
-addopts = "-vvv"
-
-[tool.mypy]
-python_version = "3.10"
-warn_unused_configs = true
-
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-module = ["backoff.*"]
-
-[tool.poetry-dynamic-versioning]
-enable = false
-format-jinja = """
-    {%- if distance == 0 -%}
-        {{ serialize_pep440(base, stage, revision) }}
-    {%- elif revision is not none -%}
-        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
-    {%- else -%}
-        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
-    {%- endif -%}
-"""
-metadata = true
-style = "pep440"
-vcs = "git"
```

### Comparing `tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/client.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/client.py`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/streams.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     records_jsonpath = "$.updates[*]"
 
     parent_stream_type = Stacks
 
     schema = th.PropertiesList(
         th.Property(
             "version",
-            th.IntegerType,
+            th.StringType,
             description="The ID of the update.",
         ),
         th.Property(
             "org_name",
             th.StringType,
             description="The name of the organization that owns the stack.",
         ),
```

### Comparing `tap_pulumi_cloud-0.0.2/tap_pulumi_cloud/tap.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/tap.py`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.2/PKG-INFO` & `tap_pulumi_cloud-0.0.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-pulumi-cloud
-Version: 0.0.2
+Version: 0.0.2a1
 Summary: `tap-pulumi-cloud` is a Singer tap for Pulumi Cloud, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-pulumi-cloud
 License: Apache-2.0
 Keywords: ELT,singer.io,Pulumi Cloud
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: singer-sdk (==0.30.0)
+Requires-Dist: singer-sdk (==0.27.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pulumi-cloud#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-pulumi-cloud
 Description-Content-Type: text/markdown
 
 # `tap-pulumi-cloud`
 
 Singer tap for Pulumi Cloud.
```

