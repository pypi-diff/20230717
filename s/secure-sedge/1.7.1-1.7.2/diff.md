# Comparing `tmp/secure_sedge-1.7.1.tar.gz` & `tmp/secure_sedge-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_sedge-1.7.1.tar", last modified: Fri Feb 24 18:45:16 2023, max compression
+gzip compressed data, was "secure_sedge-1.7.2.tar", last modified: Mon Jul 17 07:07:39 2023, max compression
```

## Comparing `secure_sedge-1.7.1.tar` & `secure_sedge-1.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-09-12 16:52:26.000000 secure_sedge-1.7.1/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/PKG-INFO
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/docs/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2022-12-16 04:04:13.000000 secure_sedge-1.7.1/docs/index.rst
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/secure_sedge.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      105 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/secure_sedge.egg-info/top_level.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/sedge/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-24 18:39:46.000000 secure_sedge-1.7.1/sedge/README.md
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2022-09-12 16:49:44.000000 secure_sedge-1.7.1/sedge/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    15958 2023-02-15 01:29:06.000000 secure_sedge-1.7.1/sedge/installers.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1207 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/sedge/main.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    29492 2023-02-24 18:42:37.000000 secure_sedge-1.7.1/sedge/sewer.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/sedge/version.txt
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2023-02-24 18:45:16.619833 secure_sedge-1.7.1/setup.cfg
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2599 2023-02-24 18:45:16.000000 secure_sedge-1.7.1/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-07-30 10:57:45.000000 secure_sedge-1.7.2/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/PKG-INFO
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/docs/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2023-01-24 17:30:51.000000 secure_sedge-1.7.2/docs/index.rst
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/secure_sedge.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      111 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/top_level.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/sedge/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-21 19:50:49.000000 secure_sedge-1.7.2/sedge/README.md
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2021-08-03 07:09:12.000000 secure_sedge-1.7.2/sedge/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    19655 2023-07-17 07:05:30.000000 secure_sedge-1.7.2/sedge/installers.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1207 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/sedge/main.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    29492 2023-04-06 05:19:53.000000 secure_sedge-1.7.2/sedge/sewer.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/sedge/version.txt
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/setup.cfg
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2616 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/setup.py
```

### Comparing `secure_sedge-1.7.1/PKG-INFO` & `secure_sedge-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_sedge
-Version: 1.7.1
+Version: 1.7.2
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.7.1/docs/index.rst` & `secure_sedge-1.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.1/secure_sedge.egg-info/PKG-INFO` & `secure_sedge-1.7.2/secure_sedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-sedge
-Version: 1.7.1
+Version: 1.7.2
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.7.1/sedge/README.md` & `secure_sedge-1.7.2/sedge/README.md`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.1/sedge/main.py` & `secure_sedge-1.7.2/sedge/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
             'handlers': [ 'console-brief', ],
             'propagate': False,
         }
     }
 ))
 ns = Collection.from_module(sewer)
 ns.add_collection(installers.installers_collection, 'install')
-program = Program(version='1.7.1', namespace=ns)
+program = Program(version='1.7.2', namespace=ns)
```

### Comparing `secure_sedge-1.7.1/sedge/sewer.py` & `secure_sedge-1.7.2/sedge/sewer.py`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.1/setup.py` & `secure_sedge-1.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     from pkg_resources import resource_string
     readme_text = resource_string('sedge', 'README.md')
     readme_text = readme_text.decode('utf-8')
 
 # Version info -- read without importing
 _locals = {}
-version = '1.7.1'
+version = '1.7.2'
 
 
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ['*.yaml2', 'tests']
 
@@ -67,10 +67,11 @@
     install_requires=[
         'raft>=1.4.1.2',
         'boto3',
         'sewer[route53]==0.8.2',
         'pyyaml',
         'colorlog',
         'requests',
+        'pyjks',
         "pythonnet; sys.platform == 'win32'",
     ],
 )
```

