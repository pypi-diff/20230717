# Comparing `tmp/flespi-1.2.0.tar.gz` & `tmp/flespi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flespi-1.2.0.tar", last modified: Wed Oct 19 02:53:18 2022, max compression
+gzip compressed data, was "flespi-1.2.1.tar", last modified: Mon Jul 17 20:00:03 2023, max compression
```

## Comparing `flespi-1.2.0.tar` & `flespi-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 mochi     (1000) mochi     (1000)        0 2022-10-19 02:53:18.815028 flespi-1.2.0/
--rw-r--r--   0 mochi     (1000) mochi     (1000)     1064 2022-10-19 00:22:50.000000 flespi-1.2.0/LICENSE
--rw-r--r--   0 mochi     (1000) mochi     (1000)     1496 2022-10-19 02:53:18.815028 flespi-1.2.0/PKG-INFO
--rw-r--r--   0 mochi     (1000) mochi     (1000)      912 2022-10-19 01:08:35.000000 flespi-1.2.0/README.md
-drwxr-xr-x   0 mochi     (1000) mochi     (1000)        0 2022-10-19 02:53:18.815028 flespi-1.2.0/flespi/
--rw-r--r--   0 mochi     (1000) mochi     (1000)       49 2022-10-19 00:56:54.000000 flespi-1.2.0/flespi/__init__.py
--rw-r--r--   0 mochi     (1000) mochi     (1000)     4612 2022-10-19 02:12:16.000000 flespi-1.2.0/flespi/rest.py
-drwxr-xr-x   0 mochi     (1000) mochi     (1000)        0 2022-10-19 02:53:18.815028 flespi-1.2.0/flespi.egg-info/
--rw-r--r--   0 mochi     (1000) mochi     (1000)     1496 2022-10-19 02:53:18.000000 flespi-1.2.0/flespi.egg-info/PKG-INFO
--rw-r--r--   0 mochi     (1000) mochi     (1000)      180 2022-10-19 02:53:18.000000 flespi-1.2.0/flespi.egg-info/SOURCES.txt
--rw-r--r--   0 mochi     (1000) mochi     (1000)        1 2022-10-19 02:53:18.000000 flespi-1.2.0/flespi.egg-info/dependency_links.txt
--rw-r--r--   0 mochi     (1000) mochi     (1000)        7 2022-10-19 02:53:18.000000 flespi-1.2.0/flespi.egg-info/top_level.txt
--rw-r--r--   0 mochi     (1000) mochi     (1000)       38 2022-10-19 02:53:18.815028 flespi-1.2.0/setup.cfg
--rw-r--r--   0 mochi     (1000) mochi     (1000)      499 2022-10-19 02:52:02.000000 flespi-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:00:03.778771 flespi-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     6148 2023-07-17 19:59:47.000000 flespi-1.2.1/.DS_Store
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-17 19:59:47.000000 flespi-1.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-17 19:59:47.000000 flespi-1.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13992 2023-07-17 19:59:47.000000 flespi-1.2.1/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:00:03.775771 flespi-1.2.1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-17 19:59:47.000000 flespi-1.2.1/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 19:59:47.000000 flespi-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-17 20:00:03.777771 flespi-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-07-17 19:59:47.000000 flespi-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:00:03.776771 flespi-1.2.1/flespi/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-17 19:59:47.000000 flespi-1.2.1/flespi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4372 2023-07-17 19:59:47.000000 flespi-1.2.1/flespi/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 20:00:03.777771 flespi-1.2.1/flespi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-17 20:00:03.000000 flespi-1.2.1/flespi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-17 20:00:03.000000 flespi-1.2.1/flespi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 20:00:03.000000 flespi-1.2.1/flespi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 20:00:03.000000 flespi-1.2.1/flespi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 20:00:03.000000 flespi-1.2.1/flespi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-07-17 19:59:47.000000 flespi-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 20:00:03.778771 flespi-1.2.1/setup.cfg
```

### Comparing `flespi-1.2.0/LICENSE` & `flespi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flespi-1.2.0/README.md` & `flespi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `flespi-1.2.0/flespi/rest.py` & `flespi-1.2.1/flespi/rest.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,14 @@
       If True, prints request and parameters to console
       Deprecation warning: Will be removed in future versions, now the logging will work
                            with the standard Python logging module, with DEBUG level
     """
     self._token = token
     self._url = 'https://flespi.io'
     self._log = logging.getLogger('flespi.rest.FlespiClient')
-    stream_logger = logging.StreamHandler()
-    formatter = logging.Formatter('[%(levelname)s] %(name)s: %(message)s')
-    stream_logger.setFormatter(formatter)
-    self._log.addHandler(stream_logger)
-    self._log.setLevel(logging.DEBUG)
-
     self._log.debug('FlespiClient initialized with token %s', token)
 
   @property
   def _headers(self):
     """ Headers """
     return {'Accept': 'application/json', 'Authorization': f'FlespiToken {self._token}'}
```

