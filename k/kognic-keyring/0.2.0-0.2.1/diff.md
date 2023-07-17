# Comparing `tmp/kognic-keyring-0.2.0.tar.gz` & `tmp/kognic-keyring-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-keyring-0.2.0.tar", last modified: Mon Jul 17 07:16:25 2023, max compression
+gzip compressed data, was "kognic-keyring-0.2.1.tar", last modified: Mon Jul 17 07:33:52 2023, max compression
```

## Comparing `kognic-keyring-0.2.0.tar` & `kognic-keyring-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:16:25.787368 kognic-keyring-0.2.0/
--rw-r--r--   0 Merca      (501) staff       (20)      140 2023-07-17 07:16:25.787028 kognic-keyring-0.2.0/PKG-INFO
--rw-r--r--   0 Merca      (501) staff       (20)      442 2023-07-17 07:12:49.000000 kognic-keyring-0.2.0/README.md
--rw-r--r--   0 Merca      (501) staff       (20)      420 2023-07-17 07:13:14.000000 kognic-keyring-0.2.0/pyproject.toml
--rw-r--r--   0 Merca      (501) staff       (20)       38 2023-07-17 07:16:25.787471 kognic-keyring-0.2.0/setup.cfg
-drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:16:25.782058 kognic-keyring-0.2.0/src/
-drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:16:25.781862 kognic-keyring-0.2.0/src/keyrings/
-drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:16:25.783528 kognic-keyring-0.2.0/src/keyrings/kognic/
--rw-r--r--   0 Merca      (501) staff       (20)      652 2023-07-17 07:12:03.000000 kognic-keyring-0.2.0/src/keyrings/kognic/proxy_auth.py
-drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:16:25.786516 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/
--rw-r--r--   0 Merca      (501) staff       (20)      140 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/PKG-INFO
--rw-r--r--   0 Merca      (501) staff       (20)      312 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/SOURCES.txt
--rw-r--r--   0 Merca      (501) staff       (20)        1 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/dependency_links.txt
--rw-r--r--   0 Merca      (501) staff       (20)       64 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/entry_points.txt
--rw-r--r--   0 Merca      (501) staff       (20)       48 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/requires.txt
--rw-r--r--   0 Merca      (501) staff       (20)        9 2023-07-17 07:16:25.000000 kognic-keyring-0.2.0/src/kognic_keyring.egg-info/top_level.txt
+drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:33:52.042720 kognic-keyring-0.2.1/
+-rw-r--r--   0 Merca      (501) staff       (20)      140 2023-07-17 07:33:52.042514 kognic-keyring-0.2.1/PKG-INFO
+-rw-r--r--   0 Merca      (501) staff       (20)      442 2023-07-17 07:12:49.000000 kognic-keyring-0.2.1/README.md
+-rw-r--r--   0 Merca      (501) staff       (20)      420 2023-07-17 07:32:52.000000 kognic-keyring-0.2.1/pyproject.toml
+-rw-r--r--   0 Merca      (501) staff       (20)       38 2023-07-17 07:33:52.042783 kognic-keyring-0.2.1/setup.cfg
+drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:33:52.038191 kognic-keyring-0.2.1/src/
+drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:33:52.037957 kognic-keyring-0.2.1/src/keyrings/
+drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:33:52.039583 kognic-keyring-0.2.1/src/keyrings/kognic/
+-rw-r--r--   0 Merca      (501) staff       (20)      714 2023-07-17 07:31:00.000000 kognic-keyring-0.2.1/src/keyrings/kognic/proxy_auth.py
+drwxr-xr-x   0 Merca      (501) staff       (20)        0 2023-07-17 07:33:52.042237 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/
+-rw-r--r--   0 Merca      (501) staff       (20)      140 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/PKG-INFO
+-rw-r--r--   0 Merca      (501) staff       (20)      312 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/SOURCES.txt
+-rw-r--r--   0 Merca      (501) staff       (20)        1 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/dependency_links.txt
+-rw-r--r--   0 Merca      (501) staff       (20)       64 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/entry_points.txt
+-rw-r--r--   0 Merca      (501) staff       (20)       48 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/requires.txt
+-rw-r--r--   0 Merca      (501) staff       (20)        9 2023-07-17 07:33:52.000000 kognic-keyring-0.2.1/src/kognic_keyring.egg-info/top_level.txt
```

### Comparing `kognic-keyring-0.2.0/src/keyrings/kognic/proxy_auth.py` & `kognic-keyring-0.2.1/src/keyrings/kognic/proxy_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,11 +10,13 @@
     Higher priority than typical recommended backends - but one less priority than Chainer Backend.
     """
 
     def get_password(self, service, username):
         url = urlparse(service)
         if url.hostname is None: 
             return
-        if not url.hostname.endswith("pip-vproxy.annotell.com") or not (url.hostname.endswith("kognic.io") and "pypi" in url.hostname):
+        is_annotell = url.hostname.endswith("pip-vproxy.annotell.com")
+        is_kognic = (url.hostname.endswith("kognic.io") and "pypi" in url.hostname)
+        if not (is_annotell or is_kognic):
             return
 
         return super().get_password("https://dummy.pkg.dev", username)
```

