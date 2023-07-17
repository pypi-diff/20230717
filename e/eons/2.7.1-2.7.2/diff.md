# Comparing `tmp/eons-2.7.1.tar.gz` & `tmp/eons-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.7.1.tar", last modified: Mon Jul 17 05:20:13 2023, max compression
+gzip compressed data, was "eons-2.7.2.tar", last modified: Mon Jul 17 15:15:20 2023, max compression
```

## Comparing `eons-2.7.1.tar` & `eons-2.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 05:20:13.437435 eons-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-17 05:19:55.000000 eons-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.433435 eons-2.7.1/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98853 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 05:20:03.000000 eons-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 05:20:13.441435 eons-2.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.355358 eons-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 15:15:20.355358 eons-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-17 15:14:53.000000 eons-2.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.347358 eons-2.7.2/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99076 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.355358 eons-2.7.2/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 15:15:11.000000 eons-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 15:15:20.355358 eons-2.7.2/setup.cfg
```

### Comparing `eons-2.7.1/PKG-INFO` & `eons-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.1
+Version: 2.7.2
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.1/README.md` & `eons-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/pkg/eons/eons.py` & `eons-2.7.2/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,15 @@
 		# Also see FetchWith and FetchWithout for ease-of-use methods.
 		this.fetchFrom = [
 			'this',
 			'args',
 			'globals',
 			'config', #local (if applicable) or per Executor; should be before 'executor' if using a local config.
 			'precursor',
+			'caller',
 			'executor',
 			'environment',
 		]
 
 		# Fetch is modular.
 		# You can add your own {'from':this.customSearchMethod} pairs to fetchLocations by overriding PopulateFetchLocations().
 		# Alternatively, you may add to fetchLocations automatically by adding a fetchFrom entry and defining a method called f"fetch_location_{your new fetchFrom entry}(this, varName, default)".
@@ -479,14 +480,18 @@
 		this.functionSucceeded = True
 		this.rollbackSucceeded = True
 
 		# That which came before.
 		this.precursor = None
 
 		# The progenitor of *this.
+		# i.e. the object that called *this, aka 'owner', 'caller', etc.
+		this.caller = None
+
+		# The overarching program manager.
 		this.executor = None
 
 		# Those which come next (in order).
 		this.next = []
 
 		# Callback method
 		this.callbacks = util.DotDict()
@@ -1023,31 +1028,37 @@
 	######## START: Fetch Locations ########
 
 	def fetch_location_this(this, varName, default, fetchFrom, attempted):
 		if (util.HasAttr(this, varName)):
 			return util.GetAttr(this, varName), True
 		return default, False
 
-
-	def fetch_location_precursor(this, varName, default, fetchFrom, attempted):
-		if (this.precursor is None):
-			return default, False
-		return this.precursor.FetchWithAndWithout(['this'], ['environment'], varName, default, fetchFrom, False, attempted)
-
-
 	def fetch_location_args(this, varName, default, fetchFrom, attempted):
 
 		# this.args can't be searched.
 
 		for key, val in this.kwargs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 
+	def fetch_location_precursor(this, varName, default, fetchFrom, attempted):
+		if (this.precursor is None):
+			return default, False
+		return this.precursor.FetchWithAndWithout(['this'], ['environment'], varName, default, fetchFrom, False, attempted)
+	
+	
+	def fetch_location_caller(this, varName, default, fetchFrom, attempted):
+		if (not this.caller):
+			return default, False
+		
+		return this.caller.FetchWithout(['environment'], varName, default, fetchFrom, False, attempted)
+
+
 	# Call the Executor's Fetch method.
 	# Exclude 'environment' because we can check that ourselves.
 	def fetch_location_executor(this, varName, default, fetchFrom, attempted):
 		return this.GetExecutor().FetchWithout(['environment'], varName, default, fetchFrom, False, attempted)
 
 
 	#NOTE: There is no config in the default Functor. This is done for the convenience of children.
@@ -1349,18 +1360,14 @@
 		this.functionSucceeded = True
 		this.rollbackSucceeded = True
 		this.enableRollback = False
 
 		# The source code of the function we're implementing.
 		this.source = ""
 
-		# The instance of the class to which *this belongs.
-		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.caller = None
-
 		this.original = util.DotDict()
 		this.original.cls = util.DotDict()
 		this.original.cls.object = None
 		this.original.cls.name = 'None'
 		this.original.function = None
```

### Comparing `eons-2.7.1/pkg/eons/method/External.py` & `eons-2.7.2/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.7.2/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/pkg/eons/resolve/resolve_import_module.py` & `eons-2.7.2/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/pkg/eons.egg-info/PKG-INFO` & `eons-2.7.2/pkg/eons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.1
+Version: 2.7.2
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.1/pkg/eons.egg-info/SOURCES.txt` & `eons-2.7.2/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.7.1/setup.cfg` & `eons-2.7.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.7.1
+version = 2.7.2
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -19,19 +19,19 @@
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	requests_futures
-	pyyaml
-	tqdm
+	eot
 	jsonpickle
 	requests
-	eot
+	pyyaml
+	tqdm
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

