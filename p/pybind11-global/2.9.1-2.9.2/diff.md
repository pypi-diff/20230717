# Comparing `tmp/pybind11_global-2.9.1.tar.gz` & `tmp/pybind11_global-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybind11_global-2.9.1.tar", last modified: Thu Feb  3 00:30:21 2022, max compression
+gzip compressed data, was "pybind11_global-2.9.2.tar", last modified: Thu Mar 31 03:18:18 2022, max compression
```

## Comparing `pybind11_global-2.9.1.tar` & `pybind11_global-2.9.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7656 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.810556 pybind11_global-2.9.1/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.806556 pybind11_global-2.9.1/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.810556 pybind11_global-2.9.1/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)    23583 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6131 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    60413 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)     8678 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (121)    27932 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (121)    48813 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (121)    16970 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (121)    23608 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (121)    42206 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (121)    29875 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (121)    11660 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (121)     8882 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (121)    72116 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (121)   119136 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (121)    76321 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (121)    26460 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17483 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/setup_helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.806556 pybind11_global-2.9.1/pybind11/share/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.806556 pybind11_global-2.9.1/pybind11/share/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    14579 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7913 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Config.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Targets.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-02-03 00:29:27.000000 pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/pybind11_global.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11_global.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11_global.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11_global.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:29:43.000000 pybind11_global-2.9.1/pybind11_global.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:30:21.000000 pybind11_global-2.9.1/pybind11_global.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-02-03 00:30:21.814556 pybind11_global-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7656 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.637622 pybind11_global-2.9.2/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.637622 pybind11_global-2.9.2/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.641623 pybind11_global-2.9.2/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)    23920 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    64793 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8907 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.641623 pybind11_global-2.9.2/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)    28526 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (121)    51655 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    17971 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (121)    24196 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (121)    44414 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (121)    31441 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12175 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4755 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6848 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8851 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    78036 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9781 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (121)   125927 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (121)    80901 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.641623 pybind11_global-2.9.2/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (121)    14438 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    26992 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    17483 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/setup_helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.637622 pybind11_global-2.9.2/pybind11/share/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.637622 pybind11_global-2.9.2/pybind11/share/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)    10378 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    14579 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7914 2022-03-31 03:18:17.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Config.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-03-31 03:18:17.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-03-31 03:18:17.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Targets.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-03-31 03:16:54.000000 pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/pybind11_global.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-03-31 03:18:18.000000 pybind11_global-2.9.2/pybind11_global.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-03-31 03:18:18.000000 pybind11_global-2.9.2/pybind11_global.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 03:18:18.000000 pybind11_global-2.9.2/pybind11_global.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 03:17:18.000000 pybind11_global-2.9.2/pybind11_global.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 03:18:18.000000 pybind11_global-2.9.2/pybind11_global.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-03-31 03:18:18.645623 pybind11_global-2.9.2/setup.py
```

### Comparing `pybind11_global-2.9.1/LICENSE` & `pybind11_global-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/PKG-INFO` & `pybind11_global-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybind11_global
-Version: 2.9.1
+Version: 2.9.2
 Summary: Seamless operability between C++11 and Python
 Home-page: https://github.com/pybind/pybind11
 Author: Wenzel Jakob
 Author-email: wenzel.jakob@epfl.ch
 License: BSD
 Project-URL: Documentation, https://pybind11.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/pybind/pybind11/issues
```

### Comparing `pybind11_global-2.9.1/README.rst` & `pybind11_global-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/__main__.py` & `pybind11_global-2.9.2/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/commands.py` & `pybind11_global-2.9.2/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/attr.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/attr.h`

 * *Files 3% similar despite different names*

```diff
@@ -16,73 +16,81 @@
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 /// \addtogroup annotations
 /// @{
 
 /// Annotation for methods
-struct is_method { handle class_;
+struct is_method {
+    handle class_;
     explicit is_method(const handle &c) : class_(c) {}
 };
 
 /// Annotation for operators
-struct is_operator { };
+struct is_operator {};
 
 /// Annotation for classes that cannot be subclassed
-struct is_final { };
+struct is_final {};
 
 /// Annotation for parent scope
-struct scope { handle value;
+struct scope {
+    handle value;
     explicit scope(const handle &s) : value(s) {}
 };
 
 /// Annotation for documentation
-struct doc { const char *value;
+struct doc {
+    const char *value;
     explicit doc(const char *value) : value(value) {}
 };
 
 /// Annotation for function names
-struct name { const char *value;
+struct name {
+    const char *value;
     explicit name(const char *value) : value(value) {}
 };
 
 /// Annotation indicating that a function is an overload associated with a given "sibling"
-struct sibling { handle value;
+struct sibling {
+    handle value;
     explicit sibling(const handle &value) : value(value.ptr()) {}
 };
 
 /// Annotation indicating that a class derives from another given type
-template <typename T> struct base {
+template <typename T>
+struct base {
 
-    PYBIND11_DEPRECATED("base<T>() was deprecated in favor of specifying 'T' as a template argument to class_")
-    base() { } // NOLINT(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
+    PYBIND11_DEPRECATED(
+        "base<T>() was deprecated in favor of specifying 'T' as a template argument to class_")
+    base() {} // NOLINT(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
 };
 
 /// Keep patient alive while nurse lives
-template <size_t Nurse, size_t Patient> struct keep_alive { };
+template <size_t Nurse, size_t Patient>
+struct keep_alive {};
 
 /// Annotation indicating that a class is involved in a multiple inheritance relationship
-struct multiple_inheritance { };
+struct multiple_inheritance {};
 
 /// Annotation which enables dynamic attributes, i.e. adds `__dict__` to a class
-struct dynamic_attr { };
+struct dynamic_attr {};
 
 /// Annotation which enables the buffer protocol for a type
-struct buffer_protocol { };
+struct buffer_protocol {};
 
 /// Annotation which requests that a special metaclass is created for a type
 struct metaclass {
     handle value;
 
     PYBIND11_DEPRECATED("py::metaclass() is no longer required. It's turned on by default now.")
     // NOLINTNEXTLINE(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
     metaclass() {}
 
     /// Override pybind11's default metaclass
-    explicit metaclass(handle value) : value(value) { }
+    explicit metaclass(handle value) : value(value) {}
 };
 
 /// Specifies a custom callback with signature `void (PyHeapTypeObject*)` that
 /// may be used to customize the Python type.
 ///
 /// The callback is invoked immediately before `PyType_Ready`.
 ///
@@ -95,23 +103,24 @@
 
     explicit custom_type_setup(callback value) : value(std::move(value)) {}
 
     callback value;
 };
 
 /// Annotation that marks a class as local to the module:
-struct module_local { const bool value;
+struct module_local {
+    const bool value;
     constexpr explicit module_local(bool v = true) : value(v) {}
 };
 
 /// Annotation to mark enums as an arithmetic type
-struct arithmetic { };
+struct arithmetic {};
 
 /// Mark a function for addition at the beginning of the existing overload chain instead of the end
-struct prepend { };
+struct prepend {};
 
 /** \rst
     A call policy which places one or more guard variables (``Ts...``) around the function call.
 
     For example, this definition:
 
     .. code-block:: cpp
@@ -123,17 +132,21 @@
     .. code-block:: cpp
 
         m.def("foo", [](args...) {
             T scope_guard;
             return foo(args...); // forwarded arguments
         });
  \endrst */
-template <typename... Ts> struct call_guard;
+template <typename... Ts>
+struct call_guard;
 
-template <> struct call_guard<> { using type = detail::void_type; };
+template <>
+struct call_guard<> {
+    using type = detail::void_type;
+};
 
 template <typename T>
 struct call_guard<T> {
     static_assert(std::is_default_constructible<T>::value,
                   "The guard type must be default constructible");
 
     using type = T;
@@ -150,56 +163,58 @@
 /// @} annotations
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 /* Forward declarations */
 enum op_id : int;
 enum op_type : int;
 struct undefined_t;
-template <op_id id, op_type ot, typename L = undefined_t, typename R = undefined_t> struct op_;
+template <op_id id, op_type ot, typename L = undefined_t, typename R = undefined_t>
+struct op_;
 void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret);
 
 /// Internal data structure which holds metadata about a keyword argument
 struct argument_record {
     const char *name;  ///< Argument name
     const char *descr; ///< Human-readable version of the argument value
     handle value;      ///< Associated Python object
     bool convert : 1;  ///< True if the argument is allowed to convert when loading
     bool none : 1;     ///< True if None is allowed when loading
 
     argument_record(const char *name, const char *descr, handle value, bool convert, bool none)
-        : name(name), descr(descr), value(value), convert(convert), none(none) { }
+        : name(name), descr(descr), value(value), convert(convert), none(none) {}
 };
 
-/// Internal data structure which holds metadata about a bound function (signature, overloads, etc.)
+/// Internal data structure which holds metadata about a bound function (signature, overloads,
+/// etc.)
 struct function_record {
     function_record()
         : is_constructor(false), is_new_style_constructor(false), is_stateless(false),
-          is_operator(false), is_method(false), has_args(false),
-          has_kwargs(false), prepend(false) { }
+          is_operator(false), is_method(false), has_args(false), has_kwargs(false),
+          prepend(false) {}
 
     /// Function name
     char *name = nullptr; /* why no C++ strings? They generate heavier code.. */
 
     // User-specified documentation string
     char *doc = nullptr;
 
     /// Human-readable version of the function signature
     char *signature = nullptr;
 
     /// List of registered keyword arguments
     std::vector<argument_record> args;
 
     /// Pointer to lambda function which converts arguments and performs the actual call
-    handle (*impl) (function_call &) = nullptr;
+    handle (*impl)(function_call &) = nullptr;
 
     /// Storage for the wrapped function pointer and captured data, if any
-    void *data[3] = { };
+    void *data[3] = {};
 
     /// Pointer to custom destructor for 'data' (if needed)
-    void (*free_data) (function_record *ptr) = nullptr;
+    void (*free_data)(function_record *ptr) = nullptr;
 
     /// Return value policy associated with this function
     return_value_policy policy = return_value_policy::automatic;
 
     /// True if name == '__init__'
     bool is_constructor : 1;
 
@@ -247,15 +262,15 @@
     function_record *next = nullptr;
 };
 
 /// Special data structure which (temporarily) holds metadata about a bound class
 struct type_record {
     PYBIND11_NOINLINE type_record()
         : multiple_inheritance(false), dynamic_attr(false), buffer_protocol(false),
-          default_holder(true), module_local(false), is_final(false) { }
+          default_holder(true), module_local(false), is_final(false) {}
 
     /// Handle to the parent scope
     handle scope;
 
     /// Name of the class
     const char *name = nullptr;
 
@@ -306,203 +321,243 @@
 
     /// Is the class definition local to the module shared object?
     bool module_local : 1;
 
     /// Is the class inheritable from python classes?
     bool is_final : 1;
 
-    PYBIND11_NOINLINE void add_base(const std::type_info &base, void *(*caster)(void *)) {
-        auto base_info = detail::get_type_info(base, false);
+    PYBIND11_NOINLINE void add_base(const std::type_info &base, void *(*caster)(void *) ) {
+        auto *base_info = detail::get_type_info(base, false);
         if (!base_info) {
             std::string tname(base.name());
             detail::clean_type_id(tname);
-            pybind11_fail("generic_type: type \"" + std::string(name) +
-                          "\" referenced unknown base type \"" + tname + "\"");
+            pybind11_fail("generic_type: type \"" + std::string(name)
+                          + "\" referenced unknown base type \"" + tname + "\"");
         }
 
         if (default_holder != base_info->default_holder) {
             std::string tname(base.name());
             detail::clean_type_id(tname);
-            pybind11_fail("generic_type: type \"" + std::string(name) + "\" " +
-                    (default_holder ? "does not have" : "has") +
-                    " a non-default holder type while its base \"" + tname + "\" " +
-                    (base_info->default_holder ? "does not" : "does"));
+            pybind11_fail("generic_type: type \"" + std::string(name) + "\" "
+                          + (default_holder ? "does not have" : "has")
+                          + " a non-default holder type while its base \"" + tname + "\" "
+                          + (base_info->default_holder ? "does not" : "does"));
         }
 
         bases.append((PyObject *) base_info->type);
 
-        if (base_info->type->tp_dictoffset != 0)
+        if (base_info->type->tp_dictoffset != 0) {
             dynamic_attr = true;
+        }
 
-        if (caster)
+        if (caster) {
             base_info->implicit_casts.emplace_back(type, caster);
+        }
     }
 };
 
-inline function_call::function_call(const function_record &f, handle p) :
-        func(f), parent(p) {
+inline function_call::function_call(const function_record &f, handle p) : func(f), parent(p) {
     args.reserve(f.nargs);
     args_convert.reserve(f.nargs);
 }
 
 /// Tag for a new-style `__init__` defined in `detail/init.h`
-struct is_new_style_constructor { };
+struct is_new_style_constructor {};
 
 /**
  * Partial template specializations to process custom attributes provided to
  * cpp_function_ and class_. These are either used to initialize the respective
  * fields in the type_record and function_record data structures or executed at
  * runtime to deal with custom call policies (e.g. keep_alive).
  */
-template <typename T, typename SFINAE = void> struct process_attribute;
+template <typename T, typename SFINAE = void>
+struct process_attribute;
 
-template <typename T> struct process_attribute_default {
+template <typename T>
+struct process_attribute_default {
     /// Default implementation: do nothing
-    static void init(const T &, function_record *) { }
-    static void init(const T &, type_record *) { }
-    static void precall(function_call &) { }
-    static void postcall(function_call &, handle) { }
+    static void init(const T &, function_record *) {}
+    static void init(const T &, type_record *) {}
+    static void precall(function_call &) {}
+    static void postcall(function_call &, handle) {}
 };
 
 /// Process an attribute specifying the function's name
-template <> struct process_attribute<name> : process_attribute_default<name> {
+template <>
+struct process_attribute<name> : process_attribute_default<name> {
     static void init(const name &n, function_record *r) { r->name = const_cast<char *>(n.value); }
 };
 
 /// Process an attribute specifying the function's docstring
-template <> struct process_attribute<doc> : process_attribute_default<doc> {
+template <>
+struct process_attribute<doc> : process_attribute_default<doc> {
     static void init(const doc &n, function_record *r) { r->doc = const_cast<char *>(n.value); }
 };
 
 /// Process an attribute specifying the function's docstring (provided as a C-style string)
-template <> struct process_attribute<const char *> : process_attribute_default<const char *> {
+template <>
+struct process_attribute<const char *> : process_attribute_default<const char *> {
     static void init(const char *d, function_record *r) { r->doc = const_cast<char *>(d); }
     static void init(const char *d, type_record *r) { r->doc = const_cast<char *>(d); }
 };
-template <> struct process_attribute<char *> : process_attribute<const char *> { };
+template <>
+struct process_attribute<char *> : process_attribute<const char *> {};
 
 /// Process an attribute indicating the function's return value policy
-template <> struct process_attribute<return_value_policy> : process_attribute_default<return_value_policy> {
+template <>
+struct process_attribute<return_value_policy> : process_attribute_default<return_value_policy> {
     static void init(const return_value_policy &p, function_record *r) { r->policy = p; }
 };
 
-/// Process an attribute which indicates that this is an overloaded function associated with a given sibling
-template <> struct process_attribute<sibling> : process_attribute_default<sibling> {
+/// Process an attribute which indicates that this is an overloaded function associated with a
+/// given sibling
+template <>
+struct process_attribute<sibling> : process_attribute_default<sibling> {
     static void init(const sibling &s, function_record *r) { r->sibling = s.value; }
 };
 
 /// Process an attribute which indicates that this function is a method
-template <> struct process_attribute<is_method> : process_attribute_default<is_method> {
-    static void init(const is_method &s, function_record *r) { r->is_method = true; r->scope = s.class_; }
+template <>
+struct process_attribute<is_method> : process_attribute_default<is_method> {
+    static void init(const is_method &s, function_record *r) {
+        r->is_method = true;
+        r->scope = s.class_;
+    }
 };
 
 /// Process an attribute which indicates the parent scope of a method
-template <> struct process_attribute<scope> : process_attribute_default<scope> {
+template <>
+struct process_attribute<scope> : process_attribute_default<scope> {
     static void init(const scope &s, function_record *r) { r->scope = s.value; }
 };
 
 /// Process an attribute which indicates that this function is an operator
-template <> struct process_attribute<is_operator> : process_attribute_default<is_operator> {
+template <>
+struct process_attribute<is_operator> : process_attribute_default<is_operator> {
     static void init(const is_operator &, function_record *r) { r->is_operator = true; }
 };
 
-template <> struct process_attribute<is_new_style_constructor> : process_attribute_default<is_new_style_constructor> {
-    static void init(const is_new_style_constructor &, function_record *r) { r->is_new_style_constructor = true; }
+template <>
+struct process_attribute<is_new_style_constructor>
+    : process_attribute_default<is_new_style_constructor> {
+    static void init(const is_new_style_constructor &, function_record *r) {
+        r->is_new_style_constructor = true;
+    }
 };
 
 inline void check_kw_only_arg(const arg &a, function_record *r) {
-    if (r->args.size() > r->nargs_pos && (!a.name || a.name[0] == '\0'))
-        pybind11_fail("arg(): cannot specify an unnamed argument after a kw_only() annotation or args() argument");
+    if (r->args.size() > r->nargs_pos && (!a.name || a.name[0] == '\0')) {
+        pybind11_fail("arg(): cannot specify an unnamed argument after a kw_only() annotation or "
+                      "args() argument");
+    }
 }
 
 inline void append_self_arg_if_needed(function_record *r) {
-    if (r->is_method && r->args.empty())
-        r->args.emplace_back("self", nullptr, handle(), /*convert=*/ true, /*none=*/ false);
+    if (r->is_method && r->args.empty()) {
+        r->args.emplace_back("self", nullptr, handle(), /*convert=*/true, /*none=*/false);
+    }
 }
 
 /// Process a keyword argument attribute (*without* a default value)
-template <> struct process_attribute<arg> : process_attribute_default<arg> {
+template <>
+struct process_attribute<arg> : process_attribute_default<arg> {
     static void init(const arg &a, function_record *r) {
         append_self_arg_if_needed(r);
         r->args.emplace_back(a.name, nullptr, handle(), !a.flag_noconvert, a.flag_none);
 
         check_kw_only_arg(a, r);
     }
 };
 
 /// Process a keyword argument attribute (*with* a default value)
-template <> struct process_attribute<arg_v> : process_attribute_default<arg_v> {
+template <>
+struct process_attribute<arg_v> : process_attribute_default<arg_v> {
     static void init(const arg_v &a, function_record *r) {
-        if (r->is_method && r->args.empty())
-            r->args.emplace_back("self", /*descr=*/ nullptr, /*parent=*/ handle(), /*convert=*/ true, /*none=*/ false);
+        if (r->is_method && r->args.empty()) {
+            r->args.emplace_back(
+                "self", /*descr=*/nullptr, /*parent=*/handle(), /*convert=*/true, /*none=*/false);
+        }
 
         if (!a.value) {
 #if !defined(NDEBUG)
             std::string descr("'");
-            if (a.name) descr += std::string(a.name) + ": ";
+            if (a.name) {
+                descr += std::string(a.name) + ": ";
+            }
             descr += a.type + "'";
             if (r->is_method) {
-                if (r->name)
-                    descr += " in method '" + (std::string) str(r->scope) + "." + (std::string) r->name + "'";
-                else
+                if (r->name) {
+                    descr += " in method '" + (std::string) str(r->scope) + "."
+                             + (std::string) r->name + "'";
+                } else {
                     descr += " in method of '" + (std::string) str(r->scope) + "'";
+                }
             } else if (r->name) {
                 descr += " in function '" + (std::string) r->name + "'";
             }
-            pybind11_fail("arg(): could not convert default argument "
-                          + descr + " into a Python object (type not registered yet?)");
+            pybind11_fail("arg(): could not convert default argument " + descr
+                          + " into a Python object (type not registered yet?)");
 #else
             pybind11_fail("arg(): could not convert default argument "
                           "into a Python object (type not registered yet?). "
                           "Compile in debug mode for more information.");
 #endif
         }
         r->args.emplace_back(a.name, a.descr, a.value.inc_ref(), !a.flag_noconvert, a.flag_none);
 
         check_kw_only_arg(a, r);
     }
 };
 
 /// Process a keyword-only-arguments-follow pseudo argument
-template <> struct process_attribute<kw_only> : process_attribute_default<kw_only> {
+template <>
+struct process_attribute<kw_only> : process_attribute_default<kw_only> {
     static void init(const kw_only &, function_record *r) {
         append_self_arg_if_needed(r);
-        if (r->has_args && r->nargs_pos != static_cast<std::uint16_t>(r->args.size()))
-            pybind11_fail("Mismatched args() and kw_only(): they must occur at the same relative argument location (or omit kw_only() entirely)");
+        if (r->has_args && r->nargs_pos != static_cast<std::uint16_t>(r->args.size())) {
+            pybind11_fail("Mismatched args() and kw_only(): they must occur at the same relative "
+                          "argument location (or omit kw_only() entirely)");
+        }
         r->nargs_pos = static_cast<std::uint16_t>(r->args.size());
     }
 };
 
 /// Process a positional-only-argument maker
-template <> struct process_attribute<pos_only> : process_attribute_default<pos_only> {
+template <>
+struct process_attribute<pos_only> : process_attribute_default<pos_only> {
     static void init(const pos_only &, function_record *r) {
         append_self_arg_if_needed(r);
         r->nargs_pos_only = static_cast<std::uint16_t>(r->args.size());
-        if (r->nargs_pos_only > r->nargs_pos)
+        if (r->nargs_pos_only > r->nargs_pos) {
             pybind11_fail("pos_only(): cannot follow a py::args() argument");
-            // It also can't follow a kw_only, but a static_assert in pybind11.h checks that
+        }
+        // It also can't follow a kw_only, but a static_assert in pybind11.h checks that
     }
 };
 
-/// Process a parent class attribute.  Single inheritance only (class_ itself already guarantees that)
+/// Process a parent class attribute.  Single inheritance only (class_ itself already guarantees
+/// that)
 template <typename T>
-struct process_attribute<T, enable_if_t<is_pyobject<T>::value>> : process_attribute_default<handle> {
+struct process_attribute<T, enable_if_t<is_pyobject<T>::value>>
+    : process_attribute_default<handle> {
     static void init(const handle &h, type_record *r) { r->bases.append(h); }
 };
 
 /// Process a parent class attribute (deprecated, does not support multiple inheritance)
 template <typename T>
 struct process_attribute<base<T>> : process_attribute_default<base<T>> {
     static void init(const base<T> &, type_record *r) { r->add_base(typeid(T), nullptr); }
 };
 
 /// Process a multiple inheritance attribute
 template <>
 struct process_attribute<multiple_inheritance> : process_attribute_default<multiple_inheritance> {
-    static void init(const multiple_inheritance &, type_record *r) { r->multiple_inheritance = true; }
+    static void init(const multiple_inheritance &, type_record *r) {
+        r->multiple_inheritance = true;
+    }
 };
 
 template <>
 struct process_attribute<dynamic_attr> : process_attribute_default<dynamic_attr> {
     static void init(const dynamic_attr &, type_record *r) { r->dynamic_attr = true; }
 };
 
@@ -540,42 +595,49 @@
 };
 
 /// Process an 'arithmetic' attribute for enums (does nothing here)
 template <>
 struct process_attribute<arithmetic> : process_attribute_default<arithmetic> {};
 
 template <typename... Ts>
-struct process_attribute<call_guard<Ts...>> : process_attribute_default<call_guard<Ts...>> { };
+struct process_attribute<call_guard<Ts...>> : process_attribute_default<call_guard<Ts...>> {};
 
 /**
  * Process a keep_alive call policy -- invokes keep_alive_impl during the
  * pre-call handler if both Nurse, Patient != 0 and use the post-call handler
  * otherwise
  */
-template <size_t Nurse, size_t Patient> struct process_attribute<keep_alive<Nurse, Patient>> : public process_attribute_default<keep_alive<Nurse, Patient>> {
+template <size_t Nurse, size_t Patient>
+struct process_attribute<keep_alive<Nurse, Patient>>
+    : public process_attribute_default<keep_alive<Nurse, Patient>> {
     template <size_t N = Nurse, size_t P = Patient, enable_if_t<N != 0 && P != 0, int> = 0>
-    static void precall(function_call &call) { keep_alive_impl(Nurse, Patient, call, handle()); }
+    static void precall(function_call &call) {
+        keep_alive_impl(Nurse, Patient, call, handle());
+    }
     template <size_t N = Nurse, size_t P = Patient, enable_if_t<N != 0 && P != 0, int> = 0>
-    static void postcall(function_call &, handle) { }
+    static void postcall(function_call &, handle) {}
     template <size_t N = Nurse, size_t P = Patient, enable_if_t<N == 0 || P == 0, int> = 0>
-    static void precall(function_call &) { }
+    static void precall(function_call &) {}
     template <size_t N = Nurse, size_t P = Patient, enable_if_t<N == 0 || P == 0, int> = 0>
-    static void postcall(function_call &call, handle ret) { keep_alive_impl(Nurse, Patient, call, ret); }
+    static void postcall(function_call &call, handle ret) {
+        keep_alive_impl(Nurse, Patient, call, ret);
+    }
 };
 
 /// Recursively iterate over variadic template arguments
-template <typename... Args> struct process_attributes {
-    static void init(const Args&... args, function_record *r) {
+template <typename... Args>
+struct process_attributes {
+    static void init(const Args &...args, function_record *r) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(r);
         PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(r);
         using expander = int[];
         (void) expander{
             0, ((void) process_attribute<typename std::decay<Args>::type>::init(args, r), 0)...};
     }
-    static void init(const Args&... args, type_record *r) {
+    static void init(const Args &...args, type_record *r) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(r);
         PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(r);
         using expander = int[];
         (void) expander{0,
                         (process_attribute<typename std::decay<Args>::type>::init(args, r), 0)...};
     }
     static void precall(function_call &call) {
@@ -599,15 +661,15 @@
 /// Extract the ``type`` from the first `call_guard` in `Extras...` (or `void_type` if none found)
 template <typename... Extra>
 using extract_guard_t = typename exactly_one_t<is_call_guard, call_guard<>, Extra...>::type;
 
 /// Check the number of named arguments at compile time
 template <typename... Extra,
           size_t named = constexpr_sum(std::is_base_of<arg, Extra>::value...),
-          size_t self  = constexpr_sum(std::is_same<is_method, Extra>::value...)>
+          size_t self = constexpr_sum(std::is_same<is_method, Extra>::value...)>
 constexpr bool expected_num_args(size_t nargs, bool has_args, bool has_kwargs) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(nargs, has_args, has_kwargs);
     return named == 0 || (self + named + size_t(has_args) + size_t(has_kwargs)) == nargs;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/buffer_info.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/buffer_info.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,85 +15,118 @@
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Default, C-style strides
 inline std::vector<ssize_t> c_strides(const std::vector<ssize_t> &shape, ssize_t itemsize) {
     auto ndim = shape.size();
     std::vector<ssize_t> strides(ndim, itemsize);
-    if (ndim > 0)
-        for (size_t i = ndim - 1; i > 0; --i)
+    if (ndim > 0) {
+        for (size_t i = ndim - 1; i > 0; --i) {
             strides[i - 1] = strides[i] * shape[i];
+        }
+    }
     return strides;
 }
 
 // F-style strides; default when constructing an array_t with `ExtraFlags & f_style`
 inline std::vector<ssize_t> f_strides(const std::vector<ssize_t> &shape, ssize_t itemsize) {
     auto ndim = shape.size();
     std::vector<ssize_t> strides(ndim, itemsize);
-    for (size_t i = 1; i < ndim; ++i)
+    for (size_t i = 1; i < ndim; ++i) {
         strides[i] = strides[i - 1] * shape[i - 1];
+    }
     return strides;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Information record describing a Python buffer object
 struct buffer_info {
     void *ptr = nullptr;          // Pointer to the underlying storage
     ssize_t itemsize = 0;         // Size of individual items in bytes
     ssize_t size = 0;             // Total number of entries
-    std::string format;           // For homogeneous buffers, this should be set to format_descriptor<T>::format()
+    std::string format;           // For homogeneous buffers, this should be set to
+                                  // format_descriptor<T>::format()
     ssize_t ndim = 0;             // Number of dimensions
     std::vector<ssize_t> shape;   // Shape of the tensor (1 entry per dimension)
-    std::vector<ssize_t> strides; // Number of bytes between adjacent entries (for each per dimension)
+    std::vector<ssize_t> strides; // Number of bytes between adjacent entries
+                                  // (for each per dimension)
     bool readonly = false;        // flag to indicate if the underlying storage may be written to
 
     buffer_info() = default;
 
-    buffer_info(void *ptr, ssize_t itemsize, const std::string &format, ssize_t ndim,
-                detail::any_container<ssize_t> shape_in, detail::any_container<ssize_t> strides_in, bool readonly=false)
-    : ptr(ptr), itemsize(itemsize), size(1), format(format), ndim(ndim),
-      shape(std::move(shape_in)), strides(std::move(strides_in)), readonly(readonly) {
-        if (ndim != (ssize_t) shape.size() || ndim != (ssize_t) strides.size())
+    buffer_info(void *ptr,
+                ssize_t itemsize,
+                const std::string &format,
+                ssize_t ndim,
+                detail::any_container<ssize_t> shape_in,
+                detail::any_container<ssize_t> strides_in,
+                bool readonly = false)
+        : ptr(ptr), itemsize(itemsize), size(1), format(format), ndim(ndim),
+          shape(std::move(shape_in)), strides(std::move(strides_in)), readonly(readonly) {
+        if (ndim != (ssize_t) shape.size() || ndim != (ssize_t) strides.size()) {
             pybind11_fail("buffer_info: ndim doesn't match shape and/or strides length");
-        for (size_t i = 0; i < (size_t) ndim; ++i)
+        }
+        for (size_t i = 0; i < (size_t) ndim; ++i) {
             size *= shape[i];
+        }
     }
 
     template <typename T>
-    buffer_info(T *ptr, detail::any_container<ssize_t> shape_in, detail::any_container<ssize_t> strides_in, bool readonly=false)
-    : buffer_info(private_ctr_tag(), ptr, sizeof(T), format_descriptor<T>::format(), static_cast<ssize_t>(shape_in->size()), std::move(shape_in), std::move(strides_in), readonly) { }
-
-    buffer_info(void *ptr, ssize_t itemsize, const std::string &format, ssize_t size, bool readonly=false)
-    : buffer_info(ptr, itemsize, format, 1, {size}, {itemsize}, readonly) { }
+    buffer_info(T *ptr,
+                detail::any_container<ssize_t> shape_in,
+                detail::any_container<ssize_t> strides_in,
+                bool readonly = false)
+        : buffer_info(private_ctr_tag(),
+                      ptr,
+                      sizeof(T),
+                      format_descriptor<T>::format(),
+                      static_cast<ssize_t>(shape_in->size()),
+                      std::move(shape_in),
+                      std::move(strides_in),
+                      readonly) {}
+
+    buffer_info(void *ptr,
+                ssize_t itemsize,
+                const std::string &format,
+                ssize_t size,
+                bool readonly = false)
+        : buffer_info(ptr, itemsize, format, 1, {size}, {itemsize}, readonly) {}
 
     template <typename T>
-    buffer_info(T *ptr, ssize_t size, bool readonly=false)
-    : buffer_info(ptr, sizeof(T), format_descriptor<T>::format(), size, readonly) { }
+    buffer_info(T *ptr, ssize_t size, bool readonly = false)
+        : buffer_info(ptr, sizeof(T), format_descriptor<T>::format(), size, readonly) {}
 
     template <typename T>
-    buffer_info(const T *ptr, ssize_t size, bool readonly=true)
-    : buffer_info(const_cast<T*>(ptr), sizeof(T), format_descriptor<T>::format(), size, readonly) { }
+    buffer_info(const T *ptr, ssize_t size, bool readonly = true)
+        : buffer_info(
+            const_cast<T *>(ptr), sizeof(T), format_descriptor<T>::format(), size, readonly) {}
 
     explicit buffer_info(Py_buffer *view, bool ownview = true)
-    : buffer_info(view->buf, view->itemsize, view->format, view->ndim,
+        : buffer_info(
+            view->buf,
+            view->itemsize,
+            view->format,
+            view->ndim,
             {view->shape, view->shape + view->ndim},
             /* Though buffer::request() requests PyBUF_STRIDES, ctypes objects
              * ignore this flag and return a view with NULL strides.
              * When strides are NULL, build them manually.  */
             view->strides
-            ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
-            : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
+                ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
+                : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
             (view->readonly != 0)) {
+        // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         this->m_view = view;
+        // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         this->ownview = ownview;
     }
 
     buffer_info(const buffer_info &) = delete;
-    buffer_info& operator=(const buffer_info &) = delete;
+    buffer_info &operator=(const buffer_info &) = delete;
 
     buffer_info(buffer_info &&other) noexcept { (*this) = std::move(other); }
 
     buffer_info &operator=(buffer_info &&rhs) noexcept {
         ptr = rhs.ptr;
         itemsize = rhs.itemsize;
         size = rhs.size;
@@ -104,41 +137,57 @@
         std::swap(m_view, rhs.m_view);
         std::swap(ownview, rhs.ownview);
         readonly = rhs.readonly;
         return *this;
     }
 
     ~buffer_info() {
-        if (m_view && ownview) { PyBuffer_Release(m_view); delete m_view; }
+        if (m_view && ownview) {
+            PyBuffer_Release(m_view);
+            delete m_view;
+        }
     }
 
     Py_buffer *view() const { return m_view; }
     Py_buffer *&view() { return m_view; }
+
 private:
-    struct private_ctr_tag { };
+    struct private_ctr_tag {};
 
-    buffer_info(private_ctr_tag, void *ptr, ssize_t itemsize, const std::string &format, ssize_t ndim,
-                detail::any_container<ssize_t> &&shape_in, detail::any_container<ssize_t> &&strides_in, bool readonly)
-    : buffer_info(ptr, itemsize, format, ndim, std::move(shape_in), std::move(strides_in), readonly) { }
+    buffer_info(private_ctr_tag,
+                void *ptr,
+                ssize_t itemsize,
+                const std::string &format,
+                ssize_t ndim,
+                detail::any_container<ssize_t> &&shape_in,
+                detail::any_container<ssize_t> &&strides_in,
+                bool readonly)
+        : buffer_info(
+            ptr, itemsize, format, ndim, std::move(shape_in), std::move(strides_in), readonly) {}
 
     Py_buffer *m_view = nullptr;
     bool ownview = false;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T, typename SFINAE = void> struct compare_buffer_info {
-    static bool compare(const buffer_info& b) {
+template <typename T, typename SFINAE = void>
+struct compare_buffer_info {
+    static bool compare(const buffer_info &b) {
         return b.format == format_descriptor<T>::format() && b.itemsize == (ssize_t) sizeof(T);
     }
 };
 
-template <typename T> struct compare_buffer_info<T, detail::enable_if_t<std::is_integral<T>::value>> {
-    static bool compare(const buffer_info& b) {
-        return (size_t) b.itemsize == sizeof(T) && (b.format == format_descriptor<T>::value ||
-            ((sizeof(T) == sizeof(long)) && b.format == (std::is_unsigned<T>::value ? "L" : "l")) ||
-            ((sizeof(T) == sizeof(size_t)) && b.format == (std::is_unsigned<T>::value ? "N" : "n")));
+template <typename T>
+struct compare_buffer_info<T, detail::enable_if_t<std::is_integral<T>::value>> {
+    static bool compare(const buffer_info &b) {
+        return (size_t) b.itemsize == sizeof(T)
+               && (b.format == format_descriptor<T>::value
+                   || ((sizeof(T) == sizeof(long))
+                       && b.format == (std::is_unsigned<T>::value ? "L" : "l"))
+                   || ((sizeof(T) == sizeof(size_t))
+                       && b.format == (std::is_unsigned<T>::value ? "N" : "n")));
     }
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/cast.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/cast.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#include "pytypes.h"
 #include "detail/common.h"
 #include "detail/descr.h"
 #include "detail/type_caster_base.h"
 #include "detail/typeid.h"
+#include "pytypes.h"
+
 #include <array>
 #include <cstring>
 #include <functional>
 #include <iosfwd>
 #include <iterator>
 #include <memory>
 #include <string>
@@ -26,211 +27,241 @@
 #include <type_traits>
 #include <utility>
 #include <vector>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename type, typename SFINAE = void> class type_caster : public type_caster_base<type> { };
-template <typename type> using make_caster = type_caster<intrinsic_t<type>>;
+template <typename type, typename SFINAE = void>
+class type_caster : public type_caster_base<type> {};
+template <typename type>
+using make_caster = type_caster<intrinsic_t<type>>;
 
 // Shortcut for calling a caster's `cast_op_type` cast operator for casting a type_caster to a T
-template <typename T> typename make_caster<T>::template cast_op_type<T> cast_op(make_caster<T> &caster) {
+template <typename T>
+typename make_caster<T>::template cast_op_type<T> cast_op(make_caster<T> &caster) {
     return caster.operator typename make_caster<T>::template cast_op_type<T>();
 }
-template <typename T> typename make_caster<T>::template cast_op_type<typename std::add_rvalue_reference<T>::type>
+template <typename T>
+typename make_caster<T>::template cast_op_type<typename std::add_rvalue_reference<T>::type>
 cast_op(make_caster<T> &&caster) {
-    return std::move(caster).operator
-        typename make_caster<T>::template cast_op_type<typename std::add_rvalue_reference<T>::type>();
+    return std::move(caster).operator typename make_caster<T>::
+        template cast_op_type<typename std::add_rvalue_reference<T>::type>();
 }
 
-template <typename type> class type_caster<std::reference_wrapper<type>> {
+template <typename type>
+class type_caster<std::reference_wrapper<type>> {
 private:
     using caster_t = make_caster<type>;
     caster_t subcaster;
-    using reference_t = type&;
-    using subcaster_cast_op_type =
-        typename caster_t::template cast_op_type<reference_t>;
-
-    static_assert(std::is_same<typename std::remove_const<type>::type &, subcaster_cast_op_type>::value ||
-                  std::is_same<reference_t, subcaster_cast_op_type>::value,
-                  "std::reference_wrapper<T> caster requires T to have a caster with an "
-                  "`operator T &()` or `operator const T &()`");
+    using reference_t = type &;
+    using subcaster_cast_op_type = typename caster_t::template cast_op_type<reference_t>;
+
+    static_assert(
+        std::is_same<typename std::remove_const<type>::type &, subcaster_cast_op_type>::value
+            || std::is_same<reference_t, subcaster_cast_op_type>::value,
+        "std::reference_wrapper<T> caster requires T to have a caster with an "
+        "`operator T &()` or `operator const T &()`");
+
 public:
     bool load(handle src, bool convert) { return subcaster.load(src, convert); }
     static constexpr auto name = caster_t::name;
-    static handle cast(const std::reference_wrapper<type> &src, return_value_policy policy, handle parent) {
+    static handle
+    cast(const std::reference_wrapper<type> &src, return_value_policy policy, handle parent) {
         // It is definitely wrong to take ownership of this pointer, so mask that rvp
-        if (policy == return_value_policy::take_ownership || policy == return_value_policy::automatic)
+        if (policy == return_value_policy::take_ownership
+            || policy == return_value_policy::automatic) {
             policy = return_value_policy::automatic_reference;
+        }
         return caster_t::cast(&src.get(), policy, parent);
     }
-    template <typename T> using cast_op_type = std::reference_wrapper<type>;
+    template <typename T>
+    using cast_op_type = std::reference_wrapper<type>;
     explicit operator std::reference_wrapper<type>() { return cast_op<type &>(subcaster); }
 };
 
 #define PYBIND11_TYPE_CASTER(type, py_name)                                                       \
 protected:                                                                                        \
     type value;                                                                                   \
                                                                                                   \
 public:                                                                                           \
     static constexpr auto name = py_name;                                                         \
-    template <typename T_, enable_if_t<std::is_same<type, remove_cv_t<T_>>::value, int> = 0>      \
-    static handle cast(T_ *src, return_value_policy policy, handle parent) {                      \
+    template <typename T_,                                                                        \
+              ::pybind11::detail::enable_if_t<                                                    \
+                  std::is_same<type, ::pybind11::detail::remove_cv_t<T_>>::value,                 \
+                  int> = 0>                                                                       \
+    static ::pybind11::handle cast(                                                               \
+        T_ *src, ::pybind11::return_value_policy policy, ::pybind11::handle parent) {             \
         if (!src)                                                                                 \
-            return none().release();                                                              \
-        if (policy == return_value_policy::take_ownership) {                                      \
+            return ::pybind11::none().release();                                                  \
+        if (policy == ::pybind11::return_value_policy::take_ownership) {                          \
             auto h = cast(std::move(*src), policy, parent);                                       \
             delete src;                                                                           \
             return h;                                                                             \
         }                                                                                         \
         return cast(*src, policy, parent);                                                        \
     }                                                                                             \
     operator type *() { return &value; }               /* NOLINT(bugprone-macro-parentheses) */   \
     operator type &() { return value; }                /* NOLINT(bugprone-macro-parentheses) */   \
     operator type &&() && { return std::move(value); } /* NOLINT(bugprone-macro-parentheses) */   \
     template <typename T_>                                                                        \
-    using cast_op_type = pybind11::detail::movable_cast_op_type<T_>
+    using cast_op_type = ::pybind11::detail::movable_cast_op_type<T_>
 
-template <typename CharT> using is_std_char_type = any_of<
-    std::is_same<CharT, char>, /* std::string */
+template <typename CharT>
+using is_std_char_type = any_of<std::is_same<CharT, char>, /* std::string */
 #if defined(PYBIND11_HAS_U8STRING)
-    std::is_same<CharT, char8_t>, /* std::u8string */
+                                std::is_same<CharT, char8_t>, /* std::u8string */
 #endif
-    std::is_same<CharT, char16_t>, /* std::u16string */
-    std::is_same<CharT, char32_t>, /* std::u32string */
-    std::is_same<CharT, wchar_t> /* std::wstring */
->;
-
+                                std::is_same<CharT, char16_t>, /* std::u16string */
+                                std::is_same<CharT, char32_t>, /* std::u32string */
+                                std::is_same<CharT, wchar_t>   /* std::wstring */
+                                >;
 
 template <typename T>
 struct type_caster<T, enable_if_t<std::is_arithmetic<T>::value && !is_std_char_type<T>::value>> {
     using _py_type_0 = conditional_t<sizeof(T) <= sizeof(long), long, long long>;
-    using _py_type_1 = conditional_t<std::is_signed<T>::value, _py_type_0, typename std::make_unsigned<_py_type_0>::type>;
+    using _py_type_1 = conditional_t<std::is_signed<T>::value,
+                                     _py_type_0,
+                                     typename std::make_unsigned<_py_type_0>::type>;
     using py_type = conditional_t<std::is_floating_point<T>::value, double, _py_type_1>;
-public:
 
+public:
     bool load(handle src, bool convert) {
         py_type py_value;
 
-        if (!src)
+        if (!src) {
             return false;
+        }
 
 #if !defined(PYPY_VERSION)
         auto index_check = [](PyObject *o) { return PyIndex_Check(o); };
 #else
         // In PyPy 7.3.3, `PyIndex_Check` is implemented by calling `__index__`,
         // while CPython only considers the existence of `nb_index`/`__index__`.
         auto index_check = [](PyObject *o) { return hasattr(o, "__index__"); };
 #endif
 
         if (std::is_floating_point<T>::value) {
-            if (convert || PyFloat_Check(src.ptr()))
+            if (convert || PyFloat_Check(src.ptr())) {
                 py_value = (py_type) PyFloat_AsDouble(src.ptr());
-            else
+            } else {
                 return false;
+            }
         } else if (PyFloat_Check(src.ptr())
                    || (!convert && !PYBIND11_LONG_CHECK(src.ptr()) && !index_check(src.ptr()))) {
             return false;
         } else {
             handle src_or_index = src;
             // PyPy: 7.3.7's 3.8 does not implement PyLong_*'s __index__ calls.
 #if PY_VERSION_HEX < 0x03080000 || defined(PYPY_VERSION)
             object index;
-            if (!PYBIND11_LONG_CHECK(src.ptr())) {  // So: index_check(src.ptr())
+            if (!PYBIND11_LONG_CHECK(src.ptr())) { // So: index_check(src.ptr())
                 index = reinterpret_steal<object>(PyNumber_Index(src.ptr()));
                 if (!index) {
                     PyErr_Clear();
                     if (!convert)
                         return false;
-                }
-                else {
+                } else {
                     src_or_index = index;
                 }
             }
 #endif
             if (std::is_unsigned<py_type>::value) {
                 py_value = as_unsigned<py_type>(src_or_index.ptr());
             } else { // signed integer:
                 py_value = sizeof(T) <= sizeof(long)
-                    ? (py_type) PyLong_AsLong(src_or_index.ptr())
-                    : (py_type) PYBIND11_LONG_AS_LONGLONG(src_or_index.ptr());
+                               ? (py_type) PyLong_AsLong(src_or_index.ptr())
+                               : (py_type) PYBIND11_LONG_AS_LONGLONG(src_or_index.ptr());
             }
         }
 
         // Python API reported an error
         bool py_err = py_value == (py_type) -1 && PyErr_Occurred();
 
         // Check to see if the conversion is valid (integers should match exactly)
         // Signed/unsigned checks happen elsewhere
-        if (py_err || (std::is_integral<T>::value && sizeof(py_type) != sizeof(T) && py_value != (py_type) (T) py_value)) {
+        if (py_err
+            || (std::is_integral<T>::value && sizeof(py_type) != sizeof(T)
+                && py_value != (py_type) (T) py_value)) {
             PyErr_Clear();
             if (py_err && convert && (PyNumber_Check(src.ptr()) != 0)) {
                 auto tmp = reinterpret_steal<object>(std::is_floating_point<T>::value
-                                                     ? PyNumber_Float(src.ptr())
-                                                     : PyNumber_Long(src.ptr()));
+                                                         ? PyNumber_Float(src.ptr())
+                                                         : PyNumber_Long(src.ptr()));
                 PyErr_Clear();
                 return load(tmp, false);
             }
             return false;
         }
 
         value = (T) py_value;
         return true;
     }
 
-    template<typename U = T>
+    template <typename U = T>
     static typename std::enable_if<std::is_floating_point<U>::value, handle>::type
     cast(U src, return_value_policy /* policy */, handle /* parent */) {
         return PyFloat_FromDouble((double) src);
     }
 
-    template<typename U = T>
-    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_signed<U>::value && (sizeof(U) <= sizeof(long)), handle>::type
+    template <typename U = T>
+    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_signed<U>::value
+                                       && (sizeof(U) <= sizeof(long)),
+                                   handle>::type
     cast(U src, return_value_policy /* policy */, handle /* parent */) {
         return PYBIND11_LONG_FROM_SIGNED((long) src);
     }
 
-    template<typename U = T>
-    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_unsigned<U>::value && (sizeof(U) <= sizeof(unsigned long)), handle>::type
+    template <typename U = T>
+    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_unsigned<U>::value
+                                       && (sizeof(U) <= sizeof(unsigned long)),
+                                   handle>::type
     cast(U src, return_value_policy /* policy */, handle /* parent */) {
         return PYBIND11_LONG_FROM_UNSIGNED((unsigned long) src);
     }
 
-    template<typename U = T>
-    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_signed<U>::value && (sizeof(U) > sizeof(long)), handle>::type
+    template <typename U = T>
+    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_signed<U>::value
+                                       && (sizeof(U) > sizeof(long)),
+                                   handle>::type
     cast(U src, return_value_policy /* policy */, handle /* parent */) {
         return PyLong_FromLongLong((long long) src);
     }
 
-    template<typename U = T>
-    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_unsigned<U>::value && (sizeof(U) > sizeof(unsigned long)), handle>::type
+    template <typename U = T>
+    static typename std::enable_if<!std::is_floating_point<U>::value && std::is_unsigned<U>::value
+                                       && (sizeof(U) > sizeof(unsigned long)),
+                                   handle>::type
     cast(U src, return_value_policy /* policy */, handle /* parent */) {
         return PyLong_FromUnsignedLongLong((unsigned long long) src);
     }
 
     PYBIND11_TYPE_CASTER(T, const_name<std::is_integral<T>::value>("int", "float"));
 };
 
-template<typename T> struct void_caster {
+template <typename T>
+struct void_caster {
 public:
     bool load(handle src, bool) {
-        if (src && src.is_none())
+        if (src && src.is_none()) {
             return true;
+        }
         return false;
     }
     static handle cast(T, return_value_policy /* policy */, handle /* parent */) {
         return none().inc_ref();
     }
     PYBIND11_TYPE_CASTER(T, const_name("None"));
 };
 
-template <> class type_caster<void_type> : public void_caster<void_type> {};
+template <>
+class type_caster<void_type> : public void_caster<void_type> {};
 
-template <> class type_caster<void> : public type_caster<void_type> {
+template <>
+class type_caster<void> : public type_caster<void_type> {
 public:
     using type_caster<void_type>::cast;
 
     bool load(handle h, bool) {
         if (!h) {
             return false;
         }
@@ -242,72 +273,79 @@
         /* Check if this is a capsule */
         if (isinstance<capsule>(h)) {
             value = reinterpret_borrow<capsule>(h);
             return true;
         }
 
         /* Check if this is a C++ type */
-        auto &bases = all_type_info((PyTypeObject *) type::handle_of(h).ptr());
+        const auto &bases = all_type_info((PyTypeObject *) type::handle_of(h).ptr());
         if (bases.size() == 1) { // Only allowing loading from a single-value type
             value = values_and_holders(reinterpret_cast<instance *>(h.ptr())).begin()->value_ptr();
             return true;
         }
 
         /* Fail */
         return false;
     }
 
     static handle cast(const void *ptr, return_value_policy /* policy */, handle /* parent */) {
-        if (ptr)
+        if (ptr) {
             return capsule(ptr).release();
+        }
         return none().inc_ref();
     }
 
-    template <typename T> using cast_op_type = void*&;
+    template <typename T>
+    using cast_op_type = void *&;
     explicit operator void *&() { return value; }
     static constexpr auto name = const_name("capsule");
+
 private:
     void *value = nullptr;
 };
 
-template <> class type_caster<std::nullptr_t> : public void_caster<std::nullptr_t> { };
+template <>
+class type_caster<std::nullptr_t> : public void_caster<std::nullptr_t> {};
 
-template <> class type_caster<bool> {
+template <>
+class type_caster<bool> {
 public:
     bool load(handle src, bool convert) {
-        if (!src) return false;
+        if (!src) {
+            return false;
+        }
         if (src.ptr() == Py_True) {
             value = true;
             return true;
         }
         if (src.ptr() == Py_False) {
             value = false;
             return true;
         }
         if (convert || (std::strcmp("numpy.bool_", Py_TYPE(src.ptr())->tp_name) == 0)) {
             // (allow non-implicit conversion for numpy booleans)
 
             Py_ssize_t res = -1;
             if (src.is_none()) {
-                res = 0;  // None is implicitly converted to False
+                res = 0; // None is implicitly converted to False
             }
-            #if defined(PYPY_VERSION)
+#if defined(PYPY_VERSION)
             // On PyPy, check that "__bool__" (or "__nonzero__" on Python 2.7) attr exists
             else if (hasattr(src, PYBIND11_BOOL_ATTR)) {
                 res = PyObject_IsTrue(src.ptr());
             }
-            #else
+#else
             // Alternate approach for CPython: this does the same as the above, but optimized
             // using the CPython API so as to avoid an unneeded attribute lookup.
-            else if (auto tp_as_number = src.ptr()->ob_type->tp_as_number) {
+            else if (auto *tp_as_number = src.ptr()->ob_type->tp_as_number) {
                 if (PYBIND11_NB_BOOL(tp_as_number)) {
                     res = (*PYBIND11_NB_BOOL(tp_as_number))(src.ptr());
                 }
             }
-            #endif
+#endif
             if (res == 0 || res == 1) {
                 value = (res != 0);
                 return true;
             }
             PyErr_Clear();
         }
         return false;
@@ -315,28 +353,33 @@
     static handle cast(bool src, return_value_policy /* policy */, handle /* parent */) {
         return handle(src ? Py_True : Py_False).inc_ref();
     }
     PYBIND11_TYPE_CASTER(bool, const_name("bool"));
 };
 
 // Helper class for UTF-{8,16,32} C++ stl strings:
-template <typename StringType, bool IsView = false> struct string_caster {
+template <typename StringType, bool IsView = false>
+struct string_caster {
     using CharT = typename StringType::value_type;
 
     // Simplify life by being able to assume standard char sizes (the standard only guarantees
     // minimums, but Python requires exact sizes)
-    static_assert(!std::is_same<CharT, char>::value || sizeof(CharT) == 1, "Unsupported char size != 1");
+    static_assert(!std::is_same<CharT, char>::value || sizeof(CharT) == 1,
+                  "Unsupported char size != 1");
 #if defined(PYBIND11_HAS_U8STRING)
-    static_assert(!std::is_same<CharT, char8_t>::value || sizeof(CharT) == 1, "Unsupported char8_t size != 1");
+    static_assert(!std::is_same<CharT, char8_t>::value || sizeof(CharT) == 1,
+                  "Unsupported char8_t size != 1");
 #endif
-    static_assert(!std::is_same<CharT, char16_t>::value || sizeof(CharT) == 2, "Unsupported char16_t size != 2");
-    static_assert(!std::is_same<CharT, char32_t>::value || sizeof(CharT) == 4, "Unsupported char32_t size != 4");
+    static_assert(!std::is_same<CharT, char16_t>::value || sizeof(CharT) == 2,
+                  "Unsupported char16_t size != 2");
+    static_assert(!std::is_same<CharT, char32_t>::value || sizeof(CharT) == 4,
+                  "Unsupported char32_t size != 4");
     // wchar_t can be either 16 bits (Windows) or 32 (everywhere else)
     static_assert(!std::is_same<CharT, wchar_t>::value || sizeof(CharT) == 2 || sizeof(CharT) == 4,
-            "Unsupported wchar_t size != 2/4");
+                  "Unsupported wchar_t size != 2/4");
     static constexpr size_t UTF_N = 8 * sizeof(CharT);
 
     bool load(handle src, bool) {
 #if PY_MAJOR_VERSION < 3
         object temp;
 #endif
         handle load_src = src;
@@ -352,15 +395,18 @@
             }
 
             // The below is a guaranteed failure in Python 3 when PyUnicode_Check returns false
             if (!PYBIND11_BYTES_CHECK(load_src.ptr()))
                 return false;
 
             temp = reinterpret_steal<object>(PyUnicode_FromObject(load_src.ptr()));
-            if (!temp) { PyErr_Clear(); return false; }
+            if (!temp) {
+                PyErr_Clear();
+                return false;
+            }
             load_src = temp;
 #endif
         }
 
 #if PY_VERSION_HEX >= 0x03030000
         // On Python >= 3.3, for UTF-8 we avoid the need for a temporary `bytes`
         // object by using `PyUnicode_AsUTF8AndSize`.
@@ -373,55 +419,72 @@
                 return false;
             }
             value = StringType(buffer, static_cast<size_t>(size));
             return true;
         }
 #endif
 
-        auto utfNbytes = reinterpret_steal<object>(PyUnicode_AsEncodedString(
-            load_src.ptr(), UTF_N == 8 ? "utf-8" : UTF_N == 16 ? "utf-16" : "utf-32", nullptr));
-        if (!utfNbytes) { PyErr_Clear(); return false; }
+        auto utfNbytes
+            = reinterpret_steal<object>(PyUnicode_AsEncodedString(load_src.ptr(),
+                                                                  UTF_N == 8    ? "utf-8"
+                                                                  : UTF_N == 16 ? "utf-16"
+                                                                                : "utf-32",
+                                                                  nullptr));
+        if (!utfNbytes) {
+            PyErr_Clear();
+            return false;
+        }
 
-        const auto *buffer = reinterpret_cast<const CharT *>(PYBIND11_BYTES_AS_STRING(utfNbytes.ptr()));
+        const auto *buffer
+            = reinterpret_cast<const CharT *>(PYBIND11_BYTES_AS_STRING(utfNbytes.ptr()));
         size_t length = (size_t) PYBIND11_BYTES_SIZE(utfNbytes.ptr()) / sizeof(CharT);
         // Skip BOM for UTF-16/32
         if (PYBIND11_SILENCE_MSVC_C4127(UTF_N > 8)) {
             buffer++;
             length--;
         }
         value = StringType(buffer, length);
 
         // If we're loading a string_view we need to keep the encoded Python object alive:
-        if (IsView)
+        if (IsView) {
             loader_life_support::add_patient(utfNbytes);
+        }
 
         return true;
     }
 
-    static handle cast(const StringType &src, return_value_policy /* policy */, handle /* parent */) {
+    static handle
+    cast(const StringType &src, return_value_policy /* policy */, handle /* parent */) {
         const char *buffer = reinterpret_cast<const char *>(src.data());
         auto nbytes = ssize_t(src.size() * sizeof(CharT));
         handle s = decode_utfN(buffer, nbytes);
-        if (!s) throw error_already_set();
+        if (!s) {
+            throw error_already_set();
+        }
         return s;
     }
 
     PYBIND11_TYPE_CASTER(StringType, const_name(PYBIND11_STRING_NAME));
 
 private:
     static handle decode_utfN(const char *buffer, ssize_t nbytes) {
 #if !defined(PYPY_VERSION)
-        return
-            UTF_N == 8  ? PyUnicode_DecodeUTF8(buffer, nbytes, nullptr) :
-            UTF_N == 16 ? PyUnicode_DecodeUTF16(buffer, nbytes, nullptr, nullptr) :
-                          PyUnicode_DecodeUTF32(buffer, nbytes, nullptr, nullptr);
+        return UTF_N == 8    ? PyUnicode_DecodeUTF8(buffer, nbytes, nullptr)
+               : UTF_N == 16 ? PyUnicode_DecodeUTF16(buffer, nbytes, nullptr, nullptr)
+                             : PyUnicode_DecodeUTF32(buffer, nbytes, nullptr, nullptr);
 #else
-        // PyPy segfaults when on PyUnicode_DecodeUTF16 (and possibly on PyUnicode_DecodeUTF32 as well),
-        // so bypass the whole thing by just passing the encoding as a string value, which works properly:
-        return PyUnicode_Decode(buffer, nbytes, UTF_N == 8 ? "utf-8" : UTF_N == 16 ? "utf-16" : "utf-32", nullptr);
+        // PyPy segfaults when on PyUnicode_DecodeUTF16 (and possibly on PyUnicode_DecodeUTF32 as
+        // well), so bypass the whole thing by just passing the encoding as a string value, which
+        // works properly:
+        return PyUnicode_Decode(buffer,
+                                nbytes,
+                                UTF_N == 8    ? "utf-8"
+                                : UTF_N == 16 ? "utf-16"
+                                              : "utf-32",
+                                nullptr);
 #endif
     }
 
     // When loading into a std::string or char*, accept a bytes object as-is (i.e.
     // without any encoding/decoding attempt).  For other C++ char sizes this is a no-op.
     // which supports loading a unicode from a str, doesn't take this path.
     template <typename C = CharT>
@@ -436,207 +499,244 @@
             }
         }
 
         return false;
     }
 
     template <typename C = CharT>
-    bool load_bytes(enable_if_t<!std::is_same<C, char>::value, handle>) { return false; }
+    bool load_bytes(enable_if_t<!std::is_same<C, char>::value, handle>) {
+        return false;
+    }
 };
 
 template <typename CharT, class Traits, class Allocator>
-struct type_caster<std::basic_string<CharT, Traits, Allocator>, enable_if_t<is_std_char_type<CharT>::value>>
+struct type_caster<std::basic_string<CharT, Traits, Allocator>,
+                   enable_if_t<is_std_char_type<CharT>::value>>
     : string_caster<std::basic_string<CharT, Traits, Allocator>> {};
 
 #ifdef PYBIND11_HAS_STRING_VIEW
 template <typename CharT, class Traits>
-struct type_caster<std::basic_string_view<CharT, Traits>, enable_if_t<is_std_char_type<CharT>::value>>
+struct type_caster<std::basic_string_view<CharT, Traits>,
+                   enable_if_t<is_std_char_type<CharT>::value>>
     : string_caster<std::basic_string_view<CharT, Traits>, true> {};
 #endif
 
 // Type caster for C-style strings.  We basically use a std::string type caster, but also add the
 // ability to use None as a nullptr char* (which the string caster doesn't allow).
-template <typename CharT> struct type_caster<CharT, enable_if_t<is_std_char_type<CharT>::value>> {
+template <typename CharT>
+struct type_caster<CharT, enable_if_t<is_std_char_type<CharT>::value>> {
     using StringType = std::basic_string<CharT>;
     using StringCaster = type_caster<StringType>;
     StringCaster str_caster;
     bool none = false;
     CharT one_char = 0;
+
 public:
     bool load(handle src, bool convert) {
-        if (!src) return false;
+        if (!src) {
+            return false;
+        }
         if (src.is_none()) {
             // Defer accepting None to other overloads (if we aren't in convert mode):
-            if (!convert) return false;
+            if (!convert) {
+                return false;
+            }
             none = true;
             return true;
         }
         return str_caster.load(src, convert);
     }
 
     static handle cast(const CharT *src, return_value_policy policy, handle parent) {
-        if (src == nullptr) return pybind11::none().inc_ref();
+        if (src == nullptr) {
+            return pybind11::none().inc_ref();
+        }
         return StringCaster::cast(StringType(src), policy, parent);
     }
 
     static handle cast(CharT src, return_value_policy policy, handle parent) {
         if (std::is_same<char, CharT>::value) {
             handle s = PyUnicode_DecodeLatin1((const char *) &src, 1, nullptr);
-            if (!s) throw error_already_set();
+            if (!s) {
+                throw error_already_set();
+            }
             return s;
         }
         return StringCaster::cast(StringType(1, src), policy, parent);
     }
 
     explicit operator CharT *() {
         return none ? nullptr : const_cast<CharT *>(static_cast<StringType &>(str_caster).c_str());
     }
     explicit operator CharT &() {
-        if (none)
+        if (none) {
             throw value_error("Cannot convert None to a character");
+        }
 
         auto &value = static_cast<StringType &>(str_caster);
         size_t str_len = value.size();
-        if (str_len == 0)
+        if (str_len == 0) {
             throw value_error("Cannot convert empty string to a character");
+        }
 
         // If we're in UTF-8 mode, we have two possible failures: one for a unicode character that
-        // is too high, and one for multiple unicode characters (caught later), so we need to figure
-        // out how long the first encoded character is in bytes to distinguish between these two
-        // errors.  We also allow want to allow unicode characters U+0080 through U+00FF, as those
-        // can fit into a single char value.
+        // is too high, and one for multiple unicode characters (caught later), so we need to
+        // figure out how long the first encoded character is in bytes to distinguish between these
+        // two errors.  We also allow want to allow unicode characters U+0080 through U+00FF, as
+        // those can fit into a single char value.
         if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 8) && str_len > 1 && str_len <= 4) {
             auto v0 = static_cast<unsigned char>(value[0]);
             // low bits only: 0-127
             // 0b110xxxxx - start of 2-byte sequence
             // 0b1110xxxx - start of 3-byte sequence
             // 0b11110xxx - start of 4-byte sequence
             size_t char0_bytes = (v0 & 0x80) == 0      ? 1
                                  : (v0 & 0xE0) == 0xC0 ? 2
                                  : (v0 & 0xF0) == 0xE0 ? 3
                                                        : 4;
 
             if (char0_bytes == str_len) {
                 // If we have a 128-255 value, we can decode it into a single char:
                 if (char0_bytes == 2 && (v0 & 0xFC) == 0xC0) { // 0x110000xx 0x10xxxxxx
-                    one_char = static_cast<CharT>(((v0 & 3) << 6) + (static_cast<unsigned char>(value[1]) & 0x3F));
+                    one_char = static_cast<CharT>(((v0 & 3) << 6)
+                                                  + (static_cast<unsigned char>(value[1]) & 0x3F));
                     return one_char;
                 }
                 // Otherwise we have a single character, but it's > U+00FF
                 throw value_error("Character code point not in range(0x100)");
             }
         }
 
         // UTF-16 is much easier: we can only have a surrogate pair for values above U+FFFF, thus a
         // surrogate pair with total length 2 instantly indicates a range error (but not a "your
         // string was too long" error).
         else if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 16) && str_len == 2) {
             one_char = static_cast<CharT>(value[0]);
-            if (one_char >= 0xD800 && one_char < 0xE000)
+            if (one_char >= 0xD800 && one_char < 0xE000) {
                 throw value_error("Character code point not in range(0x10000)");
+            }
         }
 
-        if (str_len != 1)
+        if (str_len != 1) {
             throw value_error("Expected a character, but multi-character string found");
+        }
 
         one_char = value[0];
         return one_char;
     }
 
     static constexpr auto name = const_name(PYBIND11_STRING_NAME);
-    template <typename _T> using cast_op_type = pybind11::detail::cast_op_type<_T>;
+    template <typename _T>
+    using cast_op_type = pybind11::detail::cast_op_type<_T>;
 };
 
 // Base implementation for std::tuple and std::pair
-template <template<typename...> class Tuple, typename... Ts> class tuple_caster {
+template <template <typename...> class Tuple, typename... Ts>
+class tuple_caster {
     using type = Tuple<Ts...>;
     static constexpr auto size = sizeof...(Ts);
     using indices = make_index_sequence<size>;
-public:
 
+public:
     bool load(handle src, bool convert) {
-        if (!isinstance<sequence>(src))
+        if (!isinstance<sequence>(src)) {
             return false;
+        }
         const auto seq = reinterpret_borrow<sequence>(src);
-        if (seq.size() != size)
+        if (seq.size() != size) {
             return false;
+        }
         return load_impl(seq, convert, indices{});
     }
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         return cast_impl(std::forward<T>(src), policy, parent, indices{});
     }
 
     // copied from the PYBIND11_TYPE_CASTER macro
     template <typename T>
     static handle cast(T *src, return_value_policy policy, handle parent) {
-        if (!src) return none().release();
+        if (!src) {
+            return none().release();
+        }
         if (policy == return_value_policy::take_ownership) {
             auto h = cast(std::move(*src), policy, parent);
             delete src;
             return h;
         }
         return cast(*src, policy, parent);
     }
 
-    static constexpr auto name = const_name("Tuple[") + concat(make_caster<Ts>::name...) + const_name("]");
+    static constexpr auto name
+        = const_name("Tuple[") + concat(make_caster<Ts>::name...) + const_name("]");
 
-    template <typename T> using cast_op_type = type;
+    template <typename T>
+    using cast_op_type = type;
 
     explicit operator type() & { return implicit_cast(indices{}); }
     explicit operator type() && { return std::move(*this).implicit_cast(indices{}); }
 
 protected:
     template <size_t... Is>
-    type implicit_cast(index_sequence<Is...>) & { return type(cast_op<Ts>(std::get<Is>(subcasters))...); }
+    type implicit_cast(index_sequence<Is...>) & {
+        return type(cast_op<Ts>(std::get<Is>(subcasters))...);
+    }
     template <size_t... Is>
-    type implicit_cast(index_sequence<Is...>) && { return type(cast_op<Ts>(std::move(std::get<Is>(subcasters)))...); }
+    type implicit_cast(index_sequence<Is...>) && {
+        return type(cast_op<Ts>(std::move(std::get<Is>(subcasters)))...);
+    }
 
     static constexpr bool load_impl(const sequence &, bool, index_sequence<>) { return true; }
 
     template <size_t... Is>
     bool load_impl(const sequence &seq, bool convert, index_sequence<Is...>) {
 #ifdef __cpp_fold_expressions
-        if ((... || !std::get<Is>(subcasters).load(seq[Is], convert)))
+        if ((... || !std::get<Is>(subcasters).load(seq[Is], convert))) {
             return false;
+        }
 #else
-        for (bool r : {std::get<Is>(subcasters).load(seq[Is], convert)...})
-            if (!r)
+        for (bool r : {std::get<Is>(subcasters).load(seq[Is], convert)...}) {
+            if (!r) {
                 return false;
+            }
+        }
 #endif
         return true;
     }
 
     /* Implementation: Convert a C++ tuple into a Python tuple */
     template <typename T, size_t... Is>
-    static handle cast_impl(T &&src, return_value_policy policy, handle parent, index_sequence<Is...>) {
+    static handle
+    cast_impl(T &&src, return_value_policy policy, handle parent, index_sequence<Is...>) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(src, policy, parent);
         PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(policy, parent);
-        std::array<object, size> entries{{
-            reinterpret_steal<object>(make_caster<Ts>::cast(std::get<Is>(std::forward<T>(src)), policy, parent))...
-        }};
-        for (const auto &entry: entries)
-            if (!entry)
+        std::array<object, size> entries{{reinterpret_steal<object>(
+            make_caster<Ts>::cast(std::get<Is>(std::forward<T>(src)), policy, parent))...}};
+        for (const auto &entry : entries) {
+            if (!entry) {
                 return handle();
+            }
+        }
         tuple result(size);
         int counter = 0;
-        for (auto & entry: entries)
+        for (auto &entry : entries) {
             PyTuple_SET_ITEM(result.ptr(), counter++, entry.release().ptr());
+        }
         return result.release();
     }
 
     Tuple<make_caster<Ts>...> subcasters;
 };
 
-template <typename T1, typename T2> class type_caster<std::pair<T1, T2>>
-    : public tuple_caster<std::pair, T1, T2> {};
+template <typename T1, typename T2>
+class type_caster<std::pair<T1, T2>> : public tuple_caster<std::pair, T1, T2> {};
 
-template <typename... Ts> class type_caster<std::tuple<Ts...>>
-    : public tuple_caster<std::tuple, Ts...> {};
+template <typename... Ts>
+class type_caster<std::tuple<Ts...>> : public tuple_caster<std::tuple, Ts...> {};
 
 /// Helper class which abstracts away certain actions. Users can provide specializations for
 /// custom holders, but it's only necessary if the type has a non-standard interface.
 template <typename T>
 struct holder_helper {
     static auto get(const T &p) -> decltype(p.get()) { return p.get(); }
 };
@@ -647,41 +747,42 @@
 /// detail that may change in the future, as formal support for smart-pointer
 /// interoperability is added into pybind11.
 template <typename type, typename holder_type, typename SFINAE = void>
 struct copyable_holder_caster : public type_caster_base<type> {
 public:
     using base = type_caster_base<type>;
     static_assert(std::is_base_of<base, type_caster<type>>::value,
-            "Holder classes are only supported for custom types");
+                  "Holder classes are only supported for custom types");
     using base::base;
     using base::cast;
     using base::typeinfo;
     using base::value;
 
     bool load(handle src, bool convert) {
         return base::template load_impl<copyable_holder_caster<type, holder_type>>(src, convert);
     }
 
-    explicit operator type*() { return this->value; }
+    explicit operator type *() { return this->value; }
     // static_cast works around compiler error with MSVC 17 and CUDA 10.2
     // see issue #2180
-    explicit operator type&() { return *(static_cast<type *>(this->value)); }
-    explicit operator holder_type*() { return std::addressof(holder); }
-    explicit operator holder_type&() { return holder; }
+    explicit operator type &() { return *(static_cast<type *>(this->value)); }
+    explicit operator holder_type *() { return std::addressof(holder); }
+    explicit operator holder_type &() { return holder; }
 
     static handle cast(const holder_type &src, return_value_policy, handle) {
         const auto *ptr = holder_helper<holder_type>::get(src);
         return type_caster_base<type>::cast_holder(ptr, &src);
     }
 
 protected:
     friend class type_caster_generic;
     void check_holder_compat() {
-        if (typeinfo->default_holder)
+        if (typeinfo->default_holder) {
             throw cast_error("Unable to load a custom holder type from a default-holder instance");
+        }
     }
 
     bool load_value(value_and_holder &&v_h) {
         if (v_h.holder_constructed()) {
             value = v_h.value_ptr();
             holder = v_h.template holder<holder_type>();
             return true;
@@ -691,296 +792,405 @@
                          "(compile in debug mode for type information)");
 #else
                          "of type '"
                          + type_id<holder_type>() + "''");
 #endif
     }
 
-    template <typename T = holder_type, detail::enable_if_t<!std::is_constructible<T, const T &, type*>::value, int> = 0>
-    bool try_implicit_casts(handle, bool) { return false; }
+    template <typename T = holder_type,
+              detail::enable_if_t<!std::is_constructible<T, const T &, type *>::value, int> = 0>
+    bool try_implicit_casts(handle, bool) {
+        return false;
+    }
 
-    template <typename T = holder_type, detail::enable_if_t<std::is_constructible<T, const T &, type*>::value, int> = 0>
+    template <typename T = holder_type,
+              detail::enable_if_t<std::is_constructible<T, const T &, type *>::value, int> = 0>
     bool try_implicit_casts(handle src, bool convert) {
         for (auto &cast : typeinfo->implicit_casts) {
             copyable_holder_caster sub_caster(*cast.first);
             if (sub_caster.load(src, convert)) {
                 value = cast.second(sub_caster.value);
                 holder = holder_type(sub_caster.holder, (type *) value);
                 return true;
             }
         }
         return false;
     }
 
     static bool try_direct_conversions(handle) { return false; }
 
-
     holder_type holder;
 };
 
 /// Specialize for the common std::shared_ptr, so users don't need to
 template <typename T>
-class type_caster<std::shared_ptr<T>> : public copyable_holder_caster<T, std::shared_ptr<T>> { };
+class type_caster<std::shared_ptr<T>> : public copyable_holder_caster<T, std::shared_ptr<T>> {};
 
 /// Type caster for holder types like std::unique_ptr.
 /// Please consider the SFINAE hook an implementation detail, as explained
 /// in the comment for the copyable_holder_caster.
 template <typename type, typename holder_type, typename SFINAE = void>
 struct move_only_holder_caster {
     static_assert(std::is_base_of<type_caster_base<type>, type_caster<type>>::value,
-            "Holder classes are only supported for custom types");
+                  "Holder classes are only supported for custom types");
 
     static handle cast(holder_type &&src, return_value_policy, handle) {
         auto *ptr = holder_helper<holder_type>::get(src);
         return type_caster_base<type>::cast_holder(ptr, std::addressof(src));
     }
     static constexpr auto name = type_caster_base<type>::name;
 };
 
 template <typename type, typename deleter>
 class type_caster<std::unique_ptr<type, deleter>>
-    : public move_only_holder_caster<type, std::unique_ptr<type, deleter>> { };
+    : public move_only_holder_caster<type, std::unique_ptr<type, deleter>> {};
 
 template <typename type, typename holder_type>
 using type_caster_holder = conditional_t<is_copy_constructible<holder_type>::value,
                                          copyable_holder_caster<type, holder_type>,
                                          move_only_holder_caster<type, holder_type>>;
 
-template <typename T, bool Value = false> struct always_construct_holder { static constexpr bool value = Value; };
+template <typename T, bool Value = false>
+struct always_construct_holder {
+    static constexpr bool value = Value;
+};
 
 /// Create a specialization for custom holder types (silently ignores std::shared_ptr)
-#define PYBIND11_DECLARE_HOLDER_TYPE(type, holder_type, ...) \
-    namespace pybind11 { namespace detail { \
-    template <typename type> \
-    struct always_construct_holder<holder_type> : always_construct_holder<void, ##__VA_ARGS__>  { }; \
-    template <typename type> \
-    class type_caster<holder_type, enable_if_t<!is_shared_ptr<holder_type>::value>> \
-        : public type_caster_holder<type, holder_type> { }; \
-    }}
+#define PYBIND11_DECLARE_HOLDER_TYPE(type, holder_type, ...)                                      \
+    namespace pybind11 {                                                                          \
+    namespace detail {                                                                            \
+    template <typename type>                                                                      \
+    struct always_construct_holder<holder_type> : always_construct_holder<void, ##__VA_ARGS__> {  \
+    };                                                                                            \
+    template <typename type>                                                                      \
+    class type_caster<holder_type, enable_if_t<!is_shared_ptr<holder_type>::value>>               \
+        : public type_caster_holder<type, holder_type> {};                                        \
+    }                                                                                             \
+    }
 
 // PYBIND11_DECLARE_HOLDER_TYPE holder types:
-template <typename base, typename holder> struct is_holder_type :
-    std::is_base_of<detail::type_caster_holder<base, holder>, detail::type_caster<holder>> {};
+template <typename base, typename holder>
+struct is_holder_type
+    : std::is_base_of<detail::type_caster_holder<base, holder>, detail::type_caster<holder>> {};
 // Specialization for always-supported unique_ptr holders:
-template <typename base, typename deleter> struct is_holder_type<base, std::unique_ptr<base, deleter>> :
-    std::true_type {};
+template <typename base, typename deleter>
+struct is_holder_type<base, std::unique_ptr<base, deleter>> : std::true_type {};
 
-template <typename T> struct handle_type_name { static constexpr auto name = const_name<T>(); };
-template <> struct handle_type_name<bool_> { static constexpr auto name = const_name("bool"); };
-template <> struct handle_type_name<bytes> { static constexpr auto name = const_name(PYBIND11_BYTES_NAME); };
-template <> struct handle_type_name<int_> { static constexpr auto name = const_name("int"); };
-template <> struct handle_type_name<iterable> { static constexpr auto name = const_name("Iterable"); };
-template <> struct handle_type_name<iterator> { static constexpr auto name = const_name("Iterator"); };
-template <> struct handle_type_name<float_> { static constexpr auto name = const_name("float"); };
-template <> struct handle_type_name<none> { static constexpr auto name = const_name("None"); };
-template <> struct handle_type_name<args> { static constexpr auto name = const_name("*args"); };
-template <> struct handle_type_name<kwargs> { static constexpr auto name = const_name("**kwargs"); };
+template <typename T>
+struct handle_type_name {
+    static constexpr auto name = const_name<T>();
+};
+template <>
+struct handle_type_name<bool_> {
+    static constexpr auto name = const_name("bool");
+};
+template <>
+struct handle_type_name<bytes> {
+    static constexpr auto name = const_name(PYBIND11_BYTES_NAME);
+};
+template <>
+struct handle_type_name<int_> {
+    static constexpr auto name = const_name("int");
+};
+template <>
+struct handle_type_name<iterable> {
+    static constexpr auto name = const_name("Iterable");
+};
+template <>
+struct handle_type_name<iterator> {
+    static constexpr auto name = const_name("Iterator");
+};
+template <>
+struct handle_type_name<float_> {
+    static constexpr auto name = const_name("float");
+};
+template <>
+struct handle_type_name<none> {
+    static constexpr auto name = const_name("None");
+};
+template <>
+struct handle_type_name<args> {
+    static constexpr auto name = const_name("*args");
+};
+template <>
+struct handle_type_name<kwargs> {
+    static constexpr auto name = const_name("**kwargs");
+};
 
 template <typename type>
 struct pyobject_caster {
     template <typename T = type, enable_if_t<std::is_same<T, handle>::value, int> = 0>
-    bool load(handle src, bool /* convert */) { value = src; return static_cast<bool>(value); }
+    bool load(handle src, bool /* convert */) {
+        value = src;
+        return static_cast<bool>(value);
+    }
 
     template <typename T = type, enable_if_t<std::is_base_of<object, T>::value, int> = 0>
     bool load(handle src, bool /* convert */) {
 #if PY_MAJOR_VERSION < 3 && !defined(PYBIND11_STR_LEGACY_PERMISSIVE)
         // For Python 2, without this implicit conversion, Python code would
         // need to be cluttered with six.ensure_text() or similar, only to be
         // un-cluttered later after Python 2 support is dropped.
         if (PYBIND11_SILENCE_MSVC_C4127(std::is_same<T, str>::value) && isinstance<bytes>(src)) {
             PyObject *str_from_bytes = PyUnicode_FromEncodedObject(src.ptr(), "utf-8", nullptr);
-            if (!str_from_bytes) throw error_already_set();
+            if (!str_from_bytes)
+                throw error_already_set();
             value = reinterpret_steal<type>(str_from_bytes);
             return true;
         }
 #endif
-        if (!isinstance<type>(src))
+        if (!isinstance<type>(src)) {
             return false;
+        }
         value = reinterpret_borrow<type>(src);
         return true;
     }
 
     static handle cast(const handle &src, return_value_policy /* policy */, handle /* parent */) {
         return src.inc_ref();
     }
     PYBIND11_TYPE_CASTER(type, handle_type_name<type>::name);
 };
 
 template <typename T>
-class type_caster<T, enable_if_t<is_pyobject<T>::value>> : public pyobject_caster<T> { };
+class type_caster<T, enable_if_t<is_pyobject<T>::value>> : public pyobject_caster<T> {};
 
 // Our conditions for enabling moving are quite restrictive:
 // At compile time:
 // - T needs to be a non-const, non-pointer, non-reference type
 // - type_caster<T>::operator T&() must exist
 // - the type must be move constructible (obviously)
 // At run-time:
 // - if the type is non-copy-constructible, the object must be the sole owner of the type (i.e. it
 //   must have ref_count() == 1)h
 // If any of the above are not satisfied, we fall back to copying.
-template <typename T> using move_is_plain_type = satisfies_none_of<T,
-    std::is_void, std::is_pointer, std::is_reference, std::is_const
->;
-template <typename T, typename SFINAE = void> struct move_always : std::false_type {};
-template <typename T> struct move_always<T, enable_if_t<all_of<
-    move_is_plain_type<T>,
-    negation<is_copy_constructible<T>>,
-    std::is_move_constructible<T>,
-    std::is_same<decltype(std::declval<make_caster<T>>().operator T&()), T&>
->::value>> : std::true_type {};
-template <typename T, typename SFINAE = void> struct move_if_unreferenced : std::false_type {};
-template <typename T> struct move_if_unreferenced<T, enable_if_t<all_of<
-    move_is_plain_type<T>,
-    negation<move_always<T>>,
-    std::is_move_constructible<T>,
-    std::is_same<decltype(std::declval<make_caster<T>>().operator T&()), T&>
->::value>> : std::true_type {};
-template <typename T> using move_never = none_of<move_always<T>, move_if_unreferenced<T>>;
+template <typename T>
+using move_is_plain_type
+    = satisfies_none_of<T, std::is_void, std::is_pointer, std::is_reference, std::is_const>;
+template <typename T, typename SFINAE = void>
+struct move_always : std::false_type {};
+template <typename T>
+struct move_always<
+    T,
+    enable_if_t<
+        all_of<move_is_plain_type<T>,
+               negation<is_copy_constructible<T>>,
+               std::is_move_constructible<T>,
+               std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
+    : std::true_type {};
+template <typename T, typename SFINAE = void>
+struct move_if_unreferenced : std::false_type {};
+template <typename T>
+struct move_if_unreferenced<
+    T,
+    enable_if_t<
+        all_of<move_is_plain_type<T>,
+               negation<move_always<T>>,
+               std::is_move_constructible<T>,
+               std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
+    : std::true_type {};
+template <typename T>
+using move_never = none_of<move_always<T>, move_if_unreferenced<T>>;
 
 // Detect whether returning a `type` from a cast on type's type_caster is going to result in a
 // reference or pointer to a local variable of the type_caster.  Basically, only
 // non-reference/pointer `type`s and reference/pointers from a type_caster_generic are safe;
 // everything else returns a reference/pointer to a local variable.
-template <typename type> using cast_is_temporary_value_reference = bool_constant<
-    (std::is_reference<type>::value || std::is_pointer<type>::value) &&
-    !std::is_base_of<type_caster_generic, make_caster<type>>::value &&
-    !std::is_same<intrinsic_t<type>, void>::value
->;
+template <typename type>
+using cast_is_temporary_value_reference
+    = bool_constant<(std::is_reference<type>::value || std::is_pointer<type>::value)
+                    && !std::is_base_of<type_caster_generic, make_caster<type>>::value
+                    && !std::is_same<intrinsic_t<type>, void>::value>;
 
 // When a value returned from a C++ function is being cast back to Python, we almost always want to
 // force `policy = move`, regardless of the return value policy the function/method was declared
 // with.
-template <typename Return, typename SFINAE = void> struct return_value_policy_override {
+template <typename Return, typename SFINAE = void>
+struct return_value_policy_override {
     static return_value_policy policy(return_value_policy p) { return p; }
 };
 
-template <typename Return> struct return_value_policy_override<Return,
-        detail::enable_if_t<std::is_base_of<type_caster_generic, make_caster<Return>>::value, void>> {
+template <typename Return>
+struct return_value_policy_override<
+    Return,
+    detail::enable_if_t<std::is_base_of<type_caster_generic, make_caster<Return>>::value, void>> {
     static return_value_policy policy(return_value_policy p) {
-        return !std::is_lvalue_reference<Return>::value &&
-               !std::is_pointer<Return>::value
-                   ? return_value_policy::move : p;
+        return !std::is_lvalue_reference<Return>::value && !std::is_pointer<Return>::value
+                   ? return_value_policy::move
+                   : p;
     }
 };
 
 // Basic python -> C++ casting; throws if casting fails
-template <typename T, typename SFINAE> type_caster<T, SFINAE> &load_type(type_caster<T, SFINAE> &conv, const handle &handle) {
+template <typename T, typename SFINAE>
+type_caster<T, SFINAE> &load_type(type_caster<T, SFINAE> &conv, const handle &handle) {
     if (!conv.load(handle, true)) {
 #if defined(NDEBUG)
-        throw cast_error("Unable to cast Python instance to C++ type (compile in debug mode for details)");
+        throw cast_error(
+            "Unable to cast Python instance to C++ type (compile in debug mode for details)");
 #else
-        throw cast_error("Unable to cast Python instance of type " +
-            (std::string) str(type::handle_of(handle)) + " to C++ type '" + type_id<T>() + "'");
+        throw cast_error("Unable to cast Python instance of type "
+                         + (std::string) str(type::handle_of(handle)) + " to C++ type '"
+                         + type_id<T>() + "'");
 #endif
     }
     return conv;
 }
 // Wrapper around the above that also constructs and returns a type_caster
-template <typename T> make_caster<T> load_type(const handle &handle) {
+template <typename T>
+make_caster<T> load_type(const handle &handle) {
     make_caster<T> conv;
     load_type(conv, handle);
     return conv;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // pytype -> C++ type
 template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
 T cast(const handle &handle) {
     using namespace detail;
     static_assert(!cast_is_temporary_value_reference<T>::value,
-            "Unable to cast type to reference: value is local to type caster");
+                  "Unable to cast type to reference: value is local to type caster");
     return cast_op<T>(load_type<T>(handle));
 }
 
 // pytype -> pytype (calls converting constructor)
 template <typename T, detail::enable_if_t<detail::is_pyobject<T>::value, int> = 0>
-T cast(const handle &handle) { return T(reinterpret_borrow<object>(handle)); }
+T cast(const handle &handle) {
+    return T(reinterpret_borrow<object>(handle));
+}
 
 // C++ type -> py::object
 template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
-object cast(T &&value, return_value_policy policy = return_value_policy::automatic_reference,
+object cast(T &&value,
+            return_value_policy policy = return_value_policy::automatic_reference,
             handle parent = handle()) {
     using no_ref_T = typename std::remove_reference<T>::type;
-    if (policy == return_value_policy::automatic)
-        policy = std::is_pointer<no_ref_T>::value ? return_value_policy::take_ownership :
-                 std::is_lvalue_reference<T>::value ? return_value_policy::copy : return_value_policy::move;
-    else if (policy == return_value_policy::automatic_reference)
-        policy = std::is_pointer<no_ref_T>::value ? return_value_policy::reference :
-                 std::is_lvalue_reference<T>::value ? return_value_policy::copy : return_value_policy::move;
-    return reinterpret_steal<object>(detail::make_caster<T>::cast(std::forward<T>(value), policy, parent));
+    if (policy == return_value_policy::automatic) {
+        policy = std::is_pointer<no_ref_T>::value     ? return_value_policy::take_ownership
+                 : std::is_lvalue_reference<T>::value ? return_value_policy::copy
+                                                      : return_value_policy::move;
+    } else if (policy == return_value_policy::automatic_reference) {
+        policy = std::is_pointer<no_ref_T>::value     ? return_value_policy::reference
+                 : std::is_lvalue_reference<T>::value ? return_value_policy::copy
+                                                      : return_value_policy::move;
+    }
+    return reinterpret_steal<object>(
+        detail::make_caster<T>::cast(std::forward<T>(value), policy, parent));
 }
 
-template <typename T> T handle::cast() const { return pybind11::cast<T>(*this); }
-template <> inline void handle::cast() const { return; }
+template <typename T>
+T handle::cast() const {
+    return pybind11::cast<T>(*this);
+}
+template <>
+inline void handle::cast() const {
+    return;
+}
 
 template <typename T>
 detail::enable_if_t<!detail::move_never<T>::value, T> move(object &&obj) {
-    if (obj.ref_count() > 1)
+    if (obj.ref_count() > 1) {
 #if defined(NDEBUG)
-        throw cast_error("Unable to cast Python instance to C++ rvalue: instance has multiple references"
+        throw cast_error(
+            "Unable to cast Python instance to C++ rvalue: instance has multiple references"
             " (compile in debug mode for details)");
 #else
-        throw cast_error("Unable to move from Python " + (std::string) str(type::handle_of(obj)) +
-                " instance to C++ " + type_id<T>() + " instance: instance has multiple references");
+        throw cast_error("Unable to move from Python " + (std::string) str(type::handle_of(obj))
+                         + " instance to C++ " + type_id<T>()
+                         + " instance: instance has multiple references");
 #endif
+    }
 
     // Move into a temporary and return that, because the reference may be a local value of `conv`
-    T ret = std::move(detail::load_type<T>(obj).operator T&());
+    T ret = std::move(detail::load_type<T>(obj).operator T &());
     return ret;
 }
 
 // Calling cast() on an rvalue calls pybind11::cast with the object rvalue, which does:
 // - If we have to move (because T has no copy constructor), do it.  This will fail if the moved
 //   object has multiple references, but trying to copy will fail to compile.
 // - If both movable and copyable, check ref count: if 1, move; otherwise copy
 // - Otherwise (not movable), copy.
-template <typename T> detail::enable_if_t<detail::move_always<T>::value, T> cast(object &&object) {
+template <typename T>
+detail::enable_if_t<detail::move_always<T>::value, T> cast(object &&object) {
     return move<T>(std::move(object));
 }
-template <typename T> detail::enable_if_t<detail::move_if_unreferenced<T>::value, T> cast(object &&object) {
-    if (object.ref_count() > 1)
+template <typename T>
+detail::enable_if_t<detail::move_if_unreferenced<T>::value, T> cast(object &&object) {
+    if (object.ref_count() > 1) {
         return cast<T>(object);
+    }
     return move<T>(std::move(object));
 }
-template <typename T> detail::enable_if_t<detail::move_never<T>::value, T> cast(object &&object) {
+template <typename T>
+detail::enable_if_t<detail::move_never<T>::value, T> cast(object &&object) {
     return cast<T>(object);
 }
 
-template <typename T> T object::cast() const & { return pybind11::cast<T>(*this); }
-template <typename T> T object::cast() && { return pybind11::cast<T>(std::move(*this)); }
-template <> inline void object::cast() const & { return; }
-template <> inline void object::cast() && { return; }
+template <typename T>
+T object::cast() const & {
+    return pybind11::cast<T>(*this);
+}
+template <typename T>
+T object::cast() && {
+    return pybind11::cast<T>(std::move(*this));
+}
+template <>
+inline void object::cast() const & {
+    return;
+}
+template <>
+inline void object::cast() && {
+    return;
+}
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Declared in pytypes.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int>>
-object object_or_cast(T &&o) { return pybind11::cast(std::forward<T>(o)); }
+object object_or_cast(T &&o) {
+    return pybind11::cast(std::forward<T>(o));
+}
 
-struct override_unused {}; // Placeholder type for the unneeded (and dead code) static variable in the PYBIND11_OVERRIDE_OVERRIDE macro
-template <typename ret_type> using override_caster_t = conditional_t<
-    cast_is_temporary_value_reference<ret_type>::value, make_caster<ret_type>, override_unused>;
+// Placeholder type for the unneeded (and dead code) static variable in the
+// PYBIND11_OVERRIDE_OVERRIDE macro
+struct override_unused {};
+template <typename ret_type>
+using override_caster_t = conditional_t<cast_is_temporary_value_reference<ret_type>::value,
+                                        make_caster<ret_type>,
+                                        override_unused>;
 
 // Trampoline use: for reference/pointer types to value-converted values, we do a value cast, then
 // store the result in the given variable.  For other types, this is a no-op.
-template <typename T> enable_if_t<cast_is_temporary_value_reference<T>::value, T> cast_ref(object &&o, make_caster<T> &caster) {
+template <typename T>
+enable_if_t<cast_is_temporary_value_reference<T>::value, T> cast_ref(object &&o,
+                                                                     make_caster<T> &caster) {
     return cast_op<T>(load_type(caster, o));
 }
-template <typename T> enable_if_t<!cast_is_temporary_value_reference<T>::value, T> cast_ref(object &&, override_unused &) {
-    pybind11_fail("Internal error: cast_ref fallback invoked"); }
+template <typename T>
+enable_if_t<!cast_is_temporary_value_reference<T>::value, T> cast_ref(object &&,
+                                                                      override_unused &) {
+    pybind11_fail("Internal error: cast_ref fallback invoked");
+}
 
-// Trampoline use: Having a pybind11::cast with an invalid reference type is going to static_assert, even
-// though if it's in dead code, so we provide a "trampoline" to pybind11::cast that only does anything in
-// cases where pybind11::cast is valid.
-template <typename T> enable_if_t<!cast_is_temporary_value_reference<T>::value, T> cast_safe(object &&o) {
-    return pybind11::cast<T>(std::move(o)); }
-template <typename T> enable_if_t<cast_is_temporary_value_reference<T>::value, T> cast_safe(object &&) {
-    pybind11_fail("Internal error: cast_safe fallback invoked"); }
-template <> inline void cast_safe<void>(object &&) {}
+// Trampoline use: Having a pybind11::cast with an invalid reference type is going to
+// static_assert, even though if it's in dead code, so we provide a "trampoline" to pybind11::cast
+// that only does anything in cases where pybind11::cast is valid.
+template <typename T>
+enable_if_t<!cast_is_temporary_value_reference<T>::value, T> cast_safe(object &&o) {
+    return pybind11::cast<T>(std::move(o));
+}
+template <typename T>
+enable_if_t<cast_is_temporary_value_reference<T>::value, T> cast_safe(object &&) {
+    pybind11_fail("Internal error: cast_safe fallback invoked");
+}
+template <>
+inline void cast_safe<void>(object &&) {}
 
 PYBIND11_NAMESPACE_END(detail)
 
 // The overloads could coexist, i.e. the #if is not strictly speaking needed,
 // but it is an easy minor optimization.
 #if defined(NDEBUG)
 inline cast_error cast_error_unable_to_convert_call_arg() {
@@ -992,136 +1202,155 @@
                                                         const std::string &type) {
     return cast_error("Unable to convert call argument '" + name + "' of type '" + type
                       + "' to Python object");
 }
 #endif
 
 template <return_value_policy policy = return_value_policy::automatic_reference>
-tuple make_tuple() { return tuple(0); }
+tuple make_tuple() {
+    return tuple(0);
+}
 
-template <return_value_policy policy = return_value_policy::automatic_reference,
-          typename... Args> tuple make_tuple(Args&&... args_) {
+template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
+tuple make_tuple(Args &&...args_) {
     constexpr size_t size = sizeof...(Args);
-    std::array<object, size> args {
-        { reinterpret_steal<object>(detail::make_caster<Args>::cast(
-            std::forward<Args>(args_), policy, nullptr))... }
-    };
+    std::array<object, size> args{{reinterpret_steal<object>(
+        detail::make_caster<Args>::cast(std::forward<Args>(args_), policy, nullptr))...}};
     for (size_t i = 0; i < args.size(); i++) {
         if (!args[i]) {
 #if defined(NDEBUG)
             throw cast_error_unable_to_convert_call_arg();
 #else
-            std::array<std::string, size> argtypes { {type_id<Args>()...} };
+            std::array<std::string, size> argtypes{{type_id<Args>()...}};
             throw cast_error_unable_to_convert_call_arg(std::to_string(i), argtypes[i]);
 #endif
         }
     }
     tuple result(size);
     int counter = 0;
-    for (auto &arg_value : args)
+    for (auto &arg_value : args) {
         PyTuple_SET_ITEM(result.ptr(), counter++, arg_value.release().ptr());
+    }
     return result;
 }
 
 /// \ingroup annotations
 /// Annotation for arguments
 struct arg {
-    /// Constructs an argument with the name of the argument; if null or omitted, this is a positional argument.
-    constexpr explicit arg(const char *name = nullptr) : name(name), flag_noconvert(false), flag_none(true) { }
+    /// Constructs an argument with the name of the argument; if null or omitted, this is a
+    /// positional argument.
+    constexpr explicit arg(const char *name = nullptr)
+        : name(name), flag_noconvert(false), flag_none(true) {}
     /// Assign a value to this argument
-    template <typename T> arg_v operator=(T &&value) const;
+    template <typename T>
+    arg_v operator=(T &&value) const;
     /// Indicate that the type should not be converted in the type caster
-    arg &noconvert(bool flag = true) { flag_noconvert = flag; return *this; }
+    arg &noconvert(bool flag = true) {
+        flag_noconvert = flag;
+        return *this;
+    }
     /// Indicates that the argument should/shouldn't allow None (e.g. for nullable pointer args)
-    arg &none(bool flag = true) { flag_none = flag; return *this; }
+    arg &none(bool flag = true) {
+        flag_none = flag;
+        return *this;
+    }
 
-    const char *name; ///< If non-null, this is a named kwargs argument
-    bool flag_noconvert : 1; ///< If set, do not allow conversion (requires a supporting type caster!)
-    bool flag_none : 1; ///< If set (the default), allow None to be passed to this argument
+    const char *name;        ///< If non-null, this is a named kwargs argument
+    bool flag_noconvert : 1; ///< If set, do not allow conversion (requires a supporting type
+                             ///< caster!)
+    bool flag_none : 1;      ///< If set (the default), allow None to be passed to this argument
 };
 
 /// \ingroup annotations
 /// Annotation for arguments with values
 struct arg_v : arg {
 private:
     template <typename T>
     arg_v(arg &&base, T &&x, const char *descr = nullptr)
-        : arg(base),
-          value(reinterpret_steal<object>(
-              detail::make_caster<T>::cast(x, return_value_policy::automatic, {})
-          )),
+        : arg(base), value(reinterpret_steal<object>(
+                         detail::make_caster<T>::cast(x, return_value_policy::automatic, {}))),
           descr(descr)
 #if !defined(NDEBUG)
-        , type(type_id<T>())
+          ,
+          type(type_id<T>())
 #endif
     {
         // Workaround! See:
         // https://github.com/pybind/pybind11/issues/2336
         // https://github.com/pybind/pybind11/pull/2685#issuecomment-731286700
         if (PyErr_Occurred()) {
             PyErr_Clear();
         }
     }
 
 public:
     /// Direct construction with name, default, and description
     template <typename T>
     arg_v(const char *name, T &&x, const char *descr = nullptr)
-        : arg_v(arg(name), std::forward<T>(x), descr) { }
+        : arg_v(arg(name), std::forward<T>(x), descr) {}
 
     /// Called internally when invoking `py::arg("a") = value`
     template <typename T>
     arg_v(const arg &base, T &&x, const char *descr = nullptr)
-        : arg_v(arg(base), std::forward<T>(x), descr) { }
+        : arg_v(arg(base), std::forward<T>(x), descr) {}
 
     /// Same as `arg::noconvert()`, but returns *this as arg_v&, not arg&
-    arg_v &noconvert(bool flag = true) { arg::noconvert(flag); return *this; }
+    arg_v &noconvert(bool flag = true) {
+        arg::noconvert(flag);
+        return *this;
+    }
 
     /// Same as `arg::nonone()`, but returns *this as arg_v&, not arg&
-    arg_v &none(bool flag = true) { arg::none(flag); return *this; }
+    arg_v &none(bool flag = true) {
+        arg::none(flag);
+        return *this;
+    }
 
     /// The default value
     object value;
     /// The (optional) description of the default value
     const char *descr;
 #if !defined(NDEBUG)
     /// The C++ type name of the default value (only available when compiled in debug mode)
     std::string type;
 #endif
 };
 
 /// \ingroup annotations
-/// Annotation indicating that all following arguments are keyword-only; the is the equivalent of an
-/// unnamed '*' argument (in Python 3)
+/// Annotation indicating that all following arguments are keyword-only; the is the equivalent of
+/// an unnamed '*' argument (in Python 3)
 struct kw_only {};
 
 /// \ingroup annotations
-/// Annotation indicating that all previous arguments are positional-only; the is the equivalent of an
-/// unnamed '/' argument (in Python 3.8)
+/// Annotation indicating that all previous arguments are positional-only; the is the equivalent of
+/// an unnamed '/' argument (in Python 3.8)
 struct pos_only {};
 
 template <typename T>
 arg_v arg::operator=(T &&value) const {
     return {*this, std::forward<T>(value)};
 }
 
 /// Alias for backward compatibility -- to be removed in version 2.0
-template <typename /*unused*/> using arg_t = arg_v;
+template <typename /*unused*/>
+using arg_t = arg_v;
 
 inline namespace literals {
 /** \rst
     String literal version of `arg`
  \endrst */
 constexpr arg operator"" _a(const char *name, size_t) { return arg(name); }
 } // namespace literals
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T> using is_kw_only = std::is_same<intrinsic_t<T>, kw_only>;
-template <typename T> using is_pos_only = std::is_same<intrinsic_t<T>, pos_only>;
+template <typename T>
+using is_kw_only = std::is_same<intrinsic_t<T>, kw_only>;
+template <typename T>
+using is_pos_only = std::is_same<intrinsic_t<T>, pos_only>;
 
 // forward declaration (definition in attr.h)
 struct function_record;
 
 /// Internal data associated with a single function call
 struct function_call {
     function_call(const function_record &f, handle p); // Implementation in attr.h
@@ -1142,66 +1371,71 @@
     /// The parent, if any
     handle parent;
 
     /// If this is a call to an initializer, this argument contains `self`
     handle init_self;
 };
 
-
 /// Helper class which loads arguments for C++ functions called from Python
 template <typename... Args>
 class argument_loader {
     using indices = make_index_sequence<sizeof...(Args)>;
 
-    template <typename Arg> using argument_is_args   = std::is_same<intrinsic_t<Arg>, args>;
-    template <typename Arg> using argument_is_kwargs = std::is_same<intrinsic_t<Arg>, kwargs>;
+    template <typename Arg>
+    using argument_is_args = std::is_same<intrinsic_t<Arg>, args>;
+    template <typename Arg>
+    using argument_is_kwargs = std::is_same<intrinsic_t<Arg>, kwargs>;
     // Get kwargs argument position, or -1 if not present:
     static constexpr auto kwargs_pos = constexpr_last<argument_is_kwargs, Args...>();
 
-    static_assert(kwargs_pos == -1 || kwargs_pos == (int) sizeof...(Args) - 1, "py::kwargs is only permitted as the last argument of a function");
+    static_assert(kwargs_pos == -1 || kwargs_pos == (int) sizeof...(Args) - 1,
+                  "py::kwargs is only permitted as the last argument of a function");
 
 public:
     static constexpr bool has_kwargs = kwargs_pos != -1;
 
     // py::args argument position; -1 if not present.
     static constexpr int args_pos = constexpr_last<argument_is_args, Args...>();
 
-    static_assert(args_pos == -1 || args_pos == constexpr_first<argument_is_args, Args...>(), "py::args cannot be specified more than once");
+    static_assert(args_pos == -1 || args_pos == constexpr_first<argument_is_args, Args...>(),
+                  "py::args cannot be specified more than once");
 
     static constexpr auto arg_names = concat(type_descr(make_caster<Args>::name)...);
 
-    bool load_args(function_call &call) {
-        return load_impl_sequence(call, indices{});
-    }
+    bool load_args(function_call &call) { return load_impl_sequence(call, indices{}); }
 
     template <typename Return, typename Guard, typename Func>
     // NOLINTNEXTLINE(readability-const-return-type)
     enable_if_t<!std::is_void<Return>::value, Return> call(Func &&f) && {
-        return std::move(*this).template call_impl<remove_cv_t<Return>>(std::forward<Func>(f), indices{}, Guard{});
+        return std::move(*this).template call_impl<remove_cv_t<Return>>(
+            std::forward<Func>(f), indices{}, Guard{});
     }
 
     template <typename Return, typename Guard, typename Func>
     enable_if_t<std::is_void<Return>::value, void_type> call(Func &&f) && {
-        std::move(*this).template call_impl<remove_cv_t<Return>>(std::forward<Func>(f), indices{}, Guard{});
+        std::move(*this).template call_impl<remove_cv_t<Return>>(
+            std::forward<Func>(f), indices{}, Guard{});
         return void_type();
     }
 
 private:
-
     static bool load_impl_sequence(function_call &, index_sequence<>) { return true; }
 
     template <size_t... Is>
     bool load_impl_sequence(function_call &call, index_sequence<Is...>) {
 #ifdef __cpp_fold_expressions
-        if ((... || !std::get<Is>(argcasters).load(call.args[Is], call.args_convert[Is])))
+        if ((... || !std::get<Is>(argcasters).load(call.args[Is], call.args_convert[Is]))) {
             return false;
+        }
 #else
-        for (bool r : {std::get<Is>(argcasters).load(call.args[Is], call.args_convert[Is])...})
-            if (!r)
+        for (bool r : {std::get<Is>(argcasters).load(call.args[Is], call.args_convert[Is])...}) {
+            if (!r) {
                 return false;
+            }
+        }
 #endif
         return true;
     }
 
     template <typename Return, typename Func, size_t... Is, typename Guard>
     Return call_impl(Func &&f, index_sequence<Is...>, Guard &&) && {
         return std::forward<Func>(f)(cast_op<Args>(std::move(std::get<Is>(argcasters)))...);
@@ -1213,26 +1447,27 @@
 /// Helper class which collects only positional arguments for a Python function call.
 /// A fancier version below can collect any argument, but this one is optimal for simple calls.
 template <return_value_policy policy>
 class simple_collector {
 public:
     template <typename... Ts>
     explicit simple_collector(Ts &&...values)
-        : m_args(pybind11::make_tuple<policy>(std::forward<Ts>(values)...)) { }
+        : m_args(pybind11::make_tuple<policy>(std::forward<Ts>(values)...)) {}
 
     const tuple &args() const & { return m_args; }
     dict kwargs() const { return {}; }
 
     tuple args() && { return std::move(m_args); }
 
     /// Call a Python function and pass the collected arguments
     object call(PyObject *ptr) const {
         PyObject *result = PyObject_CallObject(ptr, m_args.ptr());
-        if (!result)
+        if (!result) {
             throw error_already_set();
+        }
         return reinterpret_steal<object>(result);
     }
 
 private:
     tuple m_args;
 };
 
@@ -1256,47 +1491,50 @@
 
     tuple args() && { return std::move(m_args); }
     dict kwargs() && { return std::move(m_kwargs); }
 
     /// Call a Python function and pass the collected arguments
     object call(PyObject *ptr) const {
         PyObject *result = PyObject_Call(ptr, m_args.ptr(), m_kwargs.ptr());
-        if (!result)
+        if (!result) {
             throw error_already_set();
+        }
         return reinterpret_steal<object>(result);
     }
 
 private:
     template <typename T>
     void process(list &args_list, T &&x) {
-        auto o = reinterpret_steal<object>(detail::make_caster<T>::cast(std::forward<T>(x), policy, {}));
+        auto o = reinterpret_steal<object>(
+            detail::make_caster<T>::cast(std::forward<T>(x), policy, {}));
         if (!o) {
 #if defined(NDEBUG)
             throw cast_error_unable_to_convert_call_arg();
 #else
-            throw cast_error_unable_to_convert_call_arg(
-                std::to_string(args_list.size()), type_id<T>());
+            throw cast_error_unable_to_convert_call_arg(std::to_string(args_list.size()),
+                                                        type_id<T>());
 #endif
         }
         args_list.append(o);
     }
 
     void process(list &args_list, detail::args_proxy ap) {
-        for (auto a : ap)
+        for (auto a : ap) {
             args_list.append(a);
+        }
     }
 
-    void process(list &/*args_list*/, arg_v a) {
-        if (!a.name)
+    void process(list & /*args_list*/, arg_v a) {
+        if (!a.name) {
 #if defined(NDEBUG)
             nameless_argument_error();
 #else
             nameless_argument_error(a.type);
 #endif
-
+        }
         if (m_kwargs.contains(a.name)) {
 #if defined(NDEBUG)
             multiple_values_error();
 #else
             multiple_values_error(a.name);
 #endif
         }
@@ -1306,17 +1544,18 @@
 #else
             throw cast_error_unable_to_convert_call_arg(a.name, a.type);
 #endif
         }
         m_kwargs[a.name] = a.value;
     }
 
-    void process(list &/*args_list*/, detail::kwargs_proxy kp) {
-        if (!kp)
+    void process(list & /*args_list*/, detail::kwargs_proxy kp) {
+        if (!kp) {
             return;
+        }
         for (auto k : reinterpret_borrow<dict>(kp)) {
             if (m_kwargs.contains(k.first)) {
 #if defined(NDEBUG)
                 multiple_values_error();
 #else
                 multiple_values_error(str(k.first));
 #endif
@@ -1327,16 +1566,17 @@
 
     [[noreturn]] static void nameless_argument_error() {
         throw type_error("Got kwargs without a name; only named arguments "
                          "may be passed via py::arg() to a python function call. "
                          "(compile in debug mode for details)");
     }
     [[noreturn]] static void nameless_argument_error(const std::string &type) {
-        throw type_error("Got kwargs without a name of type '" + type + "'; only named "
-                         "arguments may be passed via py::arg() to a python function call. ");
+        throw type_error("Got kwargs without a name of type '" + type
+                         + "'; only named "
+                           "arguments may be passed via py::arg() to a python function call. ");
     }
     [[noreturn]] static void multiple_values_error() {
         throw type_error("Got multiple values for keyword argument "
                          "(compile in debug mode for details)");
     }
 
     [[noreturn]] static void multiple_values_error(const std::string &name) {
@@ -1349,37 +1589,38 @@
 };
 
 // [workaround(intel)] Separate function required here
 // We need to put this into a separate function because the Intel compiler
 // fails to compile enable_if_t<!all_of<is_positional<Args>...>::value>
 // (tested with ICC 2021.1 Beta 20200827).
 template <typename... Args>
-constexpr bool args_are_all_positional()
-{
-  return all_of<is_positional<Args>...>::value;
+constexpr bool args_are_all_positional() {
+    return all_of<is_positional<Args>...>::value;
 }
 
 /// Collect only positional arguments for a Python function call
-template <return_value_policy policy, typename... Args,
+template <return_value_policy policy,
+          typename... Args,
           typename = enable_if_t<args_are_all_positional<Args...>()>>
 simple_collector<policy> collect_arguments(Args &&...args) {
     return simple_collector<policy>(std::forward<Args>(args)...);
 }
 
 /// Collect all arguments, including keywords and unpacking (only instantiated when needed)
-template <return_value_policy policy, typename... Args,
+template <return_value_policy policy,
+          typename... Args,
           typename = enable_if_t<!args_are_all_positional<Args...>()>>
 unpacking_collector<policy> collect_arguments(Args &&...args) {
     // Following argument order rules for generalized unpacking according to PEP 448
-    static_assert(
-        constexpr_last<is_positional, Args...>() < constexpr_first<is_keyword_or_ds, Args...>()
-        && constexpr_last<is_s_unpacking, Args...>() < constexpr_first<is_ds_unpacking, Args...>(),
-        "Invalid function call: positional args must precede keywords and ** unpacking; "
-        "* unpacking must precede ** unpacking"
-    );
+    static_assert(constexpr_last<is_positional, Args...>()
+                          < constexpr_first<is_keyword_or_ds, Args...>()
+                      && constexpr_last<is_s_unpacking, Args...>()
+                             < constexpr_first<is_ds_unpacking, Args...>(),
+                  "Invalid function call: positional args must precede keywords and ** unpacking; "
+                  "* unpacking must precede ** unpacking");
     return unpacking_collector<policy>(std::forward<Args>(args)...);
 }
 
 template <typename Derived>
 template <return_value_policy policy, typename... Args>
 object object_api<Derived>::operator()(Args &&...args) const {
 #if !defined(NDEBUG) && PY_VERSION_HEX >= 0x03060000
@@ -1394,29 +1635,29 @@
 template <return_value_policy policy, typename... Args>
 object object_api<Derived>::call(Args &&...args) const {
     return operator()<policy>(std::forward<Args>(args)...);
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
-
-template<typename T>
+template <typename T>
 handle type::handle_of() {
-   static_assert(
-      std::is_base_of<detail::type_caster_generic, detail::make_caster<T>>::value,
-      "py::type::of<T> only supports the case where T is a registered C++ types."
-    );
+    static_assert(std::is_base_of<detail::type_caster_generic, detail::make_caster<T>>::value,
+                  "py::type::of<T> only supports the case where T is a registered C++ types.");
 
     return detail::get_type_handle(typeid(T), true);
 }
 
-
-#define PYBIND11_MAKE_OPAQUE(...) \
-    namespace pybind11 { namespace detail { \
-        template<> class type_caster<__VA_ARGS__> : public type_caster_base<__VA_ARGS__> { }; \
-    }}
+#define PYBIND11_MAKE_OPAQUE(...)                                                                 \
+    namespace pybind11 {                                                                          \
+    namespace detail {                                                                            \
+    template <>                                                                                   \
+    class type_caster<__VA_ARGS__> : public type_caster_base<__VA_ARGS__> {};                     \
+    }                                                                                             \
+    }
 
 /// Lets you pass a type containing a `,` through a macro parameter without needing a separate
-/// typedef, e.g.: `PYBIND11_OVERRIDE(PYBIND11_TYPE(ReturnType<A, B>), PYBIND11_TYPE(Parent<C, D>), f, arg)`
+/// typedef, e.g.:
+/// `PYBIND11_OVERRIDE(PYBIND11_TYPE(ReturnType<A, B>), PYBIND11_TYPE(Parent<C, D>), f, arg)`
 #define PYBIND11_TYPE(...) __VA_ARGS__
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/chrono.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/chrono.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,83 +11,95 @@
 #pragma once
 
 #include "pybind11.h"
 
 #include <chrono>
 #include <cmath>
 #include <ctime>
-#include <mutex>
-
 #include <datetime.h>
+#include <mutex>
 
 // Backport the PyDateTime_DELTA functions from Python3.3 if required
 #ifndef PyDateTime_DELTA_GET_DAYS
-#define PyDateTime_DELTA_GET_DAYS(o)         (((PyDateTime_Delta*)o)->days)
+#    define PyDateTime_DELTA_GET_DAYS(o) (((PyDateTime_Delta *) o)->days)
 #endif
 #ifndef PyDateTime_DELTA_GET_SECONDS
-#define PyDateTime_DELTA_GET_SECONDS(o)      (((PyDateTime_Delta*)o)->seconds)
+#    define PyDateTime_DELTA_GET_SECONDS(o) (((PyDateTime_Delta *) o)->seconds)
 #endif
 #ifndef PyDateTime_DELTA_GET_MICROSECONDS
-#define PyDateTime_DELTA_GET_MICROSECONDS(o) (((PyDateTime_Delta*)o)->microseconds)
+#    define PyDateTime_DELTA_GET_MICROSECONDS(o) (((PyDateTime_Delta *) o)->microseconds)
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename type> class duration_caster {
+template <typename type>
+class duration_caster {
 public:
     using rep = typename type::rep;
     using period = typename type::period;
 
-    using days = std::chrono::duration<int_least32_t, std::ratio<86400>>; // signed 25 bits required by the standard.
+    // signed 25 bits required by the standard.
+    using days = std::chrono::duration<int_least32_t, std::ratio<86400>>;
 
     bool load(handle src, bool) {
         using namespace std::chrono;
 
         // Lazy initialise the PyDateTime import
-        if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
+        if (!PyDateTimeAPI) {
+            PyDateTime_IMPORT;
+        }
 
-        if (!src) return false;
+        if (!src) {
+            return false;
+        }
         // If invoked with datetime.delta object
         if (PyDelta_Check(src.ptr())) {
             value = type(duration_cast<duration<rep, period>>(
-                  days(PyDateTime_DELTA_GET_DAYS(src.ptr()))
+                days(PyDateTime_DELTA_GET_DAYS(src.ptr()))
                 + seconds(PyDateTime_DELTA_GET_SECONDS(src.ptr()))
                 + microseconds(PyDateTime_DELTA_GET_MICROSECONDS(src.ptr()))));
             return true;
         }
         // If invoked with a float we assume it is seconds and convert
         if (PyFloat_Check(src.ptr())) {
-            value = type(duration_cast<duration<rep, period>>(duration<double>(PyFloat_AsDouble(src.ptr()))));
+            value = type(duration_cast<duration<rep, period>>(
+                duration<double>(PyFloat_AsDouble(src.ptr()))));
             return true;
         }
         return false;
     }
 
     // If this is a duration just return it back
-    static const std::chrono::duration<rep, period>& get_duration(const std::chrono::duration<rep, period> &src) {
+    static const std::chrono::duration<rep, period> &
+    get_duration(const std::chrono::duration<rep, period> &src) {
         return src;
     }
 
     // If this is a time_point get the time_since_epoch
-    template <typename Clock> static std::chrono::duration<rep, period> get_duration(const std::chrono::time_point<Clock, std::chrono::duration<rep, period>> &src) {
+    template <typename Clock>
+    static std::chrono::duration<rep, period>
+    get_duration(const std::chrono::time_point<Clock, std::chrono::duration<rep, period>> &src) {
         return src.time_since_epoch();
     }
 
     static handle cast(const type &src, return_value_policy /* policy */, handle /* parent */) {
         using namespace std::chrono;
 
         // Use overloaded function to get our duration from our source
         // Works out if it is a duration or time_point and get the duration
         auto d = get_duration(src);
 
         // Lazy initialise the PyDateTime import
-        if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
+        if (!PyDateTimeAPI) {
+            PyDateTime_IMPORT;
+        }
 
-        // Declare these special duration types so the conversions happen with the correct primitive types (int)
+        // Declare these special duration types so the conversions happen with the correct
+        // primitive types (int)
         using dd_t = duration<int, std::ratio<86400>>;
         using ss_t = duration<int, std::ratio<1>>;
         using us_t = duration<int, std::micro>;
 
         auto dd = duration_cast<dd_t>(d);
         auto subd = d - dd;
         auto ss = duration_cast<ss_t>(subd);
@@ -111,101 +123,114 @@
         *buf = *tm_ptr;
     }
     return tm_ptr;
 #endif
 }
 
 // This is for casting times on the system clock into datetime.datetime instances
-template <typename Duration> class type_caster<std::chrono::time_point<std::chrono::system_clock, Duration>> {
+template <typename Duration>
+class type_caster<std::chrono::time_point<std::chrono::system_clock, Duration>> {
 public:
     using type = std::chrono::time_point<std::chrono::system_clock, Duration>;
     bool load(handle src, bool) {
         using namespace std::chrono;
 
         // Lazy initialise the PyDateTime import
-        if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
+        if (!PyDateTimeAPI) {
+            PyDateTime_IMPORT;
+        }
 
-        if (!src) return false;
+        if (!src) {
+            return false;
+        }
 
         std::tm cal;
         microseconds msecs;
 
         if (PyDateTime_Check(src.ptr())) {
-            cal.tm_sec   = PyDateTime_DATE_GET_SECOND(src.ptr());
-            cal.tm_min   = PyDateTime_DATE_GET_MINUTE(src.ptr());
-            cal.tm_hour  = PyDateTime_DATE_GET_HOUR(src.ptr());
-            cal.tm_mday  = PyDateTime_GET_DAY(src.ptr());
-            cal.tm_mon   = PyDateTime_GET_MONTH(src.ptr()) - 1;
-            cal.tm_year  = PyDateTime_GET_YEAR(src.ptr()) - 1900;
+            cal.tm_sec = PyDateTime_DATE_GET_SECOND(src.ptr());
+            cal.tm_min = PyDateTime_DATE_GET_MINUTE(src.ptr());
+            cal.tm_hour = PyDateTime_DATE_GET_HOUR(src.ptr());
+            cal.tm_mday = PyDateTime_GET_DAY(src.ptr());
+            cal.tm_mon = PyDateTime_GET_MONTH(src.ptr()) - 1;
+            cal.tm_year = PyDateTime_GET_YEAR(src.ptr()) - 1900;
             cal.tm_isdst = -1;
-            msecs        = microseconds(PyDateTime_DATE_GET_MICROSECOND(src.ptr()));
+            msecs = microseconds(PyDateTime_DATE_GET_MICROSECOND(src.ptr()));
         } else if (PyDate_Check(src.ptr())) {
-            cal.tm_sec   = 0;
-            cal.tm_min   = 0;
-            cal.tm_hour  = 0;
-            cal.tm_mday  = PyDateTime_GET_DAY(src.ptr());
-            cal.tm_mon   = PyDateTime_GET_MONTH(src.ptr()) - 1;
-            cal.tm_year  = PyDateTime_GET_YEAR(src.ptr()) - 1900;
+            cal.tm_sec = 0;
+            cal.tm_min = 0;
+            cal.tm_hour = 0;
+            cal.tm_mday = PyDateTime_GET_DAY(src.ptr());
+            cal.tm_mon = PyDateTime_GET_MONTH(src.ptr()) - 1;
+            cal.tm_year = PyDateTime_GET_YEAR(src.ptr()) - 1900;
             cal.tm_isdst = -1;
-            msecs        = microseconds(0);
+            msecs = microseconds(0);
         } else if (PyTime_Check(src.ptr())) {
-            cal.tm_sec   = PyDateTime_TIME_GET_SECOND(src.ptr());
-            cal.tm_min   = PyDateTime_TIME_GET_MINUTE(src.ptr());
-            cal.tm_hour  = PyDateTime_TIME_GET_HOUR(src.ptr());
-            cal.tm_mday  = 1;   // This date (day, month, year) = (1, 0, 70)
-            cal.tm_mon   = 0;   // represents 1-Jan-1970, which is the first
-            cal.tm_year  = 70;  // earliest available date for Python's datetime
+            cal.tm_sec = PyDateTime_TIME_GET_SECOND(src.ptr());
+            cal.tm_min = PyDateTime_TIME_GET_MINUTE(src.ptr());
+            cal.tm_hour = PyDateTime_TIME_GET_HOUR(src.ptr());
+            cal.tm_mday = 1;  // This date (day, month, year) = (1, 0, 70)
+            cal.tm_mon = 0;   // represents 1-Jan-1970, which is the first
+            cal.tm_year = 70; // earliest available date for Python's datetime
             cal.tm_isdst = -1;
-            msecs        = microseconds(PyDateTime_TIME_GET_MICROSECOND(src.ptr()));
+            msecs = microseconds(PyDateTime_TIME_GET_MICROSECOND(src.ptr()));
+        } else {
+            return false;
         }
-        else return false;
 
         value = time_point_cast<Duration>(system_clock::from_time_t(std::mktime(&cal)) + msecs);
         return true;
     }
 
-    static handle cast(const std::chrono::time_point<std::chrono::system_clock, Duration> &src, return_value_policy /* policy */, handle /* parent */) {
+    static handle cast(const std::chrono::time_point<std::chrono::system_clock, Duration> &src,
+                       return_value_policy /* policy */,
+                       handle /* parent */) {
         using namespace std::chrono;
 
         // Lazy initialise the PyDateTime import
-        if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
+        if (!PyDateTimeAPI) {
+            PyDateTime_IMPORT;
+        }
 
-        // Get out microseconds, and make sure they are positive, to avoid bug in eastern hemisphere time zones
-        // (cfr. https://github.com/pybind/pybind11/issues/2417)
+        // Get out microseconds, and make sure they are positive, to avoid bug in eastern
+        // hemisphere time zones (cfr. https://github.com/pybind/pybind11/issues/2417)
         using us_t = duration<int, std::micro>;
         auto us = duration_cast<us_t>(src.time_since_epoch() % seconds(1));
-        if (us.count() < 0)
+        if (us.count() < 0) {
             us += seconds(1);
+        }
 
         // Subtract microseconds BEFORE `system_clock::to_time_t`, because:
-        // > If std::time_t has lower precision, it is implementation-defined whether the value is rounded or truncated.
-        // (https://en.cppreference.com/w/cpp/chrono/system_clock/to_time_t)
-        std::time_t tt = system_clock::to_time_t(time_point_cast<system_clock::duration>(src - us));
+        // > If std::time_t has lower precision, it is implementation-defined whether the value is
+        // rounded or truncated. (https://en.cppreference.com/w/cpp/chrono/system_clock/to_time_t)
+        std::time_t tt
+            = system_clock::to_time_t(time_point_cast<system_clock::duration>(src - us));
 
         std::tm localtime;
         std::tm *localtime_ptr = localtime_thread_safe(&tt, &localtime);
-        if (!localtime_ptr)
+        if (!localtime_ptr) {
             throw cast_error("Unable to represent system_clock in local time");
+        }
         return PyDateTime_FromDateAndTime(localtime.tm_year + 1900,
                                           localtime.tm_mon + 1,
                                           localtime.tm_mday,
                                           localtime.tm_hour,
                                           localtime.tm_min,
                                           localtime.tm_sec,
                                           us.count());
     }
     PYBIND11_TYPE_CASTER(type, const_name("datetime.datetime"));
 };
 
 // Other clocks that are not the system clock are not measured as datetime.datetime objects
 // since they are not measured on calendar time. So instead we just make them timedeltas
 // Or if they have passed us a time as a float we convert that
-template <typename Clock, typename Duration> class type_caster<std::chrono::time_point<Clock, Duration>>
-: public duration_caster<std::chrono::time_point<Clock, Duration>> {
-};
-
-template <typename Rep, typename Period> class type_caster<std::chrono::duration<Rep, Period>>
-: public duration_caster<std::chrono::duration<Rep, Period>> {
-};
+template <typename Clock, typename Duration>
+class type_caster<std::chrono::time_point<Clock, Duration>>
+    : public duration_caster<std::chrono::time_point<Clock, Duration>> {};
+
+template <typename Rep, typename Period>
+class type_caster<std::chrono::duration<Rep, Period>>
+    : public duration_caster<std::chrono::duration<Rep, Period>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/complex.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/complex.h`

 * *Files 11% similar despite different names*

```diff
@@ -6,60 +6,69 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+
 #include <complex>
 
 /// glibc defines I as a macro which breaks things, e.g., boost template names
 #ifdef I
-#  undef I
+#    undef I
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
-template <typename T> struct format_descriptor<std::complex<T>, detail::enable_if_t<std::is_floating_point<T>::value>> {
+template <typename T>
+struct format_descriptor<std::complex<T>, detail::enable_if_t<std::is_floating_point<T>::value>> {
     static constexpr const char c = format_descriptor<T>::c;
-    static constexpr const char value[3] = { 'Z', c, '\0' };
+    static constexpr const char value[3] = {'Z', c, '\0'};
     static std::string format() { return std::string(value); }
 };
 
 #ifndef PYBIND11_CPP17
 
-template <typename T> constexpr const char format_descriptor<
-    std::complex<T>, detail::enable_if_t<std::is_floating_point<T>::value>>::value[3];
+template <typename T>
+constexpr const char
+    format_descriptor<std::complex<T>,
+                      detail::enable_if_t<std::is_floating_point<T>::value>>::value[3];
 
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T> struct is_fmt_numeric<std::complex<T>, detail::enable_if_t<std::is_floating_point<T>::value>> {
+template <typename T>
+struct is_fmt_numeric<std::complex<T>, detail::enable_if_t<std::is_floating_point<T>::value>> {
     static constexpr bool value = true;
     static constexpr int index = is_fmt_numeric<T>::index + 3;
 };
 
-template <typename T> class type_caster<std::complex<T>> {
+template <typename T>
+class type_caster<std::complex<T>> {
 public:
     bool load(handle src, bool convert) {
-        if (!src)
+        if (!src) {
             return false;
-        if (!convert && !PyComplex_Check(src.ptr()))
+        }
+        if (!convert && !PyComplex_Check(src.ptr())) {
             return false;
+        }
         Py_complex result = PyComplex_AsCComplex(src.ptr());
         if (result.real == -1.0 && PyErr_Occurred()) {
             PyErr_Clear();
             return false;
         }
         value = std::complex<T>((T) result.real, (T) result.imag);
         return true;
     }
 
-    static handle cast(const std::complex<T> &src, return_value_policy /* policy */, handle /* parent */) {
+    static handle
+    cast(const std::complex<T> &src, return_value_policy /* policy */, handle /* parent */) {
         return PyComplex_FromDoubles((double) src.real(), (double) src.imag());
     }
 
     PYBIND11_TYPE_CASTER(std::complex<T>, const_name("complex"));
 };
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/class.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/class.h`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 #include "../attr.h"
 #include "../options.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 #if PY_VERSION_HEX >= 0x03030000 && !defined(PYPY_VERSION)
-#  define PYBIND11_BUILTIN_QUALNAME
-#  define PYBIND11_SET_OLDPY_QUALNAME(obj, nameobj)
+#    define PYBIND11_BUILTIN_QUALNAME
+#    define PYBIND11_SET_OLDPY_QUALNAME(obj, nameobj)
 #else
 // In pre-3.3 Python, we still set __qualname__ so that we can produce reliable function type
 // signatures; in 3.3+ this macro expands to nothing:
-#  define PYBIND11_SET_OLDPY_QUALNAME(obj, nameobj) setattr((PyObject *) obj, "__qualname__", nameobj)
+#    define PYBIND11_SET_OLDPY_QUALNAME(obj, nameobj)                                             \
+        setattr((PyObject *) obj, "__qualname__", nameobj)
 #endif
 
 inline std::string get_fully_qualified_tp_name(PyTypeObject *type) {
 #if !defined(PYPY_VERSION)
     return type->tp_name;
 #else
     auto module_name = handle((PyObject *) type).attr("__module__").cast<std::string>();
@@ -61,32 +62,34 @@
     constexpr auto *name = "pybind11_static_property";
     auto name_obj = reinterpret_steal<object>(PYBIND11_FROM_STRING(name));
 
     /* Danger zone: from now (and until PyType_Ready), make sure to
        issue no Python C API calls which could potentially invoke the
        garbage collector (the GC will call type_traverse(), which will in
        turn find the newly constructed type in an invalid state) */
-    auto heap_type = (PyHeapTypeObject *) PyType_Type.tp_alloc(&PyType_Type, 0);
-    if (!heap_type)
+    auto *heap_type = (PyHeapTypeObject *) PyType_Type.tp_alloc(&PyType_Type, 0);
+    if (!heap_type) {
         pybind11_fail("make_static_property_type(): error allocating type!");
+    }
 
     heap_type->ht_name = name_obj.inc_ref().ptr();
-#ifdef PYBIND11_BUILTIN_QUALNAME
+#    ifdef PYBIND11_BUILTIN_QUALNAME
     heap_type->ht_qualname = name_obj.inc_ref().ptr();
-#endif
+#    endif
 
-    auto type = &heap_type->ht_type;
+    auto *type = &heap_type->ht_type;
     type->tp_name = name;
     type->tp_base = type_incref(&PyProperty_Type);
     type->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
     type->tp_descr_get = pybind11_static_get;
     type->tp_descr_set = pybind11_static_set;
 
-    if (PyType_Ready(type) < 0)
+    if (PyType_Ready(type) < 0) {
         pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
+    }
 
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     return type;
 }
 
@@ -94,45 +97,47 @@
 
 /** PyPy has some issues with the above C API, so we evaluate Python code instead.
     This function will only be called once so performance isn't really a concern.
     Return value: New reference. */
 inline PyTypeObject *make_static_property_type() {
     auto d = dict();
     PyObject *result = PyRun_String(R"(\
-        class pybind11_static_property(property):
-            def __get__(self, obj, cls):
-                return property.__get__(self, cls, cls)
-
-            def __set__(self, obj, value):
-                cls = obj if isinstance(obj, type) else type(obj)
-                property.__set__(self, cls, value)
-        )", Py_file_input, d.ptr(), d.ptr()
-    );
+class pybind11_static_property(property):
+    def __get__(self, obj, cls):
+        return property.__get__(self, cls, cls)
+
+    def __set__(self, obj, value):
+        cls = obj if isinstance(obj, type) else type(obj)
+        property.__set__(self, cls, value)
+)",
+                                    Py_file_input,
+                                    d.ptr(),
+                                    d.ptr());
     if (result == nullptr)
         throw error_already_set();
     Py_DECREF(result);
     return (PyTypeObject *) d["pybind11_static_property"].cast<object>().release().ptr();
 }
 
 #endif // PYPY
 
 /** Types with static properties need to handle `Type.static_prop = x` in a specific way.
     By default, Python replaces the `static_property` itself, but for wrapped C++ types
     we need to call `static_property.__set__()` in order to propagate the new value to
     the underlying C++ data structure. */
-extern "C" inline int pybind11_meta_setattro(PyObject* obj, PyObject* name, PyObject* value) {
+extern "C" inline int pybind11_meta_setattro(PyObject *obj, PyObject *name, PyObject *value) {
     // Use `_PyType_Lookup()` instead of `PyObject_GetAttr()` in order to get the raw
     // descriptor (`property`) instead of calling `tp_descr_get` (`property.__get__()`).
     PyObject *descr = _PyType_Lookup((PyTypeObject *) obj, name);
 
     // The following assignment combinations are possible:
     //   1. `Type.static_prop = value`             --> descr_set: `Type.static_prop.__set__(value)`
     //   2. `Type.static_prop = other_static_prop` --> setattro:  replace existing `static_prop`
     //   3. `Type.regular_attribute = value`       --> setattro:  regular attribute assignment
-    const auto static_prop = (PyObject *) get_internals().static_property_type;
+    auto *const static_prop = (PyObject *) get_internals().static_property_type;
     const auto call_descr_set = (descr != nullptr) && (value != nullptr)
                                 && (PyObject_IsInstance(descr, static_prop) != 0)
                                 && (PyObject_IsInstance(value, static_prop) == 0);
     if (call_descr_set) {
         // Call `static_property.__set__()` instead of replacing the `static_property`.
 #if !defined(PYPY_VERSION)
         return Py_TYPE(descr)->tp_descr_set(descr, obj, value);
@@ -173,20 +178,21 @@
     // use the default metaclass call to create/initialize the object
     PyObject *self = PyType_Type.tp_call(type, args, kwargs);
     if (self == nullptr) {
         return nullptr;
     }
 
     // This must be a pybind11 instance
-    auto instance = reinterpret_cast<detail::instance *>(self);
+    auto *instance = reinterpret_cast<detail::instance *>(self);
 
     // Ensure that the base __init__ function(s) were called
     for (const auto &vh : values_and_holders(instance)) {
         if (!vh.holder_constructed()) {
-            PyErr_Format(PyExc_TypeError, "%.200s.__init__() must be called when overriding __init__",
+            PyErr_Format(PyExc_TypeError,
+                         "%.200s.__init__() must be called when overriding __init__",
                          get_fully_qualified_tp_name(vh.type->type).c_str());
             Py_DECREF(self);
             return nullptr;
         }
     }
 
     return self;
@@ -197,98 +203,105 @@
     auto *type = (PyTypeObject *) obj;
     auto &internals = get_internals();
 
     // A pybind11-registered type will:
     // 1) be found in internals.registered_types_py
     // 2) have exactly one associated `detail::type_info`
     auto found_type = internals.registered_types_py.find(type);
-    if (found_type != internals.registered_types_py.end() &&
-        found_type->second.size() == 1 &&
-        found_type->second[0]->type == type) {
+    if (found_type != internals.registered_types_py.end() && found_type->second.size() == 1
+        && found_type->second[0]->type == type) {
 
         auto *tinfo = found_type->second[0];
         auto tindex = std::type_index(*tinfo->cpptype);
         internals.direct_conversions.erase(tindex);
 
-        if (tinfo->module_local)
+        if (tinfo->module_local) {
             get_local_internals().registered_types_cpp.erase(tindex);
-        else
+        } else {
             internals.registered_types_cpp.erase(tindex);
+        }
         internals.registered_types_py.erase(tinfo->type);
 
         // Actually just `std::erase_if`, but that's only available in C++20
         auto &cache = internals.inactive_override_cache;
-        for (auto it = cache.begin(), last = cache.end(); it != last; ) {
-            if (it->first == (PyObject *) tinfo->type)
+        for (auto it = cache.begin(), last = cache.end(); it != last;) {
+            if (it->first == (PyObject *) tinfo->type) {
                 it = cache.erase(it);
-            else
+            } else {
                 ++it;
+            }
         }
 
         delete tinfo;
     }
 
     PyType_Type.tp_dealloc(obj);
 }
 
 /** This metaclass is assigned by default to all pybind11 types and is required in order
     for static properties to function correctly. Users may override this using `py::metaclass`.
     Return value: New reference. */
-inline PyTypeObject* make_default_metaclass() {
+inline PyTypeObject *make_default_metaclass() {
     constexpr auto *name = "pybind11_type";
     auto name_obj = reinterpret_steal<object>(PYBIND11_FROM_STRING(name));
 
     /* Danger zone: from now (and until PyType_Ready), make sure to
        issue no Python C API calls which could potentially invoke the
        garbage collector (the GC will call type_traverse(), which will in
        turn find the newly constructed type in an invalid state) */
-    auto heap_type = (PyHeapTypeObject *) PyType_Type.tp_alloc(&PyType_Type, 0);
-    if (!heap_type)
+    auto *heap_type = (PyHeapTypeObject *) PyType_Type.tp_alloc(&PyType_Type, 0);
+    if (!heap_type) {
         pybind11_fail("make_default_metaclass(): error allocating metaclass!");
+    }
 
     heap_type->ht_name = name_obj.inc_ref().ptr();
 #ifdef PYBIND11_BUILTIN_QUALNAME
     heap_type->ht_qualname = name_obj.inc_ref().ptr();
 #endif
 
-    auto type = &heap_type->ht_type;
+    auto *type = &heap_type->ht_type;
     type->tp_name = name;
     type->tp_base = type_incref(&PyType_Type);
     type->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
 
     type->tp_call = pybind11_meta_call;
 
     type->tp_setattro = pybind11_meta_setattro;
 #if PY_MAJOR_VERSION >= 3
     type->tp_getattro = pybind11_meta_getattro;
 #endif
 
     type->tp_dealloc = pybind11_meta_dealloc;
 
-    if (PyType_Ready(type) < 0)
+    if (PyType_Ready(type) < 0) {
         pybind11_fail("make_default_metaclass(): failure in PyType_Ready()!");
+    }
 
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     return type;
 }
 
 /// For multiple inheritance types we need to recursively register/deregister base pointers for any
 /// base classes with pointers that are difference from the instance value pointer so that we can
-/// correctly recognize an offset base class pointer. This calls a function with any offset base ptrs.
-inline void traverse_offset_bases(void *valueptr, const detail::type_info *tinfo, instance *self,
-        bool (*f)(void * /*parentptr*/, instance * /*self*/)) {
+/// correctly recognize an offset base class pointer. This calls a function with any offset base
+/// ptrs.
+inline void traverse_offset_bases(void *valueptr,
+                                  const detail::type_info *tinfo,
+                                  instance *self,
+                                  bool (*f)(void * /*parentptr*/, instance * /*self*/)) {
     for (handle h : reinterpret_borrow<tuple>(tinfo->type->tp_bases)) {
-        if (auto parent_tinfo = get_type_info((PyTypeObject *) h.ptr())) {
+        if (auto *parent_tinfo = get_type_info((PyTypeObject *) h.ptr())) {
             for (auto &c : parent_tinfo->implicit_casts) {
                 if (c.first == tinfo->cpptype) {
                     auto *parentptr = c.second(valueptr);
-                    if (parentptr != valueptr)
+                    if (parentptr != valueptr) {
                         f(parentptr, self);
+                    }
                     traverse_offset_bases(parentptr, parent_tinfo, self, f);
                     break;
                 }
             }
         }
     }
 }
@@ -307,39 +320,41 @@
         }
     }
     return false;
 }
 
 inline void register_instance(instance *self, void *valptr, const type_info *tinfo) {
     register_instance_impl(valptr, self);
-    if (!tinfo->simple_ancestors)
+    if (!tinfo->simple_ancestors) {
         traverse_offset_bases(valptr, tinfo, self, register_instance_impl);
+    }
 }
 
 inline bool deregister_instance(instance *self, void *valptr, const type_info *tinfo) {
     bool ret = deregister_instance_impl(valptr, self);
-    if (!tinfo->simple_ancestors)
+    if (!tinfo->simple_ancestors) {
         traverse_offset_bases(valptr, tinfo, self, deregister_instance_impl);
+    }
     return ret;
 }
 
-/// Instance creation function for all pybind11 types. It allocates the internal instance layout for
-/// holding C++ objects and holders.  Allocation is done lazily (the first time the instance is cast
-/// to a reference or pointer), and initialization is done by an `__init__` function.
+/// Instance creation function for all pybind11 types. It allocates the internal instance layout
+/// for holding C++ objects and holders.  Allocation is done lazily (the first time the instance is
+/// cast to a reference or pointer), and initialization is done by an `__init__` function.
 inline PyObject *make_new_instance(PyTypeObject *type) {
 #if defined(PYPY_VERSION)
-    // PyPy gets tp_basicsize wrong (issue 2482) under multiple inheritance when the first inherited
-    // object is a plain Python type (i.e. not derived from an extension type).  Fix it.
+    // PyPy gets tp_basicsize wrong (issue 2482) under multiple inheritance when the first
+    // inherited object is a plain Python type (i.e. not derived from an extension type).  Fix it.
     ssize_t instance_size = static_cast<ssize_t>(sizeof(instance));
     if (type->tp_basicsize < instance_size) {
         type->tp_basicsize = instance_size;
     }
 #endif
     PyObject *self = type->tp_alloc(type, 0);
-    auto inst = reinterpret_cast<instance *>(self);
+    auto *inst = reinterpret_cast<instance *>(self);
     // Allocate the value/holder internals:
     inst->allocate_layout();
 
     return self;
 }
 
 /// Instance creation function for all pybind11 types. It only allocates space for the
@@ -356,73 +371,81 @@
     std::string msg = get_fully_qualified_tp_name(type) + ": No constructor defined!";
     PyErr_SetString(PyExc_TypeError, msg.c_str());
     return -1;
 }
 
 inline void add_patient(PyObject *nurse, PyObject *patient) {
     auto &internals = get_internals();
-    auto instance = reinterpret_cast<detail::instance *>(nurse);
+    auto *instance = reinterpret_cast<detail::instance *>(nurse);
     instance->has_patients = true;
     Py_INCREF(patient);
     internals.patients[nurse].push_back(patient);
 }
 
 inline void clear_patients(PyObject *self) {
-    auto instance = reinterpret_cast<detail::instance *>(self);
+    auto *instance = reinterpret_cast<detail::instance *>(self);
     auto &internals = get_internals();
     auto pos = internals.patients.find(self);
     assert(pos != internals.patients.end());
     // Clearing the patients can cause more Python code to run, which
     // can invalidate the iterator. Extract the vector of patients
     // from the unordered_map first.
     auto patients = std::move(pos->second);
     internals.patients.erase(pos);
     instance->has_patients = false;
-    for (PyObject *&patient : patients)
+    for (PyObject *&patient : patients) {
         Py_CLEAR(patient);
+    }
 }
 
 /// Clears all internal data from the instance and removes it from registered instances in
 /// preparation for deallocation.
 inline void clear_instance(PyObject *self) {
-    auto instance = reinterpret_cast<detail::instance *>(self);
+    auto *instance = reinterpret_cast<detail::instance *>(self);
 
     // Deallocate any values/holders, if present:
     for (auto &v_h : values_and_holders(instance)) {
         if (v_h) {
 
             // We have to deregister before we call dealloc because, for virtual MI types, we still
             // need to be able to get the parent pointers.
-            if (v_h.instance_registered() && !deregister_instance(instance, v_h.value_ptr(), v_h.type))
-                pybind11_fail("pybind11_object_dealloc(): Tried to deallocate unregistered instance!");
+            if (v_h.instance_registered()
+                && !deregister_instance(instance, v_h.value_ptr(), v_h.type)) {
+                pybind11_fail(
+                    "pybind11_object_dealloc(): Tried to deallocate unregistered instance!");
+            }
 
-            if (instance->owned || v_h.holder_constructed())
+            if (instance->owned || v_h.holder_constructed()) {
                 v_h.type->dealloc(v_h);
+            }
         }
     }
     // Deallocate the value/holder layout internals:
     instance->deallocate_layout();
 
-    if (instance->weakrefs)
+    if (instance->weakrefs) {
         PyObject_ClearWeakRefs(self);
+    }
 
     PyObject **dict_ptr = _PyObject_GetDictPtr(self);
-    if (dict_ptr)
+    if (dict_ptr) {
         Py_CLEAR(*dict_ptr);
+    }
 
-    if (instance->has_patients)
+    if (instance->has_patients) {
         clear_patients(self);
+    }
 }
 
 /// Instance destructor function for all pybind11 types. It calls `type_info.dealloc`
 /// to destroy the C++ object itself, while the rest is Python bookkeeping.
 extern "C" inline void pybind11_object_dealloc(PyObject *self) {
     clear_instance(self);
 
-    auto type = Py_TYPE(self);
+    auto *type = Py_TYPE(self);
     type->tp_free(self);
 
 #if PY_VERSION_HEX < 0x03080000
     // `type->tp_dealloc != pybind11_object_dealloc` means that we're being called
     // as part of a derived type's dealloc, in which case we're not allowed to decref
     // the type here. For cross-module compatibility, we shouldn't compare directly
     // with `pybind11_object_dealloc`, but with the common one stashed in internals.
@@ -443,59 +466,63 @@
     constexpr auto *name = "pybind11_object";
     auto name_obj = reinterpret_steal<object>(PYBIND11_FROM_STRING(name));
 
     /* Danger zone: from now (and until PyType_Ready), make sure to
        issue no Python C API calls which could potentially invoke the
        garbage collector (the GC will call type_traverse(), which will in
        turn find the newly constructed type in an invalid state) */
-    auto heap_type = (PyHeapTypeObject *) metaclass->tp_alloc(metaclass, 0);
-    if (!heap_type)
+    auto *heap_type = (PyHeapTypeObject *) metaclass->tp_alloc(metaclass, 0);
+    if (!heap_type) {
         pybind11_fail("make_object_base_type(): error allocating type!");
+    }
 
     heap_type->ht_name = name_obj.inc_ref().ptr();
 #ifdef PYBIND11_BUILTIN_QUALNAME
     heap_type->ht_qualname = name_obj.inc_ref().ptr();
 #endif
 
-    auto type = &heap_type->ht_type;
+    auto *type = &heap_type->ht_type;
     type->tp_name = name;
     type->tp_base = type_incref(&PyBaseObject_Type);
     type->tp_basicsize = static_cast<ssize_t>(sizeof(instance));
     type->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
 
     type->tp_new = pybind11_object_new;
     type->tp_init = pybind11_object_init;
     type->tp_dealloc = pybind11_object_dealloc;
 
     /* Support weak references (needed for the keep_alive feature) */
     type->tp_weaklistoffset = offsetof(instance, weakrefs);
 
-    if (PyType_Ready(type) < 0)
+    if (PyType_Ready(type) < 0) {
         pybind11_fail("PyType_Ready failed in make_object_base_type():" + error_string());
+    }
 
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     assert(!PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
     return (PyObject *) heap_type;
 }
 
 /// dynamic_attr: Support for `d = instance.__dict__`.
 extern "C" inline PyObject *pybind11_get_dict(PyObject *self, void *) {
     PyObject *&dict = *_PyObject_GetDictPtr(self);
-    if (!dict)
+    if (!dict) {
         dict = PyDict_New();
+    }
     Py_XINCREF(dict);
     return dict;
 }
 
 /// dynamic_attr: Support for `instance.__dict__ = dict()`.
 extern "C" inline int pybind11_set_dict(PyObject *self, PyObject *new_dict, void *) {
     if (!PyDict_Check(new_dict)) {
-        PyErr_Format(PyExc_TypeError, "__dict__ must be set to a dictionary, not a '%.200s'",
+        PyErr_Format(PyExc_TypeError,
+                     "__dict__ must be set to a dictionary, not a '%.200s'",
                      get_fully_qualified_tp_name(Py_TYPE(new_dict)).c_str());
         return -1;
     }
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_INCREF(new_dict);
     Py_CLEAR(dict);
     dict = new_dict;
@@ -514,40 +541,41 @@
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_CLEAR(dict);
     return 0;
 }
 
 /// Give instances of this type a `__dict__` and opt into garbage collection.
 inline void enable_dynamic_attributes(PyHeapTypeObject *heap_type) {
-    auto type = &heap_type->ht_type;
+    auto *type = &heap_type->ht_type;
     type->tp_flags |= Py_TPFLAGS_HAVE_GC;
-    type->tp_dictoffset = type->tp_basicsize; // place dict at the end
-    type->tp_basicsize += (ssize_t)sizeof(PyObject *); // and allocate enough space for it
+    type->tp_dictoffset = type->tp_basicsize;           // place dict at the end
+    type->tp_basicsize += (ssize_t) sizeof(PyObject *); // and allocate enough space for it
     type->tp_traverse = pybind11_traverse;
     type->tp_clear = pybind11_clear;
 
     static PyGetSetDef getset[] = {
-        {const_cast<char*>("__dict__"), pybind11_get_dict, pybind11_set_dict, nullptr, nullptr},
-        {nullptr, nullptr, nullptr, nullptr, nullptr}
-    };
+        {const_cast<char *>("__dict__"), pybind11_get_dict, pybind11_set_dict, nullptr, nullptr},
+        {nullptr, nullptr, nullptr, nullptr, nullptr}};
     type->tp_getset = getset;
 }
 
 /// buffer_protocol: Fill in the view as specified by flags.
 extern "C" inline int pybind11_getbuffer(PyObject *obj, Py_buffer *view, int flags) {
     // Look for a `get_buffer` implementation in this type's info or any bases (following MRO).
     type_info *tinfo = nullptr;
     for (auto type : reinterpret_borrow<tuple>(Py_TYPE(obj)->tp_mro)) {
         tinfo = get_type_info((PyTypeObject *) type.ptr());
-        if (tinfo && tinfo->get_buffer)
+        if (tinfo && tinfo->get_buffer) {
             break;
+        }
     }
     if (view == nullptr || !tinfo || !tinfo->get_buffer) {
-        if (view)
+        if (view) {
             view->obj = nullptr;
+        }
         PyErr_SetString(PyExc_BufferError, "pybind11_getbuffer(): Internal error");
         return -1;
     }
     std::memset(view, 0, sizeof(Py_buffer));
     buffer_info *info = tinfo->get_buffer(obj, tinfo->get_buffer_data);
     if ((flags & PyBUF_WRITABLE) == PyBUF_WRITABLE && info->readonly) {
         delete info;
@@ -557,23 +585,25 @@
     }
     view->obj = obj;
     view->ndim = 1;
     view->internal = info;
     view->buf = info->ptr;
     view->itemsize = info->itemsize;
     view->len = view->itemsize;
-    for (auto s : info->shape)
+    for (auto s : info->shape) {
         view->len *= s;
+    }
     view->readonly = static_cast<int>(info->readonly);
-    if ((flags & PyBUF_FORMAT) == PyBUF_FORMAT)
+    if ((flags & PyBUF_FORMAT) == PyBUF_FORMAT) {
         view->format = const_cast<char *>(info->format.c_str());
+    }
     if ((flags & PyBUF_STRIDES) == PyBUF_STRIDES) {
         view->ndim = (int) info->ndim;
-        view->strides = &info->strides[0];
-        view->shape = &info->shape[0];
+        view->strides = info->strides.data();
+        view->shape = info->shape.data();
     }
     Py_INCREF(view->obj);
     return 0;
 }
 
 /// buffer_protocol: Release the resources of the buffer.
 extern "C" inline void pybind11_releasebuffer(PyObject *, Py_buffer *view) {
@@ -589,78 +619,80 @@
 
     heap_type->as_buffer.bf_getbuffer = pybind11_getbuffer;
     heap_type->as_buffer.bf_releasebuffer = pybind11_releasebuffer;
 }
 
 /** Create a brand new Python type according to the `type_record` specification.
     Return value: New reference. */
-inline PyObject* make_new_python_type(const type_record &rec) {
+inline PyObject *make_new_python_type(const type_record &rec) {
     auto name = reinterpret_steal<object>(PYBIND11_FROM_STRING(rec.name));
 
     auto qualname = name;
     if (rec.scope && !PyModule_Check(rec.scope.ptr()) && hasattr(rec.scope, "__qualname__")) {
 #if PY_MAJOR_VERSION >= 3
         qualname = reinterpret_steal<object>(
             PyUnicode_FromFormat("%U.%U", rec.scope.attr("__qualname__").ptr(), name.ptr()));
 #else
         qualname = str(rec.scope.attr("__qualname__").cast<std::string>() + "." + rec.name);
 #endif
     }
 
     object module_;
     if (rec.scope) {
-        if (hasattr(rec.scope, "__module__"))
+        if (hasattr(rec.scope, "__module__")) {
             module_ = rec.scope.attr("__module__");
-        else if (hasattr(rec.scope, "__name__"))
+        } else if (hasattr(rec.scope, "__name__")) {
             module_ = rec.scope.attr("__name__");
+        }
     }
 
-    auto full_name = c_str(
+    const auto *full_name = c_str(
 #if !defined(PYPY_VERSION)
         module_ ? str(module_).cast<std::string>() + "." + rec.name :
 #endif
-        rec.name);
+                rec.name);
 
     char *tp_doc = nullptr;
     if (rec.doc && options::show_user_defined_docstrings()) {
         /* Allocate memory for docstring (using PyObject_MALLOC, since
            Python will free this later on) */
         size_t size = std::strlen(rec.doc) + 1;
         tp_doc = (char *) PyObject_MALLOC(size);
         std::memcpy((void *) tp_doc, rec.doc, size);
     }
 
     auto &internals = get_internals();
     auto bases = tuple(rec.bases);
-    auto base = (bases.empty()) ? internals.instance_base
-                                    : bases[0].ptr();
+    auto *base = (bases.empty()) ? internals.instance_base : bases[0].ptr();
 
     /* Danger zone: from now (and until PyType_Ready), make sure to
        issue no Python C API calls which could potentially invoke the
        garbage collector (the GC will call type_traverse(), which will in
        turn find the newly constructed type in an invalid state) */
-    auto metaclass = rec.metaclass.ptr() ? (PyTypeObject *) rec.metaclass.ptr()
-                                         : internals.default_metaclass;
+    auto *metaclass
+        = rec.metaclass.ptr() ? (PyTypeObject *) rec.metaclass.ptr() : internals.default_metaclass;
 
-    auto heap_type = (PyHeapTypeObject *) metaclass->tp_alloc(metaclass, 0);
-    if (!heap_type)
+    auto *heap_type = (PyHeapTypeObject *) metaclass->tp_alloc(metaclass, 0);
+    if (!heap_type) {
         pybind11_fail(std::string(rec.name) + ": Unable to create type object!");
+    }
 
     heap_type->ht_name = name.release().ptr();
 #ifdef PYBIND11_BUILTIN_QUALNAME
     heap_type->ht_qualname = qualname.inc_ref().ptr();
 #endif
 
-    auto type = &heap_type->ht_type;
+    auto *type = &heap_type->ht_type;
     type->tp_name = full_name;
     type->tp_doc = tp_doc;
-    type->tp_base = type_incref((PyTypeObject *)base);
+    type->tp_base = type_incref((PyTypeObject *) base);
     type->tp_basicsize = static_cast<ssize_t>(sizeof(instance));
-    if (!bases.empty())
+    if (!bases.empty()) {
         type->tp_bases = bases.release().ptr();
+    }
 
     /* Don't inherit base __init__ */
     type->tp_init = pybind11_object_init;
 
     /* Supported protocols */
     type->tp_as_number = &heap_type->as_number;
     type->tp_as_sequence = &heap_type->as_sequence;
@@ -670,39 +702,46 @@
 #endif
 
     /* Flags */
     type->tp_flags |= Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HEAPTYPE;
 #if PY_MAJOR_VERSION < 3
     type->tp_flags |= Py_TPFLAGS_CHECKTYPES;
 #endif
-    if (!rec.is_final)
+    if (!rec.is_final) {
         type->tp_flags |= Py_TPFLAGS_BASETYPE;
+    }
 
-    if (rec.dynamic_attr)
+    if (rec.dynamic_attr) {
         enable_dynamic_attributes(heap_type);
+    }
 
-    if (rec.buffer_protocol)
+    if (rec.buffer_protocol) {
         enable_buffer_protocol(heap_type);
+    }
 
-    if (rec.custom_type_setup_callback)
+    if (rec.custom_type_setup_callback) {
         rec.custom_type_setup_callback(heap_type);
+    }
 
-    if (PyType_Ready(type) < 0)
+    if (PyType_Ready(type) < 0) {
         pybind11_fail(std::string(rec.name) + ": PyType_Ready failed (" + error_string() + ")!");
+    }
 
     assert(!rec.dynamic_attr || PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
 
     /* Register type with the parent scope */
-    if (rec.scope)
+    if (rec.scope) {
         setattr(rec.scope, rec.name, (PyObject *) type);
-    else
+    } else {
         Py_INCREF(type); // Keep it alive forever (reference leak)
+    }
 
-    if (module_) // Needed by pydoc
+    if (module_) { // Needed by pydoc
         setattr((PyObject *) type, "__module__", module_);
+    }
 
     PYBIND11_SET_OLDPY_QUALNAME(type, qualname);
 
     return (PyObject *) type;
 }
 
 PYBIND11_NAMESPACE_END(detail)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/common.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/common.h`

 * *Files 5% similar despite different names*

```diff
@@ -7,260 +7,258 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
 #define PYBIND11_VERSION_MINOR 9
-#define PYBIND11_VERSION_PATCH 1
+#define PYBIND11_VERSION_PATCH 2
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x02090100
+#define PYBIND11_VERSION_HEX 0x02090200
 
 #define PYBIND11_NAMESPACE_BEGIN(name) namespace name {
 #define PYBIND11_NAMESPACE_END(name) }
 
 // Robust support for some features and loading modules compiled against different pybind versions
-// requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute on
-// the main `pybind11` namespace.
+// requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute
+// on the main `pybind11` namespace.
 #if !defined(PYBIND11_NAMESPACE)
-#  ifdef __GNUG__
-#    define PYBIND11_NAMESPACE pybind11 __attribute__((visibility("hidden")))
-#  else
-#    define PYBIND11_NAMESPACE pybind11
-#  endif
+#    ifdef __GNUG__
+#        define PYBIND11_NAMESPACE pybind11 __attribute__((visibility("hidden")))
+#    else
+#        define PYBIND11_NAMESPACE pybind11
+#    endif
 #endif
 
 #if !(defined(_MSC_VER) && __cplusplus == 199711L)
-#  if __cplusplus >= 201402L
-#    define PYBIND11_CPP14
-#    if __cplusplus >= 201703L
-#      define PYBIND11_CPP17
-#      if __cplusplus >= 202002L
-#        define PYBIND11_CPP20
-#      endif
+#    if __cplusplus >= 201402L
+#        define PYBIND11_CPP14
+#        if __cplusplus >= 201703L
+#            define PYBIND11_CPP17
+#            if __cplusplus >= 202002L
+#                define PYBIND11_CPP20
+#            endif
+#        endif
 #    endif
-#  endif
 #elif defined(_MSC_VER) && __cplusplus == 199711L
-// MSVC sets _MSVC_LANG rather than __cplusplus (supposedly until the standard is fully implemented)
-// Unless you use the /Zc:__cplusplus flag on Visual Studio 2017 15.7 Preview 3 or newer
-#  if _MSVC_LANG >= 201402L
-#    define PYBIND11_CPP14
-#    if _MSVC_LANG > 201402L && _MSC_VER >= 1910
-#      define PYBIND11_CPP17
-#      if _MSVC_LANG >= 202002L
-#        define PYBIND11_CPP20
-#      endif
+// MSVC sets _MSVC_LANG rather than __cplusplus (supposedly until the standard is fully
+// implemented). Unless you use the /Zc:__cplusplus flag on Visual Studio 2017 15.7 Preview 3
+// or newer.
+#    if _MSVC_LANG >= 201402L
+#        define PYBIND11_CPP14
+#        if _MSVC_LANG > 201402L && _MSC_VER >= 1910
+#            define PYBIND11_CPP17
+#            if _MSVC_LANG >= 202002L
+#                define PYBIND11_CPP20
+#            endif
+#        endif
 #    endif
-#  endif
 #endif
 
 // Compiler version assertions
 #if defined(__INTEL_COMPILER)
-#  if __INTEL_COMPILER < 1800
-#    error pybind11 requires Intel C++ compiler v18 or newer
-#  elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
-#    error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
-#  endif
+#    if __INTEL_COMPILER < 1800
+#        error pybind11 requires Intel C++ compiler v18 or newer
+#    elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
+#        error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
+#    endif
 /* The following pragma cannot be pop'ed:
    https://community.intel.com/t5/Intel-C-Compiler/Inline-and-no-inline-warning/td-p/1216764 */
-#  pragma warning disable 2196 // warning #2196: routine is both "inline" and "noinline"
+#    pragma warning disable 2196 // warning #2196: routine is both "inline" and "noinline"
 #elif defined(__clang__) && !defined(__apple_build_version__)
-#  if __clang_major__ < 3 || (__clang_major__ == 3 && __clang_minor__ < 3)
-#    error pybind11 requires clang 3.3 or newer
-#  endif
+#    if __clang_major__ < 3 || (__clang_major__ == 3 && __clang_minor__ < 3)
+#        error pybind11 requires clang 3.3 or newer
+#    endif
 #elif defined(__clang__)
 // Apple changes clang version macros to its Xcode version; the first Xcode release based on
 // (upstream) clang 3.3 was Xcode 5:
-#  if __clang_major__ < 5
-#    error pybind11 requires Xcode/clang 5.0 or newer
-#  endif
+#    if __clang_major__ < 5
+#        error pybind11 requires Xcode/clang 5.0 or newer
+#    endif
 #elif defined(__GNUG__)
-#  if __GNUC__ < 4 || (__GNUC__ == 4 && __GNUC_MINOR__ < 8)
-#    error pybind11 requires gcc 4.8 or newer
-#  endif
+#    if __GNUC__ < 4 || (__GNUC__ == 4 && __GNUC_MINOR__ < 8)
+#        error pybind11 requires gcc 4.8 or newer
+#    endif
 #elif defined(_MSC_VER)
 // Pybind hits various compiler bugs in 2015u2 and earlier, and also makes use of some stl features
 // (e.g. std::negation) added in 2015u3:
-#  if _MSC_FULL_VER < 190024210
-#    error pybind11 requires MSVC 2015 update 3 or newer
-#  endif
+#    if _MSC_FULL_VER < 190024210
+#        error pybind11 requires MSVC 2015 update 3 or newer
+#    endif
 #endif
 
 #if !defined(PYBIND11_EXPORT)
-#  if defined(WIN32) || defined(_WIN32)
-#    define PYBIND11_EXPORT __declspec(dllexport)
-#  else
-#    define PYBIND11_EXPORT __attribute__ ((visibility("default")))
-#  endif
+#    if defined(WIN32) || defined(_WIN32)
+#        define PYBIND11_EXPORT __declspec(dllexport)
+#    else
+#        define PYBIND11_EXPORT __attribute__((visibility("default")))
+#    endif
 #endif
 
 #if !defined(PYBIND11_EXPORT_EXCEPTION)
-#  ifdef __MINGW32__
+#    ifdef __MINGW32__
 // workaround for:
-// error: 'dllexport' implies default visibility, but xxx has already been declared with a different visibility
-#    define PYBIND11_EXPORT_EXCEPTION
-#  else
-#    define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
-#  endif
+// error: 'dllexport' implies default visibility, but xxx has already been declared with a
+// different visibility
+#        define PYBIND11_EXPORT_EXCEPTION
+#    else
+#        define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
+#    endif
 #endif
 
 // For CUDA, GCC7, GCC8:
 // PYBIND11_NOINLINE_FORCED is incompatible with `-Wattributes -Werror`.
 // When defining PYBIND11_NOINLINE_FORCED, it is best to also use `-Wno-attributes`.
 // However, the measured shared-library size saving when using noinline are only
 // 1.7% for CUDA, -0.2% for GCC7, and 0.0% for GCC8 (using -DCMAKE_BUILD_TYPE=MinSizeRel,
 // the default under pybind11/tests).
-#if !defined(PYBIND11_NOINLINE_FORCED) && \
-    (defined(__CUDACC__) || (defined(__GNUC__) && (__GNUC__ == 7 || __GNUC__ == 8)))
-#  define PYBIND11_NOINLINE_DISABLED
+#if !defined(PYBIND11_NOINLINE_FORCED)                                                            \
+    && (defined(__CUDACC__) || (defined(__GNUC__) && (__GNUC__ == 7 || __GNUC__ == 8)))
+#    define PYBIND11_NOINLINE_DISABLED
 #endif
 
 // The PYBIND11_NOINLINE macro is for function DEFINITIONS.
 // In contrast, FORWARD DECLARATIONS should never use this macro:
 // https://stackoverflow.com/questions/9317473/forward-declaration-of-inline-functions
 #if defined(PYBIND11_NOINLINE_DISABLED) // Option for maximum portability and experimentation.
-#  define PYBIND11_NOINLINE inline
+#    define PYBIND11_NOINLINE inline
 #elif defined(_MSC_VER)
-#  define PYBIND11_NOINLINE __declspec(noinline) inline
+#    define PYBIND11_NOINLINE __declspec(noinline) inline
 #else
-#  define PYBIND11_NOINLINE __attribute__ ((noinline)) inline
+#    define PYBIND11_NOINLINE __attribute__((noinline)) inline
 #endif
 
 #if defined(__MINGW32__)
 // For unknown reasons all PYBIND11_DEPRECATED member trigger a warning when declared
 // whether it is used or not
-#  define PYBIND11_DEPRECATED(reason)
+#    define PYBIND11_DEPRECATED(reason)
 #elif defined(PYBIND11_CPP14)
-#  define PYBIND11_DEPRECATED(reason) [[deprecated(reason)]]
+#    define PYBIND11_DEPRECATED(reason) [[deprecated(reason)]]
 #else
-#  define PYBIND11_DEPRECATED(reason) __attribute__((deprecated(reason)))
+#    define PYBIND11_DEPRECATED(reason) __attribute__((deprecated(reason)))
 #endif
 
 #if defined(PYBIND11_CPP17)
-#  define PYBIND11_MAYBE_UNUSED [[maybe_unused]]
+#    define PYBIND11_MAYBE_UNUSED [[maybe_unused]]
 #elif defined(_MSC_VER) && !defined(__clang__)
-#  define PYBIND11_MAYBE_UNUSED
+#    define PYBIND11_MAYBE_UNUSED
 #else
-#  define PYBIND11_MAYBE_UNUSED __attribute__ ((__unused__))
+#    define PYBIND11_MAYBE_UNUSED __attribute__((__unused__))
 #endif
 
 /* Don't let Python.h #define (v)snprintf as macro because they are implemented
    properly in Visual Studio since 2015. */
 #if defined(_MSC_VER) && _MSC_VER >= 1900
-#  define HAVE_SNPRINTF 1
+#    define HAVE_SNPRINTF 1
 #endif
 
 /// Include Python header, disable linking to pythonX_d.lib on Windows in debug mode
 #if defined(_MSC_VER)
-#  if (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION < 4)
-#    define HAVE_ROUND 1
-#  endif
-#  pragma warning(push)
+#    pragma warning(push)
 // C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
-#  pragma warning(disable: 4505)
-#  if defined(_DEBUG) && !defined(Py_DEBUG)
+#    pragma warning(disable : 4505)
+#    if defined(_DEBUG) && !defined(Py_DEBUG)
 // Workaround for a VS 2022 issue.
 // NOTE: This workaround knowingly violates the Python.h include order requirement:
 // https://docs.python.org/3/c-api/intro.html#include-files
 // See https://github.com/pybind/pybind11/pull/3497 for full context.
-#    include <yvals.h>
-#    if _MSVC_STL_VERSION >= 143
-#      include <crtdefs.h>
+#        include <yvals.h>
+#        if _MSVC_STL_VERSION >= 143
+#            include <crtdefs.h>
+#        endif
+#        define PYBIND11_DEBUG_MARKER
+#        undef _DEBUG
 #    endif
-#    define PYBIND11_DEBUG_MARKER
-#    undef _DEBUG
-#  endif
 #endif
 
 // https://en.cppreference.com/w/c/chrono/localtime
 #if defined(__STDC_LIB_EXT1__) && !defined(__STDC_WANT_LIB_EXT1__)
-#  define __STDC_WANT_LIB_EXT1__
+#    define __STDC_WANT_LIB_EXT1__
 #endif
 
 #ifdef __has_include
 // std::optional (but including it in c++14 mode isn't allowed)
-#  if defined(PYBIND11_CPP17) && __has_include(<optional>)
-#    define PYBIND11_HAS_OPTIONAL 1
-#  endif
+#    if defined(PYBIND11_CPP17) && __has_include(<optional>)
+#        define PYBIND11_HAS_OPTIONAL 1
+#    endif
 // std::experimental::optional (but not allowed in c++11 mode)
-#  if defined(PYBIND11_CPP14) && (__has_include(<experimental/optional>) && \
+#    if defined(PYBIND11_CPP14) && (__has_include(<experimental/optional>) && \
                                  !__has_include(<optional>))
-#    define PYBIND11_HAS_EXP_OPTIONAL 1
-#  endif
+#        define PYBIND11_HAS_EXP_OPTIONAL 1
+#    endif
 // std::variant
-#  if defined(PYBIND11_CPP17) && __has_include(<variant>)
-#    define PYBIND11_HAS_VARIANT 1
-#  endif
+#    if defined(PYBIND11_CPP17) && __has_include(<variant>)
+#        define PYBIND11_HAS_VARIANT 1
+#    endif
 #elif defined(_MSC_VER) && defined(PYBIND11_CPP17)
-#  define PYBIND11_HAS_OPTIONAL 1
-#  define PYBIND11_HAS_VARIANT 1
+#    define PYBIND11_HAS_OPTIONAL 1
+#    define PYBIND11_HAS_VARIANT 1
 #endif
 
 #if defined(PYBIND11_CPP17)
-#  if defined(__has_include)
-#    if __has_include(<string_view>)
-#      define PYBIND11_HAS_STRING_VIEW
+#    if defined(__has_include)
+#        if __has_include(<string_view>)
+#            define PYBIND11_HAS_STRING_VIEW
+#        endif
+#    elif defined(_MSC_VER)
+#        define PYBIND11_HAS_STRING_VIEW
 #    endif
-#  elif defined(_MSC_VER)
-#    define PYBIND11_HAS_STRING_VIEW
-#  endif
 #endif
 
 #if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
-#  define PYBIND11_HAS_U8STRING
+#    define PYBIND11_HAS_U8STRING
 #endif
 
-
 #include <Python.h>
 #include <frameobject.h>
 #include <pythread.h>
 
 /* Python #defines overrides on all sorts of core functions, which
    tends to weak havok in C++ codebases that expect these to work
    like regular functions (potentially with several overloads) */
 #if defined(isalnum)
-#  undef isalnum
-#  undef isalpha
-#  undef islower
-#  undef isspace
-#  undef isupper
-#  undef tolower
-#  undef toupper
+#    undef isalnum
+#    undef isalpha
+#    undef islower
+#    undef isspace
+#    undef isupper
+#    undef tolower
+#    undef toupper
 #endif
 
 #if defined(copysign)
-#  undef copysign
+#    undef copysign
 #endif
 
 #if defined(_MSC_VER)
-#  if defined(PYBIND11_DEBUG_MARKER)
-#    define _DEBUG
-#    undef PYBIND11_DEBUG_MARKER
-#  endif
-#  pragma warning(pop)
+#    if defined(PYBIND11_DEBUG_MARKER)
+#        define _DEBUG
+#        undef PYBIND11_DEBUG_MARKER
+#    endif
+#    pragma warning(pop)
 #endif
 
 #include <cstddef>
 #include <cstring>
-#include <forward_list>
-#include <vector>
-#include <string>
-#include <stdexcept>
 #include <exception>
-#include <unordered_set>
-#include <unordered_map>
+#include <forward_list>
 #include <memory>
-#include <typeindex>
+#include <stdexcept>
+#include <string>
 #include <type_traits>
+#include <typeindex>
+#include <unordered_map>
+#include <unordered_set>
+#include <vector>
 #if defined(__has_include)
-#  if __has_include(<version>)
-#    include <version>
-#  endif
+#    if __has_include(<version>)
+#        include <version>
+#    endif
 #endif
 
 // #define PYBIND11_STR_LEGACY_PERMISSIVE
 // If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
 //             (probably surprising and never documented, but this was the
 //             legacy behavior until and including v2.6.x). As a side-effect,
 //             pybind11::isinstance<str>() is true for both pybind11::str and
@@ -269,125 +267,128 @@
 //               pybind11::isinstance<str>() is true only for pybind11::str.
 //               However, for Python 2 only (!), the pybind11::str caster
 //               implicitly decodes bytes to PyUnicodeObject. This is to ease
 //               the transition from the legacy behavior to the non-permissive
 //               behavior.
 
 #if PY_MAJOR_VERSION >= 3 /// Compatibility macros for various Python versions
-#define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyInstanceMethod_New(ptr)
-#define PYBIND11_INSTANCE_METHOD_CHECK PyInstanceMethod_Check
-#define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyInstanceMethod_GET_FUNCTION
-#define PYBIND11_BYTES_CHECK PyBytes_Check
-#define PYBIND11_BYTES_FROM_STRING PyBytes_FromString
-#define PYBIND11_BYTES_FROM_STRING_AND_SIZE PyBytes_FromStringAndSize
-#define PYBIND11_BYTES_AS_STRING_AND_SIZE PyBytes_AsStringAndSize
-#define PYBIND11_BYTES_AS_STRING PyBytes_AsString
-#define PYBIND11_BYTES_SIZE PyBytes_Size
-#define PYBIND11_LONG_CHECK(o) PyLong_Check(o)
-#define PYBIND11_LONG_AS_LONGLONG(o) PyLong_AsLongLong(o)
-#define PYBIND11_LONG_FROM_SIGNED(o) PyLong_FromSsize_t((ssize_t) (o))
-#define PYBIND11_LONG_FROM_UNSIGNED(o) PyLong_FromSize_t((size_t) (o))
-#define PYBIND11_BYTES_NAME "bytes"
-#define PYBIND11_STRING_NAME "str"
-#define PYBIND11_SLICE_OBJECT PyObject
-#define PYBIND11_FROM_STRING PyUnicode_FromString
-#define PYBIND11_STR_TYPE ::pybind11::str
-#define PYBIND11_BOOL_ATTR "__bool__"
-#define PYBIND11_NB_BOOL(ptr) ((ptr)->nb_bool)
-#define PYBIND11_BUILTINS_MODULE "builtins"
+#    define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyInstanceMethod_New(ptr)
+#    define PYBIND11_INSTANCE_METHOD_CHECK PyInstanceMethod_Check
+#    define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyInstanceMethod_GET_FUNCTION
+#    define PYBIND11_BYTES_CHECK PyBytes_Check
+#    define PYBIND11_BYTES_FROM_STRING PyBytes_FromString
+#    define PYBIND11_BYTES_FROM_STRING_AND_SIZE PyBytes_FromStringAndSize
+#    define PYBIND11_BYTES_AS_STRING_AND_SIZE PyBytes_AsStringAndSize
+#    define PYBIND11_BYTES_AS_STRING PyBytes_AsString
+#    define PYBIND11_BYTES_SIZE PyBytes_Size
+#    define PYBIND11_LONG_CHECK(o) PyLong_Check(o)
+#    define PYBIND11_LONG_AS_LONGLONG(o) PyLong_AsLongLong(o)
+#    define PYBIND11_LONG_FROM_SIGNED(o) PyLong_FromSsize_t((ssize_t) (o))
+#    define PYBIND11_LONG_FROM_UNSIGNED(o) PyLong_FromSize_t((size_t) (o))
+#    define PYBIND11_BYTES_NAME "bytes"
+#    define PYBIND11_STRING_NAME "str"
+#    define PYBIND11_SLICE_OBJECT PyObject
+#    define PYBIND11_FROM_STRING PyUnicode_FromString
+#    define PYBIND11_STR_TYPE ::pybind11::str
+#    define PYBIND11_BOOL_ATTR "__bool__"
+#    define PYBIND11_NB_BOOL(ptr) ((ptr)->nb_bool)
+#    define PYBIND11_BUILTINS_MODULE "builtins"
 // Providing a separate declaration to make Clang's -Wmissing-prototypes happy.
 // See comment for PYBIND11_MODULE below for why this is marked "maybe unused".
-#define PYBIND11_PLUGIN_IMPL(name) \
-    extern "C" PYBIND11_MAYBE_UNUSED PYBIND11_EXPORT PyObject *PyInit_##name(); \
-    extern "C" PYBIND11_EXPORT PyObject *PyInit_##name()
+#    define PYBIND11_PLUGIN_IMPL(name)                                                            \
+        extern "C" PYBIND11_MAYBE_UNUSED PYBIND11_EXPORT PyObject *PyInit_##name();               \
+        extern "C" PYBIND11_EXPORT PyObject *PyInit_##name()
 
 #else
-#define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyMethod_New(ptr, nullptr, class_)
-#define PYBIND11_INSTANCE_METHOD_CHECK PyMethod_Check
-#define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyMethod_GET_FUNCTION
-#define PYBIND11_BYTES_CHECK PyString_Check
-#define PYBIND11_BYTES_FROM_STRING PyString_FromString
-#define PYBIND11_BYTES_FROM_STRING_AND_SIZE PyString_FromStringAndSize
-#define PYBIND11_BYTES_AS_STRING_AND_SIZE PyString_AsStringAndSize
-#define PYBIND11_BYTES_AS_STRING PyString_AsString
-#define PYBIND11_BYTES_SIZE PyString_Size
-#define PYBIND11_LONG_CHECK(o) (PyInt_Check(o) || PyLong_Check(o))
-#define PYBIND11_LONG_AS_LONGLONG(o) (PyInt_Check(o) ? (long long) PyLong_AsLong(o) : PyLong_AsLongLong(o))
-#define PYBIND11_LONG_FROM_SIGNED(o) PyInt_FromSsize_t((ssize_t) o) // Returns long if needed.
-#define PYBIND11_LONG_FROM_UNSIGNED(o) PyInt_FromSize_t((size_t) o) // Returns long if needed.
-#define PYBIND11_BYTES_NAME "str"
-#define PYBIND11_STRING_NAME "unicode"
-#define PYBIND11_SLICE_OBJECT PySliceObject
-#define PYBIND11_FROM_STRING PyString_FromString
-#define PYBIND11_STR_TYPE ::pybind11::bytes
-#define PYBIND11_BOOL_ATTR "__nonzero__"
-#define PYBIND11_NB_BOOL(ptr) ((ptr)->nb_nonzero)
-#define PYBIND11_BUILTINS_MODULE "__builtin__"
+#    define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyMethod_New(ptr, nullptr, class_)
+#    define PYBIND11_INSTANCE_METHOD_CHECK PyMethod_Check
+#    define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyMethod_GET_FUNCTION
+#    define PYBIND11_BYTES_CHECK PyString_Check
+#    define PYBIND11_BYTES_FROM_STRING PyString_FromString
+#    define PYBIND11_BYTES_FROM_STRING_AND_SIZE PyString_FromStringAndSize
+#    define PYBIND11_BYTES_AS_STRING_AND_SIZE PyString_AsStringAndSize
+#    define PYBIND11_BYTES_AS_STRING PyString_AsString
+#    define PYBIND11_BYTES_SIZE PyString_Size
+#    define PYBIND11_LONG_CHECK(o) (PyInt_Check(o) || PyLong_Check(o))
+#    define PYBIND11_LONG_AS_LONGLONG(o)                                                          \
+        (PyInt_Check(o) ? (long long) PyLong_AsLong(o) : PyLong_AsLongLong(o))
+#    define PYBIND11_LONG_FROM_SIGNED(o) PyInt_FromSsize_t((ssize_t) o) // Returns long if needed.
+#    define PYBIND11_LONG_FROM_UNSIGNED(o) PyInt_FromSize_t((size_t) o) // Returns long if needed.
+#    define PYBIND11_BYTES_NAME "str"
+#    define PYBIND11_STRING_NAME "unicode"
+#    define PYBIND11_SLICE_OBJECT PySliceObject
+#    define PYBIND11_FROM_STRING PyString_FromString
+#    define PYBIND11_STR_TYPE ::pybind11::bytes
+#    define PYBIND11_BOOL_ATTR "__nonzero__"
+#    define PYBIND11_NB_BOOL(ptr) ((ptr)->nb_nonzero)
+#    define PYBIND11_BUILTINS_MODULE "__builtin__"
 // Providing a separate PyInit decl to make Clang's -Wmissing-prototypes happy.
 // See comment for PYBIND11_MODULE below for why this is marked "maybe unused".
-#define PYBIND11_PLUGIN_IMPL(name) \
-    static PyObject *pybind11_init_wrapper();                           \
-    extern "C" PYBIND11_MAYBE_UNUSED PYBIND11_EXPORT void init##name(); \
-    extern "C" PYBIND11_EXPORT void init##name() {                      \
-        (void)pybind11_init_wrapper();                                  \
-    }                                                                   \
-    PyObject *pybind11_init_wrapper()
+#    define PYBIND11_PLUGIN_IMPL(name)                                                            \
+        static PyObject *pybind11_init_wrapper();                                                 \
+        extern "C" PYBIND11_MAYBE_UNUSED PYBIND11_EXPORT void init##name();                       \
+        extern "C" PYBIND11_EXPORT void init##name() { (void) pybind11_init_wrapper(); }          \
+        PyObject *pybind11_init_wrapper()
 #endif
 
 #if PY_VERSION_HEX >= 0x03050000 && PY_VERSION_HEX < 0x03050200
 extern "C" {
-    struct _Py_atomic_address { void *value; };
-    PyAPI_DATA(_Py_atomic_address) _PyThreadState_Current;
+struct _Py_atomic_address {
+    void *value;
+};
+PyAPI_DATA(_Py_atomic_address) _PyThreadState_Current;
 }
 #endif
 
 #define PYBIND11_TRY_NEXT_OVERLOAD ((PyObject *) 1) // special failure return code
 #define PYBIND11_STRINGIFY(x) #x
 #define PYBIND11_TOSTRING(x) PYBIND11_STRINGIFY(x)
 #define PYBIND11_CONCAT(first, second) first##second
-#define PYBIND11_ENSURE_INTERNALS_READY \
-    pybind11::detail::get_internals();
+#define PYBIND11_ENSURE_INTERNALS_READY pybind11::detail::get_internals();
 
-#define PYBIND11_CHECK_PYTHON_VERSION \
-    {                                                                          \
-        const char *compiled_ver = PYBIND11_TOSTRING(PY_MAJOR_VERSION)         \
-            "." PYBIND11_TOSTRING(PY_MINOR_VERSION);                           \
-        const char *runtime_ver = Py_GetVersion();                             \
-        size_t len = std::strlen(compiled_ver);                                \
-        if (std::strncmp(runtime_ver, compiled_ver, len) != 0                  \
-                || (runtime_ver[len] >= '0' && runtime_ver[len] <= '9')) {     \
-            PyErr_Format(PyExc_ImportError,                                    \
-                "Python version mismatch: module was compiled for Python %s, " \
-                "but the interpreter version is incompatible: %s.",            \
-                compiled_ver, runtime_ver);                                    \
-            return nullptr;                                                    \
-        }                                                                      \
+#define PYBIND11_CHECK_PYTHON_VERSION                                                             \
+    {                                                                                             \
+        const char *compiled_ver                                                                  \
+            = PYBIND11_TOSTRING(PY_MAJOR_VERSION) "." PYBIND11_TOSTRING(PY_MINOR_VERSION);        \
+        const char *runtime_ver = Py_GetVersion();                                                \
+        size_t len = std::strlen(compiled_ver);                                                   \
+        if (std::strncmp(runtime_ver, compiled_ver, len) != 0                                     \
+            || (runtime_ver[len] >= '0' && runtime_ver[len] <= '9')) {                            \
+            PyErr_Format(PyExc_ImportError,                                                       \
+                         "Python version mismatch: module was compiled for Python %s, "           \
+                         "but the interpreter version is incompatible: %s.",                      \
+                         compiled_ver,                                                            \
+                         runtime_ver);                                                            \
+            return nullptr;                                                                       \
+        }                                                                                         \
     }
 
 #if PY_VERSION_HEX >= 0x03030000
 
-#define PYBIND11_CATCH_INIT_EXCEPTIONS \
-        catch (pybind11::error_already_set &e) {                                 \
-            pybind11::raise_from(e, PyExc_ImportError, "initialization failed"); \
-            return nullptr;                                                      \
-        } catch (const std::exception &e) {                                      \
-            PyErr_SetString(PyExc_ImportError, e.what());                        \
-            return nullptr;                                                      \
-        }                                                                        \
+#    define PYBIND11_CATCH_INIT_EXCEPTIONS                                                        \
+        catch (pybind11::error_already_set & e) {                                                 \
+            pybind11::raise_from(e, PyExc_ImportError, "initialization failed");                  \
+            return nullptr;                                                                       \
+        }                                                                                         \
+        catch (const std::exception &e) {                                                         \
+            PyErr_SetString(PyExc_ImportError, e.what());                                         \
+            return nullptr;                                                                       \
+        }
 
 #else
 
-#define PYBIND11_CATCH_INIT_EXCEPTIONS \
-        catch (pybind11::error_already_set &e) {                               \
-            PyErr_SetString(PyExc_ImportError, e.what());                      \
-            return nullptr;                                                    \
-        } catch (const std::exception &e) {                                    \
-            PyErr_SetString(PyExc_ImportError, e.what());                      \
-            return nullptr;                                                    \
-        }                                                                      \
+#    define PYBIND11_CATCH_INIT_EXCEPTIONS                                                        \
+        catch (pybind11::error_already_set & e) {                                                 \
+            PyErr_SetString(PyExc_ImportError, e.what());                                         \
+            return nullptr;                                                                       \
+        }                                                                                         \
+        catch (const std::exception &e) {                                                         \
+            PyErr_SetString(PyExc_ImportError, e.what());                                         \
+            return nullptr;                                                                       \
+        }
 
 #endif
 
 /** \rst
     ***Deprecated in favor of PYBIND11_MODULE***
 
     This macro creates the entry point that will be invoked when the Python interpreter
@@ -398,24 +399,25 @@
 
         PYBIND11_PLUGIN(example) {
             pybind11::module_ m("example", "pybind11 example plugin");
             /// Set up bindings here
             return m.ptr();
         }
 \endrst */
-#define PYBIND11_PLUGIN(name)                                                  \
-    PYBIND11_DEPRECATED("PYBIND11_PLUGIN is deprecated, use PYBIND11_MODULE")  \
-    static PyObject *pybind11_init();                                          \
-    PYBIND11_PLUGIN_IMPL(name) {                                               \
-        PYBIND11_CHECK_PYTHON_VERSION                                          \
-        PYBIND11_ENSURE_INTERNALS_READY                                        \
-        try {                                                                  \
-            return pybind11_init();                                            \
-        } PYBIND11_CATCH_INIT_EXCEPTIONS                                       \
-    }                                                                          \
+#define PYBIND11_PLUGIN(name)                                                                     \
+    PYBIND11_DEPRECATED("PYBIND11_PLUGIN is deprecated, use PYBIND11_MODULE")                     \
+    static PyObject *pybind11_init();                                                             \
+    PYBIND11_PLUGIN_IMPL(name) {                                                                  \
+        PYBIND11_CHECK_PYTHON_VERSION                                                             \
+        PYBIND11_ENSURE_INTERNALS_READY                                                           \
+        try {                                                                                     \
+            return pybind11_init();                                                               \
+        }                                                                                         \
+        PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
+    }                                                                                             \
     PyObject *pybind11_init()
 
 /** \rst
     This macro creates the entry point that will be invoked when the Python interpreter
     imports an extension module. The module name is given as the fist argument and it
     should not be in quotes. The second macro argument defines a variable of type
     `py::module_` which can be used to initialize the module.
@@ -452,15 +454,15 @@
         PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     }                                                                                             \
     void PYBIND11_CONCAT(pybind11_init_, name)(::pybind11::module_ & (variable))
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ssize_t = Py_ssize_t;
-using size_t  = std::size_t;
+using size_t = std::size_t;
 
 template <typename IntType>
 inline ssize_t ssize_t_cast(const IntType &val) {
     static_assert(sizeof(IntType) <= sizeof(ssize_t), "Implicit narrowing is not permitted.");
     return static_cast<ssize_t>(val);
 }
 
@@ -514,28 +516,32 @@
         variations of this scheme are also possible using combinations of
         return_value_policy::reference and the keep_alive call policy */
     reference_internal
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-inline static constexpr int log2(size_t n, int k = 0) { return (n <= 1) ? k : log2(n >> 1, k + 1); }
+inline static constexpr int log2(size_t n, int k = 0) {
+    return (n <= 1) ? k : log2(n >> 1, k + 1);
+}
 
 // Returns the size as a multiple of sizeof(void *), rounded up.
-inline static constexpr size_t size_in_ptrs(size_t s) { return 1 + ((s - 1) >> log2(sizeof(void *))); }
+inline static constexpr size_t size_in_ptrs(size_t s) {
+    return 1 + ((s - 1) >> log2(sizeof(void *)));
+}
 
 /**
  * The space to allocate for simple layout instance holders (see below) in multiple of the size of
  * a pointer (e.g.  2 means 16 bytes on 64-bit architectures).  The default is the minimum required
  * to holder either a std::unique_ptr or std::shared_ptr (which is almost always
  * sizeof(std::shared_ptr<T>)).
  */
 constexpr size_t instance_simple_holder_in_ptrs() {
     static_assert(sizeof(std::shared_ptr<int>) >= sizeof(std::unique_ptr<int>),
-            "pybind assumes std::shared_ptrs are at least as big as std::unique_ptrs");
+                  "pybind assumes std::shared_ptrs are at least as big as std::unique_ptrs");
     return size_in_ptrs(sizeof(std::shared_ptr<int>));
 }
 
 // Forward declarations
 struct type_info;
 struct value_and_holder;
 
@@ -555,71 +561,78 @@
     /// Weak references
     PyObject *weakrefs;
     /// If true, the pointer is owned which means we're free to manage it with a holder.
     bool owned : 1;
     /**
      * An instance has two possible value/holder layouts.
      *
-     * Simple layout (when this flag is true), means the `simple_value_holder` is set with a pointer
-     * and the holder object governing that pointer, i.e. [val1*][holder].  This layout is applied
-     * whenever there is no python-side multiple inheritance of bound C++ types *and* the type's
-     * holder will fit in the default space (which is large enough to hold either a std::unique_ptr
-     * or std::shared_ptr).
+     * Simple layout (when this flag is true), means the `simple_value_holder` is set with a
+     * pointer and the holder object governing that pointer, i.e. [val1*][holder].  This layout is
+     * applied whenever there is no python-side multiple inheritance of bound C++ types *and* the
+     * type's holder will fit in the default space (which is large enough to hold either a
+     * std::unique_ptr or std::shared_ptr).
      *
-     * Non-simple layout applies when using custom holders that require more space than `shared_ptr`
-     * (which is typically the size of two pointers), or when multiple inheritance is used on the
-     * python side.  Non-simple layout allocates the required amount of memory to have multiple
-     * bound C++ classes as parents.  Under this layout, `nonsimple.values_and_holders` is set to a
-     * pointer to allocated space of the required space to hold a sequence of value pointers and
-     * holders followed `status`, a set of bit flags (1 byte each), i.e.
-     * [val1*][holder1][val2*][holder2]...[bb...]  where each [block] is rounded up to a multiple of
-     * `sizeof(void *)`.  `nonsimple.status` is, for convenience, a pointer to the
-     * beginning of the [bb...] block (but not independently allocated).
+     * Non-simple layout applies when using custom holders that require more space than
+     * `shared_ptr` (which is typically the size of two pointers), or when multiple inheritance is
+     * used on the python side.  Non-simple layout allocates the required amount of memory to have
+     * multiple bound C++ classes as parents.  Under this layout, `nonsimple.values_and_holders` is
+     * set to a pointer to allocated space of the required space to hold a sequence of value
+     * pointers and holders followed `status`, a set of bit flags (1 byte each), i.e.
+     * [val1*][holder1][val2*][holder2]...[bb...]  where each [block] is rounded up to a multiple
+     * of `sizeof(void *)`.  `nonsimple.status` is, for convenience, a pointer to the beginning of
+     * the [bb...] block (but not independently allocated).
      *
      * Status bits indicate whether the associated holder is constructed (&
      * status_holder_constructed) and whether the value pointer is registered (&
      * status_instance_registered) in `registered_instances`.
      */
     bool simple_layout : 1;
     /// For simple layout, tracks whether the holder has been constructed
     bool simple_holder_constructed : 1;
     /// For simple layout, tracks whether the instance is registered in `registered_instances`
     bool simple_instance_registered : 1;
     /// If true, get_internals().patients has an entry for this object
     bool has_patients : 1;
 
-    /// Initializes all of the above type/values/holders data (but not the instance values themselves)
+    /// Initializes all of the above type/values/holders data (but not the instance values
+    /// themselves)
     void allocate_layout();
 
     /// Destroys/deallocates all of the above
     void deallocate_layout();
 
     /// Returns the value_and_holder wrapper for the given type (or the first, if `find_type`
     /// omitted).  Returns a default-constructed (with `.inst = nullptr`) object on failure if
     /// `throw_if_missing` is false.
-    value_and_holder get_value_and_holder(const type_info *find_type = nullptr, bool throw_if_missing = true);
+    value_and_holder get_value_and_holder(const type_info *find_type = nullptr,
+                                          bool throw_if_missing = true);
 
     /// Bit values for the non-simple status flags
-    static constexpr uint8_t status_holder_constructed  = 1;
+    static constexpr uint8_t status_holder_constructed = 1;
     static constexpr uint8_t status_instance_registered = 2;
 };
 
-static_assert(std::is_standard_layout<instance>::value, "Internal error: `pybind11::detail::instance` is not standard layout!");
+static_assert(std::is_standard_layout<instance>::value,
+              "Internal error: `pybind11::detail::instance` is not standard layout!");
 
 /// from __cpp_future__ import (convenient aliases from C++14/17)
 #if defined(PYBIND11_CPP14) && (!defined(_MSC_VER) || _MSC_VER >= 1910)
-using std::enable_if_t;
 using std::conditional_t;
+using std::enable_if_t;
 using std::remove_cv_t;
 using std::remove_reference_t;
 #else
-template <bool B, typename T = void> using enable_if_t = typename std::enable_if<B, T>::type;
-template <bool B, typename T, typename F> using conditional_t = typename std::conditional<B, T, F>::type;
-template <typename T> using remove_cv_t = typename std::remove_cv<T>::type;
-template <typename T> using remove_reference_t = typename std::remove_reference<T>::type;
+template <bool B, typename T = void>
+using enable_if_t = typename std::enable_if<B, T>::type;
+template <bool B, typename T, typename F>
+using conditional_t = typename std::conditional<B, T, F>::type;
+template <typename T>
+using remove_cv_t = typename std::remove_cv<T>::type;
+template <typename T>
+using remove_reference_t = typename std::remove_reference<T>::type;
 #endif
 
 #if defined(PYBIND11_CPP20)
 using std::remove_cvref;
 using std::remove_cvref_t;
 #else
 template <class T>
@@ -631,369 +644,501 @@
 #endif
 
 /// Index sequences
 #if defined(PYBIND11_CPP14)
 using std::index_sequence;
 using std::make_index_sequence;
 #else
-template<size_t ...> struct index_sequence  { };
-template<size_t N, size_t ...S> struct make_index_sequence_impl : make_index_sequence_impl <N - 1, N - 1, S...> { };
-template<size_t ...S> struct make_index_sequence_impl <0, S...> { using type = index_sequence<S...>; };
-template<size_t N> using make_index_sequence = typename make_index_sequence_impl<N>::type;
+template <size_t...>
+struct index_sequence {};
+template <size_t N, size_t... S>
+struct make_index_sequence_impl : make_index_sequence_impl<N - 1, N - 1, S...> {};
+template <size_t... S>
+struct make_index_sequence_impl<0, S...> {
+    using type = index_sequence<S...>;
+};
+template <size_t N>
+using make_index_sequence = typename make_index_sequence_impl<N>::type;
 #endif
 
 /// Make an index sequence of the indices of true arguments
-template <typename ISeq, size_t, bool...> struct select_indices_impl { using type = ISeq; };
-template <size_t... IPrev, size_t I, bool B, bool... Bs> struct select_indices_impl<index_sequence<IPrev...>, I, B, Bs...>
-    : select_indices_impl<conditional_t<B, index_sequence<IPrev..., I>, index_sequence<IPrev...>>, I + 1, Bs...> {};
-template <bool... Bs> using select_indices = typename select_indices_impl<index_sequence<>, 0, Bs...>::type;
+template <typename ISeq, size_t, bool...>
+struct select_indices_impl {
+    using type = ISeq;
+};
+template <size_t... IPrev, size_t I, bool B, bool... Bs>
+struct select_indices_impl<index_sequence<IPrev...>, I, B, Bs...>
+    : select_indices_impl<conditional_t<B, index_sequence<IPrev..., I>, index_sequence<IPrev...>>,
+                          I + 1,
+                          Bs...> {};
+template <bool... Bs>
+using select_indices = typename select_indices_impl<index_sequence<>, 0, Bs...>::type;
 
 /// Backports of std::bool_constant and std::negation to accommodate older compilers
-template <bool B> using bool_constant = std::integral_constant<bool, B>;
-template <typename T> struct negation : bool_constant<!T::value> { };
+template <bool B>
+using bool_constant = std::integral_constant<bool, B>;
+template <typename T>
+struct negation : bool_constant<!T::value> {};
 
 // PGI/Intel cannot detect operator delete with the "compatible" void_t impl, so
 // using the new one (C++14 defect, so generally works on newer compilers, even
 // if not in C++17 mode)
 #if defined(__PGIC__) || defined(__INTEL_COMPILER)
-template<typename... > using void_t = void;
+template <typename...>
+using void_t = void;
 #else
-template <typename...> struct void_t_impl { using type = void; };
-template <typename... Ts> using void_t = typename void_t_impl<Ts...>::type;
+template <typename...>
+struct void_t_impl {
+    using type = void;
+};
+template <typename... Ts>
+using void_t = typename void_t_impl<Ts...>::type;
 #endif
 
-
 /// Compile-time all/any/none of that check the boolean value of all template types
 #if defined(__cpp_fold_expressions) && !(defined(_MSC_VER) && (_MSC_VER < 1916))
-template <class... Ts> using all_of = bool_constant<(Ts::value && ...)>;
-template <class... Ts> using any_of = bool_constant<(Ts::value || ...)>;
+template <class... Ts>
+using all_of = bool_constant<(Ts::value && ...)>;
+template <class... Ts>
+using any_of = bool_constant<(Ts::value || ...)>;
 #elif !defined(_MSC_VER)
-template <bool...> struct bools {};
-template <class... Ts> using all_of = std::is_same<
-    bools<Ts::value..., true>,
-    bools<true, Ts::value...>>;
-template <class... Ts> using any_of = negation<all_of<negation<Ts>...>>;
+template <bool...>
+struct bools {};
+template <class... Ts>
+using all_of = std::is_same<bools<Ts::value..., true>, bools<true, Ts::value...>>;
+template <class... Ts>
+using any_of = negation<all_of<negation<Ts>...>>;
 #else
 // MSVC has trouble with the above, but supports std::conjunction, which we can use instead (albeit
 // at a slight loss of compilation efficiency).
-template <class... Ts> using all_of = std::conjunction<Ts...>;
-template <class... Ts> using any_of = std::disjunction<Ts...>;
-#endif
-template <class... Ts> using none_of = negation<any_of<Ts...>>;
-
-template <class T, template<class> class... Predicates> using satisfies_all_of = all_of<Predicates<T>...>;
-template <class T, template<class> class... Predicates> using satisfies_any_of = any_of<Predicates<T>...>;
-template <class T, template<class> class... Predicates> using satisfies_none_of = none_of<Predicates<T>...>;
+template <class... Ts>
+using all_of = std::conjunction<Ts...>;
+template <class... Ts>
+using any_of = std::disjunction<Ts...>;
+#endif
+template <class... Ts>
+using none_of = negation<any_of<Ts...>>;
+
+template <class T, template <class> class... Predicates>
+using satisfies_all_of = all_of<Predicates<T>...>;
+template <class T, template <class> class... Predicates>
+using satisfies_any_of = any_of<Predicates<T>...>;
+template <class T, template <class> class... Predicates>
+using satisfies_none_of = none_of<Predicates<T>...>;
 
 /// Strip the class from a method type
-template <typename T> struct remove_class { };
-template <typename C, typename R, typename... A> struct remove_class<R (C::*)(A...)> { using type = R (A...); };
-template <typename C, typename R, typename... A> struct remove_class<R (C::*)(A...) const> { using type = R (A...); };
+template <typename T>
+struct remove_class {};
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...)> {
+    using type = R(A...);
+};
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...) const> {
+    using type = R(A...);
+};
 
 /// Helper template to strip away type modifiers
-template <typename T> struct intrinsic_type                       { using type = T; };
-template <typename T> struct intrinsic_type<const T>              { using type = typename intrinsic_type<T>::type; };
-template <typename T> struct intrinsic_type<T*>                   { using type = typename intrinsic_type<T>::type; };
-template <typename T> struct intrinsic_type<T&>                   { using type = typename intrinsic_type<T>::type; };
-template <typename T> struct intrinsic_type<T&&>                  { using type = typename intrinsic_type<T>::type; };
-template <typename T, size_t N> struct intrinsic_type<const T[N]> { using type = typename intrinsic_type<T>::type; };
-template <typename T, size_t N> struct intrinsic_type<T[N]>       { using type = typename intrinsic_type<T>::type; };
-template <typename T> using intrinsic_t = typename intrinsic_type<T>::type;
+template <typename T>
+struct intrinsic_type {
+    using type = T;
+};
+template <typename T>
+struct intrinsic_type<const T> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T>
+struct intrinsic_type<T *> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T>
+struct intrinsic_type<T &> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T>
+struct intrinsic_type<T &&> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T, size_t N>
+struct intrinsic_type<const T[N]> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T, size_t N>
+struct intrinsic_type<T[N]> {
+    using type = typename intrinsic_type<T>::type;
+};
+template <typename T>
+using intrinsic_t = typename intrinsic_type<T>::type;
 
 /// Helper type to replace 'void' in some expressions
-struct void_type { };
+struct void_type {};
 
 /// Helper template which holds a list of types
-template <typename...> struct type_list { };
+template <typename...>
+struct type_list {};
 
 /// Compile-time integer sum
 #ifdef __cpp_fold_expressions
-template <typename... Ts> constexpr size_t constexpr_sum(Ts... ns) { return (0 + ... + size_t{ns}); }
+template <typename... Ts>
+constexpr size_t constexpr_sum(Ts... ns) {
+    return (0 + ... + size_t{ns});
+}
 #else
 constexpr size_t constexpr_sum() { return 0; }
 template <typename T, typename... Ts>
-constexpr size_t constexpr_sum(T n, Ts... ns) { return size_t{n} + constexpr_sum(ns...); }
+constexpr size_t constexpr_sum(T n, Ts... ns) {
+    return size_t{n} + constexpr_sum(ns...);
+}
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(constexpr_impl)
 /// Implementation details for constexpr functions
 constexpr int first(int i) { return i; }
 template <typename T, typename... Ts>
-constexpr int first(int i, T v, Ts... vs) { return v ? i : first(i + 1, vs...); }
+constexpr int first(int i, T v, Ts... vs) {
+    return v ? i : first(i + 1, vs...);
+}
 
 constexpr int last(int /*i*/, int result) { return result; }
 template <typename T, typename... Ts>
-constexpr int last(int i, int result, T v, Ts... vs) { return last(i + 1, v ? i : result, vs...); }
+constexpr int last(int i, int result, T v, Ts... vs) {
+    return last(i + 1, v ? i : result, vs...);
+}
 PYBIND11_NAMESPACE_END(constexpr_impl)
 
-/// Return the index of the first type in Ts which satisfies Predicate<T>.  Returns sizeof...(Ts) if
-/// none match.
-template <template<typename> class Predicate, typename... Ts>
-constexpr int constexpr_first() { return constexpr_impl::first(0, Predicate<Ts>::value...); }
+/// Return the index of the first type in Ts which satisfies Predicate<T>.
+/// Returns sizeof...(Ts) if none match.
+template <template <typename> class Predicate, typename... Ts>
+constexpr int constexpr_first() {
+    return constexpr_impl::first(0, Predicate<Ts>::value...);
+}
 
 /// Return the index of the last type in Ts which satisfies Predicate<T>, or -1 if none match.
-template <template<typename> class Predicate, typename... Ts>
-constexpr int constexpr_last() { return constexpr_impl::last(0, -1, Predicate<Ts>::value...); }
+template <template <typename> class Predicate, typename... Ts>
+constexpr int constexpr_last() {
+    return constexpr_impl::last(0, -1, Predicate<Ts>::value...);
+}
 
 /// Return the Nth element from the parameter pack
 template <size_t N, typename T, typename... Ts>
-struct pack_element { using type = typename pack_element<N - 1, Ts...>::type; };
+struct pack_element {
+    using type = typename pack_element<N - 1, Ts...>::type;
+};
 template <typename T, typename... Ts>
-struct pack_element<0, T, Ts...> { using type = T; };
+struct pack_element<0, T, Ts...> {
+    using type = T;
+};
 
 /// Return the one and only type which matches the predicate, or Default if none match.
 /// If more than one type matches the predicate, fail at compile-time.
-template <template<typename> class Predicate, typename Default, typename... Ts>
+template <template <typename> class Predicate, typename Default, typename... Ts>
 struct exactly_one {
     static constexpr auto found = constexpr_sum(Predicate<Ts>::value...);
     static_assert(found <= 1, "Found more than one type matching the predicate");
 
     static constexpr auto index = found ? constexpr_first<Predicate, Ts...>() : 0;
     using type = conditional_t<found, typename pack_element<index, Ts...>::type, Default>;
 };
-template <template<typename> class P, typename Default>
-struct exactly_one<P, Default> { using type = Default; };
+template <template <typename> class P, typename Default>
+struct exactly_one<P, Default> {
+    using type = Default;
+};
 
-template <template<typename> class Predicate, typename Default, typename... Ts>
+template <template <typename> class Predicate, typename Default, typename... Ts>
 using exactly_one_t = typename exactly_one<Predicate, Default, Ts...>::type;
 
 /// Defer the evaluation of type T until types Us are instantiated
-template <typename T, typename... /*Us*/> struct deferred_type { using type = T; };
-template <typename T, typename... Us> using deferred_t = typename deferred_type<T, Us...>::type;
+template <typename T, typename... /*Us*/>
+struct deferred_type {
+    using type = T;
+};
+template <typename T, typename... Us>
+using deferred_t = typename deferred_type<T, Us...>::type;
 
 /// Like is_base_of, but requires a strict base (i.e. `is_strict_base_of<T, T>::value == false`,
 /// unlike `std::is_base_of`)
-template <typename Base, typename Derived> using is_strict_base_of = bool_constant<
-    std::is_base_of<Base, Derived>::value && !std::is_same<Base, Derived>::value>;
-
-/// Like is_base_of, but also requires that the base type is accessible (i.e. that a Derived pointer
-/// can be converted to a Base pointer)
-/// For unions, `is_base_of<T, T>::value` is False, so we need to check `is_same` as well.
-template <typename Base, typename Derived> using is_accessible_base_of = bool_constant<
-    (std::is_same<Base, Derived>::value || std::is_base_of<Base, Derived>::value) && std::is_convertible<Derived *, Base *>::value>;
+template <typename Base, typename Derived>
+using is_strict_base_of
+    = bool_constant<std::is_base_of<Base, Derived>::value && !std::is_same<Base, Derived>::value>;
+
+/// Like is_base_of, but also requires that the base type is accessible (i.e. that a Derived
+/// pointer can be converted to a Base pointer) For unions, `is_base_of<T, T>::value` is False, so
+/// we need to check `is_same` as well.
+template <typename Base, typename Derived>
+using is_accessible_base_of
+    = bool_constant<(std::is_same<Base, Derived>::value || std::is_base_of<Base, Derived>::value)
+                    && std::is_convertible<Derived *, Base *>::value>;
 
-template <template<typename...> class Base>
+template <template <typename...> class Base>
 struct is_template_base_of_impl {
-    template <typename... Us> static std::true_type check(Base<Us...> *);
+    template <typename... Us>
+    static std::true_type check(Base<Us...> *);
     static std::false_type check(...);
 };
 
 /// Check if a template is the base of a type. For example:
 /// `is_template_base_of<Base, T>` is true if `struct T : Base<U> {}` where U can be anything
-template <template<typename...> class Base, typename T>
+template <template <typename...> class Base, typename T>
 #if !defined(_MSC_VER)
-using is_template_base_of = decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T>*)nullptr));
+using is_template_base_of
+    = decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T> *) nullptr));
 #else // MSVC2015 has trouble with decltype in template aliases
-struct is_template_base_of : decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T>*)nullptr)) { };
+struct is_template_base_of
+    : decltype(is_template_base_of_impl<Base>::check((intrinsic_t<T> *) nullptr)) {
+};
 #endif
 
 /// Check if T is an instantiation of the template `Class`. For example:
 /// `is_instantiation<shared_ptr, T>` is true if `T == shared_ptr<U>` where U can be anything.
-template <template<typename...> class Class, typename T>
-struct is_instantiation : std::false_type { };
-template <template<typename...> class Class, typename... Us>
-struct is_instantiation<Class, Class<Us...>> : std::true_type { };
+template <template <typename...> class Class, typename T>
+struct is_instantiation : std::false_type {};
+template <template <typename...> class Class, typename... Us>
+struct is_instantiation<Class, Class<Us...>> : std::true_type {};
 
 /// Check if T is std::shared_ptr<U> where U can be anything
-template <typename T> using is_shared_ptr = is_instantiation<std::shared_ptr, T>;
+template <typename T>
+using is_shared_ptr = is_instantiation<std::shared_ptr, T>;
 
 /// Check if T looks like an input iterator
-template <typename T, typename = void> struct is_input_iterator : std::false_type {};
+template <typename T, typename = void>
+struct is_input_iterator : std::false_type {};
 template <typename T>
-struct is_input_iterator<T, void_t<decltype(*std::declval<T &>()), decltype(++std::declval<T &>())>>
+struct is_input_iterator<T,
+                         void_t<decltype(*std::declval<T &>()), decltype(++std::declval<T &>())>>
     : std::true_type {};
 
-template <typename T> using is_function_pointer = bool_constant<
-    std::is_pointer<T>::value && std::is_function<typename std::remove_pointer<T>::type>::value>;
+template <typename T>
+using is_function_pointer
+    = bool_constant<std::is_pointer<T>::value
+                    && std::is_function<typename std::remove_pointer<T>::type>::value>;
 
-template <typename F> struct strip_function_object {
+template <typename F>
+struct strip_function_object {
     // If you are encountering an
     // 'error: name followed by "::" must be a class or namespace name'
     // with the Intel compiler and a noexcept function here,
     // try to use noexcept(true) instead of plain noexcept.
     using type = typename remove_class<decltype(&F::operator())>::type;
 };
 
 // Extracts the function signature from a function, function pointer or lambda.
 template <typename Function, typename F = remove_reference_t<Function>>
 using function_signature_t = conditional_t<
     std::is_function<F>::value,
     F,
-    typename conditional_t<
-        std::is_pointer<F>::value || std::is_member_pointer<F>::value,
-        std::remove_pointer<F>,
-        strip_function_object<F>
-    >::type
->;
+    typename conditional_t<std::is_pointer<F>::value || std::is_member_pointer<F>::value,
+                           std::remove_pointer<F>,
+                           strip_function_object<F>>::type>;
 
 /// Returns true if the type looks like a lambda: that is, isn't a function, pointer or member
 /// pointer.  Note that this can catch all sorts of other things, too; this is intended to be used
 /// in a place where passing a lambda makes sense.
-template <typename T> using is_lambda = satisfies_none_of<remove_reference_t<T>,
-        std::is_function, std::is_pointer, std::is_member_pointer>;
+template <typename T>
+using is_lambda = satisfies_none_of<remove_reference_t<T>,
+                                    std::is_function,
+                                    std::is_pointer,
+                                    std::is_member_pointer>;
 
 // [workaround(intel)] Internal error on fold expression
 /// Apply a function over each element of a parameter pack
 #if defined(__cpp_fold_expressions) && !defined(__INTEL_COMPILER)
 // Intel compiler produces an internal error on this fold expression (tested with ICC 19.0.2)
-#define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (((PATTERN), void()), ...)
+#    define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (((PATTERN), void()), ...)
 #else
 using expand_side_effects = bool[];
-#define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (void)pybind11::detail::expand_side_effects{ ((PATTERN), void(), false)..., false }
+#    define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN)                                                 \
+        (void) pybind11::detail::expand_side_effects { ((PATTERN), void(), false)..., false }
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
 #if defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4275) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#    pragma warning(push)
+#    pragma warning(disable : 4275)
+//     warning C4275: An exported class was derived from a class that wasn't exported.
+//     Can be ignored when derived from a STL class.
 #endif
 /// C++ bindings of builtin Python exceptions
 class PYBIND11_EXPORT_EXCEPTION builtin_exception : public std::runtime_error {
 public:
     using std::runtime_error::runtime_error;
     /// Set the error using the Python C API
     virtual void set_error() const = 0;
 };
 #if defined(_MSC_VER)
-#  pragma warning(pop)
+#    pragma warning(pop)
 #endif
 
-#define PYBIND11_RUNTIME_EXCEPTION(name, type) \
-    class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception { public: \
-        using builtin_exception::builtin_exception; \
-        name() : name("") { } \
-        void set_error() const override { PyErr_SetString(type, what()); } \
+#define PYBIND11_RUNTIME_EXCEPTION(name, type)                                                    \
+    class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception {                             \
+    public:                                                                                       \
+        using builtin_exception::builtin_exception;                                               \
+        name() : name("") {}                                                                      \
+        void set_error() const override { PyErr_SetString(type, what()); }                        \
     };
 
 PYBIND11_RUNTIME_EXCEPTION(stop_iteration, PyExc_StopIteration)
 PYBIND11_RUNTIME_EXCEPTION(index_error, PyExc_IndexError)
 PYBIND11_RUNTIME_EXCEPTION(key_error, PyExc_KeyError)
 PYBIND11_RUNTIME_EXCEPTION(value_error, PyExc_ValueError)
 PYBIND11_RUNTIME_EXCEPTION(type_error, PyExc_TypeError)
 PYBIND11_RUNTIME_EXCEPTION(buffer_error, PyExc_BufferError)
 PYBIND11_RUNTIME_EXCEPTION(import_error, PyExc_ImportError)
 PYBIND11_RUNTIME_EXCEPTION(attribute_error, PyExc_AttributeError)
-PYBIND11_RUNTIME_EXCEPTION(cast_error, PyExc_RuntimeError) /// Thrown when pybind11::cast or handle::call fail due to a type casting error
+PYBIND11_RUNTIME_EXCEPTION(cast_error, PyExc_RuntimeError) /// Thrown when pybind11::cast or
+                                                           /// handle::call fail due to a type
+                                                           /// casting error
 PYBIND11_RUNTIME_EXCEPTION(reference_cast_error, PyExc_RuntimeError) /// Used internally
 
-[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const char *reason) { throw std::runtime_error(reason); }
-[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const std::string &reason) { throw std::runtime_error(reason); }
+[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const char *reason) {
+    throw std::runtime_error(reason);
+}
+[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const std::string &reason) {
+    throw std::runtime_error(reason);
+}
 
-template <typename T, typename SFINAE = void> struct format_descriptor { };
+template <typename T, typename SFINAE = void>
+struct format_descriptor {};
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns the index of the given type in the type char array below, and in the list in numpy.h
 // The order here is: bool; 8 ints ((signed,unsigned)x(8,16,32,64)bits); float,double,long double;
 // complex float,double,long double.  Note that the long double types only participate when long
 // double is actually longer than double (it isn't under MSVC).
 // NB: not only the string below but also complex.h and numpy.h rely on this order.
-template <typename T, typename SFINAE = void> struct is_fmt_numeric { static constexpr bool value = false; };
-template <typename T> struct is_fmt_numeric<T, enable_if_t<std::is_arithmetic<T>::value>> {
+template <typename T, typename SFINAE = void>
+struct is_fmt_numeric {
+    static constexpr bool value = false;
+};
+template <typename T>
+struct is_fmt_numeric<T, enable_if_t<std::is_arithmetic<T>::value>> {
     static constexpr bool value = true;
-    static constexpr int index = std::is_same<T, bool>::value ? 0 : 1 + (
-        std::is_integral<T>::value ? detail::log2(sizeof(T))*2 + std::is_unsigned<T>::value : 8 + (
-        std::is_same<T, double>::value ? 1 : std::is_same<T, long double>::value ? 2 : 0));
+    static constexpr int index
+        = std::is_same<T, bool>::value
+              ? 0
+              : 1
+                    + (std::is_integral<T>::value
+                           ? detail::log2(sizeof(T)) * 2 + std::is_unsigned<T>::value
+                           : 8
+                                 + (std::is_same<T, double>::value        ? 1
+                                    : std::is_same<T, long double>::value ? 2
+                                                                          : 0));
 };
 PYBIND11_NAMESPACE_END(detail)
 
-template <typename T> struct format_descriptor<T, detail::enable_if_t<std::is_arithmetic<T>::value>> {
+template <typename T>
+struct format_descriptor<T, detail::enable_if_t<std::is_arithmetic<T>::value>> {
     static constexpr const char c = "?bBhHiIqQfdg"[detail::is_fmt_numeric<T>::index];
-    static constexpr const char value[2] = { c, '\0' };
+    static constexpr const char value[2] = {c, '\0'};
     static std::string format() { return std::string(1, c); }
 };
 
 #if !defined(PYBIND11_CPP17)
 
-template <typename T> constexpr const char format_descriptor<
-    T, detail::enable_if_t<std::is_arithmetic<T>::value>>::value[2];
+template <typename T>
+constexpr const char
+    format_descriptor<T, detail::enable_if_t<std::is_arithmetic<T>::value>>::value[2];
 
 #endif
 
 /// RAII wrapper that temporarily clears any Python error state
 struct error_scope {
     PyObject *type, *value, *trace;
     error_scope() { PyErr_Fetch(&type, &value, &trace); }
     ~error_scope() { PyErr_Restore(type, value, trace); }
 };
 
 /// Dummy destructor wrapper that can be used to expose classes with a private destructor
-struct nodelete { template <typename T> void operator()(T*) { } };
+struct nodelete {
+    template <typename T>
+    void operator()(T *) {}
+};
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 template <typename... Args>
 struct overload_cast_impl {
     // NOLINTNEXTLINE(modernize-use-equals-default):  MSVC 2015 needs this
     constexpr overload_cast_impl() {}
 
     template <typename Return>
-    constexpr auto operator()(Return (*pf)(Args...)) const noexcept
-                              -> decltype(pf) { return pf; }
+    constexpr auto operator()(Return (*pf)(Args...)) const noexcept -> decltype(pf) {
+        return pf;
+    }
 
     template <typename Return, typename Class>
     constexpr auto operator()(Return (Class::*pmf)(Args...), std::false_type = {}) const noexcept
-                              -> decltype(pmf) { return pmf; }
+        -> decltype(pmf) {
+        return pmf;
+    }
 
     template <typename Return, typename Class>
     constexpr auto operator()(Return (Class::*pmf)(Args...) const, std::true_type) const noexcept
-                              -> decltype(pmf) { return pmf; }
+        -> decltype(pmf) {
+        return pmf;
+    }
 };
 PYBIND11_NAMESPACE_END(detail)
 
 // overload_cast requires variable templates: C++14
 #if defined(PYBIND11_CPP14)
-#define PYBIND11_OVERLOAD_CAST 1
+#    define PYBIND11_OVERLOAD_CAST 1
 /// Syntax sugar for resolving overloaded function pointers:
 ///  - regular: static_cast<Return (Class::*)(Arg0, Arg1, Arg2)>(&Class::func)
 ///  - sweet:   overload_cast<Arg0, Arg1, Arg2>(&Class::func)
 template <typename... Args>
 static constexpr detail::overload_cast_impl<Args...> overload_cast = {};
 // MSVC 2015 only accepts this particular initialization syntax for this variable template.
 #endif
 
 /// Const member function selector for overload_cast
 ///  - regular: static_cast<Return (Class::*)(Arg) const>(&Class::func)
 ///  - sweet:   overload_cast<Arg>(&Class::func, const_)
 static constexpr auto const_ = std::true_type{};
 
 #if !defined(PYBIND11_CPP14) // no overload_cast: providing something that static_assert-fails:
-template <typename... Args> struct overload_cast {
+template <typename... Args>
+struct overload_cast {
     static_assert(detail::deferred_t<std::false_type, Args...>::value,
                   "pybind11::overload_cast<...> requires compiling in C++14 mode");
 };
 #endif // overload_cast
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Adaptor for converting arbitrary container arguments into a vector; implicitly convertible from
 // any standard container (or C-style array) supporting std::begin/std::end, any singleton
 // arithmetic type (if T is arithmetic), or explicitly constructible from an iterator pair.
 template <typename T>
 class any_container {
     std::vector<T> v;
+
 public:
     any_container() = default;
 
     // Can construct from a pair of iterators
     template <typename It, typename = enable_if_t<is_input_iterator<It>::value>>
-    any_container(It first, It last) : v(first, last) { }
+    any_container(It first, It last) : v(first, last) {}
 
-    // Implicit conversion constructor from any arbitrary container type with values convertible to T
-    template <typename Container, typename = enable_if_t<std::is_convertible<decltype(*std::begin(std::declval<const Container &>())), T>::value>>
+    // Implicit conversion constructor from any arbitrary container type
+    // with values convertible to T
+    template <typename Container,
+              typename = enable_if_t<
+                  std::is_convertible<decltype(*std::begin(std::declval<const Container &>())),
+                                      T>::value>>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    any_container(const Container &c) : any_container(std::begin(c), std::end(c)) { }
+    any_container(const Container &c) : any_container(std::begin(c), std::end(c)) {}
 
-    // initializer_list's aren't deducible, so don't get matched by the above template; we need this
-    // to explicitly allow implicit conversion from one:
+    // initializer_list's aren't deducible, so don't get matched by the above template;
+    // we need this to explicitly allow implicit conversion from one:
     template <typename TIn, typename = enable_if_t<std::is_convertible<TIn, T>::value>>
-    any_container(const std::initializer_list<TIn> &c) : any_container(c.begin(), c.end()) { }
+    any_container(const std::initializer_list<TIn> &c) : any_container(c.begin(), c.end()) {}
 
     // Avoid copying if given an rvalue vector of the correct type.
     // NOLINTNEXTLINE(google-explicit-constructor)
-    any_container(std::vector<T> &&v) : v(std::move(v)) { }
+    any_container(std::vector<T> &&v) : v(std::move(v)) {}
 
     // Moves the vector out of an rvalue any_container
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::vector<T> &&() && { return std::move(v); }
 
     // Dereferencing obtains a reference to the underlying vector
     std::vector<T> &operator*() { return v; }
@@ -1001,52 +1146,54 @@
 
     // -> lets you call methods on the underlying vector
     std::vector<T> *operator->() { return &v; }
     const std::vector<T> *operator->() const { return &v; }
 };
 
 // Forward-declaration; see detail/class.h
-std::string get_fully_qualified_tp_name(PyTypeObject*);
+std::string get_fully_qualified_tp_name(PyTypeObject *);
 
 template <typename T>
-inline static std::shared_ptr<T> try_get_shared_from_this(std::enable_shared_from_this<T> *holder_value_ptr) {
+inline static std::shared_ptr<T>
+try_get_shared_from_this(std::enable_shared_from_this<T> *holder_value_ptr) {
 // Pre C++17, this code path exploits undefined behavior, but is known to work on many platforms.
 // Use at your own risk!
 // See also https://en.cppreference.com/w/cpp/memory/enable_shared_from_this, and in particular
 // the `std::shared_ptr<Good> gp1 = not_so_good.getptr();` and `try`-`catch` parts of the example.
 #if defined(__cpp_lib_enable_shared_from_this) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
     return holder_value_ptr->weak_from_this().lock();
 #else
     try {
         return holder_value_ptr->shared_from_this();
-    }
-    catch (const std::bad_weak_ptr &) {
+    } catch (const std::bad_weak_ptr &) {
         return nullptr;
     }
 #endif
 }
 
 // For silencing "unused" compiler warnings in special situations.
 template <typename... Args>
 #if defined(_MSC_VER) && _MSC_VER >= 1910 && _MSC_VER < 1920 // MSVC 2017
 constexpr
 #endif
-inline void silence_unused_warnings(Args &&...) {}
+    inline void
+    silence_unused_warnings(Args &&...) {
+}
 
 // MSVC warning C4100: Unreferenced formal parameter
 #if defined(_MSC_VER) && _MSC_VER <= 1916
 #    define PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(...)                                         \
         detail::silence_unused_warnings(__VA_ARGS__)
 #else
 #    define PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(...)
 #endif
 
 // GCC -Wunused-but-set-parameter  All GCC versions (as of July 2021).
 #if defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)                   \
+#    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)                       \
         detail::silence_unused_warnings(__VA_ARGS__)
 #else
 #    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)
 #endif
 
 #if defined(_MSC_VER) // All versions (as of July 2021).
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/init.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/init.h`

 * *Files 10% similar despite different names*

```diff
@@ -18,78 +18,97 @@
 class type_caster<value_and_holder> {
 public:
     bool load(handle h, bool) {
         value = reinterpret_cast<value_and_holder *>(h.ptr());
         return true;
     }
 
-    template <typename> using cast_op_type = value_and_holder &;
+    template <typename>
+    using cast_op_type = value_and_holder &;
     explicit operator value_and_holder &() { return *value; }
     static constexpr auto name = const_name<value_and_holder>();
 
 private:
     value_and_holder *value = nullptr;
 };
 
 PYBIND11_NAMESPACE_BEGIN(initimpl)
 
 inline void no_nullptr(void *ptr) {
-    if (!ptr) throw type_error("pybind11::init(): factory function returned nullptr");
+    if (!ptr) {
+        throw type_error("pybind11::init(): factory function returned nullptr");
+    }
 }
 
 // Implementing functions for all forms of py::init<...> and py::init(...)
-template <typename Class> using Cpp = typename Class::type;
-template <typename Class> using Alias = typename Class::type_alias;
-template <typename Class> using Holder = typename Class::holder_type;
+template <typename Class>
+using Cpp = typename Class::type;
+template <typename Class>
+using Alias = typename Class::type_alias;
+template <typename Class>
+using Holder = typename Class::holder_type;
 
-template <typename Class> using is_alias_constructible = std::is_constructible<Alias<Class>, Cpp<Class> &&>;
+template <typename Class>
+using is_alias_constructible = std::is_constructible<Alias<Class>, Cpp<Class> &&>;
 
 // Takes a Cpp pointer and returns true if it actually is a polymorphic Alias instance.
 template <typename Class, enable_if_t<Class::has_alias, int> = 0>
 bool is_alias(Cpp<Class> *ptr) {
     return dynamic_cast<Alias<Class> *>(ptr) != nullptr;
 }
 // Failing fallback version of the above for a no-alias class (always returns false)
 template <typename /*Class*/>
-constexpr bool is_alias(void *) { return false; }
+constexpr bool is_alias(void *) {
+    return false;
+}
 
 // Constructs and returns a new object; if the given arguments don't map to a constructor, we fall
 // back to brace aggregate initiailization so that for aggregate initialization can be used with
 // py::init, e.g.  `py::init<int, int>` to initialize a `struct T { int a; int b; }`.  For
 // non-aggregate types, we need to use an ordinary T(...) constructor (invoking as `T{...}` usually
 // works, but will not do the expected thing when `T` has an `initializer_list<T>` constructor).
-template <typename Class, typename... Args, detail::enable_if_t<std::is_constructible<Class, Args...>::value, int> = 0>
-inline Class *construct_or_initialize(Args &&...args) { return new Class(std::forward<Args>(args)...); }
-template <typename Class, typename... Args, detail::enable_if_t<!std::is_constructible<Class, Args...>::value, int> = 0>
-inline Class *construct_or_initialize(Args &&...args) { return new Class{std::forward<Args>(args)...}; }
+template <typename Class,
+          typename... Args,
+          detail::enable_if_t<std::is_constructible<Class, Args...>::value, int> = 0>
+inline Class *construct_or_initialize(Args &&...args) {
+    return new Class(std::forward<Args>(args)...);
+}
+template <typename Class,
+          typename... Args,
+          detail::enable_if_t<!std::is_constructible<Class, Args...>::value, int> = 0>
+inline Class *construct_or_initialize(Args &&...args) {
+    return new Class{std::forward<Args>(args)...};
+}
 
 // Attempts to constructs an alias using a `Alias(Cpp &&)` constructor.  This allows types with
 // an alias to provide only a single Cpp factory function as long as the Alias can be
 // constructed from an rvalue reference of the base Cpp type.  This means that Alias classes
 // can, when appropriate, simply define a `Alias(Cpp &&)` constructor rather than needing to
 // inherit all the base class constructors.
 template <typename Class>
 void construct_alias_from_cpp(std::true_type /*is_alias_constructible*/,
-                              value_and_holder &v_h, Cpp<Class> &&base) {
+                              value_and_holder &v_h,
+                              Cpp<Class> &&base) {
     v_h.value_ptr() = new Alias<Class>(std::move(base));
 }
 template <typename Class>
 [[noreturn]] void construct_alias_from_cpp(std::false_type /*!is_alias_constructible*/,
-                                           value_and_holder &, Cpp<Class> &&) {
+                                           value_and_holder &,
+                                           Cpp<Class> &&) {
     throw type_error("pybind11::init(): unable to convert returned instance to required "
                      "alias class: no `Alias<Class>(Class &&)` constructor available");
 }
 
 // Error-generating fallback for factories that don't match one of the below construction
 // mechanisms.
 template <typename Class>
 void construct(...) {
     static_assert(!std::is_same<Class, Class>::value /* always false */,
-            "pybind11::init(): init function must return a compatible pointer, "
-            "holder, or value");
+                  "pybind11::init(): init function must return a compatible pointer, "
+                  "holder, or value");
 }
 
 // Pointer return v1: the factory function returns a class pointer for a registered class.
 // If we don't need an alias (because this class doesn't have one, or because the final type is
 // inherited on the Python side) we can simply take over ownership.  Otherwise we need to try to
 // construct an Alias from the returned base instance.
 template <typename Class>
@@ -102,15 +121,15 @@
         // moved away leftover, if the alias construction works, or the value itself if we
         // throw an error), but we can't just call `delete ptr`: it might have a special
         // deleter, or might be shared_from_this.  So we construct a holder around it as if
         // it was a normal instance, then steal the holder away into a local variable; thus
         // the holder and destruction happens when we leave the C++ scope, and the holder
         // class gets to handle the destruction however it likes.
         v_h.value_ptr() = ptr;
-        v_h.set_instance_registered(true); // To prevent init_instance from registering it
+        v_h.set_instance_registered(true);          // To prevent init_instance from registering it
         v_h.type->init_instance(v_h.inst, nullptr); // Set up the holder
         Holder<Class> temp_holder(std::move(v_h.holder<Holder<Class>>())); // Steal the holder
         v_h.type->dealloc(v_h); // Destroys the moved-out holder remains, resets value ptr to null
         v_h.set_instance_registered(false);
 
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(*ptr));
     } else {
@@ -125,100 +144,132 @@
 void construct(value_and_holder &v_h, Alias<Class> *alias_ptr, bool) {
     no_nullptr(alias_ptr);
     v_h.value_ptr() = static_cast<Cpp<Class> *>(alias_ptr);
 }
 
 // Holder return: copy its pointer, and move or copy the returned holder into the new instance's
 // holder.  This also handles types like std::shared_ptr<T> and std::unique_ptr<T> where T is a
-// derived type (through those holder's implicit conversion from derived class holder constructors).
+// derived type (through those holder's implicit conversion from derived class holder
+// constructors).
 template <typename Class>
 void construct(value_and_holder &v_h, Holder<Class> holder, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     auto *ptr = holder_helper<Holder<Class>>::get(holder);
     no_nullptr(ptr);
     // If we need an alias, check that the held pointer is actually an alias instance
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr))
+    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
         throw type_error("pybind11::init(): construction failed: returned holder-wrapped instance "
                          "is not an alias instance");
+    }
 
     v_h.value_ptr() = ptr;
     v_h.type->init_instance(v_h.inst, &holder);
 }
 
 // return-by-value version 1: returning a cpp class by value.  If the class has an alias and an
 // alias is required the alias must have an `Alias(Cpp &&)` constructor so that we can construct
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     static_assert(std::is_move_constructible<Cpp<Class>>::value,
-        "pybind11::init() return-by-value factory function requires a movable class");
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias)
+                  "pybind11::init() return-by-value factory function requires a movable class");
+    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias) {
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
-    else
+    } else {
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
+    }
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
 // Alias instance (even if no the python-side inheritance is involved).  The is intended for
 // cases where Alias initialization is always desired.
 template <typename Class>
 void construct(value_and_holder &v_h, Alias<Class> &&result, bool) {
-    static_assert(std::is_move_constructible<Alias<Class>>::value,
+    static_assert(
+        std::is_move_constructible<Alias<Class>>::value,
         "pybind11::init() return-by-alias-value factory function requires a movable alias class");
     v_h.value_ptr() = new Alias<Class>(std::move(result));
 }
 
 // Implementing class for py::init<...>()
 template <typename... Args>
 struct constructor {
     template <typename Class, typename... Extra, enable_if_t<!Class::has_alias, int> = 0>
-    static void execute(Class &cl, const Extra&... extra) {
-        cl.def("__init__", [](value_and_holder &v_h, Args... args) {
-            v_h.value_ptr() = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
-        }, is_new_style_constructor(), extra...);
+    static void execute(Class &cl, const Extra &...extra) {
+        cl.def(
+            "__init__",
+            [](value_and_holder &v_h, Args... args) {
+                v_h.value_ptr() = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 
-    template <typename Class, typename... Extra,
-              enable_if_t<Class::has_alias &&
-                          std::is_constructible<Cpp<Class>, Args...>::value, int> = 0>
-    static void execute(Class &cl, const Extra&... extra) {
-        cl.def("__init__", [](value_and_holder &v_h, Args... args) {
-            if (Py_TYPE(v_h.inst) == v_h.type->type)
-                v_h.value_ptr() = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
-            else
-                v_h.value_ptr() = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
-        }, is_new_style_constructor(), extra...);
+    template <typename Class,
+              typename... Extra,
+              enable_if_t<Class::has_alias && std::is_constructible<Cpp<Class>, Args...>::value,
+                          int> = 0>
+    static void execute(Class &cl, const Extra &...extra) {
+        cl.def(
+            "__init__",
+            [](value_and_holder &v_h, Args... args) {
+                if (Py_TYPE(v_h.inst) == v_h.type->type) {
+                    v_h.value_ptr()
+                        = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
+                } else {
+                    v_h.value_ptr()
+                        = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
+                }
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 
-    template <typename Class, typename... Extra,
-              enable_if_t<Class::has_alias &&
-                          !std::is_constructible<Cpp<Class>, Args...>::value, int> = 0>
-    static void execute(Class &cl, const Extra&... extra) {
-        cl.def("__init__", [](value_and_holder &v_h, Args... args) {
-            v_h.value_ptr() = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
-        }, is_new_style_constructor(), extra...);
+    template <typename Class,
+              typename... Extra,
+              enable_if_t<Class::has_alias && !std::is_constructible<Cpp<Class>, Args...>::value,
+                          int> = 0>
+    static void execute(Class &cl, const Extra &...extra) {
+        cl.def(
+            "__init__",
+            [](value_and_holder &v_h, Args... args) {
+                v_h.value_ptr()
+                    = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 };
 
 // Implementing class for py::init_alias<...>()
-template <typename... Args> struct alias_constructor {
-    template <typename Class, typename... Extra,
-              enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value, int> = 0>
-    static void execute(Class &cl, const Extra&... extra) {
-        cl.def("__init__", [](value_and_holder &v_h, Args... args) {
-            v_h.value_ptr() = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
-        }, is_new_style_constructor(), extra...);
+template <typename... Args>
+struct alias_constructor {
+    template <typename Class,
+              typename... Extra,
+              enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value,
+                          int> = 0>
+    static void execute(Class &cl, const Extra &...extra) {
+        cl.def(
+            "__init__",
+            [](value_and_holder &v_h, Args... args) {
+                v_h.value_ptr()
+                    = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 };
 
 // Implementation class for py::init(Func) and py::init(Func, AliasFunc)
-template <typename CFunc, typename AFunc = void_type (*)(),
-          typename = function_signature_t<CFunc>, typename = function_signature_t<AFunc>>
+template <typename CFunc,
+          typename AFunc = void_type (*)(),
+          typename = function_signature_t<CFunc>,
+          typename = function_signature_t<AFunc>>
 struct factory;
 
 // Specialization for py::init(Func)
 template <typename Func, typename Return, typename... Args>
 struct factory<Func, void_type (*)(), Return(Args...)> {
     remove_reference_t<Func> class_factory;
 
@@ -228,119 +279,150 @@
     // The given class either has no alias or has no separate alias factory;
     // this always constructs the class itself.  If the class is registered with an alias
     // type and an alias instance is needed (i.e. because the final type is a Python class
     // inheriting from the C++ type) the returned value needs to either already be an alias
     // instance, or the alias needs to be constructible from a `Class &&` argument.
     template <typename Class, typename... Extra>
     void execute(Class &cl, const Extra &...extra) && {
-        #if defined(PYBIND11_CPP14)
-        cl.def("__init__", [func = std::move(class_factory)]
-        #else
+#if defined(PYBIND11_CPP14)
+        cl.def(
+            "__init__",
+            [func = std::move(class_factory)]
+#else
         auto &func = class_factory;
-        cl.def("__init__", [func]
-        #endif
-        (value_and_holder &v_h, Args... args) {
-            construct<Class>(v_h, func(std::forward<Args>(args)...),
-                             Py_TYPE(v_h.inst) != v_h.type->type);
-        }, is_new_style_constructor(), extra...);
+        cl.def(
+            "__init__",
+            [func]
+#endif
+            (value_and_holder &v_h, Args... args) {
+                construct<Class>(
+                    v_h, func(std::forward<Args>(args)...), Py_TYPE(v_h.inst) != v_h.type->type);
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 };
 
 // Specialization for py::init(Func, AliasFunc)
-template <typename CFunc, typename AFunc,
-          typename CReturn, typename... CArgs, typename AReturn, typename... AArgs>
+template <typename CFunc,
+          typename AFunc,
+          typename CReturn,
+          typename... CArgs,
+          typename AReturn,
+          typename... AArgs>
 struct factory<CFunc, AFunc, CReturn(CArgs...), AReturn(AArgs...)> {
     static_assert(sizeof...(CArgs) == sizeof...(AArgs),
                   "pybind11::init(class_factory, alias_factory): class and alias factories "
                   "must have identical argument signatures");
     static_assert(all_of<std::is_same<CArgs, AArgs>...>::value,
                   "pybind11::init(class_factory, alias_factory): class and alias factories "
                   "must have identical argument signatures");
 
     remove_reference_t<CFunc> class_factory;
     remove_reference_t<AFunc> alias_factory;
 
     factory(CFunc &&c, AFunc &&a)
-        : class_factory(std::forward<CFunc>(c)), alias_factory(std::forward<AFunc>(a)) { }
+        : class_factory(std::forward<CFunc>(c)), alias_factory(std::forward<AFunc>(a)) {}
 
     // The class factory is called when the `self` type passed to `__init__` is the direct
     // class (i.e. not inherited), the alias factory when `self` is a Python-side subtype.
     template <typename Class, typename... Extra>
-    void execute(Class &cl, const Extra&... extra) && {
-        static_assert(Class::has_alias, "The two-argument version of `py::init()` can "
-                                        "only be used if the class has an alias");
-        #if defined(PYBIND11_CPP14)
-        cl.def("__init__", [class_func = std::move(class_factory), alias_func = std::move(alias_factory)]
-        #else
+    void execute(Class &cl, const Extra &...extra) && {
+        static_assert(Class::has_alias,
+                      "The two-argument version of `py::init()` can "
+                      "only be used if the class has an alias");
+#if defined(PYBIND11_CPP14)
+        cl.def(
+            "__init__",
+            [class_func = std::move(class_factory), alias_func = std::move(alias_factory)]
+#else
         auto &class_func = class_factory;
         auto &alias_func = alias_factory;
-        cl.def("__init__", [class_func, alias_func]
-        #endif
-        (value_and_holder &v_h, CArgs... args) {
-            if (Py_TYPE(v_h.inst) == v_h.type->type)
-                // If the instance type equals the registered type we don't have inheritance, so
-                // don't need the alias and can construct using the class function:
-                construct<Class>(v_h, class_func(std::forward<CArgs>(args)...), false);
-            else
-                construct<Class>(v_h, alias_func(std::forward<CArgs>(args)...), true);
-        }, is_new_style_constructor(), extra...);
+        cl.def(
+            "__init__",
+            [class_func, alias_func]
+#endif
+            (value_and_holder &v_h, CArgs... args) {
+                if (Py_TYPE(v_h.inst) == v_h.type->type) {
+                    // If the instance type equals the registered type we don't have inheritance,
+                    // so don't need the alias and can construct using the class function:
+                    construct<Class>(v_h, class_func(std::forward<CArgs>(args)...), false);
+                } else {
+                    construct<Class>(v_h, alias_func(std::forward<CArgs>(args)...), true);
+                }
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 };
 
 /// Set just the C++ state. Same as `__init__`.
 template <typename Class, typename T>
 void setstate(value_and_holder &v_h, T &&result, bool need_alias) {
     construct<Class>(v_h, std::forward<T>(result), need_alias);
 }
 
 /// Set both the C++ and Python states
-template <typename Class, typename T, typename O,
+template <typename Class,
+          typename T,
+          typename O,
           enable_if_t<std::is_convertible<O, handle>::value, int> = 0>
 void setstate(value_and_holder &v_h, std::pair<T, O> &&result, bool need_alias) {
     construct<Class>(v_h, std::move(result.first), need_alias);
     auto d = handle(result.second);
     if (PyDict_Check(d.ptr()) && PyDict_Size(d.ptr()) == 0) {
         // Skipping setattr below, to not force use of py::dynamic_attr() for Class unnecessarily.
         // See PR #2972 for details.
         return;
     }
     setattr((PyObject *) v_h.inst, "__dict__", d);
 }
 
 /// Implementation for py::pickle(GetState, SetState)
-template <typename Get, typename Set,
-          typename = function_signature_t<Get>, typename = function_signature_t<Set>>
+template <typename Get,
+          typename Set,
+          typename = function_signature_t<Get>,
+          typename = function_signature_t<Set>>
 struct pickle_factory;
 
-template <typename Get, typename Set,
-          typename RetState, typename Self, typename NewInstance, typename ArgState>
+template <typename Get,
+          typename Set,
+          typename RetState,
+          typename Self,
+          typename NewInstance,
+          typename ArgState>
 struct pickle_factory<Get, Set, RetState(Self), NewInstance(ArgState)> {
     static_assert(std::is_same<intrinsic_t<RetState>, intrinsic_t<ArgState>>::value,
                   "The type returned by `__getstate__` must be the same "
                   "as the argument accepted by `__setstate__`");
 
     remove_reference_t<Get> get;
     remove_reference_t<Set> set;
 
-    pickle_factory(Get get, Set set)
-        : get(std::forward<Get>(get)), set(std::forward<Set>(set)) { }
+    pickle_factory(Get get, Set set) : get(std::forward<Get>(get)), set(std::forward<Set>(set)) {}
 
     template <typename Class, typename... Extra>
     void execute(Class &cl, const Extra &...extra) && {
         cl.def("__getstate__", std::move(get));
 
 #if defined(PYBIND11_CPP14)
-        cl.def("__setstate__", [func = std::move(set)]
+        cl.def(
+            "__setstate__",
+            [func = std::move(set)]
 #else
         auto &func = set;
-        cl.def("__setstate__", [func]
+        cl.def(
+            "__setstate__",
+            [func]
 #endif
-        (value_and_holder &v_h, ArgState state) {
-            setstate<Class>(v_h, func(std::forward<ArgState>(state)),
-                            Py_TYPE(v_h.inst) != v_h.type->type);
-        }, is_new_style_constructor(), extra...);
+            (value_and_holder &v_h, ArgState state) {
+                setstate<Class>(
+                    v_h, func(std::forward<ArgState>(state)), Py_TYPE(v_h.inst) != v_h.type->type);
+            },
+            is_new_style_constructor(),
+            extra...);
     }
 };
 
 PYBIND11_NAMESPACE_END(initimpl)
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(pybind11)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/internals.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/internals.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../pytypes.h"
+
 #include <exception>
 
 /// Tracks the `internals` and `type_info` ABI version independent of the main library version.
 ///
 /// Some portions of the code use an ABI that is conditional depending on this
 /// version number.  That allows ABI-breaking changes to be "pre-implemented".
 /// Once the default version number is incremented, the conditional logic that
@@ -114,16 +115,17 @@
     return lhs.name() == rhs.name() || std::strcmp(lhs.name(), rhs.name()) == 0;
 }
 
 struct type_hash {
     size_t operator()(const std::type_index &t) const {
         size_t hash = 5381;
         const char *ptr = t.name();
-        while (auto c = static_cast<unsigned char>(*ptr++))
+        while (auto c = static_cast<unsigned char>(*ptr++)) {
             hash = (hash * 33) ^ c;
+        }
         return hash;
     }
 };
 
 struct type_equal_to {
     bool operator()(const std::type_index &lhs, const std::type_index &rhs) const {
         return lhs.name() == rhs.name() || std::strcmp(lhs.name(), rhs.name()) == 0;
@@ -131,37 +133,42 @@
 };
 #endif
 
 template <typename value_type>
 using type_map = std::unordered_map<std::type_index, value_type, type_hash, type_equal_to>;
 
 struct override_hash {
-    inline size_t operator()(const std::pair<const PyObject *, const char *>& v) const {
+    inline size_t operator()(const std::pair<const PyObject *, const char *> &v) const {
         size_t value = std::hash<const void *>()(v.first);
-        value ^= std::hash<const void *>()(v.second) + 0x9e3779b9 + (value<<6) + (value>>2);
+        value ^= std::hash<const void *>()(v.second) + 0x9e3779b9 + (value << 6) + (value >> 2);
         return value;
     }
 };
 
 /// Internal data structure used to track registered instances and types.
 /// Whenever binary incompatible changes are made to this structure,
 /// `PYBIND11_INTERNALS_VERSION` must be incremented.
 struct internals {
-    type_map<type_info *> registered_types_cpp; // std::type_index -> pybind11's type information
-    std::unordered_map<PyTypeObject *, std::vector<type_info *>> registered_types_py; // PyTypeObject* -> base type_info(s)
-    std::unordered_multimap<const void *, instance*> registered_instances; // void * -> instance*
-    std::unordered_set<std::pair<const PyObject *, const char *>, override_hash> inactive_override_cache;
+    // std::type_index -> pybind11's type information
+    type_map<type_info *> registered_types_cpp;
+    // PyTypeObject* -> base type_info(s)
+    std::unordered_map<PyTypeObject *, std::vector<type_info *>> registered_types_py;
+    std::unordered_multimap<const void *, instance *> registered_instances; // void * -> instance*
+    std::unordered_set<std::pair<const PyObject *, const char *>, override_hash>
+        inactive_override_cache;
     type_map<std::vector<bool (*)(PyObject *, void *&)>> direct_conversions;
     std::unordered_map<const PyObject *, std::vector<PyObject *>> patients;
     std::forward_list<ExceptionTranslator> registered_exception_translators;
-    std::unordered_map<std::string, void *> shared_data; // Custom data to be shared across extensions
+    std::unordered_map<std::string, void *> shared_data; // Custom data to be shared across
+                                                         // extensions
 #if PYBIND11_INTERNALS_VERSION == 4
     std::vector<PyObject *> unused_loader_patient_stack_remove_at_v5;
 #endif
-    std::forward_list<std::string> static_strings; // Stores the std::strings backing detail::c_str()
+    std::forward_list<std::string> static_strings; // Stores the std::strings backing
+                                                   // detail::c_str()
     PyTypeObject *static_property_type;
     PyTypeObject *default_metaclass;
     PyObject *instance_base;
 #if defined(WITH_THREAD)
     PYBIND11_TLS_KEY_INIT(tstate)
 #    if PYBIND11_INTERNALS_VERSION > 4
     PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
@@ -189,16 +196,16 @@
 struct type_info {
     PyTypeObject *type;
     const std::type_info *cpptype;
     size_t type_size, type_align, holder_size_in_ptrs;
     void *(*operator_new)(size_t);
     void (*init_instance)(instance *, const void *);
     void (*dealloc)(value_and_holder &v_h);
-    std::vector<PyObject *(*)(PyObject *, PyTypeObject *)> implicit_conversions;
-    std::vector<std::pair<const std::type_info *, void *(*)(void *)>> implicit_casts;
+    std::vector<PyObject *(*) (PyObject *, PyTypeObject *)> implicit_conversions;
+    std::vector<std::pair<const std::type_info *, void *(*) (void *)>> implicit_casts;
     std::vector<bool (*)(PyObject *, void *&)> *direct_conversions;
     buffer_info *(*get_buffer)(PyObject *, void *) = nullptr;
     void *get_buffer_data = nullptr;
     void *(*module_local_load)(PyObject *, const type_info *) = nullptr;
     /* A simple type never occurs as a (direct or indirect) parent
      * of a class that makes use of multiple inheritance.
      * A type can be simple even if it has non-simple ancestors as long as it has no descendants.
@@ -210,75 +217,79 @@
     bool default_holder : 1;
     /* true if this is a type registered with py::module_local */
     bool module_local : 1;
 };
 
 /// On MSVC, debug and release builds are not ABI-compatible!
 #if defined(_MSC_VER) && defined(_DEBUG)
-#  define PYBIND11_BUILD_TYPE "_debug"
+#    define PYBIND11_BUILD_TYPE "_debug"
 #else
-#  define PYBIND11_BUILD_TYPE ""
+#    define PYBIND11_BUILD_TYPE ""
 #endif
 
 /// Let's assume that different compilers are ABI-incompatible.
 /// A user can manually set this string if they know their
 /// compiler is compatible.
 #ifndef PYBIND11_COMPILER_TYPE
-#  if defined(_MSC_VER)
-#    define PYBIND11_COMPILER_TYPE "_msvc"
-#  elif defined(__INTEL_COMPILER)
-#    define PYBIND11_COMPILER_TYPE "_icc"
-#  elif defined(__clang__)
-#    define PYBIND11_COMPILER_TYPE "_clang"
-#  elif defined(__PGI)
-#    define PYBIND11_COMPILER_TYPE "_pgi"
-#  elif defined(__MINGW32__)
-#    define PYBIND11_COMPILER_TYPE "_mingw"
-#  elif defined(__CYGWIN__)
-#    define PYBIND11_COMPILER_TYPE "_gcc_cygwin"
-#  elif defined(__GNUC__)
-#    define PYBIND11_COMPILER_TYPE "_gcc"
-#  else
-#    define PYBIND11_COMPILER_TYPE "_unknown"
-#  endif
+#    if defined(_MSC_VER)
+#        define PYBIND11_COMPILER_TYPE "_msvc"
+#    elif defined(__INTEL_COMPILER)
+#        define PYBIND11_COMPILER_TYPE "_icc"
+#    elif defined(__clang__)
+#        define PYBIND11_COMPILER_TYPE "_clang"
+#    elif defined(__PGI)
+#        define PYBIND11_COMPILER_TYPE "_pgi"
+#    elif defined(__MINGW32__)
+#        define PYBIND11_COMPILER_TYPE "_mingw"
+#    elif defined(__CYGWIN__)
+#        define PYBIND11_COMPILER_TYPE "_gcc_cygwin"
+#    elif defined(__GNUC__)
+#        define PYBIND11_COMPILER_TYPE "_gcc"
+#    else
+#        define PYBIND11_COMPILER_TYPE "_unknown"
+#    endif
 #endif
 
 /// Also standard libs
 #ifndef PYBIND11_STDLIB
-#  if defined(_LIBCPP_VERSION)
-#    define PYBIND11_STDLIB "_libcpp"
-#  elif defined(__GLIBCXX__) || defined(__GLIBCPP__)
-#    define PYBIND11_STDLIB "_libstdcpp"
-#  else
-#    define PYBIND11_STDLIB ""
-#  endif
+#    if defined(_LIBCPP_VERSION)
+#        define PYBIND11_STDLIB "_libcpp"
+#    elif defined(__GLIBCXX__) || defined(__GLIBCPP__)
+#        define PYBIND11_STDLIB "_libstdcpp"
+#    else
+#        define PYBIND11_STDLIB ""
+#    endif
 #endif
 
 /// On Linux/OSX, changes in __GXX_ABI_VERSION__ indicate ABI incompatibility.
 #ifndef PYBIND11_BUILD_ABI
-#  if defined(__GXX_ABI_VERSION)
-#    define PYBIND11_BUILD_ABI "_cxxabi" PYBIND11_TOSTRING(__GXX_ABI_VERSION)
-#  else
-#    define PYBIND11_BUILD_ABI ""
-#  endif
+#    if defined(__GXX_ABI_VERSION)
+#        define PYBIND11_BUILD_ABI "_cxxabi" PYBIND11_TOSTRING(__GXX_ABI_VERSION)
+#    else
+#        define PYBIND11_BUILD_ABI ""
+#    endif
 #endif
 
 #ifndef PYBIND11_INTERNALS_KIND
-#  if defined(WITH_THREAD)
-#    define PYBIND11_INTERNALS_KIND ""
-#  else
-#    define PYBIND11_INTERNALS_KIND "_without_thread"
-#  endif
+#    if defined(WITH_THREAD)
+#        define PYBIND11_INTERNALS_KIND ""
+#    else
+#        define PYBIND11_INTERNALS_KIND "_without_thread"
+#    endif
 #endif
 
-#define PYBIND11_INTERNALS_ID "__pybind11_internals_v" \
-    PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION) PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI PYBIND11_BUILD_TYPE "__"
-
-#define PYBIND11_MODULE_LOCAL_ID "__pybind11_module_local_v" \
-    PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION) PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI PYBIND11_BUILD_TYPE "__"
+#define PYBIND11_INTERNALS_ID                                                                     \
+    "__pybind11_internals_v" PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION)                        \
+        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI         \
+            PYBIND11_BUILD_TYPE "__"
+
+#define PYBIND11_MODULE_LOCAL_ID                                                                  \
+    "__pybind11_module_local_v" PYBIND11_TOSTRING(PYBIND11_INTERNALS_VERSION)                     \
+        PYBIND11_INTERNALS_KIND PYBIND11_COMPILER_TYPE PYBIND11_STDLIB PYBIND11_BUILD_ABI         \
+            PYBIND11_BUILD_TYPE "__"
 
 /// Each module locally stores a pointer to the `internals` data. The data
 /// itself is shared among modules with the same `PYBIND11_INTERNALS_ID`.
 inline internals **&get_internals_pp() {
     static internals **internals_pp = nullptr;
     return internals_pp;
 }
@@ -297,15 +308,15 @@
     }
     return false;
 }
 
 template <class T,
           enable_if_t<!std::is_same<std::nested_exception, remove_cvref_t<T>>::value, int> = 0>
 bool handle_nested_exception(const T &exc, const std::exception_ptr &p) {
-    if (auto *nep = dynamic_cast<const std::nested_exception *>(std::addressof(exc))) {
+    if (const auto *nep = dynamic_cast<const std::nested_exception *>(std::addressof(exc))) {
         return handle_nested_exception(*nep, p);
     }
     return false;
 }
 
 #else
 
@@ -334,15 +345,15 @@
         std::rethrow_exception(p);
     } catch (error_already_set &e) {
         handle_nested_exception(e, p);
         e.restore();
         return;
     } catch (const builtin_exception &e) {
         // Could not use template since it's an abstract class.
-        if (auto *nep = dynamic_cast<const std::nested_exception *>(std::addressof(e))) {
+        if (const auto *nep = dynamic_cast<const std::nested_exception *>(std::addressof(e))) {
             handle_nested_exception(*nep, p);
         }
         e.set_error();
         return;
     } catch (const std::bad_alloc &e) {
         handle_nested_exception(e, p);
         raise_err(PyExc_MemoryError, e.what());
@@ -384,31 +395,38 @@
         return;
     }
 }
 
 #if !defined(__GLIBCXX__)
 inline void translate_local_exception(std::exception_ptr p) {
     try {
-        if (p) std::rethrow_exception(p);
-    } catch (error_already_set &e)       { e.restore();   return;
-    } catch (const builtin_exception &e) { e.set_error(); return;
+        if (p) {
+            std::rethrow_exception(p);
+        }
+    } catch (error_already_set &e) {
+        e.restore();
+        return;
+    } catch (const builtin_exception &e) {
+        e.set_error();
+        return;
     }
 }
 #endif
 
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
-    if (internals_pp && *internals_pp)
+    if (internals_pp && *internals_pp) {
         return **internals_pp;
+    }
 
     // Ensure that the GIL is held since we will need to make Python calls.
     // Cannot use py::gil_scoped_acquire here since that constructor calls get_internals.
     struct gil_scoped_acquire_local {
-        gil_scoped_acquire_local() : state (PyGILState_Ensure()) {}
+        gil_scoped_acquire_local() : state(PyGILState_Ensure()) {}
         ~gil_scoped_acquire_local() { PyGILState_Release(state); }
         const PyGILState_STATE state;
     } gil;
 
     PYBIND11_STR_TYPE id(PYBIND11_INTERNALS_ID);
     auto builtins = handle(PyEval_GetBuiltins());
     if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
@@ -421,15 +439,17 @@
         // libstdc++ doesn't require this (types there are identified only by name)
         // libc++ with CPython doesn't require this (types are explicitly exported)
         // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
         (*internals_pp)->registered_exception_translators.push_front(&translate_local_exception);
 #endif
     } else {
-        if (!internals_pp) internals_pp = new internals*();
+        if (!internals_pp) {
+            internals_pp = new internals *();
+        }
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
 #if defined(WITH_THREAD)
 
 #    if PY_VERSION_HEX < 0x03090000
         PyEval_InitThreads();
 #    endif
@@ -498,19 +518,18 @@
             = static_cast<shared_loader_life_support_data *>(ptr)->loader_life_support_tls_key;
     }
 #endif //  defined(WITH_THREAD) && PYBIND11_INTERNALS_VERSION == 4
 };
 
 /// Works like `get_internals`, but for things which are locally registered.
 inline local_internals &get_local_internals() {
-  static local_internals locals;
-  return locals;
+    static local_internals locals;
+    return locals;
 }
 
-
 /// Constructs a std::string with the given arguments, stores it in `internals`, and returns its
 /// `c_str()`.  Such strings objects have a long storage duration -- the internal strings are only
 /// cleared when the program exits or after interpreter shutdown (when embedding), and so are
 /// suitable for c-style strings needed by Python internals (such as PyTypeObject's tp_name).
 template <typename... Args>
 const char *c_str(Args &&...args) {
     auto &strings = get_internals().static_strings;
@@ -534,15 +553,15 @@
     detail::get_internals().shared_data[name] = data;
     return data;
 }
 
 /// Returns a typed reference to a shared data entry (by using `get_shared_data()`) if
 /// such entry exists. Otherwise, a new object of default-constructible type `T` is
 /// added to the shared data under the given name and a reference to it is returned.
-template<typename T>
+template <typename T>
 T &get_or_create_shared_data(const std::string &name) {
     auto &internals = detail::get_internals();
     auto it = internals.shared_data.find(name);
     T *ptr = (T *) (it != internals.shared_data.end() ? it->second : nullptr);
     if (!ptr) {
         ptr = new T();
         internals.shared_data[name] = ptr;
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/type_caster_base.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #pragma once
 
 #include "../pytypes.h"
 #include "common.h"
 #include "descr.h"
 #include "internals.h"
 #include "typeid.h"
+
 #include <cstdint>
 #include <iterator>
 #include <new>
 #include <string>
 #include <type_traits>
 #include <typeindex>
 #include <typeinfo>
@@ -28,15 +29,15 @@
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// A life support system for temporary objects created by `type_caster::load()`.
 /// Adding a patient will keep it alive up until the enclosing function returns.
 class loader_life_support {
 private:
-    loader_life_support* parent = nullptr;
+    loader_life_support *parent = nullptr;
     std::unordered_set<PyObject *> keep_alive;
 
 #if defined(WITH_THREAD)
     // Store stack pointer in thread-local storage.
     static PYBIND11_TLS_KEY_REF get_stack_tls_key() {
 #    if PYBIND11_INTERNALS_VERSION == 4
         return get_local_internals().loader_life_support_tls_key;
@@ -58,26 +59,25 @@
     }
     static loader_life_support *get_stack_top() { return *get_stack_pp(); }
     static void set_stack_top(loader_life_support *value) { *get_stack_pp() = value; }
 #endif
 
 public:
     /// A new patient frame is created when a function is entered
-    loader_life_support() {
-        parent = get_stack_top();
-        set_stack_top(this);
-    }
+    loader_life_support() : parent{get_stack_top()} { set_stack_top(this); }
 
     /// ... and destroyed after it returns
     ~loader_life_support() {
-        if (get_stack_top() != this)
+        if (get_stack_top() != this) {
             pybind11_fail("loader_life_support: internal error");
+        }
         set_stack_top(parent);
-        for (auto* item : keep_alive)
+        for (auto *item : keep_alive) {
             Py_DECREF(item);
+        }
     }
 
     /// This can only be used inside a pybind11-bound function, either by `argument_loader`
     /// at argument preparation time or by `py::cast()` at execution time.
     PYBIND11_NOINLINE static void add_patient(handle h) {
         loader_life_support *frame = get_stack_top();
         if (!frame) {
@@ -86,66 +86,76 @@
             // a location is challenging. Developers could consider printing out
             // stack frame addresses here using something like __builtin_frame_address(0)
             throw cast_error("When called outside a bound function, py::cast() cannot "
                              "do Python -> C++ conversions which require the creation "
                              "of temporary values");
         }
 
-        if (frame->keep_alive.insert(h.ptr()).second)
+        if (frame->keep_alive.insert(h.ptr()).second) {
             Py_INCREF(h.ptr());
+        }
     }
 };
 
 // Gets the cache entry for the given type, creating it if necessary.  The return value is the pair
 // returned by emplace, i.e. an iterator for the entry and a bool set to `true` if the entry was
 // just created.
-inline std::pair<decltype(internals::registered_types_py)::iterator, bool> all_type_info_get_cache(PyTypeObject *type);
+inline std::pair<decltype(internals::registered_types_py)::iterator, bool>
+all_type_info_get_cache(PyTypeObject *type);
 
 // Populates a just-created cache entry.
 PYBIND11_NOINLINE void all_type_info_populate(PyTypeObject *t, std::vector<type_info *> &bases) {
     std::vector<PyTypeObject *> check;
-    for (handle parent : reinterpret_borrow<tuple>(t->tp_bases))
+    for (handle parent : reinterpret_borrow<tuple>(t->tp_bases)) {
         check.push_back((PyTypeObject *) parent.ptr());
+    }
 
     auto const &type_dict = get_internals().registered_types_py;
     for (size_t i = 0; i < check.size(); i++) {
-        auto type = check[i];
+        auto *type = check[i];
         // Ignore Python2 old-style class super type:
-        if (!PyType_Check((PyObject *) type)) continue;
+        if (!PyType_Check((PyObject *) type)) {
+            continue;
+        }
 
         // Check `type` in the current set of registered python types:
         auto it = type_dict.find(type);
         if (it != type_dict.end()) {
             // We found a cache entry for it, so it's either pybind-registered or has pre-computed
-            // pybind bases, but we have to make sure we haven't already seen the type(s) before: we
-            // want to follow Python/virtual C++ rules that there should only be one instance of a
-            // common base.
+            // pybind bases, but we have to make sure we haven't already seen the type(s) before:
+            // we want to follow Python/virtual C++ rules that there should only be one instance of
+            // a common base.
             for (auto *tinfo : it->second) {
                 // NB: Could use a second set here, rather than doing a linear search, but since
                 // having a large number of immediate pybind11-registered types seems fairly
                 // unlikely, that probably isn't worthwhile.
                 bool found = false;
                 for (auto *known : bases) {
-                    if (known == tinfo) { found = true; break; }
+                    if (known == tinfo) {
+                        found = true;
+                        break;
+                    }
+                }
+                if (!found) {
+                    bases.push_back(tinfo);
                 }
-                if (!found) bases.push_back(tinfo);
             }
-        }
-        else if (type->tp_bases) {
+        } else if (type->tp_bases) {
             // It's some python type, so keep follow its bases classes to look for one or more
             // registered types
             if (i + 1 == check.size()) {
                 // When we're at the end, we can pop off the current element to avoid growing
                 // `check` when adding just one base (which is typical--i.e. when there is no
                 // multiple inheritance)
                 check.pop_back();
                 i--;
             }
-            for (handle parent : reinterpret_borrow<tuple>(type->tp_bases))
+            for (handle parent : reinterpret_borrow<tuple>(type->tp_bases)) {
                 check.push_back((PyTypeObject *) parent.ptr());
+            }
         }
     }
 }
 
 /**
  * Extracts vector of type_info pointers of pybind-registered roots of the given Python type.  Will
  * be just 1 pybind type for the Python type of a pybind-registered class, or for any Python-side
@@ -154,139 +164,154 @@
  * pybind-registered classes.  Will be empty if neither the type nor any base classes are
  * pybind-registered.
  *
  * The value is cached for the lifetime of the Python type.
  */
 inline const std::vector<detail::type_info *> &all_type_info(PyTypeObject *type) {
     auto ins = all_type_info_get_cache(type);
-    if (ins.second)
+    if (ins.second) {
         // New cache entry: populate it
         all_type_info_populate(type, ins.first->second);
+    }
 
     return ins.first->second;
 }
 
 /**
  * Gets a single pybind11 type info for a python type.  Returns nullptr if neither the type nor any
  * ancestors are pybind11-registered.  Throws an exception if there are multiple bases--use
  * `all_type_info` instead if you want to support multiple bases.
  */
-PYBIND11_NOINLINE detail::type_info* get_type_info(PyTypeObject *type) {
-    auto &bases = all_type_info(type);
-    if (bases.empty())
+PYBIND11_NOINLINE detail::type_info *get_type_info(PyTypeObject *type) {
+    const auto &bases = all_type_info(type);
+    if (bases.empty()) {
         return nullptr;
-    if (bases.size() > 1)
-        pybind11_fail("pybind11::detail::get_type_info: type has multiple pybind11-registered bases");
+    }
+    if (bases.size() > 1) {
+        pybind11_fail(
+            "pybind11::detail::get_type_info: type has multiple pybind11-registered bases");
+    }
     return bases.front();
 }
 
 inline detail::type_info *get_local_type_info(const std::type_index &tp) {
     auto &locals = get_local_internals().registered_types_cpp;
     auto it = locals.find(tp);
-    if (it != locals.end())
+    if (it != locals.end()) {
         return it->second;
+    }
     return nullptr;
 }
 
 inline detail::type_info *get_global_type_info(const std::type_index &tp) {
     auto &types = get_internals().registered_types_cpp;
     auto it = types.find(tp);
-    if (it != types.end())
+    if (it != types.end()) {
         return it->second;
+    }
     return nullptr;
 }
 
-/// Return the type info for a given C++ type; on lookup failure can either throw or return nullptr.
+/// Return the type info for a given C++ type; on lookup failure can either throw or return
+/// nullptr.
 PYBIND11_NOINLINE detail::type_info *get_type_info(const std::type_index &tp,
-                                                          bool throw_if_missing = false) {
-    if (auto ltype = get_local_type_info(tp))
+                                                   bool throw_if_missing = false) {
+    if (auto *ltype = get_local_type_info(tp)) {
         return ltype;
-    if (auto gtype = get_global_type_info(tp))
+    }
+    if (auto *gtype = get_global_type_info(tp)) {
         return gtype;
+    }
 
     if (throw_if_missing) {
         std::string tname = tp.name();
         detail::clean_type_id(tname);
-        pybind11_fail("pybind11::detail::get_type_info: unable to find type info for \"" + tname + "\"");
+        pybind11_fail("pybind11::detail::get_type_info: unable to find type info for \"" + tname
+                      + "\"");
     }
     return nullptr;
 }
 
 PYBIND11_NOINLINE handle get_type_handle(const std::type_info &tp, bool throw_if_missing) {
     detail::type_info *type_info = get_type_info(tp, throw_if_missing);
     return handle(type_info ? ((PyObject *) type_info->type) : nullptr);
 }
 
 // Searches the inheritance graph for a registered Python instance, using all_type_info().
 PYBIND11_NOINLINE handle find_registered_python_instance(void *src,
-                                                                const detail::type_info *tinfo) {
+                                                         const detail::type_info *tinfo) {
     auto it_instances = get_internals().registered_instances.equal_range(src);
     for (auto it_i = it_instances.first; it_i != it_instances.second; ++it_i) {
-        for (auto instance_type : detail::all_type_info(Py_TYPE(it_i->second))) {
-            if (instance_type && same_type(*instance_type->cpptype, *tinfo->cpptype))
+        for (auto *instance_type : detail::all_type_info(Py_TYPE(it_i->second))) {
+            if (instance_type && same_type(*instance_type->cpptype, *tinfo->cpptype)) {
                 return handle((PyObject *) it_i->second).inc_ref();
+            }
         }
     }
     return handle();
 }
 
 struct value_and_holder {
     instance *inst = nullptr;
     size_t index = 0u;
     const detail::type_info *type = nullptr;
     void **vh = nullptr;
 
     // Main constructor for a found value/holder:
-    value_and_holder(instance *i, const detail::type_info *type, size_t vpos, size_t index) :
-        inst{i}, index{index}, type{type},
-        vh{inst->simple_layout ? inst->simple_value_holder : &inst->nonsimple.values_and_holders[vpos]}
-    {}
+    value_and_holder(instance *i, const detail::type_info *type, size_t vpos, size_t index)
+        : inst{i}, index{index}, type{type}, vh{inst->simple_layout
+                                                    ? inst->simple_value_holder
+                                                    : &inst->nonsimple.values_and_holders[vpos]} {}
 
     // Default constructor (used to signal a value-and-holder not found by get_value_and_holder())
     value_and_holder() = default;
 
     // Used for past-the-end iterator
     explicit value_and_holder(size_t index) : index{index} {}
 
-    template <typename V = void> V *&value_ptr() const {
+    template <typename V = void>
+    V *&value_ptr() const {
         return reinterpret_cast<V *&>(vh[0]);
     }
     // True if this `value_and_holder` has a non-null value pointer
     explicit operator bool() const { return value_ptr() != nullptr; }
 
-    template <typename H> H &holder() const {
+    template <typename H>
+    H &holder() const {
         return reinterpret_cast<H &>(vh[1]);
     }
     bool holder_constructed() const {
         return inst->simple_layout
                    ? inst->simple_holder_constructed
                    : (inst->nonsimple.status[index] & instance::status_holder_constructed) != 0u;
     }
     // NOLINTNEXTLINE(readability-make-member-function-const)
     void set_holder_constructed(bool v = true) {
-        if (inst->simple_layout)
+        if (inst->simple_layout) {
             inst->simple_holder_constructed = v;
-        else if (v)
+        } else if (v) {
             inst->nonsimple.status[index] |= instance::status_holder_constructed;
-        else
+        } else {
             inst->nonsimple.status[index] &= (std::uint8_t) ~instance::status_holder_constructed;
+        }
     }
     bool instance_registered() const {
         return inst->simple_layout
-            ? inst->simple_instance_registered
-            : ((inst->nonsimple.status[index] & instance::status_instance_registered) != 0);
+                   ? inst->simple_instance_registered
+                   : ((inst->nonsimple.status[index] & instance::status_instance_registered) != 0);
     }
     // NOLINTNEXTLINE(readability-make-member-function-const)
     void set_instance_registered(bool v = true) {
-        if (inst->simple_layout)
+        if (inst->simple_layout) {
             inst->simple_instance_registered = v;
-        else if (v)
+        } else if (v) {
             inst->nonsimple.status[index] |= instance::status_instance_registered;
-        else
+        } else {
             inst->nonsimple.status[index] &= (std::uint8_t) ~instance::status_instance_registered;
+        }
     }
 };
 
 // Container for accessing and iterating over an instance's values/holders
 struct values_and_holders {
 private:
     instance *inst;
@@ -301,42 +326,44 @@
     private:
         instance *inst = nullptr;
         const type_vec *types = nullptr;
         value_and_holder curr;
         friend struct values_and_holders;
         iterator(instance *inst, const type_vec *tinfo)
             : inst{inst}, types{tinfo},
-            curr(inst /* instance */,
-                 types->empty() ? nullptr : (*types)[0] /* type info */,
-                 0, /* vpos: (non-simple types only): the first vptr comes first */
-                 0 /* index */)
-        {}
+              curr(inst /* instance */,
+                   types->empty() ? nullptr : (*types)[0] /* type info */,
+                   0, /* vpos: (non-simple types only): the first vptr comes first */
+                   0 /* index */) {}
         // Past-the-end iterator:
         explicit iterator(size_t end) : curr(end) {}
 
     public:
         bool operator==(const iterator &other) const { return curr.index == other.curr.index; }
         bool operator!=(const iterator &other) const { return curr.index != other.curr.index; }
         iterator &operator++() {
-            if (!inst->simple_layout)
+            if (!inst->simple_layout) {
                 curr.vh += 1 + (*types)[curr.index]->holder_size_in_ptrs;
+            }
             ++curr.index;
             curr.type = curr.index < types->size() ? (*types)[curr.index] : nullptr;
             return *this;
         }
         value_and_holder &operator*() { return curr; }
         value_and_holder *operator->() { return &curr; }
     };
 
     iterator begin() { return iterator(inst, &tinfo); }
     iterator end() { return iterator(tinfo.size()); }
 
     iterator find(const type_info *find_type) {
         auto it = begin(), endit = end();
-        while (it != endit && it->type != find_type) ++it;
+        while (it != endit && it->type != find_type) {
+            ++it;
+        }
         return it;
     }
 
     size_t size() { return tinfo.size(); }
 };
 
 /**
@@ -345,96 +372,110 @@
  * if the given type (or ValueType, if omitted) is not a pybind11 base of the given instance.  If
  * `find_type` is omitted (or explicitly specified as nullptr) the first value/holder are returned,
  * regardless of type (and the resulting .type will be nullptr).
  *
  * The returned object should be short-lived: in particular, it must not outlive the called-upon
  * instance.
  */
-PYBIND11_NOINLINE value_and_holder instance::get_value_and_holder(const type_info *find_type /*= nullptr default in common.h*/, bool throw_if_missing /*= true in common.h*/) {
+PYBIND11_NOINLINE value_and_holder
+instance::get_value_and_holder(const type_info *find_type /*= nullptr default in common.h*/,
+                               bool throw_if_missing /*= true in common.h*/) {
     // Optimize common case:
-    if (!find_type || Py_TYPE(this) == find_type->type)
+    if (!find_type || Py_TYPE(this) == find_type->type) {
         return value_and_holder(this, find_type, 0, 0);
+    }
 
     detail::values_and_holders vhs(this);
     auto it = vhs.find(find_type);
-    if (it != vhs.end())
+    if (it != vhs.end()) {
         return *it;
+    }
 
-    if (!throw_if_missing)
+    if (!throw_if_missing) {
         return value_and_holder();
+    }
 
 #if defined(NDEBUG)
     pybind11_fail("pybind11::detail::instance::get_value_and_holder: "
-            "type is not a pybind11 base of the given instance "
-            "(compile in debug mode for type details)");
+                  "type is not a pybind11 base of the given instance "
+                  "(compile in debug mode for type details)");
 #else
-    pybind11_fail("pybind11::detail::instance::get_value_and_holder: `" +
-            get_fully_qualified_tp_name(find_type->type) + "' is not a pybind11 base of the given `" +
-            get_fully_qualified_tp_name(Py_TYPE(this)) + "' instance");
+    pybind11_fail("pybind11::detail::instance::get_value_and_holder: `"
+                  + get_fully_qualified_tp_name(find_type->type)
+                  + "' is not a pybind11 base of the given `"
+                  + get_fully_qualified_tp_name(Py_TYPE(this)) + "' instance");
 #endif
 }
 
 PYBIND11_NOINLINE void instance::allocate_layout() {
-    auto &tinfo = all_type_info(Py_TYPE(this));
+    const auto &tinfo = all_type_info(Py_TYPE(this));
 
     const size_t n_types = tinfo.size();
 
-    if (n_types == 0)
-        pybind11_fail("instance allocation failed: new instance has no pybind11-registered base types");
+    if (n_types == 0) {
+        pybind11_fail(
+            "instance allocation failed: new instance has no pybind11-registered base types");
+    }
 
-    simple_layout =
-        n_types == 1 && tinfo.front()->holder_size_in_ptrs <= instance_simple_holder_in_ptrs();
+    simple_layout
+        = n_types == 1 && tinfo.front()->holder_size_in_ptrs <= instance_simple_holder_in_ptrs();
 
     // Simple path: no python-side multiple inheritance, and a small-enough holder
     if (simple_layout) {
         simple_value_holder[0] = nullptr;
         simple_holder_constructed = false;
         simple_instance_registered = false;
-    }
-    else { // multiple base types or a too-large holder
+    } else { // multiple base types or a too-large holder
         // Allocate space to hold: [v1*][h1][v2*][h2]...[bb...] where [vN*] is a value pointer,
         // [hN] is the (uninitialized) holder instance for value N, and [bb...] is a set of bool
         // values that tracks whether each associated holder has been initialized.  Each [block] is
         // padded, if necessary, to an integer multiple of sizeof(void *).
         size_t space = 0;
-        for (auto t : tinfo) {
-            space += 1; // value pointer
+        for (auto *t : tinfo) {
+            space += 1;                      // value pointer
             space += t->holder_size_in_ptrs; // holder instance
         }
         size_t flags_at = space;
-        space += size_in_ptrs(n_types); // status bytes (holder_constructed and instance_registered)
+        space += size_in_ptrs(n_types); // status bytes (holder_constructed and
+                                        // instance_registered)
 
         // Allocate space for flags, values, and holders, and initialize it to 0 (flags and values,
         // in particular, need to be 0).  Use Python's memory allocation functions: in Python 3.6
         // they default to using pymalloc, which is designed to be efficient for small allocations
         // like the one we're doing here; in earlier versions (and for larger allocations) they are
         // just wrappers around malloc.
 #if PY_VERSION_HEX >= 0x03050000
         nonsimple.values_and_holders = (void **) PyMem_Calloc(space, sizeof(void *));
-        if (!nonsimple.values_and_holders) throw std::bad_alloc();
+        if (!nonsimple.values_and_holders) {
+            throw std::bad_alloc();
+        }
 #else
         nonsimple.values_and_holders = (void **) PyMem_New(void *, space);
-        if (!nonsimple.values_and_holders) throw std::bad_alloc();
+        if (!nonsimple.values_and_holders)
+            throw std::bad_alloc();
         std::memset(nonsimple.values_and_holders, 0, space * sizeof(void *));
 #endif
-        nonsimple.status = reinterpret_cast<std::uint8_t *>(&nonsimple.values_and_holders[flags_at]);
+        nonsimple.status
+            = reinterpret_cast<std::uint8_t *>(&nonsimple.values_and_holders[flags_at]);
     }
     owned = true;
 }
 
 // NOLINTNEXTLINE(readability-make-member-function-const)
 PYBIND11_NOINLINE void instance::deallocate_layout() {
-    if (!simple_layout)
+    if (!simple_layout) {
         PyMem_Free(nonsimple.values_and_holders);
+    }
 }
 
 PYBIND11_NOINLINE bool isinstance_generic(handle obj, const std::type_info &tp) {
     handle type = detail::get_type_handle(tp, false);
-    if (!type)
+    if (!type) {
         return false;
+    }
     return isinstance(obj, type);
 }
 
 PYBIND11_NOINLINE std::string error_string() {
     if (!PyErr_Occurred()) {
         PyErr_SetString(PyExc_RuntimeError, "Unknown internal error occurred");
         return "Unknown internal error occurred";
@@ -443,76 +484,87 @@
     error_scope scope; // Preserve error state
 
     std::string errorString;
     if (scope.type) {
         errorString += handle(scope.type).attr("__name__").cast<std::string>();
         errorString += ": ";
     }
-    if (scope.value)
+    if (scope.value) {
         errorString += (std::string) str(scope.value);
+    }
 
     PyErr_NormalizeException(&scope.type, &scope.value, &scope.trace);
 
 #if PY_MAJOR_VERSION >= 3
-    if (scope.trace != nullptr)
+    if (scope.trace != nullptr) {
         PyException_SetTraceback(scope.value, scope.trace);
+    }
 #endif
 
 #if !defined(PYPY_VERSION)
     if (scope.trace) {
         auto *trace = (PyTracebackObject *) scope.trace;
 
         /* Get the deepest trace possible */
-        while (trace->tb_next)
+        while (trace->tb_next) {
             trace = trace->tb_next;
+        }
 
         PyFrameObject *frame = trace->tb_frame;
+        Py_XINCREF(frame);
         errorString += "\n\nAt:\n";
         while (frame) {
-#if PY_VERSION_HEX >= 0x03090000
+#    if PY_VERSION_HEX >= 0x030900B1
             PyCodeObject *f_code = PyFrame_GetCode(frame);
-#else
+#    else
             PyCodeObject *f_code = frame->f_code;
             Py_INCREF(f_code);
-#endif
+#    endif
             int lineno = PyFrame_GetLineNumber(frame);
-            errorString +=
-                "  " + handle(f_code->co_filename).cast<std::string>() +
-                "(" + std::to_string(lineno) + "): " +
-                handle(f_code->co_name).cast<std::string>() + "\n";
-            frame = frame->f_back;
+            errorString += "  " + handle(f_code->co_filename).cast<std::string>() + "("
+                           + std::to_string(lineno)
+                           + "): " + handle(f_code->co_name).cast<std::string>() + "\n";
             Py_DECREF(f_code);
+#    if PY_VERSION_HEX >= 0x030900B1
+            auto *b_frame = PyFrame_GetBack(frame);
+#    else
+            auto *b_frame = frame->f_back;
+            Py_XINCREF(b_frame);
+#    endif
+            Py_DECREF(frame);
+            frame = b_frame;
         }
     }
 #endif
 
     return errorString;
 }
 
-PYBIND11_NOINLINE handle get_object_handle(const void *ptr, const detail::type_info *type ) {
+PYBIND11_NOINLINE handle get_object_handle(const void *ptr, const detail::type_info *type) {
     auto &instances = get_internals().registered_instances;
     auto range = instances.equal_range(ptr);
     for (auto it = range.first; it != range.second; ++it) {
         for (const auto &vh : values_and_holders(it->second)) {
-            if (vh.type == type)
+            if (vh.type == type) {
                 return handle((PyObject *) it->second);
+            }
         }
     }
     return handle();
 }
 
 inline PyThreadState *get_thread_state_unchecked() {
 #if defined(PYPY_VERSION)
     return PyThreadState_GET();
 #elif PY_VERSION_HEX < 0x03000000
     return _PyThreadState_Current;
 #elif PY_VERSION_HEX < 0x03050000
-    return (PyThreadState*) _Py_atomic_load_relaxed(&_PyThreadState_Current);
+    return (PyThreadState *) _Py_atomic_load_relaxed(&_PyThreadState_Current);
 #elif PY_VERSION_HEX < 0x03050200
-    return (PyThreadState*) _PyThreadState_Current.value;
+    return (PyThreadState *) _PyThreadState_Current.value;
 #else
     return _PyThreadState_UncheckedGet();
 #endif
 }
 
 // Forward declarations
 void keep_alive_impl(handle nurse, handle patient);
@@ -522,35 +574,38 @@
 public:
     PYBIND11_NOINLINE explicit type_caster_generic(const std::type_info &type_info)
         : typeinfo(get_type_info(type_info)), cpptype(&type_info) {}
 
     explicit type_caster_generic(const type_info *typeinfo)
         : typeinfo(typeinfo), cpptype(typeinfo ? typeinfo->cpptype : nullptr) {}
 
-    bool load(handle src, bool convert) {
-        return load_impl<type_caster_generic>(src, convert);
-    }
+    bool load(handle src, bool convert) { return load_impl<type_caster_generic>(src, convert); }
 
-    PYBIND11_NOINLINE static handle cast(const void *_src, return_value_policy policy, handle parent,
+    PYBIND11_NOINLINE static handle cast(const void *_src,
+                                         return_value_policy policy,
+                                         handle parent,
                                          const detail::type_info *tinfo,
                                          void *(*copy_constructor)(const void *),
                                          void *(*move_constructor)(const void *),
                                          const void *existing_holder = nullptr) {
-        if (!tinfo) // no type info: error will be set already
+        if (!tinfo) { // no type info: error will be set already
             return handle();
+        }
 
         void *src = const_cast<void *>(_src);
-        if (src == nullptr)
+        if (src == nullptr) {
             return none().release();
+        }
 
-        if (handle registered_inst = find_registered_python_instance(src, tinfo))
+        if (handle registered_inst = find_registered_python_instance(src, tinfo)) {
             return registered_inst;
+        }
 
         auto inst = reinterpret_steal<object>(make_new_instance(tinfo->type));
-        auto wrapper = reinterpret_cast<instance *>(inst.ptr());
+        auto *wrapper = reinterpret_cast<instance *>(inst.ptr());
         wrapper->owned = false;
         void *&valueptr = values_and_holders(wrapper).begin()->value_ptr();
 
         switch (policy) {
             case return_value_policy::automatic:
             case return_value_policy::take_ownership:
                 valueptr = src;
@@ -560,45 +615,45 @@
             case return_value_policy::automatic_reference:
             case return_value_policy::reference:
                 valueptr = src;
                 wrapper->owned = false;
                 break;
 
             case return_value_policy::copy:
-                if (copy_constructor)
+                if (copy_constructor) {
                     valueptr = copy_constructor(src);
-                else {
+                } else {
 #if defined(NDEBUG)
                     throw cast_error("return_value_policy = copy, but type is "
                                      "non-copyable! (compile in debug mode for details)");
 #else
                     std::string type_name(tinfo->cpptype->name());
                     detail::clean_type_id(type_name);
-                    throw cast_error("return_value_policy = copy, but type " +
-                                     type_name + " is non-copyable!");
+                    throw cast_error("return_value_policy = copy, but type " + type_name
+                                     + " is non-copyable!");
 #endif
                 }
                 wrapper->owned = true;
                 break;
 
             case return_value_policy::move:
-                if (move_constructor)
+                if (move_constructor) {
                     valueptr = move_constructor(src);
-                else if (copy_constructor)
+                } else if (copy_constructor) {
                     valueptr = copy_constructor(src);
-                else {
+                } else {
 #if defined(NDEBUG)
                     throw cast_error("return_value_policy = move, but type is neither "
                                      "movable nor copyable! "
                                      "(compile in debug mode for details)");
 #else
                     std::string type_name(tinfo->cpptype->name());
                     detail::clean_type_id(type_name);
-                    throw cast_error("return_value_policy = move, but type " +
-                                     type_name + " is neither movable nor copyable!");
+                    throw cast_error("return_value_policy = move, but type " + type_name
+                                     + " is neither movable nor copyable!");
 #endif
                 }
                 wrapper->owned = true;
                 break;
 
             case return_value_policy::reference_internal:
                 valueptr = src;
@@ -616,174 +671,193 @@
     }
 
     // Base methods for generic caster; there are overridden in copyable_holder_caster
     void load_value(value_and_holder &&v_h) {
         auto *&vptr = v_h.value_ptr();
         // Lazy allocation for unallocated values:
         if (vptr == nullptr) {
-            auto *type = v_h.type ? v_h.type : typeinfo;
+            const auto *type = v_h.type ? v_h.type : typeinfo;
             if (type->operator_new) {
                 vptr = type->operator_new(type->type_size);
             } else {
-                #if defined(__cpp_aligned_new) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
-                    if (type->type_align > __STDCPP_DEFAULT_NEW_ALIGNMENT__)
-                        vptr = ::operator new(type->type_size,
-                                              std::align_val_t(type->type_align));
-                    else
-                #endif
+#if defined(__cpp_aligned_new) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
+                if (type->type_align > __STDCPP_DEFAULT_NEW_ALIGNMENT__) {
+                    vptr = ::operator new(type->type_size, std::align_val_t(type->type_align));
+                } else {
+                    vptr = ::operator new(type->type_size);
+                }
+#else
                 vptr = ::operator new(type->type_size);
+#endif
             }
         }
         value = vptr;
     }
     bool try_implicit_casts(handle src, bool convert) {
-        for (auto &cast : typeinfo->implicit_casts) {
+        for (const auto &cast : typeinfo->implicit_casts) {
             type_caster_generic sub_caster(*cast.first);
             if (sub_caster.load(src, convert)) {
                 value = cast.second(sub_caster.value);
                 return true;
             }
         }
         return false;
     }
     bool try_direct_conversions(handle src) {
         for (auto &converter : *typeinfo->direct_conversions) {
-            if (converter(src.ptr(), value))
+            if (converter(src.ptr(), value)) {
                 return true;
+            }
         }
         return false;
     }
     void check_holder_compat() {}
 
     PYBIND11_NOINLINE static void *local_load(PyObject *src, const type_info *ti) {
         auto caster = type_caster_generic(ti);
-        if (caster.load(src, false))
+        if (caster.load(src, false)) {
             return caster.value;
+        }
         return nullptr;
     }
 
     /// Try to load with foreign typeinfo, if available. Used when there is no
     /// native typeinfo, or when the native one wasn't able to produce a value.
     PYBIND11_NOINLINE bool try_load_foreign_module_local(handle src) {
         constexpr auto *local_key = PYBIND11_MODULE_LOCAL_ID;
         const auto pytype = type::handle_of(src);
-        if (!hasattr(pytype, local_key))
+        if (!hasattr(pytype, local_key)) {
             return false;
+        }
 
         type_info *foreign_typeinfo = reinterpret_borrow<capsule>(getattr(pytype, local_key));
-        // Only consider this foreign loader if actually foreign and is a loader of the correct cpp type
+        // Only consider this foreign loader if actually foreign and is a loader of the correct cpp
+        // type
         if (foreign_typeinfo->module_local_load == &local_load
-            || (cpptype && !same_type(*cpptype, *foreign_typeinfo->cpptype)))
+            || (cpptype && !same_type(*cpptype, *foreign_typeinfo->cpptype))) {
             return false;
+        }
 
-        if (auto result = foreign_typeinfo->module_local_load(src.ptr(), foreign_typeinfo)) {
+        if (auto *result = foreign_typeinfo->module_local_load(src.ptr(), foreign_typeinfo)) {
             value = result;
             return true;
         }
         return false;
     }
 
     // Implementation of `load`; this takes the type of `this` so that it can dispatch the relevant
     // bits of code between here and copyable_holder_caster where the two classes need different
     // logic (without having to resort to virtual inheritance).
     template <typename ThisT>
     PYBIND11_NOINLINE bool load_impl(handle src, bool convert) {
-        if (!src) return false;
-        if (!typeinfo) return try_load_foreign_module_local(src);
+        if (!src) {
+            return false;
+        }
+        if (!typeinfo) {
+            return try_load_foreign_module_local(src);
+        }
 
         auto &this_ = static_cast<ThisT &>(*this);
         this_.check_holder_compat();
 
         PyTypeObject *srctype = Py_TYPE(src.ptr());
 
         // Case 1: If src is an exact type match for the target type then we can reinterpret_cast
         // the instance's value pointer to the target type:
         if (srctype == typeinfo->type) {
             this_.load_value(reinterpret_cast<instance *>(src.ptr())->get_value_and_holder());
             return true;
         }
         // Case 2: We have a derived class
         if (PyType_IsSubtype(srctype, typeinfo->type)) {
-            auto &bases = all_type_info(srctype);
+            const auto &bases = all_type_info(srctype);
             bool no_cpp_mi = typeinfo->simple_type;
 
             // Case 2a: the python type is a Python-inherited derived class that inherits from just
             // one simple (no MI) pybind11 class, or is an exact match, so the C++ instance is of
             // the right type and we can use reinterpret_cast.
             // (This is essentially the same as case 2b, but because not using multiple inheritance
             // is extremely common, we handle it specially to avoid the loop iterator and type
             // pointer lookup overhead)
             if (bases.size() == 1 && (no_cpp_mi || bases.front()->type == typeinfo->type)) {
                 this_.load_value(reinterpret_cast<instance *>(src.ptr())->get_value_and_holder());
                 return true;
             }
-            // Case 2b: the python type inherits from multiple C++ bases.  Check the bases to see if
-            // we can find an exact match (or, for a simple C++ type, an inherited match); if so, we
-            // can safely reinterpret_cast to the relevant pointer.
+            // Case 2b: the python type inherits from multiple C++ bases.  Check the bases to see
+            // if we can find an exact match (or, for a simple C++ type, an inherited match); if
+            // so, we can safely reinterpret_cast to the relevant pointer.
             if (bases.size() > 1) {
-                for (auto base : bases) {
-                    if (no_cpp_mi ? PyType_IsSubtype(base->type, typeinfo->type) : base->type == typeinfo->type) {
-                        this_.load_value(reinterpret_cast<instance *>(src.ptr())->get_value_and_holder(base));
+                for (auto *base : bases) {
+                    if (no_cpp_mi ? PyType_IsSubtype(base->type, typeinfo->type)
+                                  : base->type == typeinfo->type) {
+                        this_.load_value(
+                            reinterpret_cast<instance *>(src.ptr())->get_value_and_holder(base));
                         return true;
                     }
                 }
             }
 
-            // Case 2c: C++ multiple inheritance is involved and we couldn't find an exact type match
-            // in the registered bases, above, so try implicit casting (needed for proper C++ casting
-            // when MI is involved).
-            if (this_.try_implicit_casts(src, convert))
+            // Case 2c: C++ multiple inheritance is involved and we couldn't find an exact type
+            // match in the registered bases, above, so try implicit casting (needed for proper C++
+            // casting when MI is involved).
+            if (this_.try_implicit_casts(src, convert)) {
                 return true;
+            }
         }
 
         // Perform an implicit conversion
         if (convert) {
-            for (auto &converter : typeinfo->implicit_conversions) {
+            for (const auto &converter : typeinfo->implicit_conversions) {
                 auto temp = reinterpret_steal<object>(converter(src.ptr(), typeinfo->type));
                 if (load_impl<ThisT>(temp, false)) {
                     loader_life_support::add_patient(temp);
                     return true;
                 }
             }
-            if (this_.try_direct_conversions(src))
+            if (this_.try_direct_conversions(src)) {
                 return true;
+            }
         }
 
         // Failed to match local typeinfo. Try again with global.
         if (typeinfo->module_local) {
-            if (auto gtype = get_global_type_info(*typeinfo->cpptype)) {
+            if (auto *gtype = get_global_type_info(*typeinfo->cpptype)) {
                 typeinfo = gtype;
                 return load(src, false);
             }
         }
 
         // Global typeinfo has precedence over foreign module_local
         if (try_load_foreign_module_local(src)) {
-           return true;
+            return true;
         }
 
         // Custom converters didn't take None, now we convert None to nullptr.
         if (src.is_none()) {
-           // Defer accepting None to other overloads (if we aren't in convert mode):
-           if (!convert) return false;
-           value = nullptr;
-           return true;
+            // Defer accepting None to other overloads (if we aren't in convert mode):
+            if (!convert) {
+                return false;
+            }
+            value = nullptr;
+            return true;
         }
 
         return false;
     }
 
-
     // Called to do type lookup and wrap the pointer and type in a pair when a dynamic_cast
     // isn't needed or can't be used.  If the type is unknown, sets the error and returns a pair
     // with .second = nullptr.  (p.first = nullptr is not an error: it becomes None).
-    PYBIND11_NOINLINE static std::pair<const void *, const type_info *> src_and_type(
-            const void *src, const std::type_info &cast_type, const std::type_info *rtti_type = nullptr) {
-        if (auto *tpi = get_type_info(cast_type))
+    PYBIND11_NOINLINE static std::pair<const void *, const type_info *>
+    src_and_type(const void *src,
+                 const std::type_info &cast_type,
+                 const std::type_info *rtti_type = nullptr) {
+        if (auto *tpi = get_type_info(cast_type)) {
             return {src, const_cast<const type_info *>(tpi)};
+        }
 
         // Not found, set error:
         std::string tname = rtti_type ? rtti_type->name() : cast_type.name();
         detail::clean_type_id(tname);
         std::string msg = "Unregistered type : " + tname;
         PyErr_SetString(PyExc_TypeError, msg.c_str());
         return {nullptr, nullptr};
@@ -798,61 +872,70 @@
  * Determine suitable casting operator for pointer-or-lvalue-casting type casters.  The type caster
  * needs to provide `operator T*()` and `operator T&()` operators.
  *
  * If the type supports moving the value away via an `operator T&&() &&` method, it should use
  * `movable_cast_op_type` instead.
  */
 template <typename T>
-using cast_op_type =
-    conditional_t<std::is_pointer<remove_reference_t<T>>::value,
-        typename std::add_pointer<intrinsic_t<T>>::type,
-        typename std::add_lvalue_reference<intrinsic_t<T>>::type>;
+using cast_op_type = conditional_t<std::is_pointer<remove_reference_t<T>>::value,
+                                   typename std::add_pointer<intrinsic_t<T>>::type,
+                                   typename std::add_lvalue_reference<intrinsic_t<T>>::type>;
 
 /**
  * Determine suitable casting operator for a type caster with a movable value.  Such a type caster
  * needs to provide `operator T*()`, `operator T&()`, and `operator T&&() &&`.  The latter will be
  * called in appropriate contexts where the value can be moved rather than copied.
  *
  * These operator are automatically provided when using the PYBIND11_TYPE_CASTER macro.
  */
 template <typename T>
-using movable_cast_op_type =
-    conditional_t<std::is_pointer<typename std::remove_reference<T>::type>::value,
-        typename std::add_pointer<intrinsic_t<T>>::type,
-    conditional_t<std::is_rvalue_reference<T>::value,
-        typename std::add_rvalue_reference<intrinsic_t<T>>::type,
-        typename std::add_lvalue_reference<intrinsic_t<T>>::type>>;
+using movable_cast_op_type
+    = conditional_t<std::is_pointer<typename std::remove_reference<T>::type>::value,
+                    typename std::add_pointer<intrinsic_t<T>>::type,
+                    conditional_t<std::is_rvalue_reference<T>::value,
+                                  typename std::add_rvalue_reference<intrinsic_t<T>>::type,
+                                  typename std::add_lvalue_reference<intrinsic_t<T>>::type>>;
 
 // std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
 // T is non-copyable, but code containing such a copy constructor fails to actually compile.
-template <typename T, typename SFINAE = void> struct is_copy_constructible : std::is_copy_constructible<T> {};
+template <typename T, typename SFINAE = void>
+struct is_copy_constructible : std::is_copy_constructible<T> {};
 
 // Specialization for types that appear to be copy constructible but also look like stl containers
 // (we specifically check for: has `value_type` and `reference` with `reference = value_type&`): if
 // so, copy constructability depends on whether the value_type is copy constructible.
-template <typename Container> struct is_copy_constructible<Container, enable_if_t<all_of<
-        std::is_copy_constructible<Container>,
-        std::is_same<typename Container::value_type &, typename Container::reference>,
-        // Avoid infinite recursion
-        negation<std::is_same<Container, typename Container::value_type>>
-    >::value>> : is_copy_constructible<typename Container::value_type> {};
+template <typename Container>
+struct is_copy_constructible<
+    Container,
+    enable_if_t<
+        all_of<std::is_copy_constructible<Container>,
+               std::is_same<typename Container::value_type &, typename Container::reference>,
+               // Avoid infinite recursion
+               negation<std::is_same<Container, typename Container::value_type>>>::value>>
+    : is_copy_constructible<typename Container::value_type> {};
 
 // Likewise for std::pair
-// (after C++17 it is mandatory that the copy constructor not exist when the two types aren't themselves
-// copy constructible, but this can not be relied upon when T1 or T2 are themselves containers).
-template <typename T1, typename T2> struct is_copy_constructible<std::pair<T1, T2>>
+// (after C++17 it is mandatory that the copy constructor not exist when the two types aren't
+// themselves copy constructible, but this can not be relied upon when T1 or T2 are themselves
+// containers).
+template <typename T1, typename T2>
+struct is_copy_constructible<std::pair<T1, T2>>
     : all_of<is_copy_constructible<T1>, is_copy_constructible<T2>> {};
 
 // The same problems arise with std::is_copy_assignable, so we use the same workaround.
-template <typename T, typename SFINAE = void> struct is_copy_assignable : std::is_copy_assignable<T> {};
-template <typename Container> struct is_copy_assignable<Container, enable_if_t<all_of<
-        std::is_copy_assignable<Container>,
-        std::is_same<typename Container::value_type &, typename Container::reference>
-    >::value>> : is_copy_assignable<typename Container::value_type> {};
-template <typename T1, typename T2> struct is_copy_assignable<std::pair<T1, T2>>
+template <typename T, typename SFINAE = void>
+struct is_copy_assignable : std::is_copy_assignable<T> {};
+template <typename Container>
+struct is_copy_assignable<Container,
+                          enable_if_t<all_of<std::is_copy_assignable<Container>,
+                                             std::is_same<typename Container::value_type &,
+                                                          typename Container::reference>>::value>>
+    : is_copy_assignable<typename Container::value_type> {};
+template <typename T1, typename T2>
+struct is_copy_assignable<std::pair<T1, T2>>
     : all_of<is_copy_assignable<T1>, is_copy_assignable<T2>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 // polymorphic_type_hook<itype>::get(src, tinfo) determines whether the object pointed
 // to by `src` actually is an instance of some class derived from `itype`.
 // If so, it sets `tinfo` to point to the std::type_info representing that derived
@@ -871,111 +954,126 @@
 // polymorphic to Python but do not use C++ RTTI. (This is a not uncommon pattern
 // in performance-sensitive applications, used most notably in LLVM.)
 //
 // polymorphic_type_hook_base allows users to specialize polymorphic_type_hook with
 // std::enable_if. User provided specializations will always have higher priority than
 // the default implementation and specialization provided in polymorphic_type_hook_base.
 template <typename itype, typename SFINAE = void>
-struct polymorphic_type_hook_base
-{
-    static const void *get(const itype *src, const std::type_info*&) { return src; }
+struct polymorphic_type_hook_base {
+    static const void *get(const itype *src, const std::type_info *&) { return src; }
 };
 template <typename itype>
-struct polymorphic_type_hook_base<itype, detail::enable_if_t<std::is_polymorphic<itype>::value>>
-{
-    static const void *get(const itype *src, const std::type_info*& type) {
+struct polymorphic_type_hook_base<itype, detail::enable_if_t<std::is_polymorphic<itype>::value>> {
+    static const void *get(const itype *src, const std::type_info *&type) {
         type = src ? &typeid(*src) : nullptr;
-        return dynamic_cast<const void*>(src);
+        return dynamic_cast<const void *>(src);
     }
 };
 template <typename itype, typename SFINAE = void>
 struct polymorphic_type_hook : public polymorphic_type_hook_base<itype> {};
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Generic type caster for objects stored on the heap
-template <typename type> class type_caster_base : public type_caster_generic {
+template <typename type>
+class type_caster_base : public type_caster_generic {
     using itype = intrinsic_t<type>;
 
 public:
     static constexpr auto name = const_name<type>();
 
-    type_caster_base() : type_caster_base(typeid(type)) { }
-    explicit type_caster_base(const std::type_info &info) : type_caster_generic(info) { }
+    type_caster_base() : type_caster_base(typeid(type)) {}
+    explicit type_caster_base(const std::type_info &info) : type_caster_generic(info) {}
 
     static handle cast(const itype &src, return_value_policy policy, handle parent) {
-        if (policy == return_value_policy::automatic || policy == return_value_policy::automatic_reference)
+        if (policy == return_value_policy::automatic
+            || policy == return_value_policy::automatic_reference) {
             policy = return_value_policy::copy;
+        }
         return cast(&src, policy, parent);
     }
 
     static handle cast(itype &&src, return_value_policy, handle parent) {
         return cast(&src, return_value_policy::move, parent);
     }
 
     // Returns a (pointer, type_info) pair taking care of necessary type lookup for a
     // polymorphic type (using RTTI by default, but can be overridden by specializing
     // polymorphic_type_hook). If the instance isn't derived, returns the base version.
     static std::pair<const void *, const type_info *> src_and_type(const itype *src) {
-        auto &cast_type = typeid(itype);
+        const auto &cast_type = typeid(itype);
         const std::type_info *instance_type = nullptr;
         const void *vsrc = polymorphic_type_hook<itype>::get(src, instance_type);
         if (instance_type && !same_type(cast_type, *instance_type)) {
             // This is a base pointer to a derived type. If the derived type is registered
             // with pybind11, we want to make the full derived object available.
             // In the typical case where itype is polymorphic, we get the correct
             // derived pointer (which may be != base pointer) by a dynamic_cast to
             // most derived type. If itype is not polymorphic, we won't get here
             // except via a user-provided specialization of polymorphic_type_hook,
             // and the user has promised that no this-pointer adjustment is
             // required in that case, so it's OK to use static_cast.
-            if (const auto *tpi = get_type_info(*instance_type))
+            if (const auto *tpi = get_type_info(*instance_type)) {
                 return {vsrc, tpi};
+            }
         }
-        // Otherwise we have either a nullptr, an `itype` pointer, or an unknown derived pointer, so
-        // don't do a cast
+        // Otherwise we have either a nullptr, an `itype` pointer, or an unknown derived pointer,
+        // so don't do a cast
         return type_caster_generic::src_and_type(src, cast_type, instance_type);
     }
 
     static handle cast(const itype *src, return_value_policy policy, handle parent) {
         auto st = src_and_type(src);
-        return type_caster_generic::cast(
-            st.first, policy, parent, st.second,
-            make_copy_constructor(src), make_move_constructor(src));
+        return type_caster_generic::cast(st.first,
+                                         policy,
+                                         parent,
+                                         st.second,
+                                         make_copy_constructor(src),
+                                         make_move_constructor(src));
     }
 
     static handle cast_holder(const itype *src, const void *holder) {
         auto st = src_and_type(src);
-        return type_caster_generic::cast(
-            st.first, return_value_policy::take_ownership, {}, st.second,
-            nullptr, nullptr, holder);
+        return type_caster_generic::cast(st.first,
+                                         return_value_policy::take_ownership,
+                                         {},
+                                         st.second,
+                                         nullptr,
+                                         nullptr,
+                                         holder);
     }
 
-    template <typename T> using cast_op_type = detail::cast_op_type<T>;
+    template <typename T>
+    using cast_op_type = detail::cast_op_type<T>;
 
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator itype*() { return (type *) value; }
+    operator itype *() { return (type *) value; }
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator itype&() { if (!value) throw reference_cast_error(); return *((itype *) value); }
+    operator itype &() {
+        if (!value) {
+            throw reference_cast_error();
+        }
+        return *((itype *) value);
+    }
 
 protected:
-    using Constructor = void *(*)(const void *);
+    using Constructor = void *(*) (const void *);
 
     /* Only enabled when the types are {copy,move}-constructible *and* when the type
-       does not have a private operator new implementation. A comma operator is used in the decltype
-       argument to apply SFINAE to the public copy/move constructors.*/
+       does not have a private operator new implementation. A comma operator is used in the
+       decltype argument to apply SFINAE to the public copy/move constructors.*/
     template <typename T, typename = enable_if_t<is_copy_constructible<T>::value>>
-    static auto make_copy_constructor(const T *) -> decltype(new T(std::declval<const T>()), Constructor{}) {
-        return [](const void *arg) -> void * {
-            return new T(*reinterpret_cast<const T *>(arg));
-        };
+    static auto make_copy_constructor(const T *)
+        -> decltype(new T(std::declval<const T>()), Constructor{}) {
+        return [](const void *arg) -> void * { return new T(*reinterpret_cast<const T *>(arg)); };
     }
 
     template <typename T, typename = enable_if_t<std::is_move_constructible<T>::value>>
-    static auto make_move_constructor(const T *) -> decltype(new T(std::declval<T&&>()), Constructor{}) {
+    static auto make_move_constructor(const T *)
+        -> decltype(new T(std::declval<T &&>()), Constructor{}) {
         return [](const void *arg) -> void * {
             return new T(std::move(*const_cast<T *>(reinterpret_cast<const T *>(arg))));
         };
     }
 
     static Constructor make_copy_constructor(...) { return nullptr; }
     static Constructor make_move_constructor(...) { return nullptr; }
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/detail/typeid.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/detail/typeid.h`

 * *Files 11% similar despite different names*

```diff
@@ -9,47 +9,51 @@
 
 #pragma once
 
 #include <cstdio>
 #include <cstdlib>
 
 #if defined(__GNUG__)
-#include <cxxabi.h>
+#    include <cxxabi.h>
 #endif
 
 #include "common.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 /// Erase all occurrences of a substring
 inline void erase_all(std::string &string, const std::string &search) {
     for (size_t pos = 0;;) {
         pos = string.find(search, pos);
-        if (pos == std::string::npos) break;
+        if (pos == std::string::npos) {
+            break;
+        }
         string.erase(pos, search.length());
     }
 }
 
 PYBIND11_NOINLINE void clean_type_id(std::string &name) {
 #if defined(__GNUG__)
     int status = 0;
-    std::unique_ptr<char, void (*)(void *)> res {
-        abi::__cxa_demangle(name.c_str(), nullptr, nullptr, &status), std::free };
-    if (status == 0)
+    std::unique_ptr<char, void (*)(void *)> res{
+        abi::__cxa_demangle(name.c_str(), nullptr, nullptr, &status), std::free};
+    if (status == 0) {
         name = res.get();
+    }
 #else
     detail::erase_all(name, "class ");
     detail::erase_all(name, "struct ");
     detail::erase_all(name, "enum ");
 #endif
     detail::erase_all(name, "pybind11::");
 }
 PYBIND11_NAMESPACE_END(detail)
 
 /// Return a string representation of a C++ type
-template <typename T> static std::string type_id() {
+template <typename T>
+static std::string type_id() {
     std::string name(typeid(T).name());
     detail::clean_type_id(name);
     return name;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/eigen.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/eigen.h`

 * *Files 10% similar despite different names*

```diff
@@ -19,212 +19,247 @@
 
 // The C4127 suppression was introduced for Eigen 3.4.0. In theory we could
 // make it version specific, or even remove it later, but considering that
 // 1. C4127 is generally far more distracting than useful for modern template code, and
 // 2. we definitely want to ignore any MSVC warnings originating from Eigen code,
 // it is probably best to keep this around indefinitely.
 #if defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4127) // C4127: conditional expression is constant
+#    pragma warning(push)
+#    pragma warning(disable : 4127) // C4127: conditional expression is constant
 #endif
 
 #include <Eigen/Core>
 #include <Eigen/SparseCore>
 
 #if defined(_MSC_VER)
-#  pragma warning(pop)
+#    pragma warning(pop)
 #endif
 
 // Eigen prior to 3.2.7 doesn't have proper move constructors--but worse, some classes get implicit
 // move constructors that break things.  We could detect this an explicitly copy, but an extra copy
 // of matrices seems highly undesirable.
-static_assert(EIGEN_VERSION_AT_LEAST(3,2,7), "Eigen support in pybind11 requires Eigen >= 3.2.7");
+static_assert(EIGEN_VERSION_AT_LEAST(3, 2, 7),
+              "Eigen support in pybind11 requires Eigen >= 3.2.7");
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 // Provide a convenience alias for easier pass-by-ref usage with fully dynamic strides:
 using EigenDStride = Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>;
-template <typename MatrixType> using EigenDRef = Eigen::Ref<MatrixType, 0, EigenDStride>;
-template <typename MatrixType> using EigenDMap = Eigen::Map<MatrixType, 0, EigenDStride>;
+template <typename MatrixType>
+using EigenDRef = Eigen::Ref<MatrixType, 0, EigenDStride>;
+template <typename MatrixType>
+using EigenDMap = Eigen::Map<MatrixType, 0, EigenDStride>;
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-#if EIGEN_VERSION_AT_LEAST(3,3,0)
+#if EIGEN_VERSION_AT_LEAST(3, 3, 0)
 using EigenIndex = Eigen::Index;
-template<typename Scalar, int Flags, typename StorageIndex>
+template <typename Scalar, int Flags, typename StorageIndex>
 using EigenMapSparseMatrix = Eigen::Map<Eigen::SparseMatrix<Scalar, Flags, StorageIndex>>;
 #else
 using EigenIndex = EIGEN_DEFAULT_DENSE_INDEX_TYPE;
-template<typename Scalar, int Flags, typename StorageIndex>
+template <typename Scalar, int Flags, typename StorageIndex>
 using EigenMapSparseMatrix = Eigen::MappedSparseMatrix<Scalar, Flags, StorageIndex>;
 #endif
 
 // Matches Eigen::Map, Eigen::Ref, blocks, etc:
-template <typename T> using is_eigen_dense_map = all_of<is_template_base_of<Eigen::DenseBase, T>, std::is_base_of<Eigen::MapBase<T, Eigen::ReadOnlyAccessors>, T>>;
-template <typename T> using is_eigen_mutable_map = std::is_base_of<Eigen::MapBase<T, Eigen::WriteAccessors>, T>;
-template <typename T> using is_eigen_dense_plain = all_of<negation<is_eigen_dense_map<T>>, is_template_base_of<Eigen::PlainObjectBase, T>>;
-template <typename T> using is_eigen_sparse = is_template_base_of<Eigen::SparseMatrixBase, T>;
+template <typename T>
+using is_eigen_dense_map = all_of<is_template_base_of<Eigen::DenseBase, T>,
+                                  std::is_base_of<Eigen::MapBase<T, Eigen::ReadOnlyAccessors>, T>>;
+template <typename T>
+using is_eigen_mutable_map = std::is_base_of<Eigen::MapBase<T, Eigen::WriteAccessors>, T>;
+template <typename T>
+using is_eigen_dense_plain
+    = all_of<negation<is_eigen_dense_map<T>>, is_template_base_of<Eigen::PlainObjectBase, T>>;
+template <typename T>
+using is_eigen_sparse = is_template_base_of<Eigen::SparseMatrixBase, T>;
 // Test for objects inheriting from EigenBase<Derived> that aren't captured by the above.  This
 // basically covers anything that can be assigned to a dense matrix but that don't have a typical
 // matrix data layout that can be copied from their .data().  For example, DiagonalMatrix and
 // SelfAdjointView fall into this category.
-template <typename T> using is_eigen_other = all_of<
-    is_template_base_of<Eigen::EigenBase, T>,
-    negation<any_of<is_eigen_dense_map<T>, is_eigen_dense_plain<T>, is_eigen_sparse<T>>>
->;
+template <typename T>
+using is_eigen_other
+    = all_of<is_template_base_of<Eigen::EigenBase, T>,
+             negation<any_of<is_eigen_dense_map<T>, is_eigen_dense_plain<T>, is_eigen_sparse<T>>>>;
 
 // Captures numpy/eigen conformability status (returned by EigenProps::conformable()):
-template <bool EigenRowMajor> struct EigenConformable {
+template <bool EigenRowMajor>
+struct EigenConformable {
     bool conformable = false;
     EigenIndex rows = 0, cols = 0;
-    EigenDStride stride{0, 0};      // Only valid if negativestrides is false!
-    bool negativestrides = false;   // If true, do not use stride!
+    EigenDStride stride{0, 0};    // Only valid if negativestrides is false!
+    bool negativestrides = false; // If true, do not use stride!
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     EigenConformable(bool fits = false) : conformable{fits} {}
     // Matrix type:
-    EigenConformable(EigenIndex r, EigenIndex c,
-            EigenIndex rstride, EigenIndex cstride) :
-        conformable{true}, rows{r}, cols{c},
-        //TODO: when Eigen bug #747 is fixed, remove the tests for non-negativity. http://eigen.tuxfamily.org/bz/show_bug.cgi?id=747
-        stride{EigenRowMajor ? (rstride > 0 ? rstride : 0) : (cstride > 0 ? cstride : 0) /* outer stride */,
-               EigenRowMajor ? (cstride > 0 ? cstride : 0) : (rstride > 0 ? rstride : 0) /* inner stride */ },
-        negativestrides{rstride < 0 || cstride < 0} {
-
-    }
+    EigenConformable(EigenIndex r, EigenIndex c, EigenIndex rstride, EigenIndex cstride)
+        : conformable{true}, rows{r}, cols{c},
+          // TODO: when Eigen bug #747 is fixed, remove the tests for non-negativity.
+          // http://eigen.tuxfamily.org/bz/show_bug.cgi?id=747
+          stride{EigenRowMajor ? (rstride > 0 ? rstride : 0)
+                               : (cstride > 0 ? cstride : 0) /* outer stride */,
+                 EigenRowMajor ? (cstride > 0 ? cstride : 0)
+                               : (rstride > 0 ? rstride : 0) /* inner stride */},
+          negativestrides{rstride < 0 || cstride < 0} {}
     // Vector type:
     EigenConformable(EigenIndex r, EigenIndex c, EigenIndex stride)
-        : EigenConformable(r, c, r == 1 ? c*stride : stride, c == 1 ? r : r*stride) {}
+        : EigenConformable(r, c, r == 1 ? c * stride : stride, c == 1 ? r : r * stride) {}
 
-    template <typename props> bool stride_compatible() const {
+    template <typename props>
+    bool stride_compatible() const {
         // To have compatible strides, we need (on both dimensions) one of fully dynamic strides,
-        // matching strides, or a dimension size of 1 (in which case the stride value is irrelevant)
-        return
-            !negativestrides &&
-            (props::inner_stride == Eigen::Dynamic || props::inner_stride == stride.inner() ||
-                (EigenRowMajor ? cols : rows) == 1) &&
-            (props::outer_stride == Eigen::Dynamic || props::outer_stride == stride.outer() ||
-                (EigenRowMajor ? rows : cols) == 1);
+        // matching strides, or a dimension size of 1 (in which case the stride value is
+        // irrelevant)
+        return !negativestrides
+               && (props::inner_stride == Eigen::Dynamic || props::inner_stride == stride.inner()
+                   || (EigenRowMajor ? cols : rows) == 1)
+               && (props::outer_stride == Eigen::Dynamic || props::outer_stride == stride.outer()
+                   || (EigenRowMajor ? rows : cols) == 1);
     }
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator bool() const { return conformable; }
 };
 
-template <typename Type> struct eigen_extract_stride { using type = Type; };
+template <typename Type>
+struct eigen_extract_stride {
+    using type = Type;
+};
 template <typename PlainObjectType, int MapOptions, typename StrideType>
-struct eigen_extract_stride<Eigen::Map<PlainObjectType, MapOptions, StrideType>> { using type = StrideType; };
+struct eigen_extract_stride<Eigen::Map<PlainObjectType, MapOptions, StrideType>> {
+    using type = StrideType;
+};
 template <typename PlainObjectType, int Options, typename StrideType>
-struct eigen_extract_stride<Eigen::Ref<PlainObjectType, Options, StrideType>> { using type = StrideType; };
+struct eigen_extract_stride<Eigen::Ref<PlainObjectType, Options, StrideType>> {
+    using type = StrideType;
+};
 
 // Helper struct for extracting information from an Eigen type
-template <typename Type_> struct EigenProps {
+template <typename Type_>
+struct EigenProps {
     using Type = Type_;
     using Scalar = typename Type::Scalar;
     using StrideType = typename eigen_extract_stride<Type>::type;
-    static constexpr EigenIndex
-        rows = Type::RowsAtCompileTime,
-        cols = Type::ColsAtCompileTime,
-        size = Type::SizeAtCompileTime;
-    static constexpr bool
-        row_major = Type::IsRowMajor,
-        vector = Type::IsVectorAtCompileTime, // At least one dimension has fixed size 1
-        fixed_rows = rows != Eigen::Dynamic,
-        fixed_cols = cols != Eigen::Dynamic,
-        fixed = size != Eigen::Dynamic, // Fully-fixed size
-        dynamic = !fixed_rows && !fixed_cols; // Fully-dynamic size
-
-    template <EigenIndex i, EigenIndex ifzero> using if_zero = std::integral_constant<EigenIndex, i == 0 ? ifzero : i>;
-    static constexpr EigenIndex inner_stride = if_zero<StrideType::InnerStrideAtCompileTime, 1>::value,
-                                outer_stride = if_zero<StrideType::OuterStrideAtCompileTime,
-                                                       vector ? size : row_major ? cols : rows>::value;
-    static constexpr bool dynamic_stride = inner_stride == Eigen::Dynamic && outer_stride == Eigen::Dynamic;
-    static constexpr bool requires_row_major = !dynamic_stride && !vector && (row_major ? inner_stride : outer_stride) == 1;
-    static constexpr bool requires_col_major = !dynamic_stride && !vector && (row_major ? outer_stride : inner_stride) == 1;
+    static constexpr EigenIndex rows = Type::RowsAtCompileTime, cols = Type::ColsAtCompileTime,
+                                size = Type::SizeAtCompileTime;
+    static constexpr bool row_major = Type::IsRowMajor,
+                          vector
+                          = Type::IsVectorAtCompileTime, // At least one dimension has fixed size 1
+        fixed_rows = rows != Eigen::Dynamic, fixed_cols = cols != Eigen::Dynamic,
+                          fixed = size != Eigen::Dynamic, // Fully-fixed size
+        dynamic = !fixed_rows && !fixed_cols;             // Fully-dynamic size
+
+    template <EigenIndex i, EigenIndex ifzero>
+    using if_zero = std::integral_constant<EigenIndex, i == 0 ? ifzero : i>;
+    static constexpr EigenIndex inner_stride
+        = if_zero<StrideType::InnerStrideAtCompileTime, 1>::value,
+        outer_stride = if_zero < StrideType::OuterStrideAtCompileTime,
+        vector      ? size
+        : row_major ? cols
+                    : rows > ::value;
+    static constexpr bool dynamic_stride
+        = inner_stride == Eigen::Dynamic && outer_stride == Eigen::Dynamic;
+    static constexpr bool requires_row_major
+        = !dynamic_stride && !vector && (row_major ? inner_stride : outer_stride) == 1;
+    static constexpr bool requires_col_major
+        = !dynamic_stride && !vector && (row_major ? outer_stride : inner_stride) == 1;
 
     // Takes an input array and determines whether we can make it fit into the Eigen type.  If
     // the array is a vector, we attempt to fit it into either an Eigen 1xN or Nx1 vector
     // (preferring the latter if it will fit in either, i.e. for a fully dynamic matrix type).
     static EigenConformable<row_major> conformable(const array &a) {
         const auto dims = a.ndim();
-        if (dims < 1 || dims > 2)
+        if (dims < 1 || dims > 2) {
             return false;
+        }
 
         if (dims == 2) { // Matrix type: require exact match (or dynamic)
 
-            EigenIndex
-                np_rows = a.shape(0),
-                np_cols = a.shape(1),
-                np_rstride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar)),
-                np_cstride = a.strides(1) / static_cast<ssize_t>(sizeof(Scalar));
-            if ((PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && np_rows != rows) ||
-                (PYBIND11_SILENCE_MSVC_C4127(fixed_cols) && np_cols != cols))
+            EigenIndex np_rows = a.shape(0), np_cols = a.shape(1),
+                       np_rstride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar)),
+                       np_cstride = a.strides(1) / static_cast<ssize_t>(sizeof(Scalar));
+            if ((PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && np_rows != rows)
+                || (PYBIND11_SILENCE_MSVC_C4127(fixed_cols) && np_cols != cols)) {
                 return false;
+            }
 
             return {np_rows, np_cols, np_rstride, np_cstride};
         }
 
-        // Otherwise we're storing an n-vector.  Only one of the strides will be used, but whichever
-        // is used, we want the (single) numpy stride value.
+        // Otherwise we're storing an n-vector.  Only one of the strides will be used, but
+        // whichever is used, we want the (single) numpy stride value.
         const EigenIndex n = a.shape(0),
-              stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
+                         stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
 
         if (vector) { // Eigen type is a compile-time vector
-            if (PYBIND11_SILENCE_MSVC_C4127(fixed) && size != n)
+            if (PYBIND11_SILENCE_MSVC_C4127(fixed) && size != n) {
                 return false; // Vector size mismatch
+            }
             return {rows == 1 ? 1 : n, cols == 1 ? 1 : n, stride};
         }
         if (fixed) {
             // The type has a fixed size, but is not a vector: abort
             return false;
         }
         if (fixed_cols) {
             // Since this isn't a vector, cols must be != 1.  We allow this only if it exactly
             // equals the number of elements (rows is Dynamic, and so 1 row is allowed).
-            if (cols != n) return false;
+            if (cols != n) {
+                return false;
+            }
             return {1, n, stride};
         } // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
-            if (PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && rows != n) return false;
-            return {n, 1, stride};
+        if (PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && rows != n) {
+            return false;
+        }
+        return {n, 1, stride};
     }
 
-    static constexpr bool show_writeable = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
+    static constexpr bool show_writeable
+        = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
     static constexpr bool show_order = is_eigen_dense_map<Type>::value;
     static constexpr bool show_c_contiguous = show_order && requires_row_major;
-    static constexpr bool show_f_contiguous = !show_c_contiguous && show_order && requires_col_major;
+    static constexpr bool show_f_contiguous
+        = !show_c_contiguous && show_order && requires_col_major;
 
-    static constexpr auto descriptor =
-        const_name("numpy.ndarray[") + npy_format_descriptor<Scalar>::name +
-        const_name("[")  + const_name<fixed_rows>(const_name<(size_t) rows>(), const_name("m")) +
-        const_name(", ") + const_name<fixed_cols>(const_name<(size_t) cols>(), const_name("n")) +
-        const_name("]") +
-        // For a reference type (e.g. Ref<MatrixXd>) we have other constraints that might need to be
-        // satisfied: writeable=True (for a mutable reference), and, depending on the map's stride
-        // options, possibly f_contiguous or c_contiguous.  We include them in the descriptor output
-        // to provide some hint as to why a TypeError is occurring (otherwise it can be confusing to
-        // see that a function accepts a 'numpy.ndarray[float64[3,2]]' and an error message that you
-        // *gave* a numpy.ndarray of the right type and dimensions.
-        const_name<show_writeable>(", flags.writeable", "") +
-        const_name<show_c_contiguous>(", flags.c_contiguous", "") +
-        const_name<show_f_contiguous>(", flags.f_contiguous", "") +
-        const_name("]");
+    static constexpr auto descriptor
+        = const_name("numpy.ndarray[") + npy_format_descriptor<Scalar>::name + const_name("[")
+          + const_name<fixed_rows>(const_name<(size_t) rows>(), const_name("m")) + const_name(", ")
+          + const_name<fixed_cols>(const_name<(size_t) cols>(), const_name("n")) + const_name("]")
+          +
+          // For a reference type (e.g. Ref<MatrixXd>) we have other constraints that might need to
+          // be satisfied: writeable=True (for a mutable reference), and, depending on the map's
+          // stride options, possibly f_contiguous or c_contiguous.  We include them in the
+          // descriptor output to provide some hint as to why a TypeError is occurring (otherwise
+          // it can be confusing to see that a function accepts a 'numpy.ndarray[float64[3,2]]' and
+          // an error message that you *gave* a numpy.ndarray of the right type and dimensions.
+          const_name<show_writeable>(", flags.writeable", "")
+          + const_name<show_c_contiguous>(", flags.c_contiguous", "")
+          + const_name<show_f_contiguous>(", flags.f_contiguous", "") + const_name("]");
 };
 
 // Casts an Eigen type to numpy array.  If given a base, the numpy array references the src data,
 // otherwise it'll make a copy.  writeable lets you turn off the writeable flag for the array.
-template <typename props> handle eigen_array_cast(typename props::Type const &src, handle base = handle(), bool writeable = true) {
+template <typename props>
+handle
+eigen_array_cast(typename props::Type const &src, handle base = handle(), bool writeable = true) {
     constexpr ssize_t elem_size = sizeof(typename props::Scalar);
     array a;
-    if (props::vector)
-        a = array({ src.size() }, { elem_size * src.innerStride() }, src.data(), base);
-    else
-        a = array({ src.rows(), src.cols() }, { elem_size * src.rowStride(), elem_size * src.colStride() },
-                  src.data(), base);
+    if (props::vector) {
+        a = array({src.size()}, {elem_size * src.innerStride()}, src.data(), base);
+    } else {
+        a = array({src.rows(), src.cols()},
+                  {elem_size * src.rowStride(), elem_size * src.colStride()},
+                  src.data(),
+                  base);
+    }
 
-    if (!writeable)
+    if (!writeable) {
         array_proxy(a.ptr())->flags &= ~detail::npy_api::NPY_ARRAY_WRITEABLE_;
+    }
 
     return a.release();
 }
 
 // Takes an lvalue ref to some Eigen type and a (python) base object, creating a numpy array that
 // reference the Eigen object's data with `base` as the python-registered base class (if omitted,
 // the base will be set to None, and lifetime management is up to the caller).  The numpy array is
@@ -232,68 +267,74 @@
 template <typename props, typename Type>
 handle eigen_ref_array(Type &src, handle parent = none()) {
     // none here is to get past array's should-we-copy detection, which currently always
     // copies when there is no base.  Setting the base to None should be harmless.
     return eigen_array_cast<props>(src, parent, !std::is_const<Type>::value);
 }
 
-// Takes a pointer to some dense, plain Eigen type, builds a capsule around it, then returns a numpy
-// array that references the encapsulated data with a python-side reference to the capsule to tie
-// its destruction to that of any dependent python objects.  Const-ness is determined by whether or
-// not the Type of the pointer given is const.
+// Takes a pointer to some dense, plain Eigen type, builds a capsule around it, then returns a
+// numpy array that references the encapsulated data with a python-side reference to the capsule to
+// tie its destruction to that of any dependent python objects.  Const-ness is determined by
+// whether or not the Type of the pointer given is const.
 template <typename props, typename Type, typename = enable_if_t<is_eigen_dense_plain<Type>::value>>
 handle eigen_encapsulate(Type *src) {
     capsule base(src, [](void *o) { delete static_cast<Type *>(o); });
     return eigen_ref_array<props>(*src, base);
 }
 
 // Type caster for regular, dense matrix types (e.g. MatrixXd), but not maps/refs/etc. of dense
 // types.
-template<typename Type>
+template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_dense_plain<Type>::value>> {
     using Scalar = typename Type::Scalar;
     using props = EigenProps<Type>;
 
     bool load(handle src, bool convert) {
         // If we're in no-convert mode, only load if given an array of the correct type
-        if (!convert && !isinstance<array_t<Scalar>>(src))
+        if (!convert && !isinstance<array_t<Scalar>>(src)) {
             return false;
+        }
 
         // Coerce into an array, but don't do type conversion yet; the copy below handles it.
         auto buf = array::ensure(src);
 
-        if (!buf)
+        if (!buf) {
             return false;
+        }
 
         auto dims = buf.ndim();
-        if (dims < 1 || dims > 2)
+        if (dims < 1 || dims > 2) {
             return false;
+        }
 
         auto fits = props::conformable(buf);
-        if (!fits)
+        if (!fits) {
             return false;
+        }
 
         // Allocate the new type, then build a numpy reference into it
         value = Type(fits.rows, fits.cols);
         auto ref = reinterpret_steal<array>(eigen_ref_array<props>(value));
-        if (dims == 1) ref = ref.squeeze();
-        else if (ref.ndim() == 1) buf = buf.squeeze();
+        if (dims == 1) {
+            ref = ref.squeeze();
+        } else if (ref.ndim() == 1) {
+            buf = buf.squeeze();
+        }
 
         int result = detail::npy_api::get().PyArray_CopyInto_(ref.ptr(), buf.ptr());
 
         if (result < 0) { // Copy failed!
             PyErr_Clear();
             return false;
         }
 
         return true;
     }
 
 private:
-
     // Cast implementation
     template <typename CType>
     static handle cast_impl(CType *src, return_value_policy policy, handle parent) {
         switch (policy) {
             case return_value_policy::take_ownership:
             case return_value_policy::automatic:
                 return eigen_encapsulate<props>(src);
@@ -308,71 +349,75 @@
                 return eigen_ref_array<props>(*src, parent);
             default:
                 throw cast_error("unhandled return_value_policy: should not happen!");
         };
     }
 
 public:
-
     // Normal returned non-reference, non-const value:
     static handle cast(Type &&src, return_value_policy /* policy */, handle parent) {
         return cast_impl(&src, return_value_policy::move, parent);
     }
     // If you return a non-reference const, we mark the numpy array readonly:
     static handle cast(const Type &&src, return_value_policy /* policy */, handle parent) {
         return cast_impl(&src, return_value_policy::move, parent);
     }
     // lvalue reference return; default (automatic) becomes copy
     static handle cast(Type &src, return_value_policy policy, handle parent) {
-        if (policy == return_value_policy::automatic || policy == return_value_policy::automatic_reference)
+        if (policy == return_value_policy::automatic
+            || policy == return_value_policy::automatic_reference) {
             policy = return_value_policy::copy;
+        }
         return cast_impl(&src, policy, parent);
     }
     // const lvalue reference return; default (automatic) becomes copy
     static handle cast(const Type &src, return_value_policy policy, handle parent) {
-        if (policy == return_value_policy::automatic || policy == return_value_policy::automatic_reference)
+        if (policy == return_value_policy::automatic
+            || policy == return_value_policy::automatic_reference) {
             policy = return_value_policy::copy;
+        }
         return cast(&src, policy, parent);
     }
     // non-const pointer return
     static handle cast(Type *src, return_value_policy policy, handle parent) {
         return cast_impl(src, policy, parent);
     }
     // const pointer return
     static handle cast(const Type *src, return_value_policy policy, handle parent) {
         return cast_impl(src, policy, parent);
     }
 
     static constexpr auto name = props::descriptor;
 
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator Type*() { return &value; }
+    operator Type *() { return &value; }
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator Type&() { return value; }
+    operator Type &() { return value; }
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator Type&&() && { return std::move(value); }
-    template <typename T> using cast_op_type = movable_cast_op_type<T>;
+    operator Type &&() && { return std::move(value); }
+    template <typename T>
+    using cast_op_type = movable_cast_op_type<T>;
 
 private:
     Type value;
 };
 
 // Base class for casting reference/map/block/etc. objects back to python.
-template <typename MapType> struct eigen_map_caster {
+template <typename MapType>
+struct eigen_map_caster {
 private:
     using props = EigenProps<MapType>;
 
 public:
-
     // Directly referencing a ref/map's data is a bit dangerous (whatever the map/ref points to has
-    // to stay around), but we'll allow it under the assumption that you know what you're doing (and
-    // have an appropriate keep_alive in place).  We return a numpy array pointing directly at the
-    // ref's data (The numpy array ends up read-only if the ref was to a const matrix type.) Note
-    // that this means you need to ensure you don't destroy the object in some other way (e.g. with
-    // an appropriate keep_alive, or with a reference to a statically allocated matrix).
+    // to stay around), but we'll allow it under the assumption that you know what you're doing
+    // (and have an appropriate keep_alive in place).  We return a numpy array pointing directly at
+    // the ref's data (The numpy array ends up read-only if the ref was to a const matrix type.)
+    // Note that this means you need to ensure you don't destroy the object in some other way (e.g.
+    // with an appropriate keep_alive, or with a reference to a statically allocated matrix).
     static handle cast(const MapType &src, return_value_policy policy, handle parent) {
         switch (policy) {
             case return_value_policy::copy:
                 return eigen_array_cast<props>(src);
             case return_value_policy::reference_internal:
                 return eigen_array_cast<props>(src, parent, is_eigen_mutable_map<MapType>::value);
             case return_value_policy::reference:
@@ -388,179 +433,220 @@
     static constexpr auto name = props::descriptor;
 
     // Explicitly delete these: support python -> C++ conversion on these (i.e. these can be return
     // types but not bound arguments).  We still provide them (with an explicitly delete) so that
     // you end up here if you try anyway.
     bool load(handle, bool) = delete;
     operator MapType() = delete;
-    template <typename> using cast_op_type = MapType;
+    template <typename>
+    using cast_op_type = MapType;
 };
 
 // We can return any map-like object (but can only load Refs, specialized next):
-template <typename Type> struct type_caster<Type, enable_if_t<is_eigen_dense_map<Type>::value>>
-    : eigen_map_caster<Type> {};
+template <typename Type>
+struct type_caster<Type, enable_if_t<is_eigen_dense_map<Type>::value>> : eigen_map_caster<Type> {};
 
 // Loader for Ref<...> arguments.  See the documentation for info on how to make this work without
 // copying (it requires some extra effort in many cases).
 template <typename PlainObjectType, typename StrideType>
 struct type_caster<
     Eigen::Ref<PlainObjectType, 0, StrideType>,
-    enable_if_t<is_eigen_dense_map<Eigen::Ref<PlainObjectType, 0, StrideType>>::value>
-> : public eigen_map_caster<Eigen::Ref<PlainObjectType, 0, StrideType>> {
+    enable_if_t<is_eigen_dense_map<Eigen::Ref<PlainObjectType, 0, StrideType>>::value>>
+    : public eigen_map_caster<Eigen::Ref<PlainObjectType, 0, StrideType>> {
 private:
     using Type = Eigen::Ref<PlainObjectType, 0, StrideType>;
     using props = EigenProps<Type>;
     using Scalar = typename props::Scalar;
     using MapType = Eigen::Map<PlainObjectType, 0, StrideType>;
-    using Array = array_t<Scalar, array::forcecast |
-                ((props::row_major ? props::inner_stride : props::outer_stride) == 1 ? array::c_style :
-                 (props::row_major ? props::outer_stride : props::inner_stride) == 1 ? array::f_style : 0)>;
+    using Array
+        = array_t<Scalar,
+                  array::forcecast
+                      | ((props::row_major ? props::inner_stride : props::outer_stride) == 1
+                             ? array::c_style
+                         : (props::row_major ? props::outer_stride : props::inner_stride) == 1
+                             ? array::f_style
+                             : 0)>;
     static constexpr bool need_writeable = is_eigen_mutable_map<Type>::value;
     // Delay construction (these have no default constructor)
     std::unique_ptr<MapType> map;
     std::unique_ptr<Type> ref;
     // Our array.  When possible, this is just a numpy array pointing to the source data, but
-    // sometimes we can't avoid copying (e.g. input is not a numpy array at all, has an incompatible
-    // layout, or is an array of a type that needs to be converted).  Using a numpy temporary
-    // (rather than an Eigen temporary) saves an extra copy when we need both type conversion and
-    // storage order conversion.  (Note that we refuse to use this temporary copy when loading an
-    // argument for a Ref<M> with M non-const, i.e. a read-write reference).
+    // sometimes we can't avoid copying (e.g. input is not a numpy array at all, has an
+    // incompatible layout, or is an array of a type that needs to be converted).  Using a numpy
+    // temporary (rather than an Eigen temporary) saves an extra copy when we need both type
+    // conversion and storage order conversion.  (Note that we refuse to use this temporary copy
+    // when loading an argument for a Ref<M> with M non-const, i.e. a read-write reference).
     Array copy_or_ref;
+
 public:
     bool load(handle src, bool convert) {
-        // First check whether what we have is already an array of the right type.  If not, we can't
-        // avoid a copy (because the copy is also going to do type conversion).
+        // First check whether what we have is already an array of the right type.  If not, we
+        // can't avoid a copy (because the copy is also going to do type conversion).
         bool need_copy = !isinstance<Array>(src);
 
         EigenConformable<props::row_major> fits;
         if (!need_copy) {
             // We don't need a converting copy, but we also need to check whether the strides are
             // compatible with the Ref's stride requirements
             auto aref = reinterpret_borrow<Array>(src);
 
             if (aref && (!need_writeable || aref.writeable())) {
                 fits = props::conformable(aref);
-                if (!fits) return false; // Incompatible dimensions
-                if (!fits.template stride_compatible<props>())
+                if (!fits) {
+                    return false; // Incompatible dimensions
+                }
+                if (!fits.template stride_compatible<props>()) {
                     need_copy = true;
-                else
+                } else {
                     copy_or_ref = std::move(aref);
-            }
-            else {
+                }
+            } else {
                 need_copy = true;
             }
         }
 
         if (need_copy) {
             // We need to copy: If we need a mutable reference, or we're not supposed to convert
             // (either because we're in the no-convert overload pass, or because we're explicitly
             // instructed not to copy (via `py::arg().noconvert()`) we have to fail loading.
-            if (!convert || need_writeable) return false;
+            if (!convert || need_writeable) {
+                return false;
+            }
 
             Array copy = Array::ensure(src);
-            if (!copy) return false;
+            if (!copy) {
+                return false;
+            }
             fits = props::conformable(copy);
-            if (!fits || !fits.template stride_compatible<props>())
+            if (!fits || !fits.template stride_compatible<props>()) {
                 return false;
+            }
             copy_or_ref = std::move(copy);
             loader_life_support::add_patient(copy_or_ref);
         }
 
         ref.reset();
-        map.reset(new MapType(data(copy_or_ref), fits.rows, fits.cols, make_stride(fits.stride.outer(), fits.stride.inner())));
+        map.reset(new MapType(data(copy_or_ref),
+                              fits.rows,
+                              fits.cols,
+                              make_stride(fits.stride.outer(), fits.stride.inner())));
         ref.reset(new Type(*map));
 
         return true;
     }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator Type*() { return ref.get(); }
+    operator Type *() { return ref.get(); }
     // NOLINTNEXTLINE(google-explicit-constructor)
-    operator Type&() { return *ref; }
-    template <typename _T> using cast_op_type = pybind11::detail::cast_op_type<_T>;
+    operator Type &() { return *ref; }
+    template <typename _T>
+    using cast_op_type = pybind11::detail::cast_op_type<_T>;
 
 private:
     template <typename T = Type, enable_if_t<is_eigen_mutable_map<T>::value, int> = 0>
-    Scalar *data(Array &a) { return a.mutable_data(); }
+    Scalar *data(Array &a) {
+        return a.mutable_data();
+    }
 
     template <typename T = Type, enable_if_t<!is_eigen_mutable_map<T>::value, int> = 0>
-    const Scalar *data(Array &a) { return a.data(); }
+    const Scalar *data(Array &a) {
+        return a.data();
+    }
 
     // Attempt to figure out a constructor of `Stride` that will work.
     // If both strides are fixed, use a default constructor:
-    template <typename S> using stride_ctor_default = bool_constant<
-        S::InnerStrideAtCompileTime != Eigen::Dynamic && S::OuterStrideAtCompileTime != Eigen::Dynamic &&
-        std::is_default_constructible<S>::value>;
+    template <typename S>
+    using stride_ctor_default = bool_constant<S::InnerStrideAtCompileTime != Eigen::Dynamic
+                                              && S::OuterStrideAtCompileTime != Eigen::Dynamic
+                                              && std::is_default_constructible<S>::value>;
     // Otherwise, if there is a two-index constructor, assume it is (outer,inner) like
     // Eigen::Stride, and use it:
-    template <typename S> using stride_ctor_dual = bool_constant<
-        !stride_ctor_default<S>::value && std::is_constructible<S, EigenIndex, EigenIndex>::value>;
+    template <typename S>
+    using stride_ctor_dual
+        = bool_constant<!stride_ctor_default<S>::value
+                        && std::is_constructible<S, EigenIndex, EigenIndex>::value>;
     // Otherwise, if there is a one-index constructor, and just one of the strides is dynamic, use
     // it (passing whichever stride is dynamic).
-    template <typename S> using stride_ctor_outer = bool_constant<
-        !any_of<stride_ctor_default<S>, stride_ctor_dual<S>>::value &&
-        S::OuterStrideAtCompileTime == Eigen::Dynamic && S::InnerStrideAtCompileTime != Eigen::Dynamic &&
-        std::is_constructible<S, EigenIndex>::value>;
-    template <typename S> using stride_ctor_inner = bool_constant<
-        !any_of<stride_ctor_default<S>, stride_ctor_dual<S>>::value &&
-        S::InnerStrideAtCompileTime == Eigen::Dynamic && S::OuterStrideAtCompileTime != Eigen::Dynamic &&
-        std::is_constructible<S, EigenIndex>::value>;
+    template <typename S>
+    using stride_ctor_outer
+        = bool_constant<!any_of<stride_ctor_default<S>, stride_ctor_dual<S>>::value
+                        && S::OuterStrideAtCompileTime == Eigen::Dynamic
+                        && S::InnerStrideAtCompileTime != Eigen::Dynamic
+                        && std::is_constructible<S, EigenIndex>::value>;
+    template <typename S>
+    using stride_ctor_inner
+        = bool_constant<!any_of<stride_ctor_default<S>, stride_ctor_dual<S>>::value
+                        && S::InnerStrideAtCompileTime == Eigen::Dynamic
+                        && S::OuterStrideAtCompileTime != Eigen::Dynamic
+                        && std::is_constructible<S, EigenIndex>::value>;
 
     template <typename S = StrideType, enable_if_t<stride_ctor_default<S>::value, int> = 0>
-    static S make_stride(EigenIndex, EigenIndex) { return S(); }
+    static S make_stride(EigenIndex, EigenIndex) {
+        return S();
+    }
     template <typename S = StrideType, enable_if_t<stride_ctor_dual<S>::value, int> = 0>
-    static S make_stride(EigenIndex outer, EigenIndex inner) { return S(outer, inner); }
+    static S make_stride(EigenIndex outer, EigenIndex inner) {
+        return S(outer, inner);
+    }
     template <typename S = StrideType, enable_if_t<stride_ctor_outer<S>::value, int> = 0>
-    static S make_stride(EigenIndex outer, EigenIndex) { return S(outer); }
+    static S make_stride(EigenIndex outer, EigenIndex) {
+        return S(outer);
+    }
     template <typename S = StrideType, enable_if_t<stride_ctor_inner<S>::value, int> = 0>
-    static S make_stride(EigenIndex, EigenIndex inner) { return S(inner); }
-
+    static S make_stride(EigenIndex, EigenIndex inner) {
+        return S(inner);
+    }
 };
 
 // type_caster for special matrix types (e.g. DiagonalMatrix), which are EigenBase, but not
 // EigenDense (i.e. they don't have a data(), at least not with the usual matrix layout).
 // load() is not supported, but we can cast them into the python domain by first copying to a
 // regular Eigen::Matrix, then casting that.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_other<Type>::value>> {
 protected:
-    using Matrix = Eigen::Matrix<typename Type::Scalar, Type::RowsAtCompileTime, Type::ColsAtCompileTime>;
+    using Matrix
+        = Eigen::Matrix<typename Type::Scalar, Type::RowsAtCompileTime, Type::ColsAtCompileTime>;
     using props = EigenProps<Matrix>;
+
 public:
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
         handle h = eigen_encapsulate<props>(new Matrix(src));
         return h;
     }
-    static handle cast(const Type *src, return_value_policy policy, handle parent) { return cast(*src, policy, parent); }
+    static handle cast(const Type *src, return_value_policy policy, handle parent) {
+        return cast(*src, policy, parent);
+    }
 
     static constexpr auto name = props::descriptor;
 
     // Explicitly delete these: support python -> C++ conversion on these (i.e. these can be return
     // types but not bound arguments).  We still provide them (with an explicitly delete) so that
     // you end up here if you try anyway.
     bool load(handle, bool) = delete;
     operator Type() = delete;
-    template <typename> using cast_op_type = Type;
+    template <typename>
+    using cast_op_type = Type;
 };
 
-template<typename Type>
+template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_sparse<Type>::value>> {
     using Scalar = typename Type::Scalar;
     using StorageIndex = remove_reference_t<decltype(*std::declval<Type>().outerIndexPtr())>;
     using Index = typename Type::Index;
     static constexpr bool rowMajor = Type::IsRowMajor;
 
     bool load(handle src, bool) {
-        if (!src)
+        if (!src) {
             return false;
+        }
 
         auto obj = reinterpret_borrow<object>(src);
         object sparse_module = module_::import("scipy.sparse");
-        object matrix_type = sparse_module.attr(
-            rowMajor ? "csr_matrix" : "csc_matrix");
+        object matrix_type = sparse_module.attr(rowMajor ? "csr_matrix" : "csc_matrix");
 
         if (!type::handle_of(obj).is(matrix_type)) {
             try {
                 obj = matrix_type(obj);
             } catch (const error_already_set &) {
                 return false;
             }
@@ -568,41 +654,46 @@
 
         auto values = array_t<Scalar>((object) obj.attr("data"));
         auto innerIndices = array_t<StorageIndex>((object) obj.attr("indices"));
         auto outerIndices = array_t<StorageIndex>((object) obj.attr("indptr"));
         auto shape = pybind11::tuple((pybind11::object) obj.attr("shape"));
         auto nnz = obj.attr("nnz").cast<Index>();
 
-        if (!values || !innerIndices || !outerIndices)
+        if (!values || !innerIndices || !outerIndices) {
             return false;
+        }
 
         value = EigenMapSparseMatrix<Scalar,
-                                     Type::Flags & (Eigen::RowMajor | Eigen::ColMajor),
-                                     StorageIndex>(
-            shape[0].cast<Index>(), shape[1].cast<Index>(), nnz,
-            outerIndices.mutable_data(), innerIndices.mutable_data(), values.mutable_data());
+                                     Type::Flags &(Eigen::RowMajor | Eigen::ColMajor),
+                                     StorageIndex>(shape[0].cast<Index>(),
+                                                   shape[1].cast<Index>(),
+                                                   nnz,
+                                                   outerIndices.mutable_data(),
+                                                   innerIndices.mutable_data(),
+                                                   values.mutable_data());
 
         return true;
     }
 
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
-        const_cast<Type&>(src).makeCompressed();
+        const_cast<Type &>(src).makeCompressed();
 
-        object matrix_type = module_::import("scipy.sparse").attr(
-            rowMajor ? "csr_matrix" : "csc_matrix");
+        object matrix_type
+            = module_::import("scipy.sparse").attr(rowMajor ? "csr_matrix" : "csc_matrix");
 
         array data(src.nonZeros(), src.valuePtr());
         array outerIndices((rowMajor ? src.rows() : src.cols()) + 1, src.outerIndexPtr());
         array innerIndices(src.nonZeros(), src.innerIndexPtr());
 
-        return matrix_type(
-            std::make_tuple(data, innerIndices, outerIndices),
-            std::make_pair(src.rows(), src.cols())
-        ).release();
+        return matrix_type(std::make_tuple(data, innerIndices, outerIndices),
+                           std::make_pair(src.rows(), src.cols()))
+            .release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, const_name<(Type::IsRowMajor) != 0>("scipy.sparse.csr_matrix[", "scipy.sparse.csc_matrix[")
-            + npy_format_descriptor<Scalar>::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(Type,
+                         const_name<(Type::IsRowMajor) != 0>("scipy.sparse.csr_matrix[",
+                                                             "scipy.sparse.csc_matrix[")
+                             + npy_format_descriptor<Scalar>::name + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/embed.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/embed.h`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,25 @@
 #include "pybind11.h"
 #include "eval.h"
 
 #include <memory>
 #include <vector>
 
 #if defined(PYPY_VERSION)
-#  error Embedding the interpreter is not supported with PyPy
+#    error Embedding the interpreter is not supported with PyPy
 #endif
 
 #if PY_MAJOR_VERSION >= 3
-#  define PYBIND11_EMBEDDED_MODULE_IMPL(name)            \
-      extern "C" PyObject *pybind11_init_impl_##name();  \
-      extern "C" PyObject *pybind11_init_impl_##name() { \
-          return pybind11_init_wrapper_##name();         \
-      }
+#    define PYBIND11_EMBEDDED_MODULE_IMPL(name)                                                   \
+        extern "C" PyObject *pybind11_init_impl_##name();                                         \
+        extern "C" PyObject *pybind11_init_impl_##name() { return pybind11_init_wrapper_##name(); }
 #else
-#  define PYBIND11_EMBEDDED_MODULE_IMPL(name)            \
-      extern "C" void pybind11_init_impl_##name();       \
-      extern "C" void pybind11_init_impl_##name() {      \
-          pybind11_init_wrapper_##name();                \
-      }
+#    define PYBIND11_EMBEDDED_MODULE_IMPL(name)                                                   \
+        extern "C" void pybind11_init_impl_##name();                                              \
+        extern "C" void pybind11_init_impl_##name() { pybind11_init_wrapper_##name(); }
 #endif
 
 /** \rst
     Add a new module to the table of builtins for the interpreter. Must be
     defined in global scope. The first macro parameter is the name of the
     module (without quotes). The second parameter is the variable which will
     be used as the interface to add functions and classes to the module.
@@ -68,25 +64,27 @@
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Python 2.7/3.x compatible version of `PyImport_AppendInittab` and error checks.
 struct embedded_module {
 #if PY_MAJOR_VERSION >= 3
-    using init_t = PyObject *(*)();
+    using init_t = PyObject *(*) ();
 #else
     using init_t = void (*)();
 #endif
     embedded_module(const char *name, init_t init) {
-        if (Py_IsInitialized() != 0)
+        if (Py_IsInitialized() != 0) {
             pybind11_fail("Can't add new modules after the interpreter has been initialized");
+        }
 
         auto result = PyImport_AppendInittab(name, init);
-        if (result == -1)
+        if (result == -1) {
             pybind11_fail("Insufficient memory to add a new module");
+        }
     }
 };
 
 struct wide_char_arg_deleter {
     void operator()(wchar_t *ptr) const {
 #if PY_VERSION_HEX >= 0x030500f0
         // API docs: https://docs.python.org/3/c-api/sys.html#c.Py_DecodeLocale
@@ -100,47 +98,48 @@
 inline wchar_t *widen_chars(const char *safe_arg) {
 #if PY_VERSION_HEX >= 0x030500f0
     wchar_t *widened_arg = Py_DecodeLocale(safe_arg, nullptr);
 #else
     wchar_t *widened_arg = nullptr;
 
 // warning C4996: 'mbstowcs': This function or variable may be unsafe.
-#if defined(_MSC_VER)
-#pragma warning(push)
-#pragma warning(disable:4996)
-#endif
+#    if defined(_MSC_VER)
+#        pragma warning(push)
+#        pragma warning(disable : 4996)
+#    endif
 
 #    if defined(HAVE_BROKEN_MBSTOWCS) && HAVE_BROKEN_MBSTOWCS
     size_t count = std::strlen(safe_arg);
 #    else
     size_t count = std::mbstowcs(nullptr, safe_arg, 0);
 #    endif
     if (count != static_cast<size_t>(-1)) {
         widened_arg = new wchar_t[count + 1];
         std::mbstowcs(widened_arg, safe_arg, count + 1);
     }
 
-#if defined(_MSC_VER)
-#pragma warning(pop)
-#endif
+#    if defined(_MSC_VER)
+#        pragma warning(pop)
+#    endif
 
 #endif
     return widened_arg;
 }
 
 /// Python 2.x/3.x-compatible version of `PySys_SetArgv`
 inline void set_interpreter_argv(int argc, const char *const *argv, bool add_program_dir_to_path) {
     // Before it was special-cased in python 3.8, passing an empty or null argv
     // caused a segfault, so we have to reimplement the special case ourselves.
     bool special_case = (argv == nullptr || argc <= 0);
 
     const char *const empty_argv[]{"\0"};
     const char *const *safe_argv = special_case ? empty_argv : argv;
-    if (special_case)
+    if (special_case) {
         argc = 1;
+    }
 
     auto argv_size = static_cast<size_t>(argc);
 #if PY_MAJOR_VERSION >= 3
     // SetArgv* on python 3 takes wchar_t, so we have to convert.
     std::unique_ptr<wchar_t *[]> widened_argv(new wchar_t *[argv_size]);
     std::vector<std::unique_ptr<wchar_t[], wide_char_arg_deleter>> widened_argv_entries;
     widened_argv_entries.reserve(argv_size);
@@ -150,15 +149,15 @@
             // A null here indicates a character-encoding failure or the python
             // interpreter out of memory. Give up.
             return;
         }
         widened_argv[ii] = widened_argv_entries.back().get();
     }
 
-    auto pysys_argv = widened_argv.get();
+    auto *pysys_argv = widened_argv.get();
 #else
     // python 2.x
     std::vector<std::string> strings{safe_argv, safe_argv + argv_size};
     std::vector<char *> char_strings{argv_size};
     for (std::size_t i = 0; i < argv_size; ++i)
         char_strings[i] = &strings[i][0];
     char **pysys_argv = char_strings.data();
@@ -188,16 +187,17 @@
     .. |PySys_SetArgvEx documentation| replace:: ``PySys_SetArgvEx`` documentation
     .. _PySys_SetArgvEx documentation: https://docs.python.org/3/c-api/init.html#c.PySys_SetArgvEx
  \endrst */
 inline void initialize_interpreter(bool init_signal_handlers = true,
                                    int argc = 0,
                                    const char *const *argv = nullptr,
                                    bool add_program_dir_to_path = true) {
-    if (Py_IsInitialized() != 0)
+    if (Py_IsInitialized() != 0) {
         pybind11_fail("The interpreter is already running");
+    }
 
     Py_InitializeEx(init_signal_handlers ? 1 : 0);
 
     detail::set_interpreter_argv(argc, argv, add_program_dir_to_path);
 }
 
 /** \rst
@@ -240,16 +240,21 @@
     const char *id = PYBIND11_INTERNALS_ID;
 
     // Get the internals pointer (without creating it if it doesn't exist).  It's possible for the
     // internals to be created during Py_Finalize() (e.g. if a py::capsule calls `get_internals()`
     // during destruction), so we get the pointer-pointer here and check it after Py_Finalize().
     detail::internals **internals_ptr_ptr = detail::get_internals_pp();
     // It could also be stashed in builtins, so look there too:
-    if (builtins.contains(id) && isinstance<capsule>(builtins[id]))
+    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
         internals_ptr_ptr = capsule(builtins[id]);
+    }
+    // Local internals contains data managed by the current interpreter, so we must clear them to
+    // avoid undefined behaviors when initializing another interpreter
+    detail::get_local_internals().registered_types_cpp.clear();
+    detail::get_local_internals().registered_exception_translators.clear();
 
     Py_Finalize();
 
     if (internals_ptr_ptr) {
         delete *internals_ptr_ptr;
         *internals_ptr_ptr = nullptr;
     }
@@ -281,16 +286,17 @@
 
     scoped_interpreter(const scoped_interpreter &) = delete;
     scoped_interpreter(scoped_interpreter &&other) noexcept { other.is_valid = false; }
     scoped_interpreter &operator=(const scoped_interpreter &) = delete;
     scoped_interpreter &operator=(scoped_interpreter &&) = delete;
 
     ~scoped_interpreter() {
-        if (is_valid)
+        if (is_valid) {
             finalize_interpreter();
+        }
     }
 
 private:
     bool is_valid = true;
 };
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/eval.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/eval.h`

 * *Files 6% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#include <utility>
-
 #include "pybind11.h"
 
+#include <utility>
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 inline void ensure_builtins_in_globals(object &global) {
-    #if defined(PYPY_VERSION) || PY_VERSION_HEX < 0x03080000
-        // Running exec and eval on Python 2 and 3 adds `builtins` module under
-        // `__builtins__` key to globals if not yet present.
-        // Python 3.8 made PyRun_String behave similarly. Let's also do that for
-        // older versions, for consistency. This was missing from PyPy3.8 7.3.7.
-        if (!global.contains("__builtins__"))
-            global["__builtins__"] = module_::import(PYBIND11_BUILTINS_MODULE);
-    #else
-        (void) global;
-    #endif
+#if defined(PYPY_VERSION) || PY_VERSION_HEX < 0x03080000
+    // Running exec and eval on Python 2 and 3 adds `builtins` module under
+    // `__builtins__` key to globals if not yet present.
+    // Python 3.8 made PyRun_String behave similarly. Let's also do that for
+    // older versions, for consistency. This was missing from PyPy3.8 7.3.7.
+    if (!global.contains("__builtins__"))
+        global["__builtins__"] = module_::import(PYBIND11_BUILTINS_MODULE);
+#else
+    (void) global;
+#endif
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 enum eval_mode {
     /// Evaluate a string containing an isolated expression
     eval_expr,
@@ -42,52 +42,60 @@
 
     /// Evaluate a string containing a sequence of statement. Returns \c none
     eval_statements
 };
 
 template <eval_mode mode = eval_expr>
 object eval(const str &expr, object global = globals(), object local = object()) {
-    if (!local)
+    if (!local) {
         local = global;
+    }
 
     detail::ensure_builtins_in_globals(global);
 
     /* PyRun_String does not accept a PyObject / encoding specifier,
        this seems to be the only alternative */
     std::string buffer = "# -*- coding: utf-8 -*-\n" + (std::string) expr;
 
     int start = 0;
     switch (mode) {
-        case eval_expr:             start = Py_eval_input;   break;
-        case eval_single_statement: start = Py_single_input; break;
-        case eval_statements:       start = Py_file_input;   break;
-        default: pybind11_fail("invalid evaluation mode");
+        case eval_expr:
+            start = Py_eval_input;
+            break;
+        case eval_single_statement:
+            start = Py_single_input;
+            break;
+        case eval_statements:
+            start = Py_file_input;
+            break;
+        default:
+            pybind11_fail("invalid evaluation mode");
     }
 
     PyObject *result = PyRun_String(buffer.c_str(), start, global.ptr(), local.ptr());
-    if (!result)
+    if (!result) {
         throw error_already_set();
+    }
     return reinterpret_steal<object>(result);
 }
 
 template <eval_mode mode = eval_expr, size_t N>
 object eval(const char (&s)[N], object global = globals(), object local = object()) {
     /* Support raw string literals by removing common leading whitespace */
-    auto expr = (s[0] == '\n') ? str(module_::import("textwrap").attr("dedent")(s))
-                               : str(s);
-    return eval<mode>(expr, global, local);
+    auto expr = (s[0] == '\n') ? str(module_::import("textwrap").attr("dedent")(s)) : str(s);
+    return eval<mode>(expr, std::move(global), std::move(local));
 }
 
 inline void exec(const str &expr, object global = globals(), object local = object()) {
     eval<eval_statements>(expr, std::move(global), std::move(local));
 }
 
 template <size_t N>
 void exec(const char (&s)[N], object global = globals(), object local = object()) {
-    eval<eval_statements>(s, global, local);
+    eval<eval_statements>(s, std::move(global), std::move(local));
 }
 
 #if defined(PYPY_VERSION) && PY_VERSION_HEX >= 0x03000000
 template <eval_mode mode = eval_statements>
 object eval_file(str, object, object) {
     pybind11_fail("eval_file not supported in PyPy3. Use eval");
 }
@@ -98,66 +106,73 @@
 template <eval_mode mode = eval_statements>
 object eval_file(str) {
     pybind11_fail("eval_file not supported in PyPy3. Use eval");
 }
 #else
 template <eval_mode mode = eval_statements>
 object eval_file(str fname, object global = globals(), object local = object()) {
-    if (!local)
+    if (!local) {
         local = global;
+    }
 
     detail::ensure_builtins_in_globals(global);
 
     int start = 0;
     switch (mode) {
-        case eval_expr:             start = Py_eval_input;   break;
-        case eval_single_statement: start = Py_single_input; break;
-        case eval_statements:       start = Py_file_input;   break;
-        default: pybind11_fail("invalid evaluation mode");
+        case eval_expr:
+            start = Py_eval_input;
+            break;
+        case eval_single_statement:
+            start = Py_single_input;
+            break;
+        case eval_statements:
+            start = Py_file_input;
+            break;
+        default:
+            pybind11_fail("invalid evaluation mode");
     }
 
     int closeFile = 1;
     std::string fname_str = (std::string) fname;
-#if PY_VERSION_HEX >= 0x03040000
+#    if PY_VERSION_HEX >= 0x03040000
     FILE *f = _Py_fopen_obj(fname.ptr(), "r");
-#elif PY_VERSION_HEX >= 0x03000000
+#    elif PY_VERSION_HEX >= 0x03000000
     FILE *f = _Py_fopen(fname.ptr(), "r");
-#else
+#    else
     /* No unicode support in open() :( */
-    auto fobj = reinterpret_steal<object>(PyFile_FromString(
-        const_cast<char *>(fname_str.c_str()),
-        const_cast<char*>("r")));
+    auto fobj = reinterpret_steal<object>(
+        PyFile_FromString(const_cast<char *>(fname_str.c_str()), const_cast<char *>("r")));
     FILE *f = nullptr;
     if (fobj)
         f = PyFile_AsFile(fobj.ptr());
     closeFile = 0;
-#endif
+#    endif
     if (!f) {
         PyErr_Clear();
         pybind11_fail("File \"" + fname_str + "\" could not be opened!");
     }
 
     // In Python2, this should be encoded by getfilesystemencoding.
     // We don't boher setting it since Python2 is past EOL anyway.
     // See PR#3233
-#if PY_VERSION_HEX >= 0x03000000
+#    if PY_VERSION_HEX >= 0x03000000
     if (!global.contains("__file__")) {
         global["__file__"] = std::move(fname);
     }
-#endif
+#    endif
 
-#if PY_VERSION_HEX < 0x03000000 && defined(PYPY_VERSION)
-    PyObject *result = PyRun_File(f, fname_str.c_str(), start, global.ptr(),
-                                  local.ptr());
+#    if PY_VERSION_HEX < 0x03000000 && defined(PYPY_VERSION)
+    PyObject *result = PyRun_File(f, fname_str.c_str(), start, global.ptr(), local.ptr());
     (void) closeFile;
-#else
-    PyObject *result = PyRun_FileEx(f, fname_str.c_str(), start, global.ptr(),
-                                    local.ptr(), closeFile);
-#endif
+#    else
+    PyObject *result
+        = PyRun_FileEx(f, fname_str.c_str(), start, global.ptr(), local.ptr(), closeFile);
+#    endif
 
-    if (!result)
+    if (!result) {
         throw error_already_set();
+    }
     return reinterpret_steal<object>(result);
 }
 #endif
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/functional.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/functional.h`

 * *Files 3% similar despite different names*

```diff
@@ -6,51 +6,55 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+
 #include <functional>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename Return, typename... Args>
 struct type_caster<std::function<Return(Args...)>> {
     using type = std::function<Return(Args...)>;
     using retval_type = conditional_t<std::is_same<Return, void>::value, void_type, Return>;
-    using function_type = Return (*) (Args...);
+    using function_type = Return (*)(Args...);
 
 public:
     bool load(handle src, bool convert) {
         if (src.is_none()) {
             // Defer accepting None to other overloads (if we aren't in convert mode):
-            if (!convert) return false;
+            if (!convert) {
+                return false;
+            }
             return true;
         }
 
-        if (!isinstance<function>(src))
+        if (!isinstance<function>(src)) {
             return false;
+        }
 
         auto func = reinterpret_borrow<function>(src);
 
         /*
            When passing a C++ function as an argument to another C++
            function via Python, every function call would normally involve
            a full C++ -> Python -> C++ roundtrip, which can be prohibitive.
            Here, we try to at least detect the case where the function is
            stateless (i.e. function pointer or lambda function without
            captured variables), in which case the roundtrip can be avoided.
          */
         if (auto cfunc = func.cpp_function()) {
-            auto cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
+            auto *cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
             if (isinstance<capsule>(cfunc_self)) {
                 auto c = reinterpret_borrow<capsule>(cfunc_self);
-                auto rec = (function_record *) c;
+                auto *rec = (function_record *) c;
 
                 while (rec != nullptr) {
                     if (rec->is_stateless
                         && same_type(typeid(function_type),
                                      *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
                         struct capture {
                             function_type f;
@@ -69,15 +73,17 @@
         // ensure GIL is held during functor destruction
         struct func_handle {
             function f;
 #if !(defined(_MSC_VER) && _MSC_VER == 1916 && defined(PYBIND11_CPP17))
             // This triggers a syntax error under very special conditions (very weird indeed).
             explicit
 #endif
-            func_handle(function &&f_) noexcept : f(std::move(f_)) {}
+                func_handle(function &&f_) noexcept
+                : f(std::move(f_)) {
+            }
             func_handle(const func_handle &f_) { operator=(f_); }
             func_handle &operator=(const func_handle &f_) {
                 gil_scoped_acquire acq;
                 f = f_.f;
                 return *this;
             }
             ~func_handle() {
@@ -100,22 +106,26 @@
 
         value = func_wrapper(func_handle(std::move(func)));
         return true;
     }
 
     template <typename Func>
     static handle cast(Func &&f_, return_value_policy policy, handle /* parent */) {
-        if (!f_)
+        if (!f_) {
             return none().inc_ref();
+        }
 
         auto result = f_.template target<function_type>();
-        if (result)
+        if (result) {
             return cpp_function(*result, policy).release();
+        }
         return cpp_function(std::forward<Func>(f_), policy).release();
     }
 
-    PYBIND11_TYPE_CASTER(type, const_name("Callable[[") + concat(make_caster<Args>::name...) + const_name("], ")
-                               + make_caster<retval_type>::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(type,
+                         const_name("Callable[[") + concat(make_caster<Args>::name...)
+                             + const_name("], ") + make_caster<retval_type>::name
+                             + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/gil.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/gil.h`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 #pragma once
 
 #include "detail/common.h"
 #include "detail/internals.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
-
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // forward declarations
 PyThreadState *get_thread_state_unchecked();
 
 PYBIND11_NAMESPACE_END(detail)
 
-
 #if defined(WITH_THREAD) && !defined(PYPY_VERSION)
 
 /* The functions below essentially reproduce the PyGILState_* API using a RAII
  * pattern, but there are a few important differences:
  *
  * 1. When acquiring the GIL from an non-main thread during the finalization
  *    phase, the GILState API blindly terminates the calling thread, which
@@ -60,126 +58,137 @@
                below. Note we don't save this state with internals.tstate, since we don't
                create it we would fail to clear it (its reference count should be > 0). */
             tstate = PyGILState_GetThisThreadState();
         }
 
         if (!tstate) {
             tstate = PyThreadState_New(internals.istate);
-            #if !defined(NDEBUG)
-                if (!tstate)
-                    pybind11_fail("scoped_acquire: could not create thread state!");
-            #endif
+#    if !defined(NDEBUG)
+            if (!tstate) {
+                pybind11_fail("scoped_acquire: could not create thread state!");
+            }
+#    endif
             tstate->gilstate_counter = 0;
             PYBIND11_TLS_REPLACE_VALUE(internals.tstate, tstate);
         } else {
             release = detail::get_thread_state_unchecked() != tstate;
         }
 
         if (release) {
             PyEval_AcquireThread(tstate);
         }
 
         inc_ref();
     }
 
-    void inc_ref() {
-        ++tstate->gilstate_counter;
-    }
+    void inc_ref() { ++tstate->gilstate_counter; }
 
     PYBIND11_NOINLINE void dec_ref() {
         --tstate->gilstate_counter;
-        #if !defined(NDEBUG)
-            if (detail::get_thread_state_unchecked() != tstate)
-                pybind11_fail("scoped_acquire::dec_ref(): thread state must be current!");
-            if (tstate->gilstate_counter < 0)
-                pybind11_fail("scoped_acquire::dec_ref(): reference count underflow!");
-        #endif
+#    if !defined(NDEBUG)
+        if (detail::get_thread_state_unchecked() != tstate) {
+            pybind11_fail("scoped_acquire::dec_ref(): thread state must be current!");
+        }
+        if (tstate->gilstate_counter < 0) {
+            pybind11_fail("scoped_acquire::dec_ref(): reference count underflow!");
+        }
+#    endif
         if (tstate->gilstate_counter == 0) {
-            #if !defined(NDEBUG)
-                if (!release)
-                    pybind11_fail("scoped_acquire::dec_ref(): internal error!");
-            #endif
+#    if !defined(NDEBUG)
+            if (!release) {
+                pybind11_fail("scoped_acquire::dec_ref(): internal error!");
+            }
+#    endif
             PyThreadState_Clear(tstate);
-            if (active)
+            if (active) {
                 PyThreadState_DeleteCurrent();
+            }
             PYBIND11_TLS_DELETE_VALUE(detail::get_internals().tstate);
             release = false;
         }
     }
 
     /// This method will disable the PyThreadState_DeleteCurrent call and the
     /// GIL won't be acquired. This method should be used if the interpreter
     /// could be shutting down when this is called, as thread deletion is not
     /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
     /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
+    PYBIND11_NOINLINE void disarm() { active = false; }
 
     PYBIND11_NOINLINE ~gil_scoped_acquire() {
         dec_ref();
-        if (release)
-           PyEval_SaveThread();
+        if (release) {
+            PyEval_SaveThread();
+        }
     }
+
 private:
     PyThreadState *tstate = nullptr;
     bool release = true;
     bool active = true;
 };
 
 class gil_scoped_release {
 public:
     explicit gil_scoped_release(bool disassoc = false) : disassoc(disassoc) {
         // `get_internals()` must be called here unconditionally in order to initialize
         // `internals.tstate` for subsequent `gil_scoped_acquire` calls. Otherwise, an
         // initialization race could occur as multiple threads try `gil_scoped_acquire`.
         auto &internals = detail::get_internals();
+        // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         tstate = PyEval_SaveThread();
         if (disassoc) {
+            // Python >= 3.7 can remove this, it's an int before 3.7
+            // NOLINTNEXTLINE(readability-qualified-auto)
             auto key = internals.tstate;
             PYBIND11_TLS_DELETE_VALUE(key);
         }
     }
 
     /// This method will disable the PyThreadState_DeleteCurrent call and the
     /// GIL won't be acquired. This method should be used if the interpreter
     /// could be shutting down when this is called, as thread deletion is not
     /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
     /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
+    PYBIND11_NOINLINE void disarm() { active = false; }
 
     ~gil_scoped_release() {
-        if (!tstate)
+        if (!tstate) {
             return;
+        }
         // `PyEval_RestoreThread()` should not be called if runtime is finalizing
-        if (active)
+        if (active) {
             PyEval_RestoreThread(tstate);
+        }
         if (disassoc) {
+            // Python >= 3.7 can remove this, it's an int before 3.7
+            // NOLINTNEXTLINE(readability-qualified-auto)
             auto key = detail::get_internals().tstate;
             PYBIND11_TLS_REPLACE_VALUE(key, tstate);
         }
     }
+
 private:
     PyThreadState *tstate;
     bool disassoc;
     bool active = true;
 };
 #elif defined(PYPY_VERSION)
 class gil_scoped_acquire {
     PyGILState_STATE state;
+
 public:
     gil_scoped_acquire() { state = PyGILState_Ensure(); }
     ~gil_scoped_acquire() { PyGILState_Release(state); }
     void disarm() {}
 };
 
 class gil_scoped_release {
     PyThreadState *state;
+
 public:
     gil_scoped_release() { state = PyEval_SaveThread(); }
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
 #else
 class gil_scoped_acquire {
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/iostream.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/iostream.h`

 * *Files 3% similar despite different names*

```diff
@@ -54,96 +54,87 @@
 
     // Computes how many bytes at the end of the buffer are part of an
     // incomplete sequence of UTF-8 bytes.
     // Precondition: pbase() < pptr()
     size_t utf8_remainder() const {
         const auto rbase = std::reverse_iterator<char *>(pbase());
         const auto rpptr = std::reverse_iterator<char *>(pptr());
-        auto is_ascii = [](char c) {
-            return (static_cast<unsigned char>(c) & 0x80) == 0x00;
-        };
-        auto is_leading = [](char c) {
-            return (static_cast<unsigned char>(c) & 0xC0) == 0xC0;
-        };
-        auto is_leading_2b = [](char c) {
-            return static_cast<unsigned char>(c) <= 0xDF;
-        };
-        auto is_leading_3b = [](char c) {
-            return static_cast<unsigned char>(c) <= 0xEF;
-        };
+        auto is_ascii = [](char c) { return (static_cast<unsigned char>(c) & 0x80) == 0x00; };
+        auto is_leading = [](char c) { return (static_cast<unsigned char>(c) & 0xC0) == 0xC0; };
+        auto is_leading_2b = [](char c) { return static_cast<unsigned char>(c) <= 0xDF; };
+        auto is_leading_3b = [](char c) { return static_cast<unsigned char>(c) <= 0xEF; };
         // If the last character is ASCII, there are no incomplete code points
-        if (is_ascii(*rpptr))
+        if (is_ascii(*rpptr)) {
             return 0;
+        }
         // Otherwise, work back from the end of the buffer and find the first
         // UTF-8 leading byte
-        const auto rpend   = rbase - rpptr >= 3 ? rpptr + 3 : rbase;
+        const auto rpend = rbase - rpptr >= 3 ? rpptr + 3 : rbase;
         const auto leading = std::find_if(rpptr, rpend, is_leading);
-        if (leading == rbase)
+        if (leading == rbase) {
             return 0;
-        const auto dist    = static_cast<size_t>(leading - rpptr);
-        size_t remainder   = 0;
+        }
+        const auto dist = static_cast<size_t>(leading - rpptr);
+        size_t remainder = 0;
 
-        if (dist == 0)
+        if (dist == 0) {
             remainder = 1; // 1-byte code point is impossible
-        else if (dist == 1)
+        } else if (dist == 1) {
             remainder = is_leading_2b(*leading) ? 0 : dist + 1;
-        else if (dist == 2)
+        } else if (dist == 2) {
             remainder = is_leading_3b(*leading) ? 0 : dist + 1;
+        }
         // else if (dist >= 3), at least 4 bytes before encountering an UTF-8
         // leading byte, either no remainder or invalid UTF-8.
         // Invalid UTF-8 will cause an exception later when converting
         // to a Python string, so that's not handled here.
         return remainder;
     }
 
     // This function must be non-virtual to be called in a destructor.
     int _sync() {
         if (pbase() != pptr()) { // If buffer is not empty
             gil_scoped_acquire tmp;
             // This subtraction cannot be negative, so dropping the sign.
-            auto size        = static_cast<size_t>(pptr() - pbase());
+            auto size = static_cast<size_t>(pptr() - pbase());
             size_t remainder = utf8_remainder();
 
             if (size > remainder) {
                 str line(pbase(), size - remainder);
                 pywrite(line);
                 pyflush();
             }
 
             // Copy the remainder at the end of the buffer to the beginning:
-            if (remainder > 0)
+            if (remainder > 0) {
                 std::memmove(pbase(), pptr() - remainder, remainder);
+            }
             setp(pbase(), epptr());
             pbump(static_cast<int>(remainder));
         }
         return 0;
     }
 
-    int sync() override {
-        return _sync();
-    }
+    int sync() override { return _sync(); }
 
 public:
     explicit pythonbuf(const object &pyostream, size_t buffer_size = 1024)
         : buf_size(buffer_size), d_buffer(new char[buf_size]), pywrite(pyostream.attr("write")),
           pyflush(pyostream.attr("flush")) {
         setp(d_buffer.get(), d_buffer.get() + buf_size - 1);
     }
 
-    pythonbuf(pythonbuf&&) = default;
+    pythonbuf(pythonbuf &&) = default;
 
     /// Sync before destroy
-    ~pythonbuf() override {
-        _sync();
-    }
+    ~pythonbuf() override { _sync(); }
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
-
 /** \rst
     This a move-only guard that redirects output.
 
     .. code-block:: cpp
 
         #include <pybind11/iostream.h>
 
@@ -156,15 +147,16 @@
 
     You can explicitly pass the c++ stream and the python object,
     for example to guard stderr instead.
 
     .. code-block:: cpp
 
         {
-            py::scoped_ostream_redirect output{std::cerr, py::module::import("sys").attr("stderr")};
+            py::scoped_ostream_redirect output{
+                std::cerr, py::module::import("sys").attr("stderr")};
             std::cout << "Hello, World!";
         }
  \endrst */
 class scoped_ostream_redirect {
 protected:
     std::streambuf *old;
     std::ostream &costream;
@@ -174,25 +166,22 @@
     explicit scoped_ostream_redirect(std::ostream &costream = std::cout,
                                      const object &pyostream
                                      = module_::import("sys").attr("stdout"))
         : costream(costream), buffer(pyostream) {
         old = costream.rdbuf(&buffer);
     }
 
-    ~scoped_ostream_redirect() {
-        costream.rdbuf(old);
-    }
+    ~scoped_ostream_redirect() { costream.rdbuf(old); }
 
     scoped_ostream_redirect(const scoped_ostream_redirect &) = delete;
     scoped_ostream_redirect(scoped_ostream_redirect &&other) = default;
     scoped_ostream_redirect &operator=(const scoped_ostream_redirect &) = delete;
     scoped_ostream_redirect &operator=(scoped_ostream_redirect &&) = delete;
 };
 
-
 /** \rst
     Like `scoped_ostream_redirect`, but redirects cerr by default. This class
     is provided primary to make ``py::call_guard`` easier to make.
 
     .. code-block:: cpp
 
      m.def("noisy_func", &noisy_func,
@@ -204,33 +193,34 @@
 public:
     explicit scoped_estream_redirect(std::ostream &costream = std::cerr,
                                      const object &pyostream
                                      = module_::import("sys").attr("stderr"))
         : scoped_ostream_redirect(costream, pyostream) {}
 };
 
-
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Class to redirect output as a context manager. C++ backend.
 class OstreamRedirect {
     bool do_stdout_;
     bool do_stderr_;
     std::unique_ptr<scoped_ostream_redirect> redirect_stdout;
     std::unique_ptr<scoped_estream_redirect> redirect_stderr;
 
 public:
     explicit OstreamRedirect(bool do_stdout = true, bool do_stderr = true)
         : do_stdout_(do_stdout), do_stderr_(do_stderr) {}
 
     void enter() {
-        if (do_stdout_)
+        if (do_stdout_) {
             redirect_stdout.reset(new scoped_ostream_redirect());
-        if (do_stderr_)
+        }
+        if (do_stderr_) {
             redirect_stderr.reset(new scoped_estream_redirect());
+        }
     }
 
     void exit() {
         redirect_stdout.reset();
         redirect_stderr.reset();
     }
 };
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/numpy.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/numpy.h`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,28 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
 #include "complex.h"
-#include <numeric>
+
 #include <algorithm>
 #include <array>
 #include <cstdint>
 #include <cstdlib>
 #include <cstring>
+#include <functional>
+#include <numeric>
 #include <sstream>
 #include <string>
-#include <functional>
 #include <type_traits>
+#include <typeindex>
 #include <utility>
 #include <vector>
-#include <typeindex>
 
 /* This will be true on all flat address space platforms and allows us to reduce the
    whole npy_intp / ssize_t / Py_intptr_t business down to just ssize_t for all size
    and dimension types (e.g. shape, strides, indexing), instead of inflicting this
    upon the library user. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
@@ -35,17 +36,21 @@
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <> struct handle_type_name<array> { static constexpr auto name = const_name("numpy.ndarray"); };
+template <>
+struct handle_type_name<array> {
+    static constexpr auto name = const_name("numpy.ndarray");
+};
 
-template <typename type, typename SFINAE = void> struct npy_format_descriptor;
+template <typename type, typename SFINAE = void>
+struct npy_format_descriptor;
 
 struct PyArrayDescr_Proxy {
     PyObject_HEAD
     PyObject *typeobj;
     char kind;
     char type;
     char byteorder;
@@ -66,59 +71,67 @@
     ssize_t *strides;
     PyObject *base;
     PyObject *descr;
     int flags;
 };
 
 struct PyVoidScalarObject_Proxy {
-    PyObject_VAR_HEAD
-    char *obval;
+    PyObject_VAR_HEAD char *obval;
     PyArrayDescr_Proxy *descr;
     int flags;
     PyObject *base;
 };
 
 struct numpy_type_info {
-    PyObject* dtype_ptr;
+    PyObject *dtype_ptr;
     std::string format_str;
 };
 
 struct numpy_internals {
     std::unordered_map<std::type_index, numpy_type_info> registered_dtypes;
 
-    numpy_type_info *get_type_info(const std::type_info& tinfo, bool throw_if_missing = true) {
+    numpy_type_info *get_type_info(const std::type_info &tinfo, bool throw_if_missing = true) {
         auto it = registered_dtypes.find(std::type_index(tinfo));
-        if (it != registered_dtypes.end())
+        if (it != registered_dtypes.end()) {
             return &(it->second);
-        if (throw_if_missing)
+        }
+        if (throw_if_missing) {
             pybind11_fail(std::string("NumPy type info missing for ") + tinfo.name());
+        }
         return nullptr;
     }
 
-    template<typename T> numpy_type_info *get_type_info(bool throw_if_missing = true) {
+    template <typename T>
+    numpy_type_info *get_type_info(bool throw_if_missing = true) {
         return get_type_info(typeid(typename std::remove_cv<T>::type), throw_if_missing);
     }
 };
 
-PYBIND11_NOINLINE void load_numpy_internals(numpy_internals* &ptr) {
+PYBIND11_NOINLINE void load_numpy_internals(numpy_internals *&ptr) {
     ptr = &get_or_create_shared_data<numpy_internals>("_numpy_internals");
 }
 
-inline numpy_internals& get_numpy_internals() {
-    static numpy_internals* ptr = nullptr;
-    if (!ptr)
+inline numpy_internals &get_numpy_internals() {
+    static numpy_internals *ptr = nullptr;
+    if (!ptr) {
         load_numpy_internals(ptr);
+    }
     return *ptr;
 }
 
-template <typename T> struct same_size {
-    template <typename U> using as = bool_constant<sizeof(T) == sizeof(U)>;
+template <typename T>
+struct same_size {
+    template <typename U>
+    using as = bool_constant<sizeof(T) == sizeof(U)>;
 };
 
-template <typename Concrete> constexpr int platform_lookup() { return -1; }
+template <typename Concrete>
+constexpr int platform_lookup() {
+    return -1;
+}
 
 // Lookup a type according to its size, and return a value corresponding to the NumPy typenum.
 template <typename Concrete, typename T, typename... Ts, typename... Ints>
 constexpr int platform_lookup(int I, Ints... Is) {
     return sizeof(Concrete) == sizeof(T) ? I : platform_lookup<Concrete, Ts...>(Is...);
 }
 
@@ -128,82 +141,105 @@
         NPY_ARRAY_F_CONTIGUOUS_ = 0x0002,
         NPY_ARRAY_OWNDATA_ = 0x0004,
         NPY_ARRAY_FORCECAST_ = 0x0010,
         NPY_ARRAY_ENSUREARRAY_ = 0x0040,
         NPY_ARRAY_ALIGNED_ = 0x0100,
         NPY_ARRAY_WRITEABLE_ = 0x0400,
         NPY_BOOL_ = 0,
-        NPY_BYTE_, NPY_UBYTE_,
-        NPY_SHORT_, NPY_USHORT_,
-        NPY_INT_, NPY_UINT_,
-        NPY_LONG_, NPY_ULONG_,
-        NPY_LONGLONG_, NPY_ULONGLONG_,
-        NPY_FLOAT_, NPY_DOUBLE_, NPY_LONGDOUBLE_,
-        NPY_CFLOAT_, NPY_CDOUBLE_, NPY_CLONGDOUBLE_,
+        NPY_BYTE_,
+        NPY_UBYTE_,
+        NPY_SHORT_,
+        NPY_USHORT_,
+        NPY_INT_,
+        NPY_UINT_,
+        NPY_LONG_,
+        NPY_ULONG_,
+        NPY_LONGLONG_,
+        NPY_ULONGLONG_,
+        NPY_FLOAT_,
+        NPY_DOUBLE_,
+        NPY_LONGDOUBLE_,
+        NPY_CFLOAT_,
+        NPY_CDOUBLE_,
+        NPY_CLONGDOUBLE_,
         NPY_OBJECT_ = 17,
-        NPY_STRING_, NPY_UNICODE_, NPY_VOID_,
+        NPY_STRING_,
+        NPY_UNICODE_,
+        NPY_VOID_,
         // Platform-dependent normalization
         NPY_INT8_ = NPY_BYTE_,
         NPY_UINT8_ = NPY_UBYTE_,
         NPY_INT16_ = NPY_SHORT_,
         NPY_UINT16_ = NPY_USHORT_,
         // `npy_common.h` defines the integer aliases. In order, it checks:
         // NPY_BITSOF_LONG, NPY_BITSOF_LONGLONG, NPY_BITSOF_INT, NPY_BITSOF_SHORT, NPY_BITSOF_CHAR
         // and assigns the alias to the first matching size, so we should check in this order.
-        NPY_INT32_ = platform_lookup<std::int32_t, long, int, short>(
-            NPY_LONG_, NPY_INT_, NPY_SHORT_),
+        NPY_INT32_
+        = platform_lookup<std::int32_t, long, int, short>(NPY_LONG_, NPY_INT_, NPY_SHORT_),
         NPY_UINT32_ = platform_lookup<std::uint32_t, unsigned long, unsigned int, unsigned short>(
             NPY_ULONG_, NPY_UINT_, NPY_USHORT_),
-        NPY_INT64_ = platform_lookup<std::int64_t, long, long long, int>(
-            NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
-        NPY_UINT64_ = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
+        NPY_INT64_
+        = platform_lookup<std::int64_t, long, long long, int>(NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
+        NPY_UINT64_
+        = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
             NPY_ULONG_, NPY_ULONGLONG_, NPY_UINT_),
     };
 
     struct PyArray_Dims {
         Py_intptr_t *ptr;
         int len;
     };
 
-    static npy_api& get() {
+    static npy_api &get() {
         static npy_api api = lookup();
         return api;
     }
 
     bool PyArray_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArray_Type_) != 0;
     }
     bool PyArrayDescr_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArrayDescr_Type_) != 0;
     }
 
     unsigned int (*PyArray_GetNDArrayCFeatureVersion_)();
     PyObject *(*PyArray_DescrFromType_)(int);
-    PyObject *(*PyArray_NewFromDescr_)
-        (PyTypeObject *, PyObject *, int, Py_intptr_t const *,
-         Py_intptr_t const *, void *, int, PyObject *);
+    PyObject *(*PyArray_NewFromDescr_)(PyTypeObject *,
+                                       PyObject *,
+                                       int,
+                                       Py_intptr_t const *,
+                                       Py_intptr_t const *,
+                                       void *,
+                                       int,
+                                       PyObject *);
     // Unused. Not removed because that affects ABI of the class.
     PyObject *(*PyArray_DescrNewFromType_)(int);
     int (*PyArray_CopyInto_)(PyObject *, PyObject *);
     PyObject *(*PyArray_NewCopy_)(PyObject *, int);
     PyTypeObject *PyArray_Type_;
     PyTypeObject *PyVoidArrType_Type_;
     PyTypeObject *PyArrayDescr_Type_;
     PyObject *(*PyArray_DescrFromScalar_)(PyObject *);
-    PyObject *(*PyArray_FromAny_) (PyObject *, PyObject *, int, int, int, PyObject *);
-    int (*PyArray_DescrConverter_) (PyObject *, PyObject **);
-    bool (*PyArray_EquivTypes_) (PyObject *, PyObject *);
-    int (*PyArray_GetArrayParamsFromObject_)(PyObject *, PyObject *, unsigned char, PyObject **, int *,
-                                             Py_intptr_t *, PyObject **, PyObject *);
+    PyObject *(*PyArray_FromAny_)(PyObject *, PyObject *, int, int, int, PyObject *);
+    int (*PyArray_DescrConverter_)(PyObject *, PyObject **);
+    bool (*PyArray_EquivTypes_)(PyObject *, PyObject *);
+    int (*PyArray_GetArrayParamsFromObject_)(PyObject *,
+                                             PyObject *,
+                                             unsigned char,
+                                             PyObject **,
+                                             int *,
+                                             Py_intptr_t *,
+                                             PyObject **,
+                                             PyObject *);
     PyObject *(*PyArray_Squeeze_)(PyObject *);
     // Unused. Not removed because that affects ABI of the class.
     int (*PyArray_SetBaseObject_)(PyObject *, PyObject *);
-    PyObject* (*PyArray_Resize_)(PyObject*, PyArray_Dims*, int, int);
-    PyObject* (*PyArray_Newshape_)(PyObject*, PyArray_Dims*, int);
-    PyObject* (*PyArray_View_)(PyObject*, PyObject*, PyObject*);
+    PyObject *(*PyArray_Resize_)(PyObject *, PyArray_Dims *, int, int);
+    PyObject *(*PyArray_Newshape_)(PyObject *, PyArray_Dims *, int);
+    PyObject *(*PyArray_View_)(PyObject *, PyObject *, PyObject *);
 
 private:
     enum functions {
         API_PyArray_GetNDArrayCFeatureVersion = 211,
         API_PyArray_Type = 2,
         API_PyArrayDescr_Type = 3,
         API_PyVoidArrType_Type = 39,
@@ -231,16 +267,17 @@
         void **api_ptr = (void **) PyCapsule_GetPointer(c.ptr(), NULL);
 #else
         void **api_ptr = (void **) PyCObject_AsVoidPtr(c.ptr());
 #endif
         npy_api api;
 #define DECL_NPY_API(Func) api.Func##_ = (decltype(api.Func##_)) api_ptr[API_##Func];
         DECL_NPY_API(PyArray_GetNDArrayCFeatureVersion);
-        if (api.PyArray_GetNDArrayCFeatureVersion_() < 0x7)
+        if (api.PyArray_GetNDArrayCFeatureVersion_() < 0x7) {
             pybind11_fail("pybind11 numpy support requires numpy >= 1.7.0");
+        }
         DECL_NPY_API(PyArray_Type);
         DECL_NPY_API(PyVoidArrType_Type);
         DECL_NPY_API(PyArrayDescr_Type);
         DECL_NPY_API(PyArray_DescrFromType);
         DECL_NPY_API(PyArray_DescrFromScalar);
         DECL_NPY_API(PyArray_FromAny);
         DECL_NPY_API(PyArray_Resize);
@@ -257,211 +294,252 @@
         DECL_NPY_API(PyArray_SetBaseObject);
 
 #undef DECL_NPY_API
         return api;
     }
 };
 
-inline PyArray_Proxy* array_proxy(void* ptr) {
-    return reinterpret_cast<PyArray_Proxy*>(ptr);
-}
+inline PyArray_Proxy *array_proxy(void *ptr) { return reinterpret_cast<PyArray_Proxy *>(ptr); }
 
-inline const PyArray_Proxy* array_proxy(const void* ptr) {
-    return reinterpret_cast<const PyArray_Proxy*>(ptr);
+inline const PyArray_Proxy *array_proxy(const void *ptr) {
+    return reinterpret_cast<const PyArray_Proxy *>(ptr);
 }
 
-inline PyArrayDescr_Proxy* array_descriptor_proxy(PyObject* ptr) {
-   return reinterpret_cast<PyArrayDescr_Proxy*>(ptr);
+inline PyArrayDescr_Proxy *array_descriptor_proxy(PyObject *ptr) {
+    return reinterpret_cast<PyArrayDescr_Proxy *>(ptr);
 }
 
-inline const PyArrayDescr_Proxy* array_descriptor_proxy(const PyObject* ptr) {
-   return reinterpret_cast<const PyArrayDescr_Proxy*>(ptr);
+inline const PyArrayDescr_Proxy *array_descriptor_proxy(const PyObject *ptr) {
+    return reinterpret_cast<const PyArrayDescr_Proxy *>(ptr);
 }
 
-inline bool check_flags(const void* ptr, int flag) {
+inline bool check_flags(const void *ptr, int flag) {
     return (flag == (array_proxy(ptr)->flags & flag));
 }
 
-template <typename T> struct is_std_array : std::false_type { };
-template <typename T, size_t N> struct is_std_array<std::array<T, N>> : std::true_type { };
-template <typename T> struct is_complex : std::false_type { };
-template <typename T> struct is_complex<std::complex<T>> : std::true_type { };
+template <typename T>
+struct is_std_array : std::false_type {};
+template <typename T, size_t N>
+struct is_std_array<std::array<T, N>> : std::true_type {};
+template <typename T>
+struct is_complex : std::false_type {};
+template <typename T>
+struct is_complex<std::complex<T>> : std::true_type {};
 
-template <typename T> struct array_info_scalar {
+template <typename T>
+struct array_info_scalar {
     using type = T;
     static constexpr bool is_array = false;
     static constexpr bool is_empty = false;
     static constexpr auto extents = const_name("");
-    static void append_extents(list& /* shape */) { }
+    static void append_extents(list & /* shape */) {}
 };
 // Computes underlying type and a comma-separated list of extents for array
 // types (any mix of std::array and built-in arrays). An array of char is
 // treated as scalar because it gets special handling.
-template <typename T> struct array_info : array_info_scalar<T> { };
-template <typename T, size_t N> struct array_info<std::array<T, N>> {
+template <typename T>
+struct array_info : array_info_scalar<T> {};
+template <typename T, size_t N>
+struct array_info<std::array<T, N>> {
     using type = typename array_info<T>::type;
     static constexpr bool is_array = true;
     static constexpr bool is_empty = (N == 0) || array_info<T>::is_empty;
     static constexpr size_t extent = N;
 
     // appends the extents to shape
-    static void append_extents(list& shape) {
+    static void append_extents(list &shape) {
         shape.append(N);
         array_info<T>::append_extents(shape);
     }
 
     static constexpr auto extents = const_name<array_info<T>::is_array>(
-        concat(const_name<N>(), array_info<T>::extents), const_name<N>()
-    );
+        concat(const_name<N>(), array_info<T>::extents), const_name<N>());
 };
 // For numpy we have special handling for arrays of characters, so we don't include
 // the size in the array extents.
-template <size_t N> struct array_info<char[N]> : array_info_scalar<char[N]> { };
-template <size_t N> struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> { };
-template <typename T, size_t N> struct array_info<T[N]> : array_info<std::array<T, N>> { };
-template <typename T> using remove_all_extents_t = typename array_info<T>::type;
-
-template <typename T> using is_pod_struct = all_of<
-    std::is_standard_layout<T>,     // since we're accessing directly in memory we need a standard layout type
-#if defined(__GLIBCXX__) && (__GLIBCXX__ < 20150422 || __GLIBCXX__ == 20150426 || __GLIBCXX__ == 20150623 || __GLIBCXX__ == 20150626 || __GLIBCXX__ == 20160803)
-    // libstdc++ < 5 (including versions 4.8.5, 4.9.3 and 4.9.4 which were released after 5)
-    // don't implement is_trivially_copyable, so approximate it
-    std::is_trivially_destructible<T>,
-    satisfies_any_of<T, std::has_trivial_copy_constructor, std::has_trivial_copy_assign>,
+template <size_t N>
+struct array_info<char[N]> : array_info_scalar<char[N]> {};
+template <size_t N>
+struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> {};
+template <typename T, size_t N>
+struct array_info<T[N]> : array_info<std::array<T, N>> {};
+template <typename T>
+using remove_all_extents_t = typename array_info<T>::type;
+
+template <typename T>
+using is_pod_struct
+    = all_of<std::is_standard_layout<T>, // since we're accessing directly in memory
+                                         // we need a standard layout type
+#if defined(__GLIBCXX__)                                                                          \
+    && (__GLIBCXX__ < 20150422 || __GLIBCXX__ == 20150426 || __GLIBCXX__ == 20150623              \
+        || __GLIBCXX__ == 20150626 || __GLIBCXX__ == 20160803)
+             // libstdc++ < 5 (including versions 4.8.5, 4.9.3 and 4.9.4 which were released after
+             // 5) don't implement is_trivially_copyable, so approximate it
+             std::is_trivially_destructible<T>,
+             satisfies_any_of<T, std::has_trivial_copy_constructor, std::has_trivial_copy_assign>,
 #else
-    std::is_trivially_copyable<T>,
+             std::is_trivially_copyable<T>,
 #endif
-    satisfies_none_of<T, std::is_reference, std::is_array, is_std_array, std::is_arithmetic, is_complex, std::is_enum>
->;
+             satisfies_none_of<T,
+                               std::is_reference,
+                               std::is_array,
+                               is_std_array,
+                               std::is_arithmetic,
+                               is_complex,
+                               std::is_enum>>;
 
 // Replacement for std::is_pod (deprecated in C++20)
-template <typename T> using is_pod = all_of<
-    std::is_standard_layout<T>,
-    std::is_trivial<T>
->;
+template <typename T>
+using is_pod = all_of<std::is_standard_layout<T>, std::is_trivial<T>>;
 
-template <ssize_t Dim = 0, typename Strides> ssize_t byte_offset_unsafe(const Strides &) { return 0; }
+template <ssize_t Dim = 0, typename Strides>
+ssize_t byte_offset_unsafe(const Strides &) {
+    return 0;
+}
 template <ssize_t Dim = 0, typename Strides, typename... Ix>
 ssize_t byte_offset_unsafe(const Strides &strides, ssize_t i, Ix... index) {
     return i * strides[Dim] + byte_offset_unsafe<Dim + 1>(strides, index...);
 }
 
 /**
  * Proxy class providing unsafe, unchecked const access to array data.  This is constructed through
- * the `unchecked<T, N>()` method of `array` or the `unchecked<N>()` method of `array_t<T>`.  `Dims`
+ * the `unchecked<T, N>()` method of `array` or the `unchecked<N>()` method of `array_t<T>`. `Dims`
  * will be -1 for dimensions determined at runtime.
  */
 template <typename T, ssize_t Dims>
 class unchecked_reference {
 protected:
     static constexpr bool Dynamic = Dims < 0;
     const unsigned char *data_;
     // Storing the shape & strides in local variables (i.e. these arrays) allows the compiler to
     // make large performance gains on big, nested loops, but requires compile-time dimensions
-    conditional_t<Dynamic, const ssize_t *, std::array<ssize_t, (size_t) Dims>>
-            shape_, strides_;
+    conditional_t<Dynamic, const ssize_t *, std::array<ssize_t, (size_t) Dims>> shape_, strides_;
     const ssize_t dims_;
 
     friend class pybind11::array;
     // Constructor for compile-time dimensions:
     template <bool Dyn = Dynamic>
-    unchecked_reference(const void *data, const ssize_t *shape, const ssize_t *strides, enable_if_t<!Dyn, ssize_t>)
-    : data_{reinterpret_cast<const unsigned char *>(data)}, dims_{Dims} {
+    unchecked_reference(const void *data,
+                        const ssize_t *shape,
+                        const ssize_t *strides,
+                        enable_if_t<!Dyn, ssize_t>)
+        : data_{reinterpret_cast<const unsigned char *>(data)}, dims_{Dims} {
         for (size_t i = 0; i < (size_t) dims_; i++) {
             shape_[i] = shape[i];
             strides_[i] = strides[i];
         }
     }
     // Constructor for runtime dimensions:
     template <bool Dyn = Dynamic>
-    unchecked_reference(const void *data, const ssize_t *shape, const ssize_t *strides, enable_if_t<Dyn, ssize_t> dims)
-    : data_{reinterpret_cast<const unsigned char *>(data)}, shape_{shape}, strides_{strides}, dims_{dims} {}
+    unchecked_reference(const void *data,
+                        const ssize_t *shape,
+                        const ssize_t *strides,
+                        enable_if_t<Dyn, ssize_t> dims)
+        : data_{reinterpret_cast<const unsigned char *>(data)}, shape_{shape}, strides_{strides},
+          dims_{dims} {}
 
 public:
     /**
      * Unchecked const reference access to data at the given indices.  For a compile-time known
      * number of dimensions, this requires the correct number of arguments; for run-time
      * dimensionality, this is not checked (and so is up to the caller to use safely).
      */
-    template <typename... Ix> const T &operator()(Ix... index) const {
+    template <typename... Ix>
+    const T &operator()(Ix... index) const {
         static_assert(ssize_t{sizeof...(Ix)} == Dims || Dynamic,
-                "Invalid number of indices for unchecked array reference");
-        return *reinterpret_cast<const T *>(data_ + byte_offset_unsafe(strides_, ssize_t(index)...));
+                      "Invalid number of indices for unchecked array reference");
+        return *reinterpret_cast<const T *>(data_
+                                            + byte_offset_unsafe(strides_, ssize_t(index)...));
     }
     /**
      * Unchecked const reference access to data; this operator only participates if the reference
      * is to a 1-dimensional array.  When present, this is exactly equivalent to `obj(index)`.
      */
     template <ssize_t D = Dims, typename = enable_if_t<D == 1 || Dynamic>>
-    const T &operator[](ssize_t index) const { return operator()(index); }
+    const T &operator[](ssize_t index) const {
+        return operator()(index);
+    }
 
     /// Pointer access to the data at the given indices.
-    template <typename... Ix> const T *data(Ix... ix) const { return &operator()(ssize_t(ix)...); }
+    template <typename... Ix>
+    const T *data(Ix... ix) const {
+        return &operator()(ssize_t(ix)...);
+    }
 
     /// Returns the item size, i.e. sizeof(T)
     constexpr static ssize_t itemsize() { return sizeof(T); }
 
     /// Returns the shape (i.e. size) of dimension `dim`
     ssize_t shape(ssize_t dim) const { return shape_[(size_t) dim]; }
 
     /// Returns the number of dimensions of the array
     ssize_t ndim() const { return dims_; }
 
-    /// Returns the total number of elements in the referenced array, i.e. the product of the shapes
+    /// Returns the total number of elements in the referenced array, i.e. the product of the
+    /// shapes
     template <bool Dyn = Dynamic>
     enable_if_t<!Dyn, ssize_t> size() const {
-        return std::accumulate(shape_.begin(), shape_.end(), (ssize_t) 1, std::multiplies<ssize_t>());
+        return std::accumulate(
+            shape_.begin(), shape_.end(), (ssize_t) 1, std::multiplies<ssize_t>());
     }
     template <bool Dyn = Dynamic>
     enable_if_t<Dyn, ssize_t> size() const {
         return std::accumulate(shape_, shape_ + ndim(), (ssize_t) 1, std::multiplies<ssize_t>());
     }
 
-    /// Returns the total number of bytes used by the referenced data.  Note that the actual span in
-    /// memory may be larger if the referenced array has non-contiguous strides (e.g. for a slice).
-    ssize_t nbytes() const {
-        return size() * itemsize();
-    }
+    /// Returns the total number of bytes used by the referenced data.  Note that the actual span
+    /// in memory may be larger if the referenced array has non-contiguous strides (e.g. for a
+    /// slice).
+    ssize_t nbytes() const { return size() * itemsize(); }
 };
 
 template <typename T, ssize_t Dims>
 class unchecked_mutable_reference : public unchecked_reference<T, Dims> {
     friend class pybind11::array;
     using ConstBase = unchecked_reference<T, Dims>;
     using ConstBase::ConstBase;
     using ConstBase::Dynamic;
+
 public:
     // Bring in const-qualified versions from base class
     using ConstBase::operator();
     using ConstBase::operator[];
 
     /// Mutable, unchecked access to data at the given indices.
-    template <typename... Ix> T& operator()(Ix... index) {
+    template <typename... Ix>
+    T &operator()(Ix... index) {
         static_assert(ssize_t{sizeof...(Ix)} == Dims || Dynamic,
-                "Invalid number of indices for unchecked array reference");
+                      "Invalid number of indices for unchecked array reference");
         return const_cast<T &>(ConstBase::operator()(index...));
     }
     /**
      * Mutable, unchecked access data at the given index; this operator only participates if the
      * reference is to a 1-dimensional array (or has runtime dimensions).  When present, this is
      * exactly equivalent to `obj(index)`.
      */
     template <ssize_t D = Dims, typename = enable_if_t<D == 1 || Dynamic>>
-    T &operator[](ssize_t index) { return operator()(index); }
+    T &operator[](ssize_t index) {
+        return operator()(index);
+    }
 
     /// Mutable pointer access to the data at the given indices.
-    template <typename... Ix> T *mutable_data(Ix... ix) { return &operator()(ssize_t(ix)...); }
+    template <typename... Ix>
+    T *mutable_data(Ix... ix) {
+        return &operator()(ssize_t(ix)...);
+    }
 };
 
 template <typename T, ssize_t Dim>
 struct type_caster<unchecked_reference<T, Dim>> {
-    static_assert(Dim == 0 && Dim > 0 /* always fail */, "unchecked array proxy object is not castable");
+    static_assert(Dim == 0 && Dim > 0 /* always fail */,
+                  "unchecked array proxy object is not castable");
 };
 template <typename T, ssize_t Dim>
-struct type_caster<unchecked_mutable_reference<T, Dim>> : type_caster<unchecked_reference<T, Dim>> {};
+struct type_caster<unchecked_mutable_reference<T, Dim>>
+    : type_caster<unchecked_reference<T, Dim>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 class dtype : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(dtype, object, detail::npy_api::get().PyArrayDescr_Check_);
 
@@ -487,82 +565,89 @@
         args["itemsize"] = pybind11::int_(itemsize);
         m_ptr = from_args(std::move(args)).release().ptr();
     }
 
     /// This is essentially the same as calling numpy.dtype(args) in Python.
     static dtype from_args(object args) {
         PyObject *ptr = nullptr;
-        if ((detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) == 0) || !ptr)
+        if ((detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) == 0) || !ptr) {
             throw error_already_set();
+        }
         return reinterpret_steal<dtype>(ptr);
     }
 
     /// Return dtype associated with a C++ type.
-    template <typename T> static dtype of() {
+    template <typename T>
+    static dtype of() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::dtype();
     }
 
     /// Size of the data type in bytes.
-    ssize_t itemsize() const {
-        return detail::array_descriptor_proxy(m_ptr)->elsize;
-    }
+    ssize_t itemsize() const { return detail::array_descriptor_proxy(m_ptr)->elsize; }
 
     /// Returns true for structured data types.
-    bool has_fields() const {
-        return detail::array_descriptor_proxy(m_ptr)->names != nullptr;
-    }
+    bool has_fields() const { return detail::array_descriptor_proxy(m_ptr)->names != nullptr; }
 
     /// Single-character code for dtype's kind.
     /// For example, floating point types are 'f' and integral types are 'i'.
-    char kind() const {
-        return detail::array_descriptor_proxy(m_ptr)->kind;
-    }
+    char kind() const { return detail::array_descriptor_proxy(m_ptr)->kind; }
 
     /// Single-character for dtype's type.
     /// For example, ``float`` is 'f', ``double`` 'd', ``int`` 'i', and ``long`` 'l'.
     char char_() const {
         // Note: The signature, `dtype::char_` follows the naming of NumPy's
         // public Python API (i.e., ``dtype.char``), rather than its internal
         // C API (``PyArray_Descr::type``).
         return detail::array_descriptor_proxy(m_ptr)->type;
     }
 
 private:
     static object _dtype_from_pep3118() {
         static PyObject *obj = module_::import("numpy.core._internal")
-            .attr("_dtype_from_pep3118").cast<object>().release().ptr();
+                                   .attr("_dtype_from_pep3118")
+                                   .cast<object>()
+                                   .release()
+                                   .ptr();
         return reinterpret_borrow<object>(obj);
     }
 
     dtype strip_padding(ssize_t itemsize) {
         // Recursively strip all void fields with empty names that are generated for
         // padding fields (as of NumPy v1.11).
-        if (!has_fields())
+        if (!has_fields()) {
             return *this;
+        }
 
-        struct field_descr { PYBIND11_STR_TYPE name; object format; pybind11::int_ offset; };
+        struct field_descr {
+            PYBIND11_STR_TYPE name;
+            object format;
+            pybind11::int_ offset;
+        };
         std::vector<field_descr> field_descriptors;
 
         for (auto field : attr("fields").attr("items")()) {
             auto spec = field.cast<tuple>();
             auto name = spec[0].cast<pybind11::str>();
             auto format = spec[1].cast<tuple>()[0].cast<dtype>();
             auto offset = spec[1].cast<tuple>()[1].cast<pybind11::int_>();
-            if ((len(name) == 0u) && format.kind() == 'V')
+            if ((len(name) == 0u) && format.kind() == 'V') {
                 continue;
-            field_descriptors.push_back({(PYBIND11_STR_TYPE) name, format.strip_padding(format.itemsize()), offset});
+            }
+            field_descriptors.push_back(
+                {(PYBIND11_STR_TYPE) name, format.strip_padding(format.itemsize()), offset});
         }
 
-        std::sort(field_descriptors.begin(), field_descriptors.end(),
-                  [](const field_descr& a, const field_descr& b) {
+        std::sort(field_descriptors.begin(),
+                  field_descriptors.end(),
+                  [](const field_descr &a, const field_descr &b) {
                       return a.offset.cast<int>() < b.offset.cast<int>();
                   });
 
         list names, formats, offsets;
-        for (auto& descr : field_descriptors) {
+        for (auto &descr : field_descriptors) {
             names.append(descr.name);
             formats.append(descr.format);
             offsets.append(descr.offset);
         }
         return dtype(std::move(names), std::move(formats), std::move(offsets), itemsize);
     }
 };
@@ -579,74 +664,93 @@
 
     array() : array(0, static_cast<const double *>(nullptr)) {}
 
     using ShapeContainer = detail::any_container<ssize_t>;
     using StridesContainer = detail::any_container<ssize_t>;
 
     // Constructs an array taking shape/strides from arbitrary container types
-    array(const pybind11::dtype &dt, ShapeContainer shape, StridesContainer strides,
-          const void *ptr = nullptr, handle base = handle()) {
+    array(const pybind11::dtype &dt,
+          ShapeContainer shape,
+          StridesContainer strides,
+          const void *ptr = nullptr,
+          handle base = handle()) {
 
-        if (strides->empty())
+        if (strides->empty()) {
             *strides = detail::c_strides(*shape, dt.itemsize());
+        }
 
         auto ndim = shape->size();
-        if (ndim != strides->size())
+        if (ndim != strides->size()) {
             pybind11_fail("NumPy: shape ndim doesn't match strides ndim");
+        }
         auto descr = dt;
 
         int flags = 0;
         if (base && ptr) {
-            if (isinstance<array>(base))
+            if (isinstance<array>(base)) {
                 /* Copy flags from base (except ownership bit) */
-                flags = reinterpret_borrow<array>(base).flags() & ~detail::npy_api::NPY_ARRAY_OWNDATA_;
-            else
+                flags = reinterpret_borrow<array>(base).flags()
+                        & ~detail::npy_api::NPY_ARRAY_OWNDATA_;
+            } else {
                 /* Writable by default, easy to downgrade later on if needed */
                 flags = detail::npy_api::NPY_ARRAY_WRITEABLE_;
+            }
         }
 
         auto &api = detail::npy_api::get();
         auto tmp = reinterpret_steal<object>(api.PyArray_NewFromDescr_(
-            api.PyArray_Type_, descr.release().ptr(), (int) ndim,
+            api.PyArray_Type_,
+            descr.release().ptr(),
+            (int) ndim,
             // Use reinterpret_cast for PyPy on Windows (remove if fixed, checked on 7.3.1)
-            reinterpret_cast<Py_intptr_t*>(shape->data()),
-            reinterpret_cast<Py_intptr_t*>(strides->data()),
-            const_cast<void *>(ptr), flags, nullptr));
-        if (!tmp)
+            reinterpret_cast<Py_intptr_t *>(shape->data()),
+            reinterpret_cast<Py_intptr_t *>(strides->data()),
+            const_cast<void *>(ptr),
+            flags,
+            nullptr));
+        if (!tmp) {
             throw error_already_set();
+        }
         if (ptr) {
             if (base) {
                 api.PyArray_SetBaseObject_(tmp.ptr(), base.inc_ref().ptr());
             } else {
-                tmp = reinterpret_steal<object>(api.PyArray_NewCopy_(tmp.ptr(), -1 /* any order */));
+                tmp = reinterpret_steal<object>(
+                    api.PyArray_NewCopy_(tmp.ptr(), -1 /* any order */));
             }
         }
         m_ptr = tmp.release().ptr();
     }
 
-    array(const pybind11::dtype &dt, ShapeContainer shape, const void *ptr = nullptr, handle base = handle())
-        : array(dt, std::move(shape), {}, ptr, base) { }
+    array(const pybind11::dtype &dt,
+          ShapeContainer shape,
+          const void *ptr = nullptr,
+          handle base = handle())
+        : array(dt, std::move(shape), {}, ptr, base) {}
 
-    template <typename T, typename = detail::enable_if_t<std::is_integral<T>::value && !std::is_same<bool, T>::value>>
+    template <typename T,
+              typename
+              = detail::enable_if_t<std::is_integral<T>::value && !std::is_same<bool, T>::value>>
     array(const pybind11::dtype &dt, T count, const void *ptr = nullptr, handle base = handle())
-        : array(dt, {{count}}, ptr, base) { }
+        : array(dt, {{count}}, ptr, base) {}
 
     template <typename T>
     array(ShapeContainer shape, StridesContainer strides, const T *ptr, handle base = handle())
-        : array(pybind11::dtype::of<T>(), std::move(shape), std::move(strides), ptr, base) { }
+        : array(pybind11::dtype::of<T>(), std::move(shape), std::move(strides), ptr, base) {}
 
     template <typename T>
     array(ShapeContainer shape, const T *ptr, handle base = handle())
-        : array(std::move(shape), {}, ptr, base) { }
+        : array(std::move(shape), {}, ptr, base) {}
 
     template <typename T>
-    explicit array(ssize_t count, const T *ptr, handle base = handle()) : array({count}, {}, ptr, base) { }
+    explicit array(ssize_t count, const T *ptr, handle base = handle())
+        : array({count}, {}, ptr, base) {}
 
     explicit array(const buffer_info &info, handle base = handle())
-    : array(pybind11::dtype(info), info.shape, info.strides, info.ptr, base) { }
+        : array(pybind11::dtype(info), info.shape, info.strides, info.ptr, base) {}
 
     /// Array descriptor (dtype)
     pybind11::dtype dtype() const {
         return reinterpret_borrow<pybind11::dtype>(detail::array_proxy(m_ptr)->descr);
     }
 
     /// Total number of elements
@@ -656,145 +760,149 @@
 
     /// Byte size of a single element
     ssize_t itemsize() const {
         return detail::array_descriptor_proxy(detail::array_proxy(m_ptr)->descr)->elsize;
     }
 
     /// Total number of bytes
-    ssize_t nbytes() const {
-        return size() * itemsize();
-    }
+    ssize_t nbytes() const { return size() * itemsize(); }
 
     /// Number of dimensions
-    ssize_t ndim() const {
-        return detail::array_proxy(m_ptr)->nd;
-    }
+    ssize_t ndim() const { return detail::array_proxy(m_ptr)->nd; }
 
     /// Base object
-    object base() const {
-        return reinterpret_borrow<object>(detail::array_proxy(m_ptr)->base);
-    }
+    object base() const { return reinterpret_borrow<object>(detail::array_proxy(m_ptr)->base); }
 
     /// Dimensions of the array
-    const ssize_t* shape() const {
-        return detail::array_proxy(m_ptr)->dimensions;
-    }
+    const ssize_t *shape() const { return detail::array_proxy(m_ptr)->dimensions; }
 
     /// Dimension along a given axis
     ssize_t shape(ssize_t dim) const {
-        if (dim >= ndim())
+        if (dim >= ndim()) {
             fail_dim_check(dim, "invalid axis");
+        }
         return shape()[dim];
     }
 
     /// Strides of the array
-    const ssize_t* strides() const {
-        return detail::array_proxy(m_ptr)->strides;
-    }
+    const ssize_t *strides() const { return detail::array_proxy(m_ptr)->strides; }
 
     /// Stride along a given axis
     ssize_t strides(ssize_t dim) const {
-        if (dim >= ndim())
+        if (dim >= ndim()) {
             fail_dim_check(dim, "invalid axis");
+        }
         return strides()[dim];
     }
 
     /// Return the NumPy array flags
-    int flags() const {
-        return detail::array_proxy(m_ptr)->flags;
-    }
+    int flags() const { return detail::array_proxy(m_ptr)->flags; }
 
     /// If set, the array is writeable (otherwise the buffer is read-only)
     bool writeable() const {
         return detail::check_flags(m_ptr, detail::npy_api::NPY_ARRAY_WRITEABLE_);
     }
 
     /// If set, the array owns the data (will be freed when the array is deleted)
     bool owndata() const {
         return detail::check_flags(m_ptr, detail::npy_api::NPY_ARRAY_OWNDATA_);
     }
 
     /// Pointer to the contained data. If index is not provided, points to the
     /// beginning of the buffer. May throw if the index would lead to out of bounds access.
-    template<typename... Ix> const void* data(Ix... index) const {
+    template <typename... Ix>
+    const void *data(Ix... index) const {
         return static_cast<const void *>(detail::array_proxy(m_ptr)->data + offset_at(index...));
     }
 
     /// Mutable pointer to the contained data. If index is not provided, points to the
     /// beginning of the buffer. May throw if the index would lead to out of bounds access.
     /// May throw if the array is not writeable.
-    template<typename... Ix> void* mutable_data(Ix... index) {
+    template <typename... Ix>
+    void *mutable_data(Ix... index) {
         check_writeable();
         return static_cast<void *>(detail::array_proxy(m_ptr)->data + offset_at(index...));
     }
 
     /// Byte offset from beginning of the array to a given index (full or partial).
     /// May throw if the index would lead to out of bounds access.
-    template<typename... Ix> ssize_t offset_at(Ix... index) const {
-        if ((ssize_t) sizeof...(index) > ndim())
+    template <typename... Ix>
+    ssize_t offset_at(Ix... index) const {
+        if ((ssize_t) sizeof...(index) > ndim()) {
             fail_dim_check(sizeof...(index), "too many indices for an array");
+        }
         return byte_offset(ssize_t(index)...);
     }
 
     ssize_t offset_at() const { return 0; }
 
     /// Item count from beginning of the array to a given index (full or partial).
     /// May throw if the index would lead to out of bounds access.
-    template<typename... Ix> ssize_t index_at(Ix... index) const {
+    template <typename... Ix>
+    ssize_t index_at(Ix... index) const {
         return offset_at(index...) / itemsize();
     }
 
     /**
      * Returns a proxy object that provides access to the array's data without bounds or
      * dimensionality checking.  Will throw if the array is missing the `writeable` flag.  Use with
      * care: the array must not be destroyed or reshaped for the duration of the returned object,
      * and the caller must take care not to access invalid dimensions or dimension indices.
      */
-    template <typename T, ssize_t Dims = -1> detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims)
-            throw std::domain_error("array has incorrect number of dimensions: " + std::to_string(ndim()) +
-                    "; expected " + std::to_string(Dims));
-        return detail::unchecked_mutable_reference<T, Dims>(mutable_data(), shape(), strides(), ndim());
+    template <typename T, ssize_t Dims = -1>
+    detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
+        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+            throw std::domain_error("array has incorrect number of dimensions: "
+                                    + std::to_string(ndim()) + "; expected "
+                                    + std::to_string(Dims));
+        }
+        return detail::unchecked_mutable_reference<T, Dims>(
+            mutable_data(), shape(), strides(), ndim());
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
      * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
-     * underlying array have the `writable` flag.  Use with care: the array must not be destroyed or
-     * reshaped for the duration of the returned object, and the caller must take care not to access
-     * invalid dimensions or dimension indices.
+     * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
+     * or reshaped for the duration of the returned object, and the caller must take care not to
+     * access invalid dimensions or dimension indices.
      */
-    template <typename T, ssize_t Dims = -1> detail::unchecked_reference<T, Dims> unchecked() const & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims)
-            throw std::domain_error("array has incorrect number of dimensions: " + std::to_string(ndim()) +
-                    "; expected " + std::to_string(Dims));
+    template <typename T, ssize_t Dims = -1>
+    detail::unchecked_reference<T, Dims> unchecked() const & {
+        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+            throw std::domain_error("array has incorrect number of dimensions: "
+                                    + std::to_string(ndim()) + "; expected "
+                                    + std::to_string(Dims));
+        }
         return detail::unchecked_reference<T, Dims>(data(), shape(), strides(), ndim());
     }
 
     /// Return a new view with all of the dimensions of length 1 removed
     array squeeze() {
-        auto& api = detail::npy_api::get();
+        auto &api = detail::npy_api::get();
         return reinterpret_steal<array>(api.PyArray_Squeeze_(m_ptr));
     }
 
     /// Resize array to given shape
     /// If refcheck is true and more that one reference exist to this array
     /// then resize will succeed only if it makes a reshape, i.e. original size doesn't change
     void resize(ShapeContainer new_shape, bool refcheck = true) {
-        detail::npy_api::PyArray_Dims d = {
-            // Use reinterpret_cast for PyPy on Windows (remove if fixed, checked on 7.3.1)
-            reinterpret_cast<Py_intptr_t*>(new_shape->data()),
-            int(new_shape->size())
-        };
+        detail::npy_api::PyArray_Dims d
+            = {// Use reinterpret_cast for PyPy on Windows (remove if fixed, checked on 7.3.1)
+               reinterpret_cast<Py_intptr_t *>(new_shape->data()),
+               int(new_shape->size())};
         // try to resize, set ordering param to -1 cause it's not used anyway
         auto new_array = reinterpret_steal<object>(
-            detail::npy_api::get().PyArray_Resize_(m_ptr, &d, int(refcheck), -1)
-        );
-        if (!new_array) throw error_already_set();
-        if (isinstance<array>(new_array)) { *this = std::move(new_array); }
+            detail::npy_api::get().PyArray_Resize_(m_ptr, &d, int(refcheck), -1));
+        if (!new_array) {
+            throw error_already_set();
+        }
+        if (isinstance<array>(new_array)) {
+            *this = std::move(new_array);
+        }
     }
 
     /// Optional `order` parameter omitted, to be added as needed.
     array reshape(ShapeContainer new_shape) {
         detail::npy_api::PyArray_Dims d
             = {reinterpret_cast<Py_intptr_t *>(new_shape->data()), int(new_shape->size())};
         auto new_array
@@ -820,48 +928,54 @@
         return new_view;
     }
 
     /// Ensure that the argument is a NumPy array
     /// In case of an error, nullptr is returned and the Python error is cleared.
     static array ensure(handle h, int ExtraFlags = 0) {
         auto result = reinterpret_steal<array>(raw_array(h.ptr(), ExtraFlags));
-        if (!result)
+        if (!result) {
             PyErr_Clear();
+        }
         return result;
     }
 
 protected:
-    template<typename, typename> friend struct detail::npy_format_descriptor;
+    template <typename, typename>
+    friend struct detail::npy_format_descriptor;
 
-    void fail_dim_check(ssize_t dim, const std::string& msg) const {
-        throw index_error(msg + ": " + std::to_string(dim) +
-                          " (ndim = " + std::to_string(ndim()) + ")");
+    void fail_dim_check(ssize_t dim, const std::string &msg) const {
+        throw index_error(msg + ": " + std::to_string(dim) + " (ndim = " + std::to_string(ndim())
+                          + ")");
     }
 
-    template<typename... Ix> ssize_t byte_offset(Ix... index) const {
+    template <typename... Ix>
+    ssize_t byte_offset(Ix... index) const {
         check_dimensions(index...);
         return detail::byte_offset_unsafe(strides(), ssize_t(index)...);
     }
 
     void check_writeable() const {
-        if (!writeable())
+        if (!writeable()) {
             throw std::domain_error("array is not writeable");
+        }
     }
 
-    template<typename... Ix> void check_dimensions(Ix... index) const {
+    template <typename... Ix>
+    void check_dimensions(Ix... index) const {
         check_dimensions_impl(ssize_t(0), shape(), ssize_t(index)...);
     }
 
-    void check_dimensions_impl(ssize_t, const ssize_t*) const { }
+    void check_dimensions_impl(ssize_t, const ssize_t *) const {}
 
-    template<typename... Ix> void check_dimensions_impl(ssize_t axis, const ssize_t* shape, ssize_t i, Ix... index) const {
+    template <typename... Ix>
+    void check_dimensions_impl(ssize_t axis, const ssize_t *shape, ssize_t i, Ix... index) const {
         if (i >= *shape) {
-            throw index_error(std::string("index ") + std::to_string(i) +
-                              " is out of bounds for axis " + std::to_string(axis) +
-                              " with size " + std::to_string(*shape));
+            throw index_error(std::string("index ") + std::to_string(i)
+                              + " is out of bounds for axis " + std::to_string(axis)
+                              + " with size " + std::to_string(*shape));
         }
         check_dimensions_impl(axis + 1, shape + 1, index...);
     }
 
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array(PyObject *ptr, int ExtraFlags = 0) {
         if (ptr == nullptr) {
@@ -869,147 +983,179 @@
             return nullptr;
         }
         return detail::npy_api::get().PyArray_FromAny_(
             ptr, nullptr, 0, 0, detail::npy_api::NPY_ARRAY_ENSUREARRAY_ | ExtraFlags, nullptr);
     }
 };
 
-template <typename T, int ExtraFlags = array::forcecast> class array_t : public array {
+template <typename T, int ExtraFlags = array::forcecast>
+class array_t : public array {
 private:
     struct private_ctor {};
     // Delegating constructor needed when both moving and accessing in the same constructor
-    array_t(private_ctor, ShapeContainer &&shape, StridesContainer &&strides, const T *ptr, handle base)
+    array_t(private_ctor,
+            ShapeContainer &&shape,
+            StridesContainer &&strides,
+            const T *ptr,
+            handle base)
         : array(std::move(shape), std::move(strides), ptr, base) {}
+
 public:
     static_assert(!detail::array_info<T>::is_array, "Array types cannot be used with array_t");
 
     using value_type = T;
 
     array_t() : array(0, static_cast<const T *>(nullptr)) {}
-    array_t(handle h, borrowed_t) : array(h, borrowed_t{}) { }
-    array_t(handle h, stolen_t) : array(h, stolen_t{}) { }
+    array_t(handle h, borrowed_t) : array(h, borrowed_t{}) {}
+    array_t(handle h, stolen_t) : array(h, stolen_t{}) {}
 
     PYBIND11_DEPRECATED("Use array_t<T>::ensure() instead")
     array_t(handle h, bool is_borrowed) : array(raw_array_t(h.ptr()), stolen_t{}) {
-        if (!m_ptr) PyErr_Clear();
-        if (!is_borrowed) Py_XDECREF(h.ptr());
+        if (!m_ptr) {
+            PyErr_Clear();
+        }
+        if (!is_borrowed) {
+            Py_XDECREF(h.ptr());
+        }
     }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     array_t(const object &o) : array(raw_array_t(o.ptr()), stolen_t{}) {
-        if (!m_ptr) throw error_already_set();
+        if (!m_ptr) {
+            throw error_already_set();
+        }
     }
 
-    explicit array_t(const buffer_info& info, handle base = handle()) : array(info, base) { }
+    explicit array_t(const buffer_info &info, handle base = handle()) : array(info, base) {}
 
-    array_t(ShapeContainer shape, StridesContainer strides, const T *ptr = nullptr, handle base = handle())
-        : array(std::move(shape), std::move(strides), ptr, base) { }
+    array_t(ShapeContainer shape,
+            StridesContainer strides,
+            const T *ptr = nullptr,
+            handle base = handle())
+        : array(std::move(shape), std::move(strides), ptr, base) {}
 
     explicit array_t(ShapeContainer shape, const T *ptr = nullptr, handle base = handle())
         : array_t(private_ctor{},
                   std::move(shape),
                   (ExtraFlags & f_style) != 0 ? detail::f_strides(*shape, itemsize())
                                               : detail::c_strides(*shape, itemsize()),
                   ptr,
                   base) {}
 
     explicit array_t(ssize_t count, const T *ptr = nullptr, handle base = handle())
-        : array({count}, {}, ptr, base) { }
+        : array({count}, {}, ptr, base) {}
 
-    constexpr ssize_t itemsize() const {
-        return sizeof(T);
-    }
+    constexpr ssize_t itemsize() const { return sizeof(T); }
 
-    template<typename... Ix> ssize_t index_at(Ix... index) const {
+    template <typename... Ix>
+    ssize_t index_at(Ix... index) const {
         return offset_at(index...) / itemsize();
     }
 
-    template<typename... Ix> const T* data(Ix... index) const {
-        return static_cast<const T*>(array::data(index...));
+    template <typename... Ix>
+    const T *data(Ix... index) const {
+        return static_cast<const T *>(array::data(index...));
     }
 
-    template<typename... Ix> T* mutable_data(Ix... index) {
-        return static_cast<T*>(array::mutable_data(index...));
+    template <typename... Ix>
+    T *mutable_data(Ix... index) {
+        return static_cast<T *>(array::mutable_data(index...));
     }
 
     // Reference to element at a given index
-    template<typename... Ix> const T& at(Ix... index) const {
-        if ((ssize_t) sizeof...(index) != ndim())
+    template <typename... Ix>
+    const T &at(Ix... index) const {
+        if ((ssize_t) sizeof...(index) != ndim()) {
             fail_dim_check(sizeof...(index), "index dimension mismatch");
-        return *(static_cast<const T*>(array::data()) + byte_offset(ssize_t(index)...) / itemsize());
+        }
+        return *(static_cast<const T *>(array::data())
+                 + byte_offset(ssize_t(index)...) / itemsize());
     }
 
     // Mutable reference to element at a given index
-    template<typename... Ix> T& mutable_at(Ix... index) {
-        if ((ssize_t) sizeof...(index) != ndim())
+    template <typename... Ix>
+    T &mutable_at(Ix... index) {
+        if ((ssize_t) sizeof...(index) != ndim()) {
             fail_dim_check(sizeof...(index), "index dimension mismatch");
-        return *(static_cast<T*>(array::mutable_data()) + byte_offset(ssize_t(index)...) / itemsize());
+        }
+        return *(static_cast<T *>(array::mutable_data())
+                 + byte_offset(ssize_t(index)...) / itemsize());
     }
 
     /**
      * Returns a proxy object that provides access to the array's data without bounds or
      * dimensionality checking.  Will throw if the array is missing the `writeable` flag.  Use with
      * care: the array must not be destroyed or reshaped for the duration of the returned object,
      * and the caller must take care not to access invalid dimensions or dimension indices.
      */
-    template <ssize_t Dims = -1> detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
+    template <ssize_t Dims = -1>
+    detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
         return array::mutable_unchecked<T, Dims>();
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
      * dimensionality checking.  Unlike `unchecked()`, this does not require that the underlying
      * array have the `writable` flag.  Use with care: the array must not be destroyed or reshaped
      * for the duration of the returned object, and the caller must take care not to access invalid
      * dimensions or dimension indices.
      */
-    template <ssize_t Dims = -1> detail::unchecked_reference<T, Dims> unchecked() const & {
+    template <ssize_t Dims = -1>
+    detail::unchecked_reference<T, Dims> unchecked() const & {
         return array::unchecked<T, Dims>();
     }
 
     /// Ensure that the argument is a NumPy array of the correct dtype (and if not, try to convert
     /// it).  In case of an error, nullptr is returned and the Python error is cleared.
     static array_t ensure(handle h) {
         auto result = reinterpret_steal<array_t>(raw_array_t(h.ptr()));
-        if (!result)
+        if (!result) {
             PyErr_Clear();
+        }
         return result;
     }
 
     static bool check_(handle h) {
         const auto &api = detail::npy_api::get();
         return api.PyArray_Check_(h.ptr())
-               && api.PyArray_EquivTypes_(detail::array_proxy(h.ptr())->descr, dtype::of<T>().ptr())
+               && api.PyArray_EquivTypes_(detail::array_proxy(h.ptr())->descr,
+                                          dtype::of<T>().ptr())
                && detail::check_flags(h.ptr(), ExtraFlags & (array::c_style | array::f_style));
     }
 
 protected:
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array_t(PyObject *ptr) {
         if (ptr == nullptr) {
             PyErr_SetString(PyExc_ValueError, "cannot create a pybind11::array_t from a nullptr");
             return nullptr;
         }
-        return detail::npy_api::get().PyArray_FromAny_(
-            ptr, dtype::of<T>().release().ptr(), 0, 0,
-            detail::npy_api::NPY_ARRAY_ENSUREARRAY_ | ExtraFlags, nullptr);
+        return detail::npy_api::get().PyArray_FromAny_(ptr,
+                                                       dtype::of<T>().release().ptr(),
+                                                       0,
+                                                       0,
+                                                       detail::npy_api::NPY_ARRAY_ENSUREARRAY_
+                                                           | ExtraFlags,
+                                                       nullptr);
     }
 };
 
 template <typename T>
 struct format_descriptor<T, detail::enable_if_t<detail::is_pod_struct<T>::value>> {
     static std::string format() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::format();
     }
 };
 
-template <size_t N> struct format_descriptor<char[N]> {
+template <size_t N>
+struct format_descriptor<char[N]> {
     static std::string format() { return std::to_string(N) + "s"; }
 };
-template <size_t N> struct format_descriptor<std::array<char, N>> {
+template <size_t N>
+struct format_descriptor<std::array<char, N>> {
     static std::string format() { return std::to_string(N) + "s"; }
 };
 
 template <typename T>
 struct format_descriptor<T, detail::enable_if_t<std::is_enum<T>::value>> {
     static std::string format() {
         return format_descriptor<
@@ -1028,148 +1174,179 @@
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 template <typename T, int ExtraFlags>
 struct pyobject_caster<array_t<T, ExtraFlags>> {
     using type = array_t<T, ExtraFlags>;
 
     bool load(handle src, bool convert) {
-        if (!convert && !type::check_(src))
+        if (!convert && !type::check_(src)) {
             return false;
+        }
         value = type::ensure(src);
         return static_cast<bool>(value);
     }
 
     static handle cast(const handle &src, return_value_policy /* policy */, handle /* parent */) {
         return src.inc_ref();
     }
     PYBIND11_TYPE_CASTER(type, handle_type_name<type>::name);
 };
 
 template <typename T>
 struct compare_buffer_info<T, detail::enable_if_t<detail::is_pod_struct<T>::value>> {
-    static bool compare(const buffer_info& b) {
+    static bool compare(const buffer_info &b) {
         return npy_api::get().PyArray_EquivTypes_(dtype::of<T>().ptr(), dtype(b).ptr());
     }
 };
 
 template <typename T, typename = void>
 struct npy_format_descriptor_name;
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<std::is_integral<T>::value>> {
     static constexpr auto name = const_name<std::is_same<T, bool>::value>(
-        const_name("bool"), const_name<std::is_signed<T>::value>("numpy.int", "numpy.uint") + const_name<sizeof(T)*8>()
-    );
+        const_name("bool"),
+        const_name<std::is_signed<T>::value>("numpy.int", "numpy.uint")
+            + const_name<sizeof(T) * 8>());
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<std::is_floating_point<T>::value>> {
-    static constexpr auto name = const_name<std::is_same<T, float>::value
-                                   || std::is_same<T, const float>::value
-                                   || std::is_same<T, double>::value
-                                   || std::is_same<T, const double>::value>(
-        const_name("numpy.float") + const_name<sizeof(T)*8>(), const_name("numpy.longdouble")
-    );
+    static constexpr auto name = const_name < std::is_same<T, float>::value
+                                 || std::is_same<T, const float>::value
+                                 || std::is_same<T, double>::value
+                                 || std::is_same<T, const double>::value
+                                        > (const_name("numpy.float") + const_name<sizeof(T) * 8>(),
+                                           const_name("numpy.longdouble"));
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<is_complex<T>::value>> {
-    static constexpr auto name = const_name<std::is_same<typename T::value_type, float>::value
-                                   || std::is_same<typename T::value_type, const float>::value
-                                   || std::is_same<typename T::value_type, double>::value
-                                   || std::is_same<typename T::value_type, const double>::value>(
-        const_name("numpy.complex") + const_name<sizeof(typename T::value_type)*16>(), const_name("numpy.longcomplex")
-    );
+    static constexpr auto name = const_name < std::is_same<typename T::value_type, float>::value
+                                 || std::is_same<typename T::value_type, const float>::value
+                                 || std::is_same<typename T::value_type, double>::value
+                                 || std::is_same<typename T::value_type, const double>::value
+                                        > (const_name("numpy.complex")
+                                               + const_name<sizeof(typename T::value_type) * 16>(),
+                                           const_name("numpy.longcomplex"));
 };
 
 template <typename T>
-struct npy_format_descriptor<T, enable_if_t<satisfies_any_of<T, std::is_arithmetic, is_complex>::value>>
+struct npy_format_descriptor<
+    T,
+    enable_if_t<satisfies_any_of<T, std::is_arithmetic, is_complex>::value>>
     : npy_format_descriptor_name<T> {
 private:
     // NB: the order here must match the one in common.h
-    constexpr static const int values[15] = {
-        npy_api::NPY_BOOL_,
-        npy_api::NPY_BYTE_,   npy_api::NPY_UBYTE_,   npy_api::NPY_INT16_,    npy_api::NPY_UINT16_,
-        npy_api::NPY_INT32_,  npy_api::NPY_UINT32_,  npy_api::NPY_INT64_,    npy_api::NPY_UINT64_,
-        npy_api::NPY_FLOAT_,  npy_api::NPY_DOUBLE_,  npy_api::NPY_LONGDOUBLE_,
-        npy_api::NPY_CFLOAT_, npy_api::NPY_CDOUBLE_, npy_api::NPY_CLONGDOUBLE_
-    };
+    constexpr static const int values[15] = {npy_api::NPY_BOOL_,
+                                             npy_api::NPY_BYTE_,
+                                             npy_api::NPY_UBYTE_,
+                                             npy_api::NPY_INT16_,
+                                             npy_api::NPY_UINT16_,
+                                             npy_api::NPY_INT32_,
+                                             npy_api::NPY_UINT32_,
+                                             npy_api::NPY_INT64_,
+                                             npy_api::NPY_UINT64_,
+                                             npy_api::NPY_FLOAT_,
+                                             npy_api::NPY_DOUBLE_,
+                                             npy_api::NPY_LONGDOUBLE_,
+                                             npy_api::NPY_CFLOAT_,
+                                             npy_api::NPY_CDOUBLE_,
+                                             npy_api::NPY_CLONGDOUBLE_};
 
 public:
     static constexpr int value = values[detail::is_fmt_numeric<T>::index];
 
     static pybind11::dtype dtype() {
-        if (auto ptr = npy_api::get().PyArray_DescrFromType_(value))
+        if (auto *ptr = npy_api::get().PyArray_DescrFromType_(value)) {
             return reinterpret_steal<pybind11::dtype>(ptr);
+        }
         pybind11_fail("Unsupported buffer format!");
     }
 };
 
-#define PYBIND11_DECL_CHAR_FMT \
-    static constexpr auto name = const_name("S") + const_name<N>(); \
-    static pybind11::dtype dtype() { return pybind11::dtype(std::string("S") + std::to_string(N)); }
-template <size_t N> struct npy_format_descriptor<char[N]> { PYBIND11_DECL_CHAR_FMT };
-template <size_t N> struct npy_format_descriptor<std::array<char, N>> { PYBIND11_DECL_CHAR_FMT };
+#define PYBIND11_DECL_CHAR_FMT                                                                    \
+    static constexpr auto name = const_name("S") + const_name<N>();                               \
+    static pybind11::dtype dtype() {                                                              \
+        return pybind11::dtype(std::string("S") + std::to_string(N));                             \
+    }
+template <size_t N>
+struct npy_format_descriptor<char[N]> {
+    PYBIND11_DECL_CHAR_FMT
+};
+template <size_t N>
+struct npy_format_descriptor<std::array<char, N>> {
+    PYBIND11_DECL_CHAR_FMT
+};
 #undef PYBIND11_DECL_CHAR_FMT
 
-template<typename T> struct npy_format_descriptor<T, enable_if_t<array_info<T>::is_array>> {
+template <typename T>
+struct npy_format_descriptor<T, enable_if_t<array_info<T>::is_array>> {
 private:
     using base_descr = npy_format_descriptor<typename array_info<T>::type>;
+
 public:
     static_assert(!array_info<T>::is_empty, "Zero-sized arrays are not supported");
 
-    static constexpr auto name = const_name("(") + array_info<T>::extents + const_name(")") + base_descr::name;
+    static constexpr auto name
+        = const_name("(") + array_info<T>::extents + const_name(")") + base_descr::name;
     static pybind11::dtype dtype() {
         list shape;
         array_info<T>::append_extents(shape);
         return pybind11::dtype::from_args(pybind11::make_tuple(base_descr::dtype(), shape));
     }
 };
 
-template<typename T> struct npy_format_descriptor<T, enable_if_t<std::is_enum<T>::value>> {
+template <typename T>
+struct npy_format_descriptor<T, enable_if_t<std::is_enum<T>::value>> {
 private:
     using base_descr = npy_format_descriptor<typename std::underlying_type<T>::type>;
+
 public:
     static constexpr auto name = base_descr::name;
     static pybind11::dtype dtype() { return base_descr::dtype(); }
 };
 
 struct field_descriptor {
     const char *name;
     ssize_t offset;
     ssize_t size;
     std::string format;
     dtype descr;
 };
 
-PYBIND11_NOINLINE void register_structured_dtype(
-    any_container<field_descriptor> fields,
-    const std::type_info& tinfo, ssize_t itemsize,
-    bool (*direct_converter)(PyObject *, void *&)) {
+PYBIND11_NOINLINE void register_structured_dtype(any_container<field_descriptor> fields,
+                                                 const std::type_info &tinfo,
+                                                 ssize_t itemsize,
+                                                 bool (*direct_converter)(PyObject *, void *&)) {
 
-    auto& numpy_internals = get_numpy_internals();
-    if (numpy_internals.get_type_info(tinfo, false))
+    auto &numpy_internals = get_numpy_internals();
+    if (numpy_internals.get_type_info(tinfo, false)) {
         pybind11_fail("NumPy: dtype is already registered");
+    }
 
     // Use ordered fields because order matters as of NumPy 1.14:
     // https://docs.scipy.org/doc/numpy/release.html#multiple-field-indexing-assignment-of-structured-arrays
     std::vector<field_descriptor> ordered_fields(std::move(fields));
-    std::sort(ordered_fields.begin(), ordered_fields.end(),
+    std::sort(
+        ordered_fields.begin(),
+        ordered_fields.end(),
         [](const field_descriptor &a, const field_descriptor &b) { return a.offset < b.offset; });
 
     list names, formats, offsets;
-    for (auto& field : ordered_fields) {
-        if (!field.descr)
-            pybind11_fail(std::string("NumPy: unsupported field dtype: `") +
-                            field.name + "` @ " + tinfo.name());
+    for (auto &field : ordered_fields) {
+        if (!field.descr) {
+            pybind11_fail(std::string("NumPy: unsupported field dtype: `") + field.name + "` @ "
+                          + tinfo.name());
+        }
         names.append(PYBIND11_STR_TYPE(field.name));
         formats.append(field.descr);
         offsets.append(pybind11::int_(field.offset));
     }
-    auto dtype_ptr
+    auto *dtype_ptr
         = pybind11::dtype(std::move(names), std::move(formats), std::move(offsets), itemsize)
               .release()
               .ptr();
 
     // There is an existing bug in NumPy (as of v1.11): trailing bytes are
     // not encoded explicitly into the format string. This will supposedly
     // get fixed in v1.12; for further details, see these:
@@ -1181,412 +1358,425 @@
     std::ostringstream oss;
     // mark the structure as unaligned with '^', because numpy and C++ don't
     // always agree about alignment (particularly for complex), and we're
     // explicitly listing all our padding. This depends on none of the fields
     // overriding the endianness. Putting the ^ in front of individual fields
     // isn't guaranteed to work due to https://github.com/numpy/numpy/issues/9049
     oss << "^T{";
-    for (auto& field : ordered_fields) {
-        if (field.offset > offset)
+    for (auto &field : ordered_fields) {
+        if (field.offset > offset) {
             oss << (field.offset - offset) << 'x';
+        }
         oss << field.format << ':' << field.name << ':';
         offset = field.offset + field.size;
     }
-    if (itemsize > offset)
+    if (itemsize > offset) {
         oss << (itemsize - offset) << 'x';
+    }
     oss << '}';
     auto format_str = oss.str();
 
     // Sanity check: verify that NumPy properly parses our buffer format string
-    auto& api = npy_api::get();
-    auto arr =  array(buffer_info(nullptr, itemsize, format_str, 1));
-    if (!api.PyArray_EquivTypes_(dtype_ptr, arr.dtype().ptr()))
+    auto &api = npy_api::get();
+    auto arr = array(buffer_info(nullptr, itemsize, format_str, 1));
+    if (!api.PyArray_EquivTypes_(dtype_ptr, arr.dtype().ptr())) {
         pybind11_fail("NumPy: invalid buffer descriptor!");
+    }
 
     auto tindex = std::type_index(tinfo);
-    numpy_internals.registered_dtypes[tindex] = { dtype_ptr, format_str };
+    numpy_internals.registered_dtypes[tindex] = {dtype_ptr, format_str};
     get_internals().direct_conversions[tindex].push_back(direct_converter);
 }
 
-template <typename T, typename SFINAE> struct npy_format_descriptor {
-    static_assert(is_pod_struct<T>::value, "Attempt to use a non-POD or unimplemented POD type as a numpy dtype");
+template <typename T, typename SFINAE>
+struct npy_format_descriptor {
+    static_assert(is_pod_struct<T>::value,
+                  "Attempt to use a non-POD or unimplemented POD type as a numpy dtype");
 
     static constexpr auto name = make_caster<T>::name;
 
-    static pybind11::dtype dtype() {
-        return reinterpret_borrow<pybind11::dtype>(dtype_ptr());
-    }
+    static pybind11::dtype dtype() { return reinterpret_borrow<pybind11::dtype>(dtype_ptr()); }
 
     static std::string format() {
         static auto format_str = get_numpy_internals().get_type_info<T>(true)->format_str;
         return format_str;
     }
 
     static void register_dtype(any_container<field_descriptor> fields) {
-        register_structured_dtype(std::move(fields), typeid(typename std::remove_cv<T>::type),
-                                  sizeof(T), &direct_converter);
+        register_structured_dtype(std::move(fields),
+                                  typeid(typename std::remove_cv<T>::type),
+                                  sizeof(T),
+                                  &direct_converter);
     }
 
 private:
-    static PyObject* dtype_ptr() {
-        static PyObject* ptr = get_numpy_internals().get_type_info<T>(true)->dtype_ptr;
+    static PyObject *dtype_ptr() {
+        static PyObject *ptr = get_numpy_internals().get_type_info<T>(true)->dtype_ptr;
         return ptr;
     }
 
-    static bool direct_converter(PyObject *obj, void*& value) {
-        auto& api = npy_api::get();
-        if (!PyObject_TypeCheck(obj, api.PyVoidArrType_Type_))
+    static bool direct_converter(PyObject *obj, void *&value) {
+        auto &api = npy_api::get();
+        if (!PyObject_TypeCheck(obj, api.PyVoidArrType_Type_)) {
             return false;
+        }
         if (auto descr = reinterpret_steal<object>(api.PyArray_DescrFromScalar_(obj))) {
             if (api.PyArray_EquivTypes_(dtype_ptr(), descr.ptr())) {
                 value = ((PyVoidScalarObject_Proxy *) obj)->obval;
                 return true;
             }
         }
         return false;
     }
 };
 
 #ifdef __CLION_IDE__ // replace heavy macro with dummy code for the IDE (doesn't affect code)
-# define PYBIND11_NUMPY_DTYPE(Type, ...) ((void)0)
-# define PYBIND11_NUMPY_DTYPE_EX(Type, ...) ((void)0)
+#    define PYBIND11_NUMPY_DTYPE(Type, ...) ((void) 0)
+#    define PYBIND11_NUMPY_DTYPE_EX(Type, ...) ((void) 0)
 #else
 
-#define PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, Name)                                          \
-    ::pybind11::detail::field_descriptor {                                                    \
-        Name, offsetof(T, Field), sizeof(decltype(std::declval<T>().Field)),                  \
-        ::pybind11::format_descriptor<decltype(std::declval<T>().Field)>::format(),           \
-        ::pybind11::detail::npy_format_descriptor<decltype(std::declval<T>().Field)>::dtype() \
-    }
+#    define PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, Name)                                          \
+        ::pybind11::detail::field_descriptor {                                                    \
+            Name, offsetof(T, Field), sizeof(decltype(std::declval<T>().Field)),                  \
+                ::pybind11::format_descriptor<decltype(std::declval<T>().Field)>::format(),       \
+                ::pybind11::detail::npy_format_descriptor<                                        \
+                    decltype(std::declval<T>().Field)>::dtype()                                   \
+        }
 
 // Extract name, offset and format descriptor for a struct field
-#define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #Field)
+#    define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #    Field)
 
 // The main idea of this macro is borrowed from https://github.com/swansontec/map-macro
 // (C) William Swanson, Paul Fultz
-#define PYBIND11_EVAL0(...) __VA_ARGS__
-#define PYBIND11_EVAL1(...) PYBIND11_EVAL0 (PYBIND11_EVAL0 (PYBIND11_EVAL0 (__VA_ARGS__)))
-#define PYBIND11_EVAL2(...) PYBIND11_EVAL1 (PYBIND11_EVAL1 (PYBIND11_EVAL1 (__VA_ARGS__)))
-#define PYBIND11_EVAL3(...) PYBIND11_EVAL2 (PYBIND11_EVAL2 (PYBIND11_EVAL2 (__VA_ARGS__)))
-#define PYBIND11_EVAL4(...) PYBIND11_EVAL3 (PYBIND11_EVAL3 (PYBIND11_EVAL3 (__VA_ARGS__)))
-#define PYBIND11_EVAL(...)  PYBIND11_EVAL4 (PYBIND11_EVAL4 (PYBIND11_EVAL4 (__VA_ARGS__)))
-#define PYBIND11_MAP_END(...)
-#define PYBIND11_MAP_OUT
-#define PYBIND11_MAP_COMMA ,
-#define PYBIND11_MAP_GET_END() 0, PYBIND11_MAP_END
-#define PYBIND11_MAP_NEXT0(test, next, ...) next PYBIND11_MAP_OUT
-#define PYBIND11_MAP_NEXT1(test, next) PYBIND11_MAP_NEXT0 (test, next, 0)
-#define PYBIND11_MAP_NEXT(test, next)  PYBIND11_MAP_NEXT1 (PYBIND11_MAP_GET_END test, next)
-#if defined(_MSC_VER) && !defined(__clang__) // MSVC is not as eager to expand macros, hence this workaround
-#define PYBIND11_MAP_LIST_NEXT1(test, next) \
-    PYBIND11_EVAL0 (PYBIND11_MAP_NEXT0 (test, PYBIND11_MAP_COMMA next, 0))
-#else
-#define PYBIND11_MAP_LIST_NEXT1(test, next) \
-    PYBIND11_MAP_NEXT0 (test, PYBIND11_MAP_COMMA next, 0)
-#endif
-#define PYBIND11_MAP_LIST_NEXT(test, next) \
-    PYBIND11_MAP_LIST_NEXT1 (PYBIND11_MAP_GET_END test, next)
-#define PYBIND11_MAP_LIST0(f, t, x, peek, ...) \
-    f(t, x) PYBIND11_MAP_LIST_NEXT (peek, PYBIND11_MAP_LIST1) (f, t, peek, __VA_ARGS__)
-#define PYBIND11_MAP_LIST1(f, t, x, peek, ...) \
-    f(t, x) PYBIND11_MAP_LIST_NEXT (peek, PYBIND11_MAP_LIST0) (f, t, peek, __VA_ARGS__)
+#    define PYBIND11_EVAL0(...) __VA_ARGS__
+#    define PYBIND11_EVAL1(...) PYBIND11_EVAL0(PYBIND11_EVAL0(PYBIND11_EVAL0(__VA_ARGS__)))
+#    define PYBIND11_EVAL2(...) PYBIND11_EVAL1(PYBIND11_EVAL1(PYBIND11_EVAL1(__VA_ARGS__)))
+#    define PYBIND11_EVAL3(...) PYBIND11_EVAL2(PYBIND11_EVAL2(PYBIND11_EVAL2(__VA_ARGS__)))
+#    define PYBIND11_EVAL4(...) PYBIND11_EVAL3(PYBIND11_EVAL3(PYBIND11_EVAL3(__VA_ARGS__)))
+#    define PYBIND11_EVAL(...) PYBIND11_EVAL4(PYBIND11_EVAL4(PYBIND11_EVAL4(__VA_ARGS__)))
+#    define PYBIND11_MAP_END(...)
+#    define PYBIND11_MAP_OUT
+#    define PYBIND11_MAP_COMMA ,
+#    define PYBIND11_MAP_GET_END() 0, PYBIND11_MAP_END
+#    define PYBIND11_MAP_NEXT0(test, next, ...) next PYBIND11_MAP_OUT
+#    define PYBIND11_MAP_NEXT1(test, next) PYBIND11_MAP_NEXT0(test, next, 0)
+#    define PYBIND11_MAP_NEXT(test, next) PYBIND11_MAP_NEXT1(PYBIND11_MAP_GET_END test, next)
+#    if defined(_MSC_VER)                                                                         \
+        && !defined(__clang__) // MSVC is not as eager to expand macros, hence this workaround
+#        define PYBIND11_MAP_LIST_NEXT1(test, next)                                               \
+            PYBIND11_EVAL0(PYBIND11_MAP_NEXT0(test, PYBIND11_MAP_COMMA next, 0))
+#    else
+#        define PYBIND11_MAP_LIST_NEXT1(test, next)                                               \
+            PYBIND11_MAP_NEXT0(test, PYBIND11_MAP_COMMA next, 0)
+#    endif
+#    define PYBIND11_MAP_LIST_NEXT(test, next)                                                    \
+        PYBIND11_MAP_LIST_NEXT1(PYBIND11_MAP_GET_END test, next)
+#    define PYBIND11_MAP_LIST0(f, t, x, peek, ...)                                                \
+        f(t, x) PYBIND11_MAP_LIST_NEXT(peek, PYBIND11_MAP_LIST1)(f, t, peek, __VA_ARGS__)
+#    define PYBIND11_MAP_LIST1(f, t, x, peek, ...)                                                \
+        f(t, x) PYBIND11_MAP_LIST_NEXT(peek, PYBIND11_MAP_LIST0)(f, t, peek, __VA_ARGS__)
 // PYBIND11_MAP_LIST(f, t, a1, a2, ...) expands to f(t, a1), f(t, a2), ...
-#define PYBIND11_MAP_LIST(f, t, ...) \
-    PYBIND11_EVAL (PYBIND11_MAP_LIST1 (f, t, __VA_ARGS__, (), 0))
+#    define PYBIND11_MAP_LIST(f, t, ...)                                                          \
+        PYBIND11_EVAL(PYBIND11_MAP_LIST1(f, t, __VA_ARGS__, (), 0))
 
-#define PYBIND11_NUMPY_DTYPE(Type, ...) \
-    ::pybind11::detail::npy_format_descriptor<Type>::register_dtype \
-        (::std::vector<::pybind11::detail::field_descriptor> \
-         {PYBIND11_MAP_LIST (PYBIND11_FIELD_DESCRIPTOR, Type, __VA_ARGS__)})
-
-#if defined(_MSC_VER) && !defined(__clang__)
-#define PYBIND11_MAP2_LIST_NEXT1(test, next) \
-    PYBIND11_EVAL0 (PYBIND11_MAP_NEXT0 (test, PYBIND11_MAP_COMMA next, 0))
-#else
-#define PYBIND11_MAP2_LIST_NEXT1(test, next) \
-    PYBIND11_MAP_NEXT0 (test, PYBIND11_MAP_COMMA next, 0)
-#endif
-#define PYBIND11_MAP2_LIST_NEXT(test, next) \
-    PYBIND11_MAP2_LIST_NEXT1 (PYBIND11_MAP_GET_END test, next)
-#define PYBIND11_MAP2_LIST0(f, t, x1, x2, peek, ...) \
-    f(t, x1, x2) PYBIND11_MAP2_LIST_NEXT (peek, PYBIND11_MAP2_LIST1) (f, t, peek, __VA_ARGS__)
-#define PYBIND11_MAP2_LIST1(f, t, x1, x2, peek, ...) \
-    f(t, x1, x2) PYBIND11_MAP2_LIST_NEXT (peek, PYBIND11_MAP2_LIST0) (f, t, peek, __VA_ARGS__)
+#    define PYBIND11_NUMPY_DTYPE(Type, ...)                                                       \
+        ::pybind11::detail::npy_format_descriptor<Type>::register_dtype(                          \
+            ::std::vector<::pybind11::detail::field_descriptor>{                                  \
+                PYBIND11_MAP_LIST(PYBIND11_FIELD_DESCRIPTOR, Type, __VA_ARGS__)})
+
+#    if defined(_MSC_VER) && !defined(__clang__)
+#        define PYBIND11_MAP2_LIST_NEXT1(test, next)                                              \
+            PYBIND11_EVAL0(PYBIND11_MAP_NEXT0(test, PYBIND11_MAP_COMMA next, 0))
+#    else
+#        define PYBIND11_MAP2_LIST_NEXT1(test, next)                                              \
+            PYBIND11_MAP_NEXT0(test, PYBIND11_MAP_COMMA next, 0)
+#    endif
+#    define PYBIND11_MAP2_LIST_NEXT(test, next)                                                   \
+        PYBIND11_MAP2_LIST_NEXT1(PYBIND11_MAP_GET_END test, next)
+#    define PYBIND11_MAP2_LIST0(f, t, x1, x2, peek, ...)                                          \
+        f(t, x1, x2) PYBIND11_MAP2_LIST_NEXT(peek, PYBIND11_MAP2_LIST1)(f, t, peek, __VA_ARGS__)
+#    define PYBIND11_MAP2_LIST1(f, t, x1, x2, peek, ...)                                          \
+        f(t, x1, x2) PYBIND11_MAP2_LIST_NEXT(peek, PYBIND11_MAP2_LIST0)(f, t, peek, __VA_ARGS__)
 // PYBIND11_MAP2_LIST(f, t, a1, a2, ...) expands to f(t, a1, a2), f(t, a3, a4), ...
-#define PYBIND11_MAP2_LIST(f, t, ...) \
-    PYBIND11_EVAL (PYBIND11_MAP2_LIST1 (f, t, __VA_ARGS__, (), 0))
+#    define PYBIND11_MAP2_LIST(f, t, ...)                                                         \
+        PYBIND11_EVAL(PYBIND11_MAP2_LIST1(f, t, __VA_ARGS__, (), 0))
 
-#define PYBIND11_NUMPY_DTYPE_EX(Type, ...) \
-    ::pybind11::detail::npy_format_descriptor<Type>::register_dtype \
-        (::std::vector<::pybind11::detail::field_descriptor> \
-         {PYBIND11_MAP2_LIST (PYBIND11_FIELD_DESCRIPTOR_EX, Type, __VA_ARGS__)})
+#    define PYBIND11_NUMPY_DTYPE_EX(Type, ...)                                                    \
+        ::pybind11::detail::npy_format_descriptor<Type>::register_dtype(                          \
+            ::std::vector<::pybind11::detail::field_descriptor>{                                  \
+                PYBIND11_MAP2_LIST(PYBIND11_FIELD_DESCRIPTOR_EX, Type, __VA_ARGS__)})
 
 #endif // __CLION_IDE__
 
 class common_iterator {
 public:
     using container_type = std::vector<ssize_t>;
     using value_type = container_type::value_type;
     using size_type = container_type::size_type;
 
     common_iterator() : m_strides() {}
 
-    common_iterator(void* ptr, const container_type& strides, const container_type& shape)
-        : p_ptr(reinterpret_cast<char*>(ptr)), m_strides(strides.size()) {
+    common_iterator(void *ptr, const container_type &strides, const container_type &shape)
+        : p_ptr(reinterpret_cast<char *>(ptr)), m_strides(strides.size()) {
         m_strides.back() = static_cast<value_type>(strides.back());
         for (size_type i = m_strides.size() - 1; i != 0; --i) {
             size_type j = i - 1;
             auto s = static_cast<value_type>(shape[i]);
             m_strides[j] = strides[j] + m_strides[i] - strides[i] * s;
         }
     }
 
-    void increment(size_type dim) {
-        p_ptr += m_strides[dim];
-    }
+    void increment(size_type dim) { p_ptr += m_strides[dim]; }
 
-    void* data() const {
-        return p_ptr;
-    }
+    void *data() const { return p_ptr; }
 
 private:
     char *p_ptr{0};
     container_type m_strides;
 };
 
-template <size_t N> class multi_array_iterator {
+template <size_t N>
+class multi_array_iterator {
 public:
     using container_type = std::vector<ssize_t>;
 
-    multi_array_iterator(const std::array<buffer_info, N> &buffers,
-                         const container_type &shape)
-        : m_shape(shape.size()), m_index(shape.size(), 0),
-          m_common_iterator() {
+    multi_array_iterator(const std::array<buffer_info, N> &buffers, const container_type &shape)
+        : m_shape(shape.size()), m_index(shape.size(), 0), m_common_iterator() {
 
         // Manual copy to avoid conversion warning if using std::copy
-        for (size_t i = 0; i < shape.size(); ++i)
+        for (size_t i = 0; i < shape.size(); ++i) {
             m_shape[i] = shape[i];
+        }
 
         container_type strides(shape.size());
-        for (size_t i = 0; i < N; ++i)
+        for (size_t i = 0; i < N; ++i) {
             init_common_iterator(buffers[i], shape, m_common_iterator[i], strides);
+        }
     }
 
-    multi_array_iterator& operator++() {
+    multi_array_iterator &operator++() {
         for (size_t j = m_index.size(); j != 0; --j) {
             size_t i = j - 1;
             if (++m_index[i] != m_shape[i]) {
                 increment_common_iterator(i);
                 break;
             }
             m_index[i] = 0;
         }
         return *this;
     }
 
-    template <size_t K, class T = void> T* data() const {
-        return reinterpret_cast<T*>(m_common_iterator[K].data());
+    template <size_t K, class T = void>
+    T *data() const {
+        return reinterpret_cast<T *>(m_common_iterator[K].data());
     }
 
 private:
-
     using common_iter = common_iterator;
 
     void init_common_iterator(const buffer_info &buffer,
                               const container_type &shape,
                               common_iter &iterator,
                               container_type &strides) {
         auto buffer_shape_iter = buffer.shape.rbegin();
         auto buffer_strides_iter = buffer.strides.rbegin();
         auto shape_iter = shape.rbegin();
         auto strides_iter = strides.rbegin();
 
         while (buffer_shape_iter != buffer.shape.rend()) {
-            if (*shape_iter == *buffer_shape_iter)
+            if (*shape_iter == *buffer_shape_iter) {
                 *strides_iter = *buffer_strides_iter;
-            else
+            } else {
                 *strides_iter = 0;
+            }
 
             ++buffer_shape_iter;
             ++buffer_strides_iter;
             ++shape_iter;
             ++strides_iter;
         }
 
         std::fill(strides_iter, strides.rend(), 0);
         iterator = common_iter(buffer.ptr, strides, shape);
     }
 
     void increment_common_iterator(size_t dim) {
-        for (auto &iter : m_common_iterator)
+        for (auto &iter : m_common_iterator) {
             iter.increment(dim);
+        }
     }
 
     container_type m_shape;
     container_type m_index;
     std::array<common_iter, N> m_common_iterator;
 };
 
 enum class broadcast_trivial { non_trivial, c_trivial, f_trivial };
 
-// Populates the shape and number of dimensions for the set of buffers.  Returns a broadcast_trivial
-// enum value indicating whether the broadcast is "trivial"--that is, has each buffer being either a
-// singleton or a full-size, C-contiguous (`c_trivial`) or Fortran-contiguous (`f_trivial`) storage
-// buffer; returns `non_trivial` otherwise.
+// Populates the shape and number of dimensions for the set of buffers.  Returns a
+// broadcast_trivial enum value indicating whether the broadcast is "trivial"--that is, has each
+// buffer being either a singleton or a full-size, C-contiguous (`c_trivial`) or Fortran-contiguous
+// (`f_trivial`) storage buffer; returns `non_trivial` otherwise.
 template <size_t N>
-broadcast_trivial broadcast(const std::array<buffer_info, N> &buffers, ssize_t &ndim, std::vector<ssize_t> &shape) {
-    ndim = std::accumulate(buffers.begin(), buffers.end(), ssize_t(0), [](ssize_t res, const buffer_info &buf) {
-        return std::max(res, buf.ndim);
-    });
+broadcast_trivial
+broadcast(const std::array<buffer_info, N> &buffers, ssize_t &ndim, std::vector<ssize_t> &shape) {
+    ndim = std::accumulate(
+        buffers.begin(), buffers.end(), ssize_t(0), [](ssize_t res, const buffer_info &buf) {
+            return std::max(res, buf.ndim);
+        });
 
     shape.clear();
     shape.resize((size_t) ndim, 1);
 
-    // Figure out the output size, and make sure all input arrays conform (i.e. are either size 1 or
-    // the full size).
+    // Figure out the output size, and make sure all input arrays conform (i.e. are either size 1
+    // or the full size).
     for (size_t i = 0; i < N; ++i) {
         auto res_iter = shape.rbegin();
         auto end = buffers[i].shape.rend();
-        for (auto shape_iter = buffers[i].shape.rbegin(); shape_iter != end; ++shape_iter, ++res_iter) {
+        for (auto shape_iter = buffers[i].shape.rbegin(); shape_iter != end;
+             ++shape_iter, ++res_iter) {
             const auto &dim_size_in = *shape_iter;
             auto &dim_size_out = *res_iter;
 
-            // Each input dimension can either be 1 or `n`, but `n` values must match across buffers
-            if (dim_size_out == 1)
+            // Each input dimension can either be 1 or `n`, but `n` values must match across
+            // buffers
+            if (dim_size_out == 1) {
                 dim_size_out = dim_size_in;
-            else if (dim_size_in != 1 && dim_size_in != dim_size_out)
+            } else if (dim_size_in != 1 && dim_size_in != dim_size_out) {
                 pybind11_fail("pybind11::vectorize: incompatible size/dimension of inputs!");
+            }
         }
     }
 
     bool trivial_broadcast_c = true;
     bool trivial_broadcast_f = true;
     for (size_t i = 0; i < N && (trivial_broadcast_c || trivial_broadcast_f); ++i) {
-        if (buffers[i].size == 1)
+        if (buffers[i].size == 1) {
             continue;
+        }
 
         // Require the same number of dimensions:
-        if (buffers[i].ndim != ndim)
+        if (buffers[i].ndim != ndim) {
             return broadcast_trivial::non_trivial;
+        }
 
         // Require all dimensions be full-size:
-        if (!std::equal(buffers[i].shape.cbegin(), buffers[i].shape.cend(), shape.cbegin()))
+        if (!std::equal(buffers[i].shape.cbegin(), buffers[i].shape.cend(), shape.cbegin())) {
             return broadcast_trivial::non_trivial;
+        }
 
         // Check for C contiguity (but only if previous inputs were also C contiguous)
         if (trivial_broadcast_c) {
             ssize_t expect_stride = buffers[i].itemsize;
             auto end = buffers[i].shape.crend();
-            for (auto shape_iter = buffers[i].shape.crbegin(), stride_iter = buffers[i].strides.crbegin();
-                    trivial_broadcast_c && shape_iter != end; ++shape_iter, ++stride_iter) {
-                if (expect_stride == *stride_iter)
+            for (auto shape_iter = buffers[i].shape.crbegin(),
+                      stride_iter = buffers[i].strides.crbegin();
+                 trivial_broadcast_c && shape_iter != end;
+                 ++shape_iter, ++stride_iter) {
+                if (expect_stride == *stride_iter) {
                     expect_stride *= *shape_iter;
-                else
+                } else {
                     trivial_broadcast_c = false;
+                }
             }
         }
 
         // Check for Fortran contiguity (if previous inputs were also F contiguous)
         if (trivial_broadcast_f) {
             ssize_t expect_stride = buffers[i].itemsize;
             auto end = buffers[i].shape.cend();
-            for (auto shape_iter = buffers[i].shape.cbegin(), stride_iter = buffers[i].strides.cbegin();
-                    trivial_broadcast_f && shape_iter != end; ++shape_iter, ++stride_iter) {
-                if (expect_stride == *stride_iter)
+            for (auto shape_iter = buffers[i].shape.cbegin(),
+                      stride_iter = buffers[i].strides.cbegin();
+                 trivial_broadcast_f && shape_iter != end;
+                 ++shape_iter, ++stride_iter) {
+                if (expect_stride == *stride_iter) {
                     expect_stride *= *shape_iter;
-                else
+                } else {
                     trivial_broadcast_f = false;
+                }
             }
         }
     }
 
-    return
-        trivial_broadcast_c ? broadcast_trivial::c_trivial :
-        trivial_broadcast_f ? broadcast_trivial::f_trivial :
-        broadcast_trivial::non_trivial;
+    return trivial_broadcast_c   ? broadcast_trivial::c_trivial
+           : trivial_broadcast_f ? broadcast_trivial::f_trivial
+                                 : broadcast_trivial::non_trivial;
 }
 
 template <typename T>
 struct vectorize_arg {
-    static_assert(!std::is_rvalue_reference<T>::value, "Functions with rvalue reference arguments cannot be vectorized");
+    static_assert(!std::is_rvalue_reference<T>::value,
+                  "Functions with rvalue reference arguments cannot be vectorized");
     // The wrapped function gets called with this type:
     using call_type = remove_reference_t<T>;
     // Is this a vectorized argument?
-    static constexpr bool vectorize =
-        satisfies_any_of<call_type, std::is_arithmetic, is_complex, is_pod>::value &&
-        satisfies_none_of<call_type, std::is_pointer, std::is_array, is_std_array, std::is_enum>::value &&
-        (!std::is_reference<T>::value ||
-         (std::is_lvalue_reference<T>::value && std::is_const<call_type>::value));
+    static constexpr bool vectorize
+        = satisfies_any_of<call_type, std::is_arithmetic, is_complex, is_pod>::value
+          && satisfies_none_of<call_type,
+                               std::is_pointer,
+                               std::is_array,
+                               is_std_array,
+                               std::is_enum>::value
+          && (!std::is_reference<T>::value
+              || (std::is_lvalue_reference<T>::value && std::is_const<call_type>::value));
     // Accept this type: an array for vectorized types, otherwise the type as-is:
     using type = conditional_t<vectorize, array_t<remove_cv_t<call_type>, array::forcecast>, T>;
 };
 
-
 // py::vectorize when a return type is present
 template <typename Func, typename Return, typename... Args>
 struct vectorize_returned_array {
     using Type = array_t<Return>;
 
     static Type create(broadcast_trivial trivial, const std::vector<ssize_t> &shape) {
-        if (trivial == broadcast_trivial::f_trivial)
+        if (trivial == broadcast_trivial::f_trivial) {
             return array_t<Return, array::f_style>(shape);
+        }
         return array_t<Return>(shape);
     }
 
-    static Return *mutable_data(Type &array) {
-        return array.mutable_data();
-    }
+    static Return *mutable_data(Type &array) { return array.mutable_data(); }
 
-    static Return call(Func &f, Args &... args) {
-        return f(args...);
-    }
+    static Return call(Func &f, Args &...args) { return f(args...); }
 
-    static void call(Return *out, size_t i, Func &f, Args &... args) {
-        out[i] = f(args...);
-    }
+    static void call(Return *out, size_t i, Func &f, Args &...args) { out[i] = f(args...); }
 };
 
 // py::vectorize when a return type is not present
 template <typename Func, typename... Args>
 struct vectorize_returned_array<Func, void, Args...> {
     using Type = none;
 
-    static Type create(broadcast_trivial, const std::vector<ssize_t> &) {
-        return none();
-    }
+    static Type create(broadcast_trivial, const std::vector<ssize_t> &) { return none(); }
 
-    static void *mutable_data(Type &) {
-        return nullptr;
-    }
+    static void *mutable_data(Type &) { return nullptr; }
 
-    static detail::void_type call(Func &f, Args &... args) {
+    static detail::void_type call(Func &f, Args &...args) {
         f(args...);
         return {};
     }
 
-    static void call(void *, size_t, Func &f, Args &... args) {
-        f(args...);
-    }
+    static void call(void *, size_t, Func &f, Args &...args) { f(args...); }
 };
 
-
 template <typename Func, typename Return, typename... Args>
 struct vectorize_helper {
 
 // NVCC for some reason breaks if NVectorized is private
 #ifdef __CUDACC__
 public:
 #else
 private:
 #endif
 
     static constexpr size_t N = sizeof...(Args);
     static constexpr size_t NVectorized = constexpr_sum(vectorize_arg<Args>::vectorize...);
-    static_assert(NVectorized >= 1,
-            "pybind11::vectorize(...) requires a function with at least one vectorizable argument");
+    static_assert(
+        NVectorized >= 1,
+        "pybind11::vectorize(...) requires a function with at least one vectorizable argument");
 
 public:
     template <typename T,
               // SFINAE to prevent shadowing the copy constructor.
               typename = detail::enable_if_t<
                   !std::is_same<vectorize_helper, typename std::decay<T>::type>::value>>
     explicit vectorize_helper(T &&f) : f(std::forward<T>(f)) {}
@@ -1597,145 +1787,172 @@
                    select_indices<vectorize_arg<Args>::vectorize...>(),
                    make_index_sequence<NVectorized>());
     }
 
 private:
     remove_reference_t<Func> f;
 
-    // Internal compiler error in MSVC 19.16.27025.1 (Visual Studio 2017 15.9.4), when compiling with "/permissive-" flag
-    // when arg_call_types is manually inlined.
+    // Internal compiler error in MSVC 19.16.27025.1 (Visual Studio 2017 15.9.4), when compiling
+    // with "/permissive-" flag when arg_call_types is manually inlined.
     using arg_call_types = std::tuple<typename vectorize_arg<Args>::call_type...>;
-    template <size_t Index> using param_n_t = typename std::tuple_element<Index, arg_call_types>::type;
+    template <size_t Index>
+    using param_n_t = typename std::tuple_element<Index, arg_call_types>::type;
 
     using returned_array = vectorize_returned_array<Func, Return, Args...>;
 
     // Runs a vectorized function given arguments tuple and three index sequences:
     //     - Index is the full set of 0 ... (N-1) argument indices;
     //     - VIndex is the subset of argument indices with vectorized parameters, letting us access
     //       vectorized arguments (anything not in this sequence is passed through)
     //     - BIndex is a incremental sequence (beginning at 0) of the same size as VIndex, so that
     //       we can store vectorized buffer_infos in an array (argument VIndex has its buffer at
     //       index BIndex in the array).
-    template <size_t... Index, size_t... VIndex, size_t... BIndex> object run(
-            typename vectorize_arg<Args>::type &...args,
-            index_sequence<Index...> i_seq, index_sequence<VIndex...> vi_seq, index_sequence<BIndex...> bi_seq) {
+    template <size_t... Index, size_t... VIndex, size_t... BIndex>
+    object run(typename vectorize_arg<Args>::type &...args,
+               index_sequence<Index...> i_seq,
+               index_sequence<VIndex...> vi_seq,
+               index_sequence<BIndex...> bi_seq) {
 
         // Pointers to values the function was called with; the vectorized ones set here will start
         // out as array_t<T> pointers, but they will be changed them to T pointers before we make
         // call the wrapped function.  Non-vectorized pointers are left as-is.
-        std::array<void *, N> params{{ &args... }};
+        std::array<void *, N> params{{&args...}};
 
         // The array of `buffer_info`s of vectorized arguments:
-        std::array<buffer_info, NVectorized> buffers{{ reinterpret_cast<array *>(params[VIndex])->request()... }};
+        std::array<buffer_info, NVectorized> buffers{
+            {reinterpret_cast<array *>(params[VIndex])->request()...}};
 
         /* Determine dimensions parameters of output array */
         ssize_t nd = 0;
         std::vector<ssize_t> shape(0);
         auto trivial = broadcast(buffers, nd, shape);
         auto ndim = (size_t) nd;
 
-        size_t size = std::accumulate(shape.begin(), shape.end(), (size_t) 1, std::multiplies<size_t>());
+        size_t size
+            = std::accumulate(shape.begin(), shape.end(), (size_t) 1, std::multiplies<size_t>());
 
         // If all arguments are 0-dimension arrays (i.e. single values) return a plain value (i.e.
         // not wrapped in an array).
         if (size == 1 && ndim == 0) {
             PYBIND11_EXPAND_SIDE_EFFECTS(params[VIndex] = buffers[BIndex].ptr);
-            return cast(returned_array::call(f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...));
+            return cast(
+                returned_array::call(f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...));
         }
 
         auto result = returned_array::create(trivial, shape);
 
-        if (size == 0) return std::move(result);
+        if (size == 0) {
+            return std::move(result);
+        }
 
         /* Call the function */
-        auto mutable_data = returned_array::mutable_data(result);
-        if (trivial == broadcast_trivial::non_trivial)
+        auto *mutable_data = returned_array::mutable_data(result);
+        if (trivial == broadcast_trivial::non_trivial) {
             apply_broadcast(buffers, params, mutable_data, size, shape, i_seq, vi_seq, bi_seq);
-        else
+        } else {
             apply_trivial(buffers, params, mutable_data, size, i_seq, vi_seq, bi_seq);
+        }
 
         return std::move(result);
     }
 
     template <size_t... Index, size_t... VIndex, size_t... BIndex>
     void apply_trivial(std::array<buffer_info, NVectorized> &buffers,
                        std::array<void *, N> &params,
                        Return *out,
                        size_t size,
-                       index_sequence<Index...>, index_sequence<VIndex...>, index_sequence<BIndex...>) {
+                       index_sequence<Index...>,
+                       index_sequence<VIndex...>,
+                       index_sequence<BIndex...>) {
 
         // Initialize an array of mutable byte references and sizes with references set to the
         // appropriate pointer in `params`; as we iterate, we'll increment each pointer by its size
         // (except for singletons, which get an increment of 0).
-        std::array<std::pair<unsigned char *&, const size_t>, NVectorized> vecparams{{
-            std::pair<unsigned char *&, const size_t>(
-                    reinterpret_cast<unsigned char *&>(params[VIndex] = buffers[BIndex].ptr),
-                    buffers[BIndex].size == 1 ? 0 : sizeof(param_n_t<VIndex>)
-            )...
-        }};
+        std::array<std::pair<unsigned char *&, const size_t>, NVectorized> vecparams{
+            {std::pair<unsigned char *&, const size_t>(
+                reinterpret_cast<unsigned char *&>(params[VIndex] = buffers[BIndex].ptr),
+                buffers[BIndex].size == 1 ? 0 : sizeof(param_n_t<VIndex>))...}};
 
         for (size_t i = 0; i < size; ++i) {
-            returned_array::call(out, i, f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...);
-            for (auto &x : vecparams) x.first += x.second;
+            returned_array::call(
+                out, i, f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...);
+            for (auto &x : vecparams) {
+                x.first += x.second;
+            }
         }
     }
 
     template <size_t... Index, size_t... VIndex, size_t... BIndex>
     void apply_broadcast(std::array<buffer_info, NVectorized> &buffers,
                          std::array<void *, N> &params,
                          Return *out,
                          size_t size,
                          const std::vector<ssize_t> &output_shape,
-                         index_sequence<Index...>, index_sequence<VIndex...>, index_sequence<BIndex...>) {
+                         index_sequence<Index...>,
+                         index_sequence<VIndex...>,
+                         index_sequence<BIndex...>) {
 
         multi_array_iterator<NVectorized> input_iter(buffers, output_shape);
 
         for (size_t i = 0; i < size; ++i, ++input_iter) {
-            PYBIND11_EXPAND_SIDE_EFFECTS((
-                params[VIndex] = input_iter.template data<BIndex>()
-            ));
-            returned_array::call(out, i, f, *reinterpret_cast<param_n_t<Index> *>(std::get<Index>(params))...);
+            PYBIND11_EXPAND_SIDE_EFFECTS((params[VIndex] = input_iter.template data<BIndex>()));
+            returned_array::call(
+                out, i, f, *reinterpret_cast<param_n_t<Index> *>(std::get<Index>(params))...);
         }
     }
 };
 
 template <typename Func, typename Return, typename... Args>
-vectorize_helper<Func, Return, Args...>
-vectorize_extractor(const Func &f, Return (*) (Args ...)) {
+vectorize_helper<Func, Return, Args...> vectorize_extractor(const Func &f, Return (*)(Args...)) {
     return detail::vectorize_helper<Func, Return, Args...>(f);
 }
 
-template <typename T, int Flags> struct handle_type_name<array_t<T, Flags>> {
-    static constexpr auto name = const_name("numpy.ndarray[") + npy_format_descriptor<T>::name + const_name("]");
+template <typename T, int Flags>
+struct handle_type_name<array_t<T, Flags>> {
+    static constexpr auto name
+        = const_name("numpy.ndarray[") + npy_format_descriptor<T>::name + const_name("]");
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 // Vanilla pointer vectorizer:
 template <typename Return, typename... Args>
-detail::vectorize_helper<Return (*)(Args...), Return, Args...>
-vectorize(Return (*f) (Args ...)) {
+detail::vectorize_helper<Return (*)(Args...), Return, Args...> vectorize(Return (*f)(Args...)) {
     return detail::vectorize_helper<Return (*)(Args...), Return, Args...>(f);
 }
 
 // lambda vectorizer:
 template <typename Func, detail::enable_if_t<detail::is_lambda<Func>::value, int> = 0>
-auto vectorize(Func &&f) -> decltype(
-        detail::vectorize_extractor(std::forward<Func>(f), (detail::function_signature_t<Func> *) nullptr)) {
-    return detail::vectorize_extractor(std::forward<Func>(f), (detail::function_signature_t<Func> *) nullptr);
+auto vectorize(Func &&f)
+    -> decltype(detail::vectorize_extractor(std::forward<Func>(f),
+                                            (detail::function_signature_t<Func> *) nullptr)) {
+    return detail::vectorize_extractor(std::forward<Func>(f),
+                                       (detail::function_signature_t<Func> *) nullptr);
 }
 
 // Vectorize a class method (non-const):
-template <typename Return, typename Class, typename... Args,
-          typename Helper = detail::vectorize_helper<decltype(std::mem_fn(std::declval<Return (Class::*)(Args...)>())), Return, Class *, Args...>>
+template <typename Return,
+          typename Class,
+          typename... Args,
+          typename Helper = detail::vectorize_helper<
+              decltype(std::mem_fn(std::declval<Return (Class::*)(Args...)>())),
+              Return,
+              Class *,
+              Args...>>
 Helper vectorize(Return (Class::*f)(Args...)) {
     return Helper(std::mem_fn(f));
 }
 
 // Vectorize a class method (const):
-template <typename Return, typename Class, typename... Args,
-          typename Helper = detail::vectorize_helper<decltype(std::mem_fn(std::declval<Return (Class::*)(Args...) const>())), Return, const Class *, Args...>>
+template <typename Return,
+          typename Class,
+          typename... Args,
+          typename Helper = detail::vectorize_helper<
+              decltype(std::mem_fn(std::declval<Return (Class::*)(Args...) const>())),
+              Return,
+              const Class *,
+              Args...>>
 Helper vectorize(Return (Class::*f)(Args...) const) {
     return Helper(std::mem_fn(f));
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/operators.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/operators.h`

 * *Files 13% similar despite different names*

```diff
@@ -12,148 +12,205 @@
 #include "pybind11.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Enumeration with all supported operator types
 enum op_id : int {
-    op_add, op_sub, op_mul, op_div, op_mod, op_divmod, op_pow, op_lshift,
-    op_rshift, op_and, op_xor, op_or, op_neg, op_pos, op_abs, op_invert,
-    op_int, op_long, op_float, op_str, op_cmp, op_gt, op_ge, op_lt, op_le,
-    op_eq, op_ne, op_iadd, op_isub, op_imul, op_idiv, op_imod, op_ilshift,
-    op_irshift, op_iand, op_ixor, op_ior, op_complex, op_bool, op_nonzero,
-    op_repr, op_truediv, op_itruediv, op_hash
+    op_add,
+    op_sub,
+    op_mul,
+    op_div,
+    op_mod,
+    op_divmod,
+    op_pow,
+    op_lshift,
+    op_rshift,
+    op_and,
+    op_xor,
+    op_or,
+    op_neg,
+    op_pos,
+    op_abs,
+    op_invert,
+    op_int,
+    op_long,
+    op_float,
+    op_str,
+    op_cmp,
+    op_gt,
+    op_ge,
+    op_lt,
+    op_le,
+    op_eq,
+    op_ne,
+    op_iadd,
+    op_isub,
+    op_imul,
+    op_idiv,
+    op_imod,
+    op_ilshift,
+    op_irshift,
+    op_iand,
+    op_ixor,
+    op_ior,
+    op_complex,
+    op_bool,
+    op_nonzero,
+    op_repr,
+    op_truediv,
+    op_itruediv,
+    op_hash
 };
 
 enum op_type : int {
     op_l, /* base type on left */
     op_r, /* base type on right */
     op_u  /* unary operator */
 };
 
-struct self_t { };
+struct self_t {};
 static const self_t self = self_t();
 
 /// Type for an unused type slot
-struct undefined_t { };
+struct undefined_t {};
 
 /// Don't warn about an unused variable
 inline self_t __self() { return self; }
 
 /// base template of operator implementations
-template <op_id, op_type, typename B, typename L, typename R> struct op_impl { };
+template <op_id, op_type, typename B, typename L, typename R>
+struct op_impl {};
 
 /// Operator implementation generator
-template <op_id id, op_type ot, typename L, typename R> struct op_ {
-    template <typename Class, typename... Extra> void execute(Class &cl, const Extra&... extra) const {
+template <op_id id, op_type ot, typename L, typename R>
+struct op_ {
+    template <typename Class, typename... Extra>
+    void execute(Class &cl, const Extra &...extra) const {
         using Base = typename Class::type;
         using L_type = conditional_t<std::is_same<L, self_t>::value, Base, L>;
         using R_type = conditional_t<std::is_same<R, self_t>::value, Base, R>;
         using op = op_impl<id, ot, Base, L_type, R_type>;
         cl.def(op::name(), &op::execute, is_operator(), extra...);
-        #if PY_MAJOR_VERSION < 3
-        if (PYBIND11_SILENCE_MSVC_C4127(id == op_truediv) ||
-            PYBIND11_SILENCE_MSVC_C4127(id == op_itruediv))
-            cl.def(id == op_itruediv ? "__idiv__" : ot == op_l ? "__div__" : "__rdiv__",
-                    &op::execute, is_operator(), extra...);
-        #endif
+#if PY_MAJOR_VERSION < 3
+        if (PYBIND11_SILENCE_MSVC_C4127(id == op_truediv)
+            || PYBIND11_SILENCE_MSVC_C4127(id == op_itruediv))
+            cl.def(id == op_itruediv ? "__idiv__"
+                   : ot == op_l      ? "__div__"
+                                     : "__rdiv__",
+                   &op::execute,
+                   is_operator(),
+                   extra...);
+#endif
     }
-    template <typename Class, typename... Extra> void execute_cast(Class &cl, const Extra&... extra) const {
+    template <typename Class, typename... Extra>
+    void execute_cast(Class &cl, const Extra &...extra) const {
         using Base = typename Class::type;
         using L_type = conditional_t<std::is_same<L, self_t>::value, Base, L>;
         using R_type = conditional_t<std::is_same<R, self_t>::value, Base, R>;
         using op = op_impl<id, ot, Base, L_type, R_type>;
         cl.def(op::name(), &op::execute_cast, is_operator(), extra...);
-        #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
         if (id == op_truediv || id == op_itruediv)
-            cl.def(id == op_itruediv ? "__idiv__" : ot == op_l ? "__div__" : "__rdiv__",
-                    &op::execute, is_operator(), extra...);
-        #endif
+            cl.def(id == op_itruediv ? "__idiv__"
+                   : ot == op_l      ? "__div__"
+                                     : "__rdiv__",
+                   &op::execute,
+                   is_operator(),
+                   extra...);
+#endif
     }
 };
 
-#define PYBIND11_BINARY_OPERATOR(id, rid, op, expr)                                    \
-template <typename B, typename L, typename R> struct op_impl<op_##id, op_l, B, L, R> { \
-    static char const* name() { return "__" #id "__"; }                                \
-    static auto execute(const L &l, const R &r) -> decltype(expr) { return (expr); }   \
-    static B execute_cast(const L &l, const R &r) { return B(expr); }                  \
-};                                                                                     \
-template <typename B, typename L, typename R> struct op_impl<op_##id, op_r, B, L, R> { \
-    static char const* name() { return "__" #rid "__"; }                               \
-    static auto execute(const R &r, const L &l) -> decltype(expr) { return (expr); }   \
-    static B execute_cast(const R &r, const L &l) { return B(expr); }                  \
-};                                                                                     \
-inline op_<op_##id, op_l, self_t, self_t> op(const self_t &, const self_t &) {         \
-    return op_<op_##id, op_l, self_t, self_t>();                                       \
-}                                                                                      \
-template <typename T> op_<op_##id, op_l, self_t, T> op(const self_t &, const T &) {    \
-    return op_<op_##id, op_l, self_t, T>();                                            \
-}                                                                                      \
-template <typename T> op_<op_##id, op_r, T, self_t> op(const T &, const self_t &) {    \
-    return op_<op_##id, op_r, T, self_t>();                                            \
-}
-
-#define PYBIND11_INPLACE_OPERATOR(id, op, expr)                                        \
-template <typename B, typename L, typename R> struct op_impl<op_##id, op_l, B, L, R> { \
-    static char const* name() { return "__" #id "__"; }                                \
-    static auto execute(L &l, const R &r) -> decltype(expr) { return expr; }           \
-    static B execute_cast(L &l, const R &r) { return B(expr); }                        \
-};                                                                                     \
-template <typename T> op_<op_##id, op_l, self_t, T> op(const self_t &, const T &) {    \
-    return op_<op_##id, op_l, self_t, T>();                                            \
-}
-
-#define PYBIND11_UNARY_OPERATOR(id, op, expr)                                          \
-template <typename B, typename L> struct op_impl<op_##id, op_u, B, L, undefined_t> {   \
-    static char const* name() { return "__" #id "__"; }                                \
-    static auto execute(const L &l) -> decltype(expr) { return expr; }                 \
-    static B execute_cast(const L &l) { return B(expr); }                              \
-};                                                                                     \
-inline op_<op_##id, op_u, self_t, undefined_t> op(const self_t &) {                    \
-    return op_<op_##id, op_u, self_t, undefined_t>();                                  \
-}
-
-PYBIND11_BINARY_OPERATOR(sub,       rsub,         operator-,    l - r)
-PYBIND11_BINARY_OPERATOR(add,       radd,         operator+,    l + r)
-PYBIND11_BINARY_OPERATOR(mul,       rmul,         operator*,    l * r)
-PYBIND11_BINARY_OPERATOR(truediv,   rtruediv,     operator/,    l / r)
-PYBIND11_BINARY_OPERATOR(mod,       rmod,         operator%,    l % r)
-PYBIND11_BINARY_OPERATOR(lshift,    rlshift,      operator<<,   l << r)
-PYBIND11_BINARY_OPERATOR(rshift,    rrshift,      operator>>,   l >> r)
-PYBIND11_BINARY_OPERATOR(and,       rand,         operator&,    l & r)
-PYBIND11_BINARY_OPERATOR(xor,       rxor,         operator^,    l ^ r)
-PYBIND11_BINARY_OPERATOR(eq,        eq,           operator==,   l == r)
-PYBIND11_BINARY_OPERATOR(ne,        ne,           operator!=,   l != r)
-PYBIND11_BINARY_OPERATOR(or,        ror,          operator|,    l | r)
-PYBIND11_BINARY_OPERATOR(gt,        lt,           operator>,    l > r)
-PYBIND11_BINARY_OPERATOR(ge,        le,           operator>=,   l >= r)
-PYBIND11_BINARY_OPERATOR(lt,        gt,           operator<,    l < r)
-PYBIND11_BINARY_OPERATOR(le,        ge,           operator<=,   l <= r)
-//PYBIND11_BINARY_OPERATOR(pow,       rpow,         pow,          std::pow(l,  r))
-PYBIND11_INPLACE_OPERATOR(iadd,     operator+=,   l += r)
-PYBIND11_INPLACE_OPERATOR(isub,     operator-=,   l -= r)
-PYBIND11_INPLACE_OPERATOR(imul,     operator*=,   l *= r)
-PYBIND11_INPLACE_OPERATOR(itruediv, operator/=,   l /= r)
-PYBIND11_INPLACE_OPERATOR(imod,     operator%=,   l %= r)
-PYBIND11_INPLACE_OPERATOR(ilshift,  operator<<=,  l <<= r)
-PYBIND11_INPLACE_OPERATOR(irshift,  operator>>=,  l >>= r)
-PYBIND11_INPLACE_OPERATOR(iand,     operator&=,   l &= r)
-PYBIND11_INPLACE_OPERATOR(ixor,     operator^=,   l ^= r)
-PYBIND11_INPLACE_OPERATOR(ior,      operator|=,   l |= r)
-PYBIND11_UNARY_OPERATOR(neg,        operator-,    -l)
-PYBIND11_UNARY_OPERATOR(pos,        operator+,    +l)
+#define PYBIND11_BINARY_OPERATOR(id, rid, op, expr)                                               \
+    template <typename B, typename L, typename R>                                                 \
+    struct op_impl<op_##id, op_l, B, L, R> {                                                      \
+        static char const *name() { return "__" #id "__"; }                                       \
+        static auto execute(const L &l, const R &r) -> decltype(expr) { return (expr); }          \
+        static B execute_cast(const L &l, const R &r) { return B(expr); }                         \
+    };                                                                                            \
+    template <typename B, typename L, typename R>                                                 \
+    struct op_impl<op_##id, op_r, B, L, R> {                                                      \
+        static char const *name() { return "__" #rid "__"; }                                      \
+        static auto execute(const R &r, const L &l) -> decltype(expr) { return (expr); }          \
+        static B execute_cast(const R &r, const L &l) { return B(expr); }                         \
+    };                                                                                            \
+    inline op_<op_##id, op_l, self_t, self_t> op(const self_t &, const self_t &) {                \
+        return op_<op_##id, op_l, self_t, self_t>();                                              \
+    }                                                                                             \
+    template <typename T>                                                                         \
+    op_<op_##id, op_l, self_t, T> op(const self_t &, const T &) {                                 \
+        return op_<op_##id, op_l, self_t, T>();                                                   \
+    }                                                                                             \
+    template <typename T>                                                                         \
+    op_<op_##id, op_r, T, self_t> op(const T &, const self_t &) {                                 \
+        return op_<op_##id, op_r, T, self_t>();                                                   \
+    }
+
+#define PYBIND11_INPLACE_OPERATOR(id, op, expr)                                                   \
+    template <typename B, typename L, typename R>                                                 \
+    struct op_impl<op_##id, op_l, B, L, R> {                                                      \
+        static char const *name() { return "__" #id "__"; }                                       \
+        static auto execute(L &l, const R &r) -> decltype(expr) { return expr; }                  \
+        static B execute_cast(L &l, const R &r) { return B(expr); }                               \
+    };                                                                                            \
+    template <typename T>                                                                         \
+    op_<op_##id, op_l, self_t, T> op(const self_t &, const T &) {                                 \
+        return op_<op_##id, op_l, self_t, T>();                                                   \
+    }
+
+#define PYBIND11_UNARY_OPERATOR(id, op, expr)                                                     \
+    template <typename B, typename L>                                                             \
+    struct op_impl<op_##id, op_u, B, L, undefined_t> {                                            \
+        static char const *name() { return "__" #id "__"; }                                       \
+        static auto execute(const L &l) -> decltype(expr) { return expr; }                        \
+        static B execute_cast(const L &l) { return B(expr); }                                     \
+    };                                                                                            \
+    inline op_<op_##id, op_u, self_t, undefined_t> op(const self_t &) {                           \
+        return op_<op_##id, op_u, self_t, undefined_t>();                                         \
+    }
+
+PYBIND11_BINARY_OPERATOR(sub, rsub, operator-, l - r)
+PYBIND11_BINARY_OPERATOR(add, radd, operator+, l + r)
+PYBIND11_BINARY_OPERATOR(mul, rmul, operator*, l *r)
+PYBIND11_BINARY_OPERATOR(truediv, rtruediv, operator/, l / r)
+PYBIND11_BINARY_OPERATOR(mod, rmod, operator%, l % r)
+PYBIND11_BINARY_OPERATOR(lshift, rlshift, operator<<, l << r)
+PYBIND11_BINARY_OPERATOR(rshift, rrshift, operator>>, l >> r)
+PYBIND11_BINARY_OPERATOR(and, rand, operator&, l &r)
+PYBIND11_BINARY_OPERATOR(xor, rxor, operator^, l ^ r)
+PYBIND11_BINARY_OPERATOR(eq, eq, operator==, l == r)
+PYBIND11_BINARY_OPERATOR(ne, ne, operator!=, l != r)
+PYBIND11_BINARY_OPERATOR(or, ror, operator|, l | r)
+PYBIND11_BINARY_OPERATOR(gt, lt, operator>, l > r)
+PYBIND11_BINARY_OPERATOR(ge, le, operator>=, l >= r)
+PYBIND11_BINARY_OPERATOR(lt, gt, operator<, l < r)
+PYBIND11_BINARY_OPERATOR(le, ge, operator<=, l <= r)
+// PYBIND11_BINARY_OPERATOR(pow,       rpow,         pow,          std::pow(l,  r))
+PYBIND11_INPLACE_OPERATOR(iadd, operator+=, l += r)
+PYBIND11_INPLACE_OPERATOR(isub, operator-=, l -= r)
+PYBIND11_INPLACE_OPERATOR(imul, operator*=, l *= r)
+PYBIND11_INPLACE_OPERATOR(itruediv, operator/=, l /= r)
+PYBIND11_INPLACE_OPERATOR(imod, operator%=, l %= r)
+PYBIND11_INPLACE_OPERATOR(ilshift, operator<<=, l <<= r)
+PYBIND11_INPLACE_OPERATOR(irshift, operator>>=, l >>= r)
+PYBIND11_INPLACE_OPERATOR(iand, operator&=, l &= r)
+PYBIND11_INPLACE_OPERATOR(ixor, operator^=, l ^= r)
+PYBIND11_INPLACE_OPERATOR(ior, operator|=, l |= r)
+PYBIND11_UNARY_OPERATOR(neg, operator-, -l)
+PYBIND11_UNARY_OPERATOR(pos, operator+, +l)
 // WARNING: This usage of `abs` should only be done for existing STL overloads.
 // Adding overloads directly in to the `std::` namespace is advised against:
 // https://en.cppreference.com/w/cpp/language/extending_std
-PYBIND11_UNARY_OPERATOR(abs,        abs,          std::abs(l))
-PYBIND11_UNARY_OPERATOR(hash,       hash,         std::hash<L>()(l))
-PYBIND11_UNARY_OPERATOR(invert,     operator~,    (~l))
-PYBIND11_UNARY_OPERATOR(bool,       operator!,    !!l)
-PYBIND11_UNARY_OPERATOR(int,        int_,         (int) l)
-PYBIND11_UNARY_OPERATOR(float,      float_,       (double) l)
+PYBIND11_UNARY_OPERATOR(abs, abs, std::abs(l))
+PYBIND11_UNARY_OPERATOR(hash, hash, std::hash<L>()(l))
+PYBIND11_UNARY_OPERATOR(invert, operator~, (~l))
+PYBIND11_UNARY_OPERATOR(bool, operator!, !!l)
+PYBIND11_UNARY_OPERATOR(int, int_, (int) l)
+PYBIND11_UNARY_OPERATOR(float, float_, (double) l)
 
 #undef PYBIND11_BINARY_OPERATOR
 #undef PYBIND11_INPLACE_OPERATOR
 #undef PYBIND11_UNARY_OPERATOR
 PYBIND11_NAMESPACE_END(detail)
 
 using detail::self;
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/options.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/options.h`

 * *Files 10% similar despite different names*

```diff
@@ -11,51 +11,62 @@
 
 #include "detail/common.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 class options {
 public:
-
     // Default RAII constructor, which leaves settings as they currently are.
     options() : previous_state(global_state()) {}
 
     // Class is non-copyable.
-    options(const options&) = delete;
-    options& operator=(const options&) = delete;
+    options(const options &) = delete;
+    options &operator=(const options &) = delete;
 
     // Destructor, which restores settings that were in effect before.
-    ~options() {
-        global_state() = previous_state;
-    }
+    ~options() { global_state() = previous_state; }
 
     // Setter methods (affect the global state):
 
-    options& disable_user_defined_docstrings() & { global_state().show_user_defined_docstrings = false; return *this; }
+    options &disable_user_defined_docstrings() & {
+        global_state().show_user_defined_docstrings = false;
+        return *this;
+    }
 
-    options& enable_user_defined_docstrings() & { global_state().show_user_defined_docstrings = true; return *this; }
+    options &enable_user_defined_docstrings() & {
+        global_state().show_user_defined_docstrings = true;
+        return *this;
+    }
 
-    options& disable_function_signatures() & { global_state().show_function_signatures = false; return *this; }
+    options &disable_function_signatures() & {
+        global_state().show_function_signatures = false;
+        return *this;
+    }
 
-    options& enable_function_signatures() & { global_state().show_function_signatures = true; return *this; }
+    options &enable_function_signatures() & {
+        global_state().show_function_signatures = true;
+        return *this;
+    }
 
     // Getter methods (return the global state):
 
-    static bool show_user_defined_docstrings() { return global_state().show_user_defined_docstrings; }
+    static bool show_user_defined_docstrings() {
+        return global_state().show_user_defined_docstrings;
+    }
 
     static bool show_function_signatures() { return global_state().show_function_signatures; }
 
     // This type is not meant to be allocated on the heap.
-    void* operator new(size_t) = delete;
+    void *operator new(size_t) = delete;
 
 private:
-
     struct state {
-        bool show_user_defined_docstrings = true;  //< Include user-supplied texts in docstrings.
-        bool show_function_signatures = true;      //< Include auto-generated function signatures in docstrings.
+        bool show_user_defined_docstrings = true; //< Include user-supplied texts in docstrings.
+        bool show_function_signatures = true;     //< Include auto-generated function signatures
+                                                  //  in docstrings.
     };
 
     static state &global_state() {
         static state instance;
         return instance;
     }
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/pybind11.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/pybind11.h`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,37 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include "detail/class.h"
+#include "detail/init.h"
 #include "attr.h"
 #include "gil.h"
 #include "options.h"
-#include "detail/class.h"
-#include "detail/init.h"
 
 #include <cstdlib>
+#include <cstring>
 #include <memory>
 #include <new>
-#include <vector>
 #include <string>
 #include <utility>
-
-#include <cstring>
+#include <vector>
 
 #if defined(__cpp_lib_launder) && !(defined(_MSC_VER) && (_MSC_VER < 1914))
-#  define PYBIND11_STD_LAUNDER std::launder
-#  define PYBIND11_HAS_STD_LAUNDER 1
+#    define PYBIND11_STD_LAUNDER std::launder
+#    define PYBIND11_HAS_STD_LAUNDER 1
 #else
-#  define PYBIND11_STD_LAUNDER
-#  define PYBIND11_HAS_STD_LAUNDER 0
+#    define PYBIND11_STD_LAUNDER
+#    define PYBIND11_HAS_STD_LAUNDER 0
 #endif
 #if defined(__GNUG__) && !defined(__clang__)
-#  include <cxxabi.h>
+#    include <cxxabi.h>
 #endif
 
 /* https://stackoverflow.com/questions/46798456/handling-gccs-noexcept-type-warning
    This warning is about ABI compatibility, not code health.
    It is only actually needed in a couple places, but apparently GCC 7 "generates this warning if
    and only if the first template instantiation ... involves noexcept" [stackoverflow], therefore
    it could get triggered from seemingly random places, depending on user code.
@@ -52,15 +51,15 @@
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Apply all the extensions translators from a list
 // Return true if one of the translators completed without raising an exception
 // itself. Return of false indicates that if there are other translators
 // available, they should be tried.
-inline bool apply_exception_translators(std::forward_list<ExceptionTranslator>& translators) {
+inline bool apply_exception_translators(std::forward_list<ExceptionTranslator> &translators) {
     auto last_exception = std::current_exception();
 
     for (auto &translator : translators) {
         try {
             translator(last_exception);
             return true;
         } catch (...) {
@@ -79,291 +78,334 @@
 PYBIND11_NAMESPACE_END(detail)
 
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(std::nullptr_t) { }
+    cpp_function(std::nullptr_t) {}
 
     /// Construct a cpp_function from a vanilla function pointer
     template <typename Return, typename... Args, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Return (*f)(Args...), const Extra&... extra) {
+    cpp_function(Return (*f)(Args...), const Extra &...extra) {
         initialize(f, f, extra...);
     }
 
     /// Construct a cpp_function from a lambda function (possibly with internal state)
-    template <typename Func, typename... Extra,
+    template <typename Func,
+              typename... Extra,
               typename = detail::enable_if_t<detail::is_lambda<Func>::value>>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Func &&f, const Extra&... extra) {
-        initialize(std::forward<Func>(f),
-                   (detail::function_signature_t<Func> *) nullptr, extra...);
+    cpp_function(Func &&f, const Extra &...extra) {
+        initialize(
+            std::forward<Func>(f), (detail::function_signature_t<Func> *) nullptr, extra...);
     }
 
     /// Construct a cpp_function from a class method (non-const, no ref-qualifier)
     template <typename Return, typename Class, typename... Arg, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Return (Class::*f)(Arg...), const Extra&... extra) {
-        initialize([f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
-                   (Return (*) (Class *, Arg...)) nullptr, extra...);
+    cpp_function(Return (Class::*f)(Arg...), const Extra &...extra) {
+        initialize(
+            [f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
+            (Return(*)(Class *, Arg...)) nullptr,
+            extra...);
     }
 
     /// Construct a cpp_function from a class method (non-const, lvalue ref-qualifier)
     /// A copy of the overload for non-const functions without explicit ref-qualifier
     /// but with an added `&`.
     template <typename Return, typename Class, typename... Arg, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Return (Class::*f)(Arg...)&, const Extra&... extra) {
-        initialize([f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
-                   (Return (*) (Class *, Arg...)) nullptr, extra...);
+    cpp_function(Return (Class::*f)(Arg...) &, const Extra &...extra) {
+        initialize(
+            [f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
+            (Return(*)(Class *, Arg...)) nullptr,
+            extra...);
     }
 
     /// Construct a cpp_function from a class method (const, no ref-qualifier)
     template <typename Return, typename Class, typename... Arg, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Return (Class::*f)(Arg...) const, const Extra&... extra) {
-        initialize([f](const Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
-                   (Return (*)(const Class *, Arg ...)) nullptr, extra...);
+    cpp_function(Return (Class::*f)(Arg...) const, const Extra &...extra) {
+        initialize([f](const Class *c,
+                       Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
+                   (Return(*)(const Class *, Arg...)) nullptr,
+                   extra...);
     }
 
     /// Construct a cpp_function from a class method (const, lvalue ref-qualifier)
     /// A copy of the overload for const functions without explicit ref-qualifier
     /// but with an added `&`.
     template <typename Return, typename Class, typename... Arg, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    cpp_function(Return (Class::*f)(Arg...) const&, const Extra&... extra) {
-        initialize([f](const Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
-                   (Return (*)(const Class *, Arg ...)) nullptr, extra...);
+    cpp_function(Return (Class::*f)(Arg...) const &, const Extra &...extra) {
+        initialize([f](const Class *c,
+                       Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
+                   (Return(*)(const Class *, Arg...)) nullptr,
+                   extra...);
     }
 
     /// Return the function name
     object name() const { return attr("__name__"); }
 
 protected:
     struct InitializingFunctionRecordDeleter {
         // `destruct(function_record, false)`: `initialize_generic` copies strings and
         // takes care of cleaning up in case of exceptions. So pass `false` to `free_strings`.
-        void operator()(detail::function_record * rec) { destruct(rec, false); }
+        void operator()(detail::function_record *rec) { destruct(rec, false); }
     };
-    using unique_function_record = std::unique_ptr<detail::function_record, InitializingFunctionRecordDeleter>;
+    using unique_function_record
+        = std::unique_ptr<detail::function_record, InitializingFunctionRecordDeleter>;
 
     /// Space optimization: don't inline this frequently instantiated fragment
     PYBIND11_NOINLINE unique_function_record make_function_record() {
         return unique_function_record(new detail::function_record());
     }
 
     /// Special internal constructor for functors, lambda functions, etc.
     template <typename Func, typename Return, typename... Args, typename... Extra>
-    void initialize(Func &&f, Return (*)(Args...), const Extra&... extra) {
+    void initialize(Func &&f, Return (*)(Args...), const Extra &...extra) {
         using namespace detail;
-        struct capture { remove_reference_t<Func> f; };
+        struct capture {
+            remove_reference_t<Func> f;
+        };
 
-        /* Store the function including any extra state it might have (e.g. a lambda capture object) */
+        /* Store the function including any extra state it might have (e.g. a lambda capture
+         * object) */
         // The unique_ptr makes sure nothing is leaked in case of an exception.
         auto unique_rec = make_function_record();
-        auto rec = unique_rec.get();
+        auto *rec = unique_rec.get();
 
         /* Store the capture object directly in the function record if there is enough space */
         if (PYBIND11_SILENCE_MSVC_C4127(sizeof(capture) <= sizeof(rec->data))) {
             /* Without these pragmas, GCC warns that there might not be
                enough space to use the placement new operator. However, the
                'if' statement above ensures that this is the case. */
 #if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#  pragma GCC diagnostic push
-#  pragma GCC diagnostic ignored "-Wplacement-new"
+#    pragma GCC diagnostic push
+#    pragma GCC diagnostic ignored "-Wplacement-new"
 #endif
-            new ((capture *) &rec->data) capture { std::forward<Func>(f) };
+            new ((capture *) &rec->data) capture{std::forward<Func>(f)};
 #if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#  pragma GCC diagnostic pop
+#    pragma GCC diagnostic pop
 #endif
 #if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#  pragma GCC diagnostic push
-#  pragma GCC diagnostic ignored "-Wstrict-aliasing"
+#    pragma GCC diagnostic push
+#    pragma GCC diagnostic ignored "-Wstrict-aliasing"
 #endif
             // UB without std::launder, but without breaking ABI and/or
             // a significant refactoring it's "impossible" to solve.
-            if (!std::is_trivially_destructible<capture>::value)
+            if (!std::is_trivially_destructible<capture>::value) {
                 rec->free_data = [](function_record *r) {
                     auto data = PYBIND11_STD_LAUNDER((capture *) &r->data);
                     (void) data;
                     data->~capture();
                 };
+            }
 #if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#  pragma GCC diagnostic pop
+#    pragma GCC diagnostic pop
 #endif
         } else {
-            rec->data[0] = new capture { std::forward<Func>(f) };
+            rec->data[0] = new capture{std::forward<Func>(f)};
             rec->free_data = [](function_record *r) { delete ((capture *) r->data[0]); };
         }
 
         /* Type casters for the function arguments and return value */
         using cast_in = argument_loader<Args...>;
-        using cast_out = make_caster<
-            conditional_t<std::is_void<Return>::value, void_type, Return>
-        >;
+        using cast_out
+            = make_caster<conditional_t<std::is_void<Return>::value, void_type, Return>>;
 
-        static_assert(expected_num_args<Extra...>(sizeof...(Args), cast_in::args_pos >= 0, cast_in::has_kwargs),
-                      "The number of argument annotations does not match the number of function arguments");
+        static_assert(
+            expected_num_args<Extra...>(
+                sizeof...(Args), cast_in::args_pos >= 0, cast_in::has_kwargs),
+            "The number of argument annotations does not match the number of function arguments");
 
         /* Dispatch code which converts function arguments and performs the actual function call */
         rec->impl = [](function_call &call) -> handle {
             cast_in args_converter;
 
             /* Try to cast the function arguments into the C++ domain */
-            if (!args_converter.load_args(call))
+            if (!args_converter.load_args(call)) {
                 return PYBIND11_TRY_NEXT_OVERLOAD;
+            }
 
             /* Invoke call policy pre-call hook */
             process_attributes<Extra...>::precall(call);
 
             /* Get a pointer to the capture object */
-            auto data = (sizeof(capture) <= sizeof(call.func.data)
-                         ? &call.func.data : call.func.data[0]);
+            const auto *data = (sizeof(capture) <= sizeof(call.func.data) ? &call.func.data
+                                                                          : call.func.data[0]);
             auto *cap = const_cast<capture *>(reinterpret_cast<const capture *>(data));
 
             /* Override policy for rvalues -- usually to enforce rvp::move on an rvalue */
-            return_value_policy policy = return_value_policy_override<Return>::policy(call.func.policy);
+            return_value_policy policy
+                = return_value_policy_override<Return>::policy(call.func.policy);
 
             /* Function scope guard -- defaults to the compile-to-nothing `void_type` */
             using Guard = extract_guard_t<Extra...>;
 
             /* Perform the function call */
-            handle result = cast_out::cast(
-                std::move(args_converter).template call<Return, Guard>(cap->f), policy, call.parent);
+            handle result
+                = cast_out::cast(std::move(args_converter).template call<Return, Guard>(cap->f),
+                                 policy,
+                                 call.parent);
 
             /* Invoke call policy post-call hook */
             process_attributes<Extra...>::postcall(call, result);
 
             return result;
         };
 
         rec->nargs_pos = cast_in::args_pos >= 0
-            ? static_cast<std::uint16_t>(cast_in::args_pos)
-            : sizeof...(Args) - cast_in::has_kwargs; // Will get reduced more if we have a kw_only
+                             ? static_cast<std::uint16_t>(cast_in::args_pos)
+                             : sizeof...(Args) - cast_in::has_kwargs; // Will get reduced more if
+                                                                      // we have a kw_only
         rec->has_args = cast_in::args_pos >= 0;
         rec->has_kwargs = cast_in::has_kwargs;
 
         /* Process any user-provided function attributes */
         process_attributes<Extra...>::init(extra..., rec);
 
         {
             constexpr bool has_kw_only_args = any_of<std::is_same<kw_only, Extra>...>::value,
                            has_pos_only_args = any_of<std::is_same<pos_only, Extra>...>::value,
                            has_arg_annotations = any_of<is_keyword<Extra>...>::value;
-            static_assert(has_arg_annotations || !has_kw_only_args, "py::kw_only requires the use of argument annotations");
-            static_assert(has_arg_annotations || !has_pos_only_args, "py::pos_only requires the use of argument annotations (for docstrings and aligning the annotations to the argument)");
-
-            static_assert(constexpr_sum(is_kw_only<Extra>::value...) <= 1, "py::kw_only may be specified only once");
-            static_assert(constexpr_sum(is_pos_only<Extra>::value...) <= 1, "py::pos_only may be specified only once");
+            static_assert(has_arg_annotations || !has_kw_only_args,
+                          "py::kw_only requires the use of argument annotations");
+            static_assert(has_arg_annotations || !has_pos_only_args,
+                          "py::pos_only requires the use of argument annotations (for docstrings "
+                          "and aligning the annotations to the argument)");
+
+            static_assert(constexpr_sum(is_kw_only<Extra>::value...) <= 1,
+                          "py::kw_only may be specified only once");
+            static_assert(constexpr_sum(is_pos_only<Extra>::value...) <= 1,
+                          "py::pos_only may be specified only once");
             constexpr auto kw_only_pos = constexpr_first<is_kw_only, Extra...>();
             constexpr auto pos_only_pos = constexpr_first<is_pos_only, Extra...>();
-            static_assert(!(has_kw_only_args && has_pos_only_args) || pos_only_pos < kw_only_pos, "py::pos_only must come before py::kw_only");
+            static_assert(!(has_kw_only_args && has_pos_only_args) || pos_only_pos < kw_only_pos,
+                          "py::pos_only must come before py::kw_only");
         }
 
-        /* Generate a readable signature describing the function's arguments and return value types */
-        static constexpr auto signature = const_name("(") + cast_in::arg_names + const_name(") -> ") + cast_out::name;
+        /* Generate a readable signature describing the function's arguments and return
+           value types */
+        static constexpr auto signature
+            = const_name("(") + cast_in::arg_names + const_name(") -> ") + cast_out::name;
         PYBIND11_DESCR_CONSTEXPR auto types = decltype(signature)::types();
 
         /* Register the function with Python from generic (non-templated) code */
         // Pass on the ownership over the `unique_rec` to `initialize_generic`. `rec` stays valid.
         initialize_generic(std::move(unique_rec), signature.text, types.data(), sizeof...(Args));
 
         /* Stash some additional information used by an important optimization in 'functional.h' */
         using FunctionType = Return (*)(Args...);
-        constexpr bool is_function_ptr =
-            std::is_convertible<Func, FunctionType>::value &&
-            sizeof(capture) == sizeof(void *);
+        constexpr bool is_function_ptr
+            = std::is_convertible<Func, FunctionType>::value && sizeof(capture) == sizeof(void *);
         if (is_function_ptr) {
             rec->is_stateless = true;
-            rec->data[1] = const_cast<void *>(reinterpret_cast<const void *>(&typeid(FunctionType)));
+            rec->data[1]
+                = const_cast<void *>(reinterpret_cast<const void *>(&typeid(FunctionType)));
         }
     }
 
-    // Utility class that keeps track of all duplicated strings, and cleans them up in its destructor,
-    // unless they are released. Basically a RAII-solution to deal with exceptions along the way.
+    // Utility class that keeps track of all duplicated strings, and cleans them up in its
+    // destructor, unless they are released. Basically a RAII-solution to deal with exceptions
+    // along the way.
     class strdup_guard {
     public:
         ~strdup_guard() {
-            for (auto s : strings)
+            for (auto *s : strings) {
                 std::free(s);
+            }
         }
         char *operator()(const char *s) {
-            auto t = PYBIND11_COMPAT_STRDUP(s);
+            auto *t = PYBIND11_COMPAT_STRDUP(s);
             strings.push_back(t);
             return t;
         }
-        void release() {
-            strings.clear();
-        }
+        void release() { strings.clear(); }
+
     private:
         std::vector<char *> strings;
     };
 
     /// Register a function call with Python (generic non-templated code goes here)
-    void initialize_generic(unique_function_record &&unique_rec, const char *text,
-                            const std::type_info *const *types, size_t args) {
+    void initialize_generic(unique_function_record &&unique_rec,
+                            const char *text,
+                            const std::type_info *const *types,
+                            size_t args) {
         // Do NOT receive `unique_rec` by value. If this function fails to move out the unique_ptr,
-        // we do not want this to destuct the pointer. `initialize` (the caller) still relies on the
-        // pointee being alive after this call. Only move out if a `capsule` is going to keep it alive.
-        auto rec = unique_rec.get();
+        // we do not want this to destruct the pointer. `initialize` (the caller) still relies on
+        // the pointee being alive after this call. Only move out if a `capsule` is going to keep
+        // it alive.
+        auto *rec = unique_rec.get();
 
         // Keep track of strdup'ed strings, and clean them up as long as the function's capsule
         // has not taken ownership yet (when `unique_rec.release()` is called).
-        // Note: This cannot easily be fixed by a `unique_ptr` with custom deleter, because the strings
-        // are only referenced before strdup'ing. So only *after* the following block could `destruct`
-        // safely be called, but even then, `repr` could still throw in the middle of copying all strings.
+        // Note: This cannot easily be fixed by a `unique_ptr` with custom deleter, because the
+        // strings are only referenced before strdup'ing. So only *after* the following block could
+        // `destruct` safely be called, but even then, `repr` could still throw in the middle of
+        // copying all strings.
         strdup_guard guarded_strdup;
 
         /* Create copies of all referenced C-style strings */
         rec->name = guarded_strdup(rec->name ? rec->name : "");
-        if (rec->doc) rec->doc = guarded_strdup(rec->doc);
-        for (auto &a: rec->args) {
-            if (a.name)
+        if (rec->doc) {
+            rec->doc = guarded_strdup(rec->doc);
+        }
+        for (auto &a : rec->args) {
+            if (a.name) {
                 a.name = guarded_strdup(a.name);
-            if (a.descr)
+            }
+            if (a.descr) {
                 a.descr = guarded_strdup(a.descr);
-            else if (a.value)
+            } else if (a.value) {
                 a.descr = guarded_strdup(repr(a.value).cast<std::string>().c_str());
+            }
         }
 
         rec->is_constructor = (std::strcmp(rec->name, "__init__") == 0)
                               || (std::strcmp(rec->name, "__setstate__") == 0);
 
 #if !defined(NDEBUG) && !defined(PYBIND11_DISABLE_NEW_STYLE_INIT_WARNING)
         if (rec->is_constructor && !rec->is_new_style_constructor) {
-            const auto class_name = detail::get_fully_qualified_tp_name((PyTypeObject *) rec->scope.ptr());
+            const auto class_name
+                = detail::get_fully_qualified_tp_name((PyTypeObject *) rec->scope.ptr());
             const auto func_name = std::string(rec->name);
-            PyErr_WarnEx(
-                PyExc_FutureWarning,
-                ("pybind11-bound class '" + class_name + "' is using an old-style "
-                 "placement-new '" + func_name + "' which has been deprecated. See "
-                 "the upgrade guide in pybind11's docs. This message is only visible "
-                 "when compiled in debug mode.").c_str(), 0
-            );
+            PyErr_WarnEx(PyExc_FutureWarning,
+                         ("pybind11-bound class '" + class_name
+                          + "' is using an old-style "
+                            "placement-new '"
+                          + func_name
+                          + "' which has been deprecated. See "
+                            "the upgrade guide in pybind11's docs. This message is only visible "
+                            "when compiled in debug mode.")
+                             .c_str(),
+                         0);
         }
 #endif
 
         /* Generate a proper function signature */
         std::string signature;
         size_t type_index = 0, arg_index = 0;
         bool is_starred = false;
-        for (auto *pc = text; *pc != '\0'; ++pc) {
+        for (const auto *pc = text; *pc != '\0'; ++pc) {
             const auto c = *pc;
 
             if (c == '{') {
                 // Write arg name for everything except *args and **kwargs.
                 is_starred = *(pc + 1) == '*';
-                if (is_starred)
+                if (is_starred) {
                     continue;
+                }
                 // Separator for keyword-only arguments, placed before the kw
                 // arguments start (unless we are already putting an *args)
-                if (!rec->has_args && arg_index == rec->nargs_pos)
+                if (!rec->has_args && arg_index == rec->nargs_pos) {
                     signature += "*, ";
+                }
                 if (arg_index < rec->args.size() && rec->args[arg_index].name) {
                     signature += rec->args[arg_index].name;
                 } else if (arg_index == 0 && rec->is_method) {
                     signature += "self";
                 } else {
                     signature += "arg" + std::to_string(arg_index - (rec->is_method ? 1 : 0));
                 }
@@ -372,133 +414,147 @@
                 // Write default value if available.
                 if (!is_starred && arg_index < rec->args.size() && rec->args[arg_index].descr) {
                     signature += " = ";
                     signature += rec->args[arg_index].descr;
                 }
                 // Separator for positional-only arguments (placed after the
                 // argument, rather than before like *
-                if (rec->nargs_pos_only > 0 && (arg_index + 1) == rec->nargs_pos_only)
+                if (rec->nargs_pos_only > 0 && (arg_index + 1) == rec->nargs_pos_only) {
                     signature += ", /";
-                if (!is_starred)
+                }
+                if (!is_starred) {
                     arg_index++;
+                }
             } else if (c == '%') {
                 const std::type_info *t = types[type_index++];
-                if (!t)
+                if (!t) {
                     pybind11_fail("Internal error while parsing type signature (1)");
-                if (auto tinfo = detail::get_type_info(*t)) {
+                }
+                if (auto *tinfo = detail::get_type_info(*t)) {
                     handle th((PyObject *) tinfo->type);
-                    signature +=
-                        th.attr("__module__").cast<std::string>() + "." +
-                        th.attr("__qualname__").cast<std::string>(); // Python 3.3+, but we backport it to earlier versions
+                    signature += th.attr("__module__").cast<std::string>() + "." +
+                                 // Python 3.3+, but we backport it to earlier versions
+                                 th.attr("__qualname__").cast<std::string>();
                 } else if (rec->is_new_style_constructor && arg_index == 0) {
                     // A new-style `__init__` takes `self` as `value_and_holder`.
                     // Rewrite it to the proper class type.
-                    signature +=
-                        rec->scope.attr("__module__").cast<std::string>() + "." +
-                        rec->scope.attr("__qualname__").cast<std::string>();
+                    signature += rec->scope.attr("__module__").cast<std::string>() + "."
+                                 + rec->scope.attr("__qualname__").cast<std::string>();
                 } else {
                     std::string tname(t->name());
                     detail::clean_type_id(tname);
                     signature += tname;
                 }
             } else {
                 signature += c;
             }
         }
 
-        if (arg_index != args - rec->has_args - rec->has_kwargs || types[type_index] != nullptr)
+        if (arg_index != args - rec->has_args - rec->has_kwargs || types[type_index] != nullptr) {
             pybind11_fail("Internal error while parsing type signature (2)");
+        }
 
 #if PY_MAJOR_VERSION < 3
         if (std::strcmp(rec->name, "__next__") == 0) {
             std::free(rec->name);
             rec->name = guarded_strdup("next");
         } else if (std::strcmp(rec->name, "__bool__") == 0) {
             std::free(rec->name);
             rec->name = guarded_strdup("__nonzero__");
         }
 #endif
         rec->signature = guarded_strdup(signature.c_str());
         rec->args.shrink_to_fit();
         rec->nargs = (std::uint16_t) args;
 
-        if (rec->sibling && PYBIND11_INSTANCE_METHOD_CHECK(rec->sibling.ptr()))
+        if (rec->sibling && PYBIND11_INSTANCE_METHOD_CHECK(rec->sibling.ptr())) {
             rec->sibling = PYBIND11_INSTANCE_METHOD_GET_FUNCTION(rec->sibling.ptr());
+        }
 
         detail::function_record *chain = nullptr, *chain_start = rec;
         if (rec->sibling) {
             if (PyCFunction_Check(rec->sibling.ptr())) {
                 auto *self = PyCFunction_GET_SELF(rec->sibling.ptr());
-                capsule rec_capsule = isinstance<capsule>(self) ? reinterpret_borrow<capsule>(self) : capsule(self);
+                capsule rec_capsule = isinstance<capsule>(self) ? reinterpret_borrow<capsule>(self)
+                                                                : capsule(self);
                 chain = (detail::function_record *) rec_capsule;
                 /* Never append a method to an overload chain of a parent class;
                    instead, hide the parent's overloads in this case */
-                if (!chain->scope.is(rec->scope))
+                if (!chain->scope.is(rec->scope)) {
                     chain = nullptr;
+                }
+            }
+            // Don't trigger for things like the default __init__, which are wrapper_descriptors
+            // that we are intentionally replacing
+            else if (!rec->sibling.is_none() && rec->name[0] != '_') {
+                pybind11_fail("Cannot overload existing non-function object \""
+                              + std::string(rec->name) + "\" with a function of the same name");
             }
-            // Don't trigger for things like the default __init__, which are wrapper_descriptors that we are intentionally replacing
-            else if (!rec->sibling.is_none() && rec->name[0] != '_')
-                pybind11_fail("Cannot overload existing non-function object \"" + std::string(rec->name) +
-                        "\" with a function of the same name");
         }
 
         if (!chain) {
             /* No existing overload was found, create a new function object */
             rec->def = new PyMethodDef();
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
             rec->def->ml_meth
                 = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
-            capsule rec_capsule(unique_rec.release(), [](void *ptr) {
-                destruct((detail::function_record *) ptr);
-            });
+            capsule rec_capsule(unique_rec.release(),
+                                [](void *ptr) { destruct((detail::function_record *) ptr); });
             guarded_strdup.release();
 
             object scope_module;
             if (rec->scope) {
                 if (hasattr(rec->scope, "__module__")) {
                     scope_module = rec->scope.attr("__module__");
                 } else if (hasattr(rec->scope, "__name__")) {
                     scope_module = rec->scope.attr("__name__");
                 }
             }
 
             m_ptr = PyCFunction_NewEx(rec->def, rec_capsule.ptr(), scope_module.ptr());
-            if (!m_ptr)
+            if (!m_ptr) {
                 pybind11_fail("cpp_function::cpp_function(): Could not allocate function object");
+            }
         } else {
             /* Append at the beginning or end of the overload chain */
             m_ptr = rec->sibling.ptr();
             inc_ref();
-            if (chain->is_method != rec->is_method)
-                pybind11_fail("overloading a method with both static and instance methods is not supported; "
-                    #if defined(NDEBUG)
-                        "compile in debug mode for more details"
-                    #else
-                        "error while attempting to bind " + std::string(rec->is_method ? "instance" : "static") + " method " +
-                        std::string(pybind11::str(rec->scope.attr("__name__"))) + "." + std::string(rec->name) + signature
-                    #endif
+            if (chain->is_method != rec->is_method) {
+                pybind11_fail(
+                    "overloading a method with both static and instance methods is not supported; "
+#if defined(NDEBUG)
+                    "compile in debug mode for more details"
+#else
+                    "error while attempting to bind "
+                    + std::string(rec->is_method ? "instance" : "static") + " method "
+                    + std::string(pybind11::str(rec->scope.attr("__name__"))) + "."
+                    + std::string(rec->name) + signature
+#endif
                 );
+            }
 
             if (rec->prepend) {
                 // Beginning of chain; we need to replace the capsule's current head-of-the-chain
                 // pointer with this one, then make this one point to the previous head of the
                 // chain.
                 chain_start = rec;
                 rec->next = chain;
-                auto rec_capsule = reinterpret_borrow<capsule>(((PyCFunctionObject *) m_ptr)->m_self);
+                auto rec_capsule
+                    = reinterpret_borrow<capsule>(((PyCFunctionObject *) m_ptr)->m_self);
                 rec_capsule.set_pointer(unique_rec.release());
                 guarded_strdup.release();
             } else {
                 // Or end of chain (normal behavior)
                 chain_start = chain;
-                while (chain->next)
+                while (chain->next) {
                     chain = chain->next;
+                }
                 chain->next = unique_rec.release();
                 guarded_strdup.release();
             }
         }
 
         std::string signatures;
         int index = 0;
@@ -508,124 +564,143 @@
             // First a generic signature
             signatures += rec->name;
             signatures += "(*args, **kwargs)\n";
             signatures += "Overloaded function.\n\n";
         }
         // Then specific overload signatures
         bool first_user_def = true;
-        for (auto it = chain_start; it != nullptr; it = it->next) {
+        for (auto *it = chain_start; it != nullptr; it = it->next) {
             if (options::show_function_signatures()) {
-                if (index > 0) signatures += "\n";
-                if (chain)
+                if (index > 0) {
+                    signatures += "\n";
+                }
+                if (chain) {
                     signatures += std::to_string(++index) + ". ";
+                }
                 signatures += rec->name;
                 signatures += it->signature;
                 signatures += "\n";
             }
             if (it->doc && it->doc[0] != '\0' && options::show_user_defined_docstrings()) {
-                // If we're appending another docstring, and aren't printing function signatures, we
-                // need to append a newline first:
+                // If we're appending another docstring, and aren't printing function signatures,
+                // we need to append a newline first:
                 if (!options::show_function_signatures()) {
-                    if (first_user_def) first_user_def = false;
-                    else signatures += "\n";
+                    if (first_user_def) {
+                        first_user_def = false;
+                    } else {
+                        signatures += "\n";
+                    }
+                }
+                if (options::show_function_signatures()) {
+                    signatures += "\n";
                 }
-                if (options::show_function_signatures()) signatures += "\n";
                 signatures += it->doc;
-                if (options::show_function_signatures()) signatures += "\n";
+                if (options::show_function_signatures()) {
+                    signatures += "\n";
+                }
             }
         }
 
         /* Install docstring */
         auto *func = (PyCFunctionObject *) m_ptr;
         std::free(const_cast<char *>(func->m_ml->ml_doc));
         // Install docstring if it's non-empty (when at least one option is enabled)
         func->m_ml->ml_doc
             = signatures.empty() ? nullptr : PYBIND11_COMPAT_STRDUP(signatures.c_str());
 
         if (rec->is_method) {
             m_ptr = PYBIND11_INSTANCE_METHOD_NEW(m_ptr, rec->scope.ptr());
-            if (!m_ptr)
-                pybind11_fail("cpp_function::cpp_function(): Could not allocate instance method object");
+            if (!m_ptr) {
+                pybind11_fail(
+                    "cpp_function::cpp_function(): Could not allocate instance method object");
+            }
             Py_DECREF(func);
         }
     }
 
     /// When a cpp_function is GCed, release any memory allocated by pybind11
     static void destruct(detail::function_record *rec, bool free_strings = true) {
-        // If on Python 3.9, check the interpreter "MICRO" (patch) version.
-        // If this is running on 3.9.0, we have to work around a bug.
-        #if !defined(PYPY_VERSION) && PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION == 9
-            static bool is_zero = Py_GetVersion()[4] == '0';
-        #endif
+// If on Python 3.9, check the interpreter "MICRO" (patch) version.
+// If this is running on 3.9.0, we have to work around a bug.
+#if !defined(PYPY_VERSION) && PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION == 9
+        static bool is_zero = Py_GetVersion()[4] == '0';
+#endif
 
         while (rec) {
             detail::function_record *next = rec->next;
-            if (rec->free_data)
+            if (rec->free_data) {
                 rec->free_data(rec);
+            }
             // During initialization, these strings might not have been copied yet,
             // so they cannot be freed. Once the function has been created, they can.
             // Check `make_function_record` for more details.
             if (free_strings) {
                 std::free((char *) rec->name);
                 std::free((char *) rec->doc);
                 std::free((char *) rec->signature);
-                for (auto &arg: rec->args) {
+                for (auto &arg : rec->args) {
                     std::free(const_cast<char *>(arg.name));
                     std::free(const_cast<char *>(arg.descr));
                 }
             }
-            for (auto &arg: rec->args)
+            for (auto &arg : rec->args) {
                 arg.value.dec_ref();
+            }
             if (rec->def) {
                 std::free(const_cast<char *>(rec->def->ml_doc));
-                // Python 3.9.0 decref's these in the wrong order; rec->def
-                // If loaded on 3.9.0, let these leak (use Python 3.9.1 at runtime to fix)
-                // See https://github.com/python/cpython/pull/22670
-                #if !defined(PYPY_VERSION) && PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION == 9
-                    if (!is_zero)
-                        delete rec->def;
-                #else
+// Python 3.9.0 decref's these in the wrong order; rec->def
+// If loaded on 3.9.0, let these leak (use Python 3.9.1 at runtime to fix)
+// See https://github.com/python/cpython/pull/22670
+#if !defined(PYPY_VERSION) && PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION == 9
+                if (!is_zero) {
                     delete rec->def;
-                #endif
+                }
+#else
+                delete rec->def;
+#endif
             }
             delete rec;
             rec = next;
         }
     }
 
-
     /// Main dispatch logic for calls to functions bound using pybind11
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
 
         /* Iterator over the list of potentially admissible overloads */
         const function_record *overloads = (function_record *) PyCapsule_GetPointer(self, nullptr),
                               *it = overloads;
 
-        /* Need to know how many arguments + keyword arguments there are to pick the right overload */
+        /* Need to know how many arguments + keyword arguments there are to pick the right
+           overload */
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
 
         auto self_value_and_holder = value_and_holder();
         if (overloads->is_constructor) {
-            if (!parent || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
-                PyErr_SetString(PyExc_TypeError, "__init__(self, ...) called with invalid or missing `self` argument");
+            if (!parent
+                || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
+                PyErr_SetString(
+                    PyExc_TypeError,
+                    "__init__(self, ...) called with invalid or missing `self` argument");
                 return nullptr;
             }
 
-            const auto tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
-            const auto pi = reinterpret_cast<instance *>(parent.ptr());
+            auto *const tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
+            auto *const pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder = pi->get_value_and_holder(tinfo, true);
 
             // If this value is already registered it must mean __init__ is invoked multiple times;
             // we really can't support that in C++, so just ignore the second __init__.
-            if (self_value_and_holder.instance_registered())
+            if (self_value_and_holder.instance_registered()) {
                 return none().release().ptr();
+            }
         }
 
         try {
             // We do this in two passes: in the first pass, we load arguments with `convert=false`;
             // in the second, we allow conversion (except for arguments with an explicit
             // py::arg().noconvert()).  This lets us prefer calls without conversion, with
             // conversion as a fallback.
@@ -636,78 +711,90 @@
 
             for (; it != nullptr; it = it->next) {
 
                 /* For each overload:
                    1. Copy all positional arguments we were given, also checking to make sure that
                       named positional arguments weren't *also* specified via kwarg.
                    2. If we weren't given enough, try to make up the omitted ones by checking
-                      whether they were provided by a kwarg matching the `py::arg("name")` name.  If
+                      whether they were provided by a kwarg matching the `py::arg("name")` name. If
                       so, use it (and remove it from kwargs); if not, see if the function binding
                       provided a default that we can use.
-                   3. Ensure that either all keyword arguments were "consumed", or that the function
-                      takes a kwargs argument to accept unconsumed kwargs.
+                   3. Ensure that either all keyword arguments were "consumed", or that the
+                   function takes a kwargs argument to accept unconsumed kwargs.
                    4. Any positional arguments still left get put into a tuple (for args), and any
                       leftover kwargs get put into a dict.
                    5. Pack everything into a vector; if we have py::args or py::kwargs, they are an
                       extra tuple or dict at the end of the positional arguments.
                    6. Call the function call dispatcher (function_record::impl)
 
-                   If one of these fail, move on to the next overload and keep trying until we get a
-                   result other than PYBIND11_TRY_NEXT_OVERLOAD.
+                   If one of these fail, move on to the next overload and keep trying until we get
+                   a result other than PYBIND11_TRY_NEXT_OVERLOAD.
                  */
 
                 const function_record &func = *it;
-                size_t num_args = func.nargs;    // Number of positional arguments that we need
-                if (func.has_args) --num_args;   // (but don't count py::args
-                if (func.has_kwargs) --num_args; //  or py::kwargs)
+                size_t num_args = func.nargs; // Number of positional arguments that we need
+                if (func.has_args) {
+                    --num_args; // (but don't count py::args
+                }
+                if (func.has_kwargs) {
+                    --num_args; //  or py::kwargs)
+                }
                 size_t pos_args = func.nargs_pos;
 
-                if (!func.has_args && n_args_in > pos_args)
+                if (!func.has_args && n_args_in > pos_args) {
                     continue; // Too many positional arguments for this overload
+                }
 
-                if (n_args_in < pos_args && func.args.size() < pos_args)
-                    continue; // Not enough positional arguments given, and not enough defaults to fill in the blanks
+                if (n_args_in < pos_args && func.args.size() < pos_args) {
+                    continue; // Not enough positional arguments given, and not enough defaults to
+                              // fill in the blanks
+                }
 
                 function_call call(func, parent);
 
-                size_t args_to_copy = (std::min)(pos_args, n_args_in); // Protect std::min with parentheses
+                // Protect std::min with parentheses
+                size_t args_to_copy = (std::min)(pos_args, n_args_in);
                 size_t args_copied = 0;
 
                 // 0. Inject new-style `self` argument
                 if (func.is_new_style_constructor) {
                     // The `value` may have been preallocated by an old-style `__init__`
                     // if it was a preceding candidate for overload resolution.
-                    if (self_value_and_holder)
+                    if (self_value_and_holder) {
                         self_value_and_holder.type->dealloc(self_value_and_holder);
+                    }
 
                     call.init_self = PyTuple_GET_ITEM(args_in, 0);
                     call.args.emplace_back(reinterpret_cast<PyObject *>(&self_value_and_holder));
                     call.args_convert.push_back(false);
                     ++args_copied;
                 }
 
                 // 1. Copy any position arguments given.
                 bool bad_arg = false;
                 for (; args_copied < args_to_copy; ++args_copied) {
-                    const argument_record *arg_rec = args_copied < func.args.size() ? &func.args[args_copied] : nullptr;
-                    if (kwargs_in && arg_rec && arg_rec->name && dict_getitemstring(kwargs_in, arg_rec->name)) {
+                    const argument_record *arg_rec
+                        = args_copied < func.args.size() ? &func.args[args_copied] : nullptr;
+                    if (kwargs_in && arg_rec && arg_rec->name
+                        && dict_getitemstring(kwargs_in, arg_rec->name)) {
                         bad_arg = true;
                         break;
                     }
 
                     handle arg(PyTuple_GET_ITEM(args_in, args_copied));
                     if (arg_rec && !arg_rec->none && arg.is_none()) {
                         bad_arg = true;
                         break;
                     }
                     call.args.push_back(arg);
                     call.args_convert.push_back(arg_rec ? arg_rec->convert : true);
                 }
-                if (bad_arg)
+                if (bad_arg) {
                     continue; // Maybe it was meant for another overload (issue #688)
+                }
 
                 // Keep track of how many position args we copied out in case we need to come back
                 // to copy the rest into a py::args argument.
                 size_t positional_args_copied = args_copied;
 
                 // We'll need to copy this if we steal some kwargs for defaults
                 dict kwargs = reinterpret_borrow<dict>(kwargs_in);
@@ -720,32 +807,35 @@
 
                         if (arg_rec.value) {
                             value = arg_rec.value;
                         }
                         if (value) {
                             call.args.push_back(value);
                             call.args_convert.push_back(arg_rec.convert);
-                        } else
+                        } else {
                             break;
+                        }
                     }
 
-                    if (args_copied < func.nargs_pos_only)
+                    if (args_copied < func.nargs_pos_only) {
                         continue; // Not enough defaults to fill the positional arguments
+                    }
                 }
 
                 // 2. Check kwargs and, failing that, defaults that may help complete the list
                 if (args_copied < num_args) {
                     bool copied_kwargs = false;
 
                     for (; args_copied < num_args; ++args_copied) {
                         const auto &arg_rec = func.args[args_copied];
 
                         handle value;
-                        if (kwargs_in && arg_rec.name)
+                        if (kwargs_in && arg_rec.name) {
                             value = dict_getitemstring(kwargs.ptr(), arg_rec.name);
+                        }
 
                         if (value) {
                             // Consume a kwargs value
                             if (!copied_kwargs) {
                                 kwargs = reinterpret_steal<dict>(PyDict_Copy(kwargs.ptr()));
                                 copied_kwargs = true;
                             }
@@ -757,32 +847,37 @@
                         }
 
                         if (!arg_rec.none && value.is_none()) {
                             break;
                         }
 
                         if (value) {
-                            // If we're at the py::args index then first insert a stub for it to be replaced later
-                            if (func.has_args && call.args.size() == func.nargs_pos)
+                            // If we're at the py::args index then first insert a stub for it to be
+                            // replaced later
+                            if (func.has_args && call.args.size() == func.nargs_pos) {
                                 call.args.push_back(none());
+                            }
 
                             call.args.push_back(value);
                             call.args_convert.push_back(arg_rec.convert);
-                        }
-                        else
+                        } else {
                             break;
+                        }
                     }
 
-                    if (args_copied < num_args)
-                        continue; // Not enough arguments, defaults, or kwargs to fill the positional arguments
+                    if (args_copied < num_args) {
+                        continue; // Not enough arguments, defaults, or kwargs to fill the
+                                  // positional arguments
+                    }
                 }
 
                 // 3. Check everything was consumed (unless we have a kwargs arg)
-                if (kwargs && !kwargs.empty() && !func.has_kwargs)
+                if (kwargs && !kwargs.empty() && !func.has_kwargs) {
                     continue; // Unconsumed kwargs, but no py::kwargs argument to accept them
+                }
 
                 // 4a. If we have a py::args argument, create a new tuple with leftovers
                 if (func.has_args) {
                     tuple extra_args;
                     if (args_to_copy == 0) {
                         // We didn't copy out any position arguments from the args_in tuple, so we
                         // can reuse it directly without copying:
@@ -792,37 +887,41 @@
                     } else {
                         size_t args_size = n_args_in - positional_args_copied;
                         extra_args = tuple(args_size);
                         for (size_t i = 0; i < args_size; ++i) {
                             extra_args[i] = PyTuple_GET_ITEM(args_in, positional_args_copied + i);
                         }
                     }
-                    if (call.args.size() <= func.nargs_pos)
+                    if (call.args.size() <= func.nargs_pos) {
                         call.args.push_back(extra_args);
-                    else
+                    } else {
                         call.args[func.nargs_pos] = extra_args;
+                    }
                     call.args_convert.push_back(false);
                     call.args_ref = std::move(extra_args);
                 }
 
                 // 4b. If we have a py::kwargs, pass on any remaining kwargs
                 if (func.has_kwargs) {
-                    if (!kwargs.ptr())
+                    if (!kwargs.ptr()) {
                         kwargs = dict(); // If we didn't get one, send an empty one
+                    }
                     call.args.push_back(kwargs);
                     call.args_convert.push_back(false);
                     call.kwargs_ref = std::move(kwargs);
                 }
 
-                // 5. Put everything in a vector.  Not technically step 5, we've been building it
-                // in `call.args` all along.
-                #if !defined(NDEBUG)
-                if (call.args.size() != func.nargs || call.args_convert.size() != func.nargs)
-                    pybind11_fail("Internal error: function call dispatcher inserted wrong number of arguments!");
-                #endif
+// 5. Put everything in a vector.  Not technically step 5, we've been building it
+// in `call.args` all along.
+#if !defined(NDEBUG)
+                if (call.args.size() != func.nargs || call.args_convert.size() != func.nargs) {
+                    pybind11_fail("Internal error: function call dispatcher inserted wrong number "
+                                  "of arguments!");
+                }
+#endif
 
                 std::vector<bool> second_pass_convert;
                 if (overloaded) {
                     // We're in the first no-convert pass, so swap out the conversion flags for a
                     // set of all-false flags.  If the call fails, we'll swap the flags back in for
                     // the conversion-allowed call below.
                     second_pass_convert.resize(func.nargs, false);
@@ -833,16 +932,17 @@
                 try {
                     loader_life_support guard{};
                     result = func.impl(call);
                 } catch (reference_cast_error &) {
                     result = PYBIND11_TRY_NEXT_OVERLOAD;
                 }
 
-                if (result.ptr() != PYBIND11_TRY_NEXT_OVERLOAD)
+                if (result.ptr() != PYBIND11_TRY_NEXT_OVERLOAD) {
                     break;
+                }
 
                 if (overloaded) {
                     // The (overloaded) call failed; if the call has at least one argument that
                     // permits conversion (i.e. it hasn't been explicitly specified `.noconvert()`)
                     // then add this call to the list of second pass overloads to try.
                     for (size_t i = func.is_method ? 1 : 0; i < pos_args; i++) {
                         if (second_pass_convert[i]) {
@@ -853,37 +953,39 @@
                             break;
                         }
                     }
                 }
             }
 
             if (overloaded && !second_pass.empty() && result.ptr() == PYBIND11_TRY_NEXT_OVERLOAD) {
-                // The no-conversion pass finished without success, try again with conversion allowed
+                // The no-conversion pass finished without success, try again with conversion
+                // allowed
                 for (auto &call : second_pass) {
                     try {
                         loader_life_support guard{};
                         result = call.func.impl(call);
                     } catch (reference_cast_error &) {
                         result = PYBIND11_TRY_NEXT_OVERLOAD;
                     }
 
                     if (result.ptr() != PYBIND11_TRY_NEXT_OVERLOAD) {
                         // The error reporting logic below expects 'it' to be valid, as it would be
                         // if we'd encountered this failure in the first-pass loop.
-                        if (!result)
+                        if (!result) {
                             it = &call.func;
+                        }
                         break;
                     }
                 }
             }
         } catch (error_already_set &e) {
             e.restore();
             return nullptr;
 #ifdef __GLIBCXX__
-        } catch ( abi::__forced_unwind& ) {
+        } catch (abi::__forced_unwind &) {
             throw;
 #endif
         } catch (...) {
             /* When an exception is caught, give each registered exception
                translator a chance to translate it to a Python exception. First
                all module-local translators will be tried in reverse order of
                registration. If none of the module-locale translators handle
@@ -892,99 +994,116 @@
                registration.
 
                A translator may choose to do one of the following:
 
                 - catch the exception and call PyErr_SetString or PyErr_SetObject
                   to set a standard (or custom) Python exception, or
                 - do nothing and let the exception fall through to the next translator, or
-                - delegate translation to the next translator by throwing a new type of exception. */
+                - delegate translation to the next translator by throwing a new type of exception.
+             */
 
-            auto &local_exception_translators = get_local_internals().registered_exception_translators;
+            auto &local_exception_translators
+                = get_local_internals().registered_exception_translators;
             if (detail::apply_exception_translators(local_exception_translators)) {
                 return nullptr;
             }
             auto &exception_translators = get_internals().registered_exception_translators;
             if (detail::apply_exception_translators(exception_translators)) {
                 return nullptr;
             }
 
-            PyErr_SetString(PyExc_SystemError, "Exception escaped from default exception translator!");
+            PyErr_SetString(PyExc_SystemError,
+                            "Exception escaped from default exception translator!");
             return nullptr;
         }
 
         auto append_note_if_missing_header_is_suspected = [](std::string &msg) {
             if (msg.find("std::") != std::string::npos) {
                 msg += "\n\n"
                        "Did you forget to `#include <pybind11/stl.h>`? Or <pybind11/complex.h>,\n"
                        "<pybind11/functional.h>, <pybind11/chrono.h>, etc. Some automatic\n"
                        "conversions are optional and require extra headers to be included\n"
                        "when compiling your pybind11 module.";
             }
         };
 
         if (result.ptr() == PYBIND11_TRY_NEXT_OVERLOAD) {
-            if (overloads->is_operator)
+            if (overloads->is_operator) {
                 return handle(Py_NotImplemented).inc_ref().ptr();
+            }
 
-            std::string msg = std::string(overloads->name) + "(): incompatible " +
-                std::string(overloads->is_constructor ? "constructor" : "function") +
-                " arguments. The following argument types are supported:\n";
+            std::string msg = std::string(overloads->name) + "(): incompatible "
+                              + std::string(overloads->is_constructor ? "constructor" : "function")
+                              + " arguments. The following argument types are supported:\n";
 
             int ctr = 0;
             for (const function_record *it2 = overloads; it2 != nullptr; it2 = it2->next) {
-                msg += "    "+ std::to_string(++ctr) + ". ";
+                msg += "    " + std::to_string(++ctr) + ". ";
 
                 bool wrote_sig = false;
                 if (overloads->is_constructor) {
-                    // For a constructor, rewrite `(self: Object, arg0, ...) -> NoneType` as `Object(arg0, ...)`
+                    // For a constructor, rewrite `(self: Object, arg0, ...) -> NoneType` as
+                    // `Object(arg0, ...)`
                     std::string sig = it2->signature;
                     size_t start = sig.find('(') + 7; // skip "(self: "
                     if (start < sig.size()) {
                         // End at the , for the next argument
                         size_t end = sig.find(", "), next = end + 2;
                         size_t ret = sig.rfind(" -> ");
                         // Or the ), if there is no comma:
-                        if (end >= sig.size()) next = end = sig.find(')');
+                        if (end >= sig.size()) {
+                            next = end = sig.find(')');
+                        }
                         if (start < end && next < sig.size()) {
                             msg.append(sig, start, end - start);
                             msg += '(';
                             msg.append(sig, next, ret - next);
                             wrote_sig = true;
                         }
                     }
                 }
-                if (!wrote_sig) msg += it2->signature;
+                if (!wrote_sig) {
+                    msg += it2->signature;
+                }
 
                 msg += "\n";
             }
             msg += "\nInvoked with: ";
             auto args_ = reinterpret_borrow<tuple>(args_in);
             bool some_args = false;
             for (size_t ti = overloads->is_constructor ? 1 : 0; ti < args_.size(); ++ti) {
-                if (!some_args) some_args = true;
-                else msg += ", ";
+                if (!some_args) {
+                    some_args = true;
+                } else {
+                    msg += ", ";
+                }
                 try {
                     msg += pybind11::repr(args_[ti]);
-                } catch (const error_already_set&) {
+                } catch (const error_already_set &) {
                     msg += "<repr raised Error>";
                 }
             }
             if (kwargs_in) {
                 auto kwargs = reinterpret_borrow<dict>(kwargs_in);
                 if (!kwargs.empty()) {
-                    if (some_args) msg += "; ";
+                    if (some_args) {
+                        msg += "; ";
+                    }
                     msg += "kwargs: ";
                     bool first = true;
                     for (auto kwarg : kwargs) {
-                        if (first) first = false;
-                        else msg += ", ";
+                        if (first) {
+                            first = false;
+                        } else {
+                            msg += ", ";
+                        }
                         msg += pybind11::str("{}=").format(kwarg.first);
                         try {
                             msg += pybind11::repr(kwarg.second);
-                        } catch (const error_already_set&) {
+                        } catch (const error_already_set &) {
                             msg += "<repr raised Error>";
                         }
                     }
                 }
             }
 
             append_note_if_missing_header_is_suspected(msg);
@@ -1018,15 +1137,14 @@
             auto *pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder.type->init_instance(pi, nullptr);
         }
         return result.ptr();
     }
 };
 
-
 /// Wrapper for Python extension modules
 class module_ : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(module_, object, PyModule_Check)
 
     /// Create a new top-level Python module with the given name and docstring
     PYBIND11_DEPRECATED("Use PYBIND11_MODULE or module_::create_extension_module instead")
@@ -1040,19 +1158,23 @@
 
     /** \rst
         Create Python binding for a new function within the module scope. ``Func``
         can be a plain C++ function, a function pointer, or a lambda function. For
         details on the ``Extra&& ... extra`` argument, see section :ref:`extras`.
     \endrst */
     template <typename Func, typename... Extra>
-    module_ &def(const char *name_, Func &&f, const Extra& ... extra) {
-        cpp_function func(std::forward<Func>(f), name(name_), scope(*this),
-                          sibling(getattr(*this, name_, none())), extra...);
+    module_ &def(const char *name_, Func &&f, const Extra &...extra) {
+        cpp_function func(std::forward<Func>(f),
+                          name(name_),
+                          scope(*this),
+                          sibling(getattr(*this, name_, none())),
+                          extra...);
         // NB: allow overwriting here because cpp_function sets up a chain with the intention of
-        // overwriting (and has already checked internally that it isn't overwriting non-functions).
+        // overwriting (and has already checked internally that it isn't overwriting
+        // non-functions).
         add_object(name_, func, true /* overwrite */);
         return *this;
     }
 
     /** \rst
         Create and return a new Python submodule with the given name and docstring.
         This also works recursively, i.e.
@@ -1060,50 +1182,55 @@
         .. code-block:: cpp
 
             py::module_ m("example", "pybind11 example plugin");
             py::module_ m2 = m.def_submodule("sub", "A submodule of 'example'");
             py::module_ m3 = m2.def_submodule("subsub", "A submodule of 'example.sub'");
     \endrst */
     module_ def_submodule(const char *name, const char *doc = nullptr) {
-        std::string full_name = std::string(PyModule_GetName(m_ptr))
-            + std::string(".") + std::string(name);
+        std::string full_name
+            = std::string(PyModule_GetName(m_ptr)) + std::string(".") + std::string(name);
         auto result = reinterpret_borrow<module_>(PyImport_AddModule(full_name.c_str()));
-        if (doc && options::show_user_defined_docstrings())
+        if (doc && options::show_user_defined_docstrings()) {
             result.attr("__doc__") = pybind11::str(doc);
+        }
         attr(name) = result;
         return result;
     }
 
     /// Import and return a module or throws `error_already_set`.
     static module_ import(const char *name) {
         PyObject *obj = PyImport_ImportModule(name);
-        if (!obj)
+        if (!obj) {
             throw error_already_set();
+        }
         return reinterpret_steal<module_>(obj);
     }
 
     /// Reload the module or throws `error_already_set`.
     void reload() {
         PyObject *obj = PyImport_ReloadModule(ptr());
-        if (!obj)
+        if (!obj) {
             throw error_already_set();
+        }
         *this = reinterpret_steal<module_>(obj);
     }
 
     /** \rst
         Adds an object to the module using the given name.  Throws if an object with the given name
         already exists.
 
-        ``overwrite`` should almost always be false: attempting to overwrite objects that pybind11 has
-        established will, in most cases, break things.
+        ``overwrite`` should almost always be false: attempting to overwrite objects that pybind11
+        has established will, in most cases, break things.
     \endrst */
     PYBIND11_NOINLINE void add_object(const char *name, handle obj, bool overwrite = false) {
-        if (!overwrite && hasattr(*this, name))
-            pybind11_fail("Error during initialization: multiple incompatible definitions with name \"" +
-                    std::string(name) + "\"");
+        if (!overwrite && hasattr(*this, name)) {
+            pybind11_fail(
+                "Error during initialization: multiple incompatible definitions with name \""
+                + std::string(name) + "\"");
+        }
 
         PyModule_AddObject(ptr(), name, obj.inc_ref().ptr() /* steals a reference */);
     }
 
 #if PY_MAJOR_VERSION >= 3
     using module_def = PyModuleDef;
 #else
@@ -1115,37 +1242,40 @@
 
         For Python 3, ``def`` should point to a statically allocated module_def.
         For Python 2, ``def`` can be a nullptr and is completely ignored.
     \endrst */
     static module_ create_extension_module(const char *name, const char *doc, module_def *def) {
 #if PY_MAJOR_VERSION >= 3
         // module_def is PyModuleDef
-        def = new (def) PyModuleDef {  // Placement new (not an allocation).
-            /* m_base */     PyModuleDef_HEAD_INIT,
-            /* m_name */     name,
-            /* m_doc */      options::show_user_defined_docstrings() ? doc : nullptr,
-            /* m_size */     -1,
-            /* m_methods */  nullptr,
-            /* m_slots */    nullptr,
-            /* m_traverse */ nullptr,
-            /* m_clear */    nullptr,
-            /* m_free */     nullptr
-        };
-        auto m = PyModule_Create(def);
+        // Placement new (not an allocation).
+        def = new (def)
+            PyModuleDef{/* m_base */ PyModuleDef_HEAD_INIT,
+                        /* m_name */ name,
+                        /* m_doc */ options::show_user_defined_docstrings() ? doc : nullptr,
+                        /* m_size */ -1,
+                        /* m_methods */ nullptr,
+                        /* m_slots */ nullptr,
+                        /* m_traverse */ nullptr,
+                        /* m_clear */ nullptr,
+                        /* m_free */ nullptr};
+        auto *m = PyModule_Create(def);
 #else
         // Ignore module_def *def; only necessary for Python 3
         (void) def;
-        auto m = Py_InitModule3(name, nullptr, options::show_user_defined_docstrings() ? doc : nullptr);
+        auto m = Py_InitModule3(
+            name, nullptr, options::show_user_defined_docstrings() ? doc : nullptr);
 #endif
         if (m == nullptr) {
-            if (PyErr_Occurred())
+            if (PyErr_Occurred()) {
                 throw error_already_set();
+            }
             pybind11_fail("Internal error in module_::create_extension_module()");
         }
-        // TODO: Should be reinterpret_steal for Python 3, but Python also steals it again when returned from PyInit_...
+        // TODO: Should be reinterpret_steal for Python 3, but Python also steals it again when
+        // returned from PyInit_...
         //       For Python 2, reinterpret_borrow is correct.
         return reinterpret_borrow<module_>(m);
     }
 };
 
 // When inside a namespace (or anywhere as long as it's not the first item on a line),
 // C++20 allows "module" to be used. This is provided for backward compatibility, and for
@@ -1157,37 +1287,40 @@
 /// or ``__main__.__dict__`` if there is no frame (usually when the interpreter is embedded).
 inline dict globals() {
     PyObject *p = PyEval_GetGlobals();
     return reinterpret_borrow<dict>(p ? p : module_::import("__main__").attr("__dict__").ptr());
 }
 
 #if PY_VERSION_HEX >= 0x03030000
-template <typename... Args,
-          typename = detail::enable_if_t<args_are_all_keyword_or_ds<Args...>()>>
-PYBIND11_DEPRECATED("make_simple_namespace should be replaced with py::module_::import(\"types\").attr(\"SimpleNamespace\") ")
-object make_simple_namespace(Args&&... args_) {
+template <typename... Args, typename = detail::enable_if_t<args_are_all_keyword_or_ds<Args...>()>>
+PYBIND11_DEPRECATED("make_simple_namespace should be replaced with "
+                    "py::module_::import(\"types\").attr(\"SimpleNamespace\") ")
+object make_simple_namespace(Args &&...args_) {
     return module_::import("types").attr("SimpleNamespace")(std::forward<Args>(args_)...);
 }
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 /// Generic support for creating new Python heap types
 class generic_type : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(generic_type, object, PyType_Check)
 protected:
     void initialize(const type_record &rec) {
-        if (rec.scope && hasattr(rec.scope, "__dict__") && rec.scope.attr("__dict__").contains(rec.name))
-            pybind11_fail("generic_type: cannot initialize type \"" + std::string(rec.name) +
-                          "\": an object with that name is already defined");
+        if (rec.scope && hasattr(rec.scope, "__dict__")
+            && rec.scope.attr("__dict__").contains(rec.name)) {
+            pybind11_fail("generic_type: cannot initialize type \"" + std::string(rec.name)
+                          + "\": an object with that name is already defined");
+        }
 
         if ((rec.module_local ? get_local_type_info(*rec.type) : get_global_type_info(*rec.type))
-            != nullptr)
-            pybind11_fail("generic_type: type \"" + std::string(rec.name) +
-                          "\" is already registered!");
+            != nullptr) {
+            pybind11_fail("generic_type: type \"" + std::string(rec.name)
+                          + "\" is already registered!");
+        }
 
         m_ptr = make_new_python_type(rec);
 
         /* Register supplemental type information in C++ dict */
         auto *tinfo = new detail::type_info();
         tinfo->type = (PyTypeObject *) m_ptr;
         tinfo->cpptype = rec.type;
@@ -1201,25 +1334,25 @@
         tinfo->simple_ancestors = true;
         tinfo->default_holder = rec.default_holder;
         tinfo->module_local = rec.module_local;
 
         auto &internals = get_internals();
         auto tindex = std::type_index(*rec.type);
         tinfo->direct_conversions = &internals.direct_conversions[tindex];
-        if (rec.module_local)
+        if (rec.module_local) {
             get_local_internals().registered_types_cpp[tindex] = tinfo;
-        else
+        } else {
             internals.registered_types_cpp[tindex] = tinfo;
-        internals.registered_types_py[(PyTypeObject *) m_ptr] = { tinfo };
+        }
+        internals.registered_types_py[(PyTypeObject *) m_ptr] = {tinfo};
 
         if (rec.bases.size() > 1 || rec.multiple_inheritance) {
             mark_parents_nonsimple(tinfo->type);
             tinfo->simple_ancestors = false;
-        }
-        else if (rec.bases.size() == 1) {
+        } else if (rec.bases.size() == 1) {
             auto *parent_tinfo = get_type_info((PyTypeObject *) rec.bases[0].ptr());
             assert(parent_tinfo != nullptr);
             bool parent_simple_ancestors = parent_tinfo->simple_ancestors;
             tinfo->simple_ancestors = parent_simple_ancestors;
             // The parent can no longer be a simple type if it has MI and has a child
             parent_tinfo->simple_type = parent_tinfo->simple_type && parent_simple_ancestors;
         }
@@ -1231,160 +1364,186 @@
         }
     }
 
     /// Helper function which tags all parents of a type using mult. inheritance
     void mark_parents_nonsimple(PyTypeObject *value) {
         auto t = reinterpret_borrow<tuple>(value->tp_bases);
         for (handle h : t) {
-            auto tinfo2 = get_type_info((PyTypeObject *) h.ptr());
-            if (tinfo2)
+            auto *tinfo2 = get_type_info((PyTypeObject *) h.ptr());
+            if (tinfo2) {
                 tinfo2->simple_type = false;
+            }
             mark_parents_nonsimple((PyTypeObject *) h.ptr());
         }
     }
 
-    void install_buffer_funcs(
-            buffer_info *(*get_buffer)(PyObject *, void *),
-            void *get_buffer_data) {
-        auto *type = (PyHeapTypeObject*) m_ptr;
-        auto tinfo = detail::get_type_info(&type->ht_type);
-
-        if (!type->ht_type.tp_as_buffer)
-            pybind11_fail(
-                "To be able to register buffer protocol support for the type '" +
-                get_fully_qualified_tp_name(tinfo->type) +
-                "' the associated class<>(..) invocation must "
-                "include the pybind11::buffer_protocol() annotation!");
+    void install_buffer_funcs(buffer_info *(*get_buffer)(PyObject *, void *),
+                              void *get_buffer_data) {
+        auto *type = (PyHeapTypeObject *) m_ptr;
+        auto *tinfo = detail::get_type_info(&type->ht_type);
+
+        if (!type->ht_type.tp_as_buffer) {
+            pybind11_fail("To be able to register buffer protocol support for the type '"
+                          + get_fully_qualified_tp_name(tinfo->type)
+                          + "' the associated class<>(..) invocation must "
+                            "include the pybind11::buffer_protocol() annotation!");
+        }
 
         tinfo->get_buffer = get_buffer;
         tinfo->get_buffer_data = get_buffer_data;
     }
 
     // rec_func must be set for either fget or fset.
     void def_property_static_impl(const char *name,
-                                  handle fget, handle fset,
+                                  handle fget,
+                                  handle fset,
                                   detail::function_record *rec_func) {
         const auto is_static = (rec_func != nullptr) && !(rec_func->is_method && rec_func->scope);
         const auto has_doc = (rec_func != nullptr) && (rec_func->doc != nullptr)
                              && pybind11::options::show_user_defined_docstrings();
-        auto property = handle((PyObject *) (is_static ? get_internals().static_property_type
-                                                       : &PyProperty_Type));
+        auto property = handle(
+            (PyObject *) (is_static ? get_internals().static_property_type : &PyProperty_Type));
         attr(name) = property(fget.ptr() ? fget : none(),
                               fset.ptr() ? fset : none(),
-                              /*deleter*/none(),
+                              /*deleter*/ none(),
                               pybind11::str(has_doc ? rec_func->doc : ""));
     }
 };
 
 /// Set the pointer to operator new if it exists. The cast is needed because it can be overloaded.
-template <typename T, typename = void_t<decltype(static_cast<void *(*)(size_t)>(T::operator new))>>
-void set_operator_new(type_record *r) { r->operator_new = &T::operator new; }
-
-template <typename> void set_operator_new(...) { }
-
-template <typename T, typename SFINAE = void> struct has_operator_delete : std::false_type { };
-template <typename T> struct has_operator_delete<T, void_t<decltype(static_cast<void (*)(void *)>(T::operator delete))>>
-    : std::true_type { };
-template <typename T, typename SFINAE = void> struct has_operator_delete_size : std::false_type { };
-template <typename T> struct has_operator_delete_size<T, void_t<decltype(static_cast<void (*)(void *, size_t)>(T::operator delete))>>
-    : std::true_type { };
+template <typename T,
+          typename = void_t<decltype(static_cast<void *(*) (size_t)>(T::operator new))>>
+void set_operator_new(type_record *r) {
+    r->operator_new = &T::operator new;
+}
+
+template <typename>
+void set_operator_new(...) {}
+
+template <typename T, typename SFINAE = void>
+struct has_operator_delete : std::false_type {};
+template <typename T>
+struct has_operator_delete<T, void_t<decltype(static_cast<void (*)(void *)>(T::operator delete))>>
+    : std::true_type {};
+template <typename T, typename SFINAE = void>
+struct has_operator_delete_size : std::false_type {};
+template <typename T>
+struct has_operator_delete_size<
+    T,
+    void_t<decltype(static_cast<void (*)(void *, size_t)>(T::operator delete))>> : std::true_type {
+};
 /// Call class-specific delete if it exists or global otherwise. Can also be an overload set.
 template <typename T, enable_if_t<has_operator_delete<T>::value, int> = 0>
-void call_operator_delete(T *p, size_t, size_t) { T::operator delete(p); }
-template <typename T, enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int> = 0>
-void call_operator_delete(T *p, size_t s, size_t) { T::operator delete(p, s); }
+void call_operator_delete(T *p, size_t, size_t) {
+    T::operator delete(p);
+}
+template <
+    typename T,
+    enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int> = 0>
+void call_operator_delete(T *p, size_t s, size_t) {
+    T::operator delete(p, s);
+}
 
 inline void call_operator_delete(void *p, size_t s, size_t a) {
-    (void)s; (void)a;
-    #if defined(__cpp_aligned_new) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
-        if (a > __STDCPP_DEFAULT_NEW_ALIGNMENT__) {
-            #ifdef __cpp_sized_deallocation
-                ::operator delete(p, s, std::align_val_t(a));
-            #else
-                ::operator delete(p, std::align_val_t(a));
-            #endif
-            return;
-        }
-    #endif
-    #ifdef __cpp_sized_deallocation
-        ::operator delete(p, s);
-    #else
-        ::operator delete(p);
-    #endif
+    (void) s;
+    (void) a;
+#if defined(__cpp_aligned_new) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
+    if (a > __STDCPP_DEFAULT_NEW_ALIGNMENT__) {
+#    ifdef __cpp_sized_deallocation
+        ::operator delete(p, s, std::align_val_t(a));
+#    else
+        ::operator delete(p, std::align_val_t(a));
+#    endif
+        return;
+    }
+#endif
+#ifdef __cpp_sized_deallocation
+    ::operator delete(p, s);
+#else
+    ::operator delete(p);
+#endif
 }
 
-inline void add_class_method(object& cls, const char *name_, const cpp_function &cf) {
+inline void add_class_method(object &cls, const char *name_, const cpp_function &cf) {
     cls.attr(cf.name()) = cf;
     if (std::strcmp(name_, "__eq__") == 0 && !cls.attr("__dict__").contains("__hash__")) {
         cls.attr("__hash__") = none();
     }
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Given a pointer to a member function, cast it to its `Derived` version.
 /// Forward everything else unchanged.
 template <typename /*Derived*/, typename F>
-auto method_adaptor(F &&f) -> decltype(std::forward<F>(f)) { return std::forward<F>(f); }
+auto method_adaptor(F &&f) -> decltype(std::forward<F>(f)) {
+    return std::forward<F>(f);
+}
 
 template <typename Derived, typename Return, typename Class, typename... Args>
 auto method_adaptor(Return (Class::*pmf)(Args...)) -> Return (Derived::*)(Args...) {
-    static_assert(detail::is_accessible_base_of<Class, Derived>::value,
+    static_assert(
+        detail::is_accessible_base_of<Class, Derived>::value,
         "Cannot bind an inaccessible base class method; use a lambda definition instead");
     return pmf;
 }
 
 template <typename Derived, typename Return, typename Class, typename... Args>
 auto method_adaptor(Return (Class::*pmf)(Args...) const) -> Return (Derived::*)(Args...) const {
-    static_assert(detail::is_accessible_base_of<Class, Derived>::value,
+    static_assert(
+        detail::is_accessible_base_of<Class, Derived>::value,
         "Cannot bind an inaccessible base class method; use a lambda definition instead");
     return pmf;
 }
 
 template <typename type_, typename... options>
 class class_ : public detail::generic_type {
-    template <typename T> using is_holder = detail::is_holder_type<type_, T>;
-    template <typename T> using is_subtype = detail::is_strict_base_of<type_, T>;
-    template <typename T> using is_base = detail::is_strict_base_of<T, type_>;
+    template <typename T>
+    using is_holder = detail::is_holder_type<type_, T>;
+    template <typename T>
+    using is_subtype = detail::is_strict_base_of<type_, T>;
+    template <typename T>
+    using is_base = detail::is_strict_base_of<T, type_>;
     // struct instead of using here to help MSVC:
-    template <typename T> struct is_valid_class_option :
-        detail::any_of<is_holder<T>, is_subtype<T>, is_base<T>> {};
+    template <typename T>
+    struct is_valid_class_option : detail::any_of<is_holder<T>, is_subtype<T>, is_base<T>> {};
 
 public:
     using type = type_;
     using type_alias = detail::exactly_one_t<is_subtype, void, options...>;
     constexpr static bool has_alias = !std::is_void<type_alias>::value;
     using holder_type = detail::exactly_one_t<is_holder, std::unique_ptr<type>, options...>;
 
     static_assert(detail::all_of<is_valid_class_option<options>...>::value,
-            "Unknown/invalid class_ template parameters provided");
+                  "Unknown/invalid class_ template parameters provided");
 
     static_assert(!has_alias || std::is_polymorphic<type>::value,
-            "Cannot use an alias class with a non-polymorphic type");
+                  "Cannot use an alias class with a non-polymorphic type");
 
     PYBIND11_OBJECT(class_, generic_type, PyType_Check)
 
     template <typename... Extra>
-    class_(handle scope, const char *name, const Extra &... extra) {
+    class_(handle scope, const char *name, const Extra &...extra) {
         using namespace detail;
 
         // MI can only be specified via class_ template options, not constructor parameters
         static_assert(
             none_of<is_pyobject<Extra>...>::value || // no base class arguments, or:
-            (   constexpr_sum(is_pyobject<Extra>::value...) == 1 && // Exactly one base
-                constexpr_sum(is_base<options>::value...)   == 0 && // no template option bases
-                none_of<std::is_same<multiple_inheritance, Extra>...>::value), // no multiple_inheritance attr
+                (constexpr_sum(is_pyobject<Extra>::value...) == 1 && // Exactly one base
+                 constexpr_sum(is_base<options>::value...) == 0 &&   // no template option bases
+                 // no multiple_inheritance attr
+                 none_of<std::is_same<multiple_inheritance, Extra>...>::value),
             "Error: multiple inheritance bases must be specified via class_ template options");
 
         type_record record;
         record.scope = scope;
         record.name = name;
         record.type = &typeid(type);
         record.type_size = sizeof(conditional_t<has_alias, type_alias, type>);
-        record.type_align = alignof(conditional_t<has_alias, type_alias, type>&);
+        record.type_align = alignof(conditional_t<has_alias, type_alias, type> &);
         record.holder_size = sizeof(holder_type);
         record.init_instance = init_instance;
         record.dealloc = dealloc;
         record.default_holder = detail::is_instantiation<std::unique_ptr, holder_type>::value;
 
         set_operator_new<type>(&record);
 
@@ -1393,264 +1552,316 @@
 
         /* Process optional arguments, if any */
         process_attributes<Extra...>::init(extra..., &record);
 
         generic_type::initialize(record);
 
         if (has_alias) {
-            auto &instances = record.module_local ? get_local_internals().registered_types_cpp : get_internals().registered_types_cpp;
-            instances[std::type_index(typeid(type_alias))] = instances[std::type_index(typeid(type))];
+            auto &instances = record.module_local ? get_local_internals().registered_types_cpp
+                                                  : get_internals().registered_types_cpp;
+            instances[std::type_index(typeid(type_alias))]
+                = instances[std::type_index(typeid(type))];
         }
     }
 
     template <typename Base, detail::enable_if_t<is_base<Base>::value, int> = 0>
     static void add_base(detail::type_record &rec) {
         rec.add_base(typeid(Base), [](void *src) -> void * {
             return static_cast<Base *>(reinterpret_cast<type *>(src));
         });
     }
 
     template <typename Base, detail::enable_if_t<!is_base<Base>::value, int> = 0>
-    static void add_base(detail::type_record &) { }
+    static void add_base(detail::type_record &) {}
 
     template <typename Func, typename... Extra>
-    class_ &def(const char *name_, Func&& f, const Extra&... extra) {
-        cpp_function cf(method_adaptor<type>(std::forward<Func>(f)), name(name_), is_method(*this),
-                        sibling(getattr(*this, name_, none())), extra...);
+    class_ &def(const char *name_, Func &&f, const Extra &...extra) {
+        cpp_function cf(method_adaptor<type>(std::forward<Func>(f)),
+                        name(name_),
+                        is_method(*this),
+                        sibling(getattr(*this, name_, none())),
+                        extra...);
         add_class_method(*this, name_, cf);
         return *this;
     }
 
-    template <typename Func, typename... Extra> class_ &
-    def_static(const char *name_, Func &&f, const Extra&... extra) {
+    template <typename Func, typename... Extra>
+    class_ &def_static(const char *name_, Func &&f, const Extra &...extra) {
         static_assert(!std::is_member_function_pointer<Func>::value,
-                "def_static(...) called with a non-static member function pointer");
-        cpp_function cf(std::forward<Func>(f), name(name_), scope(*this),
-                        sibling(getattr(*this, name_, none())), extra...);
+                      "def_static(...) called with a non-static member function pointer");
+        cpp_function cf(std::forward<Func>(f),
+                        name(name_),
+                        scope(*this),
+                        sibling(getattr(*this, name_, none())),
+                        extra...);
         attr(cf.name()) = staticmethod(cf);
         return *this;
     }
 
     template <detail::op_id id, detail::op_type ot, typename L, typename R, typename... Extra>
-    class_ &def(const detail::op_<id, ot, L, R> &op, const Extra&... extra) {
+    class_ &def(const detail::op_<id, ot, L, R> &op, const Extra &...extra) {
         op.execute(*this, extra...);
         return *this;
     }
 
     template <detail::op_id id, detail::op_type ot, typename L, typename R, typename... Extra>
-    class_ & def_cast(const detail::op_<id, ot, L, R> &op, const Extra&... extra) {
+    class_ &def_cast(const detail::op_<id, ot, L, R> &op, const Extra &...extra) {
         op.execute_cast(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
-    class_ &def(const detail::initimpl::constructor<Args...> &init, const Extra&... extra) {
+    class_ &def(const detail::initimpl::constructor<Args...> &init, const Extra &...extra) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(init);
         init.execute(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
-    class_ &def(const detail::initimpl::alias_constructor<Args...> &init, const Extra&... extra) {
+    class_ &def(const detail::initimpl::alias_constructor<Args...> &init, const Extra &...extra) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(init);
         init.execute(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
-    class_ &def(detail::initimpl::factory<Args...> &&init, const Extra&... extra) {
+    class_ &def(detail::initimpl::factory<Args...> &&init, const Extra &...extra) {
         std::move(init).execute(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
     class_ &def(detail::initimpl::pickle_factory<Args...> &&pf, const Extra &...extra) {
         std::move(pf).execute(*this, extra...);
         return *this;
     }
 
     template <typename Func>
-    class_& def_buffer(Func &&func) {
-        struct capture { Func func; };
-        auto *ptr = new capture { std::forward<Func>(func) };
-        install_buffer_funcs([](PyObject *obj, void *ptr) -> buffer_info* {
-            detail::make_caster<type> caster;
-            if (!caster.load(obj, false))
-                return nullptr;
-            return new buffer_info(((capture *) ptr)->func(caster));
-        }, ptr);
+    class_ &def_buffer(Func &&func) {
+        struct capture {
+            Func func;
+        };
+        auto *ptr = new capture{std::forward<Func>(func)};
+        install_buffer_funcs(
+            [](PyObject *obj, void *ptr) -> buffer_info * {
+                detail::make_caster<type> caster;
+                if (!caster.load(obj, false)) {
+                    return nullptr;
+                }
+                return new buffer_info(((capture *) ptr)->func(caster));
+            },
+            ptr);
         weakref(m_ptr, cpp_function([ptr](handle wr) {
-            delete ptr;
-            wr.dec_ref();
-        })).release();
+                    delete ptr;
+                    wr.dec_ref();
+                }))
+            .release();
         return *this;
     }
 
     template <typename Return, typename Class, typename... Args>
     class_ &def_buffer(Return (Class::*func)(Args...)) {
-        return def_buffer([func] (type &obj) { return (obj.*func)(); });
+        return def_buffer([func](type &obj) { return (obj.*func)(); });
     }
 
     template <typename Return, typename Class, typename... Args>
     class_ &def_buffer(Return (Class::*func)(Args...) const) {
-        return def_buffer([func] (const type &obj) { return (obj.*func)(); });
+        return def_buffer([func](const type &obj) { return (obj.*func)(); });
     }
 
     template <typename C, typename D, typename... Extra>
-    class_ &def_readwrite(const char *name, D C::*pm, const Extra&... extra) {
-        static_assert(std::is_same<C, type>::value || std::is_base_of<C, type>::value, "def_readwrite() requires a class member (or base class member)");
-        cpp_function fget([pm](const type &c) -> const D &{ return c.*pm; }, is_method(*this)),
-                     fset([pm](type &c, const D &value) { c.*pm = value; }, is_method(*this));
+    class_ &def_readwrite(const char *name, D C::*pm, const Extra &...extra) {
+        static_assert(std::is_same<C, type>::value || std::is_base_of<C, type>::value,
+                      "def_readwrite() requires a class member (or base class member)");
+        cpp_function fget([pm](const type &c) -> const D & { return c.*pm; }, is_method(*this)),
+            fset([pm](type &c, const D &value) { c.*pm = value; }, is_method(*this));
         def_property(name, fget, fset, return_value_policy::reference_internal, extra...);
         return *this;
     }
 
     template <typename C, typename D, typename... Extra>
-    class_ &def_readonly(const char *name, const D C::*pm, const Extra& ...extra) {
-        static_assert(std::is_same<C, type>::value || std::is_base_of<C, type>::value, "def_readonly() requires a class member (or base class member)");
-        cpp_function fget([pm](const type &c) -> const D &{ return c.*pm; }, is_method(*this));
+    class_ &def_readonly(const char *name, const D C::*pm, const Extra &...extra) {
+        static_assert(std::is_same<C, type>::value || std::is_base_of<C, type>::value,
+                      "def_readonly() requires a class member (or base class member)");
+        cpp_function fget([pm](const type &c) -> const D & { return c.*pm; }, is_method(*this));
         def_property_readonly(name, fget, return_value_policy::reference_internal, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
-    class_ &def_readwrite_static(const char *name, D *pm, const Extra& ...extra) {
+    class_ &def_readwrite_static(const char *name, D *pm, const Extra &...extra) {
         cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this)),
             fset([pm](const object &, const D &value) { *pm = value; }, scope(*this));
         def_property_static(name, fget, fset, return_value_policy::reference, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
-    class_ &def_readonly_static(const char *name, const D *pm, const Extra& ...extra) {
+    class_ &def_readonly_static(const char *name, const D *pm, const Extra &...extra) {
         cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this));
         def_property_readonly_static(name, fget, return_value_policy::reference, extra...);
         return *this;
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename... Extra>
-    class_ &def_property_readonly(const char *name, const Getter &fget, const Extra& ...extra) {
-        return def_property_readonly(name, cpp_function(method_adaptor<type>(fget)),
-                                     return_value_policy::reference_internal, extra...);
+    class_ &def_property_readonly(const char *name, const Getter &fget, const Extra &...extra) {
+        return def_property_readonly(name,
+                                     cpp_function(method_adaptor<type>(fget)),
+                                     return_value_policy::reference_internal,
+                                     extra...);
     }
 
     /// Uses cpp_function's return_value_policy by default
     template <typename... Extra>
-    class_ &def_property_readonly(const char *name, const cpp_function &fget, const Extra& ...extra) {
+    class_ &
+    def_property_readonly(const char *name, const cpp_function &fget, const Extra &...extra) {
         return def_property(name, fget, nullptr, extra...);
     }
 
     /// Uses return_value_policy::reference by default
     template <typename Getter, typename... Extra>
-    class_ &def_property_readonly_static(const char *name, const Getter &fget, const Extra& ...extra) {
-        return def_property_readonly_static(name, cpp_function(fget), return_value_policy::reference, extra...);
+    class_ &
+    def_property_readonly_static(const char *name, const Getter &fget, const Extra &...extra) {
+        return def_property_readonly_static(
+            name, cpp_function(fget), return_value_policy::reference, extra...);
     }
 
     /// Uses cpp_function's return_value_policy by default
     template <typename... Extra>
-    class_ &def_property_readonly_static(const char *name, const cpp_function &fget, const Extra& ...extra) {
+    class_ &def_property_readonly_static(const char *name,
+                                         const cpp_function &fget,
+                                         const Extra &...extra) {
         return def_property_static(name, fget, nullptr, extra...);
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename Setter, typename... Extra>
-    class_ &def_property(const char *name, const Getter &fget, const Setter &fset, const Extra& ...extra) {
+    class_ &
+    def_property(const char *name, const Getter &fget, const Setter &fset, const Extra &...extra) {
         return def_property(name, fget, cpp_function(method_adaptor<type>(fset)), extra...);
     }
     template <typename Getter, typename... Extra>
-    class_ &def_property(const char *name, const Getter &fget, const cpp_function &fset, const Extra& ...extra) {
-        return def_property(name, cpp_function(method_adaptor<type>(fget)), fset,
-                            return_value_policy::reference_internal, extra...);
+    class_ &def_property(const char *name,
+                         const Getter &fget,
+                         const cpp_function &fset,
+                         const Extra &...extra) {
+        return def_property(name,
+                            cpp_function(method_adaptor<type>(fget)),
+                            fset,
+                            return_value_policy::reference_internal,
+                            extra...);
     }
 
     /// Uses cpp_function's return_value_policy by default
     template <typename... Extra>
-    class_ &def_property(const char *name, const cpp_function &fget, const cpp_function &fset, const Extra& ...extra) {
+    class_ &def_property(const char *name,
+                         const cpp_function &fget,
+                         const cpp_function &fset,
+                         const Extra &...extra) {
         return def_property_static(name, fget, fset, is_method(*this), extra...);
     }
 
     /// Uses return_value_policy::reference by default
     template <typename Getter, typename... Extra>
-    class_ &def_property_static(const char *name, const Getter &fget, const cpp_function &fset, const Extra& ...extra) {
-        return def_property_static(name, cpp_function(fget), fset, return_value_policy::reference, extra...);
+    class_ &def_property_static(const char *name,
+                                const Getter &fget,
+                                const cpp_function &fset,
+                                const Extra &...extra) {
+        return def_property_static(
+            name, cpp_function(fget), fset, return_value_policy::reference, extra...);
     }
 
     /// Uses cpp_function's return_value_policy by default
     template <typename... Extra>
-    class_ &def_property_static(const char *name, const cpp_function &fget, const cpp_function &fset, const Extra& ...extra) {
-        static_assert( 0 == detail::constexpr_sum(std::is_base_of<arg, Extra>::value...),
+    class_ &def_property_static(const char *name,
+                                const cpp_function &fget,
+                                const cpp_function &fset,
+                                const Extra &...extra) {
+        static_assert(0 == detail::constexpr_sum(std::is_base_of<arg, Extra>::value...),
                       "Argument annotations are not allowed for properties");
         auto rec_fget = get_function_record(fget), rec_fset = get_function_record(fset);
         auto *rec_active = rec_fget;
         if (rec_fget) {
-           char *doc_prev = rec_fget->doc; /* 'extra' field may include a property-specific documentation string */
-           detail::process_attributes<Extra...>::init(extra..., rec_fget);
-           if (rec_fget->doc && rec_fget->doc != doc_prev) {
-              std::free(doc_prev);
-              rec_fget->doc = PYBIND11_COMPAT_STRDUP(rec_fget->doc);
-           }
+            char *doc_prev = rec_fget->doc; /* 'extra' field may include a property-specific
+                                               documentation string */
+            detail::process_attributes<Extra...>::init(extra..., rec_fget);
+            if (rec_fget->doc && rec_fget->doc != doc_prev) {
+                std::free(doc_prev);
+                rec_fget->doc = PYBIND11_COMPAT_STRDUP(rec_fget->doc);
+            }
         }
         if (rec_fset) {
             char *doc_prev = rec_fset->doc;
             detail::process_attributes<Extra...>::init(extra..., rec_fset);
             if (rec_fset->doc && rec_fset->doc != doc_prev) {
                 std::free(doc_prev);
                 rec_fset->doc = PYBIND11_COMPAT_STRDUP(rec_fset->doc);
             }
-            if (! rec_active) rec_active = rec_fset;
+            if (!rec_active) {
+                rec_active = rec_fset;
+            }
         }
         def_property_static_impl(name, fget, fset, rec_active);
         return *this;
     }
 
 private:
     /// Initialize holder object, variant 1: object derives from enable_shared_from_this
     template <typename T>
-    static void init_holder(detail::instance *inst, detail::value_and_holder &v_h,
-            const holder_type * /* unused */, const std::enable_shared_from_this<T> * /* dummy */) {
+    static void init_holder(detail::instance *inst,
+                            detail::value_and_holder &v_h,
+                            const holder_type * /* unused */,
+                            const std::enable_shared_from_this<T> * /* dummy */) {
 
         auto sh = std::dynamic_pointer_cast<typename holder_type::element_type>(
-                detail::try_get_shared_from_this(v_h.value_ptr<type>()));
+            detail::try_get_shared_from_this(v_h.value_ptr<type>()));
         if (sh) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(sh));
             v_h.set_holder_constructed();
         }
 
         if (!v_h.holder_constructed() && inst->owned) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
     static void init_holder_from_existing(const detail::value_and_holder &v_h,
-            const holder_type *holder_ptr, std::true_type /*is_copy_constructible*/) {
-        new (std::addressof(v_h.holder<holder_type>())) holder_type(*reinterpret_cast<const holder_type *>(holder_ptr));
+                                          const holder_type *holder_ptr,
+                                          std::true_type /*is_copy_constructible*/) {
+        new (std::addressof(v_h.holder<holder_type>()))
+            holder_type(*reinterpret_cast<const holder_type *>(holder_ptr));
     }
 
     static void init_holder_from_existing(const detail::value_and_holder &v_h,
-            const holder_type *holder_ptr, std::false_type /*is_copy_constructible*/) {
-        new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(*const_cast<holder_type *>(holder_ptr)));
+                                          const holder_type *holder_ptr,
+                                          std::false_type /*is_copy_constructible*/) {
+        new (std::addressof(v_h.holder<holder_type>()))
+            holder_type(std::move(*const_cast<holder_type *>(holder_ptr)));
     }
 
-    /// Initialize holder object, variant 2: try to construct from existing holder object, if possible
-    static void init_holder(detail::instance *inst, detail::value_and_holder &v_h,
-            const holder_type *holder_ptr, const void * /* dummy -- not enable_shared_from_this<T>) */) {
+    /// Initialize holder object, variant 2: try to construct from existing holder object, if
+    /// possible
+    static void init_holder(detail::instance *inst,
+                            detail::value_and_holder &v_h,
+                            const holder_type *holder_ptr,
+                            const void * /* dummy -- not enable_shared_from_this<T>) */) {
         if (holder_ptr) {
             init_holder_from_existing(v_h, holder_ptr, std::is_copy_constructible<holder_type>());
             v_h.set_holder_constructed();
         } else if (inst->owned || detail::always_construct_holder<holder_type>::value) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
     /// Performs instance initialization including constructing a holder and registering the known
-    /// instance.  Should be called as soon as the `type` value_ptr is set for an instance.  Takes an
-    /// optional pointer to an existing holder to use; if not specified and the instance is
+    /// instance.  Should be called as soon as the `type` value_ptr is set for an instance.  Takes
+    /// an optional pointer to an existing holder to use; if not specified and the instance is
     /// `.owned`, a new holder will be constructed to manage the value pointer.
     static void init_instance(detail::instance *inst, const void *holder_ptr) {
         auto v_h = inst->get_value_and_holder(detail::get_type_info(typeid(type)));
         if (!v_h.instance_registered()) {
             register_instance(inst, v_h.value_ptr(), v_h.type);
             v_h.set_instance_registered();
         }
@@ -1665,43 +1876,50 @@
         // If we don't, the Python API will exit with an exception, and pybind11 will
         // throw error_already_set from the C++ destructor which is forbidden and triggers
         // std::terminate().
         error_scope scope;
         if (v_h.holder_constructed()) {
             v_h.holder<holder_type>().~holder_type();
             v_h.set_holder_constructed(false);
-        }
-        else {
-            detail::call_operator_delete(v_h.value_ptr<type>(),
-                v_h.type->type_size,
-                v_h.type->type_align
-            );
+        } else {
+            detail::call_operator_delete(
+                v_h.value_ptr<type>(), v_h.type->type_size, v_h.type->type_align);
         }
         v_h.value_ptr() = nullptr;
     }
 
     static detail::function_record *get_function_record(handle h) {
         h = detail::get_function(h);
-        return h ? (detail::function_record *) reinterpret_borrow<capsule>(PyCFunction_GET_SELF(h.ptr()))
+        return h ? (detail::function_record *) reinterpret_borrow<capsule>(
+                   PyCFunction_GET_SELF(h.ptr()))
                  : nullptr;
     }
 };
 
 /// Binds an existing constructor taking arguments Args...
-template <typename... Args> detail::initimpl::constructor<Args...> init() { return {}; }
+template <typename... Args>
+detail::initimpl::constructor<Args...> init() {
+    return {};
+}
 /// Like `init<Args...>()`, but the instance is always constructed through the alias class (even
 /// when not inheriting on the Python side).
-template <typename... Args> detail::initimpl::alias_constructor<Args...> init_alias() { return {}; }
+template <typename... Args>
+detail::initimpl::alias_constructor<Args...> init_alias() {
+    return {};
+}
 
 /// Binds a factory function as a constructor
 template <typename Func, typename Ret = detail::initimpl::factory<Func>>
-Ret init(Func &&f) { return {std::forward<Func>(f)}; }
+Ret init(Func &&f) {
+    return {std::forward<Func>(f)};
+}
 
-/// Dual-argument factory function: the first function is called when no alias is needed, the second
-/// when an alias is needed (i.e. due to python-side inheritance).  Arguments must be identical.
+/// Dual-argument factory function: the first function is called when no alias is needed, the
+/// second when an alias is needed (i.e. due to python-side inheritance).  Arguments must be
+/// identical.
 template <typename CFunc, typename AFunc, typename Ret = detail::initimpl::factory<CFunc, AFunc>>
 Ret init(CFunc &&c, AFunc &&a) {
     return {std::forward<CFunc>(c), std::forward<AFunc>(a)};
 }
 
 /// Binds pickling functions `__getstate__` and `__setstate__` and ensures that the type
 /// returned by `__getstate__` is the same as the argument accepted by `__setstate__`.
@@ -1711,22 +1929,23 @@
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 inline str enum_name(handle arg) {
     dict entries = arg.get_type().attr("__entries");
     for (auto kv : entries) {
-        if (handle(kv.second[int_(0)]).equal(arg))
+        if (handle(kv.second[int_(0)]).equal(arg)) {
             return pybind11::str(kv.first);
+        }
     }
     return "???";
 }
 
 struct enum_base {
-    enum_base(const handle &base, const handle &parent) : m_base(base), m_parent(parent) { }
+    enum_base(const handle &base, const handle &parent) : m_base(base), m_parent(parent) {}
 
     PYBIND11_NOINLINE void init(bool is_arithmetic, bool is_convertible) {
         m_base.attr("__entries") = dict();
         auto property = handle((PyObject *) &PyProperty_Type);
         auto static_property = handle((PyObject *) get_internals().static_property_type);
 
         m_base.attr("__repr__") = cpp_function(
@@ -1740,43 +1959,55 @@
 
         m_base.attr("name") = property(cpp_function(&enum_name, name("name"), is_method(m_base)));
 
         m_base.attr("__str__") = cpp_function(
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(type_name, enum_name(arg));
-            }, name("name"), is_method(m_base)
-        );
+            },
+            name("name"),
+            is_method(m_base));
 
-        m_base.attr("__doc__") = static_property(cpp_function(
-            [](handle arg) -> std::string {
-                std::string docstring;
-                dict entries = arg.attr("__entries");
-                if (((PyTypeObject *) arg.ptr())->tp_doc)
-                    docstring += std::string(((PyTypeObject *) arg.ptr())->tp_doc) + "\n\n";
-                docstring += "Members:";
-                for (auto kv : entries) {
-                    auto key = std::string(pybind11::str(kv.first));
-                    auto comment = kv.second[int_(1)];
-                    docstring += "\n\n  " + key;
-                    if (!comment.is_none())
-                        docstring += " : " + (std::string) pybind11::str(comment);
-                }
-                return docstring;
-            }, name("__doc__")
-        ), none(), none(), "");
+        m_base.attr("__doc__") = static_property(
+            cpp_function(
+                [](handle arg) -> std::string {
+                    std::string docstring;
+                    dict entries = arg.attr("__entries");
+                    if (((PyTypeObject *) arg.ptr())->tp_doc) {
+                        docstring += std::string(((PyTypeObject *) arg.ptr())->tp_doc) + "\n\n";
+                    }
+                    docstring += "Members:";
+                    for (auto kv : entries) {
+                        auto key = std::string(pybind11::str(kv.first));
+                        auto comment = kv.second[int_(1)];
+                        docstring += "\n\n  " + key;
+                        if (!comment.is_none()) {
+                            docstring += " : " + (std::string) pybind11::str(comment);
+                        }
+                    }
+                    return docstring;
+                },
+                name("__doc__")),
+            none(),
+            none(),
+            "");
 
         m_base.attr("__members__") = static_property(cpp_function(
-            [](handle arg) -> dict {
-                dict entries = arg.attr("__entries"), m;
-                for (auto kv : entries)
-                    m[kv.first] = kv.second[int_(0)];
-                return m;
-            }, name("__members__")), none(), none(), ""
-        );
+                                                         [](handle arg) -> dict {
+                                                             dict entries = arg.attr("__entries"),
+                                                                  m;
+                                                             for (auto kv : entries) {
+                                                                 m[kv.first] = kv.second[int_(0)];
+                                                             }
+                                                             return m;
+                                                         },
+                                                         name("__members__")),
+                                                     none(),
+                                                     none(),
+                                                     "");
 
 #define PYBIND11_ENUM_OP_STRICT(op, expr, strict_behavior)                                        \
     m_base.attr(op) = cpp_function(                                                               \
         [](const object &a, const object &b) {                                                    \
             if (!type::handle_of(a).is(type::handle_of(b)))                                       \
                 strict_behavior; /* NOLINT(bugprone-macro-parentheses) */                         \
             return expr;                                                                          \
@@ -1802,429 +2033,478 @@
             return expr;                                                                          \
         },                                                                                        \
         name(op),                                                                                 \
         is_method(m_base),                                                                        \
         arg("other"))
 
         if (is_convertible) {
-            PYBIND11_ENUM_OP_CONV_LHS("__eq__", !b.is_none() &&  a.equal(b));
-            PYBIND11_ENUM_OP_CONV_LHS("__ne__",  b.is_none() || !a.equal(b));
+            PYBIND11_ENUM_OP_CONV_LHS("__eq__", !b.is_none() && a.equal(b));
+            PYBIND11_ENUM_OP_CONV_LHS("__ne__", b.is_none() || !a.equal(b));
 
             if (is_arithmetic) {
-                PYBIND11_ENUM_OP_CONV("__lt__",   a <  b);
-                PYBIND11_ENUM_OP_CONV("__gt__",   a >  b);
-                PYBIND11_ENUM_OP_CONV("__le__",   a <= b);
-                PYBIND11_ENUM_OP_CONV("__ge__",   a >= b);
-                PYBIND11_ENUM_OP_CONV("__and__",  a &  b);
-                PYBIND11_ENUM_OP_CONV("__rand__", a &  b);
-                PYBIND11_ENUM_OP_CONV("__or__",   a |  b);
-                PYBIND11_ENUM_OP_CONV("__ror__",  a |  b);
-                PYBIND11_ENUM_OP_CONV("__xor__",  a ^  b);
-                PYBIND11_ENUM_OP_CONV("__rxor__", a ^  b);
+                PYBIND11_ENUM_OP_CONV("__lt__", a < b);
+                PYBIND11_ENUM_OP_CONV("__gt__", a > b);
+                PYBIND11_ENUM_OP_CONV("__le__", a <= b);
+                PYBIND11_ENUM_OP_CONV("__ge__", a >= b);
+                PYBIND11_ENUM_OP_CONV("__and__", a & b);
+                PYBIND11_ENUM_OP_CONV("__rand__", a & b);
+                PYBIND11_ENUM_OP_CONV("__or__", a | b);
+                PYBIND11_ENUM_OP_CONV("__ror__", a | b);
+                PYBIND11_ENUM_OP_CONV("__xor__", a ^ b);
+                PYBIND11_ENUM_OP_CONV("__rxor__", a ^ b);
                 m_base.attr("__invert__")
                     = cpp_function([](const object &arg) { return ~(int_(arg)); },
                                    name("__invert__"),
                                    is_method(m_base));
             }
         } else {
-            PYBIND11_ENUM_OP_STRICT("__eq__",  int_(a).equal(int_(b)), return false);
+            PYBIND11_ENUM_OP_STRICT("__eq__", int_(a).equal(int_(b)), return false);
             PYBIND11_ENUM_OP_STRICT("__ne__", !int_(a).equal(int_(b)), return true);
 
             if (is_arithmetic) {
-                #define PYBIND11_THROW throw type_error("Expected an enumeration of matching type!");
-                PYBIND11_ENUM_OP_STRICT("__lt__", int_(a) <  int_(b), PYBIND11_THROW);
-                PYBIND11_ENUM_OP_STRICT("__gt__", int_(a) >  int_(b), PYBIND11_THROW);
+#define PYBIND11_THROW throw type_error("Expected an enumeration of matching type!");
+                PYBIND11_ENUM_OP_STRICT("__lt__", int_(a) < int_(b), PYBIND11_THROW);
+                PYBIND11_ENUM_OP_STRICT("__gt__", int_(a) > int_(b), PYBIND11_THROW);
                 PYBIND11_ENUM_OP_STRICT("__le__", int_(a) <= int_(b), PYBIND11_THROW);
                 PYBIND11_ENUM_OP_STRICT("__ge__", int_(a) >= int_(b), PYBIND11_THROW);
-                #undef PYBIND11_THROW
+#undef PYBIND11_THROW
             }
         }
 
-        #undef PYBIND11_ENUM_OP_CONV_LHS
-        #undef PYBIND11_ENUM_OP_CONV
-        #undef PYBIND11_ENUM_OP_STRICT
+#undef PYBIND11_ENUM_OP_CONV_LHS
+#undef PYBIND11_ENUM_OP_CONV
+#undef PYBIND11_ENUM_OP_STRICT
 
         m_base.attr("__getstate__") = cpp_function(
             [](const object &arg) { return int_(arg); }, name("__getstate__"), is_method(m_base));
 
         m_base.attr("__hash__") = cpp_function(
             [](const object &arg) { return int_(arg); }, name("__hash__"), is_method(m_base));
     }
 
-    PYBIND11_NOINLINE void value(char const* name_, object value, const char *doc = nullptr) {
+    PYBIND11_NOINLINE void value(char const *name_, object value, const char *doc = nullptr) {
         dict entries = m_base.attr("__entries");
         str name(name_);
         if (entries.contains(name)) {
             std::string type_name = (std::string) str(m_base.attr("__name__"));
-            throw value_error(type_name + ": element \"" + std::string(name_) + "\" already exists!");
+            throw value_error(type_name + ": element \"" + std::string(name_)
+                              + "\" already exists!");
         }
 
         entries[name] = std::make_pair(value, doc);
         m_base.attr(name) = value;
     }
 
     PYBIND11_NOINLINE void export_values() {
         dict entries = m_base.attr("__entries");
-        for (auto kv : entries)
+        for (auto kv : entries) {
             m_parent.attr(kv.first) = kv.second[int_(0)];
+        }
     }
 
     handle m_base;
     handle m_parent;
 };
 
-template <bool is_signed, size_t length> struct equivalent_integer {};
-template <> struct equivalent_integer<true,  1> { using type = int8_t;   };
-template <> struct equivalent_integer<false, 1> { using type = uint8_t;  };
-template <> struct equivalent_integer<true,  2> { using type = int16_t;  };
-template <> struct equivalent_integer<false, 2> { using type = uint16_t; };
-template <> struct equivalent_integer<true,  4> { using type = int32_t;  };
-template <> struct equivalent_integer<false, 4> { using type = uint32_t; };
-template <> struct equivalent_integer<true,  8> { using type = int64_t;  };
-template <> struct equivalent_integer<false, 8> { using type = uint64_t; };
+template <bool is_signed, size_t length>
+struct equivalent_integer {};
+template <>
+struct equivalent_integer<true, 1> {
+    using type = int8_t;
+};
+template <>
+struct equivalent_integer<false, 1> {
+    using type = uint8_t;
+};
+template <>
+struct equivalent_integer<true, 2> {
+    using type = int16_t;
+};
+template <>
+struct equivalent_integer<false, 2> {
+    using type = uint16_t;
+};
+template <>
+struct equivalent_integer<true, 4> {
+    using type = int32_t;
+};
+template <>
+struct equivalent_integer<false, 4> {
+    using type = uint32_t;
+};
+template <>
+struct equivalent_integer<true, 8> {
+    using type = int64_t;
+};
+template <>
+struct equivalent_integer<false, 8> {
+    using type = uint64_t;
+};
 
 template <typename IntLike>
-using equivalent_integer_t = typename equivalent_integer<std::is_signed<IntLike>::value, sizeof(IntLike)>::type;
+using equivalent_integer_t =
+    typename equivalent_integer<std::is_signed<IntLike>::value, sizeof(IntLike)>::type;
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Binds C++ enumerations and enumeration classes to Python
-template <typename Type> class enum_ : public class_<Type> {
+template <typename Type>
+class enum_ : public class_<Type> {
 public:
     using Base = class_<Type>;
-    using Base::def;
     using Base::attr;
+    using Base::def;
     using Base::def_property_readonly;
     using Base::def_property_readonly_static;
     using Underlying = typename std::underlying_type<Type>::type;
     // Scalar is the integer representation of underlying type
-    using Scalar = detail::conditional_t<detail::any_of<
-        detail::is_std_char_type<Underlying>, std::is_same<Underlying, bool>
-    >::value, detail::equivalent_integer_t<Underlying>, Underlying>;
+    using Scalar = detail::conditional_t<detail::any_of<detail::is_std_char_type<Underlying>,
+                                                        std::is_same<Underlying, bool>>::value,
+                                         detail::equivalent_integer_t<Underlying>,
+                                         Underlying>;
 
     template <typename... Extra>
-    enum_(const handle &scope, const char *name, const Extra&... extra)
-      : class_<Type>(scope, name, extra...), m_base(*this, scope) {
+    enum_(const handle &scope, const char *name, const Extra &...extra)
+        : class_<Type>(scope, name, extra...), m_base(*this, scope) {
         constexpr bool is_arithmetic = detail::any_of<std::is_same<arithmetic, Extra>...>::value;
         constexpr bool is_convertible = std::is_convertible<Type, Underlying>::value;
         m_base.init(is_arithmetic, is_convertible);
 
         def(init([](Scalar i) { return static_cast<Type>(i); }), arg("value"));
         def_property_readonly("value", [](Type value) { return (Scalar) value; });
         def("__int__", [](Type value) { return (Scalar) value; });
-        #if PY_MAJOR_VERSION < 3
-            def("__long__", [](Type value) { return (Scalar) value; });
-        #endif
-        #if PY_MAJOR_VERSION > 3 || (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION >= 8)
-            def("__index__", [](Type value) { return (Scalar) value; });
-        #endif
-
+        def("__index__", [](Type value) { return (Scalar) value; });
+#if PY_MAJOR_VERSION < 3
+        def("__long__", [](Type value) { return (Scalar) value; });
+#endif
         attr("__setstate__") = cpp_function(
             [](detail::value_and_holder &v_h, Scalar arg) {
-                detail::initimpl::setstate<Base>(v_h, static_cast<Type>(arg),
-                        Py_TYPE(v_h.inst) != v_h.type->type); },
+                detail::initimpl::setstate<Base>(
+                    v_h, static_cast<Type>(arg), Py_TYPE(v_h.inst) != v_h.type->type);
+            },
             detail::is_new_style_constructor(),
-            pybind11::name("__setstate__"), is_method(*this), arg("state"));
+            pybind11::name("__setstate__"),
+            is_method(*this),
+            arg("state"));
     }
 
     /// Export enumeration entries into the parent scope
-    enum_& export_values() {
+    enum_ &export_values() {
         m_base.export_values();
         return *this;
     }
 
     /// Add an enumeration entry
-    enum_& value(char const* name, Type value, const char *doc = nullptr) {
+    enum_ &value(char const *name, Type value, const char *doc = nullptr) {
         m_base.value(name, pybind11::cast(value, return_value_policy::copy), doc);
         return *this;
     }
 
 private:
     detail::enum_base m_base;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-
 PYBIND11_NOINLINE void keep_alive_impl(handle nurse, handle patient) {
-    if (!nurse || !patient)
+    if (!nurse || !patient) {
         pybind11_fail("Could not activate keep_alive!");
+    }
 
-    if (patient.is_none() || nurse.is_none())
+    if (patient.is_none() || nurse.is_none()) {
         return; /* Nothing to keep alive or nothing to be kept alive by */
+    }
 
     auto tinfo = all_type_info(Py_TYPE(nurse.ptr()));
     if (!tinfo.empty()) {
         /* It's a pybind-registered type, so we can store the patient in the
          * internal list. */
         add_patient(nurse.ptr(), patient.ptr());
-    }
-    else {
+    } else {
         /* Fall back to clever approach based on weak references taken from
          * Boost.Python. This is not used for pybind-registered types because
          * the objects can be destroyed out-of-order in a GC pass. */
-        cpp_function disable_lifesupport(
-            [patient](handle weakref) { patient.dec_ref(); weakref.dec_ref(); });
+        cpp_function disable_lifesupport([patient](handle weakref) {
+            patient.dec_ref();
+            weakref.dec_ref();
+        });
 
         weakref wr(nurse, disable_lifesupport);
 
         patient.inc_ref(); /* reference patient and leak the weak reference */
         (void) wr.release();
     }
 }
 
-PYBIND11_NOINLINE void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret) {
+PYBIND11_NOINLINE void
+keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret) {
     auto get_arg = [&](size_t n) {
-        if (n == 0)
+        if (n == 0) {
             return ret;
-        if (n == 1 && call.init_self)
+        }
+        if (n == 1 && call.init_self) {
             return call.init_self;
-        if (n <= call.args.size())
+        }
+        if (n <= call.args.size()) {
             return call.args[n - 1];
+        }
         return handle();
     };
 
     keep_alive_impl(get_arg(Nurse), get_arg(Patient));
 }
 
-inline std::pair<decltype(internals::registered_types_py)::iterator, bool> all_type_info_get_cache(PyTypeObject *type) {
-    auto res = get_internals().registered_types_py
+inline std::pair<decltype(internals::registered_types_py)::iterator, bool>
+all_type_info_get_cache(PyTypeObject *type) {
+    auto res = get_internals()
+                   .registered_types_py
 #ifdef __cpp_lib_unordered_map_try_emplace
-        .try_emplace(type);
+                   .try_emplace(type);
 #else
-        .emplace(type, std::vector<detail::type_info *>());
+                   .emplace(type, std::vector<detail::type_info *>());
 #endif
     if (res.second) {
         // New cache entry created; set up a weak reference to automatically remove it if the type
         // gets destroyed:
         weakref((PyObject *) type, cpp_function([type](handle wr) {
-            get_internals().registered_types_py.erase(type);
+                    get_internals().registered_types_py.erase(type);
 
-            // TODO consolidate the erasure code in pybind11_meta_dealloc() in class.h
-            auto &cache = get_internals().inactive_override_cache;
-            for (auto it = cache.begin(), last = cache.end(); it != last; ) {
-                if (it->first == reinterpret_cast<PyObject *>(type))
-                    it = cache.erase(it);
-                else
-                    ++it;
-            }
+                    // TODO consolidate the erasure code in pybind11_meta_dealloc() in class.h
+                    auto &cache = get_internals().inactive_override_cache;
+                    for (auto it = cache.begin(), last = cache.end(); it != last;) {
+                        if (it->first == reinterpret_cast<PyObject *>(type)) {
+                            it = cache.erase(it);
+                        } else {
+                            ++it;
+                        }
+                    }
 
-            wr.dec_ref();
-        })).release();
+                    wr.dec_ref();
+                }))
+            .release();
     }
 
     return res;
 }
 
 /* There are a large number of apparently unused template arguments because
  * each combination requires a separate py::class_ registration.
  */
-template <typename Access, return_value_policy Policy, typename Iterator, typename Sentinel, typename ValueType, typename... Extra>
+template <typename Access,
+          return_value_policy Policy,
+          typename Iterator,
+          typename Sentinel,
+          typename ValueType,
+          typename... Extra>
 struct iterator_state {
     Iterator it;
     Sentinel end;
     bool first_or_done;
 };
 
 // Note: these helpers take the iterator by non-const reference because some
 // iterators in the wild can't be dereferenced when const. The & after Iterator
 // is required for MSVC < 16.9. SFINAE cannot be reused for result_type due to
 // bugs in ICC, NVCC, and PGI compilers. See PR #3293.
 template <typename Iterator, typename SFINAE = decltype(*std::declval<Iterator &>())>
 struct iterator_access {
     using result_type = decltype(*std::declval<Iterator &>());
     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
-    result_type operator()(Iterator &it) const {
-        return *it;
-    }
+    result_type operator()(Iterator &it) const { return *it; }
 };
 
-template <typename Iterator, typename SFINAE = decltype((*std::declval<Iterator &>()).first) >
+template <typename Iterator, typename SFINAE = decltype((*std::declval<Iterator &>()).first)>
 class iterator_key_access {
 private:
     using pair_type = decltype(*std::declval<Iterator &>());
 
 public:
     /* If either the pair itself or the element of the pair is a reference, we
      * want to return a reference, otherwise a value. When the decltype
      * expression is parenthesized it is based on the value category of the
      * expression; otherwise it is the declared type of the pair member.
      * The use of declval<pair_type> in the second branch rather than directly
      * using *std::declval<Iterator &>() is a workaround for nvcc
      * (it's not used in the first branch because going via decltype and back
      * through declval does not perfectly preserve references).
      */
-    using result_type = conditional_t<
-        std::is_reference<decltype(*std::declval<Iterator &>())>::value,
-        decltype(((*std::declval<Iterator &>()).first)),
-        decltype(std::declval<pair_type>().first)
-    >;
-    result_type operator()(Iterator &it) const {
-        return (*it).first;
-    }
+    using result_type
+        = conditional_t<std::is_reference<decltype(*std::declval<Iterator &>())>::value,
+                        decltype(((*std::declval<Iterator &>()).first)),
+                        decltype(std::declval<pair_type>().first)>;
+    result_type operator()(Iterator &it) const { return (*it).first; }
 };
 
 template <typename Iterator, typename SFINAE = decltype((*std::declval<Iterator &>()).second)>
 class iterator_value_access {
 private:
     using pair_type = decltype(*std::declval<Iterator &>());
 
 public:
-    using result_type = conditional_t<
-        std::is_reference<decltype(*std::declval<Iterator &>())>::value,
-        decltype(((*std::declval<Iterator &>()).second)),
-        decltype(std::declval<pair_type>().second)
-    >;
-    result_type operator()(Iterator &it) const {
-        return (*it).second;
-    }
+    using result_type
+        = conditional_t<std::is_reference<decltype(*std::declval<Iterator &>())>::value,
+                        decltype(((*std::declval<Iterator &>()).second)),
+                        decltype(std::declval<pair_type>().second)>;
+    result_type operator()(Iterator &it) const { return (*it).second; }
 };
 
 template <typename Access,
           return_value_policy Policy,
           typename Iterator,
           typename Sentinel,
           typename ValueType,
           typename... Extra>
-iterator make_iterator_impl(Iterator first, Sentinel last, Extra &&... extra) {
+iterator make_iterator_impl(Iterator first, Sentinel last, Extra &&...extra) {
     using state = detail::iterator_state<Access, Policy, Iterator, Sentinel, ValueType, Extra...>;
     // TODO: state captures only the types of Extra, not the values
 
     if (!detail::get_type_info(typeid(state), false)) {
         class_<state>(handle(), "iterator", pybind11::module_local())
-            .def("__iter__", [](state &s) -> state& { return s; })
-            .def("__next__", [](state &s) -> ValueType {
-                if (!s.first_or_done)
-                    ++s.it;
-                else
-                    s.first_or_done = false;
-                if (s.it == s.end) {
-                    s.first_or_done = true;
-                    throw stop_iteration();
-                }
-                return Access()(s.it);
-            // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
-            }, std::forward<Extra>(extra)..., Policy);
+            .def("__iter__", [](state &s) -> state & { return s; })
+            .def(
+                "__next__",
+                [](state &s) -> ValueType {
+                    if (!s.first_or_done) {
+                        ++s.it;
+                    } else {
+                        s.first_or_done = false;
+                    }
+                    if (s.it == s.end) {
+                        s.first_or_done = true;
+                        throw stop_iteration();
+                    }
+                    return Access()(s.it);
+                    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
+                },
+                std::forward<Extra>(extra)...,
+                Policy);
     }
 
     return cast(state{first, last, true});
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_access<Iterator>::result_type,
           typename... Extra>
-iterator make_iterator(Iterator first, Sentinel last, Extra &&... extra) {
-    return detail::make_iterator_impl<
-        detail::iterator_access<Iterator>,
-        Policy,
-        Iterator,
-        Sentinel,
-        ValueType,
-        Extra...>(first, last, std::forward<Extra>(extra)...);
+iterator make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+    return detail::make_iterator_impl<detail::iterator_access<Iterator>,
+                                      Policy,
+                                      Iterator,
+                                      Sentinel,
+                                      ValueType,
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the keys (`.first`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename KeyType = typename detail::iterator_key_access<Iterator>::result_type,
           typename... Extra>
 iterator make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
-    return detail::make_iterator_impl<
-        detail::iterator_key_access<Iterator>,
-        Policy,
-        Iterator,
-        Sentinel,
-        KeyType,
-        Extra...>(first, last, std::forward<Extra>(extra)...);
+    return detail::make_iterator_impl<detail::iterator_key_access<Iterator>,
+                                      Policy,
+                                      Iterator,
+                                      Sentinel,
+                                      KeyType,
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the values (`.second`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_value_access<Iterator>::result_type,
           typename... Extra>
 iterator make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
-    return detail::make_iterator_impl<
-        detail::iterator_value_access<Iterator>,
-        Policy, Iterator,
-        Sentinel,
-        ValueType,
-        Extra...>(first, last, std::forward<Extra>(extra)...);
+    return detail::make_iterator_impl<detail::iterator_value_access<Iterator>,
+                                      Policy,
+                                      Iterator,
+                                      Sentinel,
+                                      ValueType,
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over values of an stl container or other container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
-          typename Type, typename... Extra> iterator make_iterator(Type &value, Extra&&... extra) {
+          typename Type,
+          typename... Extra>
+iterator make_iterator(Type &value, Extra &&...extra) {
     return make_iterator<Policy>(std::begin(value), std::end(value), extra...);
 }
 
 /// Makes an iterator over the keys (`.first`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
-          typename Type, typename... Extra> iterator make_key_iterator(Type &value, Extra&&... extra) {
+          typename Type,
+          typename... Extra>
+iterator make_key_iterator(Type &value, Extra &&...extra) {
     return make_key_iterator<Policy>(std::begin(value), std::end(value), extra...);
 }
 
 /// Makes an iterator over the values (`.second`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
-          typename Type, typename... Extra> iterator make_value_iterator(Type &value, Extra&&... extra) {
+          typename Type,
+          typename... Extra>
+iterator make_value_iterator(Type &value, Extra &&...extra) {
     return make_value_iterator<Policy>(std::begin(value), std::end(value), extra...);
 }
 
-template <typename InputType, typename OutputType> void implicitly_convertible() {
+template <typename InputType, typename OutputType>
+void implicitly_convertible() {
     struct set_flag {
         bool &flag;
         explicit set_flag(bool &flag_) : flag(flag_) { flag_ = true; }
         ~set_flag() { flag = false; }
     };
     auto implicit_caster = [](PyObject *obj, PyTypeObject *type) -> PyObject * {
         static bool currently_used = false;
-        if (currently_used) // implicit conversions are non-reentrant
+        if (currently_used) { // implicit conversions are non-reentrant
             return nullptr;
+        }
         set_flag flag_helper(currently_used);
-        if (!detail::make_caster<InputType>().load(obj, false))
+        if (!detail::make_caster<InputType>().load(obj, false)) {
             return nullptr;
+        }
         tuple args(1);
         args[0] = obj;
         PyObject *result = PyObject_Call((PyObject *) type, args.ptr(), nullptr);
-        if (result == nullptr)
+        if (result == nullptr) {
             PyErr_Clear();
+        }
         return result;
     };
 
-    if (auto tinfo = detail::get_type_info(typeid(OutputType)))
+    if (auto *tinfo = detail::get_type_info(typeid(OutputType))) {
         tinfo->implicit_conversions.push_back(implicit_caster);
-    else
+    } else {
         pybind11_fail("implicitly_convertible: Unable to find type " + type_id<OutputType>());
+    }
 }
 
-
 inline void register_exception_translator(ExceptionTranslator &&translator) {
     detail::get_internals().registered_exception_translators.push_front(
         std::forward<ExceptionTranslator>(translator));
 }
 
-
 /**
-  * Add a new module-local exception translator. Locally registered functions
-  * will be tried before any globally registered exception translators, which
-  * will only be invoked if the module-local handlers do not deal with
-  * the exception.
-  */
+ * Add a new module-local exception translator. Locally registered functions
+ * will be tried before any globally registered exception translators, which
+ * will only be invoked if the module-local handlers do not deal with
+ * the exception.
+ */
 inline void register_local_exception_translator(ExceptionTranslator &&translator) {
     detail::get_local_internals().registered_exception_translators.push_front(
         std::forward<ExceptionTranslator>(translator));
 }
 
 /**
  * Wrapper to generate a new Python exception type.
@@ -2234,50 +2514,55 @@
  * Template type argument is reserved for future use.
  */
 template <typename type>
 class exception : public object {
 public:
     exception() = default;
     exception(handle scope, const char *name, handle base = PyExc_Exception) {
-        std::string full_name = scope.attr("__name__").cast<std::string>() +
-                                std::string(".") + name;
+        std::string full_name
+            = scope.attr("__name__").cast<std::string>() + std::string(".") + name;
         m_ptr = PyErr_NewException(const_cast<char *>(full_name.c_str()), base.ptr(), NULL);
-        if (hasattr(scope, "__dict__") && scope.attr("__dict__").contains(name))
+        if (hasattr(scope, "__dict__") && scope.attr("__dict__").contains(name)) {
             pybind11_fail("Error during initialization: multiple incompatible "
-                          "definitions with name \"" + std::string(name) + "\"");
+                          "definitions with name \""
+                          + std::string(name) + "\"");
+        }
         scope.attr(name) = *this;
     }
 
     // Sets the current python exception to this exception object with the given message
-    void operator()(const char *message) {
-        PyErr_SetString(m_ptr, message);
-    }
+    void operator()(const char *message) { PyErr_SetString(m_ptr, message); }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns a reference to a function-local static exception object used in the simple
 // register_exception approach below.  (It would be simpler to have the static local variable
 // directly in register_exception, but that makes clang <3.5 segfault - issue #1349).
 template <typename CppException>
-exception<CppException> &get_exception_object() { static exception<CppException> ex; return ex; }
+exception<CppException> &get_exception_object() {
+    static exception<CppException> ex;
+    return ex;
+}
 
 // Helper function for register_exception and register_local_exception
 template <typename CppException>
-exception<CppException> &register_exception_impl(handle scope,
-                                                const char *name,
-                                                handle base,
-                                                bool isLocal) {
+exception<CppException> &
+register_exception_impl(handle scope, const char *name, handle base, bool isLocal) {
     auto &ex = detail::get_exception_object<CppException>();
-    if (!ex) ex = exception<CppException>(scope, name, base);
+    if (!ex) {
+        ex = exception<CppException>(scope, name, base);
+    }
 
-    auto register_func = isLocal ? &register_local_exception_translator
-                                 : &register_exception_translator;
+    auto register_func
+        = isLocal ? &register_local_exception_translator : &register_exception_translator;
 
     register_func([](std::exception_ptr p) {
-        if (!p) return;
+        if (!p) {
+            return;
+        }
         try {
             std::rethrow_exception(p);
         } catch (const CppException &e) {
             detail::get_exception_object<CppException>()(e.what());
         }
     });
     return ex;
@@ -2288,32 +2573,30 @@
 /**
  * Registers a Python exception in `m` of the given `name` and installs a translator to
  * translate the C++ exception to the created Python exception using the what() method.
  * This is intended for simple exception translations; for more complex translation, register the
  * exception object and translator directly.
  */
 template <typename CppException>
-exception<CppException> &register_exception(handle scope,
-                                            const char *name,
-                                            handle base = PyExc_Exception) {
+exception<CppException> &
+register_exception(handle scope, const char *name, handle base = PyExc_Exception) {
     return detail::register_exception_impl<CppException>(scope, name, base, false /* isLocal */);
 }
 
 /**
  * Registers a Python exception in `m` of the given `name` and installs a translator to
  * translate the C++ exception to the created Python exception using the what() method.
  * This translator will only be used for exceptions that are thrown in this module and will be
  * tried before global exception translators, including those registered with register_exception.
  * This is intended for simple exception translations; for more complex translation, register the
  * exception object and translator directly.
  */
 template <typename CppException>
-exception<CppException> &register_local_exception(handle scope,
-                                                  const char *name,
-                                                  handle base = PyExc_Exception) {
+exception<CppException> &
+register_local_exception(handle scope, const char *name, handle base = PyExc_Exception) {
     return detail::register_exception_impl<CppException>(scope, name, base, true /* isLocal */);
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 PYBIND11_NOINLINE void print(const tuple &args, const dict &kwargs) {
     auto strings = tuple(args.size());
     for (size_t i = 0; i < args.size(); ++i) {
@@ -2337,16 +2620,17 @@
         }
     }
 
     auto write = file.attr("write");
     write(line);
     write(kwargs.contains("end") ? kwargs["end"] : cast("\n"));
 
-    if (kwargs.contains("flush") && kwargs["flush"].cast<bool>())
+    if (kwargs.contains("flush") && kwargs["flush"].cast<bool>()) {
         file.attr("flush")();
+    }
 }
 PYBIND11_NAMESPACE_END(detail)
 
 template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
 void print(Args &&...args) {
     auto c = detail::collect_arguments<policy>(std::forward<Args>(args)...);
     detail::print(c.args(), c.kwargs());
@@ -2359,108 +2643,117 @@
         m_type.release().dec_ref();
         m_value.release().dec_ref();
         m_trace.release().dec_ref();
     }
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-inline function get_type_override(const void *this_ptr, const type_info *this_type, const char *name)  {
+inline function
+get_type_override(const void *this_ptr, const type_info *this_type, const char *name) {
     handle self = get_object_handle(this_ptr, this_type);
-    if (!self)
+    if (!self) {
         return function();
+    }
     handle type = type::handle_of(self);
     auto key = std::make_pair(type.ptr(), name);
 
     /* Cache functions that aren't overridden in Python to avoid
        many costly Python dictionary lookups below */
     auto &cache = get_internals().inactive_override_cache;
-    if (cache.find(key) != cache.end())
+    if (cache.find(key) != cache.end()) {
         return function();
+    }
 
     function override = getattr(self, name, function());
     if (override.is_cpp_function()) {
         cache.insert(key);
         return function();
     }
 
     /* Don't call dispatch code if invoked from overridden function.
        Unfortunately this doesn't work on PyPy. */
-#if !defined(PYPY_VERSION) && PY_VERSION_HEX < 0x030B0000
-    // TODO: Remove PyPy workaround for Python 3.11.
-    // Current API fails on 3.11 since co_varnames can be null.
-#if PY_VERSION_HEX >= 0x03090000
+#if !defined(PYPY_VERSION)
+#    if PY_VERSION_HEX >= 0x03090000
     PyFrameObject *frame = PyThreadState_GetFrame(PyThreadState_Get());
     if (frame != nullptr) {
         PyCodeObject *f_code = PyFrame_GetCode(frame);
         // f_code is guaranteed to not be NULL
         if ((std::string) str(f_code->co_name) == name && f_code->co_argcount > 0) {
-            PyObject* locals = PyEval_GetLocals();
-            if (locals != nullptr && f_code->co_varnames != nullptr) {
-                PyObject *self_caller = dict_getitem(
-                    locals, PyTuple_GET_ITEM(f_code->co_varnames, 0)
-                );
+            PyObject *locals = PyEval_GetLocals();
+            if (locals != nullptr) {
+                PyObject *co_varnames = PyObject_GetAttrString((PyObject *) f_code, "co_varnames");
+                PyObject *self_arg = PyTuple_GET_ITEM(co_varnames, 0);
+                Py_DECREF(co_varnames);
+                PyObject *self_caller = dict_getitem(locals, self_arg);
                 if (self_caller == self.ptr()) {
                     Py_DECREF(f_code);
                     Py_DECREF(frame);
                     return function();
                 }
             }
         }
         Py_DECREF(f_code);
         Py_DECREF(frame);
     }
-#else
+#    else
     PyFrameObject *frame = PyThreadState_Get()->frame;
     if (frame != nullptr && (std::string) str(frame->f_code->co_name) == name
         && frame->f_code->co_argcount > 0) {
         PyFrame_FastToLocals(frame);
-        PyObject *self_caller = dict_getitem(
-            frame->f_locals, PyTuple_GET_ITEM(frame->f_code->co_varnames, 0));
-        if (self_caller == self.ptr())
+        PyObject *self_caller
+            = dict_getitem(frame->f_locals, PyTuple_GET_ITEM(frame->f_code->co_varnames, 0));
+        if (self_caller == self.ptr()) {
             return function();
+        }
     }
-#endif
+#    endif
 
 #else
     /* PyPy currently doesn't provide a detailed cpyext emulation of
        frame objects, so we have to emulate this using Python. This
        is going to be slow..*/
-    dict d; d["self"] = self; d["name"] = pybind11::str(name);
-    PyObject *result = PyRun_String(
-        "import inspect\n"
-        "frame = inspect.currentframe()\n"
-        "if frame is not None:\n"
-        "    frame = frame.f_back\n"
-        "    if frame is not None and str(frame.f_code.co_name) == name and "
-        "frame.f_code.co_argcount > 0:\n"
-        "        self_caller = frame.f_locals[frame.f_code.co_varnames[0]]\n"
-        "        if self_caller == self:\n"
-        "            self = None\n",
-        Py_file_input, d.ptr(), d.ptr());
+    dict d;
+    d["self"] = self;
+    d["name"] = pybind11::str(name);
+    PyObject *result
+        = PyRun_String("import inspect\n"
+                       "frame = inspect.currentframe()\n"
+                       "if frame is not None:\n"
+                       "    frame = frame.f_back\n"
+                       "    if frame is not None and str(frame.f_code.co_name) == name and "
+                       "frame.f_code.co_argcount > 0:\n"
+                       "        self_caller = frame.f_locals[frame.f_code.co_varnames[0]]\n"
+                       "        if self_caller == self:\n"
+                       "            self = None\n",
+                       Py_file_input,
+                       d.ptr(),
+                       d.ptr());
     if (result == nullptr)
         throw error_already_set();
+    Py_DECREF(result);
     if (d["self"].is_none())
         return function();
-    Py_DECREF(result);
 #endif
 
     return override;
 }
 PYBIND11_NAMESPACE_END(detail)
 
 /** \rst
-  Try to retrieve a python method by the provided name from the instance pointed to by the this_ptr.
+  Try to retrieve a python method by the provided name from the instance pointed to by the
+  this_ptr.
 
-  :this_ptr: The pointer to the object the overridden method should be retrieved for. This should be
-             the first non-trampoline class encountered in the inheritance chain.
+  :this_ptr: The pointer to the object the overridden method should be retrieved for. This should
+             be the first non-trampoline class encountered in the inheritance chain.
   :name: The name of the overridden Python method to retrieve.
   :return: The Python method by this name from the object or an empty function wrapper.
  \endrst */
-template <class T> function get_override(const T *this_ptr, const char *name) {
-    auto tinfo = detail::get_type_info(typeid(T));
+template <class T>
+function get_override(const T *this_ptr, const char *name) {
+    auto *tinfo = detail::get_type_info(typeid(T));
     return tinfo ? detail::get_type_override(this_ptr, tinfo, name) : function();
 }
 
 #define PYBIND11_OVERRIDE_IMPL(ret_type, cname, name, ...)                                        \
     do {                                                                                          \
         pybind11::gil_scoped_acquire gil;                                                         \
         pybind11::function override                                                               \
@@ -2472,50 +2765,53 @@
                 return pybind11::detail::cast_ref<ret_type>(std::move(o), caster);                \
             }                                                                                     \
             return pybind11::detail::cast_safe<ret_type>(std::move(o));                           \
         }                                                                                         \
     } while (false)
 
 /** \rst
-    Macro to populate the virtual method in the trampoline class. This macro tries to look up a method named 'fn'
-    from the Python side, deals with the :ref:`gil` and necessary argument conversions to call this method and return
-    the appropriate type. See :ref:`overriding_virtuals` for more information. This macro should be used when the method
+    Macro to populate the virtual method in the trampoline class. This macro tries to look up a
+    method named 'fn' from the Python side, deals with the :ref:`gil` and necessary argument
+    conversions to call this method and return the appropriate type.
+    See :ref:`overriding_virtuals` for more information. This macro should be used when the method
     name in C is not the same as the method name in Python. For example with `__str__`.
 
     .. code-block:: cpp
 
       std::string toString() override {
         PYBIND11_OVERRIDE_NAME(
             std::string, // Return type (ret_type)
             Animal,      // Parent class (cname)
             "__str__",   // Name of method in Python (name)
             toString,    // Name of function in C++ (fn)
         );
       }
 \endrst */
-#define PYBIND11_OVERRIDE_NAME(ret_type, cname, name, fn, ...) \
-    do { \
+#define PYBIND11_OVERRIDE_NAME(ret_type, cname, name, fn, ...)                                    \
+    do {                                                                                          \
         PYBIND11_OVERRIDE_IMPL(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, __VA_ARGS__); \
-        return cname::fn(__VA_ARGS__); \
+        return cname::fn(__VA_ARGS__);                                                            \
     } while (false)
 
 /** \rst
-    Macro for pure virtual functions, this function is identical to :c:macro:`PYBIND11_OVERRIDE_NAME`, except that it
-    throws if no override can be found.
+    Macro for pure virtual functions, this function is identical to
+    :c:macro:`PYBIND11_OVERRIDE_NAME`, except that it throws if no override can be found.
 \endrst */
-#define PYBIND11_OVERRIDE_PURE_NAME(ret_type, cname, name, fn, ...) \
-    do { \
+#define PYBIND11_OVERRIDE_PURE_NAME(ret_type, cname, name, fn, ...)                               \
+    do {                                                                                          \
         PYBIND11_OVERRIDE_IMPL(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, __VA_ARGS__); \
-        pybind11::pybind11_fail("Tried to call pure virtual function \"" PYBIND11_STRINGIFY(cname) "::" name "\""); \
+        pybind11::pybind11_fail(                                                                  \
+            "Tried to call pure virtual function \"" PYBIND11_STRINGIFY(cname) "::" name "\"");   \
     } while (false)
 
 /** \rst
-    Macro to populate the virtual method in the trampoline class. This macro tries to look up the method
-    from the Python side, deals with the :ref:`gil` and necessary argument conversions to call this method and return
-    the appropriate type. This macro should be used if the method name in C and in Python are identical.
+    Macro to populate the virtual method in the trampoline class. This macro tries to look up the
+    method from the Python side, deals with the :ref:`gil` and necessary argument conversions to
+    call this method and return the appropriate type. This macro should be used if the method name
+    in C and in Python are identical.
     See :ref:`overriding_virtuals` for more information.
 
     .. code-block:: cpp
 
       class PyAnimal : public Animal {
       public:
           // Inherit the constructors
@@ -2528,46 +2824,48 @@
                   Animal,      // Parent class (cname)
                   go,          // Name of function in C++ (must match Python name) (fn)
                   n_times      // Argument(s) (...)
               );
           }
       };
 \endrst */
-#define PYBIND11_OVERRIDE(ret_type, cname, fn, ...) \
+#define PYBIND11_OVERRIDE(ret_type, cname, fn, ...)                                               \
     PYBIND11_OVERRIDE_NAME(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), #fn, fn, __VA_ARGS__)
 
 /** \rst
-    Macro for pure virtual functions, this function is identical to :c:macro:`PYBIND11_OVERRIDE`, except that it throws
-    if no override can be found.
+    Macro for pure virtual functions, this function is identical to :c:macro:`PYBIND11_OVERRIDE`,
+    except that it throws if no override can be found.
 \endrst */
-#define PYBIND11_OVERRIDE_PURE(ret_type, cname, fn, ...) \
-    PYBIND11_OVERRIDE_PURE_NAME(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), #fn, fn, __VA_ARGS__)
-
+#define PYBIND11_OVERRIDE_PURE(ret_type, cname, fn, ...)                                          \
+    PYBIND11_OVERRIDE_PURE_NAME(                                                                  \
+        PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), #fn, fn, __VA_ARGS__)
 
 // Deprecated versions
 
 PYBIND11_DEPRECATED("get_type_overload has been deprecated")
-inline function get_type_overload(const void *this_ptr, const detail::type_info *this_type, const char *name) {
+inline function
+get_type_overload(const void *this_ptr, const detail::type_info *this_type, const char *name) {
     return detail::get_type_override(this_ptr, this_type, name);
 }
 
 template <class T>
 inline function get_overload(const T *this_ptr, const char *name) {
     return get_override(this_ptr, name);
 }
 
-#define PYBIND11_OVERLOAD_INT(ret_type, cname, name, ...) \
+#define PYBIND11_OVERLOAD_INT(ret_type, cname, name, ...)                                         \
     PYBIND11_OVERRIDE_IMPL(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, __VA_ARGS__)
-#define PYBIND11_OVERLOAD_NAME(ret_type, cname, name, fn, ...) \
+#define PYBIND11_OVERLOAD_NAME(ret_type, cname, name, fn, ...)                                    \
     PYBIND11_OVERRIDE_NAME(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, fn, __VA_ARGS__)
-#define PYBIND11_OVERLOAD_PURE_NAME(ret_type, cname, name, fn, ...) \
-    PYBIND11_OVERRIDE_PURE_NAME(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, fn, __VA_ARGS__);
-#define PYBIND11_OVERLOAD(ret_type, cname, fn, ...) \
+#define PYBIND11_OVERLOAD_PURE_NAME(ret_type, cname, name, fn, ...)                               \
+    PYBIND11_OVERRIDE_PURE_NAME(                                                                  \
+        PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, fn, __VA_ARGS__);
+#define PYBIND11_OVERLOAD(ret_type, cname, fn, ...)                                               \
     PYBIND11_OVERRIDE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__)
-#define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...) \
+#define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...)                                          \
     PYBIND11_OVERRIDE_PURE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__);
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
 
 #if defined(__GNUC__) && __GNUC__ == 7
 #    pragma GCC diagnostic pop // -Wnoexcept-type
 #endif
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/pytypes.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/pytypes.h`

 * *Files 6% similar despite different names*

```diff
@@ -7,57 +7,63 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
 #include "buffer_info.h"
-#include <utility>
+
 #include <type_traits>
+#include <utility>
 
 #if defined(PYBIND11_HAS_OPTIONAL)
-#  include <optional>
+#    include <optional>
 #endif
 
 #ifdef PYBIND11_HAS_STRING_VIEW
-#  include <string_view>
+#    include <string_view>
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 /* A few forward declarations */
-class handle; class object;
-class str; class iterator;
+class handle;
+class object;
+class str;
+class iterator;
 class type;
-struct arg; struct arg_v;
+struct arg;
+struct arg_v;
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 class args_proxy;
 bool isinstance_generic(handle obj, const std::type_info &tp);
 
 // Accessor forward declarations
-template <typename Policy> class accessor;
+template <typename Policy>
+class accessor;
 namespace accessor_policies {
-    struct obj_attr;
-    struct str_attr;
-    struct generic_item;
-    struct sequence_item;
-    struct list_item;
-    struct tuple_item;
+struct obj_attr;
+struct str_attr;
+struct generic_item;
+struct sequence_item;
+struct list_item;
+struct tuple_item;
 } // namespace accessor_policies
 using obj_attr_accessor = accessor<accessor_policies::obj_attr>;
 using str_attr_accessor = accessor<accessor_policies::str_attr>;
 using item_accessor = accessor<accessor_policies::generic_item>;
 using sequence_accessor = accessor<accessor_policies::sequence_item>;
 using list_accessor = accessor<accessor_policies::list_item>;
 using tuple_accessor = accessor<accessor_policies::tuple_item>;
 
 /// Tag and check to identify a class which implements the Python object API
-class pyobject_tag { };
-template <typename T> using is_pyobject = std::is_base_of<pyobject_tag, remove_reference_t<T>>;
+class pyobject_tag {};
+template <typename T>
+using is_pyobject = std::is_base_of<pyobject_tag, remove_reference_t<T>>;
 
 /** \rst
     A mixin class which adds common functions to `handle`, `object` and various accessors.
     The only requirement for `Derived` is to implement ``PyObject *Derived::ptr() const``.
 \endrst */
 template <typename Derived>
 class object_api : public pyobject_tag {
@@ -97,42 +103,45 @@
         or ``list`` for a function call. Applying another * to the result yields
         ** unpacking, e.g. to unpack a dict as function keyword arguments.
         See :ref:`calling_python_functions`.
     \endrst */
     args_proxy operator*() const;
 
     /// Check if the given item is contained within this object, i.e. ``item in obj``.
-    template <typename T> bool contains(T &&item) const;
+    template <typename T>
+    bool contains(T &&item) const;
 
     /** \rst
         Assuming the Python object is a function or implements the ``__call__``
         protocol, ``operator()`` invokes the underlying function, passing an
         arbitrary set of parameters. The result is returned as a `object` and
         may need to be converted back into a Python object using `handle::cast()`.
 
         When some of the arguments cannot be converted to Python objects, the
         function will throw a `cast_error` exception. When the Python function
         call fails, a `error_already_set` exception is thrown.
     \endrst */
-    template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
+    template <return_value_policy policy = return_value_policy::automatic_reference,
+              typename... Args>
     object operator()(Args &&...args) const;
-    template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
+    template <return_value_policy policy = return_value_policy::automatic_reference,
+              typename... Args>
     PYBIND11_DEPRECATED("call(...) was deprecated in favor of operator()(...)")
-        object call(Args&&... args) const;
+    object call(Args &&...args) const;
 
     /// Equivalent to ``obj is other`` in Python.
-    bool is(object_api const& other) const { return derived().ptr() == other.derived().ptr(); }
+    bool is(object_api const &other) const { return derived().ptr() == other.derived().ptr(); }
     /// Equivalent to ``obj is None`` in Python.
     bool is_none() const { return derived().ptr() == Py_None; }
     /// Equivalent to obj == other in Python
-    bool equal(object_api const &other) const      { return rich_compare(other, Py_EQ); }
-    bool not_equal(object_api const &other) const  { return rich_compare(other, Py_NE); }
-    bool operator<(object_api const &other) const  { return rich_compare(other, Py_LT); }
+    bool equal(object_api const &other) const { return rich_compare(other, Py_EQ); }
+    bool not_equal(object_api const &other) const { return rich_compare(other, Py_NE); }
+    bool operator<(object_api const &other) const { return rich_compare(other, Py_LT); }
     bool operator<=(object_api const &other) const { return rich_compare(other, Py_LE); }
-    bool operator>(object_api const &other) const  { return rich_compare(other, Py_GT); }
+    bool operator>(object_api const &other) const { return rich_compare(other, Py_GT); }
     bool operator>=(object_api const &other) const { return rich_compare(other, Py_GE); }
 
     object operator-() const;
     object operator~() const;
     object operator+(object_api const &other) const;
     object operator+=(object_api const &other) const;
     object operator-(object_api const &other) const;
@@ -157,15 +166,16 @@
 
     /// Get or set the object's docstring, i.e. ``obj.__doc__``.
     str_attr_accessor doc() const;
 
     /// Return the object's current reference count
     int ref_count() const { return static_cast<int>(Py_REFCNT(derived().ptr())); }
 
-    // TODO PYBIND11_DEPRECATED("Call py::type::handle_of(h) or py::type::of(h) instead of h.get_type()")
+    // TODO PYBIND11_DEPRECATED(
+    //     "Call py::type::handle_of(h) or py::type::of(h) instead of h.get_type()")
     handle get_type() const;
 
 private:
     bool rich_compare(object_api const &other, int value) const;
 };
 
 PYBIND11_NAMESPACE_END(detail)
@@ -183,51 +193,59 @@
 \endrst */
 class handle : public detail::object_api<handle> {
 public:
     /// The default constructor creates a handle with a ``nullptr``-valued pointer
     handle() = default;
     /// Creates a ``handle`` from the given raw Python object pointer
     // NOLINTNEXTLINE(google-explicit-constructor)
-    handle(PyObject *ptr) : m_ptr(ptr) { } // Allow implicit conversion from PyObject*
+    handle(PyObject *ptr) : m_ptr(ptr) {} // Allow implicit conversion from PyObject*
 
     /// Return the underlying ``PyObject *`` pointer
     PyObject *ptr() const { return m_ptr; }
     PyObject *&ptr() { return m_ptr; }
 
     /** \rst
         Manually increase the reference count of the Python object. Usually, it is
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
-    const handle& inc_ref() const & { Py_XINCREF(m_ptr); return *this; }
+    const handle &inc_ref() const & {
+        Py_XINCREF(m_ptr);
+        return *this;
+    }
 
     /** \rst
         Manually decrease the reference count of the Python object. Usually, it is
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
-    const handle& dec_ref() const & { Py_XDECREF(m_ptr); return *this; }
+    const handle &dec_ref() const & {
+        Py_XDECREF(m_ptr);
+        return *this;
+    }
 
     /** \rst
         Attempt to cast the Python object into the given C++ type. A `cast_error`
         will be throw upon failure.
     \endrst */
-    template <typename T> T cast() const;
+    template <typename T>
+    T cast() const;
     /// Return ``true`` when the `handle` wraps a valid Python object
     explicit operator bool() const { return m_ptr != nullptr; }
     /** \rst
         Deprecated: Check that the underlying pointers are the same.
         Equivalent to ``obj1 is obj2`` in Python.
     \endrst */
     PYBIND11_DEPRECATED("Use obj1.is(obj2) instead")
     bool operator==(const handle &h) const { return m_ptr == h.m_ptr; }
     PYBIND11_DEPRECATED("Use !obj1.is(obj2) instead")
     bool operator!=(const handle &h) const { return m_ptr != h.m_ptr; }
     PYBIND11_DEPRECATED("Use handle::operator bool() instead")
     bool check() const { return m_ptr != nullptr; }
+
 protected:
     PyObject *m_ptr = nullptr;
 };
 
 /** \rst
     Holds a reference to a Python object (with reference counting)
 
@@ -238,72 +256,83 @@
     scope and is destructed. When using `object` instances consistently, it is much
     easier to get reference counting right at the first attempt.
 \endrst */
 class object : public handle {
 public:
     object() = default;
     PYBIND11_DEPRECATED("Use reinterpret_borrow<object>() or reinterpret_steal<object>()")
-    object(handle h, bool is_borrowed) : handle(h) { if (is_borrowed) inc_ref(); }
+    object(handle h, bool is_borrowed) : handle(h) {
+        if (is_borrowed) {
+            inc_ref();
+        }
+    }
     /// Copy constructor; always increases the reference count
     object(const object &o) : handle(o) { inc_ref(); }
     /// Move constructor; steals the object from ``other`` and preserves its reference count
-    object(object &&other) noexcept { m_ptr = other.m_ptr; other.m_ptr = nullptr; }
+    object(object &&other) noexcept {
+        m_ptr = other.m_ptr;
+        other.m_ptr = nullptr;
+    }
     /// Destructor; automatically calls `handle::dec_ref()`
     ~object() { dec_ref(); }
 
     /** \rst
         Resets the internal pointer to ``nullptr`` without decreasing the
         object's reference count. The function returns a raw handle to the original
         Python object.
     \endrst */
     handle release() {
-      PyObject *tmp = m_ptr;
-      m_ptr = nullptr;
-      return handle(tmp);
+        PyObject *tmp = m_ptr;
+        m_ptr = nullptr;
+        return handle(tmp);
     }
 
-    object& operator=(const object &other) {
+    object &operator=(const object &other) {
         other.inc_ref();
         // Use temporary variable to ensure `*this` remains valid while
         // `Py_XDECREF` executes, in case `*this` is accessible from Python.
         handle temp(m_ptr);
         m_ptr = other.m_ptr;
         temp.dec_ref();
         return *this;
     }
 
-    object& operator=(object &&other) noexcept {
+    object &operator=(object &&other) noexcept {
         if (this != &other) {
             handle temp(m_ptr);
             m_ptr = other.m_ptr;
             other.m_ptr = nullptr;
             temp.dec_ref();
         }
         return *this;
     }
 
     // Calling cast() on an object lvalue just copies (via handle::cast)
-    template <typename T> T cast() const &;
+    template <typename T>
+    T cast() const &;
     // Calling on an object rvalue does a move, if needed and/or possible
-    template <typename T> T cast() &&;
+    template <typename T>
+    T cast() &&;
 
 protected:
     // Tags for choosing constructors from raw PyObject *
-    struct borrowed_t { };
-    struct stolen_t { };
+    struct borrowed_t {};
+    struct stolen_t {};
 
     /// @cond BROKEN
-    template <typename T> friend T reinterpret_borrow(handle);
-    template <typename T> friend T reinterpret_steal(handle);
+    template <typename T>
+    friend T reinterpret_borrow(handle);
+    template <typename T>
+    friend T reinterpret_steal(handle);
     /// @endcond
 
 public:
     // Only accessible from derived classes and the reinterpret_* functions
     object(handle h, borrowed_t) : handle(h) { inc_ref(); }
-    object(handle h, stolen_t) : handle(h) { }
+    object(handle h, stolen_t) : handle(h) {}
 };
 
 /** \rst
     Declare that a `handle` or ``PyObject *`` is a certain type and borrow the reference.
     The target type ``T`` must be `object` or one of its derived classes. The function
     doesn't do any conversions or checks. It's up to the user to make sure that the
     target type is correct.
@@ -311,33 +340,41 @@
     .. code-block:: cpp
 
         PyObject *p = PyList_GetItem(obj, index);
         py::object o = reinterpret_borrow<py::object>(p);
         // or
         py::tuple t = reinterpret_borrow<py::tuple>(p); // <-- `p` must be already be a `tuple`
 \endrst */
-template <typename T> T reinterpret_borrow(handle h) { return {h, object::borrowed_t{}}; }
+template <typename T>
+T reinterpret_borrow(handle h) {
+    return {h, object::borrowed_t{}};
+}
 
 /** \rst
     Like `reinterpret_borrow`, but steals the reference.
 
      .. code-block:: cpp
 
         PyObject *p = PyObject_Str(obj);
         py::str s = reinterpret_steal<py::str>(p); // <-- `p` must be already be a `str`
 \endrst */
-template <typename T> T reinterpret_steal(handle h) { return {h, object::stolen_t{}}; }
+template <typename T>
+T reinterpret_steal(handle h) {
+    return {h, object::stolen_t{}};
+}
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 std::string error_string();
 PYBIND11_NAMESPACE_END(detail)
 
 #if defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4275 4251) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#    pragma warning(push)
+#    pragma warning(disable : 4275 4251)
+//     warning C4275: An exported class was derived from a class that wasn't exported.
+//     Can be ignored when derived from a STL class.
 #endif
 /// Fetch and hold an error which was already set in Python.  An instance of this is typically
 /// thrown to propagate python-side errors back through C++ which can either be caught manually or
 /// else falls back to the function dispatcher (which then raises the captured error back to
 /// python).
 class PYBIND11_EXPORT_EXCEPTION error_already_set : public std::runtime_error {
 public:
@@ -351,27 +388,30 @@
     error_already_set(error_already_set &&) = default;
 
     inline ~error_already_set() override;
 
     /// Give the currently-held error back to Python, if any.  If there is currently a Python error
     /// already set it is cleared first.  After this call, the current object no longer stores the
     /// error variables (but the `.what()` string is still available).
-    void restore() { PyErr_Restore(m_type.release().ptr(), m_value.release().ptr(), m_trace.release().ptr()); }
+    void restore() {
+        PyErr_Restore(m_type.release().ptr(), m_value.release().ptr(), m_trace.release().ptr());
+    }
 
-    /// If it is impossible to raise the currently-held error, such as in a destructor, we can write
-    /// it out using Python's unraisable hook (`sys.unraisablehook`). The error context should be
-    /// some object whose `repr()` helps identify the location of the error. Python already knows the
-    /// type and value of the error, so there is no need to repeat that. After this call, the current
-    /// object no longer stores the error variables, and neither does Python.
+    /// If it is impossible to raise the currently-held error, such as in a destructor, we can
+    /// write it out using Python's unraisable hook (`sys.unraisablehook`). The error context
+    /// should be some object whose `repr()` helps identify the location of the error. Python
+    /// already knows the type and value of the error, so there is no need to repeat that. After
+    /// this call, the current object no longer stores the error variables, and neither does
+    /// Python.
     void discard_as_unraisable(object err_context) {
         restore();
         PyErr_WriteUnraisable(err_context.ptr());
     }
-    /// An alternate version of `discard_as_unraisable()`, where a string provides information on the
-    /// location of the error. For example, `__func__` could be helpful.
+    /// An alternate version of `discard_as_unraisable()`, where a string provides information on
+    /// the location of the error. For example, `__func__` could be helpful.
     void discard_as_unraisable(const char *err_context) {
         discard_as_unraisable(reinterpret_steal<object>(PYBIND11_FROM_STRING(err_context)));
     }
 
     // Does nothing; provided for backwards compatibility.
     PYBIND11_DEPRECATED("Use of error_already_set.clear() is deprecated")
     void clear() {}
@@ -379,23 +419,23 @@
     /// Check if the currently trapped error type matches the given Python exception class (or a
     /// subclass thereof).  May also be passed a tuple to search for any exception class matches in
     /// the given tuple.
     bool matches(handle exc) const {
         return (PyErr_GivenExceptionMatches(m_type.ptr(), exc.ptr()) != 0);
     }
 
-    const object& type() const { return m_type; }
-    const object& value() const { return m_value; }
-    const object& trace() const { return m_trace; }
+    const object &type() const { return m_type; }
+    const object &value() const { return m_value; }
+    const object &trace() const { return m_trace; }
 
 private:
     object m_type, m_value, m_trace;
 };
 #if defined(_MSC_VER)
-#  pragma warning(pop)
+#    pragma warning(pop)
 #endif
 
 #if PY_VERSION_HEX >= 0x03030000
 
 /// Replaces the current Python error indicator with the chosen error, performing a
 /// 'raise from' to indicate that the chosen error was caused by the original error.
 inline void raise_from(PyObject *type, const char *message) {
@@ -424,15 +464,15 @@
     PyErr_Restore(exc, val2, tb);
 }
 
 /// Sets the current Python error indicator with the chosen error, performing a 'raise from'
 /// from the error contained in error_already_set to indicate that the chosen error was
 /// caused by the original error. After this function is called error_already_set will
 /// no longer contain an error.
-inline void raise_from(error_already_set& err, PyObject *type, const char *message) {
+inline void raise_from(error_already_set &err, PyObject *type, const char *message) {
     err.restore();
     raise_from(type, message);
 }
 
 #endif
 
 /** \defgroup python_builtins const_name
@@ -442,58 +482,75 @@
 
 /** \ingroup python_builtins
     \rst
     Return true if ``obj`` is an instance of ``T``. Type ``T`` must be a subclass of
     `object` or a class which was exposed to Python as ``py::class_<T>``.
 \endrst */
 template <typename T, detail::enable_if_t<std::is_base_of<object, T>::value, int> = 0>
-bool isinstance(handle obj) { return T::check_(obj); }
+bool isinstance(handle obj) {
+    return T::check_(obj);
+}
 
 template <typename T, detail::enable_if_t<!std::is_base_of<object, T>::value, int> = 0>
-bool isinstance(handle obj) { return detail::isinstance_generic(obj, typeid(T)); }
+bool isinstance(handle obj) {
+    return detail::isinstance_generic(obj, typeid(T));
+}
 
-template <> inline bool isinstance<handle>(handle) = delete;
-template <> inline bool isinstance<object>(handle obj) { return obj.ptr() != nullptr; }
+template <>
+inline bool isinstance<handle>(handle) = delete;
+template <>
+inline bool isinstance<object>(handle obj) {
+    return obj.ptr() != nullptr;
+}
 
 /// \ingroup python_builtins
 /// Return true if ``obj`` is an instance of the ``type``.
 inline bool isinstance(handle obj, handle type) {
     const auto result = PyObject_IsInstance(obj.ptr(), type.ptr());
-    if (result == -1)
+    if (result == -1) {
         throw error_already_set();
+    }
     return result != 0;
 }
 
 /// \addtogroup python_builtins
 /// @{
 inline bool hasattr(handle obj, handle name) {
     return PyObject_HasAttr(obj.ptr(), name.ptr()) == 1;
 }
 
 inline bool hasattr(handle obj, const char *name) {
     return PyObject_HasAttrString(obj.ptr(), name) == 1;
 }
 
 inline void delattr(handle obj, handle name) {
-    if (PyObject_DelAttr(obj.ptr(), name.ptr()) != 0) { throw error_already_set(); }
+    if (PyObject_DelAttr(obj.ptr(), name.ptr()) != 0) {
+        throw error_already_set();
+    }
 }
 
 inline void delattr(handle obj, const char *name) {
-    if (PyObject_DelAttrString(obj.ptr(), name) != 0) { throw error_already_set(); }
+    if (PyObject_DelAttrString(obj.ptr(), name) != 0) {
+        throw error_already_set();
+    }
 }
 
 inline object getattr(handle obj, handle name) {
     PyObject *result = PyObject_GetAttr(obj.ptr(), name.ptr());
-    if (!result) { throw error_already_set(); }
+    if (!result) {
+        throw error_already_set();
+    }
     return reinterpret_steal<object>(result);
 }
 
 inline object getattr(handle obj, const char *name) {
     PyObject *result = PyObject_GetAttrString(obj.ptr(), name);
-    if (!result) { throw error_already_set(); }
+    if (!result) {
+        throw error_already_set();
+    }
     return reinterpret_steal<object>(result);
 }
 
 inline object getattr(handle obj, handle name, handle default_) {
     if (PyObject *result = PyObject_GetAttr(obj.ptr(), name.ptr())) {
         return reinterpret_steal<object>(result);
     }
@@ -506,49 +563,55 @@
         return reinterpret_steal<object>(result);
     }
     PyErr_Clear();
     return reinterpret_borrow<object>(default_);
 }
 
 inline void setattr(handle obj, handle name, handle value) {
-    if (PyObject_SetAttr(obj.ptr(), name.ptr(), value.ptr()) != 0) { throw error_already_set(); }
+    if (PyObject_SetAttr(obj.ptr(), name.ptr(), value.ptr()) != 0) {
+        throw error_already_set();
+    }
 }
 
 inline void setattr(handle obj, const char *name, handle value) {
-    if (PyObject_SetAttrString(obj.ptr(), name, value.ptr()) != 0) { throw error_already_set(); }
+    if (PyObject_SetAttrString(obj.ptr(), name, value.ptr()) != 0) {
+        throw error_already_set();
+    }
 }
 
 inline ssize_t hash(handle obj) {
     auto h = PyObject_Hash(obj.ptr());
-    if (h == -1) { throw error_already_set(); }
+    if (h == -1) {
+        throw error_already_set();
+    }
     return h;
 }
 
 /// @} python_builtins
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 inline handle get_function(handle value) {
     if (value) {
 #if PY_MAJOR_VERSION >= 3
-        if (PyInstanceMethod_Check(value.ptr()))
+        if (PyInstanceMethod_Check(value.ptr())) {
             value = PyInstanceMethod_GET_FUNCTION(value.ptr());
-        else
+        } else
 #endif
-        if (PyMethod_Check(value.ptr()))
+            if (PyMethod_Check(value.ptr())) {
             value = PyMethod_GET_FUNCTION(value.ptr());
+        }
     }
     return value;
 }
 
 // Reimplementation of python's dict helper functions to ensure that exceptions
 // aren't swallowed (see #2862)
 
 // copied from cpython _PyDict_GetItemStringWithError
-inline PyObject * dict_getitemstring(PyObject *v, const char *key)
-{
+inline PyObject *dict_getitemstring(PyObject *v, const char *key) {
 #if PY_MAJOR_VERSION >= 3
     PyObject *kv = nullptr, *rv = nullptr;
     kv = PyUnicode_FromString(key);
     if (kv == NULL) {
         throw error_already_set();
     }
 
@@ -559,93 +622,105 @@
     }
     return rv;
 #else
     return PyDict_GetItemString(v, key);
 #endif
 }
 
-inline PyObject * dict_getitem(PyObject *v, PyObject *key)
-{
+inline PyObject *dict_getitem(PyObject *v, PyObject *key) {
 #if PY_MAJOR_VERSION >= 3
     PyObject *rv = PyDict_GetItemWithError(v, key);
     if (rv == NULL && PyErr_Occurred()) {
         throw error_already_set();
     }
     return rv;
 #else
     return PyDict_GetItem(v, key);
 #endif
 }
 
-// Helper aliases/functions to support implicit casting of values given to python accessors/methods.
-// When given a pyobject, this simply returns the pyobject as-is; for other C++ type, the value goes
-// through pybind11::cast(obj) to convert it to an `object`.
+// Helper aliases/functions to support implicit casting of values given to python
+// accessors/methods. When given a pyobject, this simply returns the pyobject as-is; for other C++
+// type, the value goes through pybind11::cast(obj) to convert it to an `object`.
 template <typename T, enable_if_t<is_pyobject<T>::value, int> = 0>
-auto object_or_cast(T &&o) -> decltype(std::forward<T>(o)) { return std::forward<T>(o); }
+auto object_or_cast(T &&o) -> decltype(std::forward<T>(o)) {
+    return std::forward<T>(o);
+}
 // The following casting version is implemented in cast.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int> = 0>
 object object_or_cast(T &&o);
 // Match a PyObject*, which we want to convert directly to handle via its converting constructor
 inline handle object_or_cast(PyObject *ptr) { return ptr; }
 
 #if defined(_MSC_VER) && _MSC_VER < 1920
-#  pragma warning(push)
-#  pragma warning(disable: 4522) // warning C4522: multiple assignment operators specified
+#    pragma warning(push)
+#    pragma warning(disable : 4522) // warning C4522: multiple assignment operators specified
 #endif
 template <typename Policy>
 class accessor : public object_api<accessor<Policy>> {
     using key_type = typename Policy::key_type;
 
 public:
-    accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) { }
+    accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) {}
     accessor(const accessor &) = default;
     accessor(accessor &&) noexcept = default;
 
-    // accessor overload required to override default assignment operator (templates are not allowed
-    // to replace default compiler-generated assignments).
+    // accessor overload required to override default assignment operator (templates are not
+    // allowed to replace default compiler-generated assignments).
     void operator=(const accessor &a) && { std::move(*this).operator=(handle(a)); }
     void operator=(const accessor &a) & { operator=(handle(a)); }
 
-    template <typename T> void operator=(T &&value) && {
+    template <typename T>
+    void operator=(T &&value) && {
         Policy::set(obj, key, object_or_cast(std::forward<T>(value)));
     }
-    template <typename T> void operator=(T &&value) & {
+    template <typename T>
+    void operator=(T &&value) & {
         get_cache() = reinterpret_borrow<object>(object_or_cast(std::forward<T>(value)));
     }
 
     template <typename T = Policy>
-    PYBIND11_DEPRECATED("Use of obj.attr(...) as bool is deprecated in favor of pybind11::hasattr(obj, ...)")
-    explicit operator enable_if_t<std::is_same<T, accessor_policies::str_attr>::value ||
-            std::is_same<T, accessor_policies::obj_attr>::value, bool>() const {
+    PYBIND11_DEPRECATED(
+        "Use of obj.attr(...) as bool is deprecated in favor of pybind11::hasattr(obj, ...)")
+    explicit
+    operator enable_if_t<std::is_same<T, accessor_policies::str_attr>::value
+                             || std::is_same<T, accessor_policies::obj_attr>::value,
+                         bool>() const {
         return hasattr(obj, key);
     }
     template <typename T = Policy>
     PYBIND11_DEPRECATED("Use of obj[key] as bool is deprecated in favor of obj.contains(key)")
-    explicit operator enable_if_t<std::is_same<T, accessor_policies::generic_item>::value, bool>() const {
+    explicit
+    operator enable_if_t<std::is_same<T, accessor_policies::generic_item>::value, bool>() const {
         return obj.contains(key);
     }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator object() const { return get_cache(); }
     PyObject *ptr() const { return get_cache().ptr(); }
-    template <typename T> T cast() const { return get_cache().template cast<T>(); }
+    template <typename T>
+    T cast() const {
+        return get_cache().template cast<T>();
+    }
 
 private:
     object &get_cache() const {
-        if (!cache) { cache = Policy::get(obj, key); }
+        if (!cache) {
+            cache = Policy::get(obj, key);
+        }
         return cache;
     }
 
 private:
     handle obj;
     key_type key;
     mutable object cache;
 };
 #if defined(_MSC_VER) && _MSC_VER < 1920
-#  pragma warning(pop)
+#    pragma warning(pop)
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(accessor_policies)
 struct obj_attr {
     using key_type = object;
     static object get(handle obj, handle key) { return getattr(obj, key); }
     static void set(handle obj, handle key, handle val) { setattr(obj, key, val); }
@@ -658,30 +733,36 @@
 };
 
 struct generic_item {
     using key_type = object;
 
     static object get(handle obj, handle key) {
         PyObject *result = PyObject_GetItem(obj.ptr(), key.ptr());
-        if (!result) { throw error_already_set(); }
+        if (!result) {
+            throw error_already_set();
+        }
         return reinterpret_steal<object>(result);
     }
 
     static void set(handle obj, handle key, handle val) {
-        if (PyObject_SetItem(obj.ptr(), key.ptr(), val.ptr()) != 0) { throw error_already_set(); }
+        if (PyObject_SetItem(obj.ptr(), key.ptr(), val.ptr()) != 0) {
+            throw error_already_set();
+        }
     }
 };
 
 struct sequence_item {
     using key_type = size_t;
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static object get(handle obj, const IdxType &index) {
         PyObject *result = PySequence_GetItem(obj.ptr(), ssize_t_cast(index));
-        if (!result) { throw error_already_set(); }
+        if (!result) {
+            throw error_already_set();
+        }
         return reinterpret_steal<object>(result);
     }
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static void set(handle obj, const IdxType &index, handle val) {
         // PySequence_SetItem does not steal a reference to 'val'
         if (PySequence_SetItem(obj.ptr(), ssize_t_cast(index), val.ptr()) != 0) {
@@ -692,15 +773,17 @@
 
 struct list_item {
     using key_type = size_t;
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static object get(handle obj, const IdxType &index) {
         PyObject *result = PyList_GetItem(obj.ptr(), ssize_t_cast(index));
-        if (!result) { throw error_already_set(); }
+        if (!result) {
+            throw error_already_set();
+        }
         return reinterpret_borrow<object>(result);
     }
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static void set(handle obj, const IdxType &index, handle val) {
         // PyList_SetItem steals a reference to 'val'
         if (PyList_SetItem(obj.ptr(), ssize_t_cast(index), val.inc_ref().ptr()) != 0) {
@@ -711,15 +794,17 @@
 
 struct tuple_item {
     using key_type = size_t;
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static object get(handle obj, const IdxType &index) {
         PyObject *result = PyTuple_GetItem(obj.ptr(), ssize_t_cast(index));
-        if (!result) { throw error_already_set(); }
+        if (!result) {
+            throw error_already_set();
+        }
         return reinterpret_borrow<object>(result);
     }
 
     template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     static void set(handle obj, const IdxType &index, handle val) {
         // PyTuple_SetItem steals a reference to 'val'
         if (PyTuple_SetItem(obj.ptr(), ssize_t_cast(index), val.inc_ref().ptr()) != 0) {
@@ -738,62 +823,88 @@
     using difference_type = ssize_t;
     using iterator_category = typename Policy::iterator_category;
     using value_type = typename Policy::value_type;
     using reference = typename Policy::reference;
     using pointer = typename Policy::pointer;
 
     generic_iterator() = default;
-    generic_iterator(handle seq, ssize_t index) : Policy(seq, index) { }
+    generic_iterator(handle seq, ssize_t index) : Policy(seq, index) {}
 
     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator*() const { return Policy::dereference(); }
     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator[](difference_type n) const { return *(*this + n); }
     pointer operator->() const { return **this; }
 
-    It &operator++() { Policy::increment(); return *this; }
-    It operator++(int) { auto copy = *this; Policy::increment(); return copy; }
-    It &operator--() { Policy::decrement(); return *this; }
-    It operator--(int) { auto copy = *this; Policy::decrement(); return copy; }
-    It &operator+=(difference_type n) { Policy::advance(n); return *this; }
-    It &operator-=(difference_type n) { Policy::advance(-n); return *this; }
+    It &operator++() {
+        Policy::increment();
+        return *this;
+    }
+    It operator++(int) {
+        auto copy = *this;
+        Policy::increment();
+        return copy;
+    }
+    It &operator--() {
+        Policy::decrement();
+        return *this;
+    }
+    It operator--(int) {
+        auto copy = *this;
+        Policy::decrement();
+        return copy;
+    }
+    It &operator+=(difference_type n) {
+        Policy::advance(n);
+        return *this;
+    }
+    It &operator-=(difference_type n) {
+        Policy::advance(-n);
+        return *this;
+    }
 
-    friend It operator+(const It &a, difference_type n) { auto copy = a; return copy += n; }
+    friend It operator+(const It &a, difference_type n) {
+        auto copy = a;
+        return copy += n;
+    }
     friend It operator+(difference_type n, const It &b) { return b + n; }
-    friend It operator-(const It &a, difference_type n) { auto copy = a; return copy -= n; }
+    friend It operator-(const It &a, difference_type n) {
+        auto copy = a;
+        return copy -= n;
+    }
     friend difference_type operator-(const It &a, const It &b) { return a.distance_to(b); }
 
     friend bool operator==(const It &a, const It &b) { return a.equal(b); }
     friend bool operator!=(const It &a, const It &b) { return !(a == b); }
-    friend bool operator< (const It &a, const It &b) { return b - a > 0; }
-    friend bool operator> (const It &a, const It &b) { return b < a; }
+    friend bool operator<(const It &a, const It &b) { return b - a > 0; }
+    friend bool operator>(const It &a, const It &b) { return b < a; }
     friend bool operator>=(const It &a, const It &b) { return !(a < b); }
     friend bool operator<=(const It &a, const It &b) { return !(a > b); }
 };
 
 PYBIND11_NAMESPACE_BEGIN(iterator_policies)
 /// Quick proxy class needed to implement ``operator->`` for iterators which can't return pointers
 template <typename T>
 struct arrow_proxy {
     T value;
 
     // NOLINTNEXTLINE(google-explicit-constructor)
-    arrow_proxy(T &&value) noexcept : value(std::move(value)) { }
+    arrow_proxy(T &&value) noexcept : value(std::move(value)) {}
     T *operator->() const { return &value; }
 };
 
 /// Lightweight iterator policy using just a simple pointer: see ``PySequence_Fast_ITEMS``
 class sequence_fast_readonly {
 protected:
     using iterator_category = std::random_access_iterator_tag;
     using value_type = handle;
     using reference = const handle; // PR #3263
     using pointer = arrow_proxy<const handle>;
 
-    sequence_fast_readonly(handle obj, ssize_t n) : ptr(PySequence_Fast_ITEMS(obj.ptr()) + n) { }
+    sequence_fast_readonly(handle obj, ssize_t n) : ptr(PySequence_Fast_ITEMS(obj.ptr()) + n) {}
 
     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference dereference() const { return *ptr; }
     void increment() { ++ptr; }
     void decrement() { --ptr; }
     void advance(ssize_t n) { ptr += n; }
     bool equal(const sequence_fast_readonly &b) const { return ptr == b.ptr; }
@@ -807,15 +918,15 @@
 class sequence_slow_readwrite {
 protected:
     using iterator_category = std::random_access_iterator_tag;
     using value_type = object;
     using reference = sequence_accessor;
     using pointer = arrow_proxy<const sequence_accessor>;
 
-    sequence_slow_readwrite(handle obj, ssize_t index) : obj(obj), index(index) { }
+    sequence_slow_readwrite(handle obj, ssize_t index) : obj(obj), index(index) {}
 
     reference dereference() const { return {obj, static_cast<size_t>(index)}; }
     void increment() { ++index; }
     void decrement() { --index; }
     void advance(ssize_t n) { index += n; }
     bool equal(const sequence_slow_readwrite &b) const { return index == b.index; }
     ssize_t distance_to(const sequence_slow_readwrite &b) const { return index - b.index; }
@@ -873,101 +984,113 @@
     return false;
 }
 
 inline bool PyNone_Check(PyObject *o) { return o == Py_None; }
 inline bool PyEllipsis_Check(PyObject *o) { return o == Py_Ellipsis; }
 
 #ifdef PYBIND11_STR_LEGACY_PERMISSIVE
-inline bool PyUnicode_Check_Permissive(PyObject *o) { return PyUnicode_Check(o) || PYBIND11_BYTES_CHECK(o); }
-#define PYBIND11_STR_CHECK_FUN detail::PyUnicode_Check_Permissive
+inline bool PyUnicode_Check_Permissive(PyObject *o) {
+    return PyUnicode_Check(o) || PYBIND11_BYTES_CHECK(o);
+}
+#    define PYBIND11_STR_CHECK_FUN detail::PyUnicode_Check_Permissive
 #else
-#define PYBIND11_STR_CHECK_FUN PyUnicode_Check
+#    define PYBIND11_STR_CHECK_FUN PyUnicode_Check
 #endif
 
 inline bool PyStaticMethod_Check(PyObject *o) { return o->ob_type == &PyStaticMethod_Type; }
 
 class kwargs_proxy : public handle {
 public:
-    explicit kwargs_proxy(handle h) : handle(h) { }
+    explicit kwargs_proxy(handle h) : handle(h) {}
 };
 
 class args_proxy : public handle {
 public:
-    explicit args_proxy(handle h) : handle(h) { }
+    explicit args_proxy(handle h) : handle(h) {}
     kwargs_proxy operator*() const { return kwargs_proxy(*this); }
 };
 
 /// Python argument categories (using PEP 448 terms)
-template <typename T> using is_keyword = std::is_base_of<arg, T>;
-template <typename T> using is_s_unpacking = std::is_same<args_proxy, T>; // * unpacking
-template <typename T> using is_ds_unpacking = std::is_same<kwargs_proxy, T>; // ** unpacking
-template <typename T> using is_positional = satisfies_none_of<T,
-    is_keyword, is_s_unpacking, is_ds_unpacking
->;
-template <typename T> using is_keyword_or_ds = satisfies_any_of<T, is_keyword, is_ds_unpacking>;
+template <typename T>
+using is_keyword = std::is_base_of<arg, T>;
+template <typename T>
+using is_s_unpacking = std::is_same<args_proxy, T>; // * unpacking
+template <typename T>
+using is_ds_unpacking = std::is_same<kwargs_proxy, T>; // ** unpacking
+template <typename T>
+using is_positional = satisfies_none_of<T, is_keyword, is_s_unpacking, is_ds_unpacking>;
+template <typename T>
+using is_keyword_or_ds = satisfies_any_of<T, is_keyword, is_ds_unpacking>;
 
 // Call argument collector forward declarations
 template <return_value_policy policy = return_value_policy::automatic_reference>
 class simple_collector;
 template <return_value_policy policy = return_value_policy::automatic_reference>
 class unpacking_collector;
 
 PYBIND11_NAMESPACE_END(detail)
 
 // TODO: After the deprecated constructors are removed, this macro can be simplified by
 //       inheriting ctors: `using Parent::Parent`. It's not an option right now because
 //       the `using` statement triggers the parent deprecation warning even if the ctor
 //       isn't even used.
-#define PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
-    public: \
-        PYBIND11_DEPRECATED("Use reinterpret_borrow<"#Name">() or reinterpret_steal<"#Name">()") \
-        Name(handle h, bool is_borrowed) : Parent(is_borrowed ? Parent(h, borrowed_t{}) : Parent(h, stolen_t{})) { } \
-        Name(handle h, borrowed_t) : Parent(h, borrowed_t{}) { } \
-        Name(handle h, stolen_t) : Parent(h, stolen_t{}) { } \
-        PYBIND11_DEPRECATED("Use py::isinstance<py::python_type>(obj) instead") \
-        bool check() const { return m_ptr != nullptr && (CheckFun(m_ptr) != 0); } \
-        static bool check_(handle h) { return h.ptr() != nullptr && CheckFun(h.ptr()); } \
-        template <typename Policy_> \
-        /* NOLINTNEXTLINE(google-explicit-constructor) */ \
-        Name(const ::pybind11::detail::accessor<Policy_> &a) : Name(object(a)) { }
-
-#define PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
-    PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
-    /* This is deliberately not 'explicit' to allow implicit conversion from object: */ \
-    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
-    Name(const object &o) \
-    : Parent(check_(o) ? o.inc_ref().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
-    { if (!m_ptr) throw error_already_set(); } \
-    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
-    Name(object &&o) \
-    : Parent(check_(o) ? o.release().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
-    { if (!m_ptr) throw error_already_set(); }
-
-#define PYBIND11_OBJECT_CVT_DEFAULT(Name, Parent, CheckFun, ConvertFun) \
-    PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
-    Name() : Parent() { }
-
-#define PYBIND11_OBJECT_CHECK_FAILED(Name, o_ptr) \
-    ::pybind11::type_error("Object of type '" + \
-                           ::pybind11::detail::get_fully_qualified_tp_name(Py_TYPE(o_ptr)) + \
-                           "' is not an instance of '" #Name "'")
-
-#define PYBIND11_OBJECT(Name, Parent, CheckFun) \
-    PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
-    /* This is deliberately not 'explicit' to allow implicit conversion from object: */ \
-    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
-    Name(const object &o) : Parent(o) \
-    { if (m_ptr && !check_(m_ptr)) throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr); } \
-    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
-    Name(object &&o) : Parent(std::move(o)) \
-    { if (m_ptr && !check_(m_ptr)) throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr); }
-
-#define PYBIND11_OBJECT_DEFAULT(Name, Parent, CheckFun) \
-    PYBIND11_OBJECT(Name, Parent, CheckFun) \
-    Name() : Parent() { }
+#define PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun)                                            \
+public:                                                                                           \
+    PYBIND11_DEPRECATED("Use reinterpret_borrow<" #Name ">() or reinterpret_steal<" #Name ">()")  \
+    Name(handle h, bool is_borrowed)                                                              \
+        : Parent(is_borrowed ? Parent(h, borrowed_t{}) : Parent(h, stolen_t{})) {}                \
+    Name(handle h, borrowed_t) : Parent(h, borrowed_t{}) {}                                       \
+    Name(handle h, stolen_t) : Parent(h, stolen_t{}) {}                                           \
+    PYBIND11_DEPRECATED("Use py::isinstance<py::python_type>(obj) instead")                       \
+    bool check() const { return m_ptr != nullptr && (CheckFun(m_ptr) != 0); }                     \
+    static bool check_(handle h) { return h.ptr() != nullptr && CheckFun(h.ptr()); }              \
+    template <typename Policy_> /* NOLINTNEXTLINE(google-explicit-constructor) */                 \
+    Name(const ::pybind11::detail::accessor<Policy_> &a) : Name(object(a)) {}
+
+#define PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun)                                   \
+    PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun)                                                \
+    /* This is deliberately not 'explicit' to allow implicit conversion from object: */           \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */                                             \
+    Name(const object &o)                                                                         \
+        : Parent(check_(o) ? o.inc_ref().ptr() : ConvertFun(o.ptr()), stolen_t{}) {               \
+        if (!m_ptr)                                                                               \
+            throw error_already_set();                                                            \
+    }                                                                                             \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */                                             \
+    Name(object &&o) : Parent(check_(o) ? o.release().ptr() : ConvertFun(o.ptr()), stolen_t{}) {  \
+        if (!m_ptr)                                                                               \
+            throw error_already_set();                                                            \
+    }
+
+#define PYBIND11_OBJECT_CVT_DEFAULT(Name, Parent, CheckFun, ConvertFun)                           \
+    PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun)                                       \
+    Name() : Parent() {}
+
+#define PYBIND11_OBJECT_CHECK_FAILED(Name, o_ptr)                                                 \
+    ::pybind11::type_error("Object of type '"                                                     \
+                           + ::pybind11::detail::get_fully_qualified_tp_name(Py_TYPE(o_ptr))      \
+                           + "' is not an instance of '" #Name "'")
+
+#define PYBIND11_OBJECT(Name, Parent, CheckFun)                                                   \
+    PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun)                                                \
+    /* This is deliberately not 'explicit' to allow implicit conversion from object: */           \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */                                             \
+    Name(const object &o) : Parent(o) {                                                           \
+        if (m_ptr && !check_(m_ptr))                                                              \
+            throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr);                                      \
+    }                                                                                             \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */                                             \
+    Name(object &&o) : Parent(std::move(o)) {                                                     \
+        if (m_ptr && !check_(m_ptr))                                                              \
+            throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr);                                      \
+    }
+
+#define PYBIND11_OBJECT_DEFAULT(Name, Parent, CheckFun)                                           \
+    PYBIND11_OBJECT(Name, Parent, CheckFun)                                                       \
+    Name() : Parent() {}
 
 /// \addtogroup pytypes
 /// @{
 
 /** \rst
     Wraps a Python iterator so that it can also be used as a C++ input iterator
 
@@ -982,35 +1105,38 @@
     using difference_type = ssize_t;
     using value_type = handle;
     using reference = const handle; // PR #3263
     using pointer = const handle *;
 
     PYBIND11_OBJECT_DEFAULT(iterator, object, PyIter_Check)
 
-    iterator& operator++() {
+    iterator &operator++() {
         advance();
         return *this;
     }
 
     iterator operator++(int) {
         auto rv = *this;
         advance();
         return rv;
     }
 
     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator*() const {
         if (m_ptr && !value.ptr()) {
-            auto& self = const_cast<iterator &>(*this);
+            auto &self = const_cast<iterator &>(*this);
             self.advance();
         }
         return value;
     }
 
-    pointer operator->() const { operator*(); return &value; }
+    pointer operator->() const {
+        operator*();
+        return &value;
+    }
 
     /** \rst
          The value which marks the end of the iteration. ``it == iterator::sentinel()``
          is equivalent to catching ``StopIteration`` in Python.
 
          .. code-block:: cpp
 
@@ -1025,45 +1151,47 @@
 
     friend bool operator==(const iterator &a, const iterator &b) { return a->ptr() == b->ptr(); }
     friend bool operator!=(const iterator &a, const iterator &b) { return a->ptr() != b->ptr(); }
 
 private:
     void advance() {
         value = reinterpret_steal<object>(PyIter_Next(m_ptr));
-        if (PyErr_Occurred()) { throw error_already_set(); }
+        if (PyErr_Occurred()) {
+            throw error_already_set();
+        }
     }
 
 private:
     object value = {};
 };
 
-
-
 class type : public object {
 public:
     PYBIND11_OBJECT(type, object, PyType_Check)
 
     /// Return a type handle from a handle or an object
-    static handle handle_of(handle h) { return handle((PyObject*) Py_TYPE(h.ptr())); }
+    static handle handle_of(handle h) { return handle((PyObject *) Py_TYPE(h.ptr())); }
 
     /// Return a type object from a handle or an object
     static type of(handle h) { return type(type::handle_of(h), borrowed_t{}); }
 
     // Defined in pybind11/cast.h
     /// Convert C++ type to handle if previously registered. Does not convert
     /// standard types, like int, float. etc. yet.
     /// See https://github.com/pybind/pybind11/issues/2486
-    template<typename T>
+    template <typename T>
     static handle handle_of();
 
     /// Convert C++ type to type if previously registered. Does not convert
     /// standard types, like int, float. etc. yet.
     /// See https://github.com/pybind/pybind11/issues/2486
-    template<typename T>
-    static type of() {return type(type::handle_of<T>(), borrowed_t{}); }
+    template <typename T>
+    static type of() {
+        return type(type::handle_of<T>(), borrowed_t{});
+    }
 };
 
 class iterable : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(iterable, object, detail::PyIterable_Check)
 };
 
@@ -1072,77 +1200,89 @@
 class str : public object {
 public:
     PYBIND11_OBJECT_CVT(str, object, PYBIND11_STR_CHECK_FUN, raw_str)
 
     template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     str(const char *c, const SzType &n)
         : object(PyUnicode_FromStringAndSize(c, ssize_t_cast(n)), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate string object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate string object!");
+        }
     }
 
-    // 'explicit' is explicitly omitted from the following constructors to allow implicit conversion to py::str from C++ string-like objects
+    // 'explicit' is explicitly omitted from the following constructors to allow implicit
+    // conversion to py::str from C++ string-like objects
     // NOLINTNEXTLINE(google-explicit-constructor)
-    str(const char *c = "")
-        : object(PyUnicode_FromString(c), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate string object!");
+    str(const char *c = "") : object(PyUnicode_FromString(c), stolen_t{}) {
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate string object!");
+        }
     }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
-    str(const std::string &s) : str(s.data(), s.size()) { }
+    str(const std::string &s) : str(s.data(), s.size()) {}
 
 #ifdef PYBIND11_HAS_STRING_VIEW
     // enable_if is needed to avoid "ambiguous conversion" errors (see PR #3521).
     template <typename T, detail::enable_if_t<std::is_same<T, std::string_view>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    str(T s) : str(s.data(), s.size()) { }
+    str(T s) : str(s.data(), s.size()) {}
 
-# ifdef PYBIND11_HAS_U8STRING
+#    ifdef PYBIND11_HAS_U8STRING
     // reinterpret_cast here is safe (C++20 guarantees char8_t has the same size/alignment as char)
     // NOLINTNEXTLINE(google-explicit-constructor)
-    str(std::u8string_view s) : str(reinterpret_cast<const char*>(s.data()), s.size()) { }
-# endif
+    str(std::u8string_view s) : str(reinterpret_cast<const char *>(s.data()), s.size()) {}
+#    endif
 
 #endif
 
     explicit str(const bytes &b);
 
     /** \rst
         Return a string representation of the object. This is analogous to
         the ``str()`` function in Python.
     \endrst */
-    explicit str(handle h) : object(raw_str(h.ptr()), stolen_t{}) { if (!m_ptr) throw error_already_set(); }
+    explicit str(handle h) : object(raw_str(h.ptr()), stolen_t{}) {
+        if (!m_ptr) {
+            throw error_already_set();
+        }
+    }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::string() const {
         object temp = *this;
         if (PyUnicode_Check(m_ptr)) {
             temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(m_ptr));
-            if (!temp)
+            if (!temp) {
                 throw error_already_set();
+            }
         }
         char *buffer = nullptr;
         ssize_t length = 0;
-        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
+        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length)) {
             pybind11_fail("Unable to extract string contents! (invalid type)");
+        }
         return std::string(buffer, (size_t) length);
     }
 
     template <typename... Args>
     str format(Args &&...args) const {
         return attr("format")(std::forward<Args>(args)...);
     }
 
 private:
     /// Return string representation -- always returns a new reference, even if already a str
     static PyObject *raw_str(PyObject *op) {
         PyObject *str_value = PyObject_Str(op);
 #if PY_MAJOR_VERSION < 3
-        if (!str_value) throw error_already_set();
+        if (!str_value)
+            throw error_already_set();
         PyObject *unicode = PyUnicode_FromEncodedObject(str_value, "utf-8", nullptr);
-        Py_XDECREF(str_value); str_value = unicode;
+        Py_XDECREF(str_value);
+        str_value = unicode;
 #endif
         return str_value;
     }
 };
 /// @} pytypes
 
 inline namespace literals {
@@ -1156,108 +1296,118 @@
 /// @{
 class bytes : public object {
 public:
     PYBIND11_OBJECT(bytes, object, PYBIND11_BYTES_CHECK)
 
     // Allow implicit conversion:
     // NOLINTNEXTLINE(google-explicit-constructor)
-    bytes(const char *c = "")
-        : object(PYBIND11_BYTES_FROM_STRING(c), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate bytes object!");
+    bytes(const char *c = "") : object(PYBIND11_BYTES_FROM_STRING(c), stolen_t{}) {
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate bytes object!");
+        }
     }
 
     template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     bytes(const char *c, const SzType &n)
         : object(PYBIND11_BYTES_FROM_STRING_AND_SIZE(c, ssize_t_cast(n)), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate bytes object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate bytes object!");
+        }
     }
 
     // Allow implicit conversion:
     // NOLINTNEXTLINE(google-explicit-constructor)
-    bytes(const std::string &s) : bytes(s.data(), s.size()) { }
+    bytes(const std::string &s) : bytes(s.data(), s.size()) {}
 
     explicit bytes(const pybind11::str &s);
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::string() const {
         char *buffer = nullptr;
         ssize_t length = 0;
-        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length))
+        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length)) {
             pybind11_fail("Unable to extract bytes contents!");
+        }
         return std::string(buffer, (size_t) length);
     }
 
 #ifdef PYBIND11_HAS_STRING_VIEW
     // enable_if is needed to avoid "ambiguous conversion" errors (see PR #3521).
     template <typename T, detail::enable_if_t<std::is_same<T, std::string_view>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
-    bytes(T s) : bytes(s.data(), s.size()) { }
+    bytes(T s) : bytes(s.data(), s.size()) {}
 
     // Obtain a string view that views the current `bytes` buffer value.  Note that this is only
     // valid so long as the `bytes` instance remains alive and so generally should not outlive the
     // lifetime of the `bytes` instance.
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::string_view() const {
         char *buffer = nullptr;
         ssize_t length = 0;
-        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length))
+        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length)) {
             pybind11_fail("Unable to extract bytes contents!");
+        }
         return {buffer, static_cast<size_t>(length)};
     }
 #endif
-
 };
 // Note: breathe >= 4.17.0 will fail to build docs if the below two constructors
 // are included in the doxygen group; close here and reopen after as a workaround
 /// @} pytypes
 
 inline bytes::bytes(const pybind11::str &s) {
     object temp = s;
     if (PyUnicode_Check(s.ptr())) {
         temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(s.ptr()));
-        if (!temp)
+        if (!temp) {
             pybind11_fail("Unable to extract string contents! (encoding issue)");
+        }
     }
     char *buffer = nullptr;
     ssize_t length = 0;
-    if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
+    if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length)) {
         pybind11_fail("Unable to extract string contents! (invalid type)");
+    }
     auto obj = reinterpret_steal<object>(PYBIND11_BYTES_FROM_STRING_AND_SIZE(buffer, length));
-    if (!obj)
+    if (!obj) {
         pybind11_fail("Could not allocate bytes object!");
+    }
     m_ptr = obj.release().ptr();
 }
 
-inline str::str(const bytes& b) {
+inline str::str(const bytes &b) {
     char *buffer = nullptr;
     ssize_t length = 0;
-    if (PYBIND11_BYTES_AS_STRING_AND_SIZE(b.ptr(), &buffer, &length))
+    if (PYBIND11_BYTES_AS_STRING_AND_SIZE(b.ptr(), &buffer, &length)) {
         pybind11_fail("Unable to extract bytes contents!");
+    }
     auto obj = reinterpret_steal<object>(PyUnicode_FromStringAndSize(buffer, length));
-    if (!obj)
+    if (!obj) {
         pybind11_fail("Could not allocate string object!");
+    }
     m_ptr = obj.release().ptr();
 }
 
 /// \addtogroup pytypes
 /// @{
 class bytearray : public object {
 public:
     PYBIND11_OBJECT_CVT(bytearray, object, PyByteArray_Check, PyByteArray_FromObject)
 
     template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     bytearray(const char *c, const SzType &n)
         : object(PyByteArray_FromStringAndSize(c, ssize_t_cast(n)), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate bytearray object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate bytearray object!");
+        }
     }
 
-    bytearray()
-        : bytearray("", 0) {}
+    bytearray() : bytearray("", 0) {}
 
-    explicit bytearray(const std::string &s) : bytearray(s.data(), s.size()) { }
+    explicit bytearray(const std::string &s) : bytearray(s.data(), s.size()) {}
 
     size_t size() const { return static_cast<size_t>(PyByteArray_Size(m_ptr)); }
 
     explicit operator std::string() const {
         char *buffer = PyByteArray_AS_STRING(m_ptr);
         ssize_t size = PyByteArray_GET_SIZE(m_ptr);
         return std::string(buffer, static_cast<size_t>(size));
@@ -1268,38 +1418,40 @@
 /// @} pytypes
 
 /// \addtogroup pytypes
 /// @{
 class none : public object {
 public:
     PYBIND11_OBJECT(none, object, detail::PyNone_Check)
-    none() : object(Py_None, borrowed_t{}) { }
+    none() : object(Py_None, borrowed_t{}) {}
 };
 
 class ellipsis : public object {
 public:
     PYBIND11_OBJECT(ellipsis, object, detail::PyEllipsis_Check)
-    ellipsis() : object(Py_Ellipsis, borrowed_t{}) { }
+    ellipsis() : object(Py_Ellipsis, borrowed_t{}) {}
 };
 
 class bool_ : public object {
 public:
     PYBIND11_OBJECT_CVT(bool_, object, PyBool_Check, raw_bool)
-    bool_() : object(Py_False, borrowed_t{}) { }
+    bool_() : object(Py_False, borrowed_t{}) {}
     // Allow implicit conversion from and to `bool`:
     // NOLINTNEXTLINE(google-explicit-constructor)
-    bool_(bool value) : object(value ? Py_True : Py_False, borrowed_t{}) { }
+    bool_(bool value) : object(value ? Py_True : Py_False, borrowed_t{}) {}
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator bool() const { return (m_ptr != nullptr) && PyLong_AsLong(m_ptr) != 0; }
 
 private:
     /// Return the truth value of an object -- always returns a new reference
     static PyObject *raw_bool(PyObject *op) {
         const auto value = PyObject_IsTrue(op);
-        if (value == -1) return nullptr;
+        if (value == -1) {
+            return nullptr;
+        }
         return handle(value != 0 ? Py_True : Py_False).inc_ref().ptr();
     }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Converts a value to the given unsigned type.  If an error occurs, you get back (Unsigned) -1;
 // otherwise you get back the unsigned long or unsigned long long value cast to (Unsigned).
@@ -1319,169 +1471,184 @@
     return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
 }
 PYBIND11_NAMESPACE_END(detail)
 
 class int_ : public object {
 public:
     PYBIND11_OBJECT_CVT(int_, object, PYBIND11_LONG_CHECK, PyNumber_Long)
-    int_() : object(PyLong_FromLong(0), stolen_t{}) { }
+    int_() : object(PyLong_FromLong(0), stolen_t{}) {}
     // Allow implicit conversion from C++ integral types:
-    template <typename T,
-              detail::enable_if_t<std::is_integral<T>::value, int> = 0>
+    template <typename T, detail::enable_if_t<std::is_integral<T>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     int_(T value) {
         if (PYBIND11_SILENCE_MSVC_C4127(sizeof(T) <= sizeof(long))) {
-            if (std::is_signed<T>::value)
+            if (std::is_signed<T>::value) {
                 m_ptr = PyLong_FromLong((long) value);
-            else
+            } else {
                 m_ptr = PyLong_FromUnsignedLong((unsigned long) value);
+            }
         } else {
-            if (std::is_signed<T>::value)
+            if (std::is_signed<T>::value) {
                 m_ptr = PyLong_FromLongLong((long long) value);
-            else
+            } else {
                 m_ptr = PyLong_FromUnsignedLongLong((unsigned long long) value);
+            }
+        }
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate int object!");
         }
-        if (!m_ptr) pybind11_fail("Could not allocate int object!");
     }
 
-    template <typename T,
-              detail::enable_if_t<std::is_integral<T>::value, int> = 0>
+    template <typename T, detail::enable_if_t<std::is_integral<T>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator T() const {
-        return std::is_unsigned<T>::value
-            ? detail::as_unsigned<T>(m_ptr)
-            : sizeof(T) <= sizeof(long)
-              ? (T) PyLong_AsLong(m_ptr)
-              : (T) PYBIND11_LONG_AS_LONGLONG(m_ptr);
+        return std::is_unsigned<T>::value  ? detail::as_unsigned<T>(m_ptr)
+               : sizeof(T) <= sizeof(long) ? (T) PyLong_AsLong(m_ptr)
+                                           : (T) PYBIND11_LONG_AS_LONGLONG(m_ptr);
     }
 };
 
 class float_ : public object {
 public:
     PYBIND11_OBJECT_CVT(float_, object, PyFloat_Check, PyNumber_Float)
     // Allow implicit conversion from float/double:
     // NOLINTNEXTLINE(google-explicit-constructor)
     float_(float value) : object(PyFloat_FromDouble((double) value), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate float object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate float object!");
+        }
     }
     // NOLINTNEXTLINE(google-explicit-constructor)
     float_(double value = .0) : object(PyFloat_FromDouble((double) value), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate float object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate float object!");
+        }
     }
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator float() const { return (float) PyFloat_AsDouble(m_ptr); }
     // NOLINTNEXTLINE(google-explicit-constructor)
     operator double() const { return (double) PyFloat_AsDouble(m_ptr); }
 };
 
 class weakref : public object {
 public:
     PYBIND11_OBJECT_CVT_DEFAULT(weakref, object, PyWeakref_Check, raw_weakref)
     explicit weakref(handle obj, handle callback = {})
         : object(PyWeakref_NewRef(obj.ptr(), callback.ptr()), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate weak reference!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate weak reference!");
+        }
     }
 
 private:
-    static PyObject *raw_weakref(PyObject *o) {
-        return PyWeakref_NewRef(o, nullptr);
-    }
+    static PyObject *raw_weakref(PyObject *o) { return PyWeakref_NewRef(o, nullptr); }
 };
 
 class slice : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(slice, object, PySlice_Check)
     slice(handle start, handle stop, handle step) {
         m_ptr = PySlice_New(start.ptr(), stop.ptr(), step.ptr());
-        if (!m_ptr)
+        if (!m_ptr) {
             pybind11_fail("Could not allocate slice object!");
+        }
     }
 
 #ifdef PYBIND11_HAS_OPTIONAL
     slice(std::optional<ssize_t> start, std::optional<ssize_t> stop, std::optional<ssize_t> step)
         : slice(index_to_object(start), index_to_object(stop), index_to_object(step)) {}
 #else
     slice(ssize_t start_, ssize_t stop_, ssize_t step_)
         : slice(int_(start_), int_(stop_), int_(step_)) {}
 #endif
 
-    bool compute(size_t length, size_t *start, size_t *stop, size_t *step,
-                 size_t *slicelength) const {
+    bool
+    compute(size_t length, size_t *start, size_t *stop, size_t *step, size_t *slicelength) const {
         return PySlice_GetIndicesEx((PYBIND11_SLICE_OBJECT *) m_ptr,
-                                    (ssize_t) length, (ssize_t *) start,
-                                    (ssize_t *) stop, (ssize_t *) step,
-                                    (ssize_t *) slicelength) == 0;
-    }
-    bool compute(ssize_t length, ssize_t *start, ssize_t *stop, ssize_t *step,
-      ssize_t *slicelength) const {
-      return PySlice_GetIndicesEx((PYBIND11_SLICE_OBJECT *) m_ptr,
-          length, start,
-          stop, step,
-          slicelength) == 0;
+                                    (ssize_t) length,
+                                    (ssize_t *) start,
+                                    (ssize_t *) stop,
+                                    (ssize_t *) step,
+                                    (ssize_t *) slicelength)
+               == 0;
+    }
+    bool compute(
+        ssize_t length, ssize_t *start, ssize_t *stop, ssize_t *step, ssize_t *slicelength) const {
+        return PySlice_GetIndicesEx(
+                   (PYBIND11_SLICE_OBJECT *) m_ptr, length, start, stop, step, slicelength)
+               == 0;
     }
 
 private:
     template <typename T>
     static object index_to_object(T index) {
         return index ? object(int_(*index)) : object(none());
     }
 };
 
 class capsule : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(capsule, object, PyCapsule_CheckExact)
     PYBIND11_DEPRECATED("Use reinterpret_borrow<capsule>() or reinterpret_steal<capsule>()")
-    capsule(PyObject *ptr, bool is_borrowed) : object(is_borrowed ? object(ptr, borrowed_t{}) : object(ptr, stolen_t{})) { }
+    capsule(PyObject *ptr, bool is_borrowed)
+        : object(is_borrowed ? object(ptr, borrowed_t{}) : object(ptr, stolen_t{})) {}
 
-    explicit capsule(const void *value, const char *name = nullptr, void (*destructor)(PyObject *) = nullptr)
+    explicit capsule(const void *value,
+                     const char *name = nullptr,
+                     void (*destructor)(PyObject *) = nullptr)
         : object(PyCapsule_New(const_cast<void *>(value), name, destructor), stolen_t{}) {
-        if (!m_ptr)
+        if (!m_ptr) {
             pybind11_fail("Could not allocate capsule object!");
+        }
     }
 
     PYBIND11_DEPRECATED("Please pass a destructor that takes a void pointer as input")
     capsule(const void *value, void (*destruct)(PyObject *))
-        : object(PyCapsule_New(const_cast<void*>(value), nullptr, destruct), stolen_t{}) {
-        if (!m_ptr)
+        : object(PyCapsule_New(const_cast<void *>(value), nullptr, destruct), stolen_t{}) {
+        if (!m_ptr) {
             pybind11_fail("Could not allocate capsule object!");
+        }
     }
 
     capsule(const void *value, void (*destructor)(void *)) {
         m_ptr = PyCapsule_New(const_cast<void *>(value), nullptr, [](PyObject *o) {
             auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
             void *ptr = PyCapsule_GetPointer(o, nullptr);
             destructor(ptr);
         });
 
-        if (!m_ptr)
+        if (!m_ptr) {
             pybind11_fail("Could not allocate capsule object!");
+        }
 
-        if (PyCapsule_SetContext(m_ptr, (void *) destructor) != 0)
+        if (PyCapsule_SetContext(m_ptr, (void *) destructor) != 0) {
             pybind11_fail("Could not set capsule context!");
+        }
     }
 
     explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             auto destructor = reinterpret_cast<void (*)()>(PyCapsule_GetPointer(o, nullptr));
             destructor();
         });
 
-        if (!m_ptr)
+        if (!m_ptr) {
             pybind11_fail("Could not allocate capsule object!");
+        }
     }
 
-    // NOLINTNEXTLINE(google-explicit-constructor)
-    template <typename T> operator T *() const {
+    template <typename T>
+    operator T *() const { // NOLINT(google-explicit-constructor)
         return get_pointer<T>();
     }
 
     /// Get the pointer the capsule holds.
-    template<typename T = void>
-    T* get_pointer() const {
-        auto name = this->name();
+    template <typename T = void>
+    T *get_pointer() const {
+        const auto *name = this->name();
         T *result = static_cast<T *>(PyCapsule_GetPointer(m_ptr, name));
         if (!result) {
             PyErr_Clear();
             pybind11_fail("Unable to extract capsule contents!");
         }
         return result;
     }
@@ -1500,70 +1667,77 @@
 class tuple : public object {
 public:
     PYBIND11_OBJECT_CVT(tuple, object, PyTuple_Check, PySequence_Tuple)
     template <typename SzType = ssize_t,
               detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     // Some compilers generate link errors when using `const SzType &` here:
     explicit tuple(SzType size = 0) : object(PyTuple_New(ssize_t_cast(size)), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate tuple object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate tuple object!");
+        }
     }
     size_t size() const { return (size_t) PyTuple_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::tuple_accessor operator[](size_t index) const { return {*this, index}; }
     detail::item_accessor operator[](handle h) const { return object::operator[](h); }
     detail::tuple_iterator begin() const { return {*this, 0}; }
     detail::tuple_iterator end() const { return {*this, PyTuple_GET_SIZE(m_ptr)}; }
 };
 
 // We need to put this into a separate function because the Intel compiler
 // fails to compile enable_if_t<all_of<is_keyword_or_ds<Args>...>::value> part below
 // (tested with ICC 2021.1 Beta 20200827).
 template <typename... Args>
-constexpr bool args_are_all_keyword_or_ds()
-{
-  return detail::all_of<detail::is_keyword_or_ds<Args>...>::value;
+constexpr bool args_are_all_keyword_or_ds() {
+    return detail::all_of<detail::is_keyword_or_ds<Args>...>::value;
 }
 
 class dict : public object {
 public:
     PYBIND11_OBJECT_CVT(dict, object, PyDict_Check, raw_dict)
     dict() : object(PyDict_New(), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate dict object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate dict object!");
+        }
     }
     template <typename... Args,
               typename = detail::enable_if_t<args_are_all_keyword_or_ds<Args...>()>,
-              // MSVC workaround: it can't compile an out-of-line definition, so defer the collector
+              // MSVC workaround: it can't compile an out-of-line definition, so defer the
+              // collector
               typename collector = detail::deferred_t<detail::unpacking_collector<>, Args...>>
-    explicit dict(Args &&...args) : dict(collector(std::forward<Args>(args)...).kwargs()) { }
+    explicit dict(Args &&...args) : dict(collector(std::forward<Args>(args)...).kwargs()) {}
 
     size_t size() const { return (size_t) PyDict_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::dict_iterator begin() const { return {*this, 0}; }
     detail::dict_iterator end() const { return {}; }
     void clear() /* py-non-const */ { PyDict_Clear(ptr()); }
-    template <typename T> bool contains(T &&key) const {
+    template <typename T>
+    bool contains(T &&key) const {
         return PyDict_Contains(m_ptr, detail::object_or_cast(std::forward<T>(key)).ptr()) == 1;
     }
 
 private:
     /// Call the `dict` Python type -- always returns a new reference
     static PyObject *raw_dict(PyObject *op) {
-        if (PyDict_Check(op))
+        if (PyDict_Check(op)) {
             return handle(op).inc_ref().ptr();
+        }
         return PyObject_CallFunctionObjArgs((PyObject *) &PyDict_Type, op, nullptr);
     }
 };
 
 class sequence : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(sequence, object, PySequence_Check)
     size_t size() const {
         ssize_t result = PySequence_Size(m_ptr);
-        if (result == -1)
+        if (result == -1) {
             throw error_already_set();
+        }
         return (size_t) result;
     }
     bool empty() const { return size() == 0; }
     detail::sequence_accessor operator[](size_t index) const { return {*this, index}; }
     detail::item_accessor operator[](handle h) const { return object::operator[](h); }
     detail::sequence_iterator begin() const { return {*this, 0}; }
     detail::sequence_iterator end() const { return {*this, PySequence_Size(m_ptr)}; }
@@ -1572,61 +1746,73 @@
 class list : public object {
 public:
     PYBIND11_OBJECT_CVT(list, object, PyList_Check, PySequence_List)
     template <typename SzType = ssize_t,
               detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     // Some compilers generate link errors when using `const SzType &` here:
     explicit list(SzType size = 0) : object(PyList_New(ssize_t_cast(size)), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate list object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate list object!");
+        }
     }
     size_t size() const { return (size_t) PyList_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::list_accessor operator[](size_t index) const { return {*this, index}; }
     detail::item_accessor operator[](handle h) const { return object::operator[](h); }
     detail::list_iterator begin() const { return {*this, 0}; }
     detail::list_iterator end() const { return {*this, PyList_GET_SIZE(m_ptr)}; }
-    template <typename T> void append(T &&val) /* py-non-const */ {
+    template <typename T>
+    void append(T &&val) /* py-non-const */ {
         PyList_Append(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr());
     }
     template <typename IdxType,
               typename ValType,
               detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     void insert(const IdxType &index, ValType &&val) /* py-non-const */ {
         PyList_Insert(
             m_ptr, ssize_t_cast(index), detail::object_or_cast(std::forward<ValType>(val)).ptr());
     }
 };
 
-class args : public tuple { PYBIND11_OBJECT_DEFAULT(args, tuple, PyTuple_Check) };
-class kwargs : public dict { PYBIND11_OBJECT_DEFAULT(kwargs, dict, PyDict_Check)  };
+class args : public tuple {
+    PYBIND11_OBJECT_DEFAULT(args, tuple, PyTuple_Check)
+};
+class kwargs : public dict {
+    PYBIND11_OBJECT_DEFAULT(kwargs, dict, PyDict_Check)
+};
 
 class set : public object {
 public:
     PYBIND11_OBJECT_CVT(set, object, PySet_Check, PySet_New)
     set() : object(PySet_New(nullptr), stolen_t{}) {
-        if (!m_ptr) pybind11_fail("Could not allocate set object!");
+        if (!m_ptr) {
+            pybind11_fail("Could not allocate set object!");
+        }
     }
     size_t size() const { return (size_t) PySet_Size(m_ptr); }
     bool empty() const { return size() == 0; }
-    template <typename T> bool add(T &&val) /* py-non-const */ {
+    template <typename T>
+    bool add(T &&val) /* py-non-const */ {
         return PySet_Add(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) == 0;
     }
     void clear() /* py-non-const */ { PySet_Clear(m_ptr); }
-    template <typename T> bool contains(T &&val) const {
+    template <typename T>
+    bool contains(T &&val) const {
         return PySet_Contains(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) == 1;
     }
 };
 
 class function : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(function, object, PyCallable_Check)
     handle cpp_function() const {
         handle fun = detail::get_function(m_ptr);
-        if (fun && PyCFunction_Check(fun.ptr()))
+        if (fun && PyCFunction_Check(fun.ptr())) {
             return fun;
+        }
         return handle();
     }
     bool is_cpp_function() const { return (bool) cpp_function(); }
 };
 
 class staticmethod : public object {
 public:
@@ -1635,15 +1821,17 @@
 
 class buffer : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(buffer, object, PyObject_CheckBuffer)
 
     buffer_info request(bool writable = false) const {
         int flags = PyBUF_STRIDES | PyBUF_FORMAT;
-        if (writable) flags |= PyBUF_WRITABLE;
+        if (writable) {
+            flags |= PyBUF_WRITABLE;
+        }
         auto *view = new Py_buffer();
         if (PyObject_GetBuffer(m_ptr, view, flags) != 0) {
             delete view;
             throw error_already_set();
         }
         return buffer_info(view);
     }
@@ -1658,153 +1846,168 @@
 
         ``buffer_info`` must be created from ``buffer::request()``. Otherwise
         throws an exception.
 
         For creating a ``memoryview`` from objects that support buffer protocol,
         use ``memoryview(const object& obj)`` instead of this constructor.
      \endrst */
-    explicit memoryview(const buffer_info& info) {
-        if (!info.view())
+    explicit memoryview(const buffer_info &info) {
+        if (!info.view()) {
             pybind11_fail("Prohibited to create memoryview without Py_buffer");
+        }
         // Note: PyMemoryView_FromBuffer never increments obj reference.
-        m_ptr = (info.view()->obj) ?
-            PyMemoryView_FromObject(info.view()->obj) :
-            PyMemoryView_FromBuffer(info.view());
-        if (!m_ptr)
+        m_ptr = (info.view()->obj) ? PyMemoryView_FromObject(info.view()->obj)
+                                   : PyMemoryView_FromBuffer(info.view());
+        if (!m_ptr) {
             pybind11_fail("Unable to create memoryview from buffer descriptor");
+        }
     }
 
     /** \rst
         Creates ``memoryview`` from static buffer.
 
         This method is meant for providing a ``memoryview`` for C/C++ buffer not
         managed by Python. The caller is responsible for managing the lifetime
         of ``ptr`` and ``format``, which MUST outlive the memoryview constructed
         here.
 
         See also: Python C API documentation for `PyMemoryView_FromBuffer`_.
 
-        .. _PyMemoryView_FromBuffer: https://docs.python.org/c-api/memoryview.html#c.PyMemoryView_FromBuffer
+        .. _PyMemoryView_FromBuffer:
+           https://docs.python.org/c-api/memoryview.html#c.PyMemoryView_FromBuffer
 
         :param ptr: Pointer to the buffer.
         :param itemsize: Byte size of an element.
         :param format: Pointer to the null-terminated format string. For
             homogeneous Buffers, this should be set to
             ``format_descriptor<T>::value``.
         :param shape: Shape of the tensor (1 entry per dimension).
         :param strides: Number of bytes between adjacent entries (for each
             per dimension).
         :param readonly: Flag to indicate if the underlying storage may be
             written to.
      \endrst */
-    static memoryview from_buffer(
-        void *ptr, ssize_t itemsize, const char *format,
-        detail::any_container<ssize_t> shape,
-        detail::any_container<ssize_t> strides, bool readonly = false);
-
-    static memoryview from_buffer(
-        const void *ptr, ssize_t itemsize, const char *format,
-        detail::any_container<ssize_t> shape,
-        detail::any_container<ssize_t> strides) {
+    static memoryview from_buffer(void *ptr,
+                                  ssize_t itemsize,
+                                  const char *format,
+                                  detail::any_container<ssize_t> shape,
+                                  detail::any_container<ssize_t> strides,
+                                  bool readonly = false);
+
+    static memoryview from_buffer(const void *ptr,
+                                  ssize_t itemsize,
+                                  const char *format,
+                                  detail::any_container<ssize_t> shape,
+                                  detail::any_container<ssize_t> strides) {
         return memoryview::from_buffer(
             const_cast<void *>(ptr), itemsize, format, std::move(shape), std::move(strides), true);
     }
 
-    template<typename T>
-    static memoryview from_buffer(
-        T *ptr, detail::any_container<ssize_t> shape,
-        detail::any_container<ssize_t> strides, bool readonly = false) {
-        return memoryview::from_buffer(
-            reinterpret_cast<void*>(ptr), sizeof(T),
-            format_descriptor<T>::value, shape, strides, readonly);
+    template <typename T>
+    static memoryview from_buffer(T *ptr,
+                                  detail::any_container<ssize_t> shape,
+                                  detail::any_container<ssize_t> strides,
+                                  bool readonly = false) {
+        return memoryview::from_buffer(reinterpret_cast<void *>(ptr),
+                                       sizeof(T),
+                                       format_descriptor<T>::value,
+                                       shape,
+                                       strides,
+                                       readonly);
     }
 
-    template<typename T>
-    static memoryview from_buffer(
-        const T *ptr, detail::any_container<ssize_t> shape,
-        detail::any_container<ssize_t> strides) {
-        return memoryview::from_buffer(
-            const_cast<T*>(ptr), shape, strides, true);
+    template <typename T>
+    static memoryview from_buffer(const T *ptr,
+                                  detail::any_container<ssize_t> shape,
+                                  detail::any_container<ssize_t> strides) {
+        return memoryview::from_buffer(const_cast<T *>(ptr), shape, strides, true);
     }
 
 #if PY_MAJOR_VERSION >= 3
     /** \rst
         Creates ``memoryview`` from static memory.
 
         This method is meant for providing a ``memoryview`` for C/C++ buffer not
         managed by Python. The caller is responsible for managing the lifetime
         of ``mem``, which MUST outlive the memoryview constructed here.
 
         This method is not available in Python 2.
 
         See also: Python C API documentation for `PyMemoryView_FromBuffer`_.
 
-        .. _PyMemoryView_FromMemory: https://docs.python.org/c-api/memoryview.html#c.PyMemoryView_FromMemory
+        .. _PyMemoryView_FromMemory:
+           https://docs.python.org/c-api/memoryview.html#c.PyMemoryView_FromMemory
      \endrst */
     static memoryview from_memory(void *mem, ssize_t size, bool readonly = false) {
-        PyObject* ptr = PyMemoryView_FromMemory(
-            reinterpret_cast<char*>(mem), size,
-            (readonly) ? PyBUF_READ : PyBUF_WRITE);
-        if (!ptr)
+        PyObject *ptr = PyMemoryView_FromMemory(
+            reinterpret_cast<char *>(mem), size, (readonly) ? PyBUF_READ : PyBUF_WRITE);
+        if (!ptr) {
             pybind11_fail("Could not allocate memoryview object!");
+        }
         return memoryview(object(ptr, stolen_t{}));
     }
 
     static memoryview from_memory(const void *mem, ssize_t size) {
-        return memoryview::from_memory(const_cast<void*>(mem), size, true);
+        return memoryview::from_memory(const_cast<void *>(mem), size, true);
     }
 
-#ifdef PYBIND11_HAS_STRING_VIEW
+#    ifdef PYBIND11_HAS_STRING_VIEW
     static memoryview from_memory(std::string_view mem) {
-        return from_memory(const_cast<char*>(mem.data()), static_cast<ssize_t>(mem.size()), true);
+        return from_memory(const_cast<char *>(mem.data()), static_cast<ssize_t>(mem.size()), true);
     }
-#endif
+#    endif
 
 #endif
 };
 
 /// @cond DUPLICATE
-inline memoryview memoryview::from_buffer(
-    void *ptr, ssize_t itemsize, const char* format,
-    detail::any_container<ssize_t> shape,
-    detail::any_container<ssize_t> strides, bool readonly) {
+inline memoryview memoryview::from_buffer(void *ptr,
+                                          ssize_t itemsize,
+                                          const char *format,
+                                          detail::any_container<ssize_t> shape,
+                                          detail::any_container<ssize_t> strides,
+                                          bool readonly) {
     size_t ndim = shape->size();
-    if (ndim != strides->size())
+    if (ndim != strides->size()) {
         pybind11_fail("memoryview: shape length doesn't match strides length");
+    }
     ssize_t size = ndim != 0u ? 1 : 0;
-    for (size_t i = 0; i < ndim; ++i)
+    for (size_t i = 0; i < ndim; ++i) {
         size *= (*shape)[i];
+    }
     Py_buffer view;
     view.buf = ptr;
     view.obj = nullptr;
     view.len = size * itemsize;
     view.readonly = static_cast<int>(readonly);
     view.itemsize = itemsize;
-    view.format = const_cast<char*>(format);
+    view.format = const_cast<char *>(format);
     view.ndim = static_cast<int>(ndim);
     view.shape = shape->data();
     view.strides = strides->data();
     view.suboffsets = nullptr;
     view.internal = nullptr;
-    PyObject* obj = PyMemoryView_FromBuffer(&view);
-    if (!obj)
+    PyObject *obj = PyMemoryView_FromBuffer(&view);
+    if (!obj) {
         throw error_already_set();
+    }
     return memoryview(object(obj, stolen_t{}));
 }
 /// @endcond
 /// @} pytypes
 
 /// \addtogroup python_builtins
 /// @{
 
 /// Get the length of a Python object.
 inline size_t len(handle h) {
     ssize_t result = PyObject_Length(h.ptr());
-    if (result < 0)
+    if (result < 0) {
         throw error_already_set();
+    }
     return (size_t) result;
 }
 
 /// Get the length hint of a Python object.
 /// Returns 0 when this cannot be determined.
 inline size_t len_hint(handle h) {
 #if PY_VERSION_HEX >= 0x03040000
@@ -1819,106 +2022,132 @@
         return 0;
     }
     return (size_t) result;
 }
 
 inline str repr(handle h) {
     PyObject *str_value = PyObject_Repr(h.ptr());
-    if (!str_value) throw error_already_set();
+    if (!str_value) {
+        throw error_already_set();
+    }
 #if PY_MAJOR_VERSION < 3
     PyObject *unicode = PyUnicode_FromEncodedObject(str_value, "utf-8", nullptr);
-    Py_XDECREF(str_value); str_value = unicode;
-    if (!str_value) throw error_already_set();
+    Py_XDECREF(str_value);
+    str_value = unicode;
+    if (!str_value)
+        throw error_already_set();
 #endif
     return reinterpret_steal<str>(str_value);
 }
 
 inline iterator iter(handle obj) {
     PyObject *result = PyObject_GetIter(obj.ptr());
-    if (!result) { throw error_already_set(); }
+    if (!result) {
+        throw error_already_set();
+    }
     return reinterpret_steal<iterator>(result);
 }
 /// @} python_builtins
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-template <typename D> iterator object_api<D>::begin() const { return iter(derived()); }
-template <typename D> iterator object_api<D>::end() const { return iterator::sentinel(); }
-template <typename D> item_accessor object_api<D>::operator[](handle key) const {
+template <typename D>
+iterator object_api<D>::begin() const {
+    return iter(derived());
+}
+template <typename D>
+iterator object_api<D>::end() const {
+    return iterator::sentinel();
+}
+template <typename D>
+item_accessor object_api<D>::operator[](handle key) const {
     return {derived(), reinterpret_borrow<object>(key)};
 }
-template <typename D> item_accessor object_api<D>::operator[](const char *key) const {
+template <typename D>
+item_accessor object_api<D>::operator[](const char *key) const {
     return {derived(), pybind11::str(key)};
 }
-template <typename D> obj_attr_accessor object_api<D>::attr(handle key) const {
+template <typename D>
+obj_attr_accessor object_api<D>::attr(handle key) const {
     return {derived(), reinterpret_borrow<object>(key)};
 }
-template <typename D> str_attr_accessor object_api<D>::attr(const char *key) const {
+template <typename D>
+str_attr_accessor object_api<D>::attr(const char *key) const {
     return {derived(), key};
 }
-template <typename D> args_proxy object_api<D>::operator*() const {
+template <typename D>
+args_proxy object_api<D>::operator*() const {
     return args_proxy(derived().ptr());
 }
-template <typename D> template <typename T> bool object_api<D>::contains(T &&item) const {
+template <typename D>
+template <typename T>
+bool object_api<D>::contains(T &&item) const {
     return attr("__contains__")(std::forward<T>(item)).template cast<bool>();
 }
 
 template <typename D>
-pybind11::str object_api<D>::str() const { return pybind11::str(derived()); }
+pybind11::str object_api<D>::str() const {
+    return pybind11::str(derived());
+}
 
 template <typename D>
-str_attr_accessor object_api<D>::doc() const { return attr("__doc__"); }
+str_attr_accessor object_api<D>::doc() const {
+    return attr("__doc__");
+}
 
 template <typename D>
-handle object_api<D>::get_type() const { return type::handle_of(derived()); }
+handle object_api<D>::get_type() const {
+    return type::handle_of(derived());
+}
 
 template <typename D>
 bool object_api<D>::rich_compare(object_api const &other, int value) const {
     int rv = PyObject_RichCompareBool(derived().ptr(), other.derived().ptr(), value);
-    if (rv == -1)
+    if (rv == -1) {
         throw error_already_set();
+    }
     return rv == 1;
 }
 
-#define PYBIND11_MATH_OPERATOR_UNARY(op, fn)                                   \
-    template <typename D> object object_api<D>::op() const {                   \
-        object result = reinterpret_steal<object>(fn(derived().ptr()));        \
-        if (!result.ptr())                                                     \
-            throw error_already_set();                                         \
-        return result;                                                         \
-    }
-
-#define PYBIND11_MATH_OPERATOR_BINARY(op, fn)                                  \
-    template <typename D>                                                      \
-    object object_api<D>::op(object_api const &other) const {                  \
-        object result = reinterpret_steal<object>(                             \
-            fn(derived().ptr(), other.derived().ptr()));                       \
-        if (!result.ptr())                                                     \
-            throw error_already_set();                                         \
-        return result;                                                         \
-    }
-
-PYBIND11_MATH_OPERATOR_UNARY (operator~,   PyNumber_Invert)
-PYBIND11_MATH_OPERATOR_UNARY (operator-,   PyNumber_Negative)
-PYBIND11_MATH_OPERATOR_BINARY(operator+,   PyNumber_Add)
-PYBIND11_MATH_OPERATOR_BINARY(operator+=,  PyNumber_InPlaceAdd)
-PYBIND11_MATH_OPERATOR_BINARY(operator-,   PyNumber_Subtract)
-PYBIND11_MATH_OPERATOR_BINARY(operator-=,  PyNumber_InPlaceSubtract)
-PYBIND11_MATH_OPERATOR_BINARY(operator*,   PyNumber_Multiply)
-PYBIND11_MATH_OPERATOR_BINARY(operator*=,  PyNumber_InPlaceMultiply)
-PYBIND11_MATH_OPERATOR_BINARY(operator/,   PyNumber_TrueDivide)
-PYBIND11_MATH_OPERATOR_BINARY(operator/=,  PyNumber_InPlaceTrueDivide)
-PYBIND11_MATH_OPERATOR_BINARY(operator|,   PyNumber_Or)
-PYBIND11_MATH_OPERATOR_BINARY(operator|=,  PyNumber_InPlaceOr)
-PYBIND11_MATH_OPERATOR_BINARY(operator&,   PyNumber_And)
-PYBIND11_MATH_OPERATOR_BINARY(operator&=,  PyNumber_InPlaceAnd)
-PYBIND11_MATH_OPERATOR_BINARY(operator^,   PyNumber_Xor)
-PYBIND11_MATH_OPERATOR_BINARY(operator^=,  PyNumber_InPlaceXor)
-PYBIND11_MATH_OPERATOR_BINARY(operator<<,  PyNumber_Lshift)
+#define PYBIND11_MATH_OPERATOR_UNARY(op, fn)                                                      \
+    template <typename D>                                                                         \
+    object object_api<D>::op() const {                                                            \
+        object result = reinterpret_steal<object>(fn(derived().ptr()));                           \
+        if (!result.ptr())                                                                        \
+            throw error_already_set();                                                            \
+        return result;                                                                            \
+    }
+
+#define PYBIND11_MATH_OPERATOR_BINARY(op, fn)                                                     \
+    template <typename D>                                                                         \
+    object object_api<D>::op(object_api const &other) const {                                     \
+        object result = reinterpret_steal<object>(fn(derived().ptr(), other.derived().ptr()));    \
+        if (!result.ptr())                                                                        \
+            throw error_already_set();                                                            \
+        return result;                                                                            \
+    }
+
+PYBIND11_MATH_OPERATOR_UNARY(operator~, PyNumber_Invert)
+PYBIND11_MATH_OPERATOR_UNARY(operator-, PyNumber_Negative)
+PYBIND11_MATH_OPERATOR_BINARY(operator+, PyNumber_Add)
+PYBIND11_MATH_OPERATOR_BINARY(operator+=, PyNumber_InPlaceAdd)
+PYBIND11_MATH_OPERATOR_BINARY(operator-, PyNumber_Subtract)
+PYBIND11_MATH_OPERATOR_BINARY(operator-=, PyNumber_InPlaceSubtract)
+PYBIND11_MATH_OPERATOR_BINARY(operator*, PyNumber_Multiply)
+PYBIND11_MATH_OPERATOR_BINARY(operator*=, PyNumber_InPlaceMultiply)
+PYBIND11_MATH_OPERATOR_BINARY(operator/, PyNumber_TrueDivide)
+PYBIND11_MATH_OPERATOR_BINARY(operator/=, PyNumber_InPlaceTrueDivide)
+PYBIND11_MATH_OPERATOR_BINARY(operator|, PyNumber_Or)
+PYBIND11_MATH_OPERATOR_BINARY(operator|=, PyNumber_InPlaceOr)
+PYBIND11_MATH_OPERATOR_BINARY(operator&, PyNumber_And)
+PYBIND11_MATH_OPERATOR_BINARY(operator&=, PyNumber_InPlaceAnd)
+PYBIND11_MATH_OPERATOR_BINARY(operator^, PyNumber_Xor)
+PYBIND11_MATH_OPERATOR_BINARY(operator^=, PyNumber_InPlaceXor)
+PYBIND11_MATH_OPERATOR_BINARY(operator<<, PyNumber_Lshift)
 PYBIND11_MATH_OPERATOR_BINARY(operator<<=, PyNumber_InPlaceLshift)
-PYBIND11_MATH_OPERATOR_BINARY(operator>>,  PyNumber_Rshift)
+PYBIND11_MATH_OPERATOR_BINARY(operator>>, PyNumber_Rshift)
 PYBIND11_MATH_OPERATOR_BINARY(operator>>=, PyNumber_InPlaceRshift)
 
 #undef PYBIND11_MATH_OPERATOR_UNARY
 #undef PYBIND11_MATH_OPERATOR_BINARY
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/stl/filesystem.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/stl/filesystem.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 // Copyright (c) 2021 The Pybind Development Team.
 // All rights reserved. Use of this source code is governed by a
 // BSD-style license that can be found in the LICENSE file.
 
 #pragma once
 
-#include "../cast.h"
 #include "../pybind11.h"
-#include "../pytypes.h"
-
 #include "../detail/common.h"
 #include "../detail/descr.h"
+#include "../cast.h"
+#include "../pytypes.h"
 
 #include <string>
 
 #ifdef __has_include
-#  if defined(PYBIND11_CPP17) && __has_include(<filesystem>) && \
+#    if defined(PYBIND11_CPP17) && __has_include(<filesystem>) && \
       PY_VERSION_HEX >= 0x03060000
-#    include <filesystem>
-#    define PYBIND11_HAS_FILESYSTEM 1
-#  endif
+#        include <filesystem>
+#        define PYBIND11_HAS_FILESYSTEM 1
+#    endif
 #endif
 
 #if !defined(PYBIND11_HAS_FILESYSTEM) && !defined(PYBIND11_HAS_FILESYSTEM_IS_OPTIONAL)
 #    error                                                                                        \
         "#include <filesystem> is not available. (Use -DPYBIND11_HAS_FILESYSTEM_IS_OPTIONAL to ignore.)"
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 #if defined(PYBIND11_HAS_FILESYSTEM)
-template<typename T> struct path_caster {
+template <typename T>
+struct path_caster {
 
 private:
-    static PyObject* unicode_from_fs_native(const std::string& w) {
-#if !defined(PYPY_VERSION)
+    static PyObject *unicode_from_fs_native(const std::string &w) {
+#    if !defined(PYPY_VERSION)
         return PyUnicode_DecodeFSDefaultAndSize(w.c_str(), ssize_t(w.size()));
-#else
+#    else
         // PyPy mistakenly declares the first parameter as non-const.
-        return PyUnicode_DecodeFSDefaultAndSize(
-            const_cast<char*>(w.c_str()), ssize_t(w.size()));
-#endif
+        return PyUnicode_DecodeFSDefaultAndSize(const_cast<char *>(w.c_str()), ssize_t(w.size()));
+#    endif
     }
 
-    static PyObject* unicode_from_fs_native(const std::wstring& w) {
+    static PyObject *unicode_from_fs_native(const std::wstring &w) {
         return PyUnicode_FromWideChar(w.c_str(), ssize_t(w.size()));
     }
 
 public:
-    static handle cast(const T& path, return_value_policy, handle) {
+    static handle cast(const T &path, return_value_policy, handle) {
         if (auto py_str = unicode_from_fs_native(path.native())) {
-            return module_::import("pathlib").attr("Path")(reinterpret_steal<object>(py_str))
-                   .release();
+            return module_::import("pathlib")
+                .attr("Path")(reinterpret_steal<object>(py_str))
+                .release();
         }
         return nullptr;
     }
 
     bool load(handle handle, bool) {
         // PyUnicode_FSConverter and PyUnicode_FSDecoder normally take care of
         // calling PyOS_FSPath themselves, but that's broken on PyPy (PyPy
         // issue #3168) so we do it ourselves instead.
-        PyObject* buf = PyOS_FSPath(handle.ptr());
+        PyObject *buf = PyOS_FSPath(handle.ptr());
         if (!buf) {
             PyErr_Clear();
             return false;
         }
-        PyObject* native = nullptr;
+        PyObject *native = nullptr;
         if constexpr (std::is_same_v<typename T::value_type, char>) {
             if (PyUnicode_FSConverter(buf, &native) != 0) {
-                if (auto c_str = PyBytes_AsString(native)) {
+                if (auto *c_str = PyBytes_AsString(native)) {
                     // AsString returns a pointer to the internal buffer, which
                     // must not be free'd.
                     value = c_str;
                 }
             }
         } else if constexpr (std::is_same_v<typename T::value_type, wchar_t>) {
             if (PyUnicode_FSDecoder(buf, &native) != 0) {
-                if (auto c_str = PyUnicode_AsWideCharString(native, nullptr)) {
+                if (auto *c_str = PyUnicode_AsWideCharString(native, nullptr)) {
                     // AsWideCharString returns a new string that must be free'd.
-                    value = c_str;  // Copies the string.
+                    value = c_str; // Copies the string.
                     PyMem_Free(c_str);
                 }
             }
         }
         Py_XDECREF(native);
         Py_DECREF(buf);
         if (PyErr_Occurred()) {
@@ -91,13 +91,13 @@
         }
         return true;
     }
 
     PYBIND11_TYPE_CASTER(T, const_name("os.PathLike"));
 };
 
-template<> struct type_caster<std::filesystem::path>
-    : public path_caster<std::filesystem::path> {};
+template <>
+struct type_caster<std::filesystem::path> : public path_caster<std::filesystem::path> {};
 #endif // PYBIND11_HAS_FILESYSTEM
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/stl.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/stl.h`

 * *Files 4% similar despite different names*

```diff
@@ -5,101 +5,111 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#include "detail/common.h"
 #include "pybind11.h"
-#include <set>
-#include <unordered_set>
-#include <map>
-#include <unordered_map>
+#include "detail/common.h"
+
+#include <deque>
 #include <iostream>
 #include <list>
-#include <deque>
+#include <map>
+#include <set>
+#include <unordered_map>
+#include <unordered_set>
 #include <valarray>
 
 // See `detail/common.h` for implementation of these guards.
 #if defined(PYBIND11_HAS_OPTIONAL)
-#  include <optional>
+#    include <optional>
 #elif defined(PYBIND11_HAS_EXP_OPTIONAL)
-#  include <experimental/optional>
+#    include <experimental/optional>
 #endif
 
 #if defined(PYBIND11_HAS_VARIANT)
-#  include <variant>
+#    include <variant>
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Extracts an const lvalue reference or rvalue reference for U based on the type of T (e.g. for
 /// forwarding a container element).  Typically used indirect via forwarded_type(), below.
 template <typename T, typename U>
-using forwarded_type = conditional_t<
-    std::is_lvalue_reference<T>::value, remove_reference_t<U> &, remove_reference_t<U> &&>;
+using forwarded_type = conditional_t<std::is_lvalue_reference<T>::value,
+                                     remove_reference_t<U> &,
+                                     remove_reference_t<U> &&>;
 
 /// Forwards a value U as rvalue or lvalue according to whether T is rvalue or lvalue; typically
 /// used for forwarding a container's elements.
 template <typename T, typename U>
 forwarded_type<T, U> forward_like(U &&u) {
     return std::forward<detail::forwarded_type<T, U>>(std::forward<U>(u));
 }
 
-template <typename Type, typename Key> struct set_caster {
+template <typename Type, typename Key>
+struct set_caster {
     using type = Type;
     using key_conv = make_caster<Key>;
 
     bool load(handle src, bool convert) {
-        if (!isinstance<pybind11::set>(src))
+        if (!isinstance<pybind11::set>(src)) {
             return false;
+        }
         auto s = reinterpret_borrow<pybind11::set>(src);
         value.clear();
         for (auto entry : s) {
             key_conv conv;
-            if (!conv.load(entry, convert))
+            if (!conv.load(entry, convert)) {
                 return false;
+            }
             value.insert(cast_op<Key &&>(std::move(conv)));
         }
         return true;
     }
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
-        if (!std::is_lvalue_reference<T>::value)
+        if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Key>::policy(policy);
+        }
         pybind11::set s;
         for (auto &&value : src) {
-            auto value_ = reinterpret_steal<object>(key_conv::cast(forward_like<T>(value), policy, parent));
-            if (!value_ || !s.add(value_))
+            auto value_ = reinterpret_steal<object>(
+                key_conv::cast(forward_like<T>(value), policy, parent));
+            if (!value_ || !s.add(value_)) {
                 return handle();
+            }
         }
         return s.release();
     }
 
     PYBIND11_TYPE_CASTER(type, const_name("Set[") + key_conv::name + const_name("]"));
 };
 
-template <typename Type, typename Key, typename Value> struct map_caster {
-    using key_conv   = make_caster<Key>;
+template <typename Type, typename Key, typename Value>
+struct map_caster {
+    using key_conv = make_caster<Key>;
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
-        if (!isinstance<dict>(src))
+        if (!isinstance<dict>(src)) {
             return false;
+        }
         auto d = reinterpret_borrow<dict>(src);
         value.clear();
         for (auto it : d) {
             key_conv kconv;
             value_conv vconv;
-            if (!kconv.load(it.first.ptr(), convert) ||
-                !vconv.load(it.second.ptr(), convert))
+            if (!kconv.load(it.first.ptr(), convert) || !vconv.load(it.second.ptr(), convert)) {
                 return false;
+            }
             value.emplace(cast_op<Key &&>(std::move(kconv)), cast_op<Value &&>(std::move(vconv)));
         }
         return true;
     }
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
@@ -107,192 +117,225 @@
         return_value_policy policy_key = policy;
         return_value_policy policy_value = policy;
         if (!std::is_lvalue_reference<T>::value) {
             policy_key = return_value_policy_override<Key>::policy(policy_key);
             policy_value = return_value_policy_override<Value>::policy(policy_value);
         }
         for (auto &&kv : src) {
-            auto key = reinterpret_steal<object>(key_conv::cast(forward_like<T>(kv.first), policy_key, parent));
-            auto value = reinterpret_steal<object>(value_conv::cast(forward_like<T>(kv.second), policy_value, parent));
-            if (!key || !value)
+            auto key = reinterpret_steal<object>(
+                key_conv::cast(forward_like<T>(kv.first), policy_key, parent));
+            auto value = reinterpret_steal<object>(
+                value_conv::cast(forward_like<T>(kv.second), policy_value, parent));
+            if (!key || !value) {
                 return handle();
+            }
             d[key] = value;
         }
         return d.release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, const_name("Dict[") + key_conv::name + const_name(", ") + value_conv::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(Type,
+                         const_name("Dict[") + key_conv::name + const_name(", ") + value_conv::name
+                             + const_name("]"));
 };
 
-template <typename Type, typename Value> struct list_caster {
+template <typename Type, typename Value>
+struct list_caster {
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
-        if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src))
+        if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src)) {
             return false;
+        }
         auto s = reinterpret_borrow<sequence>(src);
         value.clear();
         reserve_maybe(s, &value);
         for (auto it : s) {
             value_conv conv;
-            if (!conv.load(it, convert))
+            if (!conv.load(it, convert)) {
                 return false;
+            }
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
     }
 
 private:
     template <
-        typename T                                                                          = Type,
+        typename T = Type,
         enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
     void reserve_maybe(const sequence &s, Type *) {
         value.reserve(s.size());
     }
     void reserve_maybe(const sequence &, void *) {}
 
 public:
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
-        if (!std::is_lvalue_reference<T>::value)
+        if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
+        }
         list l(src.size());
         ssize_t index = 0;
         for (auto &&value : src) {
-            auto value_ = reinterpret_steal<object>(value_conv::cast(forward_like<T>(value), policy, parent));
-            if (!value_)
+            auto value_ = reinterpret_steal<object>(
+                value_conv::cast(forward_like<T>(value), policy, parent));
+            if (!value_) {
                 return handle();
+            }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(Type, const_name("List[") + value_conv::name + const_name("]"));
 };
 
-template <typename Type, typename Alloc> struct type_caster<std::vector<Type, Alloc>>
- : list_caster<std::vector<Type, Alloc>, Type> { };
+template <typename Type, typename Alloc>
+struct type_caster<std::vector<Type, Alloc>> : list_caster<std::vector<Type, Alloc>, Type> {};
 
-template <typename Type, typename Alloc> struct type_caster<std::deque<Type, Alloc>>
- : list_caster<std::deque<Type, Alloc>, Type> { };
+template <typename Type, typename Alloc>
+struct type_caster<std::deque<Type, Alloc>> : list_caster<std::deque<Type, Alloc>, Type> {};
 
-template <typename Type, typename Alloc> struct type_caster<std::list<Type, Alloc>>
- : list_caster<std::list<Type, Alloc>, Type> { };
+template <typename Type, typename Alloc>
+struct type_caster<std::list<Type, Alloc>> : list_caster<std::list<Type, Alloc>, Type> {};
 
-template <typename ArrayType, typename Value, bool Resizable, size_t Size = 0> struct array_caster {
+template <typename ArrayType, typename Value, bool Resizable, size_t Size = 0>
+struct array_caster {
     using value_conv = make_caster<Value>;
 
 private:
     template <bool R = Resizable>
     bool require_size(enable_if_t<R, size_t> size) {
-        if (value.size() != size)
+        if (value.size() != size) {
             value.resize(size);
+        }
         return true;
     }
     template <bool R = Resizable>
     bool require_size(enable_if_t<!R, size_t> size) {
         return size == Size;
     }
 
 public:
     bool load(handle src, bool convert) {
-        if (!isinstance<sequence>(src))
+        if (!isinstance<sequence>(src)) {
             return false;
+        }
         auto l = reinterpret_borrow<sequence>(src);
-        if (!require_size(l.size()))
+        if (!require_size(l.size())) {
             return false;
+        }
         size_t ctr = 0;
         for (auto it : l) {
             value_conv conv;
-            if (!conv.load(it, convert))
+            if (!conv.load(it, convert)) {
                 return false;
+            }
             value[ctr++] = cast_op<Value &&>(std::move(conv));
         }
         return true;
     }
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         list l(src.size());
         ssize_t index = 0;
         for (auto &&value : src) {
-            auto value_ = reinterpret_steal<object>(value_conv::cast(forward_like<T>(value), policy, parent));
-            if (!value_)
+            auto value_ = reinterpret_steal<object>(
+                value_conv::cast(forward_like<T>(value), policy, parent));
+            if (!value_) {
                 return handle();
+            }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
-    PYBIND11_TYPE_CASTER(ArrayType, const_name("List[") + value_conv::name + const_name<Resizable>(const_name(""), const_name("[") + const_name<Size>() + const_name("]")) + const_name("]"));
+    PYBIND11_TYPE_CASTER(ArrayType,
+                         const_name("List[") + value_conv::name
+                             + const_name<Resizable>(const_name(""),
+                                                     const_name("[") + const_name<Size>()
+                                                         + const_name("]"))
+                             + const_name("]"));
 };
 
-template <typename Type, size_t Size> struct type_caster<std::array<Type, Size>>
- : array_caster<std::array<Type, Size>, Type, false, Size> { };
-
-template <typename Type> struct type_caster<std::valarray<Type>>
- : array_caster<std::valarray<Type>, Type, true> { };
-
-template <typename Key, typename Compare, typename Alloc> struct type_caster<std::set<Key, Compare, Alloc>>
-  : set_caster<std::set<Key, Compare, Alloc>, Key> { };
-
-template <typename Key, typename Hash, typename Equal, typename Alloc> struct type_caster<std::unordered_set<Key, Hash, Equal, Alloc>>
-  : set_caster<std::unordered_set<Key, Hash, Equal, Alloc>, Key> { };
-
-template <typename Key, typename Value, typename Compare, typename Alloc> struct type_caster<std::map<Key, Value, Compare, Alloc>>
-  : map_caster<std::map<Key, Value, Compare, Alloc>, Key, Value> { };
-
-template <typename Key, typename Value, typename Hash, typename Equal, typename Alloc> struct type_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>>
-  : map_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>, Key, Value> { };
+template <typename Type, size_t Size>
+struct type_caster<std::array<Type, Size>>
+    : array_caster<std::array<Type, Size>, Type, false, Size> {};
+
+template <typename Type>
+struct type_caster<std::valarray<Type>> : array_caster<std::valarray<Type>, Type, true> {};
+
+template <typename Key, typename Compare, typename Alloc>
+struct type_caster<std::set<Key, Compare, Alloc>>
+    : set_caster<std::set<Key, Compare, Alloc>, Key> {};
+
+template <typename Key, typename Hash, typename Equal, typename Alloc>
+struct type_caster<std::unordered_set<Key, Hash, Equal, Alloc>>
+    : set_caster<std::unordered_set<Key, Hash, Equal, Alloc>, Key> {};
+
+template <typename Key, typename Value, typename Compare, typename Alloc>
+struct type_caster<std::map<Key, Value, Compare, Alloc>>
+    : map_caster<std::map<Key, Value, Compare, Alloc>, Key, Value> {};
+
+template <typename Key, typename Value, typename Hash, typename Equal, typename Alloc>
+struct type_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>>
+    : map_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>, Key, Value> {};
 
 // This type caster is intended to be used for std::optional and std::experimental::optional
-template<typename Type, typename Value = typename Type::value_type> struct optional_caster {
+template <typename Type, typename Value = typename Type::value_type>
+struct optional_caster {
     using value_conv = make_caster<Value>;
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
-        if (!src)
+        if (!src) {
             return none().inc_ref();
+        }
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
         }
         return value_conv::cast(*std::forward<T>(src), policy, parent);
     }
 
     bool load(handle src, bool convert) {
         if (!src) {
             return false;
         }
         if (src.is_none()) {
-            return true;  // default-constructed value is already empty
+            return true; // default-constructed value is already empty
         }
         value_conv inner_caster;
-        if (!inner_caster.load(src, convert))
+        if (!inner_caster.load(src, convert)) {
             return false;
+        }
 
         value.emplace(cast_op<Value &&>(std::move(inner_caster)));
         return true;
     }
 
     PYBIND11_TYPE_CASTER(Type, const_name("Optional[") + value_conv::name + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_OPTIONAL)
-template<typename T> struct type_caster<std::optional<T>>
-    : public optional_caster<std::optional<T>> {};
+template <typename T>
+struct type_caster<std::optional<T>> : public optional_caster<std::optional<T>> {};
 
-template<> struct type_caster<std::nullopt_t>
-    : public void_caster<std::nullopt_t> {};
+template <>
+struct type_caster<std::nullopt_t> : public void_caster<std::nullopt_t> {};
 #endif
 
 #if defined(PYBIND11_HAS_EXP_OPTIONAL)
-template<typename T> struct type_caster<std::experimental::optional<T>>
+template <typename T>
+struct type_caster<std::experimental::optional<T>>
     : public optional_caster<std::experimental::optional<T>> {};
 
-template<> struct type_caster<std::experimental::nullopt_t>
+template <>
+struct type_caster<std::experimental::nullopt_t>
     : public void_caster<std::experimental::nullopt_t> {};
 #endif
 
 /// Visit a variant and cast any found type to Python
 struct variant_caster_visitor {
     return_value_policy policy;
     handle parent;
@@ -305,26 +348,27 @@
     }
 };
 
 /// Helper class which abstracts away variant's `visit` function. `std::variant` and similar
 /// `namespace::variant` types which provide a `namespace::visit()` function are handled here
 /// automatically using argument-dependent lookup. Users can provide specializations for other
 /// variant-like classes, e.g. `boost::variant` and `boost::apply_visitor`.
-template <template<typename...> class Variant>
+template <template <typename...> class Variant>
 struct visit_helper {
     template <typename... Args>
     static auto call(Args &&...args) -> decltype(visit(std::forward<Args>(args)...)) {
         return visit(std::forward<Args>(args)...);
     }
 };
 
 /// Generic variant caster
-template <typename Variant> struct variant_caster;
+template <typename Variant>
+struct variant_caster;
 
-template <template<typename...> class V, typename... Ts>
+template <template <typename...> class V, typename... Ts>
 struct variant_caster<V<Ts...>> {
     static_assert(sizeof...(Ts) > 0, "Variant must consist of at least one alternative.");
 
     template <typename U, typename... Us>
     bool load_alternative(handle src, bool convert, type_list<U, Us...>) {
         auto caster = make_caster<U>();
         if (caster.load(src, convert)) {
@@ -337,32 +381,35 @@
     bool load_alternative(handle, bool, type_list<>) { return false; }
 
     bool load(handle src, bool convert) {
         // Do a first pass without conversions to improve constructor resolution.
         // E.g. `py::int_(1).cast<variant<double, int>>()` needs to fill the `int`
         // slot of the variant. Without two-pass loading `double` would be filled
         // because it appears first and a conversion is possible.
-        if (convert && load_alternative(src, false, type_list<Ts...>{}))
+        if (convert && load_alternative(src, false, type_list<Ts...>{})) {
             return true;
+        }
         return load_alternative(src, convert, type_list<Ts...>{});
     }
 
     template <typename Variant>
     static handle cast(Variant &&src, return_value_policy policy, handle parent) {
         return visit_helper<V>::call(variant_caster_visitor{policy, parent},
                                      std::forward<Variant>(src));
     }
 
     using Type = V<Ts...>;
-    PYBIND11_TYPE_CASTER(Type, const_name("Union[") + detail::concat(make_caster<Ts>::name...) + const_name("]"));
+    PYBIND11_TYPE_CASTER(Type,
+                         const_name("Union[") + detail::concat(make_caster<Ts>::name...)
+                             + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_VARIANT)
 template <typename... Ts>
-struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> { };
+struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> {};
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
 inline std::ostream &operator<<(std::ostream &os, const handle &obj) {
 #ifdef PYBIND11_HAS_STRING_VIEW
     os << str(obj).cast<std::string_view>();
```

### Comparing `pybind11_global-2.9.1/pybind11/include/pybind11/stl_bind.h` & `pybind11_global-2.9.2/pybind11/include/pybind11/stl_bind.h`

 * *Files 7% similar despite different names*

```diff
@@ -15,145 +15,156 @@
 #include <algorithm>
 #include <sstream>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /* SFINAE helper class used by 'is_comparable */
-template <typename T>  struct container_traits {
-    template <typename T2> static std::true_type test_comparable(decltype(std::declval<const T2 &>() == std::declval<const T2 &>())*);
-    template <typename T2> static std::false_type test_comparable(...);
-    template <typename T2> static std::true_type test_value(typename T2::value_type *);
-    template <typename T2> static std::false_type test_value(...);
-    template <typename T2> static std::true_type test_pair(typename T2::first_type *, typename T2::second_type *);
-    template <typename T2> static std::false_type test_pair(...);
-
-    static constexpr const bool is_comparable = std::is_same<std::true_type, decltype(test_comparable<T>(nullptr))>::value;
-    static constexpr const bool is_pair = std::is_same<std::true_type, decltype(test_pair<T>(nullptr, nullptr))>::value;
-    static constexpr const bool is_vector = std::is_same<std::true_type, decltype(test_value<T>(nullptr))>::value;
+template <typename T>
+struct container_traits {
+    template <typename T2>
+    static std::true_type
+    test_comparable(decltype(std::declval<const T2 &>() == std::declval<const T2 &>()) *);
+    template <typename T2>
+    static std::false_type test_comparable(...);
+    template <typename T2>
+    static std::true_type test_value(typename T2::value_type *);
+    template <typename T2>
+    static std::false_type test_value(...);
+    template <typename T2>
+    static std::true_type test_pair(typename T2::first_type *, typename T2::second_type *);
+    template <typename T2>
+    static std::false_type test_pair(...);
+
+    static constexpr const bool is_comparable
+        = std::is_same<std::true_type, decltype(test_comparable<T>(nullptr))>::value;
+    static constexpr const bool is_pair
+        = std::is_same<std::true_type, decltype(test_pair<T>(nullptr, nullptr))>::value;
+    static constexpr const bool is_vector
+        = std::is_same<std::true_type, decltype(test_value<T>(nullptr))>::value;
     static constexpr const bool is_element = !is_pair && !is_vector;
 };
 
 /* Default: is_comparable -> std::false_type */
 template <typename T, typename SFINAE = void>
-struct is_comparable : std::false_type { };
+struct is_comparable : std::false_type {};
 
 /* For non-map data structures, check whether operator== can be instantiated */
 template <typename T>
 struct is_comparable<
-    T, enable_if_t<container_traits<T>::is_element &&
-                   container_traits<T>::is_comparable>>
-    : std::true_type { };
+    T,
+    enable_if_t<container_traits<T>::is_element && container_traits<T>::is_comparable>>
+    : std::true_type {};
 
-/* For a vector/map data structure, recursively check the value type (which is std::pair for maps) */
+/* For a vector/map data structure, recursively check the value type
+   (which is std::pair for maps) */
 template <typename T>
 struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>> {
-    static constexpr const bool value =
-        is_comparable<typename T::value_type>::value;
+    static constexpr const bool value = is_comparable<typename T::value_type>::value;
 };
 
 /* For pairs, recursively check the two data types */
 template <typename T>
 struct is_comparable<T, enable_if_t<container_traits<T>::is_pair>> {
-    static constexpr const bool value =
-        is_comparable<typename T::first_type>::value &&
-        is_comparable<typename T::second_type>::value;
+    static constexpr const bool value = is_comparable<typename T::first_type>::value
+                                        && is_comparable<typename T::second_type>::value;
 };
 
 /* Fallback functions */
-template <typename, typename, typename... Args> void vector_if_copy_constructible(const Args &...) { }
-template <typename, typename, typename... Args> void vector_if_equal_operator(const Args &...) { }
-template <typename, typename, typename... Args> void vector_if_insertion_operator(const Args &...) { }
-template <typename, typename, typename... Args> void vector_modifiers(const Args &...) { }
+template <typename, typename, typename... Args>
+void vector_if_copy_constructible(const Args &...) {}
+template <typename, typename, typename... Args>
+void vector_if_equal_operator(const Args &...) {}
+template <typename, typename, typename... Args>
+void vector_if_insertion_operator(const Args &...) {}
+template <typename, typename, typename... Args>
+void vector_modifiers(const Args &...) {}
 
-template<typename Vector, typename Class_>
+template <typename Vector, typename Class_>
 void vector_if_copy_constructible(enable_if_t<is_copy_constructible<Vector>::value, Class_> &cl) {
     cl.def(init<const Vector &>(), "Copy constructor");
 }
 
-template<typename Vector, typename Class_>
+template <typename Vector, typename Class_>
 void vector_if_equal_operator(enable_if_t<is_comparable<Vector>::value, Class_> &cl) {
     using T = typename Vector::value_type;
 
     cl.def(self == self);
     cl.def(self != self);
 
-    cl.def("count",
-        [](const Vector &v, const T &x) {
-            return std::count(v.begin(), v.end(), x);
-        },
+    cl.def(
+        "count",
+        [](const Vector &v, const T &x) { return std::count(v.begin(), v.end(), x); },
         arg("x"),
-        "Return the number of times ``x`` appears in the list"
-    );
+        "Return the number of times ``x`` appears in the list");
 
-    cl.def("remove", [](Vector &v, const T &x) {
+    cl.def(
+        "remove",
+        [](Vector &v, const T &x) {
             auto p = std::find(v.begin(), v.end(), x);
-            if (p != v.end())
+            if (p != v.end()) {
                 v.erase(p);
-            else
+            } else {
                 throw value_error();
+            }
         },
         arg("x"),
         "Remove the first item from the list whose value is x. "
-        "It is an error if there is no such item."
-    );
+        "It is an error if there is no such item.");
 
-    cl.def("__contains__",
-        [](const Vector &v, const T &x) {
-            return std::find(v.begin(), v.end(), x) != v.end();
-        },
+    cl.def(
+        "__contains__",
+        [](const Vector &v, const T &x) { return std::find(v.begin(), v.end(), x) != v.end(); },
         arg("x"),
-        "Return true the container contains ``x``"
-    );
+        "Return true the container contains ``x``");
 }
 
 // Vector modifiers -- requires a copyable vector_type:
-// (Technically, some of these (pop and __delitem__) don't actually require copyability, but it seems
-// silly to allow deletion but not insertion, so include them here too.)
+// (Technically, some of these (pop and __delitem__) don't actually require copyability, but it
+// seems silly to allow deletion but not insertion, so include them here too.)
 template <typename Vector, typename Class_>
-void vector_modifiers(enable_if_t<is_copy_constructible<typename Vector::value_type>::value, Class_> &cl) {
+void vector_modifiers(
+    enable_if_t<is_copy_constructible<typename Vector::value_type>::value, Class_> &cl) {
     using T = typename Vector::value_type;
     using SizeType = typename Vector::size_type;
     using DiffType = typename Vector::difference_type;
 
     auto wrap_i = [](DiffType i, SizeType n) {
-        if (i < 0)
+        if (i < 0) {
             i += n;
-        if (i < 0 || (SizeType)i >= n)
+        }
+        if (i < 0 || (SizeType) i >= n) {
             throw index_error();
+        }
         return i;
     };
 
-    cl.def("append",
-           [](Vector &v, const T &value) { v.push_back(value); },
-           arg("x"),
-           "Add an item to the end of the list");
+    cl.def(
+        "append",
+        [](Vector &v, const T &value) { v.push_back(value); },
+        arg("x"),
+        "Add an item to the end of the list");
 
     cl.def(init([](const iterable &it) {
         auto v = std::unique_ptr<Vector>(new Vector());
         v->reserve(len_hint(it));
-        for (handle h : it)
+        for (handle h : it) {
             v->push_back(h.cast<T>());
+        }
         return v.release();
     }));
 
-    cl.def("clear",
-        [](Vector &v) {
-            v.clear();
-        },
-        "Clear the contents"
-    );
+    cl.def(
+        "clear", [](Vector &v) { v.clear(); }, "Clear the contents");
 
-    cl.def("extend",
-       [](Vector &v, const Vector &src) {
-           v.insert(v.end(), src.begin(), src.end());
-       },
-       arg("L"),
-       "Extend the list by appending all the items in the given list"
-    );
+    cl.def(
+        "extend",
+        [](Vector &v, const Vector &src) { v.insert(v.end(), src.begin(), src.end()); },
+        arg("L"),
+        "Extend the list by appending all the items in the given list");
 
     cl.def(
         "extend",
         [](Vector &v, const iterable &it) {
             const size_t old_size = v.size();
             v.reserve(old_size + len_hint(it));
             try {
@@ -170,109 +181,116 @@
                 }
                 throw;
             }
         },
         arg("L"),
         "Extend the list by appending all the items in the given list");
 
-    cl.def("insert",
+    cl.def(
+        "insert",
         [](Vector &v, DiffType i, const T &x) {
             // Can't use wrap_i; i == v.size() is OK
-            if (i < 0)
+            if (i < 0) {
                 i += v.size();
-            if (i < 0 || (SizeType)i > v.size())
+            }
+            if (i < 0 || (SizeType) i > v.size()) {
                 throw index_error();
+            }
             v.insert(v.begin() + i, x);
         },
-        arg("i") , arg("x"),
-        "Insert an item at a given position."
-    );
+        arg("i"),
+        arg("x"),
+        "Insert an item at a given position.");
 
-    cl.def("pop",
+    cl.def(
+        "pop",
         [](Vector &v) {
-            if (v.empty())
+            if (v.empty()) {
                 throw index_error();
+            }
             T t = std::move(v.back());
             v.pop_back();
             return t;
         },
-        "Remove and return the last item"
-    );
+        "Remove and return the last item");
 
-    cl.def("pop",
+    cl.def(
+        "pop",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
             T t = std::move(v[(SizeType) i]);
             v.erase(std::next(v.begin(), i));
             return t;
         },
         arg("i"),
-        "Remove and return the item at index ``i``"
-    );
+        "Remove and return the item at index ``i``");
 
-    cl.def("__setitem__",
-        [wrap_i](Vector &v, DiffType i, const T &t) {
-            i = wrap_i(i, v.size());
-            v[(SizeType)i] = t;
-        }
-    );
+    cl.def("__setitem__", [wrap_i](Vector &v, DiffType i, const T &t) {
+        i = wrap_i(i, v.size());
+        v[(SizeType) i] = t;
+    });
 
     /// Slicing protocol
     cl.def(
         "__getitem__",
         [](const Vector &v, slice slice) -> Vector * {
             size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
-            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
+            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength)) {
                 throw error_already_set();
+            }
 
             auto *seq = new Vector();
             seq->reserve((size_t) slicelength);
 
-            for (size_t i=0; i<slicelength; ++i) {
+            for (size_t i = 0; i < slicelength; ++i) {
                 seq->push_back(v[start]);
                 start += step;
             }
             return seq;
         },
         arg("s"),
         "Retrieve list elements using a slice object");
 
     cl.def(
         "__setitem__",
         [](Vector &v, slice slice, const Vector &value) {
             size_t start = 0, stop = 0, step = 0, slicelength = 0;
-            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
+            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength)) {
                 throw error_already_set();
+            }
 
-            if (slicelength != value.size())
-                throw std::runtime_error("Left and right hand size of slice assignment have different sizes!");
+            if (slicelength != value.size()) {
+                throw std::runtime_error(
+                    "Left and right hand size of slice assignment have different sizes!");
+            }
 
-            for (size_t i=0; i<slicelength; ++i) {
+            for (size_t i = 0; i < slicelength; ++i) {
                 v[start] = value[i];
                 start += step;
             }
         },
         "Assign list elements using a slice object");
 
-    cl.def("__delitem__",
+    cl.def(
+        "__delitem__",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
             v.erase(v.begin() + i);
         },
-        "Delete the list elements at index ``i``"
-    );
+        "Delete the list elements at index ``i``");
 
     cl.def(
         "__delitem__",
         [](Vector &v, slice slice) {
             size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
-            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
+            if (!slice.compute(v.size(), &start, &stop, &step, &slicelength)) {
                 throw error_already_set();
+            }
 
             if (step == 1 && false) {
                 v.erase(v.begin() + (DiffType) start, v.begin() + DiffType(start + slicelength));
             } else {
                 for (size_t i = 0; i < slicelength; ++i) {
                     v.erase(v.begin() + DiffType(start));
                     start += step - 1;
@@ -280,175 +298,199 @@
             }
         },
         "Delete list elements using a slice object");
 }
 
 // If the type has an operator[] that doesn't return a reference (most notably std::vector<bool>),
 // we have to access by copying; otherwise we return by reference.
-template <typename Vector> using vector_needs_copy = negation<
-    std::is_same<decltype(std::declval<Vector>()[typename Vector::size_type()]), typename Vector::value_type &>>;
+template <typename Vector>
+using vector_needs_copy
+    = negation<std::is_same<decltype(std::declval<Vector>()[typename Vector::size_type()]),
+                            typename Vector::value_type &>>;
 
 // The usual case: access and iterate by reference
 template <typename Vector, typename Class_>
 void vector_accessor(enable_if_t<!vector_needs_copy<Vector>::value, Class_> &cl) {
     using T = typename Vector::value_type;
     using SizeType = typename Vector::size_type;
     using DiffType = typename Vector::difference_type;
-    using ItType   = typename Vector::iterator;
+    using ItType = typename Vector::iterator;
 
     auto wrap_i = [](DiffType i, SizeType n) {
-        if (i < 0)
+        if (i < 0) {
             i += n;
-        if (i < 0 || (SizeType)i >= n)
+        }
+        if (i < 0 || (SizeType) i >= n) {
             throw index_error();
+        }
         return i;
     };
 
-    cl.def("__getitem__",
+    cl.def(
+        "__getitem__",
         [wrap_i](Vector &v, DiffType i) -> T & {
             i = wrap_i(i, v.size());
-            return v[(SizeType)i];
+            return v[(SizeType) i];
         },
         return_value_policy::reference_internal // ref + keepalive
     );
 
-    cl.def("__iter__",
-           [](Vector &v) {
-               return make_iterator<
-                   return_value_policy::reference_internal, ItType, ItType, T&>(
-                   v.begin(), v.end());
-           },
-           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+    cl.def(
+        "__iter__",
+        [](Vector &v) {
+            return make_iterator<return_value_policy::reference_internal, ItType, ItType, T &>(
+                v.begin(), v.end());
+        },
+        keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
     );
 }
 
 // The case for special objects, like std::vector<bool>, that have to be returned-by-copy:
 template <typename Vector, typename Class_>
 void vector_accessor(enable_if_t<vector_needs_copy<Vector>::value, Class_> &cl) {
     using T = typename Vector::value_type;
     using SizeType = typename Vector::size_type;
     using DiffType = typename Vector::difference_type;
-    using ItType   = typename Vector::iterator;
-    cl.def("__getitem__",
-        [](const Vector &v, DiffType i) -> T {
-            if (i < 0 && (i += v.size()) < 0)
-                throw index_error();
-            if ((SizeType)i >= v.size())
-                throw index_error();
-            return v[(SizeType)i];
+    using ItType = typename Vector::iterator;
+    cl.def("__getitem__", [](const Vector &v, DiffType i) -> T {
+        if (i < 0 && (i += v.size()) < 0) {
+            throw index_error();
         }
-    );
+        if ((SizeType) i >= v.size()) {
+            throw index_error();
+        }
+        return v[(SizeType) i];
+    });
 
-    cl.def("__iter__",
-           [](Vector &v) {
-               return make_iterator<
-                   return_value_policy::copy, ItType, ItType, T>(
-                   v.begin(), v.end());
-           },
-           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+    cl.def(
+        "__iter__",
+        [](Vector &v) {
+            return make_iterator<return_value_policy::copy, ItType, ItType, T>(v.begin(), v.end());
+        },
+        keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
     );
 }
 
-template <typename Vector, typename Class_> auto vector_if_insertion_operator(Class_ &cl, std::string const &name)
-    -> decltype(std::declval<std::ostream&>() << std::declval<typename Vector::value_type>(), void()) {
+template <typename Vector, typename Class_>
+auto vector_if_insertion_operator(Class_ &cl, std::string const &name)
+    -> decltype(std::declval<std::ostream &>() << std::declval<typename Vector::value_type>(),
+                void()) {
     using size_type = typename Vector::size_type;
 
-    cl.def("__repr__",
-           [name](Vector &v) {
+    cl.def(
+        "__repr__",
+        [name](Vector &v) {
             std::ostringstream s;
             s << name << '[';
-            for (size_type i=0; i < v.size(); ++i) {
+            for (size_type i = 0; i < v.size(); ++i) {
                 s << v[i];
-                if (i != v.size() - 1)
+                if (i != v.size() - 1) {
                     s << ", ";
+                }
             }
             s << ']';
             return s.str();
         },
-        "Return the canonical string representation of this list."
-    );
+        "Return the canonical string representation of this list.");
 }
 
 // Provide the buffer interface for vectors if we have data() and we have a format for it
-// GCC seems to have "void std::vector<bool>::data()" - doing SFINAE on the existence of data() is insufficient, we need to check it returns an appropriate pointer
+// GCC seems to have "void std::vector<bool>::data()" - doing SFINAE on the existence of data()
+// is insufficient, we need to check it returns an appropriate pointer
 template <typename Vector, typename = void>
 struct vector_has_data_and_format : std::false_type {};
 template <typename Vector>
-struct vector_has_data_and_format<Vector, enable_if_t<std::is_same<decltype(format_descriptor<typename Vector::value_type>::format(), std::declval<Vector>().data()), typename Vector::value_type*>::value>> : std::true_type {};
+struct vector_has_data_and_format<
+    Vector,
+    enable_if_t<std::is_same<decltype(format_descriptor<typename Vector::value_type>::format(),
+                                      std::declval<Vector>().data()),
+                             typename Vector::value_type *>::value>> : std::true_type {};
 
 // [workaround(intel)] Separate function required here
 // Workaround as the Intel compiler does not compile the enable_if_t part below
 // (tested with icc (ICC) 2021.1 Beta 20200827)
 template <typename... Args>
 constexpr bool args_any_are_buffer() {
     return detail::any_of<std::is_same<Args, buffer_protocol>...>::value;
 }
 
 // [workaround(intel)] Separate function required here
 // [workaround(msvc)] Can't use constexpr bool in return type
 
 // Add the buffer interface to a vector
 template <typename Vector, typename Class_, typename... Args>
-void vector_buffer_impl(Class_& cl, std::true_type) {
+void vector_buffer_impl(Class_ &cl, std::true_type) {
     using T = typename Vector::value_type;
 
-    static_assert(vector_has_data_and_format<Vector>::value, "There is not an appropriate format descriptor for this vector");
+    static_assert(vector_has_data_and_format<Vector>::value,
+                  "There is not an appropriate format descriptor for this vector");
 
-    // numpy.h declares this for arbitrary types, but it may raise an exception and crash hard at runtime if PYBIND11_NUMPY_DTYPE hasn't been called, so check here
+    // numpy.h declares this for arbitrary types, but it may raise an exception and crash hard
+    // at runtime if PYBIND11_NUMPY_DTYPE hasn't been called, so check here
     format_descriptor<T>::format();
 
-    cl.def_buffer([](Vector& v) -> buffer_info {
-        return buffer_info(v.data(), static_cast<ssize_t>(sizeof(T)), format_descriptor<T>::format(), 1, {v.size()}, {sizeof(T)});
+    cl.def_buffer([](Vector &v) -> buffer_info {
+        return buffer_info(v.data(),
+                           static_cast<ssize_t>(sizeof(T)),
+                           format_descriptor<T>::format(),
+                           1,
+                           {v.size()},
+                           {sizeof(T)});
     });
 
     cl.def(init([](const buffer &buf) {
         auto info = buf.request();
-        if (info.ndim != 1 || info.strides[0] % static_cast<ssize_t>(sizeof(T)))
+        if (info.ndim != 1 || info.strides[0] % static_cast<ssize_t>(sizeof(T))) {
             throw type_error("Only valid 1D buffers can be copied to a vector");
-        if (!detail::compare_buffer_info<T>::compare(info) || (ssize_t) sizeof(T) != info.itemsize)
-            throw type_error("Format mismatch (Python: " + info.format + " C++: " + format_descriptor<T>::format() + ")");
+        }
+        if (!detail::compare_buffer_info<T>::compare(info)
+            || (ssize_t) sizeof(T) != info.itemsize) {
+            throw type_error("Format mismatch (Python: " + info.format
+                             + " C++: " + format_descriptor<T>::format() + ")");
+        }
 
-        T *p = static_cast<T*>(info.ptr);
+        T *p = static_cast<T *>(info.ptr);
         ssize_t step = info.strides[0] / static_cast<ssize_t>(sizeof(T));
         T *end = p + info.shape[0] * step;
         if (step == 1) {
             return Vector(p, end);
         }
         Vector vec;
         vec.reserve((size_t) info.shape[0]);
-        for (; p != end; p += step)
+        for (; p != end; p += step) {
             vec.push_back(*p);
+        }
         return vec;
-
     }));
 
     return;
 }
 
 template <typename Vector, typename Class_, typename... Args>
-void vector_buffer_impl(Class_&, std::false_type) {}
+void vector_buffer_impl(Class_ &, std::false_type) {}
 
 template <typename Vector, typename Class_, typename... Args>
-void vector_buffer(Class_& cl) {
-    vector_buffer_impl<Vector, Class_, Args...>(cl, detail::any_of<std::is_same<Args, buffer_protocol>...>{});
+void vector_buffer(Class_ &cl) {
+    vector_buffer_impl<Vector, Class_, Args...>(
+        cl, detail::any_of<std::is_same<Args, buffer_protocol>...>{});
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 //
 // std::vector
 //
 template <typename Vector, typename holder_type = std::unique_ptr<Vector>, typename... Args>
-class_<Vector, holder_type> bind_vector(handle scope, std::string const &name, Args&&... args) {
+class_<Vector, holder_type> bind_vector(handle scope, std::string const &name, Args &&...args) {
     using Class_ = class_<Vector, holder_type>;
 
     // If the value_type is unregistered (e.g. a converting type) or is itself registered
     // module-local then make the vector binding module-local as well:
     using vtype = typename Vector::value_type;
-    auto vtype_info = detail::get_type_info(typeid(vtype));
+    auto *vtype_info = detail::get_type_info(typeid(vtype));
     bool local = !vtype_info || vtype_info->module_local;
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
 
     // Declare the buffer interface if a buffer_protocol() is passed in
     detail::vector_buffer<Vector, Class_, Args...>(cl);
 
@@ -465,26 +507,21 @@
 
     // Modifiers require copyable vector value type
     detail::vector_modifiers<Vector, Class_>(cl);
 
     // Accessor and iterator; return by value if copyable, otherwise we return by ref + keep-alive
     detail::vector_accessor<Vector, Class_>(cl);
 
-    cl.def("__bool__",
-        [](const Vector &v) -> bool {
-            return !v.empty();
-        },
-        "Check whether the list is nonempty"
-    );
+    cl.def(
+        "__bool__",
+        [](const Vector &v) -> bool { return !v.empty(); },
+        "Check whether the list is nonempty");
 
     cl.def("__len__", &Vector::size);
 
-
-
-
 #if 0
     // C++ style functions deprecated, leaving it here as an example
     cl.def(init<size_type>());
 
     cl.def("resize",
          (void (Vector::*) (size_type count)) & Vector::resize,
          "changes the number of elements stored");
@@ -520,118 +557,119 @@
     }, "access the last element ");
 
 #endif
 
     return cl;
 }
 
-
-
 //
 // std::map, std::unordered_map
 //
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /* Fallback functions */
-template <typename, typename, typename... Args> void map_if_insertion_operator(const Args &...) { }
-template <typename, typename, typename... Args> void map_assignment(const Args &...) { }
+template <typename, typename, typename... Args>
+void map_if_insertion_operator(const Args &...) {}
+template <typename, typename, typename... Args>
+void map_assignment(const Args &...) {}
 
 // Map assignment when copy-assignable: just copy the value
 template <typename Map, typename Class_>
-void map_assignment(enable_if_t<is_copy_assignable<typename Map::mapped_type>::value, Class_> &cl) {
+void map_assignment(
+    enable_if_t<is_copy_assignable<typename Map::mapped_type>::value, Class_> &cl) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
 
-    cl.def("__setitem__",
-           [](Map &m, const KeyType &k, const MappedType &v) {
-               auto it = m.find(k);
-               if (it != m.end()) it->second = v;
-               else m.emplace(k, v);
-           }
-    );
+    cl.def("__setitem__", [](Map &m, const KeyType &k, const MappedType &v) {
+        auto it = m.find(k);
+        if (it != m.end()) {
+            it->second = v;
+        } else {
+            m.emplace(k, v);
+        }
+    });
 }
 
-// Not copy-assignable, but still copy-constructible: we can update the value by erasing and reinserting
-template<typename Map, typename Class_>
-void map_assignment(enable_if_t<
-        !is_copy_assignable<typename Map::mapped_type>::value &&
-        is_copy_constructible<typename Map::mapped_type>::value,
-        Class_> &cl) {
+// Not copy-assignable, but still copy-constructible: we can update the value by erasing and
+// reinserting
+template <typename Map, typename Class_>
+void map_assignment(enable_if_t<!is_copy_assignable<typename Map::mapped_type>::value
+                                    && is_copy_constructible<typename Map::mapped_type>::value,
+                                Class_> &cl) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
 
-    cl.def("__setitem__",
-           [](Map &m, const KeyType &k, const MappedType &v) {
-               // We can't use m[k] = v; because value type might not be default constructable
-               auto r = m.emplace(k, v);
-               if (!r.second) {
-                   // value type is not copy assignable so the only way to insert it is to erase it first...
-                   m.erase(r.first);
-                   m.emplace(k, v);
-               }
-           }
-    );
+    cl.def("__setitem__", [](Map &m, const KeyType &k, const MappedType &v) {
+        // We can't use m[k] = v; because value type might not be default constructable
+        auto r = m.emplace(k, v);
+        if (!r.second) {
+            // value type is not copy assignable so the only way to insert it is to erase it
+            // first...
+            m.erase(r.first);
+            m.emplace(k, v);
+        }
+    });
 }
 
+template <typename Map, typename Class_>
+auto map_if_insertion_operator(Class_ &cl, std::string const &name)
+    -> decltype(std::declval<std::ostream &>() << std::declval<typename Map::key_type>()
+                                               << std::declval<typename Map::mapped_type>(),
+                void()) {
 
-template <typename Map, typename Class_> auto map_if_insertion_operator(Class_ &cl, std::string const &name)
--> decltype(std::declval<std::ostream&>() << std::declval<typename Map::key_type>() << std::declval<typename Map::mapped_type>(), void()) {
-
-    cl.def("__repr__",
-           [name](Map &m) {
+    cl.def(
+        "__repr__",
+        [name](Map &m) {
             std::ostringstream s;
             s << name << '{';
             bool f = false;
             for (auto const &kv : m) {
-                if (f)
+                if (f) {
                     s << ", ";
+                }
                 s << kv.first << ": " << kv.second;
                 f = true;
             }
             s << '}';
             return s.str();
         },
-        "Return the canonical string representation of this map."
-    );
+        "Return the canonical string representation of this map.");
 }
 
-template<typename Map>
-struct keys_view
-{
+template <typename Map>
+struct keys_view {
     Map &map;
 };
 
-template<typename Map>
-struct values_view
-{
+template <typename Map>
+struct values_view {
     Map &map;
 };
 
-template<typename Map>
-struct items_view
-{
+template <typename Map>
+struct items_view {
     Map &map;
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
-class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args&&... args) {
+class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args &&...args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
     using KeysView = detail::keys_view<Map>;
     using ValuesView = detail::values_view<Map>;
     using ItemsView = detail::items_view<Map>;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
-    auto tinfo = detail::get_type_info(typeid(MappedType));
+    auto *tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
@@ -643,105 +681,105 @@
         scope, ("ItemsView[" + name + "]").c_str(), pybind11::module_local(local));
 
     cl.def(init<>());
 
     // Register stream insertion operator (if possible)
     detail::map_if_insertion_operator<Map, Class_>(cl, name);
 
-    cl.def("__bool__",
+    cl.def(
+        "__bool__",
         [](const Map &m) -> bool { return !m.empty(); },
-        "Check whether the map is nonempty"
-    );
+        "Check whether the map is nonempty");
 
-    cl.def("__iter__",
-           [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
-           keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
+    cl.def(
+        "__iter__",
+        [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
+        keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
     );
 
-    cl.def("keys",
-           [](Map &m) { return KeysView{m}; },
-           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
+    cl.def(
+        "keys",
+        [](Map &m) { return KeysView{m}; },
+        keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
-    cl.def("values",
-           [](Map &m) { return ValuesView{m}; },
-           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
+    cl.def(
+        "values",
+        [](Map &m) { return ValuesView{m}; },
+        keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
-    cl.def("items",
-           [](Map &m) { return ItemsView{m}; },
-           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
+    cl.def(
+        "items",
+        [](Map &m) { return ItemsView{m}; },
+        keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
-    cl.def("__getitem__",
+    cl.def(
+        "__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
-            if (it == m.end())
-              throw key_error();
-           return it->second;
+            if (it == m.end()) {
+                throw key_error();
+            }
+            return it->second;
         },
         return_value_policy::reference_internal // ref + keepalive
     );
 
-    cl.def("__contains__",
-        [](Map &m, const KeyType &k) -> bool {
-            auto it = m.find(k);
-            if (it == m.end())
-              return false;
-           return true;
+    cl.def("__contains__", [](Map &m, const KeyType &k) -> bool {
+        auto it = m.find(k);
+        if (it == m.end()) {
+            return false;
         }
-    );
+        return true;
+    });
     // Fallback for when the object is not of the key type
     cl.def("__contains__", [](Map &, const object &) -> bool { return false; });
 
     // Assignment provided only if the type is copyable
     detail::map_assignment<Map, Class_>(cl);
 
-    cl.def("__delitem__",
-           [](Map &m, const KeyType &k) {
-               auto it = m.find(k);
-               if (it == m.end())
-                   throw key_error();
-               m.erase(it);
-           }
-    );
+    cl.def("__delitem__", [](Map &m, const KeyType &k) {
+        auto it = m.find(k);
+        if (it == m.end()) {
+            throw key_error();
+        }
+        m.erase(it);
+    });
 
     cl.def("__len__", &Map::size);
 
     keys_view.def("__len__", [](KeysView &view) { return view.map.size(); });
-    keys_view.def("__iter__",
-        [](KeysView &view) {
-            return make_key_iterator(view.map.begin(), view.map.end());
-        },
+    keys_view.def(
+        "__iter__",
+        [](KeysView &view) { return make_key_iterator(view.map.begin(), view.map.end()); },
         keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
     );
-    keys_view.def("__contains__",
-        [](KeysView &view, const KeyType &k) -> bool {
-            auto it = view.map.find(k);
-            if (it == view.map.end())
-                return false;
-            return true;
+    keys_view.def("__contains__", [](KeysView &view, const KeyType &k) -> bool {
+        auto it = view.map.find(k);
+        if (it == view.map.end()) {
+            return false;
         }
-    );
+        return true;
+    });
     // Fallback for when the object is not of the key type
     keys_view.def("__contains__", [](KeysView &, const object &) -> bool { return false; });
 
     values_view.def("__len__", [](ValuesView &view) { return view.map.size(); });
-    values_view.def("__iter__",
-        [](ValuesView &view) {
-            return make_value_iterator(view.map.begin(), view.map.end());
-        },
+    values_view.def(
+        "__iter__",
+        [](ValuesView &view) { return make_value_iterator(view.map.begin(), view.map.end()); },
         keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
     );
 
     items_view.def("__len__", [](ItemsView &view) { return view.map.size(); });
-    items_view.def("__iter__",
-        [](ItemsView &view) {
-            return make_iterator(view.map.begin(), view.map.end());
-        },
+    items_view.def(
+        "__iter__",
+        [](ItemsView &view) { return make_iterator(view.map.begin(), view.map.end()); },
         keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
     );
 
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pybind11_global-2.9.1/pybind11/setup_helpers.py` & `pybind11_global-2.9.2/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/setup_helpers.pyi` & `pybind11_global-2.9.2/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/FindPythonLibsNew.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,32 @@
 # testing whether sys has the gettotalrefcount function is a reliable, cross-platform
 # way to detect a CPython debug interpreter.
 #
 # The library suffix is from the config var LDVERSION sometimes, otherwise
 # VERSION. VERSION will typically be like "2.7" on unix, and "27" on windows.
 execute_process(
   COMMAND
-    "${PYTHON_EXECUTABLE}" "-c" "from distutils import sysconfig as s;import sys;import struct;
+    "${PYTHON_EXECUTABLE}" "-c" "
+import sys;import struct;
+import sysconfig as s
+USE_SYSCONFIG = sys.version_info >= (3, 10)
+if not USE_SYSCONFIG:
+    from distutils import sysconfig as ds
 print('.'.join(str(v) for v in sys.version_info));
 print(sys.prefix);
-print(s.get_python_inc(plat_specific=True));
-print(s.get_python_lib(plat_specific=True));
+if USE_SYSCONFIG:
+    scheme = s.get_default_scheme()
+    if scheme == 'posix_local':
+        # Debian's default scheme installs to /usr/local/ but we want to find headers in /usr/
+        scheme = 'posix_prefix'
+    print(s.get_path('platinclude', scheme))
+    print(s.get_path('platlib'))
+else:
+    print(ds.get_python_inc(plat_specific=True));
+    print(ds.get_python_lib(plat_specific=True));
 print(s.get_config_var('EXT_SUFFIX') or s.get_config_var('SO'));
 print(hasattr(sys, 'gettotalrefcount')+0);
 print(struct.calcsize('@P'));
 print(s.get_config_var('LDVERSION') or s.get_config_var('VERSION'));
 print(s.get_config_var('LIBDIR') or '');
 print(s.get_config_var('MULTIARCH') or '');
 "
```

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Common.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Config.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Config.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
   # Python method:
   Python_add_library(MyModule2 src2.cpp)
   target_link_libraries(MyModule2 pybind11::headers)
   set_target_properties(MyModule2 PROPERTIES
                                   INTERPROCEDURAL_OPTIMIZATION ON
                                   CXX_VISIBILITY_PRESET ON
-                                  VISIBLITY_INLINES_HIDDEN ON)
+                                  VISIBILITY_INLINES_HIDDEN ON)
 
 If you build targets yourself, you may be interested in stripping the output
 for reduced size; this is the one other feature that the helper function gives you.
 
 Classic mode
 ^^^^^^^^^^^^
```

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11ConfigVersion.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # to create a version-file which can be installed along a config.cmake file.
 #
 # The created file sets PACKAGE_VERSION_EXACT if the current version string and
 # the requested version string are exactly the same and it sets
 # PACKAGE_VERSION_COMPATIBLE if the current version is >= requested version.
 # The variable CVF_VERSION must be set before calling configure_file().
 
-set(PACKAGE_VERSION "2.9.1")
+set(PACKAGE_VERSION "2.9.2")
 
 if (PACKAGE_FIND_VERSION_RANGE)
   # Package version must be in the requested version range
   if ((PACKAGE_FIND_VERSION_RANGE_MIN STREQUAL "INCLUDE" AND PACKAGE_VERSION VERSION_LESS PACKAGE_FIND_VERSION_MIN)
       OR ((PACKAGE_FIND_VERSION_RANGE_MAX STREQUAL "INCLUDE" AND PACKAGE_VERSION VERSION_GREATER PACKAGE_FIND_VERSION_MAX)
         OR (PACKAGE_FIND_VERSION_RANGE_MAX STREQUAL "EXCLUDE" AND PACKAGE_VERSION VERSION_GREATER_EQUAL PACKAGE_FIND_VERSION_MAX)))
     set(PACKAGE_VERSION_COMPATIBLE FALSE)
```

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11NewTools.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Targets.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Targets.cmake`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11/share/cmake/pybind11/pybind11Tools.cmake` & `pybind11_global-2.9.2/pybind11/share/cmake/pybind11/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/pybind11_global.egg-info/PKG-INFO` & `pybind11_global-2.9.2/pybind11_global.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybind11-global
-Version: 2.9.1
+Version: 2.9.2
 Summary: Seamless operability between C++11 and Python
 Home-page: https://github.com/pybind/pybind11
 Author: Wenzel Jakob
 Author-email: wenzel.jakob@epfl.ch
 License: BSD
 Project-URL: Documentation, https://pybind11.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/pybind/pybind11/issues
```

### Comparing `pybind11_global-2.9.1/pybind11_global.egg-info/SOURCES.txt` & `pybind11_global-2.9.2/pybind11_global.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/setup.cfg` & `pybind11_global-2.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pybind11_global-2.9.1/setup.py` & `pybind11_global-2.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 # Must have a separator
 if base and not base.endswith("/"):
     base += "/"
 
 setup(
     name="pybind11_global",
-    version="2.9.1",
+    version="2.9.2",
     packages=[],
     headers=headers,
     data_files=[
         (base + "share/cmake/pybind11", cmake_files),
         (base + "include/pybind11", main_headers),
         (base + "include/pybind11/detail", detail_headers),
         (base + "include/pybind11/stl", stl_headers),
```

