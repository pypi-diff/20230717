# Comparing `tmp/fabrictestbed-extensions-1.6.0b4.tar.gz` & `tmp/fabrictestbed-extensions-1.6.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.6.0b4.tar", last modified: Fri Jul 14 18:43:54 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.6.0b5.tar", last modified: Mon Jul 17 15:16:39 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.6.0b4.tar` & `fabrictestbed-extensions-1.6.0b5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b4/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-07-13 19:11:12.627899 fabrictestbed-extensions-1.6.0b4/.gitignore
--rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b4/.readthedocs.yaml
--rw-r--r--   0        0        0     3134 2023-07-13 19:11:12.628291 fabrictestbed-extensions-1.6.0b4/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b4/LICENSE
--rw-r--r--   0        0        0     4093 2023-07-13 19:11:12.628878 fabrictestbed-extensions-1.6.0b4/README.md
--rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b4/docs/Makefile
--rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b4/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b4/docs/source/conf.py
--rw-r--r--   0        0        0     8968 2023-07-13 19:11:12.629746 fabrictestbed-extensions-1.6.0b4/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b4/docs/source/index.rst
--rw-r--r--   0        0        0      149 2023-07-14 18:43:52.265380 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-07-13 19:11:12.632370 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77361 2023-07-13 19:11:12.634055 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    26310 2023-07-13 19:11:12.634666 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    96387 2023-07-13 19:11:12.635705 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81759 2023-07-13 19:11:12.636971 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1585 2023-07-14 18:43:46.407790 fabrictestbed-extensions-1.6.0b4/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b4/sphinx.sh
--rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b4/tests/benchmarks/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b4/tests/benchmarks/link_benchmark.py
--rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b4/tests/benchmarks/local_network_benchmark.py
--rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b4/tests/benchmarks/network_benchmark_tests.py
--rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b4/tests/benchmarks/nvme_benchmark.py
--rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b4/tests/integration/abc_test.py
--rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b4/tests/integration/component_tests.py
--rw-r--r--   0        0        0    10205 2023-07-13 19:11:12.644478 fabrictestbed-extensions-1.6.0b4/tests/integration/hello_fabric.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b4/tests/unit/__init__.py
--rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b4/tests/unit/data/dummy-token.json
--rw-r--r--   0        0        0     5095 2023-07-13 19:11:12.645235 fabrictestbed-extensions-1.6.0b4/tests/unit/test_basic.py
--rw-r--r--   0        0        0      398 2023-07-13 19:11:12.645487 fabrictestbed-extensions-1.6.0b4/tox.ini
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b5/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b5/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-07-13 19:11:12.627899 fabrictestbed-extensions-1.6.0b5/.gitignore
+-rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b5/.readthedocs.yaml
+-rw-r--r--   0        0        0     3134 2023-07-13 19:11:12.628291 fabrictestbed-extensions-1.6.0b5/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b5/LICENSE
+-rw-r--r--   0        0        0     4093 2023-07-13 19:11:12.628878 fabrictestbed-extensions-1.6.0b5/README.md
+-rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b5/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b5/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b5/docs/source/conf.py
+-rw-r--r--   0        0        0     8968 2023-07-13 19:11:12.629746 fabrictestbed-extensions-1.6.0b5/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b5/docs/source/index.rst
+-rw-r--r--   0        0        0      149 2023-07-17 15:16:23.311675 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-13 19:11:12.632370 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77361 2023-07-13 19:11:12.634055 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26310 2023-07-13 19:11:12.634666 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    96387 2023-07-13 19:11:12.635705 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81759 2023-07-13 19:11:12.636971 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1585 2023-07-17 15:16:17.572520 fabrictestbed-extensions-1.6.0b5/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b5/sphinx.sh
+-rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b5/tests/benchmarks/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b5/tests/benchmarks/link_benchmark.py
+-rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b5/tests/benchmarks/local_network_benchmark.py
+-rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b5/tests/benchmarks/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b5/tests/benchmarks/nvme_benchmark.py
+-rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b5/tests/integration/abc_test.py
+-rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b5/tests/integration/component_tests.py
+-rw-r--r--   0        0        0    10205 2023-07-13 19:11:12.644478 fabrictestbed-extensions-1.6.0b5/tests/integration/hello_fabric.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b5/tests/unit/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b5/tests/unit/data/dummy-token.json
+-rw-r--r--   0        0        0     5095 2023-07-13 19:11:12.645235 fabrictestbed-extensions-1.6.0b5/tests/unit/test_basic.py
+-rw-r--r--   0        0        0      398 2023-07-13 19:11:12.645487 fabrictestbed-extensions-1.6.0b5/tox.ini
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b5/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.6.0b4/.github/workflows/build.yml` & `fabrictestbed-extensions-1.6.0b5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.6.0b5/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/.github/workflows/test.yml` & `fabrictestbed-extensions-1.6.0b5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/.gitignore` & `fabrictestbed-extensions-1.6.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/.readthedocs.yaml` & `fabrictestbed-extensions-1.6.0b5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/CHANGELOG.md` & `fabrictestbed-extensions-1.6.0b5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/LICENSE` & `fabrictestbed-extensions-1.6.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/README.md` & `fabrictestbed-extensions-1.6.0b5/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/docs/Makefile` & `fabrictestbed-extensions-1.6.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/docs/make.bat` & `fabrictestbed-extensions-1.6.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/docs/source/conf.py` & `fabrictestbed-extensions-1.6.0b5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/docs/source/fablib.rst` & `fabrictestbed-extensions-1.6.0b5/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/docs/source/index.rst` & `fabrictestbed-extensions-1.6.0b5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/interface.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.6.0b5/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/pyproject.toml` & `fabrictestbed-extensions-1.6.0b5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.6.0b3",
+    "fabrictestbed==1.6.0b4",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
     ]
```

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/benchmarks/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.6.0b5/tests/benchmarks/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/benchmarks/link_benchmark.py` & `fabrictestbed-extensions-1.6.0b5/tests/benchmarks/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/benchmarks/local_network_benchmark.py` & `fabrictestbed-extensions-1.6.0b5/tests/benchmarks/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/benchmarks/network_benchmark_tests.py` & `fabrictestbed-extensions-1.6.0b5/tests/benchmarks/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/benchmarks/nvme_benchmark.py` & `fabrictestbed-extensions-1.6.0b5/tests/benchmarks/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/integration/abc_test.py` & `fabrictestbed-extensions-1.6.0b5/tests/integration/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/integration/component_tests.py` & `fabrictestbed-extensions-1.6.0b5/tests/integration/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/integration/hello_fabric.py` & `fabrictestbed-extensions-1.6.0b5/tests/integration/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/tests/unit/test_basic.py` & `fabrictestbed-extensions-1.6.0b5/tests/unit/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b4/PKG-INFO` & `fabrictestbed-extensions-1.6.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.6.0b3
+Requires-Dist: fabrictestbed==1.6.0b4
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
```

