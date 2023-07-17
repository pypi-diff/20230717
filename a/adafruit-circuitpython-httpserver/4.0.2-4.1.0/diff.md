# Comparing `tmp/adafruit-circuitpython-httpserver-4.0.2.tar.gz` & `tmp/adafruit-circuitpython-httpserver-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-4.0.2.tar", last modified: Tue May 30 00:58:11 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-4.1.0.tar", last modified: Mon Jul 17 15:39:17 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-4.0.2.tar` & `adafruit-circuitpython-httpserver-4.1.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.038245 adafruit-circuitpython-httpserver-4.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 00:58:11.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.042245 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.046245 adafruit-circuitpython-httpserver-4.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.046245 adafruit-circuitpython-httpserver-4.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:58:11.050245 adafruit-circuitpython-httpserver-4.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/examples/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_handler_serves_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_multiple_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_start_and_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_static_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/examples/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-30 00:58:02.000000 adafruit-circuitpython-httpserver-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-30 00:57:46.000000 adafruit-circuitpython-httpserver-4.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:58:11.054245 adafruit-circuitpython-httpserver-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.877951 adafruit-circuitpython-httpserver-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.877951 adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.885950 adafruit-circuitpython-httpserver-4.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.885950 adafruit-circuitpython-httpserver-4.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_ethernet_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_form_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/.gitignore` & `adafruit-circuitpython-httpserver-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/.pylintrc` & `adafruit-circuitpython-httpserver-4.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-4.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/LICENSE` & `adafruit-circuitpython-httpserver-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-4.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-4.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-4.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/PKG-INFO` & `adafruit-circuitpython-httpserver-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.0.2
+Version: 4.1.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,15 +41,15 @@
 
 HTTP Server for CircuitPython.
 
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
-- Gives access to request headers, query parameters, body and client's address, the one from which the request came.
+- Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/README.rst` & `adafruit-circuitpython-httpserver-4.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 HTTP Server for CircuitPython.
 
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
-- Gives access to request headers, query parameters, body and client's address, the one from which the request came.
+- Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.0.2
+Version: 4.1.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,15 +41,15 @@
 
 HTTP Server for CircuitPython.
 
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
-- Gives access to request headers, query parameters, body and client's address, the one from which the request came.
+- Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/home.html
 examples/httpserver_authentication_handlers.py
 examples/httpserver_authentication_server.py
 examples/httpserver_chunked.py
 examples/httpserver_cpu_information.py
+examples/httpserver_ethernet_simpletest.py
+examples/httpserver_form_data.py
 examples/httpserver_handler_serves_file.py
 examples/httpserver_mdns.py
 examples/httpserver_methods.py
 examples/httpserver_multiple_servers.py
 examples/httpserver_neopixel.py
 examples/httpserver_redirects.py
 examples/httpserver_simpletest_auto.py
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "4.0.2"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
 
 
 from .authentication import (
     Basic,
     Bearer,
     check_authentication,
@@ -47,23 +47,29 @@
     PATCH,
     HEAD,
     OPTIONS,
     TRACE,
     CONNECT,
 )
 from .mime_types import MIMETypes
-from .request import Request
+from .request import QueryParams, FormData, Request
 from .response import (
     Response,
     FileResponse,
     ChunkedResponse,
     JSONResponse,
     Redirect,
 )
-from .server import Server
+from .server import (
+    Server,
+    NO_REQUEST,
+    CONNECTION_TIMED_OUT,
+    REQUEST_HANDLED_NO_RESPONSE,
+    REQUEST_HANDLED_RESPONSE_SENT,
+)
 from .status import (
     Status,
     OK_200,
     CREATED_201,
     ACCEPTED_202,
     NO_CONTENT_204,
     PARTIAL_CONTENT_206,
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/authentication.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     def __str__(self) -> str:
         return f"Bearer {self._value}"
 
 
 def check_authentication(request: Request, auths: List[Union[Basic, Bearer]]) -> bool:
     """
     Returns ``True`` if request is authorized by any of the authentications, ``False`` otherwise.
+
+    Example::
+
+        check_authentication(request, [Basic("username", "password")])
     """
 
     auth_header = request.headers.get("Authorization")
 
     if auth_header is None:
         return False
 
@@ -52,13 +56,17 @@
 
 
 def require_authentication(request: Request, auths: List[Union[Basic, Bearer]]) -> None:
     """
     Checks if the request is authorized and raises ``AuthenticationError`` if not.
 
     If the error is not caught, the server will return ``401 Unauthorized``.
+
+    Example::
+
+        require_authentication(request, [Basic("username", "password")])
     """
 
     if not check_authentication(request, auths):
         raise AuthenticationError(
             "Request is not authenticated by any of the provided authentications"
         )
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/exceptions.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/mime_types.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/mime_types.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/response.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,16 @@
         self._send_bytes(self._request.connection, encoded_chunk)
         self._send_bytes(self._request.connection, b"\r\n")
 
     def _send(self) -> None:
         self._send_headers()
 
         for chunk in self._body():
-            self._send_chunk(chunk)
+            if 0 < len(chunk):  # Don't send empty chunks
+                self._send_chunk(chunk)
 
         # Empty chunk to indicate end of response
         self._send_chunk()
 
 
 class JSONResponse(Response):  # pylint: disable=too-few-public-methods
     """
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/route.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/route.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 `adafruit_httpserver.server`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
 
 try:
-    from typing import Callable, Protocol, Union, List, Set, Tuple
+    from typing import Callable, Protocol, Union, List, Set, Tuple, Dict
     from socket import socket
     from socketpool import SocketPool
 except ImportError:
     pass
 
 from errno import EAGAIN, ECONNRESET, ETIMEDOUT
 from traceback import print_exception
@@ -21,29 +21,39 @@
 from .exceptions import (
     ServerStoppedError,
     AuthenticationError,
     FileNotExistsError,
     InvalidPathError,
     ServingFilesDisabledError,
 )
+from .headers import Headers
 from .methods import GET, HEAD
 from .request import Request
 from .response import Response, FileResponse
 from .route import _Routes, _Route
 from .status import BAD_REQUEST_400, UNAUTHORIZED_401, FORBIDDEN_403, NOT_FOUND_404
 
 
-class Server:
+NO_REQUEST = "no_request"
+CONNECTION_TIMED_OUT = "connection_timed_out"
+REQUEST_HANDLED_NO_RESPONSE = "request_handled_no_response"
+REQUEST_HANDLED_RESPONSE_SENT = "request_handled_response_sent"
+
+
+class Server:  # pylint: disable=too-many-instance-attributes
     """A basic socket-based HTTP server."""
 
-    host: str = None
-    """Host name or IP address the server is listening on."""
+    host: str
+    """Host name or IP address the server is listening on. ``None`` if server is stopped."""
+
+    port: int
+    """Port the server is listening on. ``None`` if server is stopped."""
 
-    port: int = None
-    """Port the server is listening on."""
+    root_path: str
+    """Root directory to serve files from. ``None`` if serving files is disabled."""
 
     def __init__(
         self, socket_source: Protocol, root_path: str = None, *, debug: bool = False
     ) -> None:
         """Create a server, and get it ready to run.
 
         :param socket: An object that is a source of sockets. This could be a `socketpool`
@@ -53,18 +63,20 @@
         """
         self._auths = []
         self._buffer = bytearray(1024)
         self._timeout = 1
         self._routes = _Routes()
         self._socket_source = socket_source
         self._sock = None
+        self.headers = Headers()
+        self.host, self.port = None, None
         self.root_path = root_path
         if root_path in ["", "/"] and debug:
             _debug_warning_exposed_files(root_path)
-        self.stopped = False
+        self.stopped = True
 
         self.debug = debug
 
     def route(
         self,
         path: str,
         methods: Union[str, Set[str]] = GET,
@@ -302,75 +314,110 @@
         except (FileNotExistsError, ServingFilesDisabledError) as error:
             return Response(
                 request,
                 str(error) if self.debug else "File not found",
                 status=NOT_FOUND_404,
             )
 
-    def poll(self):
+    def _set_default_server_headers(self, response: Response) -> None:
+        for name, value in self.headers.items():
+            response._headers.setdefault(  # pylint: disable=protected-access
+                name, value
+            )
+
+    def poll(self) -> str:
         """
         Call this method inside your main loop to get the server to check for new incoming client
         requests. When a request comes in, it will be handled by the handler function.
+
+        Returns str representing the result of the poll
+        e.g. ``NO_REQUEST`` or ``REQUEST_HANDLED_RESPONSE_SENT``.
         """
         if self.stopped:
             raise ServerStoppedError
 
         try:
             conn, client_address = self._sock.accept()
             with conn:
                 conn.settimeout(self._timeout)
 
                 # Receive the whole request
                 if (request := self._receive_request(conn, client_address)) is None:
-                    return
+                    return CONNECTION_TIMED_OUT
 
                 # Find a handler for the route
                 handler = self._routes.find_handler(
                     _Route(request.path, request.method)
                 )
 
                 # Handle the request
                 response = self._handle_request(request, handler)
 
                 if response is None:
-                    return
+                    return REQUEST_HANDLED_NO_RESPONSE
+
+                self._set_default_server_headers(response)
 
                 # Send the response
                 response._send()  # pylint: disable=protected-access
 
                 if self.debug:
                     _debug_response_sent(response)
 
+                return REQUEST_HANDLED_RESPONSE_SENT
+
         except Exception as error:  # pylint: disable=broad-except
             if isinstance(error, OSError):
                 # There is no data available right now, try again later.
                 if error.errno == EAGAIN:
-                    return
+                    return NO_REQUEST
                 # Connection reset by peer, try again later.
                 if error.errno == ECONNRESET:
-                    return
+                    return NO_REQUEST
 
             if self.debug:
                 _debug_exception_in_handler(error)
 
             raise error  # Raise the exception again to be handled by the user.
 
     def require_authentication(self, auths: List[Union[Basic, Bearer]]) -> None:
         """
         Requires authentication for all routes and files in ``root_path``.
         Any non-authenticated request will be rejected with a 401 status code.
 
         Example::
 
             server = Server(pool, "/static")
-            server.require_authentication([Basic("user", "pass")])
+            server.require_authentication([Basic("username", "password")])
         """
         self._auths = auths
 
     @property
+    def headers(self) -> Headers:
+        """
+        Headers to be sent with every response, without the need to specify them in each handler.
+
+        If a header is specified in both the handler and the server, the handler's header will be
+        used.
+
+        Example::
+
+            server = Server(pool, "/static")
+            server.headers = {
+                "X-Server": "Adafruit CircuitPython HTTP Server",
+                "Access-Control-Allow-Origin": "*",
+            }
+        """
+        return self._headers
+
+    @headers.setter
+    def headers(self, value: Union[Headers, Dict[str, str]]) -> None:
+        self._headers = value.copy() if isinstance(value, Headers) else Headers(value)
+
+    @property
     def request_buffer_size(self) -> int:
         """
         The maximum size of the incoming request buffer. If the default size isn't
         adequate to handle your incoming data you can set this after creating the
         server instance.
 
         Default size is 1024 bytes.
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/docs/api.rst` & `adafruit-circuitpython-httpserver-4.1.0/docs/api.rst`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     :members:
 
 .. automodule:: adafruit_httpserver.server
     :members:
 
 .. automodule:: adafruit_httpserver.request
     :members:
+    :inherited-members:
 
 .. automodule:: adafruit_httpserver.response
     :members:
 
 .. automodule:: adafruit_httpserver.headers
     :members:
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/docs/conf.py` & `adafruit-circuitpython-httpserver-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/docs/examples.rst` & `adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst`

 * *Files 12% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 If you want your code to do more than just serve web pages,
 use the ``.start()``/``.poll()`` methods as shown in this example.
 
 Between calling ``.poll()`` you can do something useful,
 for example read a sensor and capture an average or
 a running total of the last 10 samples.
 
+``.poll()`` return value can be used to check if there was a request and if it was handled.
+
 .. literalinclude:: ../examples/httpserver_start_and_poll.py
     :caption: examples/httpserver_start_and_poll.py
     :emphasize-lines: 24,33
     :linenos:
 
 Server with MDNS
 ----------------
@@ -93,17 +95,20 @@
 
 Get CPU information
 -------------------
 
 You can return data from sensors or any computed value as JSON.
 That makes it easy to use the data in other applications.
 
+If you want to use the data in a web browser, it might be necessary to enable CORS.
+More info: https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
+
 .. literalinclude:: ../examples/httpserver_cpu_information.py
     :caption: examples/httpserver_cpu_information.py
-    :emphasize-lines: 9,27
+    :emphasize-lines: 9,15-18,33
     :linenos:
 
 Handling different methods
 ---------------------------------------
 
 On every ``server.route()`` call you can specify which HTTP methods are allowed.
 By default, only ``GET`` method is allowed.
@@ -139,14 +144,42 @@
 Tested on ESP32-S2 Feather.
 
 .. literalinclude:: ../examples/httpserver_neopixel.py
     :caption: examples/httpserver_neopixel.py
     :emphasize-lines: 25-27,39,51,60,66
     :linenos:
 
+Form data parsing
+---------------------
+
+Another way to pass data to the handler function is to use form data.
+Remember that it is only possible to use it with ``POST`` method.
+`More about POST method. <https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST>`_
+
+It is important to use correct ``enctype``, depending on the type of data you want to send.
+
+- ``application/x-www-form-urlencoded`` - For sending simple text data without any special characters including spaces.
+    If you use it, values will be automatically parsed as strings, but special characters will be URL encoded
+    e.g. ``"Hello World! ^-$%"`` will be saved as ``"Hello+World%21+%5E-%24%25"``
+- ``multipart/form-data`` - For sending text and binary files and/or text data with special characters
+    When used, values will **not** be automatically parsed as strings, they will stay as bytes instead.
+    e.g. ``"Hello World! ^-$%"`` will be saved as ``b'Hello World! ^-$%'``, which can be decoded using ``.decode()`` method.
+- ``text/plain`` - For sending text data with special characters.
+    If used, values will be automatically parsed as strings, including special characters, emojis etc.
+    e.g. ``"Hello World! ^-$%"`` will be saved as ``"Hello World! ^-$%"``, this is the **recommended** option.
+
+If you pass multiple values with the same name, they will be saved as a list, that can be accessed using ``request.form_data.get_list()``.
+Even if there is only one value, it will still get a list, and if there multiple values, but you use ``request.form_data.get()`` it will
+return only the first one.
+
+.. literalinclude:: ../examples/httpserver_form_data.py
+    :caption: examples/httpserver_form_data.py
+    :emphasize-lines: 32,47,50
+    :linenos:
+
 Chunked response
 ----------------
 
 Library supports chunked responses. This is useful for streaming large amounts of data.
 In order to use it, you need pass a generator that yields chunks of data to a ``ChunkedResponse``
 constructor.
 
@@ -173,24 +206,26 @@
 If you specify multiple routes for single handler function and they have different number of URL parameters,
 make sure to add default values for all the ones that might not be passed.
 In the example below the second route has only one URL parameter, so the ``action`` parameter has a default value.
 
 Keep in mind that URL parameters are always passed as strings, so you need to convert them to the desired type.
 Also note that the names of the function parameters **have to match** with the ones used in route, but they **do not have to** be in the same order.
 
+Alternatively you can use e.g. ``**params`` to get all the parameters as a dictionary and access them using ``params['parameter_name']``.
+
 It is also possible to specify a wildcard route:
 
 - ``...`` - matches one path segment, e.g ``/api/...`` will match ``/api/123``, but **not** ``/api/123/456``
 - ``....`` - matches multiple path segments, e.g ``/api/....`` will match ``/api/123`` and ``/api/123/456``
 
 In both cases, wildcards will not match empty path segment, so ``/api/.../users`` will match ``/api/v1/users``, but not ``/api//users`` or ``/api/users``.
 
 .. literalinclude:: ../examples/httpserver_url_parameters.py
     :caption: examples/httpserver_url_parameters.py
-    :emphasize-lines: 30-34,53-54
+    :emphasize-lines: 30-34,53-54,65-66
     :linenos:
 
 Authentication
 --------------
 
 In order to increase security of your server, you can use ``Basic`` and ``Bearer`` authentication.
 Remember that it is **not a replacement for HTTPS**, traffic is still sent **in plain text**, but it can be used to protect your server from unauthorized access.
@@ -229,20 +264,23 @@
 
 Although it is not the primary use case, it is possible to run multiple servers at the same time.
 In order to do that, you need to create multiple ``Server`` instances and call ``.start()`` and ``.poll()`` on each of them.
 Using ``.serve_forever()`` for this is not possible because of it's blocking behaviour.
 
 Each server **must have a different port number**.
 
+In order to distinguish between responses from different servers a 'X-Server' header is added to each response.
+**This is an optional step**, both servers will work without it.
+
 In combination with separate authentication and diffrent ``root_path`` this allows creating moderately complex setups.
 You can share same handler functions between servers or use different ones for each server.
 
 .. literalinclude:: ../examples/httpserver_multiple_servers.py
     :caption: examples/httpserver_multiple_servers.py
-    :emphasize-lines: 13-14,17,25,33-34,45-46,51-52
+    :emphasize-lines: 13-14,16-17,20,28,36-37,48-49,54-55
     :linenos:
 
 Debug mode
 ----------------
 
 It is highly recommended to **disable debug mode in production**.
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/docs/index.rst` & `adafruit-circuitpython-httpserver-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_handlers.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_handlers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_authentication_server.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_cpu_information.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 
 import microcontroller
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, JSONResponse
 
+
 pool = socketpool.SocketPool(wifi.radio)
 server = Server(pool, debug=True)
 
+# (Optional) Allow cross-origin requests.
+server.headers = {
+    "Access-Control-Allow-Origin": "*",
+}
+
 
 @server.route("/cpu-information", append_slash=True)
 def cpu_information_handler(request: Request):
     """
     Return the current CPU temperature, frequency, and voltage as JSON.
     """
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_methods.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_multiple_servers.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_multiple_servers.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 from adafruit_httpserver import Server, Request, Response
 
 
 pool = socketpool.SocketPool(wifi.radio)
 
 bedroom_server = Server(pool, "/bedroom", debug=True)
+bedroom_server.headers["X-Server"] = "Bedroom"
+
 office_server = Server(pool, "/office", debug=True)
+office_server.headers["X-Server"] = "Office"
 
 
 @bedroom_server.route("/bedroom")
 def bedroom(request: Request):
     """
     This route is registered only on ``bedroom_server``.
     """
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_neopixel.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,38 @@
     b = request.query_params.get("b") or 0
 
     pixel.fill((int(r), int(g), int(b)))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
-@server.route("/change-neopixel-color", POST)
+@server.route("/change-neopixel-color/body", POST)
 def change_neopixel_color_handler_post_body(request: Request):
     """Changes the color of the built-in NeoPixel using POST body."""
 
     data = request.body  # e.g b"255,0,0"
     r, g, b = data.decode().split(",")  # ["255", "0", "0"]
 
     pixel.fill((int(r), int(g), int(b)))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
+@server.route("/change-neopixel-color/form-data", POST)
+def change_neopixel_color_handler_post_form_data(request: Request):
+    """Changes the color of the built-in NeoPixel using POST form data."""
+
+    data = request.form_data  # e.g. r=255&g=0&b=0 or r=255\r\nb=0\r\ng=0
+    r, g, b = data.get("r", 0), data.get("g", 0), data.get("b", 0)
+
+    pixel.fill((int(r), int(g), int(b)))
+
+    return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
+
+
 @server.route("/change-neopixel-color/json", POST)
 def change_neopixel_color_handler_post_json(request: Request):
     """Changes the color of the built-in NeoPixel using JSON POST body."""
 
     data = request.json()  # e.g {"r": 255, "g": 0, "b": 0}
     r, g, b = data.get("r", 0), data.get("g", 0), data.get("b", 0)
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_redirects.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_redirects.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_auto.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_auto.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_simpletest_manual.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_manual.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_start_and_poll.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_start_and_poll.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
-from adafruit_httpserver import Server, Request, FileResponse
+from adafruit_httpserver import (
+    Server,
+    REQUEST_HANDLED_RESPONSE_SENT,
+    Request,
+    FileResponse,
+)
 
 
 pool = socketpool.SocketPool(wifi.radio)
 server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
@@ -26,13 +31,17 @@
 while True:
     try:
         # Do something useful in this section,
         # for example read a sensor and capture an average,
         # or a running total of the last 10 samples
 
         # Process any waiting requests
-        server.poll()
+        pool_result = server.poll()
+
+        if pool_result == REQUEST_HANDLED_RESPONSE_SENT:
+            # Do something only after handling a request
+            pass
 
         # If you want you can stop the server by calling server.stop() anywhere in your code
     except OSError as error:
         print(error)
         continue
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_static_files_serving.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_static_files_serving.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.0.2/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_url_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,14 +46,26 @@
         return Response(request, f"Unknown action ({action})")
 
     return Response(
         request, f"Action ({action}) performed on device with ID: {device_id}"
     )
 
 
+@server.route("/device/<device_id>/status/<date>")
+def device_status_on_date(request: Request, **params: dict):
+    """
+    Return the status of a specified device between two dates.
+    """
+
+    device_id = params.get("device_id")
+    date = params.get("date")
+
+    return Response(request, f"Status of {device_id} on {date}: ...")
+
+
 @server.route("/device/.../status", append_slash=True)
 @server.route("/device/....", append_slash=True)
 def device_status(request: Request):
     """
     Returns the status of all devices no matter what their ID is.
     Unknown commands also return the status of all devices.
     """
```

### Comparing `adafruit-circuitpython-httpserver-4.0.2/pyproject.toml` & `adafruit-circuitpython-httpserver-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "4.0.2"
+version = "4.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

