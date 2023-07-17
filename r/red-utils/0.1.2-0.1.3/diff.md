# Comparing `tmp/red_utils-0.1.2.tar.gz` & `tmp/red_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_utils-0.1.2.tar", last modified: Mon Jul 17 02:12:55 2023, max compression
+gzip compressed data, was "red_utils-0.1.3.tar", last modified: Mon Jul 17 17:01:55 2023, max compression
```

## Comparing `red_utils-0.1.2.tar` & `red_utils-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,988 @@
--rw-r--r--   0        0        0      382 2023-07-17 01:24:33.568271 red_utils-0.1.2/README.md
--rw-r--r--   0        0        0     1611 2023-07-17 02:12:55.001429 red_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/__init__.py
--rw-r--r--   0        0        0      834 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/diskcache_utils/__init__.py
--rw-r--r--   0        0        0      414 2023-07-17 01:49:11.280717 red_utils-0.1.2/red_utils/diskcache_utils/constants.py
--rw-r--r--   0        0        0     8111 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/diskcache_utils/operations.py
--rw-r--r--   0        0        0     5287 2023-07-16 04:24:14.730610 red_utils-0.1.2/red_utils/diskcache_utils/validators.py
--rw-r--r--   0        0        0      566 2023-07-16 04:24:14.730610 red_utils-0.1.2/red_utils/fastapi_utils/__init__.py
--rw-r--r--   0        0        0      511 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/constants.py
--rw-r--r--   0        0        0      780 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/dependencies.py
--rw-r--r--   0        0        0      677 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/healthcheck.py
--rw-r--r--   0        0        0     4559 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/operations.py
--rw-r--r--   0        0        0     1263 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/tag_definitions.py
--rw-r--r--   0        0        0     2047 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/uvicorn_override.py
--rw-r--r--   0        0        0     2185 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/fastapi_utils/validators.py
--rw-r--r--   0        0        0      326 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/httpx_utils/__init__.py
--rw-r--r--   0        0        0      177 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/httpx_utils/constants.py
--rw-r--r--   0        0        0     2933 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/httpx_utils/operations.py
--rw-r--r--   0        0        0     1159 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/httpx_utils/validators.py
--rw-r--r--   0        0        0      590 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/loguru_utils/__init__.py
--rw-r--r--   0        0        0     3921 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/loguru_utils/constants.py
--rw-r--r--   0        0        0     2583 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/loguru_utils/operations.py
--rw-r--r--   0        0        0     1694 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/loguru_utils/sinks.py
--rw-r--r--   0        0        0     1954 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/loguru_utils/validators.py
--rw-r--r--   0        0        0      215 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/msgpack_utils/__init__.py
--rw-r--r--   0        0        0       78 2023-07-16 04:24:14.734610 red_utils-0.1.2/red_utils/msgpack_utils/constants.py
--rw-r--r--   0        0        0     5459 2023-07-17 02:11:25.857885 red_utils-0.1.2/red_utils/msgpack_utils/operations.py
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 red_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2349 2023-07-17 04:46:42.890102 red_utils-0.1.3/README.md
+-rw-r--r--   0        0        0     1860 2023-07-17 17:01:55.640472 red_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      372 2023-07-17 05:18:08.596080 red_utils-0.1.3/red_utils/__init__.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:19:58.454819 red_utils-0.1.3/red_utils/dict_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      182 2023-07-17 04:19:58.458819 red_utils-0.1.3/red_utils/dict_utils/.pdm-build/dict_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:19:58.458819 red_utils-0.1.3/red_utils/dict_utils/.pdm-build/dict_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:19:23.319006 red_utils-0.1.3/red_utils/dict_utils/.pdm-python
+-rw-r--r--   0        0        0       40 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/.gitignore
+-rw-r--r--   0        0        0     2207 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate
+-rw-r--r--   0        0        0     1499 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3084 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3403 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1784 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1212 2023-07-17 03:48:18.560720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/activate_this.py
+lrwxr-xr-x   0        0        0        0 2023-07-17 03:48:18.556720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/python -> /home/jack/.pyenv/versions/3.11.4/bin/python3
+lrwxr-xr-x   0        0        0        0 2023-07-17 03:48:18.556720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2023-07-17 03:48:18.556720 red_utils-0.1.3/red_utils/dict_utils/.venv/bin/python3.11 -> python
+-rw-r--r--   0        0        0       18 2023-07-17 03:48:18.556720 red_utils-0.1.3/red_utils/dict_utils/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4311 2023-07-17 03:48:18.556720 red_utils-0.1.3/red_utils/dict_utils/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      348 2023-07-17 03:48:18.564720 red_utils-0.1.3/red_utils/dict_utils/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0       13 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/README.md
+-rw-r--r--   0        0        0       85 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/pdm.lock
+-rw-r--r--   0        0        0      291 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/src/__init__.py
+-rw-r--r--   0        0        0     1775 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/src/operations.py
+-rw-r--r--   0        0        0      313 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/dict_utils/src/validators.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.894102 red_utils-0.1.3/red_utils/diskcache_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:12.666467 red_utils-0.1.3/red_utils/diskcache_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      224 2023-07-17 04:33:12.670467 red_utils-0.1.3/red_utils/diskcache_utils/.pdm-build/diskcache_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:12.670467 red_utils-0.1.3/red_utils/diskcache_utils/.pdm-build/diskcache_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:20:37.374605 red_utils-0.1.3/red_utils/diskcache_utils/.pdm-python
+-rw-r--r--   0        0        0       18 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/README.md
+-rw-r--r--   0        0        0      617 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/__init__.py
+-rw-r--r--   0        0        0       14 2023-07-17 04:21:35.594285 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:21:37.190276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/.gitignore
+-rw-r--r--   0        0        0      559 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache-5.6.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    20458 2023-07-17 04:21:35.702284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache-5.6.1.dist-info/METADATA
+-rw-r--r--   0        0        0      938 2023-07-17 04:21:35.702284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache-5.6.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:21:35.702284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache-5.6.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2023-07-17 04:21:35.702284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache-5.6.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1262 2023-07-17 04:21:35.694284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-17 04:21:35.694284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/cli.py
+-rw-r--r--   0        0        0    81969 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/core.py
+-rw-r--r--   0        0        0    16110 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/djangocache.py
+-rw-r--r--   0        0        0    22725 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/fanout.py
+-rw-r--r--   0        0        0    34681 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/persistent.py
+-rw-r--r--   0        0        0    14922 2023-07-17 04:21:35.698284 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache/recipes.py
+-rw-r--r--   0        0        0      233 2023-07-17 04:21:37.190276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache_utils-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0      506 2023-07-17 04:21:37.194276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache_utils-0.1.0+editable.dist-info/RECORD
+-rw-r--r--   0        0        0       90 2023-07-17 04:21:37.190276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache_utils-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      121 2023-07-17 04:21:37.190276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache_utils-0.1.0+editable.dist-info/direct_url.json
+-rw-r--r--   0        0        0       61 2023-07-17 04:21:37.190276 red_utils-0.1.3/red_utils/diskcache_utils/__pypackages__/3.11/lib/diskcache_utils.pth
+-rw-r--r--   0        0        0      663 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/pdm.lock
+-rw-r--r--   0        0        0      321 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/pyproject.toml
+-rw-r--r--   0        0        0      834 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/src/__init__.py
+-rw-r--r--   0        0        0      414 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/src/constants.py
+-rw-r--r--   0        0        0     8111 2023-07-17 05:03:05.876848 red_utils-0.1.3/red_utils/diskcache_utils/src/operations.py
+-rw-r--r--   0        0        0     5288 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/diskcache_utils/src/validators.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/fastapi_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:12.362468 red_utils-0.1.3/red_utils/fastapi_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      290 2023-07-17 04:33:12.370468 red_utils-0.1.3/red_utils/fastapi_utils/.pdm-build/fastapi_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:12.370468 red_utils-0.1.3/red_utils/fastapi_utils/.pdm-build/fastapi_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:21:16.154392 red_utils-0.1.3/red_utils/fastapi_utils/.pdm-python
+-rw-r--r--   0        0        0       16 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/fastapi_utils/README.md
+-rw-r--r--   0        0        0      553 2023-07-17 04:46:42.898102 red_utils-0.1.3/red_utils/fastapi_utils/__init__.py
+-rw-r--r--   0        0        0       14 2023-07-17 04:22:18.218051 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/.gitignore
+-rwxr-xr-x   0        0        0      241 2023-07-17 04:22:20.198040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/bin/dotenv
+-rwxr-xr-x   0        0        0      240 2023-07-17 04:22:21.318034 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/bin/uvicorn
+-rwxr-xr-x   0        0        0      240 2023-07-17 04:22:22.834025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/bin/watchfiles
+-rw-r--r--   0        0        0        2 2023-07-17 04:22:28.737993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/.gitignore
+-rw-r--r--   0        0        0     1101 2023-07-17 04:22:21.878030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/PyYAML-6.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2056 2023-07-17 04:22:21.878030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/PyYAML-6.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1780 2023-07-17 04:22:22.138029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/PyYAML-6.0.dist-info/RECORD
+-rw-r--r--   0        0        0      152 2023-07-17 04:22:21.870030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/PyYAML-6.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2023-07-17 04:22:21.870030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/PyYAML-6.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1402 2023-07-17 04:22:21.882030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/_yaml/__init__.py
+-rw-r--r--   0        0        0    11685 2023-07-17 04:22:18.738048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types-0.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0      584 2023-07-17 04:22:18.794047 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types-0.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:22:18.742048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types-0.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1083 2023-07-17 04:22:18.758048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types-0.5.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     9375 2023-07-17 04:22:18.722048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:18.730048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types/py.typed
+-rw-r--r--   0        0        0     5680 2023-07-17 04:22:18.734048 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/annotated_types/test_cases.py
+-rw-r--r--   0        0        0     1081 2023-07-17 04:22:19.674043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     4708 2023-07-17 04:22:19.674043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     3482 2023-07-17 04:22:19.706042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:19.690043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       39 2023-07-17 04:22:19.694043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2023-07-17 04:22:19.698042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4073 2023-07-17 04:22:18.978046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.054046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_backends/__init__.py
+-rw-r--r--   0        0        0    67056 2023-07-17 04:22:19.086046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_backends/_asyncio.py
+-rw-r--r--   0        0        0    30035 2023-07-17 04:22:19.090046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_backends/_trio.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.094046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/__init__.py
+-rw-r--r--   0        0        0     5726 2023-07-17 04:22:19.098046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_compat.py
+-rw-r--r--   0        0        0     4083 2023-07-17 04:22:19.110046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_eventloop.py
+-rw-r--r--   0        0        0     2916 2023-07-17 04:22:19.114046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_exceptions.py
+-rw-r--r--   0        0        0    18026 2023-07-17 04:22:19.118046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_fileio.py
+-rw-r--r--   0        0        0      435 2023-07-17 04:22:19.126046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_resources.py
+-rw-r--r--   0        0        0      863 2023-07-17 04:22:19.130046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_signals.py
+-rw-r--r--   0        0        0    20667 2023-07-17 04:22:19.138045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_sockets.py
+-rw-r--r--   0        0        0     1518 2023-07-17 04:22:19.146046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_streams.py
+-rw-r--r--   0        0        0     4977 2023-07-17 04:22:19.146046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_subprocesses.py
+-rw-r--r--   0        0        0    16747 2023-07-17 04:22:19.154045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_synchronization.py
+-rw-r--r--   0        0        0     5316 2023-07-17 04:22:19.158045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_tasks.py
+-rw-r--r--   0        0        0     2217 2023-07-17 04:22:19.162045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_testing.py
+-rw-r--r--   0        0        0     2551 2023-07-17 04:22:19.162045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/_core/_typedattr.py
+-rw-r--r--   0        0        0     2159 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_resources.py
+-rw-r--r--   0        0        0     5243 2023-07-17 04:22:19.170045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_sockets.py
+-rw-r--r--   0        0        0     6584 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_streams.py
+-rw-r--r--   0        0        0     2067 2023-07-17 04:22:19.178045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_subprocesses.py
+-rw-r--r--   0        0        0     3413 2023-07-17 04:22:19.254045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_tasks.py
+-rw-r--r--   0        0        0     1924 2023-07-17 04:22:19.266045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/abc/_testing.py
+-rw-r--r--   0        0        0    16563 2023-07-17 04:22:18.982046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/from_thread.py
+-rw-r--r--   0        0        0     4647 2023-07-17 04:22:18.990046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/lowlevel.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:18.994046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/py.typed
+-rw-r--r--   0        0        0     5022 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.274045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/__init__.py
+-rw-r--r--   0        0        0     4473 2023-07-17 04:22:19.274045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/buffered.py
+-rw-r--r--   0        0        0     4356 2023-07-17 04:22:19.626043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/file.py
+-rw-r--r--   0        0        0     9274 2023-07-17 04:22:19.630043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/memory.py
+-rw-r--r--   0        0        0     4275 2023-07-17 04:22:19.638043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/stapled.py
+-rw-r--r--   0        0        0     5043 2023-07-17 04:22:19.650043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/text.py
+-rw-r--r--   0        0        0    12099 2023-07-17 04:22:19.670043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/streams/tls.py
+-rw-r--r--   0        0        0     9242 2023-07-17 04:22:19.030046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/to_process.py
+-rw-r--r--   0        0        0     2146 2023-07-17 04:22:19.046046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/anyio/to_thread.py
+-rw-r--r--   0        0        0     1475 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click-8.1.5.dist-info/LICENSE.rst
+-rw-r--r--   0        0        0     3014 2023-07-17 04:22:19.170045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click-8.1.5.dist-info/METADATA
+-rw-r--r--   0        0        0     1647 2023-07-17 04:22:19.178045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click-8.1.5.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click-8.1.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click-8.1.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3138 2023-07-17 04:22:18.978046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/__init__.py
+-rw-r--r--   0        0        0    18730 2023-07-17 04:22:18.986046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/_compat.py
+-rw-r--r--   0        0        0    24069 2023-07-17 04:22:18.994046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/_termui_impl.py
+-rw-r--r--   0        0        0     1353 2023-07-17 04:22:19.002046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/_textwrap.py
+-rw-r--r--   0        0        0     7860 2023-07-17 04:22:19.018046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/_winconsole.py
+-rw-r--r--   0        0        0   114086 2023-07-17 04:22:19.054046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/core.py
+-rw-r--r--   0        0        0    19096 2023-07-17 04:22:19.082046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/decorators.py
+-rw-r--r--   0        0        0     9273 2023-07-17 04:22:19.090046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/exceptions.py
+-rw-r--r--   0        0        0     9706 2023-07-17 04:22:19.098046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/formatting.py
+-rw-r--r--   0        0        0     1961 2023-07-17 04:22:19.102046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/globals.py
+-rw-r--r--   0        0        0    19067 2023-07-17 04:22:19.110046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/parser.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.114046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/py.typed
+-rw-r--r--   0        0        0    18396 2023-07-17 04:22:19.122046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/shell_completion.py
+-rw-r--r--   0        0        0    28324 2023-07-17 04:22:19.130046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/termui.py
+-rw-r--r--   0        0        0    16084 2023-07-17 04:22:19.146046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/testing.py
+-rw-r--r--   0        0        0    36391 2023-07-17 04:22:19.154045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/types.py
+-rw-r--r--   0        0        0    20298 2023-07-17 04:22:19.162045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/click/utils.py
+-rw-r--r--   0        0        0     1292 2023-07-17 04:22:20.206040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/__init__.py
+-rw-r--r--   0        0        0      129 2023-07-17 04:22:20.210040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/__main__.py
+-rw-r--r--   0        0        0     5809 2023-07-17 04:22:20.210040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/cli.py
+-rw-r--r--   0        0        0     1303 2023-07-17 04:22:20.214040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/ipython.py
+-rw-r--r--   0        0        0    11932 2023-07-17 04:22:20.214040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/main.py
+-rw-r--r--   0        0        0     5186 2023-07-17 04:22:20.226040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/parser.py
+-rw-r--r--   0        0        0       26 2023-07-17 04:22:20.230039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/py.typed
+-rw-r--r--   0        0        0     2348 2023-07-17 04:22:20.230039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/variables.py
+-rw-r--r--   0        0        0       22 2023-07-17 04:22:20.238039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/dotenv/version.py
+-rw-r--r--   0        0        0    23461 2023-07-17 04:22:19.158045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi-0.100.0.dist-info/METADATA
+-rw-r--r--   0        0        0     3862 2023-07-17 04:22:19.234045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi-0.100.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi-0.100.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1086 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi-0.100.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     1081 2023-07-17 04:22:18.970046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/__init__.py
+-rw-r--r--   0        0        0    22213 2023-07-17 04:22:18.982046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/_compat.py
+-rw-r--r--   0        0        0    40021 2023-07-17 04:22:18.994046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/applications.py
+-rw-r--r--   0        0        0       76 2023-07-17 04:22:19.002046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/background.py
+-rw-r--r--   0        0        0     1468 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/concurrency.py
+-rw-r--r--   0        0        0     2793 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/datastructures.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.090046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-17 04:22:19.098046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/dependencies/models.py
+-rw-r--r--   0        0        0    29721 2023-07-17 04:22:19.102046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/dependencies/utils.py
+-rw-r--r--   0        0        0     8056 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/encoders.py
+-rw-r--r--   0        0        0     1332 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/exception_handlers.py
+-rw-r--r--   0        0        0     1400 2023-07-17 04:22:19.010046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/exceptions.py
+-rw-r--r--   0        0        0       54 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/logger.py
+-rw-r--r--   0        0        0       58 2023-07-17 04:22:19.106046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1035 2023-07-17 04:22:19.110046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0       79 2023-07-17 04:22:19.110046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2023-07-17 04:22:19.114046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2023-07-17 04:22:19.122046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2023-07-17 04:22:19.122046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2023-07-17 04:22:19.126046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.130046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-17 04:22:19.134045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/openapi/constants.py
+-rw-r--r--   0        0        0     6532 2023-07-17 04:22:19.134045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/openapi/docs.py
+-rw-r--r--   0        0        0    17733 2023-07-17 04:22:19.138045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/openapi/models.py
+-rw-r--r--   0        0        0    21047 2023-07-17 04:22:19.146046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/openapi/utils.py
+-rw-r--r--   0        0        0    18411 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/param_functions.py
+-rw-r--r--   0        0        0    26883 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/params.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/py.typed
+-rw-r--r--   0        0        0      142 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/requests.py
+-rw-r--r--   0        0        0     1242 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/responses.py
+-rw-r--r--   0        0        0    56905 2023-07-17 04:22:19.014046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/routing.py
+-rw-r--r--   0        0        0      881 2023-07-17 04:22:19.150045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/__init__.py
+-rw-r--r--   0        0        0     2939 2023-07-17 04:22:19.150045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/api_key.py
+-rw-r--r--   0        0        0      141 2023-07-17 04:22:19.150045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/base.py
+-rw-r--r--   0        0        0     5964 2023-07-17 04:22:19.150045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/http.py
+-rw-r--r--   0        0        0     8579 2023-07-17 04:22:19.150045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/oauth2.py
+-rw-r--r--   0        0        0     1141 2023-07-17 04:22:19.154045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2023-07-17 04:22:19.154045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/security/utils.py
+-rw-r--r--   0        0        0       69 2023-07-17 04:22:19.022046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2023-07-17 04:22:19.026046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/templating.py
+-rw-r--r--   0        0        0       66 2023-07-17 04:22:19.034046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/testclient.py
+-rw-r--r--   0        0        0      428 2023-07-17 04:22:19.066046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/types.py
+-rw-r--r--   0        0        0     8179 2023-07-17 04:22:19.082046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/utils.py
+-rw-r--r--   0        0        0      222 2023-07-17 04:22:19.086046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi/websockets.py
+-rw-r--r--   0        0        0      299 2023-07-17 04:22:28.737993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi_utils-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0      496 2023-07-17 04:22:28.741993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi_utils-0.1.0+editable.dist-info/RECORD
+-rw-r--r--   0        0        0       90 2023-07-17 04:22:28.737993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi_utils-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      119 2023-07-17 04:22:28.741993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi_utils-0.1.0+editable.dist-info/direct_url.json
+-rw-r--r--   0        0        0       59 2023-07-17 04:22:28.741993 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/fastapi_utils.pth
+-rw-r--r--   0        0        0     1124 2023-07-17 04:22:19.266045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     8175 2023-07-17 04:22:19.298045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2215 2023-07-17 04:22:19.642043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:19.634043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2023-07-17 04:22:19.638043 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1507 2023-07-17 04:22:19.018046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/__init__.py
+-rw-r--r--   0        0        0     4815 2023-07-17 04:22:19.018046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_abnf.py
+-rw-r--r--   0        0        0    26539 2023-07-17 04:22:19.030046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_connection.py
+-rw-r--r--   0        0        0    11816 2023-07-17 04:22:19.050046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_events.py
+-rw-r--r--   0        0        0    10230 2023-07-17 04:22:19.082046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_headers.py
+-rw-r--r--   0        0        0     8383 2023-07-17 04:22:19.090046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_readers.py
+-rw-r--r--   0        0        0     5252 2023-07-17 04:22:19.098046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_receivebuffer.py
+-rw-r--r--   0        0        0    13300 2023-07-17 04:22:19.102046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_state.py
+-rw-r--r--   0        0        0     4888 2023-07-17 04:22:19.106046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_util.py
+-rw-r--r--   0        0        0      686 2023-07-17 04:22:19.110046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_version.py
+-rw-r--r--   0        0        0     5081 2023-07-17 04:22:19.114046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/_writers.py
+-rw-r--r--   0        0        0        7 2023-07-17 04:22:19.118046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/py.typed
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.118046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-17 04:22:19.250045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/data/test-file
+-rw-r--r--   0        0        0     3355 2023-07-17 04:22:19.126046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/helpers.py
+-rw-r--r--   0        0        0     3995 2023-07-17 04:22:19.130046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_against_stdlib_http.py
+-rw-r--r--   0        0        0    38720 2023-07-17 04:22:19.134045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_connection.py
+-rw-r--r--   0        0        0     4657 2023-07-17 04:22:19.138045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_events.py
+-rw-r--r--   0        0        0     5612 2023-07-17 04:22:19.158045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_headers.py
+-rw-r--r--   0        0        0      794 2023-07-17 04:22:19.162045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_helpers.py
+-rw-r--r--   0        0        0    16386 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_io.py
+-rw-r--r--   0        0        0     3454 2023-07-17 04:22:19.170045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_receivebuffer.py
+-rw-r--r--   0        0        0     8928 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_state.py
+-rw-r--r--   0        0        0     2970 2023-07-17 04:22:19.218045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/h11/tests/test_util.py
+-rw-r--r--   0        0        0     1093 2023-07-17 04:22:19.830042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools-0.6.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3595 2023-07-17 04:22:19.834042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools-0.6.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1121 2023-07-17 04:22:19.834042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools-0.6.0.dist-info/RECORD
+-rw-r--r--   0        0        0      225 2023-07-17 04:22:19.830042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools-0.6.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2023-07-17 04:22:19.830042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools-0.6.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      147 2023-07-17 04:22:19.746042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/__init__.py
+-rw-r--r--   0        0        0      575 2023-07-17 04:22:19.746042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/_version.py
+-rw-r--r--   0        0        0      166 2023-07-17 04:22:19.810042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/__init__.py
+-rw-r--r--   0        0        0      566 2023-07-17 04:22:19.746042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/errors.py
+-rw-r--r--   0        0        0   406227 2023-07-17 04:22:19.750042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/parser.c
+-rwxr-xr-x   0        0        0   705784 2023-07-17 04:22:19.810042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/parser.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0   242528 2023-07-17 04:22:19.774042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/url_parser.c
+-rwxr-xr-x   0        0        0   319376 2023-07-17 04:22:19.830042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/httptools/parser/url_parser.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1523 2023-07-17 04:22:19.170045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9830 2023-07-17 04:22:19.218045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      925 2023-07-17 04:22:19.234045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2023-07-17 04:22:19.174045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0      849 2023-07-17 04:22:19.138045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2023-07-17 04:22:19.138045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/codec.py
+-rw-r--r--   0        0        0      321 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/compat.py
+-rw-r--r--   0        0        0    12950 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/core.py
+-rw-r--r--   0        0        0    44375 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/intranges.py
+-rw-r--r--   0        0        0       21 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/package_data.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.142046 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/py.typed
+-rw-r--r--   0        0        0   206539 2023-07-17 04:22:19.166045 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/idna/uts46data.py
+-rw-r--r--   0        0        0     1056 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    22272 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2018 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      626 2023-07-17 04:22:19.766042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/__init__.py
+-rw-r--r--   0        0        0    13934 2023-07-17 04:22:19.778042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/__init__.pyi
+-rw-r--r--   0        0        0      597 2023-07-17 04:22:19.778042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_asyncio_loop.py
+-rw-r--r--   0        0        0    16003 2023-07-17 04:22:19.778042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_better_exceptions.py
+-rw-r--r--   0        0        0     1431 2023-07-17 04:22:19.778042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_colorama.py
+-rw-r--r--   0        0        0    14601 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_colorizer.py
+-rw-r--r--   0        0        0      321 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_contextvars.py
+-rw-r--r--   0        0        0     1531 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_ctime_functions.py
+-rw-r--r--   0        0        0     3220 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_datetime.py
+-rw-r--r--   0        0        0     2879 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_defaults.py
+-rw-r--r--   0        0        0     1107 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_error_interceptor.py
+-rw-r--r--   0        0        0    14586 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_file_sink.py
+-rw-r--r--   0        0        0      618 2023-07-17 04:22:19.782042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_filters.py
+-rw-r--r--   0        0        0      458 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_get_frame.py
+-rw-r--r--   0        0        0    11952 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_handler.py
+-rw-r--r--   0        0        0     1307 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_locks_machinery.py
+-rw-r--r--   0        0        0    94321 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_logger.py
+-rw-r--r--   0        0        0     2174 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_recattrs.py
+-rw-r--r--   0        0        0     3160 2023-07-17 04:22:19.786042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_simple_sinks.py
+-rw-r--r--   0        0        0     4707 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/_string_parsers.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:19.790042 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/loguru/py.typed
+-rw-r--r--   0        0        0   128217 2023-07-17 04:22:23.926019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic-2.0.3.dist-info/METADATA
+-rw-r--r--   0        0        0     8079 2023-07-17 04:22:23.930019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic-2.0.3.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:22:23.926019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic-2.0.3.dist-info/WHEEL
+-rw-r--r--   0        0        0     1129 2023-07-17 04:22:23.930019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic-2.0.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     5036 2023-07-17 04:22:23.558021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:23.686020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     4090 2023-07-17 04:22:23.690020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_annotated_handlers.py
+-rw-r--r--   0        0        0     9546 2023-07-17 04:22:23.710020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3392 2023-07-17 04:22:23.722020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    23137 2023-07-17 04:22:23.734020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0    10836 2023-07-17 04:22:23.738020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    29631 2023-07-17 04:22:23.742020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6273 2023-07-17 04:22:23.746020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    24909 2023-07-17 04:22:23.750020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    11024 2023-07-17 04:22:23.754020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      425 2023-07-17 04:22:23.754020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    81058 2023-07-17 04:22:23.762020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    21152 2023-07-17 04:22:23.766020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      207 2023-07-17 04:22:23.778020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0     9552 2023-07-17 04:22:23.786020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     3011 2023-07-17 04:22:23.798020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_mock_validator.py
+-rw-r--r--   0        0        0    23532 2023-07-17 04:22:23.798020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4210 2023-07-17 04:22:23.798020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4739 2023-07-17 04:22:23.798020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0    37327 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16416 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12170 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     5087 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0     9942 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0    11570 2023-07-17 04:22:23.566021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/_migration.py
+-rw-r--r--   0        0        0     1141 2023-07-17 04:22:23.570021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/alias_generators.py
+-rw-r--r--   0        0        0      147 2023-07-17 04:22:23.574021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21521 2023-07-17 04:22:23.578021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/color.py
+-rw-r--r--   0        0        0     8376 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/config.py
+-rw-r--r--   0        0        0    11088 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/decorator.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:23.802020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9864 2023-07-17 04:22:23.810020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     1785 2023-07-17 04:22:23.818020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7644 2023-07-17 04:22:23.838020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10919 2023-07-17 04:22:23.842020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4465 2023-07-17 04:22:23.846020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2481 2023-07-17 04:22:23.846020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3278 2023-07-17 04:22:23.850020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0      147 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4557 2023-07-17 04:22:23.582021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/errors.py
+-rw-r--r--   0        0        0    38836 2023-07-17 04:22:23.586021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/fields.py
+-rw-r--r--   0        0        0    10830 2023-07-17 04:22:23.586021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    19534 2023-07-17 04:22:23.586021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2023-07-17 04:22:23.586021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2023-07-17 04:22:23.586021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/json.py
+-rw-r--r--   0        0        0    96385 2023-07-17 04:22:23.598021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/json_schema.py
+-rw-r--r--   0        0        0    59079 2023-07-17 04:22:23.602021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/main.py
+-rw-r--r--   0        0        0    48923 2023-07-17 04:22:23.626021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/mypy.py
+-rw-r--r--   0        0        0    13600 2023-07-17 04:22:23.630021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2023-07-17 04:22:23.630021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:23.634021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/py.typed
+-rw-r--r--   0        0        0     3238 2023-07-17 04:22:23.634021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2023-07-17 04:22:23.642021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2023-07-17 04:22:23.642021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/tools.py
+-rw-r--r--   0        0        0    15509 2023-07-17 04:22:23.646021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    45396 2023-07-17 04:22:23.654021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/types.py
+-rw-r--r--   0        0        0      137 2023-07-17 04:22:23.654021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2023-07-17 04:22:23.658021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/utils.py
+-rw-r--r--   0        0        0     2771 2023-07-17 04:22:23.850020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/config.py
+-rw-r--r--   0        0        0    17515 2023-07-17 04:22:23.866020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5142 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50418 2023-07-17 04:22:23.870020 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2023-07-17 04:22:23.886019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2023-07-17 04:22:23.898019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44378 2023-07-17 04:22:23.902019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38641 2023-07-17 04:22:23.910019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    21826 2023-07-17 04:22:23.914019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2023-07-17 04:22:23.918019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:23.918019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47615 2023-07-17 04:22:23.918019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2023-07-17 04:22:23.918019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35380 2023-07-17 04:22:23.918019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2023-07-17 04:22:23.922019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2023-07-17 04:22:23.922019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21887 2023-07-17 04:22:23.926019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2023-07-17 04:22:23.926019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/v1/version.py
+-rw-r--r--   0        0        0     1370 2023-07-17 04:22:23.662021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/validate_call.py
+-rw-r--r--   0        0        0      145 2023-07-17 04:22:23.666021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/validators.py
+-rw-r--r--   0        0        0     1690 2023-07-17 04:22:23.678021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/version.py
+-rw-r--r--   0        0        0     1933 2023-07-17 04:22:23.682021 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic/warnings.py
+-rw-r--r--   0        0        0     5116 2023-07-17 04:22:27.086002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core-2.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      788 2023-07-17 04:22:27.174001 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core-2.3.0.dist-info/RECORD
+-rw-r--r--   0        0        0      129 2023-07-17 04:22:27.086002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core-2.3.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1080 2023-07-17 04:22:27.086002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core-2.3.0.dist-info/license_files/LICENSE
+-rw-r--r--   0        0        0     2190 2023-07-17 04:22:27.090002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core/__init__.py
+-rwxr-xr-x   0        0        0  4611488 2023-07-17 04:22:27.174001 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core/_pydantic_core.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0    10163 2023-07-17 04:22:27.090002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0        0        0   129458 2023-07-17 04:22:27.090002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core/core_schema.py
+-rw-r--r--   0        0        0        1 2023-07-17 04:22:27.086002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/pydantic_core/py.typed
+-rw-r--r--   0        0        0     1556 2023-07-17 04:22:20.242040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    21991 2023-07-17 04:22:20.254039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1242 2023-07-17 04:22:20.266039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:20.258039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       47 2023-07-17 04:22:20.262039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        7 2023-07-17 04:22:20.266039 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/python_dotenv-1.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      185 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE.APACHE2
+-rw-r--r--   0        0        0     1046 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE.MIT
+-rw-r--r--   0        0        0     3588 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1032 2023-07-17 04:22:20.082040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2023-07-17 04:22:20.082040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      310 2023-07-17 04:22:20.058040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-17 04:22:20.058040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/_impl.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/_tests/__init__.py
+-rw-r--r--   0        0        0     2110 2023-07-17 04:22:20.062040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/_tests/test_sniffio.py
+-rw-r--r--   0        0        0       89 2023-07-17 04:22:20.058040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/_version.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:20.058040 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/sniffio/py.typed
+-rw-r--r--   0        0        0     5836 2023-07-17 04:22:20.906036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette-0.27.0.dist-info/METADATA
+-rw-r--r--   0        0        0     3190 2023-07-17 04:22:20.922036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette-0.27.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:22:20.906036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette-0.27.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1518 2023-07-17 04:22:20.910036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette-0.27.0.dist-info/licenses/LICENSE.md
+-rw-r--r--   0        0        0       23 2023-07-17 04:22:20.766037 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-17 04:22:20.766037 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/_compat.py
+-rw-r--r--   0        0        0     2091 2023-07-17 04:22:20.770037 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/_utils.py
+-rw-r--r--   0        0        0    10508 2023-07-17 04:22:20.774037 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/applications.py
+-rw-r--r--   0        0        0     5246 2023-07-17 04:22:20.782036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/authentication.py
+-rw-r--r--   0        0        0     1259 2023-07-17 04:22:20.782036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/background.py
+-rw-r--r--   0        0        0     1741 2023-07-17 04:22:20.786036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/concurrency.py
+-rw-r--r--   0        0        0     4607 2023-07-17 04:22:20.786036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/config.py
+-rw-r--r--   0        0        0     2168 2023-07-17 04:22:20.794036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/convertors.py
+-rw-r--r--   0        0        0    23087 2023-07-17 04:22:20.798036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/datastructures.py
+-rw-r--r--   0        0        0     5143 2023-07-17 04:22:20.814036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/endpoints.py
+-rw-r--r--   0        0        0     1648 2023-07-17 04:22:20.814036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/exceptions.py
+-rw-r--r--   0        0        0    10423 2023-07-17 04:22:20.822036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/formparsers.py
+-rw-r--r--   0        0        0      546 2023-07-17 04:22:20.866036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/__init__.py
+-rw-r--r--   0        0        0     1787 2023-07-17 04:22:20.870036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/authentication.py
+-rw-r--r--   0        0        0     5010 2023-07-17 04:22:20.870036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/base.py
+-rw-r--r--   0        0        0     7075 2023-07-17 04:22:20.874036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/cors.py
+-rw-r--r--   0        0        0     7833 2023-07-17 04:22:20.878036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/errors.py
+-rw-r--r--   0        0        0     4128 2023-07-17 04:22:20.882036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/exceptions.py
+-rw-r--r--   0        0        0     4507 2023-07-17 04:22:20.886036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/gzip.py
+-rw-r--r--   0        0        0      848 2023-07-17 04:22:20.890036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/httpsredirect.py
+-rw-r--r--   0        0        0     3612 2023-07-17 04:22:20.898036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/sessions.py
+-rw-r--r--   0        0        0     2207 2023-07-17 04:22:20.902036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/trustedhost.py
+-rw-r--r--   0        0        0     4906 2023-07-17 04:22:20.906036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:20.822036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/py.typed
+-rw-r--r--   0        0        0    10757 2023-07-17 04:22:20.826036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/requests.py
+-rw-r--r--   0        0        0    13147 2023-07-17 04:22:20.834036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/responses.py
+-rw-r--r--   0        0        0    32447 2023-07-17 04:22:20.838036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/routing.py
+-rw-r--r--   0        0        0     4959 2023-07-17 04:22:20.842036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/schemas.py
+-rw-r--r--   0        0        0     8733 2023-07-17 04:22:20.846036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/staticfiles.py
+-rw-r--r--   0        0        0     6086 2023-07-17 04:22:20.850036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/status.py
+-rw-r--r--   0        0        0     4170 2023-07-17 04:22:20.854036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/templating.py
+-rw-r--r--   0        0        0    29208 2023-07-17 04:22:20.858036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/testclient.py
+-rw-r--r--   0        0        0      613 2023-07-17 04:22:20.858036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/types.py
+-rw-r--r--   0        0        0     7360 2023-07-17 04:22:20.862036 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/starlette/websockets.py
+-rw-r--r--   0        0        0    13936 2023-07-17 04:22:20.446038 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/typing_extensions-4.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3078 2023-07-17 04:22:20.446038 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/typing_extensions-4.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0      414 2023-07-17 04:22:20.446038 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/typing_extensions-4.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2023-07-17 04:22:20.446038 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/typing_extensions-4.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0   111082 2023-07-17 04:22:20.442038 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/typing_extensions.py
+-rw-r--r--   0        0        0     6106 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn-0.23.0.dist-info/METADATA
+-rw-r--r--   0        0        0     3854 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn-0.23.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn-0.23.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       46 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn-0.23.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1526 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn-0.23.0.dist-info/licenses/LICENSE.md
+-rw-r--r--   0        0        0      147 2023-07-17 04:22:21.322034 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-17 04:22:21.326033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/__main__.py
+-rw-r--r--   0        0        0     2403 2023-07-17 04:22:21.326033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/_subprocess.py
+-rw-r--r--   0        0        0     7458 2023-07-17 04:22:21.334033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/_types.py
+-rw-r--r--   0        0        0    21364 2023-07-17 04:22:21.338034 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/config.py
+-rw-r--r--   0        0        0     1174 2023-07-17 04:22:21.342033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/importer.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.378033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/lifespan/__init__.py
+-rw-r--r--   0        0        0      302 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/lifespan/off.py
+-rw-r--r--   0        0        0     5182 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/lifespan/on.py
+-rw-r--r--   0        0        0     4255 2023-07-17 04:22:21.362033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/logging.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/loops/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/loops/asyncio.py
+-rw-r--r--   0        0        0      400 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/loops/auto.py
+-rw-r--r--   0        0        0      148 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/loops/uvloop.py
+-rw-r--r--   0        0        0    16939 2023-07-17 04:22:21.366033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/main.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/middleware/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/middleware/asgi2.py
+-rw-r--r--   0        0        0     2859 2023-07-17 04:22:21.382033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/middleware/message_logger.py
+-rw-r--r--   0        0        0     3261 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/middleware/proxy_headers.py
+-rw-r--r--   0        0        0     7014 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/http/__init__.py
+-rw-r--r--   0        0        0      391 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/http/auto.py
+-rw-r--r--   0        0        0     1777 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/http/flow_control.py
+-rw-r--r--   0        0        0    20262 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/http/h11_impl.py
+-rw-r--r--   0        0        0    21673 2023-07-17 04:22:21.394033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/http/httptools_impl.py
+-rw-r--r--   0        0        0     1839 2023-07-17 04:22:21.386033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/websockets/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/websockets/auto.py
+-rw-r--r--   0        0        0    13573 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/websockets/websockets_impl.py
+-rw-r--r--   0        0        0    13040 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/protocols/websockets/wsproto_impl.py
+-rw-r--r--   0        0        0        1 2023-07-17 04:22:21.378033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/py.typed
+-rw-r--r--   0        0        0    12253 2023-07-17 04:22:21.378033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/server.py
+-rw-r--r--   0        0        0      670 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/__init__.py
+-rw-r--r--   0        0        0     3922 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/basereload.py
+-rw-r--r--   0        0        0     2232 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1580 2023-07-17 04:22:21.398033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/statreload.py
+-rw-r--r--   0        0        0     2924 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/watchfilesreload.py
+-rw-r--r--   0        0        0     5490 2023-07-17 04:22:21.402033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/supervisors/watchgodreload.py
+-rw-r--r--   0        0        0     3675 2023-07-17 04:22:21.378033 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvicorn/workers.py
+-rw-r--r--   0        0        0    11439 2023-07-17 04:22:23.314023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/LICENSE-APACHE
+-rw-r--r--   0        0        0     1105 2023-07-17 04:22:23.298023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/LICENSE-MIT
+-rw-r--r--   0        0        0     4664 2023-07-17 04:22:23.306023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/METADATA
+-rw-r--r--   0        0        0     5342 2023-07-17 04:22:26.978002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/RECORD
+-rw-r--r--   0        0        0      152 2023-07-17 04:22:23.306023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2023-07-17 04:22:23.302023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop-0.17.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1538 2023-07-17 04:22:26.946003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-17 04:22:26.946003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/_noop.py
+-rw-r--r--   0        0        0    15350 2023-07-17 04:22:23.330022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/_testbase.py
+-rw-r--r--   0        0        0      576 2023-07-17 04:22:23.358022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/_version.py
+-rw-r--r--   0        0        0      752 2023-07-17 04:22:26.942003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/cbhandles.pxd
+-rw-r--r--   0        0        0    12116 2023-07-17 04:22:23.346022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/cbhandles.pyx
+-rw-r--r--   0        0        0    14159 2023-07-17 04:22:23.946019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/dns.pyx
+-rw-r--r--   0        0        0     2774 2023-07-17 04:22:23.358022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/errors.pyx
+-rw-r--r--   0        0        0      252 2023-07-17 04:22:26.970003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/async_.pxd
+-rw-r--r--   0        0        0     1500 2023-07-17 04:22:26.966003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/async_.pyx
+-rw-r--r--   0        0        0     1322 2023-07-17 04:22:26.954002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/basetransport.pxd
+-rw-r--r--   0        0        0     9553 2023-07-17 04:22:26.954002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/basetransport.pyx
+-rw-r--r--   0        0        0      276 2023-07-17 04:22:26.966003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/check.pxd
+-rw-r--r--   0        0        0     1865 2023-07-17 04:22:26.962003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/check.pyx
+-rw-r--r--   0        0        0      325 2023-07-17 04:22:26.946003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/fsevent.pxd
+-rw-r--r--   0        0        0     2826 2023-07-17 04:22:26.966003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/fsevent.pyx
+-rw-r--r--   0        0        0     1189 2023-07-17 04:22:26.950003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/handle.pxd
+-rw-r--r--   0        0        0    13219 2023-07-17 04:22:26.962003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/handle.pyx
+-rw-r--r--   0        0        0      274 2023-07-17 04:22:26.954002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/idle.pxd
+-rw-r--r--   0        0        0     1843 2023-07-17 04:22:26.950003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/idle.pyx
+-rw-r--r--   0        0        0      933 2023-07-17 04:22:26.958003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/pipe.pxd
+-rw-r--r--   0        0        0     6950 2023-07-17 04:22:26.970003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/pipe.pyx
+-rw-r--r--   0        0        0      566 2023-07-17 04:22:26.966003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/poll.pxd
+-rw-r--r--   0        0        0     6506 2023-07-17 04:22:26.958003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/poll.pyx
+-rw-r--r--   0        0        0     2297 2023-07-17 04:22:26.950003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/process.pxd
+-rw-r--r--   0        0        0    25818 2023-07-17 04:22:26.966003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/process.pyx
+-rw-r--r--   0        0        0     1535 2023-07-17 04:22:26.962003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/stream.pxd
+-rw-r--r--   0        0        0    31977 2023-07-17 04:22:26.950003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/stream.pyx
+-rw-r--r--   0        0        0      786 2023-07-17 04:22:26.958003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/streamserver.pxd
+-rw-r--r--   0        0        0     4650 2023-07-17 04:22:26.946003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/streamserver.pyx
+-rw-r--r--   0        0        0      892 2023-07-17 04:22:26.958003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/tcp.pxd
+-rw-r--r--   0        0        0     7271 2023-07-17 04:22:26.970003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/tcp.pyx
+-rw-r--r--   0        0        0      440 2023-07-17 04:22:26.958003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/timer.pxd
+-rw-r--r--   0        0        0     2400 2023-07-17 04:22:26.954002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/timer.pyx
+-rw-r--r--   0        0        0      671 2023-07-17 04:22:26.962003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/udp.pxd
+-rw-r--r--   0        0        0    12041 2023-07-17 04:22:26.954002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/handles/udp.pyx
+-rw-r--r--   0        0        0      361 2023-07-17 04:22:26.978002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/__init__.py
+-rw-r--r--   0        0        0     1674 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/compat.h
+-rw-r--r--   0        0        0      687 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/consts.pxi
+-rw-r--r--   0        0        0       51 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/debug.h
+-rw-r--r--   0        0        0       64 2023-07-17 04:22:26.978002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/debug.pxd
+-rw-r--r--   0        0        0      458 2023-07-17 04:22:26.978002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/flowcontrol.pxd
+-rw-r--r--   0        0        0      863 2023-07-17 04:22:26.970003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/fork_handler.h
+-rw-r--r--   0        0        0      846 2023-07-17 04:22:26.970003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/python.pxd
+-rw-r--r--   0        0        0     6334 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/stdlib.pxi
+-rw-r--r--   0        0        0     2186 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/system.pxd
+-rw-r--r--   0        0        0    15998 2023-07-17 04:22:26.974002 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/includes/uv.pxd
+-rw-r--r--   0        0        0  7288791 2023-07-17 04:22:23.902019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/loop.c
+-rwxr-xr-x   0        0        0 11593760 2023-07-17 04:22:26.938003 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/loop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     6190 2023-07-17 04:22:23.378022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/loop.pxd
+-rw-r--r--   0        0        0    10449 2023-07-17 04:22:23.950019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/loop.pyi
+-rw-r--r--   0        0        0   117035 2023-07-17 04:22:23.402022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/loop.pyx
+-rw-r--r--   0        0        0     2279 2023-07-17 04:22:23.438022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/lru.pyx
+-rw-r--r--   0        0        0     5383 2023-07-17 04:22:23.910019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/pseudosock.pyx
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:23.362022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/py.typed
+-rw-r--r--   0        0        0      143 2023-07-17 04:22:23.954019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/request.pxd
+-rw-r--r--   0        0        0     2259 2023-07-17 04:22:23.354022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/request.pyx
+-rw-r--r--   0        0        0      394 2023-07-17 04:22:23.402022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/server.pxd
+-rw-r--r--   0        0        0     3623 2023-07-17 04:22:23.914019 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/server.pyx
+-rw-r--r--   0        0        0     3534 2023-07-17 04:22:23.334022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/sslproto.pxd
+-rw-r--r--   0        0        0    35381 2023-07-17 04:22:23.430022 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/uvloop/sslproto.pyx
+-rw-r--r--   0        0        0     4901 2023-07-17 04:22:22.842025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles-0.19.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1280 2023-07-17 04:22:23.314023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles-0.19.0.dist-info/RECORD
+-rw-r--r--   0        0        0      129 2023-07-17 04:22:22.846025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles-0.19.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       48 2023-07-17 04:22:22.850025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles-0.19.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1110 2023-07-17 04:22:22.854025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles-0.19.0.dist-info/license_files/LICENSE
+-rw-r--r--   0        0        0      364 2023-07-17 04:22:22.858025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-17 04:22:22.854025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/__main__.py
+-rwxr-xr-x   0        0        0  4981776 2023-07-17 04:22:23.310023 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/_rust_notify.abi3.so
+-rw-r--r--   0        0        0     4608 2023-07-17 04:22:22.882025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/_rust_notify.pyi
+-rw-r--r--   0        0        0     7194 2023-07-17 04:22:22.870025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/cli.py
+-rw-r--r--   0        0        0     5164 2023-07-17 04:22:22.862025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/filters.py
+-rw-r--r--   0        0        0    12729 2023-07-17 04:22:22.862025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/main.py
+-rw-r--r--   0        0        0       69 2023-07-17 04:22:22.886025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/py.typed
+-rw-r--r--   0        0        0    14001 2023-07-17 04:22:22.874025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/run.py
+-rw-r--r--   0        0        0       85 2023-07-17 04:22:22.878025 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/watchfiles/version.py
+-rw-r--r--   0        0        0     1514 2023-07-17 04:22:24.282017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets-11.0.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     6619 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets-11.0.3.dist-info/METADATA
+-rw-r--r--   0        0        0     3871 2023-07-17 04:22:24.282017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets-11.0.3.dist-info/RECORD
+-rw-r--r--   0        0        0      225 2023-07-17 04:22:24.282017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets-11.0.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets-11.0.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3426 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/__init__.py
+-rw-r--r--   0        0        0     4744 2023-07-17 04:22:24.206018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/__main__.py
+-rw-r--r--   0        0        0      139 2023-07-17 04:22:24.238017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/auth.py
+-rw-r--r--   0        0        0    12418 2023-07-17 04:22:24.238017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/client.py
+-rw-r--r--   0        0        0      333 2023-07-17 04:22:24.202018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/connection.py
+-rw-r--r--   0        0        0     5738 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/datastructures.py
+-rw-r--r--   0        0        0    10143 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/exceptions.py
+-rw-r--r--   0        0        0       98 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/extensions/__init__.py
+-rw-r--r--   0        0        0     3271 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/extensions/base.py
+-rw-r--r--   0        0        0    24782 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/extensions/permessage_deflate.py
+-rw-r--r--   0        0        0    12537 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/frames.py
+-rw-r--r--   0        0        0    16120 2023-07-17 04:22:24.238017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/headers.py
+-rw-r--r--   0        0        0      644 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/http.py
+-rw-r--r--   0        0        0    12565 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/http11.py
+-rw-r--r--   0        0        0     2790 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/imports.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:24.266017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/__init__.py
+-rw-r--r--   0        0        0     8540 2023-07-17 04:22:24.274017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/async_timeout.py
+-rw-r--r--   0        0        0     6287 2023-07-17 04:22:24.274017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/auth.py
+-rw-r--r--   0        0        0    26555 2023-07-17 04:22:24.274017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/client.py
+-rw-r--r--   0        0        0      758 2023-07-17 04:22:24.262017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/compatibility.py
+-rw-r--r--   0        0        0     4998 2023-07-17 04:22:24.266017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/framing.py
+-rw-r--r--   0        0        0     5479 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/handshake.py
+-rw-r--r--   0        0        0     6938 2023-07-17 04:22:24.274017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/http.py
+-rw-r--r--   0        0        0    63339 2023-07-17 04:22:24.266017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/protocol.py
+-rw-r--r--   0        0        0    45232 2023-07-17 04:22:24.278017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/legacy/server.py
+-rw-r--r--   0        0        0    23822 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/py.typed
+-rw-r--r--   0        0        0    20857 2023-07-17 04:22:24.238017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/server.py
+-rw-r--r--   0        0        0     5834 2023-07-17 04:22:24.238017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/speedups.c
+-rwxr-xr-x   0        0        0    35480 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/speedups.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     4038 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/streams.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:22:24.254017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/__init__.py
+-rw-r--r--   0        0        0    11265 2023-07-17 04:22:24.258017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/client.py
+-rw-r--r--   0        0        0      555 2023-07-17 04:22:24.254017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/compatibility.py
+-rw-r--r--   0        0        0    29284 2023-07-17 04:22:24.250018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/connection.py
+-rw-r--r--   0        0        0     9484 2023-07-17 04:22:24.254017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/messages.py
+-rw-r--r--   0        0        0    18661 2023-07-17 04:22:24.262017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/server.py
+-rw-r--r--   0        0        0     1151 2023-07-17 04:22:24.254017 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/sync/utils.py
+-rw-r--r--   0        0        0     1384 2023-07-17 04:22:24.214018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/typing.py
+-rw-r--r--   0        0        0     3215 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/uri.py
+-rw-r--r--   0        0        0     1150 2023-07-17 04:22:24.202018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/utils.py
+-rw-r--r--   0        0        0     2723 2023-07-17 04:22:24.218018 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/websockets/version.py
+-rw-r--r--   0        0        0    12309 2023-07-17 04:22:22.130029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/__init__.py
+-rwxr-xr-x   0        0        0  2504000 2023-07-17 04:22:22.110029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/_yaml.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     4883 2023-07-17 04:22:22.114029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/composer.py
+-rw-r--r--   0        0        0    28639 2023-07-17 04:22:22.126029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/constructor.py
+-rw-r--r--   0        0        0     3851 2023-07-17 04:22:22.118029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/cyaml.py
+-rw-r--r--   0        0        0     2837 2023-07-17 04:22:21.890030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/dumper.py
+-rw-r--r--   0        0        0    43006 2023-07-17 04:22:21.898030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/emitter.py
+-rw-r--r--   0        0        0     2533 2023-07-17 04:22:21.886030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/error.py
+-rw-r--r--   0        0        0     2445 2023-07-17 04:22:22.126029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/events.py
+-rw-r--r--   0        0        0     2061 2023-07-17 04:22:21.914030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/loader.py
+-rw-r--r--   0        0        0     1440 2023-07-17 04:22:21.910030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/nodes.py
+-rw-r--r--   0        0        0    25495 2023-07-17 04:22:21.914030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/parser.py
+-rw-r--r--   0        0        0     6794 2023-07-17 04:22:21.902030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/reader.py
+-rw-r--r--   0        0        0    14190 2023-07-17 04:22:22.134029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/representer.py
+-rw-r--r--   0        0        0     9004 2023-07-17 04:22:21.906030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/resolver.py
+-rw-r--r--   0        0        0    51279 2023-07-17 04:22:21.926030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/scanner.py
+-rw-r--r--   0        0        0     4165 2023-07-17 04:22:21.890030 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/serializer.py
+-rw-r--r--   0        0        0     2573 2023-07-17 04:22:22.122029 red_utils-0.1.3/red_utils/fastapi_utils/__pypackages__/3.11/lib/yaml/tokens.py
+-rw-r--r--   0        0        0    56395 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/pdm.lock
+-rw-r--r--   0        0        0      373 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/pyproject.toml
+-rw-r--r--   0        0        0      566 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/constants.py
+-rw-r--r--   0        0        0      780 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/dependencies.py
+-rw-r--r--   0        0        0      677 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/healthcheck.py
+-rw-r--r--   0        0        0     4559 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/operations.py
+-rw-r--r--   0        0        0     1263 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/tag_definitions.py
+-rw-r--r--   0        0        0     1964 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/uvicorn_override.py
+-rw-r--r--   0        0        0     2185 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/fastapi_utils/src/validators.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/file_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:12.798466 red_utils-0.1.3/red_utils/file_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      182 2023-07-17 04:33:12.806466 red_utils-0.1.3/red_utils/file_utils/.pdm-build/file_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:12.806466 red_utils-0.1.3/red_utils/file_utils/.pdm-build/file_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:23:13.921745 red_utils-0.1.3/red_utils/file_utils/.pdm-python
+-rw-r--r--   0        0        0       13 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/file_utils/README.md
+-rw-r--r--   0        0        0       67 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/file_utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-17 04:46:42.902102 red_utils-0.1.3/red_utils/file_utils/pdm.lock
+-rw-r--r--   0        0        0      291 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/file_utils/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/file_utils/src/__init__.py
+-rw-r--r--   0        0        0      150 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/file_utils/src/constants.py
+-rw-r--r--   0        0        0     1491 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/file_utils/src/operations.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:12.750466 red_utils-0.1.3/red_utils/hash_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      182 2023-07-17 04:33:12.758466 red_utils-0.1.3/red_utils/hash_utils/.pdm-build/hash_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:12.754466 red_utils-0.1.3/red_utils/hash_utils/.pdm-build/hash_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:23:52.157535 red_utils-0.1.3/red_utils/hash_utils/.pdm-python
+-rw-r--r--   0        0        0       13 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/README.md
+-rw-r--r--   0        0        0       35 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/pdm.lock
+-rw-r--r--   0        0        0      291 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/src/__init__.py
+-rw-r--r--   0        0        0     1055 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/hash_utils/src/operations.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/httpx_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:12.902465 red_utils-0.1.3/red_utils/httpx_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      213 2023-07-17 04:33:12.906465 red_utils-0.1.3/red_utils/httpx_utils/.pdm-build/httpx_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:12.906465 red_utils-0.1.3/red_utils/httpx_utils/.pdm-build/httpx_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:24:25.413352 red_utils-0.1.3/red_utils/httpx_utils/.pdm-python
+-rw-r--r--   0        0        0       14 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/httpx_utils/README.md
+-rw-r--r--   0        0        0      299 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/httpx_utils/__init__.py
+-rw-r--r--   0        0        0       14 2023-07-17 04:24:44.733246 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/.gitignore
+-rwxr-xr-x   0        0        0      233 2023-07-17 04:24:45.405243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/bin/httpx
+-rw-r--r--   0        0        0        2 2023-07-17 04:24:46.961234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/.gitignore
+-rw-r--r--   0        0        0     1081 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     4708 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     3482 2023-07-17 04:24:45.493242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       39 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio-3.7.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4073 2023-07-17 04:24:45.393243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.421243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_backends/__init__.py
+-rw-r--r--   0        0        0    67056 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_backends/_asyncio.py
+-rw-r--r--   0        0        0    30035 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_backends/_trio.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/__init__.py
+-rw-r--r--   0        0        0     5726 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_compat.py
+-rw-r--r--   0        0        0     4083 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_eventloop.py
+-rw-r--r--   0        0        0     2916 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_exceptions.py
+-rw-r--r--   0        0        0    18026 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_fileio.py
+-rw-r--r--   0        0        0      435 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_resources.py
+-rw-r--r--   0        0        0      863 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_signals.py
+-rw-r--r--   0        0        0    20667 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_sockets.py
+-rw-r--r--   0        0        0     1518 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_streams.py
+-rw-r--r--   0        0        0     4977 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_subprocesses.py
+-rw-r--r--   0        0        0    16747 2023-07-17 04:24:45.457242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_synchronization.py
+-rw-r--r--   0        0        0     5316 2023-07-17 04:24:45.457242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_tasks.py
+-rw-r--r--   0        0        0     2217 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_testing.py
+-rw-r--r--   0        0        0     2551 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/_core/_typedattr.py
+-rw-r--r--   0        0        0     2159 2023-07-17 04:24:45.477242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-17 04:24:45.477242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_resources.py
+-rw-r--r--   0        0        0     5243 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_sockets.py
+-rw-r--r--   0        0        0     6584 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_streams.py
+-rw-r--r--   0        0        0     2067 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_subprocesses.py
+-rw-r--r--   0        0        0     3413 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_tasks.py
+-rw-r--r--   0        0        0     1924 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/abc/_testing.py
+-rw-r--r--   0        0        0    16563 2023-07-17 04:24:45.393243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/from_thread.py
+-rw-r--r--   0        0        0     4647 2023-07-17 04:24:45.397243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/lowlevel.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.397243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/py.typed
+-rw-r--r--   0        0        0     5022 2023-07-17 04:24:45.413242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/__init__.py
+-rw-r--r--   0        0        0     4473 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/buffered.py
+-rw-r--r--   0        0        0     4356 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/file.py
+-rw-r--r--   0        0        0     9274 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/memory.py
+-rw-r--r--   0        0        0     4275 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/stapled.py
+-rw-r--r--   0        0        0     5043 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/text.py
+-rw-r--r--   0        0        0    12099 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/streams/tls.py
+-rw-r--r--   0        0        0     9242 2023-07-17 04:24:45.421243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/to_process.py
+-rw-r--r--   0        0        0     2146 2023-07-17 04:24:45.421243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/anyio/to_thread.py
+-rw-r--r--   0        0        0     1052 2023-07-17 04:24:45.405243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi-2023.5.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     2190 2023-07-17 04:24:45.409242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi-2023.5.7.dist-info/METADATA
+-rw-r--r--   0        0        0      768 2023-07-17 04:24:45.413242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi-2023.5.7.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:24:45.409242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi-2023.5.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2023-07-17 04:24:45.413242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi-2023.5.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0       94 2023-07-17 04:24:45.357243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-17 04:24:45.361243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi/__main__.py
+-rw-r--r--   0        0        0   278952 2023-07-17 04:24:45.393243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi/cacert.pem
+-rw-r--r--   0        0        0     4219 2023-07-17 04:24:45.397243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi/core.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.397243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/certifi/py.typed
+-rw-r--r--   0        0        0     1124 2023-07-17 04:24:45.061245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     8175 2023-07-17 04:24:45.065245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2215 2023-07-17 04:24:45.073244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:24:45.069244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2023-07-17 04:24:45.069244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11-0.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1507 2023-07-17 04:24:44.953245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/__init__.py
+-rw-r--r--   0        0        0     4815 2023-07-17 04:24:44.957245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_abnf.py
+-rw-r--r--   0        0        0    26539 2023-07-17 04:24:44.961245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_connection.py
+-rw-r--r--   0        0        0    11816 2023-07-17 04:24:44.965245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_events.py
+-rw-r--r--   0        0        0    10230 2023-07-17 04:24:44.969245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_headers.py
+-rw-r--r--   0        0        0     8383 2023-07-17 04:24:44.981245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_readers.py
+-rw-r--r--   0        0        0     5252 2023-07-17 04:24:44.989245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_receivebuffer.py
+-rw-r--r--   0        0        0    13300 2023-07-17 04:24:44.997245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_state.py
+-rw-r--r--   0        0        0     4888 2023-07-17 04:24:45.001245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_util.py
+-rw-r--r--   0        0        0      686 2023-07-17 04:24:45.005245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_version.py
+-rw-r--r--   0        0        0     5081 2023-07-17 04:24:45.005245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/_writers.py
+-rw-r--r--   0        0        0        7 2023-07-17 04:24:45.009245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/py.typed
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.013245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-17 04:24:45.061245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/data/test-file
+-rw-r--r--   0        0        0     3355 2023-07-17 04:24:45.025245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/helpers.py
+-rw-r--r--   0        0        0     3995 2023-07-17 04:24:45.029245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_against_stdlib_http.py
+-rw-r--r--   0        0        0    38720 2023-07-17 04:24:45.033245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_connection.py
+-rw-r--r--   0        0        0     4657 2023-07-17 04:24:45.037245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_events.py
+-rw-r--r--   0        0        0     5612 2023-07-17 04:24:45.045245 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_headers.py
+-rw-r--r--   0        0        0      794 2023-07-17 04:24:45.049244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_helpers.py
+-rw-r--r--   0        0        0    16386 2023-07-17 04:24:45.049244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_io.py
+-rw-r--r--   0        0        0     3454 2023-07-17 04:24:45.053244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_receivebuffer.py
+-rw-r--r--   0        0        0     8928 2023-07-17 04:24:45.053244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_state.py
+-rw-r--r--   0        0        0     2970 2023-07-17 04:24:45.057244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/h11/tests/test_util.py
+-rw-r--r--   0        0        0     1518 2023-07-17 04:24:45.497242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore-0.17.3.dist-info/LICENSE.md
+-rw-r--r--   0        0        0    18594 2023-07-17 04:24:45.497242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore-0.17.3.dist-info/METADATA
+-rw-r--r--   0        0        0     3036 2023-07-17 04:24:45.501242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore-0.17.3.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:24:45.501242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore-0.17.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       59 2023-07-17 04:24:45.501242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore-0.17.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3338 2023-07-17 04:24:45.421243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/__init__.py
+-rw-r--r--   0        0        0     3167 2023-07-17 04:24:45.425243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_api.py
+-rw-r--r--   0        0        0     1221 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/__init__.py
+-rw-r--r--   0        0        0     8420 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/connection.py
+-rw-r--r--   0        0        0    14305 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/connection_pool.py
+-rw-r--r--   0        0        0    11968 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/http11.py
+-rw-r--r--   0        0        0    23879 2023-07-17 04:24:45.457242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/http2.py
+-rw-r--r--   0        0        0    13999 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/http_proxy.py
+-rw-r--r--   0        0        0     4486 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/interfaces.py
+-rw-r--r--   0        0        0    13810 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_async/socks_proxy.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/__init__.py
+-rw-r--r--   0        0        0     5208 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/anyio.py
+-rw-r--r--   0        0        0     1654 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/auto.py
+-rw-r--r--   0        0        0     3218 2023-07-17 04:24:45.469242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/base.py
+-rw-r--r--   0        0        0     4179 2023-07-17 04:24:45.469242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/mock.py
+-rw-r--r--   0        0        0     4444 2023-07-17 04:24:45.473242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/sync.py
+-rw-r--r--   0        0        0     6078 2023-07-17 04:24:45.477242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_backends/trio.py
+-rw-r--r--   0        0        0     1185 2023-07-17 04:24:45.433242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_exceptions.py
+-rw-r--r--   0        0        0    16343 2023-07-17 04:24:45.433242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_models.py
+-rw-r--r--   0        0        0      187 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_ssl.py
+-rw-r--r--   0        0        0     1141 2023-07-17 04:24:45.481242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/__init__.py
+-rw-r--r--   0        0        0     8209 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/connection.py
+-rw-r--r--   0        0        0    13928 2023-07-17 04:24:45.485242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/connection_pool.py
+-rw-r--r--   0        0        0    11629 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/http11.py
+-rw-r--r--   0        0        0    23343 2023-07-17 04:24:45.489242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/http2.py
+-rw-r--r--   0        0        0    13761 2023-07-17 04:24:45.493242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/http_proxy.py
+-rw-r--r--   0        0        0     4365 2023-07-17 04:24:45.497242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/interfaces.py
+-rw-r--r--   0        0        0    13595 2023-07-17 04:24:45.497242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_sync/socks_proxy.py
+-rw-r--r--   0        0        0     8751 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_synchronization.py
+-rw-r--r--   0        0        0     3954 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_trace.py
+-rw-r--r--   0        0        0     1525 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpcore/py.typed
+-rw-r--r--   0        0        0     7428 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx-0.24.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2363 2023-07-17 04:24:45.473242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx-0.24.1.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2023-07-17 04:24:45.469242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx-0.24.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       37 2023-07-17 04:24:45.469242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx-0.24.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1508 2023-07-17 04:24:45.469242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx-0.24.1.dist-info/licenses/LICENSE.md
+-rw-r--r--   0        0        0     3210 2023-07-17 04:24:45.409242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-17 04:24:45.413242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/__version__.py
+-rw-r--r--   0        0        0    13011 2023-07-17 04:24:45.421243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_api.py
+-rw-r--r--   0        0        0    11773 2023-07-17 04:24:45.425243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_auth.py
+-rw-r--r--   0        0        0    68131 2023-07-17 04:24:45.425243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_client.py
+-rw-r--r--   0        0        0     1602 2023-07-17 04:24:45.425243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_compat.py
+-rw-r--r--   0        0        0    12391 2023-07-17 04:24:45.425243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_config.py
+-rw-r--r--   0        0        0     8092 2023-07-17 04:24:45.433242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_content.py
+-rw-r--r--   0        0        0     9739 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_decoders.py
+-rw-r--r--   0        0        0     7880 2023-07-17 04:24:45.437242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_exceptions.py
+-rw-r--r--   0        0        0    15784 2023-07-17 04:24:45.441242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_main.py
+-rw-r--r--   0        0        0    42696 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_models.py
+-rw-r--r--   0        0        0     8972 2023-07-17 04:24:45.445242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_multipart.py
+-rw-r--r--   0        0        0     5584 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_status_codes.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.457242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/__init__.py
+-rw-r--r--   0        0        0     5317 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/asgi.py
+-rw-r--r--   0        0        0     2510 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/base.py
+-rw-r--r--   0        0        0    12626 2023-07-17 04:24:45.461242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/default.py
+-rw-r--r--   0        0        0     1179 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/mock.py
+-rw-r--r--   0        0        0     4754 2023-07-17 04:24:45.465242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_transports/wsgi.py
+-rw-r--r--   0        0        0     3333 2023-07-17 04:24:45.449242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_types.py
+-rw-r--r--   0        0        0    16669 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_urlparse.py
+-rw-r--r--   0        0        0    21840 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_urls.py
+-rw-r--r--   0        0        0    15397 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.453242 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx/py.typed
+-rw-r--r--   0        0        0      222 2023-07-17 04:24:46.961234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx_utils-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0      486 2023-07-17 04:24:46.965234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx_utils-0.1.0+editable.dist-info/RECORD
+-rw-r--r--   0        0        0       90 2023-07-17 04:24:46.961234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx_utils-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      117 2023-07-17 04:24:46.965234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx_utils-0.1.0+editable.dist-info/direct_url.json
+-rw-r--r--   0        0        0       57 2023-07-17 04:24:46.965234 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/httpx_utils.pth
+-rw-r--r--   0        0        0     1523 2023-07-17 04:24:45.133244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9830 2023-07-17 04:24:45.145244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      925 2023-07-17 04:24:45.149244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2023-07-17 04:24:45.137244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna-3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0      849 2023-07-17 04:24:45.089244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2023-07-17 04:24:45.109244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/codec.py
+-rw-r--r--   0        0        0      321 2023-07-17 04:24:45.109244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/compat.py
+-rw-r--r--   0        0        0    12950 2023-07-17 04:24:45.113244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/core.py
+-rw-r--r--   0        0        0    44375 2023-07-17 04:24:45.117244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2023-07-17 04:24:45.121244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/intranges.py
+-rw-r--r--   0        0        0       21 2023-07-17 04:24:45.121244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/package_data.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.125244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/py.typed
+-rw-r--r--   0        0        0   206539 2023-07-17 04:24:45.133244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/idna/uts46data.py
+-rw-r--r--   0        0        0      185 2023-07-17 04:24:45.217244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    11358 2023-07-17 04:24:45.221244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE.APACHE2
+-rw-r--r--   0        0        0     1046 2023-07-17 04:24:45.229244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/LICENSE.MIT
+-rw-r--r--   0        0        0     3588 2023-07-17 04:24:45.233244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1032 2023-07-17 04:24:45.241243 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:24:45.237244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2023-07-17 04:24:45.237244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio-1.3.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      310 2023-07-17 04:24:45.193244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-17 04:24:45.197244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/_impl.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.205244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/_tests/__init__.py
+-rw-r--r--   0        0        0     2110 2023-07-17 04:24:45.217244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/_tests/test_sniffio.py
+-rw-r--r--   0        0        0       89 2023-07-17 04:24:45.201244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/_version.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:24:45.201244 red_utils-0.1.3/red_utils/httpx_utils/__pypackages__/3.11/lib/sniffio/py.typed
+-rw-r--r--   0        0        0     3285 2023-07-17 04:46:42.906102 red_utils-0.1.3/red_utils/httpx_utils/pdm.lock
+-rw-r--r--   0        0        0      314 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/httpx_utils/pyproject.toml
+-rw-r--r--   0        0        0      326 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/httpx_utils/src/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/httpx_utils/src/constants.py
+-rw-r--r--   0        0        0     2933 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/httpx_utils/src/operations.py
+-rw-r--r--   0        0        0     1159 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/httpx_utils/src/validators.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:13.030465 red_utils-0.1.3/red_utils/loguru_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      215 2023-07-17 04:33:13.038465 red_utils-0.1.3/red_utils/loguru_utils/.pdm-build/loguru_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:13.034465 red_utils-0.1.3/red_utils/loguru_utils/.pdm-build/loguru_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:25:20.557050 red_utils-0.1.3/red_utils/loguru_utils/.pdm-python
+-rw-r--r--   0        0        0       15 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/README.md
+-rw-r--r--   0        0        0      568 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/__init__.py
+-rw-r--r--   0        0        0       14 2023-07-17 04:25:43.300925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/.gitignore
+-rw-r--r--   0        0        0     1056 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    22272 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2018 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru-0.7.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      626 2023-07-17 04:25:43.368925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/__init__.py
+-rw-r--r--   0        0        0    13934 2023-07-17 04:25:43.368925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/__init__.pyi
+-rw-r--r--   0        0        0      597 2023-07-17 04:25:43.368925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_asyncio_loop.py
+-rw-r--r--   0        0        0    16003 2023-07-17 04:25:43.368925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_better_exceptions.py
+-rw-r--r--   0        0        0     1431 2023-07-17 04:25:43.368925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_colorama.py
+-rw-r--r--   0        0        0    14601 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_colorizer.py
+-rw-r--r--   0        0        0      321 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_contextvars.py
+-rw-r--r--   0        0        0     1531 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_ctime_functions.py
+-rw-r--r--   0        0        0     3220 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_datetime.py
+-rw-r--r--   0        0        0     2879 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_defaults.py
+-rw-r--r--   0        0        0     1107 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_error_interceptor.py
+-rw-r--r--   0        0        0    14586 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_file_sink.py
+-rw-r--r--   0        0        0      618 2023-07-17 04:25:43.372925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_filters.py
+-rw-r--r--   0        0        0      458 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_get_frame.py
+-rw-r--r--   0        0        0    11952 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_handler.py
+-rw-r--r--   0        0        0     1307 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_locks_machinery.py
+-rw-r--r--   0        0        0    94321 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_logger.py
+-rw-r--r--   0        0        0     2174 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_recattrs.py
+-rw-r--r--   0        0        0     3160 2023-07-17 04:25:43.376925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_simple_sinks.py
+-rw-r--r--   0        0        0     4707 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/_string_parsers.py
+-rw-r--r--   0        0        0        0 2023-07-17 04:25:43.380925 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru/py.typed
+-rw-r--r--   0        0        0      224 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru_utils-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0      491 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru_utils-0.1.0+editable.dist-info/RECORD
+-rw-r--r--   0        0        0       90 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru_utils-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      118 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru_utils-0.1.0+editable.dist-info/direct_url.json
+-rw-r--r--   0        0        0       58 2023-07-17 04:25:44.876917 red_utils-0.1.3/red_utils/loguru_utils/__pypackages__/3.11/lib/loguru_utils.pth
+-rw-r--r--   0        0        0     1640 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/pdm.lock
+-rw-r--r--   0        0        0      315 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/pyproject.toml
+-rw-r--r--   0        0        0      590 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/src/__init__.py
+-rw-r--r--   0        0        0     3921 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/src/constants.py
+-rw-r--r--   0        0        0     2583 2023-07-17 04:46:42.910102 red_utils-0.1.3/red_utils/loguru_utils/src/operations.py
+-rw-r--r--   0        0        0     1694 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/loguru_utils/src/sinks.py
+-rw-r--r--   0        0        0     1954 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/loguru_utils/src/validators.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:13.490462 red_utils-0.1.3/red_utils/msgpack_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      218 2023-07-17 04:33:13.498462 red_utils-0.1.3/red_utils/msgpack_utils/.pdm-build/msgpack_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:13.494462 red_utils-0.1.3/red_utils/msgpack_utils/.pdm-build/msgpack_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:26:04.872807 red_utils-0.1.3/red_utils/msgpack_utils/.pdm-python
+-rw-r--r--   0        0        0       16 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/README.md
+-rw-r--r--   0        0        0      202 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/__init__.py
+-rw-r--r--   0        0        0       14 2023-07-17 04:26:14.832752 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/.gitignore
+-rw-r--r--   0        0        0      614 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack-1.0.5.dist-info/COPYING
+-rw-r--r--   0        0        0     8751 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack-1.0.5.dist-info/METADATA
+-rw-r--r--   0        0        0      796 2023-07-17 04:26:15.152751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack-1.0.5.dist-info/RECORD
+-rw-r--r--   0        0        0      152 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack-1.0.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack-1.0.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1132 2023-07-17 04:26:15.132751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack/__init__.py
+-rwxr-xr-x   0        0        0  1016256 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack/_cmsgpack.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1081 2023-07-17 04:26:15.148751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2023-07-17 04:26:15.132751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2023-07-17 04:26:15.132751 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack/fallback.py
+-rw-r--r--   0        0        0      227 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack_utils-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0      496 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack_utils-0.1.0+editable.dist-info/RECORD
+-rw-r--r--   0        0        0       90 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack_utils-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      119 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack_utils-0.1.0+editable.dist-info/direct_url.json
+-rw-r--r--   0        0        0       59 2023-07-17 04:26:16.688742 red_utils-0.1.3/red_utils/msgpack_utils/__pypackages__/3.11/lib/msgpack_utils.pth
+-rw-r--r--   0        0        0    10066 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/pdm.lock
+-rw-r--r--   0        0        0      317 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/src/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/src/constants.py
+-rw-r--r--   0        0        0     5459 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/msgpack_utils/src/operations.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/time_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:13.990459 red_utils-0.1.3/red_utils/time_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      182 2023-07-17 04:33:14.002459 red_utils-0.1.3/red_utils/time_utils/.pdm-build/time_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:13.998459 red_utils-0.1.3/red_utils/time_utils/.pdm-build/time_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:26:43.560595 red_utils-0.1.3/red_utils/time_utils/.pdm-python
+-rw-r--r--   0        0        0       13 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/time_utils/README.md
+-rw-r--r--   0        0        0      109 2023-07-17 04:46:42.914102 red_utils-0.1.3/red_utils/time_utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/time_utils/pdm.lock
+-rw-r--r--   0        0        0      291 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/time_utils/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/time_utils/src/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/time_utils/src/constants.py
+-rw-r--r--   0        0        0     1341 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/time_utils/src/operations.py
+-rw-r--r--   0        0        0     3102 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/.gitignore
+-rw-r--r--   0        0        0        2 2023-07-17 04:33:14.110459 red_utils-0.1.3/red_utils/uuid_utils/.pdm-build/.gitignore
+-rw-r--r--   0        0        0      182 2023-07-17 04:33:14.114459 red_utils-0.1.3/red_utils/uuid_utils/.pdm-build/uuid_utils-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2023-07-17 04:33:14.114459 red_utils-0.1.3/red_utils/uuid_utils/.pdm-build/uuid_utils-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       31 2023-07-17 04:29:47.275589 red_utils-0.1.3/red_utils/uuid_utils/.pdm-python
+-rw-r--r--   0        0        0       13 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/README.md
+-rw-r--r--   0        0        0      128 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/pdm.lock
+-rw-r--r--   0        0        0      291 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/src/__init__.py
+-rw-r--r--   0        0        0      162 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/src/classes.py
+-rw-r--r--   0        0        0      108 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/src/constants.py
+-rw-r--r--   0        0        0     8283 2023-07-17 04:46:42.918102 red_utils-0.1.3/red_utils/uuid_utils/src/operations.py
+-rw-r--r--   0        0        0     2768 2023-07-17 04:46:42.922102 red_utils-0.1.3/red_utils/uuid_utils/src/validators.py
+-rw-r--r--   0        0        0     3079 1970-01-01 00:00:00.000000 red_utils-0.1.3/PKG-INFO
```

### Comparing `red_utils-0.1.2/red_utils/diskcache_utils/__init__.py` & `red_utils-0.1.3/red_utils/diskcache_utils/src/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/diskcache_utils/operations.py` & `red_utils-0.1.3/red_utils/diskcache_utils/src/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/diskcache_utils/validators.py` & `red_utils-0.1.3/red_utils/diskcache_utils/src/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from . import valid_key_types, valid_tag_types, valid_val_types
 
 import diskcache
 
 from diskcache import Cache
 
+
 def validate_key(key: valid_key_types = None, none_ok: bool = False) -> Union[str, int]:
     """Validate input diskcache key.
 
     Supported key types:
     - int
     - str
     """
```

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/__init__.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/dependencies.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/dependencies.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/healthcheck.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/healthcheck.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/operations.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/tag_definitions.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/tag_definitions.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/uvicorn_override.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/uvicorn_override.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
 
-from ..loguru_utils.constants import (
-    default_color_fmt,
-    default_fmt,
-    default_log_dir,
-    uvicorn_log_conf,
-)
+from .constants import default_color_fmt
 
 from loguru import logger
 from uvicorn import Config, Server
 
 ## Get LOG_LEVEL variable from env. Default to "INFO"
 LOG_LEVEL = logging.getLevelName(os.environ.get("LOG_LEVEL", "INFO"))
 ## Enable JSON logging if JSON_LOGS env exists and is True
```

### Comparing `red_utils-0.1.2/red_utils/fastapi_utils/validators.py` & `red_utils-0.1.3/red_utils/fastapi_utils/src/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/httpx_utils/operations.py` & `red_utils-0.1.3/red_utils/httpx_utils/src/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/httpx_utils/validators.py` & `red_utils-0.1.3/red_utils/httpx_utils/src/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/loguru_utils/__init__.py` & `red_utils-0.1.3/red_utils/loguru_utils/src/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/loguru_utils/constants.py` & `red_utils-0.1.3/red_utils/loguru_utils/src/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/loguru_utils/operations.py` & `red_utils-0.1.3/red_utils/loguru_utils/src/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/loguru_utils/sinks.py` & `red_utils-0.1.3/red_utils/loguru_utils/src/sinks.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/loguru_utils/validators.py` & `red_utils-0.1.3/red_utils/loguru_utils/src/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.2/red_utils/msgpack_utils/operations.py` & `red_utils-0.1.3/red_utils/msgpack_utils/src/operations.py`

 * *Files identical despite different names*

