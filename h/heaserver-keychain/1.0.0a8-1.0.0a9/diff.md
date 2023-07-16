# Comparing `tmp/heaserver-keychain-1.0.0a8.tar.gz` & `tmp/heaserver-keychain-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-keychain-1.0.0a8.tar", last modified: Tue Aug 16 20:49:42 2022, max compression
+gzip compressed data, was "heaserver-keychain-1.0.0a9.tar", last modified: Wed Nov  2 23:02:21 2022, max compression
```

## Comparing `heaserver-keychain-1.0.0a8.tar` & `heaserver-keychain-1.0.0a9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.564789 heaserver-keychain-1.0.0a8/
--rw-rw-rw-   0        0        0      312 2022-08-16 20:46:30.000000 heaserver-keychain-1.0.0a8/.gitignore
--rw-rw-rw-   0        0        0     1524 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/Dockerfile
--rw-rw-rw-   0        0        0    11625 2021-10-27 20:37:26.000000 heaserver-keychain-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      272 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4838 2022-08-16 20:49:42.563791 heaserver-keychain-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3562 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/README.md
--rw-rw-rw-   0        0        0     2654 2022-03-10 18:51:48.000000 heaserver-keychain-1.0.0a8/RELEASING.md
--rw-rw-rw-   0        0        0      410 2022-03-10 18:51:48.000000 heaserver-keychain-1.0.0a8/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.461043 heaserver-keychain-1.0.0a8/integrationtests/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.461043 heaserver-keychain-1.0.0a8/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.523790 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/
--rw-rw-rw-   0        0        0        0 2021-10-27 20:37:26.000000 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     3757 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1083 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     3547 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/testcase.py
--rw-rw-rw-   0        0        0       92 2021-11-22 21:24:02.000000 heaserver-keychain-1.0.0a8/pytest.ini
--rw-rw-rw-   0        0        0      327 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/requirements_dev.txt
--rw-rw-rw-   0        0        0     1048 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2022-08-16 20:49:42.564789 heaserver-keychain-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1787 2022-08-16 20:42:27.000000 heaserver-keychain-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.463043 heaserver-keychain-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.462043 heaserver-keychain-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.531788 heaserver-keychain-1.0.0a8/src/heaserver/keychain/
--rw-rw-rw-   0        0        0        0 2021-10-27 20:37:26.000000 heaserver-keychain-1.0.0a8/src/heaserver/keychain/__init__.py
--rw-rw-rw-   0        0        0    13000 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/src/heaserver/keychain/service.py
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.536788 heaserver-keychain-1.0.0a8/src/heaserver/keychain/wstl/
--rw-rw-rw-   0        0        0     7408 2022-08-04 22:54:13.000000 heaserver-keychain-1.0.0a8/src/heaserver/keychain/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.547789 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/
--rw-rw-rw-   0        0        0     4838 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-16 20:49:42.000000 heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.464042 heaserver-keychain-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.464042 heaserver-keychain-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:49:42.562788 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/
--rw-rw-rw-   0        0        0        0 2021-10-27 20:37:26.000000 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/__init__.py
--rw-rw-rw-   0        0        0     3620 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/test_all.py
--rw-rw-rw-   0        0        0     1083 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     3439 2022-08-16 20:42:00.000000 heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/testcase.py
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.076179 heaserver-keychain-1.0.0a9/
+-rw-rw-rw-   0        0        0      312 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/.gitignore
+-rw-rw-rw-   0        0        0     1579 2022-11-02 20:17:16.000000 heaserver-keychain-1.0.0a9/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      272 2022-06-10 21:50:39.000000 heaserver-keychain-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4838 2022-11-02 23:02:21.075661 heaserver-keychain-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3562 2022-07-01 00:00:21.000000 heaserver-keychain-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0     2654 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/RELEASING.md
+-rw-rw-rw-   0        0        0      410 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/integrationtests/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.050625 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     3757 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     3547 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0       92 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/pytest.ini
+-rw-rw-rw-   0        0        0      327 2022-07-01 00:00:21.000000 heaserver-keychain-1.0.0a9/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1048 2022-06-10 21:50:39.000000 heaserver-keychain-1.0.0a9/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2022-11-02 23:02:21.076696 heaserver-keychain-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2022-11-02 23:02:10.000000 heaserver-keychain-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.050625 heaserver-keychain-1.0.0a9/src/heaserver/keychain/
+-rw-rw-rw-   0        0        0        0 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/src/heaserver/keychain/__init__.py
+-rw-rw-rw-   0        0        0    13000 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/src/heaserver/keychain/service.py
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.050625 heaserver-keychain-1.0.0a9/src/heaserver/keychain/wstl/
+-rw-rw-rw-   0        0        0     7408 2022-07-01 00:00:21.000000 heaserver-keychain-1.0.0a9/src/heaserver/keychain/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.069472 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/
+-rw-rw-rw-   0        0        0     4838 2022-11-02 23:02:20.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1111 2022-11-02 23:02:21.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-02 23:02:20.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2022-11-02 23:02:20.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-11-02 23:02:20.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-11-02 23:02:20.000000 heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.040619 heaserver-keychain-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-11-02 23:02:21.074632 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 01:58:57.000000 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/__init__.py
+-rw-rw-rw-   0        0        0     3620 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     3439 2022-11-02 20:16:33.000000 heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/testcase.py
```

### Comparing `heaserver-keychain-1.0.0a8/Dockerfile` & `heaserver-keychain-1.0.0a9/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #     python setup.py clean --all sdist bdist_wheel
 #
 # Run the image from the HEA Main project with the following command (see the top of the docker-compose-dev.yml file
 # for instructions):
 #     docker-compose -f ./docker-compose-dev.yml up
 #
 
-FROM hea-python-base:latest
+FROM registry.gitlab.com/huntsman-cancer-institute/risr/hea/hea-python-base:3.10.3
 
 ARG SOURCE
 ARG INDEX_URL=https://pypi.python.org/simple
 
 RUN apt-get update && \
     apt-get install --no-install-recommends -y git && \
     apt-get clean && rm -rf /var/lib/apt/lists/*
```

### Comparing `heaserver-keychain-1.0.0a8/LICENSE` & `heaserver-keychain-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/PKG-INFO` & `heaserver-keychain-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-keychain-1.0.0a8/README.md` & `heaserver-keychain-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/RELEASING.md` & `heaserver-keychain-1.0.0a9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py` & `heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py` & `heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/integrationtests/heaserver/keychainintegrationtest/testcase.py` & `heaserver-keychain-1.0.0a9/integrationtests/heaserver/keychainintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/run-swaggerui.py` & `heaserver-keychain-1.0.0a9/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/setup.py` & `heaserver-keychain-1.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-keychain',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="a service for managing laboratory credentials",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.keychain'],
     package_data={'heaserver.keychain': ['wstl/*.json']},
-    install_requires=['heaserver>=1.0.0a76, <1.0.0a77'],
+    install_requires=['heaserver>=1.0.0a84, <1.0.0a85'],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-keychain-1.0.0a8/src/heaserver/keychain/service.py` & `heaserver-keychain-1.0.0a9/src/heaserver/keychain/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/src/heaserver/keychain/wstl/all.json` & `heaserver-keychain-1.0.0a9/src/heaserver/keychain/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/PKG-INFO` & `heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-keychain-1.0.0a8/src/heaserver_keychain.egg-info/SOURCES.txt` & `heaserver-keychain-1.0.0a9/src/heaserver_keychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/permissionstestcase.py` & `heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/test_all_with_bad_permissions.py` & `heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-keychain-1.0.0a8/tests/heaserver/keychaintest/testcase.py` & `heaserver-keychain-1.0.0a9/tests/heaserver/keychaintest/testcase.py`

 * *Files identical despite different names*

