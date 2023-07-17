# Comparing `tmp/DS_test-1.1.tar.gz` & `tmp/DS_test-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DS_test-1.1.tar", last modified: Mon Jul 17 06:10:04 2023, max compression
+gzip compressed data, was "dist\DS_test-1.2.tar", last modified: Mon Jul 17 06:58:04 2023, max compression
```

## Comparing `DS_test-1.1.tar` & `DS_test-1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:10:04.461893 DS_test-1.1/
-drwxrwxrwx   0        0        0        0 2023-07-17 06:10:04.460894 DS_test-1.1/DS_test.egg-info/
--rw-rw-rw-   0        0        0      487 2023-07-17 06:10:04.000000 DS_test-1.1/DS_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-17 06:10:04.000000 DS_test-1.1/DS_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:10:04.000000 DS_test-1.1/DS_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-17 06:10:04.000000 DS_test-1.1/DS_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:10:04.000000 DS_test-1.1/DS_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      487 2023-07-17 06:10:04.461893 DS_test-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 06:10:04.461893 DS_test-1.1/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-07-17 05:42:28.000000 DS_test-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:58:04.768050 DS_test-1.2/
+drwxrwxrwx   0        0        0        0 2023-07-17 06:58:04.766056 DS_test-1.2/DS_test.egg-info/
+-rw-rw-rw-   0        0        0      487 2023-07-17 06:58:04.000000 DS_test-1.2/DS_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-17 06:58:04.000000 DS_test-1.2/DS_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:58:04.000000 DS_test-1.2/DS_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 06:58:04.000000 DS_test-1.2/DS_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:58:04.000000 DS_test-1.2/DS_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      487 2023-07-17 06:58:04.768050 DS_test-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:58:04.769087 DS_test-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-07-17 06:57:50.000000 DS_test-1.2/setup.py
```

### Comparing `DS_test-1.1/setup.py` & `DS_test-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 setup(
     name='DS_test',
-    version='1.1',
+    version='1.2',
     description='A sample Python project',
     author='wzq',
     author_email='',
     packages=find_packages(),
     install_requires=[
         'numpy',
-        'pyyaml == 6.0',
+        'pyyaml == 5.4',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

