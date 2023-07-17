# Comparing `tmp/safir-4.3.0.tar.gz` & `tmp/safir-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-4.3.0.tar", last modified: Tue May 23 23:05:04 2023, max compression
+gzip compressed data, was "safir-4.3.1.tar", last modified: Mon Jul 17 20:02:27 2023, max compression
```

## Comparing `safir-4.3.0.tar` & `safir-4.3.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 23:04:52.000000 safir-4.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 23:04:52.000000 safir-4.3.0/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-23 23:04:52.000000 safir-4.3.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-23 23:04:52.000000 safir-4.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 23:04:52.000000 safir-4.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-23 23:04:52.000000 safir-4.3.0/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 23:04:52.000000 safir-4.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-23 23:04:52.000000 safir-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-23 23:04:52.000000 safir-4.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-23 23:04:52.000000 safir-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 23:04:52.000000 safir-4.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-23 23:05:04.445803 safir-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-23 23:04:52.000000 safir-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 23:04:52.000000 safir-4.3.0/changelog.d/_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 23:04:52.000000 safir-4.3.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 23:04:52.000000 safir-4.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-23 23:04:52.000000 safir-4.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 23:04:52.000000 safir-4.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-23 23:04:52.000000 safir-4.3.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-23 23:04:52.000000 safir-4.3.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 23:04:52.000000 safir-4.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/gcs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.437803 safir-4.3.0/docs/user-guide/github-apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/api-resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/create-a-github-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/handling-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/github-apps/webhook-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/pydantic-redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-23 23:04:52.000000 safir-4.3.0/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-23 23:04:52.000000 safir-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:05:04.445803 safir-4.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/github/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/github/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77235 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-23 23:04:52.000000 safir-4.3.0/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.441803 safir-4.3.0/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 23:05:04.000000 safir-4.3.0/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 23:04:52.000000 safir-4.3.0/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-23 23:04:52.000000 safir-4.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-23 23:04:52.000000 safir-4.3.0/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-23 23:04:52.000000 safir-4.3.0/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 23:04:52.000000 safir-4.3.0/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-23 23:04:52.000000 safir-4.3.0/tests/fastapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-23 23:04:52.000000 safir-4.3.0/tests/gcs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.433803 safir-4.3.0/tests/github/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/github/data/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/check_run_created.json
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/check_suite_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/installation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/installation_repositories.json
--rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/pull_request_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/data/webhooks/push_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-23 23:04:52.000000 safir-4.3.0/tests/github/webhooks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 23:04:52.000000 safir-4.3.0/tests/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-23 23:04:52.000000 safir-4.3.0/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-23 23:04:52.000000 safir-4.3.0/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 23:04:52.000000 safir-4.3.0/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-23 23:04:52.000000 safir-4.3.0/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-23 23:04:52.000000 safir-4.3.0/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-23 23:04:52.000000 safir-4.3.0/tests/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 23:04:52.000000 safir-4.3.0/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-23 23:04:52.000000 safir-4.3.0/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:05:04.445803 safir-4.3.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-23 23:04:52.000000 safir-4.3.0/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 23:04:52.000000 safir-4.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 20:02:16.000000 safir-4.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.554480 safir-4.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 20:02:16.000000 safir-4.3.1/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 20:02:16.000000 safir-4.3.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 20:02:16.000000 safir-4.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.554480 safir-4.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-17 20:02:16.000000 safir-4.3.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-17 20:02:16.000000 safir-4.3.1/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-17 20:02:16.000000 safir-4.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-17 20:02:16.000000 safir-4.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-17 20:02:16.000000 safir-4.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 20:02:16.000000 safir-4.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 20:02:16.000000 safir-4.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-17 20:02:27.566480 safir-4.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-17 20:02:16.000000 safir-4.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.554480 safir-4.3.1/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 20:02:16.000000 safir-4.3.1/changelog.d/_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.554480 safir-4.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-17 20:02:16.000000 safir-4.3.1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-17 20:02:16.000000 safir-4.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-17 20:02:16.000000 safir-4.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 20:02:16.000000 safir-4.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.554480 safir-4.3.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-17 20:02:16.000000 safir-4.3.1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 20:02:16.000000 safir-4.3.1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-17 20:02:16.000000 safir-4.3.1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 20:02:16.000000 safir-4.3.1/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 20:02:16.000000 safir-4.3.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.558480 safir-4.3.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.558480 safir-4.3.1/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-17 20:02:16.000000 safir-4.3.1/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-17 20:02:16.000000 safir-4.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:02:27.566480 safir-4.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.550480 safir-4.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.558480 safir-4.3.1/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.562480 safir-4.3.1/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.562480 safir-4.3.1/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.562480 safir-4.3.1/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.562480 safir-4.3.1/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.562480 safir-4.3.1/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77235 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-17 20:02:16.000000 safir-4.3.1/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.558480 safir-4.3.1/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-17 20:02:27.000000 safir-4.3.1/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-17 20:02:27.000000 safir-4.3.1/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:02:27.000000 safir-4.3.1/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-17 20:02:27.000000 safir-4.3.1/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 20:02:27.000000 safir-4.3.1/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 20:02:16.000000 safir-4.3.1/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-17 20:02:16.000000 safir-4.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-17 20:02:16.000000 safir-4.3.1/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-17 20:02:16.000000 safir-4.3.1/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-17 20:02:16.000000 safir-4.3.1/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 20:02:16.000000 safir-4.3.1/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-17 20:02:16.000000 safir-4.3.1/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.550480 safir-4.3.1/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-17 20:02:16.000000 safir-4.3.1/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 20:02:16.000000 safir-4.3.1/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-17 20:02:16.000000 safir-4.3.1/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 20:02:16.000000 safir-4.3.1/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-17 20:02:16.000000 safir-4.3.1/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-17 20:02:16.000000 safir-4.3.1/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 20:02:16.000000 safir-4.3.1/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-17 20:02:16.000000 safir-4.3.1/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-17 20:02:16.000000 safir-4.3.1/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 20:02:16.000000 safir-4.3.1/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-17 20:02:16.000000 safir-4.3.1/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-17 20:02:16.000000 safir-4.3.1/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:27.566480 safir-4.3.1/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:02:16.000000 safir-4.3.1/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-17 20:02:16.000000 safir-4.3.1/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-17 20:02:16.000000 safir-4.3.1/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-07-17 20:02:16.000000 safir-4.3.1/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 20:02:16.000000 safir-4.3.1/tox.ini
```

### Comparing `safir-4.3.0/.github/workflows/ci.yaml` & `safir-4.3.1/.github/workflows/ci.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 name: Python CI
 
 "on":
+  merge_group: {}
+  pull_request: {}
   push:
     branches-ignore:
       # These should always correspond to pull requests, so ignore them for
       # the push trigger and let them be triggered by the pull_request
       # trigger, avoiding running the workflow twice.  This is a minor
       # optimization so there's no need to ensure this is comprehensive.
       - "dependabot/**"
       - "renovate/**"
       - "tickets/**"
       - "u/**"
-    tags:
-      - "*"
-  pull_request: {}
+  release:
+    types: [published]
 
 jobs:
 
   lint:
 
     runs-on: ubuntu-latest
     steps:
@@ -79,23 +80,46 @@
           dir: "docs/_build/html"
           username: ${{ secrets.LTD_USERNAME }}
           password: ${{ secrets.LTD_PASSWORD }}
         if: >
           github.event_name != 'pull_request'
           || startsWith(github.head_ref, 'tickets/')
 
-  pypi:
+  test-packaging:
 
+    name: Test packaging
+    timeout-minutes: 5
     runs-on: ubuntu-latest
     needs: [lint, test, docs]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
-        uses: lsst-sqre/build-and-publish-to-pypi@v1
+        uses: lsst-sqre/build-and-publish-to-pypi@v2
+        with:
+          python-version: "3.11"
+          upload: false
+
+  pypi:
+
+    name: Upload release to PyPI
+    runs-on: ubuntu-latest
+    timeout-minutes: 10
+    needs: [lint, test, docs, test-packaging]
+    environment:
+      name: pypi
+      url: https://pypi.org/p/safir
+    permissions:
+      id-token: write
+    if: github.event_name == 'release' && github.event.action == 'published'
+
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0 # full history for setuptools_scm
+
+      - uses: lsst-sqre/build-and-publish-to-pypi@v2
         with:
-          pypi-token: ${{ secrets.PYPI_SQRE_ADMIN }}
           python-version: "3.11"
-          upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags/') }}
```

### Comparing `safir-4.3.0/.gitignore` & `safir-4.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/.pre-commit-config.yaml` & `safir-4.3.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
   - repo: https://github.com/ambv/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
         args: [-l, '76', -t, py311]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
```

### Comparing `safir-4.3.0/CHANGELOG.md` & `safir-4.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 Versioning follows [semver](https://semver.org/).
 
 This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-4.3.1'></a>
+## 4.3.1 (2023-07-17)
+
+### Bug fixes
+
+- Safir now pins the major version of all of its non-development dependencies. The impetus for this change is to prevent upgrades to Pydantic 2.x until Safir's Pydantic models are ready for that upgrade, but a similar principle applies to other dependencies. These pins will be selectively relaxed once Safir has been confirmed to work with a new major release.
+
 <a id='changelog-4.3.0'></a>
 ## 4.3.0 (2023-05-23)
 
 ### New features
 
 - All `delete_*` APIs in the mock Kubernetes API now support `grace_period_seconds` and a `V1DeleteOptions` body. Both are ignored.
 - `delete_namespaced_job` in the mock Kubernetes API now requires `propagation_policy` to be passed as a keyword argument if provided, and does not require it be set. It is validated against the values recognized by Kubernetes, and if set to `Orphan`, pods created by the job are not deleted.
```

### Comparing `safir-4.3.0/LICENSE` & `safir-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/PKG-INFO` & `safir-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.3.0
+Version: 4.3.1
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.3.0/README.md` & `safir-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/_rst_epilog.rst` & `safir-4.3.1/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/api.rst` & `safir-4.3.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/changelog.md` & `safir-4.3.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 Versioning follows [semver](https://semver.org/).
 
 This project uses [scriv](https://scriv.readthedocs.io/en/stable/) to maintain the change log.
 Changes for the upcoming release can be found in [changelog.d](https://github.com/lsst-sqre/safir/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-4.3.1'></a>
+## 4.3.1 (2023-07-17)
+
+### Bug fixes
+
+- Safir now pins the major version of all of its non-development dependencies. The impetus for this change is to prevent upgrades to Pydantic 2.x until Safir's Pydantic models are ready for that upgrade, but a similar principle applies to other dependencies. These pins will be selectively relaxed once Safir has been confirmed to work with a new major release.
+
 <a id='changelog-4.3.0'></a>
 ## 4.3.0 (2023-05-23)
 
 ### New features
 
 - All `delete_*` APIs in the mock Kubernetes API now support `grace_period_seconds` and a `V1DeleteOptions` body. Both are ignored.
 - `delete_namespaced_job` in the mock Kubernetes API now requires `propagation_policy` to be passed as a keyword argument if provided, and does not require it be set. It is validated against the values recognized by Kubernetes, and if set to `Orphan`, pods created by the job are not deleted.
```

### Comparing `safir-4.3.0/docs/dev/development.rst` & `safir-4.3.1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/dev/release.rst` & `safir-4.3.1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/documenteer.toml` & `safir-4.3.1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/index.rst` & `safir-4.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/arq.rst` & `safir-4.3.1/docs/user-guide/arq.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/database.rst` & `safir-4.3.1/docs/user-guide/database.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/datetime.rst` & `safir-4.3.1/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/fastapi-errors.rst` & `safir-4.3.1/docs/user-guide/fastapi-errors.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/gafaelfawr.rst` & `safir-4.3.1/docs/user-guide/gafaelfawr.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/gcs.rst` & `safir-4.3.1/docs/user-guide/gcs.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/github-apps/api-resources.rst` & `safir-4.3.1/docs/user-guide/github-apps/api-resources.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/github-apps/create-a-github-client.rst` & `safir-4.3.1/docs/user-guide/github-apps/create-a-github-client.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
        github_app_private_key: SecretStr = Field(env="GITHUB_APP_PRIVATE_KEY")
 
 
    config = Config()
 
    github_client_factory = GitHubAppClientFactory(
-       app_id=config.github_app_id,
-       private_key=config.github_app_private_key.get_secret_value(),
+       id=config.github_app_id,
+       key=config.github_app_private_key.get_secret_value(),
        name="lsst-sqre/example",
        http_client=http_client,  # from http_client dependency
    )
 
 .. tip::
 
    The ``name`` parameter is the name of your GitHub App.
```

### Comparing `safir-4.3.0/docs/user-guide/github-apps/handling-webhooks.rst` & `safir-4.3.1/docs/user-guide/github-apps/handling-webhooks.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
    )
    async def post_github_webhook(
        request: Request,
        logger: BoundLogger = Depends(logger_dependency),
    ) -> Response:
        """Process GitHub webhook events."""
        webhook_secret = config.github_webhook_secret.get_secret_value()
+       body = await request.body()
        event = Event.from_http(request.headers, body, secret=webhook_secret)
 
        # Bind the X-GitHub-Delivery header to the logger context; this identifies
        # the webhook request in GitHub's API and UI for diagnostics
        logger = logger.bind(github_delivery=event.delivery_id)
 
        logger.debug("Received GitHub webhook", payload=event.data)
```

### Comparing `safir-4.3.0/docs/user-guide/github-apps/index.rst` & `safir-4.3.1/docs/user-guide/github-apps/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/github-apps/webhook-models.rst` & `safir-4.3.1/docs/user-guide/github-apps/webhook-models.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/http-client.rst` & `safir-4.3.1/docs/user-guide/http-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/ivoa.rst` & `safir-4.3.1/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/kubernetes.rst` & `safir-4.3.1/docs/user-guide/kubernetes.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/logging.rst` & `safir-4.3.1/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/pydantic-redis.rst` & `safir-4.3.1/docs/user-guide/pydantic-redis.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/pydantic.rst` & `safir-4.3.1/docs/user-guide/pydantic.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/set-up-from-template.rst` & `safir-4.3.1/docs/user-guide/set-up-from-template.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/slack-webhook.rst` & `safir-4.3.1/docs/user-guide/slack-webhook.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/uvicorn.rst` & `safir-4.3.1/docs/user-guide/uvicorn.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/docs/user-guide/x-forwarded.rst` & `safir-4.3.1/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/pyproject.toml` & `safir-4.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,31 @@
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dependencies = [
-    "cryptography",
-    "fastapi",
-    "gidgethub",
-    "httpx>=0.20.0",
-    "pydantic",
-    "starlette",
-    "structlog>=21.2.0",
+    "cryptography<42",
+    "fastapi<1",
+    "gidgethub<6",
+    "httpx>=0.20.0,<1",
+    "pydantic<2",
+    "starlette<1",
+    "structlog>=21.2.0,<24",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 arq = [
-    "arq>=0.23"
+    "arq>=0.23,<1"
 ]
 db = [
-    "asyncpg",
-    "sqlalchemy[asyncio]>=1.4.18",
+    "asyncpg<1",
+    "sqlalchemy[asyncio]>=1.4.18,<3",
 ]
 dev = [
     "asgi-lifespan",
     "coverage[toml]",
     "flake8",
     "mypy",
     "pre-commit",
@@ -51,26 +51,26 @@
     "pytest-asyncio",
     "respx",
     "scriv",
     "sqlalchemy[mypy]",
     "types-redis",
     "uvicorn",
     # documentation
-    "documenteer[guide]>=0.7.0b2",
+    "documenteer[guide]>=0.7.0,<1",
     "autodoc_pydantic",
 ]
 gcs = [
-    "google-auth",
-    "google-cloud-storage"
+    "google-auth<3",
+    "google-cloud-storage<3"
 ]
 kubernetes = [
-    "kubernetes_asyncio"
+    "kubernetes_asyncio<25"
 ]
 redis = [
-    "redis>=4.2.0rc1,!=4.5.2", # https://github.com/redis/redis-py/issues/2633
+    "redis>4.5.2,<5",
 ]
 
 [[project.authors]]
 name = "Association of Universities for Research in Astronomy, Inc. (AURA)"
 email = "sqre-admin@lists.lsst.org"
 
 [project.urls]
```

### Comparing `safir-4.3.0/src/safir/__init__.py` & `safir-4.3.1/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/arq.py` & `safir-4.3.1/src/safir/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/asyncio.py` & `safir-4.3.1/src/safir/asyncio.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/database.py` & `safir-4.3.1/src/safir/database.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/datetime.py` & `safir-4.3.1/src/safir/datetime.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/dependencies/arq.py` & `safir-4.3.1/src/safir/dependencies/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/dependencies/db_session.py` & `safir-4.3.1/src/safir/dependencies/db_session.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/dependencies/gafaelfawr.py` & `safir-4.3.1/src/safir/dependencies/gafaelfawr.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/dependencies/http_client.py` & `safir-4.3.1/src/safir/dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/dependencies/logger.py` & `safir-4.3.1/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/fastapi.py` & `safir-4.3.1/src/safir/fastapi.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/gcs.py` & `safir-4.3.1/src/safir/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/github/_client.py` & `safir-4.3.1/src/safir/github/_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/github/models.py` & `safir-4.3.1/src/safir/github/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/github/webhooks.py` & `safir-4.3.1/src/safir/github/webhooks.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/kubernetes.py` & `safir-4.3.1/src/safir/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/logging.py` & `safir-4.3.1/src/safir/logging.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/metadata.py` & `safir-4.3.1/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/middleware/ivoa.py` & `safir-4.3.1/src/safir/middleware/ivoa.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/middleware/x_forwarded.py` & `safir-4.3.1/src/safir/middleware/x_forwarded.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/models.py` & `safir-4.3.1/src/safir/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/pydantic.py` & `safir-4.3.1/src/safir/pydantic.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/redis.py` & `safir-4.3.1/src/safir/redis.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/slack/blockkit.py` & `safir-4.3.1/src/safir/slack/blockkit.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/slack/webhook.py` & `safir-4.3.1/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/testing/gcs.py` & `safir-4.3.1/src/safir/testing/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/testing/kubernetes.py` & `safir-4.3.1/src/safir/testing/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/testing/slack.py` & `safir-4.3.1/src/safir/testing/slack.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir/testing/uvicorn.py` & `safir-4.3.1/src/safir/testing/uvicorn.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/src/safir.egg-info/PKG-INFO` & `safir-4.3.1/src/safir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.3.0
+Version: 4.3.1
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.3.0/src/safir.egg-info/SOURCES.txt` & `safir-4.3.1/src/safir.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README.md
 pyproject.toml
 tox.ini
 .github/CODE_OF_CONDUCT
 .github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/workflows/ci.yaml
-.github/workflows/periodic.yaml
+.github/workflows/periodic-ci.yaml
 changelog.d/_template.md
 docs/_rst_epilog.rst
 docs/api.rst
 docs/changelog.md
 docs/conf.py
 docs/documenteer.toml
 docs/index.rst
```

### Comparing `safir-4.3.0/tests/conftest.py` & `safir-4.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/database_test.py` & `safir-4.3.1/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/datetime_test.py` & `safir-4.3.1/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/dependencies/arq_test.py` & `safir-4.3.1/tests/dependencies/arq_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/dependencies/db_session_test.py` & `safir-4.3.1/tests/dependencies/db_session_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/dependencies/gafaelfawr_test.py` & `safir-4.3.1/tests/dependencies/gafaelfawr_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/dependencies/http_client_test.py` & `safir-4.3.1/tests/dependencies/http_client_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/dependencies/logger_test.py` & `safir-4.3.1/tests/dependencies/logger_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/fastapi_test.py` & `safir-4.3.1/tests/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/gcs_test.py` & `safir-4.3.1/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/check_run_created.json` & `safir-4.3.1/tests/github/data/webhooks/check_run_created.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/check_suite_completed.json` & `safir-4.3.1/tests/github/data/webhooks/check_suite_completed.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/installation.json` & `safir-4.3.1/tests/github/data/webhooks/installation.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/installation_repositories.json` & `safir-4.3.1/tests/github/data/webhooks/installation_repositories.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/pull_request_event.json` & `safir-4.3.1/tests/github/data/webhooks/pull_request_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/data/webhooks/push_event.json` & `safir-4.3.1/tests/github/data/webhooks/push_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/github/webhooks_test.py` & `safir-4.3.1/tests/github/webhooks_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/logging_test.py` & `safir-4.3.1/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/metadata_test.py` & `safir-4.3.1/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/middleware/ivoa_test.py` & `safir-4.3.1/tests/middleware/ivoa_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/middleware/x_forwarded_test.py` & `safir-4.3.1/tests/middleware/x_forwarded_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/pydantic_test.py` & `safir-4.3.1/tests/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/redis_test.py` & `safir-4.3.1/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/slack/blockkit_test.py` & `safir-4.3.1/tests/slack/blockkit_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/slack/webhook_test.py` & `safir-4.3.1/tests/slack/webhook_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/testing/conftest.py` & `safir-4.3.1/tests/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/testing/gcs_test.py` & `safir-4.3.1/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tests/testing/kubernetes_test.py` & `safir-4.3.1/tests/testing/kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.3.0/tox.ini` & `safir-4.3.1/tox.ini`

 * *Files identical despite different names*

