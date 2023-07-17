# Comparing `tmp/oyehr-tools-package-0.0.1.tar.gz` & `tmp/oyehr-tools-package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oyehr-tools-package-0.0.1.tar", last modified: Mon Jul 17 02:35:47 2023, max compression
+gzip compressed data, was "oyehr-tools-package-0.0.2.tar", last modified: Mon Jul 17 02:43:41 2023, max compression
```

## Comparing `oyehr-tools-package-0.0.1.tar` & `oyehr-tools-package-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 02:35:47.061851 oyehr-tools-package-0.0.1/
--rw-rw-rw-   0        0        0       39 2023-07-17 02:32:40.000000 oyehr-tools-package-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      101 2023-07-17 02:35:47.060851 oyehr-tools-package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4101 2023-07-17 02:33:30.000000 oyehr-tools-package-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 02:35:47.055851 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/
--rw-rw-rw-   0        0        0      101 2023-07-17 02:35:46.000000 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-17 02:35:46.000000 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:35:46.000000 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-17 02:35:46.000000 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:35:46.000000 oyehr-tools-package-0.0.1/oyehr_tools_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 02:35:47.062853 oyehr-tools-package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-17 02:33:48.000000 oyehr-tools-package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:35:47.059852 oyehr-tools-package-0.0.1/tests/
--rw-rw-rw-   0        0        0      711 2023-07-17 02:33:14.000000 oyehr-tools-package-0.0.1/tests/test_my_tool_1.py
--rw-rw-rw-   0        0        0      867 2023-07-17 02:33:06.000000 oyehr-tools-package-0.0.1/tests/test_my_tool_2.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.080912 oyehr-tools-package-0.0.2/
+-rw-rw-rw-   0        0        0       39 2023-07-17 02:32:40.000000 oyehr-tools-package-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      101 2023-07-17 02:43:41.080912 oyehr-tools-package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4101 2023-07-17 02:33:30.000000 oyehr-tools-package-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.039913 oyehr-tools-package-0.0.2/oyehr_tool_package/
+-rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.055913 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/__init__.py
+-rw-rw-rw-   0        0        0      476 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/my_tool_1.py
+-rw-rw-rw-   0        0        0      697 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/my_tool_2.py
+-rw-rw-rw-   0        0        0      524 2023-07-17 02:41:23.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.058913 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/
+-rw-rw-rw-   0        0        0      302 2023-07-17 02:42:43.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/my_tool_1.yaml
+-rw-rw-rw-   0        0        0      333 2023-07-17 02:42:48.000000 oyehr-tools-package-0.0.2/oyehr_tool_package/yamls/my_tool_2.yaml
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.076911 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 02:43:40.000000 oyehr-tools-package-0.0.2/oyehr_tools_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 02:43:41.081912 oyehr-tools-package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-17 02:43:30.000000 oyehr-tools-package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:43:41.078910 oyehr-tools-package-0.0.2/tests/
+-rw-rw-rw-   0        0        0      711 2023-07-17 02:33:14.000000 oyehr-tools-package-0.0.2/tests/test_my_tool_1.py
+-rw-rw-rw-   0        0        0      867 2023-07-17 02:33:06.000000 oyehr-tools-package-0.0.2/tests/test_my_tool_2.py
```

### Comparing `oyehr-tools-package-0.0.1/README.md` & `oyehr-tools-package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oyehr-tools-package-0.0.1/tests/test_my_tool_1.py` & `oyehr-tools-package-0.0.2/tests/test_my_tool_1.py`

 * *Files identical despite different names*

### Comparing `oyehr-tools-package-0.0.1/tests/test_my_tool_2.py` & `oyehr-tools-package-0.0.2/tests/test_my_tool_2.py`

 * *Files identical despite different names*

