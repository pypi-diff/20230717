# Comparing `tmp/alpaka-job-coverage-1.3.1.tar.gz` & `tmp/alpaka-job-coverage-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.3.1.tar", last modified: Thu May 25 12:43:52 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.3.2.tar", last modified: Mon Jul 17 11:29:01 2023, max compression
```

## Comparing `alpaka-job-coverage-1.3.1.tar` & `alpaka-job-coverage-1.3.2.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:43:52.749857 alpaka-job-coverage-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-25 12:43:52.749857 alpaka-job-coverage-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:43:52.749857 alpaka-job-coverage-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:43:52.741857 alpaka-job-coverage-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:43:52.745857 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:43:52.749857 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-25 12:43:52.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-25 12:43:52.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:43:52.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 12:43:52.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:43:52.000000 alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 12:43:31.000000 alpaka-job-coverage-1.3.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.502150 alpaka-job-coverage-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/version.txt
```

### Comparing `alpaka-job-coverage-1.3.1/LICENSE` & `alpaka-job-coverage-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/PKG-INFO` & `alpaka-job-coverage-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.1
+Version: 1.3.2
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.1/README.md` & `alpaka-job-coverage-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/setup.py` & `alpaka-job-coverage-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,14 @@
             return False
 
     ###########################
     ## nvcc device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
-        # the CUDA backend needs to be defined
-        if backend_is_not_in_row(row, ALPAKA_ACC_GPU_CUDA_ENABLE):
-            return False
-
         # the nvcc compiler needs the same version, like the backend
         if row_check_backend_version(
             row,
             ALPAKA_ACC_GPU_CUDA_ENABLE,
             "!=",
             row[param_map[DEVICE_COMPILER]][VERSION],
         ):
```

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,71 +33,85 @@
 
     if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
         cuda_sdk_version = 0
         cuda_host_compiler_version = 1
 
         # set the and lowest highest supported gcc version for nvcc
         if row_check_name(row, HOST_COMPILER, "==", GCC):
-            # check the maximum supported compiler version
-            for combination in [
+            combinations = [
                 # (maximum_CUDA_SDK_version, "maximum_gcc_version")
-                ("11.6", "11"),
-                ("11.4", "10"),
+                ("12.1", "12"),
+                ("12.0", "12"),
+                ("11.4", "11"),
+                ("11.1", "10"),
                 ("11.0", "9"),
-                ("10.2", "8"),
+                ("10.1", "8"),
                 ("10.0", "7"),
-            ]:
-                if pk_version.parse(
-                    row[param_map[DEVICE_COMPILER]][VERSION]
-                ) >= pk_version.parse(combination[cuda_sdk_version]):
-                    if pk_version.parse(
-                        row[param_map[HOST_COMPILER]][VERSION]
-                    ) > pk_version.parse(combination[cuda_host_compiler_version]):
-                        return False
-                    else:
-                        break
+            ]
 
-            # since CUDA 11.4, the minimum supported GCC compiler is GCC 6
             if pk_version.parse(
                 row[param_map[DEVICE_COMPILER]][VERSION]
-            ) >= pk_version.parse("11.4") and pk_version.parse(
-                row[param_map[HOST_COMPILER]][VERSION]
-            ) < pk_version.parse(
-                "6"
-            ):
-                return False
+            ) <= pk_version.parse(combinations[0][cuda_sdk_version]):
+                # check the maximum supported compiler version
+                for combination in combinations:
+                    if pk_version.parse(
+                        row[param_map[DEVICE_COMPILER]][VERSION]
+                    ) >= pk_version.parse(combination[cuda_sdk_version]):
+                        if pk_version.parse(
+                            row[param_map[HOST_COMPILER]][VERSION]
+                        ) > pk_version.parse(combination[cuda_host_compiler_version]):
+                            return False
+                        else:
+                            break
+
+                # since CUDA 11.4, the minimum supported GCC compiler is GCC 6
+                if pk_version.parse(
+                    row[param_map[DEVICE_COMPILER]][VERSION]
+                ) >= pk_version.parse("11.4") and pk_version.parse(
+                    row[param_map[HOST_COMPILER]][VERSION]
+                ) < pk_version.parse(
+                    "6"
+                ):
+                    return False
 
         if row_check_name(row, HOST_COMPILER, "==", CLANG):
             # disable clang as host compiler for nvcc 11.3 until 11.5
             if row_check_version(
                 row, DEVICE_COMPILER, ">=", "11.3"
             ) and row_check_version(row, DEVICE_COMPILER, "<=", "11.5"):
                 return False
 
-            # set the and lowest highest supported clang version for nvcc
-            # check the maximum supported compiler version
-            for combination in [
+            combinations = [
                 # (maximum_CUDA_SDK_version, "maximum_clang_version")
+                ("12.1", "15"),
+                ("12.0", "14"),
                 ("11.6", "13"),
                 ("11.4", "12"),
+                ("11.2", "11"),
                 ("11.1", "10"),
                 ("11.0", "9"),
                 ("10.1", "8"),
                 ("10.0", "6"),
-                ("9.2", "5"),
-            ]:
-                if pk_version.parse(
-                    row[param_map[DEVICE_COMPILER]][VERSION]
-                ) >= pk_version.parse(combination[cuda_sdk_version]):
+            ]
+
+            if pk_version.parse(
+                row[param_map[DEVICE_COMPILER]][VERSION]
+            ) <= pk_version.parse(combinations[0][cuda_sdk_version]):
+                # set the and lowest highest supported clang version for nvcc
+                # check the maximum supported compiler version
+                for combination in combinations:
                     if pk_version.parse(
-                        row[param_map[HOST_COMPILER]][VERSION]
-                    ) > pk_version.parse(combination[cuda_host_compiler_version]):
-                        return False
-                    else:
-                        break
+                        row[param_map[DEVICE_COMPILER]][VERSION]
+                    ) >= pk_version.parse(combination[cuda_sdk_version]):
+                        if pk_version.parse(
+                            row[param_map[HOST_COMPILER]][VERSION]
+                        ) > pk_version.parse(combination[cuda_host_compiler_version]):
+                            return False
+                        else:
+                            break
 
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA):
         # disable all clang versions older than 14 as CUDA Compiler
         if row_check_version(row, DEVICE_COMPILER, "<", "14"):
             return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,23 @@
         row, CXX_STANDARD
     ):
         parsed_nvcc_version = pk_version.parse(row[param_map[DEVICE_COMPILER]][VERSION])
 
         # definition of the tuple values: if the nvcc version of the first
         # tuple is older than the cxx standard of the second value, it is not supported
         nvcc_cxx_versions = [
-            ("11.0", 14),  # NVCC versions older than 11.0 does not support C++ 17
-            ("12.0", 17),  # NVCC versions older than 12.0 does not support C++ 20
-            ("13.0", 20),
-        ]  # NVCC 12.x does not support C++ 23 and NVCC 13.x is not released yet
+            ("11.0", 17),  # NVCC versions older than 11.0 does not support C++ 17
+            ("12.0", 20),  # NVCC versions older than 12.0 does not support C++ 20
+            ("12.2", 23),  # NVCC 12.2 is not released yet, therefore we need to
+            # expect that it could support C++23
+        ]
         for nvcc_version, cxx_version in nvcc_cxx_versions:
             if (
                 parsed_nvcc_version < pk_version.parse(nvcc_version)
-                and int(row[param_map[CXX_STANDARD]][VERSION]) > cxx_version
+                and int(row[param_map[CXX_STANDARD]][VERSION]) >= cxx_version
             ):
                 return False
 
     # clang 11 and 12 are not available in the Ubuntu 18.04 ppa
     if (
         row_check_version(row, UBUNTU, "==", "18.04")
         and (
```

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,37 @@
 """Different support functions.
+
+The row type: Several utile functions to do different checks on the row 
+parameters. The type of the row is defined by the pairwise library and the 
+parameter types.
+Each element of the row have ether the type of Tuple[str, str], where the first 
+string is a name and the second string is a version number or the type 
+List[Tuple[str, str]], where tuple also stores a name and version combination. 
+The list type is only used for the backend values of the `backends` parameter.
+The position of the value decides, which parameter a value represent. For 
+example the first and second value can be ("gcc", "9"). Only the position 
+decides if the first value is the host compiler and second value the device 
+compiler or vice versa. 
+The global variable `param_map` implements a indirection which allows to 
+separate the ordering of the parameters from the algorithm. The `param_map` 
+needs to be initialized by the user at each application/test start. 
+For Example:
+    param_map[HOST_COMPILER] = 0
+    param_map[DEVICE_COMPILER] = 1
+
+Example for a row:
+    [('gcc', '6'), ('nvcc', '11.4'), 
+    [
+        ('alpaka_ACC_CPU_B_SEQ_T_SEQ_ENABLE', '1.0.0'), 
+        ('alpaka_ACC_CPU_B_OMP2_T_SEQ_ENABLE', '0.0.0'), 
+        ('alpaka_ACC_GPU_CUDA_ENABLE', '11.4'), 
+        ('alpaka_ACC_GPU_HIP_ENABLE', '0.0.0')
+    ], 
+    ('cmake', '3.19.8'), ('boost', '1.66.0'), ('alpaka', '0.6.1'), 
+    ('ubuntu', '20.04')]
 """
 
 import operator, re
 from typing import Any, List, Dict, Tuple
 from typeguard import typechecked
 from packaging import version as pk_version
 
@@ -117,20 +146,20 @@
     """Returns True, if backend is not in backend list.
 
     Args:
         row (List): Row to check.
         backend (str): Name of the backend, which version should be compared.
 
     Returns:
-        bool: Return False, if backend is not in the row. If backend is in the row and
+        bool: Return True, if backend is not in the row. If backend is in the row and
         the backend name is in the backend list return False else True.
     """
 
     if not is_in_row(row, BACKENDS):
-        return False
+        return True
     else:
         for row_backend in row[param_map[BACKENDS]]:
             if row_backend[NAME] == backend:
                 return False
     return True
 
 
@@ -282,7 +311,38 @@
     for index, job in enumerate(job_matrix):
         if index in index_list:
             new_job_list.insert(0, job)
         else:
             new_job_list.append(job)
 
     return new_job_list
+
+
+@typechecked
+def is_supported_sw_version(name: str, version: str, verbose=True) -> bool:
+    def warning_text(text: str):
+        return "\033[1;33mWARNING: " + text + "\033[0m"
+
+    support_versions: Dict[str, Tuple[str, str]] = {
+        GCC: ("5", "13"),
+        CLANG: ("6.0", "15"),
+        NVCC: ("10.0", "12.1"),
+        HIPCC: ("4.3", "5.1"),
+        CMAKE: ("3.18", "3.22"),
+        BOOST: ("1.66.0", "1.78.0"),
+        CXX_STANDARD: ("14", "20"),
+    }
+
+    if name not in support_versions:
+        if verbose:
+            print(warning_text(f"{name} is an unknown software"))
+        return False
+    else:
+        parsed_version = pk_version.parse(version)
+        if parsed_version < pk_version.parse(
+            support_versions[name][0]
+        ) or parsed_version > pk_version.parse(support_versions[name][1]):
+            if verbose:
+                print(warning_text(f"{name} {version} is not supported"))
+            return False
+
+    return True
```

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.1
+Version: 1.3.2
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.1/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 src/alpaka_job_coverage/globals.py
 src/alpaka_job_coverage/main_functions.py
 src/alpaka_job_coverage/util.py
 src/alpaka_job_coverage.egg-info/PKG-INFO
 src/alpaka_job_coverage.egg-info/SOURCES.txt
 src/alpaka_job_coverage.egg-info/dependency_links.txt
 src/alpaka_job_coverage.egg-info/requires.txt
-src/alpaka_job_coverage.egg-info/top_level.txt
+src/alpaka_job_coverage.egg-info/top_level.txt
+tests/test_compiler_names.py
+tests/test_cuda_sdk.py
+tests/test_util.py
```

