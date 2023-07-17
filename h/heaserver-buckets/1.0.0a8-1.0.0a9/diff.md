# Comparing `tmp/heaserver-buckets-1.0.0a8.tar.gz` & `tmp/heaserver-buckets-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-buckets-1.0.0a8.tar", last modified: Fri Jun 10 03:46:14 2022, max compression
+gzip compressed data, was "heaserver-buckets-1.0.0a9.tar", last modified: Fri Jun 17 20:06:12 2022, max compression
```

## Comparing `heaserver-buckets-1.0.0a8.tar` & `heaserver-buckets-1.0.0a9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.026750 heaserver-buckets-1.0.0a8/
--rw-rw-rw-   0        0        0      261 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/.editorconfig
--rw-rw-rw-   0        0        0      288 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/.gitignore
--rw-rw-rw-   0        0        0     1482 2022-06-10 03:45:07.000000 heaserver-buckets-1.0.0a8/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      272 2022-06-09 04:48:45.000000 heaserver-buckets-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4455 2022-06-10 03:46:14.026750 heaserver-buckets-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3164 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a8/README.md
--rw-rw-rw-   0        0        0     1767 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/RELEASING.md
--rw-rw-rw-   0        0        0      390 2022-04-04 15:48:22.000000 heaserver-buckets-1.0.0a8/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/integrationtests/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.006558 heaserver-buckets-1.0.0a8/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      404 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a8/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     5538 2022-06-09 00:47:25.000000 heaserver-buckets-1.0.0a8/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0       92 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/pytest.ini
--rw-rw-rw-   0        0        0      210 2022-06-09 05:25:37.000000 heaserver-buckets-1.0.0a8/requirements_dev.txt
--rw-rw-rw-   0        0        0     5773 2022-06-10 02:41:42.000000 heaserver-buckets-1.0.0a8/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2022-06-10 03:46:14.026750 heaserver-buckets-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1795 2022-06-10 03:45:34.000000 heaserver-buckets-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.006558 heaserver-buckets-1.0.0a8/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    16216 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a8/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.006558 heaserver-buckets-1.0.0a8/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0     6316 2022-04-14 23:38:17.000000 heaserver-buckets-1.0.0a8/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.026750 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     4455 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-10 03:46:13.000000 heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:13.965679 heaserver-buckets-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-06-10 03:46:14.026750 heaserver-buckets-1.0.0a8/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a8/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0      404 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a8/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     5599 2022-06-10 02:41:59.000000 heaserver-buckets-1.0.0a8/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.623222 heaserver-buckets-1.0.0a9/
+-rw-rw-rw-   0        0        0      261 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/.editorconfig
+-rw-rw-rw-   0        0        0      288 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/.gitignore
+-rw-rw-rw-   0        0        0     1482 2022-06-10 03:45:07.000000 heaserver-buckets-1.0.0a9/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      272 2022-06-09 04:48:45.000000 heaserver-buckets-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4455 2022-06-17 20:06:12.623222 heaserver-buckets-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3164 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0     1767 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/RELEASING.md
+-rw-rw-rw-   0        0        0      390 2022-04-04 15:48:22.000000 heaserver-buckets-1.0.0a9/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.531993 heaserver-buckets-1.0.0a9/integrationtests/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.531993 heaserver-buckets-1.0.0a9/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.602981 heaserver-buckets-1.0.0a9/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      404 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a9/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     5622 2022-06-17 20:03:42.000000 heaserver-buckets-1.0.0a9/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0       92 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/pytest.ini
+-rw-rw-rw-   0        0        0      210 2022-06-09 05:25:37.000000 heaserver-buckets-1.0.0a9/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5773 2022-06-10 02:41:42.000000 heaserver-buckets-1.0.0a9/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2022-06-17 20:06:12.623222 heaserver-buckets-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1795 2022-06-17 20:05:13.000000 heaserver-buckets-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.534010 heaserver-buckets-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.531993 heaserver-buckets-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.605005 heaserver-buckets-1.0.0a9/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    16216 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a9/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.605005 heaserver-buckets-1.0.0a9/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0     6316 2022-04-14 23:38:17.000000 heaserver-buckets-1.0.0a9/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.615172 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     4455 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-06-17 20:06:12.000000 heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.534010 heaserver-buckets-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.534010 heaserver-buckets-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-06-17 20:06:12.615172 heaserver-buckets-1.0.0a9/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 20:12:39.000000 heaserver-buckets-1.0.0a9/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0      404 2022-06-08 00:12:57.000000 heaserver-buckets-1.0.0a9/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     5683 2022-06-17 20:03:42.000000 heaserver-buckets-1.0.0a9/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver-buckets-1.0.0a8/Dockerfile` & `heaserver-buckets-1.0.0a9/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/LICENSE` & `heaserver-buckets-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/PKG-INFO` & `heaserver-buckets-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-buckets-1.0.0a8/README.md` & `heaserver-buckets-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/RELEASING.md` & `heaserver-buckets-1.0.0a9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver-buckets-1.0.0a9/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,23 +104,23 @@
                                      wstl_package=service.__package__,
                                      href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/',
                                      fixtures=db_store,
                                      db_manager_cls=MockS3Manager,
                                      get_actions=[Action(name='heaserver-buckets-bucket-get-properties',
                                                          rel=['hea-properties']),
                                                   Action(name='heaserver-buckets-bucket-get-open-choices',
-                                                         url='/volumes/{volume_id}/buckets/{id}/opener',
+                                                         url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/opener',
                                                          rel=['hea-opener-choices']),
                                                   Action(name='heaserver-buckets-bucket-duplicate',
-                                                         url='/volumes/{volume_id}/buckets/{id}/duplicator',
+                                                         url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/duplicator',
                                                          rel=['hea-duplicator'])
                                                   ],
                                      get_all_actions=[Action(name='heaserver-buckets-bucket-get-properties',
                                                              rel=['hea-properties']),
                                                       Action(name='heaserver-buckets-bucket-get-open-choices',
-                                                             url='/volumes/{volume_id}/buckets/{id}/opener',
+                                                             url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/opener',
                                                              rel=['hea-opener-choices']),
                                                       Action(name='heaserver-buckets-bucket-duplicate',
-                                                             url='/volumes/{volume_id}/buckets/{id}/duplicator',
+                                                             url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/duplicator',
                                                              rel=['hea-duplicator'])],
                                      duplicate_action_name='heaserver-buckets-bucket-duplicate-form',
                                      exclude=['body_put'])
```

### Comparing `heaserver-buckets-1.0.0a8/run-swaggerui.py` & `heaserver-buckets-1.0.0a9/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/setup.py` & `heaserver-buckets-1.0.0a9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.bucket'],
     package_data={'heaserver.bucket': ['wstl/*.json']},
-    install_requires=['heaserver>=1.0.0a70, <1.0.0a71'],
+    install_requires=['heaserver>=1.0.0a71, <1.0.0a72'],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-buckets-1.0.0a8/src/heaserver/bucket/service.py` & `heaserver-buckets-1.0.0a9/src/heaserver/bucket/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/src/heaserver/bucket/wstl/all.json` & `heaserver-buckets-1.0.0a9/src/heaserver/bucket/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-buckets-1.0.0a8/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver-buckets-1.0.0a9/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.0a8/tests/heaserver/buckettest/testcase.py` & `heaserver-buckets-1.0.0a9/tests/heaserver/buckettest/testcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,23 +104,23 @@
                                      wstl_package=service.__package__,
                                      href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/',
                                      fixtures=db_store,
                                      db_manager_cls=MockS3ManagerWithMockMongo,
                                      get_actions=[Action(name='heaserver-buckets-bucket-get-properties',
                                                              rel=['hea-properties']),
                                                   Action(name='heaserver-buckets-bucket-get-open-choices',
-                                                             url='/volumes/{volume_id}/buckets/{id}/opener',
+                                                             url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/opener',
                                                              rel=['hea-opener-choices']),
                                                   Action(name='heaserver-buckets-bucket-duplicate',
-                                                             url='/volumes/{volume_id}/buckets/{id}/duplicator',
+                                                             url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/duplicator',
                                                              rel=['hea-duplicator'])
                                                   ],
                                      get_all_actions=[Action(name='heaserver-buckets-bucket-get-properties',
                                                                  rel=['hea-properties']),
                                                       Action(name='heaserver-buckets-bucket-get-open-choices',
-                                                                 url='/volumes/{volume_id}/buckets/{id}/opener',
+                                                                 url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/opener',
                                                                  rel=['hea-opener-choices']),
                                                       Action(name='heaserver-buckets-bucket-duplicate',
-                                                                 url='/volumes/{volume_id}/buckets/{id}/duplicator',
+                                                                 url='http://localhost:8080/volumes/{volume_id}/buckets/{id}/duplicator',
                                                                  rel=['hea-duplicator'])],
                                      duplicate_action_name='heaserver-buckets-bucket-duplicate-form',
                                      exclude=['body_put'])
```

