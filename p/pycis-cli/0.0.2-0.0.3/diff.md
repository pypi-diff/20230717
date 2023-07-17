# Comparing `tmp/pycis_cli-0.0.2.tar.gz` & `tmp/pycis_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycis_cli-0.0.2.tar", max compression
+gzip compressed data, was "pycis_cli-0.0.3.tar", max compression
```

## Comparing `pycis_cli-0.0.2.tar` & `pycis_cli-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-07-12 18:00:09.011444 pycis_cli-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      394 2023-07-15 21:22:15.146910 pycis_cli-0.0.2/README.rst
--rw-r--r--   0        0        0      994 2023-07-15 22:28:04.932985 pycis_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 03:17:30.118993 pycis_cli-0.0.2/source/packages/pycis/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 04:12:29.753800 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      768 2023-07-15 21:02:15.428500 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/__init__.py
--rw-r--r--   0        0        0       43 2023-07-15 21:15:03.524375 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/constants.py
--rw-r--r--   0        0        0      802 2023-07-15 21:02:15.432500 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
--rw-r--r--   0        0        0     2942 2023-07-15 21:15:03.528375 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
--rw-r--r--   0        0        0     2616 2023-07-15 21:15:03.528375 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
--rw-r--r--   0        0        0      602 2023-07-15 21:02:15.432500 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
--rw-r--r--   0        0        0     2883 2023-07-15 21:15:03.528375 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
--rw-r--r--   0        0        0      713 2023-07-15 21:02:15.432500 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/__init__.py
--rw-r--r--   0        0        0      612 2023-07-15 21:02:15.432500 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-15 22:16:27.245663 pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py
--rw-r--r--   0        0        0     1273 2023-07-15 21:02:15.428500 pycis_cli-0.0.2/source/packages/pycis/cli/pycis_command.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 pycis_cli-0.0.2/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 pycis_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-12 18:00:09.011444 pycis_cli-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      394 2023-07-15 21:22:15.146910 pycis_cli-0.0.3/README.rst
+-rw-r--r--   0        0        0      994 2023-07-17 16:44:10.669246 pycis_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 03:17:30.118993 pycis_cli-0.0.3/source/packages/pycis/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 04:12:29.753800 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-15 21:02:15.428500 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-15 21:15:03.524375 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/constants.py
+-rw-r--r--   0        0        0      802 2023-07-15 21:02:15.432500 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
+-rw-r--r--   0        0        0     2942 2023-07-15 21:15:03.528375 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
+-rw-r--r--   0        0        0     2616 2023-07-15 21:15:03.528375 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
+-rw-r--r--   0        0        0      602 2023-07-15 21:02:15.432500 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
+-rw-r--r--   0        0        0     2883 2023-07-15 21:15:03.528375 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
+-rw-r--r--   0        0        0      713 2023-07-15 21:02:15.432500 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/__init__.py
+-rw-r--r--   0        0        0      612 2023-07-15 21:02:15.432500 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-15 22:16:27.245663 pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/testrun/create.py
+-rw-r--r--   0        0        0     1273 2023-07-15 21:02:15.428500 pycis_cli-0.0.3/source/packages/pycis/cli/pycis_command.py
+-rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 pycis_cli-0.0.3/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 pycis_cli-0.0.3/PKG-INFO
```

### Comparing `pycis_cli-0.0.2/LICENSE.txt` & `pycis_cli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/pyproject.toml` & `pycis_cli-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pycis-cli"
 description = "Python Continuous Integration System (PyCIS) - CLI Tools"
-version = "0.0.2"
+version = "0.0.3"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
@@ -19,15 +19,15 @@
 python = ">=3.8,<4.0"
 click = "^8.1.4"
 pymongo = {extras = ["srv"], version = "^4.0.0", optional = true}
 couchdb = {version = "^1.2", optional = true}
 mojo-xmodules = ">=0.0.55 <0.1.0"
 
 [tool.poetry.scripts]
-greet = "pycis.cli.pycis_command:pycis_root_command"
+pycis = "pycis.cli.pycis_command:pycis_root_command"
 
 [tool.poetry.extras]
 mongodb = ["pymongo"]
 couchdb = ["couchdb"]
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
```

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/__init__.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/__init__.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/cmdtree/document/testrun/create.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/cmdtree/document/testrun/create.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/source/packages/pycis/cli/pycis_command.py` & `pycis_cli-0.0.3/source/packages/pycis/cli/pycis_command.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.2/setup.py` & `pycis_cli-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 install_requires = \
 ['click>=8.1.4,<9.0.0', 'mojo-xmodules>=0.0.55,<0.1.0']
 
 extras_require = \
 {'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo[srv]>=4.0.0,<5.0.0']}
 
 entry_points = \
-{'console_scripts': ['greet = pycis.cli.pycis_command:pycis_root_command']}
+{'console_scripts': ['pycis = pycis.cli.pycis_command:pycis_root_command']}
 
 setup_kwargs = {
     'name': 'pycis-cli',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Python Continuous Integration System (PyCIS) - CLI Tools',
     'long_description': '========================================================\nPython Continuous Integration System (PyCIS) - CLI Tools\n========================================================\n\nProvides a set of CLI tools for working with the PyCIS continuous integration system.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pycis_cli-0.0.2/PKG-INFO` & `pycis_cli-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycis-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Continuous Integration System (PyCIS) - CLI Tools
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

