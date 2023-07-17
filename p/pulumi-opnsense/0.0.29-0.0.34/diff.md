# Comparing `tmp/pulumi-opnsense-0.0.0.tar.gz` & `tmp/pulumi-opnsense-.tar.gz`

## Comparing `pulumi-opnsense-0.0.0.tar` & `pulumi-opnsense-.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-14 13:29:05.000000 ./bin/build/lib/pulumi_opnsense/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-14 13:29:05.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     1809 2023-07-14 13:29:05.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/py.typed
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     4539 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/host_override.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      696 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)     4425 2023-07-14 13:29:05.000000 ./bin/pulumi_opnsense/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:05.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-07-14 13:29:05.000000 ./bin/dist/pulumi_opnsense-0.0.29.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-14 13:29:04.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     1807 2023-07-14 13:29:04.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:04.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:04.000000 ./pulumi_opnsense/py.typed
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-14 13:29:04.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-14 13:29:04.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     4539 2023-07-14 13:29:04.000000 ./pulumi_opnsense/host_override.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-07-14 13:29:04.000000 ./pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      696 2023-07-14 13:29:04.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-14 13:29:04.000000 ./pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)     4425 2023-07-14 13:29:04.000000 ./pulumi_opnsense/random.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/lib/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-17 11:31:52.000000 ./bin/README.md
+-rw-------   0 runner    (1001) docker     (123)     1809 2023-07-17 11:31:52.000000 ./bin/setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/py.typed
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/host_override.py
+-rw-------   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-17 11:31:53.000000 ./bin/dist/pulumi_opnsense-0.0.34.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-17 11:31:50.000000 ./README.md
+-rw-------   0 runner    (1001) docker     (123)     1807 2023-07-17 11:31:49.000000 ./setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/py.typed
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:49.000000 ./pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:49.000000 ./pulumi_opnsense/host_override.py
+-rw-------   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:49.000000 ./pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:49.000000 ./pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:49.000000 ./pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:49.000000 ./pulumi_opnsense/random.py
```

### ./bin/pulumi_opnsense.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.29
+Version: 0.0.34
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
 
 This repository is a boilerplate showing how to create a native Pulumi provider.
```

### ./bin/setup.py

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.29"
-PLUGIN_VERSION = "0.0.29"
+VERSION = "0.0.34"
+PLUGIN_VERSION = "0.0.34"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION])
         except OSError as error:
```

