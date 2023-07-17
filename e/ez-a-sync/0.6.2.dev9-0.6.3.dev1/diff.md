# Comparing `tmp/ez-a-sync-0.6.2.dev9.tar.gz` & `tmp/ez-a-sync-0.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.6.2.dev9.tar", last modified: Sun Jul 16 19:30:34 2023, max compression
+gzip compressed data, was "ez-a-sync-0.6.3.dev1.tar", last modified: Mon Jul 17 04:18:26 2023, max compression
```

## Comparing `ez-a-sync-0.6.2.dev9.tar` & `ez-a-sync-0.6.3.dev1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.494823 ez-a-sync-0.6.2.dev9/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.486822 ez-a-sync-0.6.2.dev9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-16 19:30:34.494823 ez-a-sync-0.6.2.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     7326 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/prio_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.490823 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-16 19:30:34.000000 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-16 19:30:34.000000 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 19:30:34.000000 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-16 19:30:34.000000 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-16 19:30:34.000000 ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-16 19:30:34.494823 ez-a-sync-0.6.2.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:34.494823 ez-a-sync-0.6.2.dev9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-16 19:30:22.000000 ez-a-sync-0.6.2.dev9/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.318651 ez-a-sync-0.6.3.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.318651 ez-a-sync-0.6.3.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7326 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-17 04:18:26.000000 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-17 04:18:26.000000 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 04:18:26.000000 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-17 04:18:26.000000 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-17 04:18:26.000000 ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:26.322651 ez-a-sync-0.6.3.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-17 04:18:11.000000 ez-a-sync-0.6.3.dev1/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.6.2.dev9/.github/workflows/codeql.yaml` & `ez-a-sync-0.6.3.dev1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/.github/workflows/mypy.yaml` & `ez-a-sync-0.6.3.dev1/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/.github/workflows/pytest.yaml` & `ez-a-sync-0.6.3.dev1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/.github/workflows/release.yaml` & `ez-a-sync-0.6.3.dev1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/LICENSE.txt` & `ez-a-sync-0.6.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/README.md` & `ez-a-sync-0.6.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/__init__.py` & `ez-a-sync-0.6.3.dev1/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_bound.py` & `ez-a-sync-0.6.3.dev1/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_flags.py` & `ez-a-sync-0.6.3.dev1/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_helpers.py` & `ez-a-sync-0.6.3.dev1/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_kwargs.py` & `ez-a-sync-0.6.3.dev1/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_meta.py` & `ez-a-sync-0.6.3.dev1/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/_typing.py` & `ez-a-sync-0.6.3.dev1/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/abstract.py` & `ez-a-sync-0.6.3.dev1/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/base.py` & `ez-a-sync-0.6.3.dev1/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/config.py` & `ez-a-sync-0.6.3.dev1/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/decorator.py` & `ez-a-sync-0.6.3.dev1/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/exceptions.py` & `ez-a-sync-0.6.3.dev1/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modified.py` & `ez-a-sync-0.6.3.dev1/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/__init__.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/limiter.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/manager.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.6.3.dev1/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/_debug.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/executor.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 With these executors, you can simply run sync fns in your executor with `await executor.run(fn, *args)`
 
 `executor.submit(fn, *args)` will work the same as the concurrent.futures implementation, but will return an asyncio.Future instead of a concurrent.futures.Future
 """
 
 import asyncio
 import concurrent.futures as cf
+import multiprocessing.context
 import queue
 import threading
 import weakref
 from concurrent.futures import _base, thread
-from typing import Callable, TypeVar
+from typing import Any, Callable, Optional, Tuple, TypeVar
 
 from typing_extensions import ParamSpec
 
 from a_sync.primitives._debug import _DebugDaemonMixin
 
 TEN_MINUTES = 60 * 10
 
@@ -32,14 +33,16 @@
         Doesn't `await this_executor.run(fn, *args)` look so much better?
         
         Oh, and you can also use kwargs!
         """
         return await self.submit(fn, *args, **kwargs)
     def submit(self, fn: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> "asyncio.Future[T]":
         """Submits a job to the executor and returns an `asyncio.Future` that can be awaited for the result without blocking."""
+        if self._max_workers == 0:
+            return fn(*args, **kwargs)
         fut = asyncio.futures.wrap_future(super().submit(fn, *args, **kwargs))
         self._start_debug_daemon(fut, fn, *args, **kwargs)
         return fut
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} object at {hex(id(self))} [{self.worker_count_current}/{self._max_workers} {self._workers}]>"
     def __len__(self) -> int:
         # NOTE: should this be queue length instead? probably
@@ -54,19 +57,43 @@
             if not fut.done():
                 self.logger.debug(f'{self} processing {fn}{args}{kwargs}')
     
 # Process
 
 class AsyncProcessPoolExecutor(_AsyncExecutorMixin, cf.ProcessPoolExecutor):
     _workers = "processes"
+    def __init__(
+        self, 
+        max_workers: Optional[int] = None, 
+        mp_context: Optional[multiprocessing.context.BaseContext] = None, 
+        initializer: Callable[..., object] = None,
+        initargs: Tuple[Any, ...] = (),
+    ) -> None:
+        if max_workers == 0:
+            super().__init__(1, mp_context, initializer, initargs)
+            self._max_workers = 0
+        else:
+            super().__init__(max_workers, mp_context, initializer, initargs)
 
 # Thread
 
 class AsyncThreadPoolExecutor(_AsyncExecutorMixin, cf.ThreadPoolExecutor):
     _workers = "threads"
+    def __init__(
+        self, 
+        max_workers: Optional[int] = None, 
+        thread_name_prefix: str = '', 
+        initializer: Callable[..., object] = None,
+        initargs: Tuple[Any, ...] = (),
+    ) -> None:
+        if max_workers == 0:
+            super().__init__(1, thread_name_prefix, initializer, initargs)
+            self._max_workers = 0
+        else:
+            super().__init__(max_workers, thread_name_prefix, initializer, initargs)
     
 # For backward-compatibility
 ProcessPoolExecutor = AsyncProcessPoolExecutor
 ThreadPoolExecutor = AsyncThreadPoolExecutor
 
 # Pruning thread pool
```

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/event.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/prio_semaphore.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/prio_semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.6.3.dev1/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/a_sync/property.py` & `ez-a-sync-0.6.3.dev1/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.6.3.dev1/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/setup.py` & `ez-a-sync-0.6.3.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/fixtures.py` & `ez-a-sync-0.6.3.dev1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_base.py` & `ez-a-sync-0.6.3.dev1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_cache.py` & `ez-a-sync-0.6.3.dev1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_decorator.py` & `ez-a-sync-0.6.3.dev1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_executor.py` & `ez-a-sync-0.6.3.dev1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_limiter.py` & `ez-a-sync-0.6.3.dev1/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_meta.py` & `ez-a-sync-0.6.3.dev1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev9/tests/test_semaphore.py` & `ez-a-sync-0.6.3.dev1/tests/test_semaphore.py`

 * *Files identical despite different names*

