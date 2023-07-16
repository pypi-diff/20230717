# Comparing `tmp/eons-2.6.6.tar.gz` & `tmp/eons-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.6.tar", last modified: Mon Jul 10 02:32:36 2023, max compression
+gzip compressed data, was "eons-2.6.7.tar", last modified: Sun Jul 16 23:47:19 2023, max compression
```

## Comparing `eons-2.6.6.tar` & `eons-2.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-07-10 02:32:36.257643 eons-2.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-10 02:32:20.000000 eons-2.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.253643 eons-2.6.6/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.253643 eons-2.6.6/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93216 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:28.000000 eons-2.6.6/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 02:32:13.000000 eons-2.6.6/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:32:36.257643 eons-2.6.6/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 02:32:36.000000 eons-2.6.6/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 02:32:28.000000 eons-2.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-10 02:32:36.261643 eons-2.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.254984 eons-2.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-07-16 23:47:19.254984 eons-2.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-07-16 23:46:59.000000 eons-2.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.250984 eons-2.6.7/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.250984 eons-2.6.7/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 23:47:09.000000 eons-2.6.7/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97060 2023-07-16 23:47:09.000000 eons-2.6.7/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.254984 eons-2.6.7/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:47:09.000000 eons-2.6.7/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.254984 eons-2.6.7/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:47:09.000000 eons-2.6.7/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 23:46:51.000000 eons-2.6.7/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:47:19.250984 eons-2.6.7/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-07-16 23:47:19.000000 eons-2.6.7/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 23:47:19.000000 eons-2.6.7/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:47:19.000000 eons-2.6.7/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 23:47:19.000000 eons-2.6.7/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 23:47:19.000000 eons-2.6.7/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 23:47:09.000000 eons-2.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-16 23:47:19.254984 eons-2.6.7/setup.cfg
```

### Comparing `eons-2.6.6/PKG-INFO` & `eons-2.6.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,74 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.6
+Version: 2.6.7
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Eons Python Framework
 
-The Eons Python Framework provides a Python counterpart to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
+The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
-## Eons vs Biology
+## Kind
 
-The Eons library is designed for plug-and-play development, unlike Biology. This means it's faster to get up and running but has fewer features, is less optimized, and will likely be slower to run. Additionally, Eons is only single threaded (due to Python limitations), while Biology is multi-threaded by default. Due to the single thread limitation of this framework, the full neural-processing of Biology is reduced to only a single sequence of operations at a time. However, by allowing those operations to be arbitrarily complex, build off each other, and be loaded from the cloud at runtime, we aim to provide the same level of functionality, if not better, than what Biology provides by default. Both systems work toward a full implementation of the [Eons Language of Development](https://github.com/develop-biology/language.development).
+Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
-Once Develop Biology is stable and the Native Biology Syntax is fully developed, the Eons Python Framework and all downstream implementations will be merged into a single, flexible, and optimized solution. However, the builtin reflection features of Biology should make it such that a successful integration means no changes to downstream code. Python can stay Python, or become any other language you want. Stay tuned!
+The most condensed form of our syntax is as follows:
+
+```python
+@eons.kind(parent/base, classes)
+def ClassName(
+    member,
+    variables,
+    which = "are injected via Fetch"
+):
+    # Your code goes here.
+    this.isHow = "you reference the object / instance"
+```
+
+Here's a more complete example:
+```python
+import eons
+
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+	external_method = eons.inject('SomeFarAwayFunctor'),
+	constructor = f"""
+# Until Execution Blocks can be created in Parameter Blocks, formatted, multiline strings are the only way to handle arbitrary logic.
+
+this.classVariable = "Whatever you want!"
+""",
+):
+	this.result.data.myResult = external_method(this.classVariable)
+
+```
+
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+
+The main differences between the Kind syntax and the Eons Language of Development are:
+* The `@eons.kind` decorator is used to declare a Type Block.
+* `this` is used instead of `$` (or `self` in Python).
+* Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
+* Sequences are built by `eons.Flow()`s (still under development).
+* Python STILL does not have multiline comments >:(
+* Python has both dictionaries and lists, vs just Containers in ELD
+* `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
+* Convenient type casting is not fully implemented in Kind.
+* Access control is not yet implemented in Kind.
 
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
@@ -58,15 +99,15 @@
 * Managed composition through External Methods.
 * Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
-2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
+2. The json configuration file supplied with `--config` (or specified by `this.defaultConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
 4. Member variables of the Executor (e.g. `this.some_key = "some value"`)
 
 The higher the number on the above list, the higher the precedence of the search location. For example, member variables will always be returned before values from the environment.
 
 Downstream implementors of the Eons library may optionally extend the `Fetch()` method to look through whatever layers are appropriate for their inputs.
 
@@ -128,17 +169,32 @@
     @method(impl="External")
     def MyExternalFunctor(): pass
 ```
 Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
 
 Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
 
+#### Kind
+
+When using Kind syntax, use `eons.inject` instead of `@method` (Python prohibits the use of decorators in Parameter Blocks).
+
+NOTE: Kind allows you to change the name of the External Method, while the decorator does not.
+
+For example:
+```python
+@eons.kind(eons.Functor)
+def MyClass(
+    WeCanChangeThisNameNow = eons.inject("MyExternalFunctor")
+):
+...
+```
+
 #### Requirements & Notes
 
-1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info. **NOTE: This is now done for you automatically by the Placement system.**
 
 2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
 
 3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
 
 ### Error Resolution for `@recoverable` Methods
 
@@ -238,15 +294,15 @@
 
 ### Self Registration
 
 Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
-NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organize inheritance dependencies, but can be disabled with `recurse=False`.
 
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
```

### Comparing `eons-2.6.6/README.md` & `eons-2.6.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,59 @@
 # Eons Python Framework
 
-The Eons Python Framework provides a Python counterpart to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
+The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
-## Eons vs Biology
+## Kind
 
-The Eons library is designed for plug-and-play development, unlike Biology. This means it's faster to get up and running but has fewer features, is less optimized, and will likely be slower to run. Additionally, Eons is only single threaded (due to Python limitations), while Biology is multi-threaded by default. Due to the single thread limitation of this framework, the full neural-processing of Biology is reduced to only a single sequence of operations at a time. However, by allowing those operations to be arbitrarily complex, build off each other, and be loaded from the cloud at runtime, we aim to provide the same level of functionality, if not better, than what Biology provides by default. Both systems work toward a full implementation of the [Eons Language of Development](https://github.com/develop-biology/language.development).
+Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
-Once Develop Biology is stable and the Native Biology Syntax is fully developed, the Eons Python Framework and all downstream implementations will be merged into a single, flexible, and optimized solution. However, the builtin reflection features of Biology should make it such that a successful integration means no changes to downstream code. Python can stay Python, or become any other language you want. Stay tuned!
+The most condensed form of our syntax is as follows:
+
+```python
+@eons.kind(parent/base, classes)
+def ClassName(
+    member,
+    variables,
+    which = "are injected via Fetch"
+):
+    # Your code goes here.
+    this.isHow = "you reference the object / instance"
+```
+
+Here's a more complete example:
+```python
+import eons
+
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+	external_method = eons.inject('SomeFarAwayFunctor'),
+	constructor = f"""
+# Until Execution Blocks can be created in Parameter Blocks, formatted, multiline strings are the only way to handle arbitrary logic.
+
+this.classVariable = "Whatever you want!"
+""",
+):
+	this.result.data.myResult = external_method(this.classVariable)
+
+```
+
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+
+The main differences between the Kind syntax and the Eons Language of Development are:
+* The `@eons.kind` decorator is used to declare a Type Block.
+* `this` is used instead of `$` (or `self` in Python).
+* Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
+* Sequences are built by `eons.Flow()`s (still under development).
+* Python STILL does not have multiline comments >:(
+* Python has both dictionaries and lists, vs just Containers in ELD
+* `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
+* Convenient type casting is not fully implemented in Kind.
+* Access control is not yet implemented in Kind.
 
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
@@ -43,15 +84,15 @@
 * Managed composition through External Methods.
 * Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
-2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
+2. The json configuration file supplied with `--config` (or specified by `this.defaultConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
 4. Member variables of the Executor (e.g. `this.some_key = "some value"`)
 
 The higher the number on the above list, the higher the precedence of the search location. For example, member variables will always be returned before values from the environment.
 
 Downstream implementors of the Eons library may optionally extend the `Fetch()` method to look through whatever layers are appropriate for their inputs.
 
@@ -113,17 +154,32 @@
     @method(impl="External")
     def MyExternalFunctor(): pass
 ```
 Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
 
 Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
 
+#### Kind
+
+When using Kind syntax, use `eons.inject` instead of `@method` (Python prohibits the use of decorators in Parameter Blocks).
+
+NOTE: Kind allows you to change the name of the External Method, while the decorator does not.
+
+For example:
+```python
+@eons.kind(eons.Functor)
+def MyClass(
+    WeCanChangeThisNameNow = eons.inject("MyExternalFunctor")
+):
+...
+```
+
 #### Requirements & Notes
 
-1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info. **NOTE: This is now done for you automatically by the Placement system.**
 
 2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
 
 3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
 
 ### Error Resolution for `@recoverable` Methods
 
@@ -223,15 +279,15 @@
 
 ### Self Registration
 
 Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
-NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organize inheritance dependencies, but can be disabled with `recurse=False`.
 
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
```

### Comparing `eons-2.6.6/pkg/eons/eons.py` & `eons-2.6.7/pkg/eons/eons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
-import operator
-import traceback
-import jsonpickle
-from copy import deepcopy
 import os
+import shutil
+from copy import deepcopy
+import builtins
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
-import inspect
-import shutil
-import builtins
-import re
+import traceback
+import jsonpickle
 from pathlib import Path
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
+import inspect
+import operator
+import re
 import argparse
 import requests
 import yaml
 from requests_futures.sessions import FuturesSession
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
@@ -61,157 +61,14 @@
 class FatalCannotExecute(Fatal, metaclass=ActualType): pass
 
 class PackageError(Exception, metaclass=ActualType): pass
 
 class MethodPendingPopulation(Exception, metaclass=ActualType): pass
 
 
-# util is a namespace for any miscellaneous utilities.
-# You cannot create a util.
-class util:
-	def __init__(this):
-		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
-
-	#dot.notation access to dictionary attributes
-	class DotDict(dict):
-		__getattr__ = dict.get
-		__setattr__ = dict.__setitem__
-		__delattr__ = dict.__delitem__
-
-		def __deepcopy__(this, memo=None):
-			return util.DotDict(deepcopy(dict(this), memo=memo))
-
-	# DotDict doesn't pickle right, since it's a class and not a native dict.
-	class DotDictPickler(jsonpickle.handlers.BaseHandler):
-		def flatten(this, dotdict, data):
-			return dict(dotdict)
-
-	@staticmethod
-	def RecursiveAttrFunc(func, obj, attrList):
-		attr = attrList.pop(0)
-		if (not attrList):
-			return eval(f"{func}attr(obj, attr)")
-		if (not hasattr(obj, attr)):
-			raise AttributeError(f"{obj} has not attribute '{attr}'")
-		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
-
-	@staticmethod
-	def HasAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
-
-	@staticmethod
-	def GetAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
-
-	@staticmethod
-	def SetAttr(obj, attrStr):
-		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
-
-
-	@staticmethod
-	def LogStack():
-		logging.debug(traceback.format_exc())
-
-
-	class console:
-
-		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
-
-		saturationCode = {
-			'dark': 3,
-			'light': 9
-		}
-
-		foregroundCodes = {
-			'black': 0,
-			'red': 1,
-			'green': 2,
-			'yellow': 3,
-			'blue': 4,
-			'magenta': 5,
-			'cyan': 6,
-			'white': 7
-		}
-
-		backgroundCodes = {
-			'none': 0,
-			'black': 40,
-			'red': 41,
-			'green': 42,
-			'yellow': 43,
-			'blue': 44,
-			'magenta': 45,
-			'cyan': 46,
-			'white': 47,
-		}
-
-		styleCodes = {
-			'none': 0,
-			'bold': 1,
-			'faint': 2, # Not widely supported.
-			'italic': 3, # Not widely supported.
-			'underline': 4,
-			'blink_slow': 5,
-			'blink_fast': 6, # Not widely supported.
-			'invert': 7,
-			'conceal': 8, # Not widely supported.
-			'strikethrough': 9, # Not widely supported.
-			'frame': 51,
-			'encircle': 52,
-			'overline': 53
-		}
-
-		@classmethod
-		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
-			if (styles is None):
-				styles = []
-			#\x1b may also work.
-			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
-			if (background != 'none'):
-				compiledCode += f";{cls.backgroundCodes[background]}"
-			if (styles):
-				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
-			compiledCode += 'm'
-			return compiledCode
-
-		resetStyle = "\033[0m"
-
-
-	# Add a logging level
-	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
-	@staticmethod
-	def AddLoggingLevel(level, value):
-		levelName = level.upper()
-		methodName = level.lower()
-
-		if hasattr(logging, levelName):
-			raise AttributeError('{} already defined in logging module'.format(levelName))
-		if hasattr(logging, methodName):
-			raise AttributeError('{} already defined in logging module'.format(methodName))
-		if hasattr(logging.getLogger(), methodName):
-			raise AttributeError('{} already defined in logger class'.format(methodName))
-
-		# This method was inspired by the answers to Stack Overflow post
-		# http://stackoverflow.com/q/2183233/2988730, especially
-		# http://stackoverflow.com/a/13638084/2988730
-		def logForLevel(this, message, *args, **kwargs):
-			if this.isEnabledFor(value):
-				this._log(value, message, args, **kwargs)
-		def logToRoot(message, *args, **kwargs):
-			logging.log(value, message, *args, **kwargs)
-
-		logging.addLevelName(value, levelName)
-		setattr(logging, levelName, value)
-		setattr(logging.getLogger(), methodName, logForLevel)
-		setattr(logging, methodName, logToRoot)
-
-
-jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
-
-
 #Self registration for use with json loading.
 #Any class that derives from SelfRegistering can be instantiated with:
 #   SelfRegistering("ClassName")
 #Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
 class SelfRegistering(object):
 
 	def __init__(this, *args, **kwargs):
@@ -321,171 +178,155 @@
 
 
 	# Sets valid to false.
 	def Invalidate(this):
 		this.valid = False
 
 
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
+# util is a namespace for any miscellaneous utilities.
+# You cannot create a util.
+class util:
+	def __init__(this):
+		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
 
+	#dot.notation access to dictionary attributes
+	class DotDict(dict):
+		__getattr__ = dict.get
+		__setattr__ = dict.__setitem__
+		__delattr__ = dict.__delitem__
 
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
+		def __deepcopy__(this, memo=None):
+			return util.DotDict(deepcopy(dict(this), memo=memo))
 
+	# DotDict doesn't pickle right, since it's a class and not a native dict.
+	class DotDictPickler(jsonpickle.handlers.BaseHandler):
+		def flatten(this, dotdict, data):
+			return dict(dotdict)
 
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
+	@staticmethod
+	def RecursiveAttrFunc(func, obj, attrList):
+		attr = attrList.pop(0)
+		if (not attrList):
+			return eval(f"{func}attr(obj, attr)")
+		if (not hasattr(obj, attr)):
+			raise AttributeError(f"{obj} has not attribute '{attr}'")
+		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
 
+	@staticmethod
+	def HasAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
 
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
+	@staticmethod
+	def GetAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
 
+	@staticmethod
+	def SetAttr(obj, attrStr):
+		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
 
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
 
+	@staticmethod
+	def LogStack():
+		logging.debug(traceback.format_exc())
 
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
 
+	class console:
 
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
+		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
 
+		saturationCode = {
+			'dark': 3,
+			'light': 9
+		}
 
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
+		foregroundCodes = {
+			'black': 0,
+			'red': 1,
+			'green': 2,
+			'yellow': 3,
+			'blue': 4,
+			'magenta': 5,
+			'cyan': 6,
+			'white': 7
+		}
 
+		backgroundCodes = {
+			'none': 0,
+			'black': 40,
+			'red': 41,
+			'green': 42,
+			'yellow': 43,
+			'blue': 44,
+			'magenta': 45,
+			'cyan': 46,
+			'white': 47,
+		}
 
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
+		styleCodes = {
+			'none': 0,
+			'bold': 1,
+			'faint': 2, # Not widely supported.
+			'italic': 3, # Not widely supported.
+			'underline': 4,
+			'blink_slow': 5,
+			'blink_fast': 6, # Not widely supported.
+			'invert': 7,
+			'conceal': 8, # Not widely supported.
+			'strikethrough': 9, # Not widely supported.
+			'frame': 51,
+			'encircle': 52,
+			'overline': 53
+		}
 
+		@classmethod
+		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
+			if (styles is None):
+				styles = []
+			#\x1b may also work.
+			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
+			if (background != 'none'):
+				compiledCode += f";{cls.backgroundCodes[background]}"
+			if (styles):
+				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
+			compiledCode += 'm'
+			return compiledCode
 
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
+		resetStyle = "\033[0m"
 
 
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
+	# Add a logging level
+	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
+	@staticmethod
+	def AddLoggingLevel(level, value):
+		levelName = level.upper()
+		methodName = level.lower()
 
+		if hasattr(logging, levelName):
+			raise AttributeError('{} already defined in logging module'.format(levelName))
+		if hasattr(logging, methodName):
+			raise AttributeError('{} already defined in logging module'.format(methodName))
+		if hasattr(logging.getLogger(), methodName):
+			raise AttributeError('{} already defined in logger class'.format(methodName))
 
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
+		# This method was inspired by the answers to Stack Overflow post
+		# http://stackoverflow.com/q/2183233/2988730, especially
+		# http://stackoverflow.com/a/13638084/2988730
+		def logForLevel(this, message, *args, **kwargs):
+			if this.isEnabledFor(value):
+				this._log(value, message, args, **kwargs)
+		def logToRoot(message, *args, **kwargs):
+			logging.log(value, message, *args, **kwargs)
 
+		logging.addLevelName(value, levelName)
+		setattr(logging, levelName, value)
+		setattr(logging.getLogger(), methodName, logForLevel)
+		setattr(logging, methodName, logToRoot)
 
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
 
+jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
 
 # FunctorTracker is a global singleton which keeps a record of all functors that are currently in the call stack.
 # Functors should add and remove themselves from this list when they are called.
 class FunctorTracker:
 	def __init__(this):
 		# Singletons man...
@@ -518,76 +359,29 @@
 			pass
 		tracker.functors.reverse()
 
 	@staticmethod
 	def GetCount():
 		return len(FunctorTracker.Instance().functors)
 
-
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
-#
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
-		else:
-			return None
-
-		this.executors = [None]
-
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
-
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
-
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
-
-		logging.debug(f"Now tracking Executor: {executor}")
-
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
-
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
-
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
 # Functors will automatically Fetch any ...Args specified.
 # You may additionally specify required methods (per @method()) and required programs (i.e. external binaries).
-# When Executing a Functor, you can say 'next=[...]', in which case multiple Functors will be Executed in sequence. This is necessary for the method propagation machinary to work.
+# When Executing a Functor, you can say 'next=[...]', in which case multiple Functors will be Executed in sequence. This is necessary for the method propagation machinery to work.
 # When invoking a sequence of Functors, only the result of the last Functor to be Executed or the first Functor to fail will be returned.
 class Functor(Datum):
 
+	# Which function should be overridden when creating a @kind from *this.
+	primaryFunctionName = 'Function'
+
 	def __init__(this, name=INVALID_NAME()):
 		super().__init__(name)
 
 		# Which method to call when executing *this through __call__.
 		this.callMethod = 'Function'
 		this.rollbackMethod = 'Rollback'
 
@@ -666,27 +460,28 @@
 
 		# Automatically return the result.data object if the function returns None
 		this.enableAutoReturn = True
 
 		# this.result encompasses the return value of *this.
 		# The code is a numerical result indication the success or failure of *this and is set automatically.
 		# 0 is success; 1 is no change; higher numbers are some kind of error.
-		# this.result.data should be set manuallly.
+		# this.result.data should be set manually.
 		# It is highly recommended that you check result.data in DidFunctionSucceed().
 		this.result = util.DotDict()
 		this.result.code = 0
 		this.result.data = util.DotDict()
 
 		# Whether or not we should pass on exceptions when calls fail.
 		this.raiseExceptions = True
 
 		# Ease of use members
 		# These can be calculated in Function and Rollback, respectively.
-		this.functionSucceeded = False
-		this.rollbackSucceeded = False
+		# Assume success to reduce the overhead of creating small Functors.
+		this.functionSucceeded = True
+		this.rollbackSucceeded = True
 
 		# That which came before.
 		this.precursor = None
 
 		# The progenitor of *this.
 		this.executor = None
 
@@ -1284,14 +1079,31 @@
 
 	######## END: Fetch Locations ########
 
 
 def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
 	raise MethodPendingPopulation("METHOD PENDING POPULATION")
 
+# Store the new method in the class
+def PrepareClassMethod(cls, name, methodToAdd):
+	# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
+	if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
+		cls.classMethods = {}
+	else:
+		# to account for the bug above, shadow classMethods out of the base class & into the derived.
+		setattr(cls, 'classMethods', getattr(cls, 'classMethods').copy())
+
+	cls.classMethods[name] = methodToAdd
+
+	# Self-destruct by replacing the decorated function.
+	# We rely on Functor.PopulateMethods to re-establish the method as callable.
+	# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
+	# Regardless deleting the method is okay as long as we add it back before anyone notices.
+	setattr(cls, name, METHOD_PENDING_POPULATION.__get__(cls))
+
 # Use the @method() decorator to turn any class function into an eons Method Functor.
 # Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
 # Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
 # All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
 #
 # If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
 # Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
@@ -1308,34 +1120,20 @@
 
 		# Apparently, this is called when the decorated function is constructed.
 		def __set_name__(this, cls, functionName):
 			logging.debug(f"Constructing new method for {this.function} in {cls}")
 
 			# Create and configure a new Method
 
-			method = SelfRegistering(impl)
-			method.Constructor(this.function, cls)
+			methodToAdd = SelfRegistering(impl)
+			methodToAdd.Constructor(this.function, cls)
 			for key, value in kwargs.items():
-				setattr(method, key, value)
+				setattr(methodToAdd, key, value)
 
-			# Store the new method in the class
-			# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
-			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
-				cls.classMethods = {}
-			else:
-				# to account for the bug above, shadow classMethods out of the base class & into the derived.
-				setattr(cls, 'classMethods', getattr(cls, 'classMethods').copy())
-			
-			cls.classMethods[functionName] = method
-
-			# Self-destruct by replacing the decorated function.
-			# We rely on Functor.PopulateMethods to re-establish the method as callable.
-			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
-			# Regardless deleting the method is okay as long as we add it back before anyone notices.
-			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
+			PrepareClassMethod(cls, functionName, methodToAdd)
 
 	return MethodDecorator
 
 class Method(Functor):
 
 	def __init__(this, name=INVALID_NAME()):
 		super().__init__(name)
@@ -1366,15 +1164,17 @@
 		this.source = ""
 
 		# The instance of the class to which *this belongs.
 		# i.e. the object that called *this, aka 'owner', 'caller', etc.
 		this.object = None
 
 		this.original = util.DotDict()
-		this.original.cls = None
+		this.original.cls = util.DotDict()
+		this.original.cls.object = None
+		this.original.cls.name = 'None'
 		this.original.function = None
 
 
 	# Make *this execute the code in this.source
 	def UpdateSource(this):
 		wrappedFunctionName = f'_eons_method_{this.name}'
 		completeSource = f'''\
@@ -1426,27 +1226,29 @@
 			this.source = this.source.replace(arg.name, replaceWith)
 
 
 	# When properly constructing a Method, rely only on the function *this should implement.
 	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
 	def Constructor(this, function, cls):
 		this.name = function.__name__
-		this.original.cls = cls
+		this.original.cls.object = cls
+		if (this.original.cls.object):
+			this.original.cls.name = this.original.cls.object.__name__
 		this.original.function = function
 
 		this.PopulateFrom(function)
 		
 		# UpdateSource is called by Functor.PopulateMethods()
 		# this.UpdateSource()
 
 
 	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
 	def PopulatePrecursor(this):
 		if (not this.object):
-			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
+			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.name}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
 
 		this.executor = this.object.executor
 
 		if ('precursor' in this.kwargs):
 			this.precursor = this.kwargs.pop('precursor')
 		else:
 			this.precursor = None
@@ -1465,114 +1267,14 @@
 		if (not this.next):
 			return None
 
 		for next in this.next:
 			next(precursor=this)
 
 
-class FetchCallbackFunctor(Functor):
-
-	def __init__(this, name = "FetchCallbackFunctor"):
-		super().__init__(name)
-
-		this.requiredKWArgs.append('varName')
-		this.requiredKWArgs.append('location')
-		this.requiredKWArgs.append('value')
-
-		this.functionSucceeded = True
-		this.enableRollback = False
-
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-#from .Executor import Executor # don't import this, it'll be circular!
-
-# @recoverable
-# Decorating another function with this method will engage the error recovery system provided by *this.
-# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
-# For more info, see Executor.ResolveError and the README.md
-def recoverable(function):
-	def RecoverableDecorator(obj, *args, **kwargs):
-		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
-	return RecoverableDecorator
-
-
-# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
-def RecoverableImplementation(obj, executor, function, *args, **kwargs):
-	try:
-		return function(obj, *args, **kwargs)
-	except FailedErrorResolution as fatal:
-		raise fatal
-	except Exception as e:
-		if (not executor.resolveErrors):
-			raise e
-		return Recover(e, obj, executor, function, *args, **kwargs)
-
-
-def Recover(error, obj, executor, function, *args, **kwargs):
-	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
-	util.LogStack()
-
-	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
-	if (str(error) not in executor.errorResolutionStack.keys()):
-		executor.errorResolutionStack.update({str(error):[]})
-
-	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
-	# ResolveError is itself @recoverable.
-	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
-	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
-	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
-
-	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
-		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
-
-	successfullyRecovered = False
-	ret = None
-	resolvedBy = None
-	for i, res in enumerate(executor.resolveErrorsWith):
-
-		logging.debug(f"Checking if {res} can fix '{error}'.")
-		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
-			# if no resolution was attempted, there's no need to re-run the function.
-			continue
-		try:
-			logging.debug(f"Trying function ({function}) again after applying {res}.")
-			resolvedBy = res
-			ret = function(obj, *args, **kwargs)
-			successfullyRecovered = True
-			break
-
-		except Exception as e2:
-			if (str(error) == str(e2)):
-				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
-				# Resolution failed. That's okay. Let's try the next.
-				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
-				continue
-			else:
-				# The error changed, maybe we're making progress.
-				ret = Recover(e2, obj, executor, function, *args, **kwargs)
-				successfullyRecovered = True
-				break
-
-	if (successfullyRecovered):
-		executor.ClearErrorResolutionStack(str(error)) # success!
-		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
-		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
-		return ret
-
-	#  We failed to resolve the error. Die
-	sys.tracebacklimit = 0 # traceback is NOT helpful here.
-	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
-
-
 # The standard Functor extends Functor to add a set of standard members and methods.
 # This is similar to the standard library in C and C++
 # You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
 class StandardFunctor(Functor):
 	def __init__(this, name="Standard Functor"):
 		super().__init__(name)
 
@@ -1687,14 +1389,446 @@
 		if (saveout):
 			return process.returncode, output
 		
 		return process.returncode
 	######## END: UTILITIES ########
 
 
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
+
+def kind(
+	base = StandardFunctor,
+	**kwargs
+):
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
+
+		ctorSource = []
+		ctorAdditions = None
+
+		# Code duplicated from Method.PopulateFrom. See that class for more info.
+		for arg in args.values():
+			if (arg.name == 'constructor' or arg.name == '__init__'):
+				ctorAdditions = arg.default
+				continue
+
+			replaceWith = arg.name
+
+			# *args
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			# **kwargs
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			# Normal argument
+			else:
+				replaceWith = f'this.{arg.name}'
+				shouldMapArg = arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]
+
+				if (arg.default != inspect.Parameter.empty):
+					if (isinstance(arg.default, Method)):
+						arg.default.name = arg.name # Rename the Functor to match what was requested
+						PrepareClassMethod(functor, arg.name, arg.default)
+						shouldMapArg = False
+					else:
+						ctorSource.append(f"this.optionalKWArgs['{arg.name}'] = {arg.default}")
+				else:
+					ctorSource.append(f"this.requiredKWArgs.append('{arg.name}')")
+
+				if (shouldMapArg):
+					ctorSource.append(f"this.argMapping.append('{arg.name}')")
+
+			# Source mangling
+			source = source.replace(arg.name, replaceWith)
+
+		# Constructor creation
+		constructorName = f"_eons_constructor_{kwargs['name']}"
+		constructorSource = f"def {constructorName}(this, name='{function.__name__}'):"
+		ctorSource.insert(0, f"super(this.__class__, this).__init__(name)")
+		constructorSource += '\n\t' + '\n\t'.join(ctorSource)
+		if (ctorAdditions):
+			constructorSource += '\n\t' + ('\n\t'.join(ctorAdditions.split('\n'))).replace('self', 'this')
+		if (shouldLog):
+			logging.debug(f"Constructor source for {kwargs['name']}:\n{constructorSource}")
+		code = compile(constructorSource, '', 'exec')
+		exec(code)
+		exec(f'functor.__init__ = {constructorName}')
+
+		wrappedPrimaryFunction = f"_eons_method_{kwargs['name']}"
+		completeSource = f'''\
+def {wrappedPrimaryFunction}(this):
+	{source}
+'''
+		if (shouldLog):
+			logging.debug(f"Primary function source for {kwargs['name']}:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'functor.{primaryFunctionName} = {wrappedPrimaryFunction}')
+
+		return functor
+
+	return FunctionToFunctor
+
+
+# Invoke the External Method machinery to fetch a Functor & return it.
+# This should be used with other eons.kinds
+@kind(Functor)
+def Inject(
+	target,
+	impl="External",
+	**kwargs
+):
+	# Prepare a dummy function to replace with a Method.
+	code = compile(f"def {target}(this):\n\tpass", '', 'exec')
+	exec(code)
+
+	methodToAdd = SelfRegistering(impl)
+	methodToAdd.Constructor(eval(target), None)
+	for key, value in kwargs.items():
+		setattr(methodToAdd, key, value)
+
+	return methodToAdd
+
+def inject(
+	target,
+	impl="External",
+	**kwargs
+):
+	return Inject()(target, impl, **kwargs)
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
+class FetchCallbackFunctor(Functor):
+
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
+
+		this.requiredKWArgs.append('varName')
+		this.requiredKWArgs.append('location')
+		this.requiredKWArgs.append('value')
+
+		this.functionSucceeded = True
+		this.enableRollback = False
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+#from .Executor import Executor # don't import this, it'll be circular!
+
+# @recoverable
+# Decorating another function with this method will engage the error recovery system provided by *this.
+# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
+# For more info, see Executor.ResolveError and the README.md
+def recoverable(function):
+	def RecoverableDecorator(obj, *args, **kwargs):
+		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
+	return RecoverableDecorator
+
+
+# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
+def RecoverableImplementation(obj, executor, function, *args, **kwargs):
+	try:
+		return function(obj, *args, **kwargs)
+	except FailedErrorResolution as fatal:
+		raise fatal
+	except Exception as e:
+		if (not executor.resolveErrors):
+			raise e
+		return Recover(e, obj, executor, function, *args, **kwargs)
+
+
+def Recover(error, obj, executor, function, *args, **kwargs):
+	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
+	util.LogStack()
+
+	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
+	if (str(error) not in executor.errorResolutionStack.keys()):
+		executor.errorResolutionStack.update({str(error):[]})
+
+	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
+	# ResolveError is itself @recoverable.
+	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
+	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
+	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
+
+	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
+		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
+
+	successfullyRecovered = False
+	ret = None
+	resolvedBy = None
+	for i, res in enumerate(executor.resolveErrorsWith):
+
+		logging.debug(f"Checking if {res} can fix '{error}'.")
+		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
+			# if no resolution was attempted, there's no need to re-run the function.
+			continue
+		try:
+			logging.debug(f"Trying function ({function}) again after applying {res}.")
+			resolvedBy = res
+			ret = function(obj, *args, **kwargs)
+			successfullyRecovered = True
+			break
+
+		except Exception as e2:
+			if (str(error) == str(e2)):
+				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
+				# Resolution failed. That's okay. Let's try the next.
+				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+				continue
+			else:
+				# The error changed, maybe we're making progress.
+				ret = Recover(e2, obj, executor, function, *args, **kwargs)
+				successfullyRecovered = True
+				break
+
+	if (successfullyRecovered):
+		executor.ClearErrorResolutionStack(str(error)) # success!
+		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
+		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
+		return ret
+
+	#  We failed to resolve the error. Die
+	sys.tracebacklimit = 0 # traceback is NOT helpful here.
+	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
+
+
 # Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
 # ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
 # Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
 # NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
 # startPosition is always positive
 # endPosition is always negative
```

### Comparing `eons-2.6.6/pkg/eons/method/External.py` & `eons-2.6.7/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.6/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.7/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.6/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.7/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.6/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.7/pkg/eons.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,74 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.6
+Version: 2.6.7
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Eons Python Framework
 
-The Eons Python Framework provides a Python counterpart to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
+The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
 
-## Eons vs Biology
+## Kind
 
-The Eons library is designed for plug-and-play development, unlike Biology. This means it's faster to get up and running but has fewer features, is less optimized, and will likely be slower to run. Additionally, Eons is only single threaded (due to Python limitations), while Biology is multi-threaded by default. Due to the single thread limitation of this framework, the full neural-processing of Biology is reduced to only a single sequence of operations at a time. However, by allowing those operations to be arbitrarily complex, build off each other, and be loaded from the cloud at runtime, we aim to provide the same level of functionality, if not better, than what Biology provides by default. Both systems work toward a full implementation of the [Eons Language of Development](https://github.com/develop-biology/language.development).
+Eons provides an easy plug-and-play style of development by melding the myriad Python packages we all love with our own custom syntax. We aim to provide you with something that is familiar when you want it to be, and powerful when you need it to be.
 
-Once Develop Biology is stable and the Native Biology Syntax is fully developed, the Eons Python Framework and all downstream implementations will be merged into a single, flexible, and optimized solution. However, the builtin reflection features of Biology should make it such that a successful integration means no changes to downstream code. Python can stay Python, or become any other language you want. Stay tuned!
+The most condensed form of our syntax is as follows:
+
+```python
+@eons.kind(parent/base, classes)
+def ClassName(
+    member,
+    variables,
+    which = "are injected via Fetch"
+):
+    # Your code goes here.
+    this.isHow = "you reference the object / instance"
+```
+
+Here's a more complete example:
+```python
+import eons
+
+@eons.kind(eons.StandardFunctor)
+def MyFunctor(
+	external_method = eons.inject('SomeFarAwayFunctor'),
+	constructor = f"""
+# Until Execution Blocks can be created in Parameter Blocks, formatted, multiline strings are the only way to handle arbitrary logic.
+
+this.classVariable = "Whatever you want!"
+""",
+):
+	this.result.data.myResult = external_method(this.classVariable)
+
+```
+
+This language style derives from the [Eons Language of Development](https://github.com/develop-biology/language.development). The only real features missing, besides some nicer character choices (e.g. use of `{}` for Execution Blocks) are Space Autofill, and the ability to define functions, classes, and Functors in Parameter Blocks (i.e. `()`). So, for now, you're restricted to just lambdas or breaking your larger logic out into a separate Functor. 
+
+The main differences between the Kind syntax and the Eons Language of Development are:
+* The `@eons.kind` decorator is used to declare a Type Block.
+* `this` is used instead of `$` (or `self` in Python).
+* Spatial Separation is big endian, rather than how domains are named (i.e. LSB..TLD).
+* Sequences are built by `eons.Flow()`s (still under development).
+* Python STILL does not have multiline comments >:(
+* Python has both dictionaries and lists, vs just Containers in ELD
+* `def` is required to start a Parameter Block & `:` is required to start an Execution Block, both of which must always happen in that order (and be preceded by a Type Block).
+* Convenient type casting is not fully implemented in Kind.
+* Access control is not yet implemented in Kind.
 
 ## Installation
 `pip install eons`
 
 ## Usage
 
 This library is intended for consumption by other libraries and executables.
@@ -58,15 +99,15 @@
 * Managed composition through External Methods.
 * Resolve errors through dynamic resolution by functors.
 
 ### Inputs Through Configuration File and `Fetch()`
 
 Eons provides a simple means of retrieving variables from a wide array of places. When you `Fetch()` a variable, we look through:
 1. The system environment (e.g. `export some_key="some value"`)
-2. The json configuration file supplied with `--config` (or specified by `this.defualtConfigFile` per `Configure()`)
+2. The json configuration file supplied with `--config` (or specified by `this.defaultConfigFile` per `Configure()`)
 3. Arguments supplied at the command line (e.g. specifying `--some-key "some value"` makes `Fetch(some_key)` return `"some value"`)
 4. Member variables of the Executor (e.g. `this.some_key = "some value"`)
 
 The higher the number on the above list, the higher the precedence of the search location. For example, member variables will always be returned before values from the environment.
 
 Downstream implementors of the Eons library may optionally extend the `Fetch()` method to look through whatever layers are appropriate for their inputs.
 
@@ -128,17 +169,32 @@
     @method(impl="External")
     def MyExternalFunctor(): pass
 ```
 Here, we use a Functor called "MyExternalFunctor" to compose MyClass. The actual code for MyExternalFunctor is not provided here, but is instead retrieved through `GetRegistered()`, as described above. 
 
 Using this technique, we can reuse Functors within other Functors, and none of the code has to be present on the local system at runtime but can be supplied as needed.
 
+#### Kind
+
+When using Kind syntax, use `eons.inject` instead of `@method` (Python prohibits the use of decorators in Parameter Blocks).
+
+NOTE: Kind allows you to change the name of the External Method, while the decorator does not.
+
+For example:
+```python
+@eons.kind(eons.Functor)
+def MyClass(
+    WeCanChangeThisNameNow = eons.inject("MyExternalFunctor")
+):
+...
+```
+
 #### Requirements & Notes
 
-1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info.
+1. Circular dependencies are not supported. Because of this, any Functors used to compose more complex classes should be stored in sub-folders in the package or repo_store. Sub-folders will be registered before parent directories. See [Self Registration](#self-registration) for more info. **NOTE: This is now done for you automatically by the Placement system.**
 
 2. When calling an External Method, the members of the Functor are not accessible through the function (e.g. `MyClass.MyExternalFunctor.DidFunctionSucceed()` is not currently supported). To accomplish such behavior, you must currently access the External Method through the `methods` member. For example, `MyClass.methods['MyExternalFunctor'].DidFunctionSucceed()`.
 
 3. All arguments the External Method accepts are valid to provide to the function. For example, if `MyExternalFunctor` accepts `my_arg` as an argument, you can call `MyClass.MyExternalFunctor(my_arg='whatever')`.
 
 ### Error Resolution for `@recoverable` Methods
 
@@ -238,15 +294,15 @@
 
 ### Self Registration
 
 Normally, one has to `import` the files they create into their "main" file in order to use them. That does not apply when using Eons. Instead, you simply have to derive from an appropriate base class and then call `SelfRegistering.RegisterAllClassesInDirectory(...)` (which is usually done for you based on the `repo.store` and `defaultRepoDirectory` members), providing the directory of the file as the only argument. This will essentially `import` all files in that directory and make them instantiable via `SelfRegistering("ClassName")`.
 
 Dynamic error resolutions enables this self registration system to work with inheritance as well. This means that, within downloaded functor, you can `from some_module_to_download import my_desired_class` to download another.
 
-NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organzie inheritance dependencies, but can be disabled with `recurse=False`.
+NOTE: `SelfRegistering.RegisterAllClassesInDirectory(...)` is depth-first, meaning any sub-folders in the given folder will be loaded before the parent directory. This helps to organize inheritance dependencies, but can be disabled with `recurse=False`.
 
 #### Example
 
 In some `MyDatum.py` in a `MyData` directory, you might have:
 ```
 import logging
 from Eons import Datum
```

### Comparing `eons-2.6.6/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.7/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.6/setup.cfg` & `eons-2.6.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.6
+version = 2.6.7
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
+	eot
 	pyyaml
 	requests_futures
-	requests
-	eot
-	tqdm
 	jsonpickle
+	tqdm
+	requests
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

