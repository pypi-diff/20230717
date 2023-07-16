# Comparing `tmp/banking_logging-0.1.0.tar.gz` & `tmp/banking_logging-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banking_logging-0.1.0.tar", last modified: Sun Jul 16 23:27:44 2023, max compression
+gzip compressed data, was "banking_logging-0.2.tar", last modified: Sun Jul 16 23:29:22 2023, max compression
```

## Comparing `banking_logging-0.1.0.tar` & `banking_logging-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:27:44.032777 banking_logging-0.1.0/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:27:44.031778 banking_logging-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 23:27:44.005777 banking_logging-0.1.0/banking_logging/
--rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.1.0/banking_logging/__init__.py
--rw-rw-rw-   0        0        0     6765 2023-07-16 23:23:20.000000 banking_logging-0.1.0/banking_logging/banking_logging.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:27:44.029776 banking_logging-0.1.0/banking_logging.egg-info/
--rw-rw-rw-   0        0        0      253 2023-07-16 23:27:43.000000 banking_logging-0.1.0/banking_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-16 23:27:43.000000 banking_logging-0.1.0/banking_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:27:43.000000 banking_logging-0.1.0/banking_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 23:27:43.000000 banking_logging-0.1.0/banking_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 23:27:44.032777 banking_logging-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-05-27 16:51:00.000000 banking_logging-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:29:22.254202 banking_logging-0.2/
+-rw-rw-rw-   0        0        0      251 2023-07-16 23:29:22.252204 banking_logging-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-27 16:57:34.000000 banking_logging-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 23:29:22.236203 banking_logging-0.2/banking_logging/
+-rw-rw-rw-   0        0        0       32 2023-05-27 16:48:39.000000 banking_logging-0.2/banking_logging/__init__.py
+-rw-rw-rw-   0        0        0     6765 2023-07-16 23:23:20.000000 banking_logging-0.2/banking_logging/banking_logging.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:29:22.251218 banking_logging-0.2/banking_logging.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-16 23:29:22.000000 banking_logging-0.2/banking_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-16 23:29:22.000000 banking_logging-0.2/banking_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:29:22.000000 banking_logging-0.2/banking_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 23:29:22.000000 banking_logging-0.2/banking_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:29:22.254202 banking_logging-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-07-16 23:29:05.000000 banking_logging-0.2/setup.py
```

### Comparing `banking_logging-0.1.0/README.md` & `banking_logging-0.2/README.md`

 * *Files identical despite different names*

### Comparing `banking_logging-0.1.0/banking_logging/banking_logging.py` & `banking_logging-0.2/banking_logging/banking_logging.py`

 * *Files identical despite different names*

### Comparing `banking_logging-0.1.0/setup.py` & `banking_logging-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
             'maintainer_email': 'edazizovv@gmail.com',
             'description': 'Shared loggers for banking_api project',
             'license': 'Proprietary',
             'url': '',
             'download_url': '',
             'packages': setuptools.find_packages(),
             'include_package_data': True,
-            'version': '0.1.0',
+            'version': '0.2',
             'long_description': '',
             'python_requires': '>=3.10',
             'install_requires': []}
 
 setup(**metadata)
```

