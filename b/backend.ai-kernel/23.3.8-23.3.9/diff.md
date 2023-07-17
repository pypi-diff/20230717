# Comparing `tmp/backend.ai-kernel-23.3.8.tar.gz` & `tmp/backend.ai-kernel-23.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-23.3.8.tar", last modified: Thu Jul  6 04:38:09 2023, max compression
+gzip compressed data, was "backend.ai-kernel-23.3.9.tar", last modified: Mon Jul 17 14:36:06 2023, max compression
```

## Comparing `backend.ai-kernel-23.3.8.tar` & `backend.ai-kernel-23.3.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/app/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42169 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/c/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/git/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/golang/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/golang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/java/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/lua/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/lua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/octave/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/octave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/php/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/php/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/python/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/r/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/rust/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/service_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/inproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.440713 backend.ai-kernel-23.3.9/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.440713 backend.ai-kernel-23.3.9/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42169 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/golang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/golang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/haskell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/haskell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/lua/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/lua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/nodejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/nodejs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/octave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/octave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/php/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/php/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/r_server_ms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/r_server_ms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.444713 backend.ai-kernel-23.3.9/ai/backend/kernel/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/ai/backend/kernel/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/service_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/aws_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/aws_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/aws_polly/inproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/h2o/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/h2o/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:36:06.448713 backend.ai-kernel-23.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-17 14:36:06.000000 backend.ai-kernel-23.3.9/setup.py
```

### Comparing `backend.ai-kernel-23.3.8/PKG-INFO` & `backend.ai-kernel-23.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/__main__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/app/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/app/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/base.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/c/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/c/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/compat.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/git/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/git/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/golang/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/haskell/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/intrinsic.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/intrinsic.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/java/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/java/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/julia/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/jupyter_client.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/logging.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/lua/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/lua/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/nodejs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/octave/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/php/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/php/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/canvas.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/canvas.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/color.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/color.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/turtle.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/drawing/turtle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/sitecustomize.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/python/types.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/python/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/r/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/r/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/r_server_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/rust/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/service.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/service_actions.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/service_actions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/terminal.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/terminal.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/utils.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/aws_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/inproc.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/aws_polly/inproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/__init__.py` & `backend.ai-kernel-23.3.9/ai/backend/kernel/vendor/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/PKG-INFO` & `backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/SOURCES.txt` & `backend.ai-kernel-23.3.9/backend.ai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/backend_shim.py` & `backend.ai-kernel-23.3.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.8/setup.py` & `backend.ai-kernel-23.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,11 +72,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.8
+    'version': """23.03.9
 """,
     'zip_safe': False,
 })
```

