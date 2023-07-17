# Comparing `tmp/eons-2.7.0.tar.gz` & `tmp/eons-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.7.0.tar", last modified: Sun Jul 16 23:55:49 2023, max compression
+gzip compressed data, was "eons-2.7.1.tar", last modified: Mon Jul 17 05:20:13 2023, max compression
```

## Comparing `eons-2.7.0.tar` & `eons-2.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.678105 eons-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-07-16 23:55:49.678105 eons-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-07-16 23:55:33.000000 eons-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.674106 eons-2.7.0/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.678105 eons-2.7.0/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 23:55:41.000000 eons-2.7.0/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97060 2023-07-16 23:55:41.000000 eons-2.7.0/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.678105 eons-2.7.0/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:55:41.000000 eons-2.7.0/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.678105 eons-2.7.0/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:55:41.000000 eons-2.7.0/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 23:55:26.000000 eons-2.7.0/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:55:49.678105 eons-2.7.0/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-07-16 23:55:49.000000 eons-2.7.0/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 23:55:49.000000 eons-2.7.0/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:55:49.000000 eons-2.7.0/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 23:55:49.000000 eons-2.7.0/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 23:55:49.000000 eons-2.7.0/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 23:55:41.000000 eons-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-16 23:55:49.682105 eons-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 05:20:13.437435 eons-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-17 05:19:55.000000 eons-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.433435 eons-2.7.1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98853 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:03.000000 eons-2.7.1/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 05:19:48.000000 eons-2.7.1/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:20:13.437435 eons-2.7.1/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 05:20:13.000000 eons-2.7.1/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 05:20:03.000000 eons-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 05:20:13.441435 eons-2.7.1/setup.cfg
```

### Comparing `eons-2.7.0/PKG-INFO` & `eons-2.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.0
+Version: 2.7.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,16 @@
 
 The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
 ## Kind
 
+(totally unrelated to the [Kind Proof Language](https://github.com/HigherOrderCO/Kind); we just wanted a short synonym to "type" that didn't collide with Python's reserved keywords)
+
 Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
 The most condensed form of our syntax is as follows:
 
 ```python
 @eons.kind(parent/base, classes)
 def ClassName(
@@ -49,27 +51,66 @@
 this.classVariable = "Whatever you want!"
 """,
 ):
 	this.result.data.myResult = external_method(this.classVariable)
 
 ```
 
-This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development) (ELD). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
 
 The main differences between the Kind syntax and the Eons Language of Development are:
 * The `@eons.kind` decorator is used to declare a Type Block.
 * `this` is used instead of `$` (or `self` in Python).
+* `caller` is used instead of `$$`.
 * Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
 * Sequences are built by `eons.Flow()`s (still under development).
 * Python STILL does not have multiline comments >:(
 * Python has both dictionaries and lists, vs just Containers in ELD
 * `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
 * Convenient type casting is not fully implemented in Kind.
 * Access control is not yet implemented in Kind.
 
+### Caller
+
+When composing Functors, the `this` keyword is often ambiguous. Between functions of a class, `this` always refers to the class itself. However, when each function is also a class, does `this` mean the Functor or the class to which it belongs?
+
+To answer this question, ELD introduces the keyword `$$`. In Kind, we simply call this `caller`.
+
+So, you can use `caller.someMember` to share access across Functors composed by the same class, and `this.someMember` to access the Functor's own members.
+
+### Access Control
+There is no true access control in Python. So, implementing it via Biology has been slow going. However, for now, you can use something akin to ELD's `public(...)` Functor to make defining method injection easier.
+
+Instead of saying:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    Method1 = eons.inject('Method1'),
+    method2 = eons.inject('SomeOtherFunctor'),
+    MeThOd3 = eons.inject('METHOD3'),
+): 
+    pass
+```
+
+you can say:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    doesNotMatter = eons.public_methods(
+        'Method1',
+        method3 = 'SomeOtherFunctor',
+        MeThOd3 = 'METHOD3',
+    ),
+): 
+    pass
+```
+Unfortunately, you have to assign the result of `eons.public_methods` to a key word arg. However, the arg name is never used. We recommend using `public` or something trivial.
+
+Eventually, a generic `eons.public(...)` method should exist such that you can specify variable in addition to methods, but that is not yet implemented.
+
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
 To create your own executable, override `Executor` to add functionality to your program then create children of `Datum` and `Functor` for adding your own data structures and operations.
```

### Comparing `eons-2.7.0/README.md` & `eons-2.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
 ## Kind
 
+(totally unrelated to the [Kind Proof Language](https://github.com/HigherOrderCO/Kind); we just wanted a short synonym to "type" that didn't collide with Python's reserved keywords)
+
 Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
 The most condensed form of our syntax is as follows:
 
 ```python
 @eons.kind(parent/base, classes)
 def ClassName(
@@ -34,27 +36,66 @@
 this.classVariable = "Whatever you want!"
 """,
 ):
 	this.result.data.myResult = external_method(this.classVariable)
 
 ```
 
-This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development) (ELD). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
 
 The main differences between the Kind syntax and the Eons Language of Development are:
 * The `@eons.kind` decorator is used to declare a Type Block.
 * `this` is used instead of `$` (or `self` in Python).
+* `caller` is used instead of `$$`.
 * Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
 * Sequences are built by `eons.Flow()`s (still under development).
 * Python STILL does not have multiline comments >:(
 * Python has both dictionaries and lists, vs just Containers in ELD
 * `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
 * Convenient type casting is not fully implemented in Kind.
 * Access control is not yet implemented in Kind.
 
+### Caller
+
+When composing Functors, the `this` keyword is often ambiguous. Between functions of a class, `this` always refers to the class itself. However, when each function is also a class, does `this` mean the Functor or the class to which it belongs?
+
+To answer this question, ELD introduces the keyword `$$`. In Kind, we simply call this `caller`.
+
+So, you can use `caller.someMember` to share access across Functors composed by the same class, and `this.someMember` to access the Functor's own members.
+
+### Access Control
+There is no true access control in Python. So, implementing it via Biology has been slow going. However, for now, you can use something akin to ELD's `public(...)` Functor to make defining method injection easier.
+
+Instead of saying:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    Method1 = eons.inject('Method1'),
+    method2 = eons.inject('SomeOtherFunctor'),
+    MeThOd3 = eons.inject('METHOD3'),
+): 
+    pass
+```
+
+you can say:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    doesNotMatter = eons.public_methods(
+        'Method1',
+        method3 = 'SomeOtherFunctor',
+        MeThOd3 = 'METHOD3',
+    ),
+): 
+    pass
+```
+Unfortunately, you have to assign the result of `eons.public_methods` to a key word arg. However, the arg name is never used. We recommend using `public` or something trivial.
+
+Eventually, a generic `eons.public(...)` method should exist such that you can specify variable in addition to methods, but that is not yet implemented.
+
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
 To create your own executable, override `Executor` to add functionality to your program then create children of `Datum` and `Functor` for adding your own data structures and operations.
```

### Comparing `eons-2.7.0/pkg/eons/eons.py` & `eons-2.7.1/pkg/eons/eons.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
 import traceback
 import jsonpickle
+import inspect
+import operator
 from pathlib import Path
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
-import inspect
-import operator
 import re
 import argparse
 import requests
 import yaml
 from requests_futures.sessions import FuturesSession
 from tqdm import tqdm
 from zipfile import ZipFile
@@ -778,15 +778,15 @@
 						this.methods[method.name].next.append(methodToInsert)
 				else:
 					this.methods[method.name] = deepcopy(method)
 					this.methods[method.name].UpdateSource()
 
 		for method in this.methods.values():
 			logging.debug(f"Populating method {this.name}.{method.name}({', '.join([a for a in method.requiredKWArgs] + [a+'='+str(v) for a,v in method.optionalKWArgs.items()])})")
-			method.object = this
+			method.caller = this
 
 			# Python < 3.11
 			# setattr(this, method.name, method.__call__.__get__(this, this.__class__))
 
 			# appears to work for all python versions >= 3.8
 			setattr(this, method.name, method.__call__.__get__(method, method.__class__))
 
@@ -1076,14 +1076,204 @@
 		if (envVar is not None):
 			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
+# Invoke the External Method machinery to fetch a Functor & return it.
+# This should be used with other eons.kinds
+class Inject(Functor):
+	def __init__(this, name = "Inject"):
+		super().__init__(name)
+		this.requiredKWArgs.append('target')
+		this.optionalKWArgs['impl'] = 'External'
+
+		this.argMapping.append('target')
+		this.argMapping.append('impl')
+	
+	def Function(this):
+		# Prepare a dummy function to replace with a Method.
+		code = compile(f"def {this.target}(this):\n\tpass", '', 'exec')
+		exec(code)
+
+		methodToAdd = SelfRegistering(this.impl)
+		methodToAdd.Constructor(eval(this.target), None)
+		for key, value in this.kwargs.items():
+			setattr(methodToAdd, key, value)
+
+		return methodToAdd
+
+def inject(
+	target,
+	impl="External",
+	**kwargs
+):
+	return Inject()(target=target, impl=impl, **kwargs)
+
+
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# The data *this contains.
+		this.data = []
+
+
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
+
+
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
+
+
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
+
+
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
+
+
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
+
+
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
+
+
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
+
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
+
+
+
 def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
 	raise MethodPendingPopulation("METHOD PENDING POPULATION")
 
 # Store the new method in the class
 def PrepareClassMethod(cls, name, methodToAdd):
 	# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
 	if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
@@ -1161,15 +1351,15 @@
 		this.enableRollback = False
 
 		# The source code of the function we're implementing.
 		this.source = ""
 
 		# The instance of the class to which *this belongs.
 		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.object = None
+		this.caller = None
 
 		this.original = util.DotDict()
 		this.original.cls = util.DotDict()
 		this.original.cls.object = None
 		this.original.cls.name = 'None'
 		this.original.function = None
 
@@ -1184,24 +1374,23 @@
 		if (this.executor and this.executor.verbosity > 3):
 			logging.debug(f"Source for {this.name} is:\n{completeSource}")
 		code = compile(completeSource, '', 'exec')
 		exec(code)
 		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
 
 
-
 	# Parse arguments and update the source code
-	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
+	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.caller.this.caller.Improvement").
 	def PopulateFrom(this, function):
 		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
 
 		args = inspect.signature(function, follow_wrapped=False).parameters
 		thisSymbol = next(iter(args))
 		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
-		this.source = this.source.replace(thisSymbol, 'this.object')
+		this.source = this.source.replace(thisSymbol, 'this.caller')
 
 		first = True
 		for arg in args.values(): #args.values[1:] also doesn't work.
 			if (first):
 				first = False
 				continue
 
@@ -1239,18 +1428,18 @@
 		
 		# UpdateSource is called by Functor.PopulateMethods()
 		# this.UpdateSource()
 
 
 	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
 	def PopulatePrecursor(this):
-		if (not this.object):
+		if (not this.caller):
 			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.name}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
 
-		this.executor = this.object.executor
+		this.executor = this.caller.executor
 
 		if ('precursor' in this.kwargs):
 			this.precursor = this.kwargs.pop('precursor')
 		else:
 			this.precursor = None
 
 
@@ -1439,48 +1628,59 @@
 			pass
 
 	@staticmethod
 	def GetLatest():
 		return ExecutorTracker.Instance().executors[-1]
 
 
-def kind(
-	base = StandardFunctor,
-	**kwargs
-):
-	def FunctionToFunctor(function):
-		executor = ExecutorTracker.GetLatest()
-		shouldLog = executor and executor.verbosity > 3
+# AccessControl is used in Kind to control how Surfaces are created on a Functor & what is injected inside them.
+# parameters should roughly map to the parameters result of inspect.signature().parameters
+class AccessControl(Functor):
+	def __init__(this, name = "AccessControl"):
+		super().__init__(name)
 
-		bases = base
-		if (isinstance(bases, type)):
-			bases = [bases]
-		
-		primaryFunctionName = bases[0].primaryFunctionName
+		this.parameters = util.DotDict()
 
-		functor = type(
-			function.__name__,
-			(*bases,),
-			{}
-		)
+# Ease of use means of specifying a number of Methods to Inject
+class PublicMethods(AccessControl):
+	def __init__(this, name = "Public Methods"):
+		super().__init__(name)
 
-		if ('name' not in kwargs):
-			kwargs['name'] = function.__name__
-	
-		args = inspect.signature(function).parameters
-		source = inspect.getsource(function)
-		source = source[source.find(':')+1:].strip()
+	def Function(this):
+		toInject = {}
 
-		ctorSource = []
-		ctorAdditions = None
+		# Functor doesn't allow arbitrary arg handling.
+		# for arg in this.parameters:
+		# 	toInject[arg] = arg
 
+		for key, value in this.kwargs.items():
+			toInject[key] = value
+		
+		for target, source in toInject.items():
+			this.parameters[target] = util.DotDict({
+				'kind': None,
+				'name': target,
+				'default': inject(source)
+			})
+
+		return this
+
+def public_methods(*args, **kwargs):
+	[kwargs.update({arg: arg}) for arg in args]
+	return PublicMethods()(**kwargs)
+
+def kind(
+	base = StandardFunctor,
+	**kwargs
+):
+	def ParseParameters(functor, args, source, ctor):
 		# Code duplicated from Method.PopulateFrom. See that class for more info.
 		for arg in args.values():
 			if (arg.name == 'constructor' or arg.name == '__init__'):
-				ctorAdditions = arg.default
+				ctor.additions += f"{arg.default}\n"
 				continue
 
 			replaceWith = arg.name
 
 			# *args
 			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
 				replaceWith = 'this.args'
@@ -1495,32 +1695,74 @@
 				shouldMapArg = arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]
 
 				if (arg.default != inspect.Parameter.empty):
 					if (isinstance(arg.default, Method)):
 						arg.default.name = arg.name # Rename the Functor to match what was requested
 						PrepareClassMethod(functor, arg.name, arg.default)
 						shouldMapArg = False
+					elif (isinstance(arg.default, AccessControl)):
+						# NOTE: arg.name is discarded.
+						functor, source, ctor = ParseParameters(
+							functor,
+							arg.default.parameters,
+							source,
+							ctor
+						)
+						shouldMapArg = False
 					else:
-						ctorSource.append(f"this.optionalKWArgs['{arg.name}'] = {arg.default}")
+						ctor.source.append(f"this.optionalKWArgs['{arg.name}'] = {arg.default}")
 				else:
-					ctorSource.append(f"this.requiredKWArgs.append('{arg.name}')")
+					ctor.source.append(f"this.requiredKWArgs.append('{arg.name}')")
 
 				if (shouldMapArg):
-					ctorSource.append(f"this.argMapping.append('{arg.name}')")
+					ctor.source.append(f"this.argMapping.append('{arg.name}')")
 
 			# Source mangling
 			source = source.replace(arg.name, replaceWith)
+			
+		return functor, source, ctor
+
+	def FunctionToFunctor(function):
+		executor = ExecutorTracker.GetLatest()
+		shouldLog = executor and executor.verbosity > 3
+
+		bases = base
+		if (isinstance(bases, type)):
+			bases = [bases]
+		
+		primaryFunctionName = bases[0].primaryFunctionName
+
+		functor = type(
+			function.__name__,
+			(*bases,),
+			{}
+		)
+
+		if ('name' not in kwargs):
+			kwargs['name'] = function.__name__
+	
+		args = inspect.signature(function).parameters
+		source = inspect.getsource(function)
+		source = source[source.find(':')+1:].strip()
+		source = source.replace('caller', 'this.caller')
+
+		ctor = util.DotDict()
+		ctor.source = []
+		ctor.additions = ""
+
+		functor, source, ctor = ParseParameters(functor, args, source, ctor)
 
 		# Constructor creation
 		constructorName = f"_eons_constructor_{kwargs['name']}"
 		constructorSource = f"def {constructorName}(this, name='{function.__name__}'):"
-		ctorSource.insert(0, f"super(this.__class__, this).__init__(name)")
-		constructorSource += '\n\t' + '\n\t'.join(ctorSource)
-		if (ctorAdditions):
-			constructorSource += '\n\t' + ('\n\t'.join(ctorAdditions.split('\n'))).replace('self', 'this')
+		ctor.source.insert(0, f"super(this.__class__, this).__init__(name)")
+		constructorSource += '\n\t' + '\n\t'.join(ctor.source)
+		if (len(ctor.additions)):
+			re.sub(r'^\s+', '\n', ctor.additions)
+			constructorSource += '\n\t' + ('\n\t'.join(ctor.additions.split('\n'))).replace('self', 'this')
 		if (shouldLog):
 			logging.debug(f"Constructor source for {kwargs['name']}:\n{constructorSource}")
 		code = compile(constructorSource, '', 'exec')
 		exec(code)
 		exec(f'functor.__init__ = {constructorName}')
 
 		wrappedPrimaryFunction = f"_eons_method_{kwargs['name']}"
@@ -1535,200 +1777,14 @@
 		exec(f'functor.{primaryFunctionName} = {wrappedPrimaryFunction}')
 
 		return functor
 
 	return FunctionToFunctor
 
 
-# Invoke the External Method machinery to fetch a Functor & return it.
-# This should be used with other eons.kinds
-@kind(Functor)
-def Inject(
-	target,
-	impl="External",
-	**kwargs
-):
-	# Prepare a dummy function to replace with a Method.
-	code = compile(f"def {target}(this):\n\tpass", '', 'exec')
-	exec(code)
-
-	methodToAdd = SelfRegistering(impl)
-	methodToAdd.Constructor(eval(target), None)
-	for key, value in kwargs.items():
-		setattr(methodToAdd, key, value)
-
-	return methodToAdd
-
-def inject(
-	target,
-	impl="External",
-	**kwargs
-):
-	return Inject()(target, impl, **kwargs)
-
-
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
-
-
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
-
-
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
-
-
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
-
-
-
 class FetchCallbackFunctor(Functor):
 
 	def __init__(this, name = "FetchCallbackFunctor"):
 		super().__init__(name)
 
 		this.requiredKWArgs.append('varName')
 		this.requiredKWArgs.append('location')
```

### Comparing `eons-2.7.0/pkg/eons/method/External.py` & `eons-2.7.1/pkg/eons/method/External.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,11 +33,14 @@
 	def PopulateFrom(this, function):
 		this.functorName = function.__name__
 
 	def Function(this):
 		kwargs = this.kwargs
 		kwargs.update({
 			'executor': this.executor,
-			'precursor': this
+			'precursor': this,
 		})
+		
+		this.functor.caller = this.caller
+		
 		return this.functor(*this.args, **kwargs)
```

### Comparing `eons-2.7.0/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.7.1/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.0/pkg/eons/resolve/resolve_import_module.py` & `eons-2.7.1/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.7.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.0/pkg/eons.egg-info/PKG-INFO` & `eons-2.7.1/pkg/eons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.0
+Version: 2.7.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,16 @@
 
 The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
 ## Kind
 
+(totally unrelated to the [Kind Proof Language](https://github.com/HigherOrderCO/Kind); we just wanted a short synonym to "type" that didn't collide with Python's reserved keywords)
+
 Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
 The most condensed form of our syntax is as follows:
 
 ```python
 @eons.kind(parent/base, classes)
 def ClassName(
@@ -49,27 +51,66 @@
 this.classVariable = "Whatever you want!"
 """,
 ):
 	this.result.data.myResult = external_method(this.classVariable)
 
 ```
 
-This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development) (ELD). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
 
 The main differences between the Kind syntax and the Eons Language of Development are:
 * The `@eons.kind` decorator is used to declare a Type Block.
 * `this` is used instead of `$` (or `self` in Python).
+* `caller` is used instead of `$$`.
 * Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
 * Sequences are built by `eons.Flow()`s (still under development).
 * Python STILL does not have multiline comments >:(
 * Python has both dictionaries and lists, vs just Containers in ELD
 * `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
 * Convenient type casting is not fully implemented in Kind.
 * Access control is not yet implemented in Kind.
 
+### Caller
+
+When composing Functors, the `this` keyword is often ambiguous. Between functions of a class, `this` always refers to the class itself. However, when each function is also a class, does `this` mean the Functor or the class to which it belongs?
+
+To answer this question, ELD introduces the keyword `$$`. In Kind, we simply call this `caller`.
+
+So, you can use `caller.someMember` to share access across Functors composed by the same class, and `this.someMember` to access the Functor's own members.
+
+### Access Control
+There is no true access control in Python. So, implementing it via Biology has been slow going. However, for now, you can use something akin to ELD's `public(...)` Functor to make defining method injection easier.
+
+Instead of saying:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    Method1 = eons.inject('Method1'),
+    method2 = eons.inject('SomeOtherFunctor'),
+    MeThOd3 = eons.inject('METHOD3'),
+): 
+    pass
+```
+
+you can say:
+```python
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+    doesNotMatter = eons.public_methods(
+        'Method1',
+        method3 = 'SomeOtherFunctor',
+        MeThOd3 = 'METHOD3',
+    ),
+): 
+    pass
+```
+Unfortunately, you have to assign the result of `eons.public_methods` to a key word arg. However, the arg name is never used. We recommend using `public` or something trivial.
+
+Eventually, a generic `eons.public(...)` method should exist such that you can specify variable in addition to methods, but that is not yet implemented.
+
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
 To create your own executable, override `Executor` to add functionality to your program then create children of `Datum` and `Functor` for adding your own data structures and operations.
```

### Comparing `eons-2.7.0/pkg/eons.egg-info/SOURCES.txt` & `eons-2.7.1/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.7.0/setup.cfg` & `eons-2.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.7.0
+version = 2.7.1
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,19 +18,19 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	jsonpickle
-	requests
 	requests_futures
 	pyyaml
 	tqdm
+	jsonpickle
+	requests
 	eot
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build =
```

