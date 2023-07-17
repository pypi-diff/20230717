# Comparing `tmp/fractal_repositories-0.0.6.tar.gz` & `tmp/fractal_repositories-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_repositories-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_repositories-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_repositories-0.0.6.tar` & `fractal_repositories-0.0.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-07-08 10:15:44.586098 fractal_repositories-0.0.6/.coveragerc
--rw-r--r--   0        0        0      100 2023-07-08 10:15:44.586098 fractal_repositories-0.0.6/.flake8
--rw-r--r--   0        0        0      945 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.gitignore
--rw-r--r--   0        0        0      161 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.isort.cfg
--rw-r--r--   0        0        0       43 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.mypy.ini
--rw-r--r--   0        0        0     1691 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/LICENSE
--rw-r--r--   0        0        0     1557 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/Makefile
--rw-r--r--   0        0        0     2276 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/README.md
--rw-r--r--   0        0        0      780 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/align_version.py
--rw-r--r--   0        0        0      182 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     5318 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3253 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1681 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2965 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      957 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3088 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/poetry.lock
--rw-r--r--   0        0        0     1667 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/setup.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-07-08 10:15:44.590098 fractal_repositories-0.0.6/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/core/__init__.py
--rw-r--r--   0        0        0     3208 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1144 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      898 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3764 2023-07-08 10:15:44.594098 fractal_repositories-0.0.6/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3150 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-07-08 10:15:44.598098 fractal_repositories-0.0.6/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.coveragerc
+-rw-r--r--   0        0        0      100 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.flake8
+-rw-r--r--   0        0        0      945 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.gitignore
+-rw-r--r--   0        0        0      161 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1557 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/Makefile
+-rw-r--r--   0        0        0     2276 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/README.md
+-rw-r--r--   0        0        0      780 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/align_version.py
+-rw-r--r--   0        0        0      182 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5318 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3253 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-07-17 14:27:04.768360 fractal_repositories-0.0.7/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2909 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      957 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3088 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/setup.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/core/__init__.py
+-rw-r--r--   0        0        0     3208 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1144 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      898 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3745 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3150 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-07-17 14:27:04.772360 fractal_repositories-0.0.7/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.7/PKG-INFO
```

### Comparing `fractal_repositories-0.0.6/.github/workflows/build.yml` & `fractal_repositories-0.0.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/.github/workflows/publish.yml` & `fractal_repositories-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/.gitignore` & `fractal_repositories-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/.pre-commit-config.yaml` & `fractal_repositories-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/LICENSE` & `fractal_repositories-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/Makefile` & `fractal_repositories-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/README.md` & `fractal_repositories-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/align_version.py` & `fractal_repositories-0.0.7/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.7/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.7/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.7/fractal_repositories/contrib/mongo/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.7/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.7/fractal_repositories/core/entity.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.7/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.7/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.7/fractal_repositories/mixins/file_repository_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 from typing import Iterator
 
 from fractal_specifications.generic.operators import NotSpecification
 from fractal_specifications.generic.specification import Specification
 
 from fractal_repositories.core.repositories import EntityType, FileRepository
-from fractal_repositories.exceptions import ObjectNotFoundException, RepositoryException
+from fractal_repositories.exceptions import ObjectNotFoundException
 from fractal_repositories.mixins.inmemory_repository_mixin import (
     InMemoryRepositoryMixin,
 )
 from fractal_repositories.utils.json_encoder import EnhancedEncoder
 
 
 class RootDirMixin(object):
@@ -25,15 +25,15 @@
     @property
     def _filename(self) -> str:
         return os.path.join(self.root_dir, "db", f"{self.__class__.__name__}.txt")
 
     @property
     def _get_entities(self) -> Iterator[EntityType]:
         if not os.path.exists(self._filename):
-            raise RepositoryException(f"Path '{self._filename}' doesn't exist.")
+            open(self._filename, "a").close()
         with open(self._filename, "r") as fp:
             for line in fp.readlines():
                 yield self.entity.from_dict(json.loads(line))
 
     def add(self, entity: EntityType) -> EntityType:
         with open(self._filename, "a") as fp:
             fp.write(json.dumps(entity.asdict(), cls=EnhancedEncoder) + "\n")
```

### Comparing `fractal_repositories-0.0.6/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.7/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.7/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.7/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.7/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.7/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/pyproject.toml` & `fractal_repositories-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.6"
+version = "0.0.7"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_repositories-0.0.6/tests/contrib/test_django.py` & `fractal_repositories-0.0.7/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.7/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.7/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.7/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/core/test_models.py` & `fractal_repositories-0.0.7/tests/core/test_models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/core/test_repositories.py` & `fractal_repositories-0.0.7/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.7/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/django/models.py` & `fractal_repositories-0.0.7/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/firestore.py` & `fractal_repositories-0.0.7/tests/fixtures/firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/mongo.py` & `fractal_repositories-0.0.7/tests/fixtures/mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/repositories.py` & `fractal_repositories-0.0.7/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.7/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_file_repository_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,11 +108,10 @@
 
     from fractal_specifications.generic.specification import Specification
 
     assert len(list(file_repository.find(Specification.parse(id=2)))) == 0
 
 
 def test_find_path_doesnt_exist(file_repository, mocker_os_path_exists_error):
-    from fractal_repositories.exceptions import RepositoryException
-
-    with pytest.raises(RepositoryException):
-        next(file_repository.find())
+    # with pytest.raises(RepositoryException):
+    #     next(file_repository.find())
+    assert list(file_repository.find()) == []
```

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.7/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.7/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.7/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.7/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/tox.ini` & `fractal_repositories-0.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.6/PKG-INFO` & `fractal_repositories-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

