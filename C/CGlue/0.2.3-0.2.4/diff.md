# Comparing `tmp/CGlue-0.2.3.tar.gz` & `tmp/CGlue-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CGlue-0.2.3.tar", last modified: Wed Jun 28 20:35:16 2023, max compression
+gzip compressed data, was "CGlue-0.2.4.tar", last modified: Mon Jul 17 09:15:00 2023, max compression
```

## Comparing `CGlue-0.2.3.tar` & `CGlue-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 20:35:16.596394 CGlue-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-06-28 20:35:16.569413 CGlue-0.2.3/CGlue.egg-info/
--rw-rw-rw-   0        0        0     7548 2023-06-28 20:35:16.000000 CGlue-0.2.3/CGlue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-28 20:35:16.000000 CGlue-0.2.3/CGlue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 20:35:16.000000 CGlue-0.2.3/CGlue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-28 20:35:16.000000 CGlue-0.2.3/CGlue.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-06-28 20:35:16.000000 CGlue-0.2.3/CGlue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1076 2023-06-28 13:45:00.000000 CGlue-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     7548 2023-06-28 20:35:16.596394 CGlue-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6995 2023-06-28 17:43:20.000000 CGlue-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 20:35:16.578463 CGlue-0.2.3/cglue/
--rw-rw-rw-   0        0        0        0 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/__init__.py
--rw-rw-rw-   0        0        0    17592 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/cglue.py
--rw-rw-rw-   0        0        0     7379 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/cli.py
--rw-rw-rw-   0        0        0     4498 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/component.py
--rw-rw-rw-   0        0        0    10074 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/data_types.py
--rw-rw-rw-   0        0        0     6340 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/function.py
-drwxrwxrwx   0        0        0        0 2023-06-28 20:35:16.586878 CGlue-0.2.3/cglue/plugins/
--rw-rw-rw-   0        0        0    20930 2023-06-28 20:23:58.000000 CGlue-0.2.3/cglue/plugins/AsyncServerCalls.py
--rw-rw-rw-   0        0        0    45688 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/BuiltinDataTypes.py
--rw-rw-rw-   0        0        0     2363 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/Locks.py
--rw-rw-rw-   0        0        0     4202 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/ProjectConfigCompactor.py
--rw-rw-rw-   0        0        0    15076 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/RuntimeEvents.py
--rw-rw-rw-   0        0        0     3914 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/UserCodePlugin.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/plugins/__init__.py
--rw-rw-rw-   0        0        0     2977 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/ports.py
--rw-rw-rw-   0        0        0     3650 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-28 20:35:16.591880 CGlue-0.2.3/cglue/utils/
--rw-rw-rw-   0        0        0        0 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/__init__.py
--rw-rw-rw-   0        0        0     3259 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/common.py
--rw-rw-rw-   0        0        0      889 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/dict_processor.py
--rw-rw-rw-   0        0        0     3425 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/filesystem.py
--rw-rw-rw-   0        0        0      750 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/multiple_instance_helpers.py
--rw-rw-rw-   0        0        0     7594 2023-06-28 13:45:00.000000 CGlue-0.2.3/cglue/utils/version.py
--rw-rw-rw-   0        0        0      339 2023-06-28 20:34:23.000000 CGlue-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 20:35:16.597393 CGlue-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-06-28 20:29:56.000000 CGlue-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.837357 CGlue-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.833357 CGlue-0.2.4/CGlue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-17 09:15:00.000000 CGlue-0.2.4/CGlue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 09:15:00.000000 CGlue-0.2.4/CGlue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:15:00.000000 CGlue-0.2.4/CGlue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 09:15:00.000000 CGlue-0.2.4/CGlue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 09:15:00.000000 CGlue-0.2.4/CGlue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-17 09:14:44.000000 CGlue-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-17 09:15:00.833357 CGlue-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-07-17 09:14:44.000000 CGlue-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.833357 CGlue-0.2.4/cglue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/cglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.833357 CGlue-0.2.4/cglue/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/AsyncServerCalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45688 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/BuiltinDataTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/Locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/ProjectConfigCompactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/RuntimeEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/UserCodePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/ports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.833357 CGlue-0.2.4/cglue/runtime_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/runtime_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/runtime_generator/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:15:00.833357 CGlue-0.2.4/cglue/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/dict_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/multiple_instance_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-17 09:14:44.000000 CGlue-0.2.4/cglue/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 09:14:44.000000 CGlue-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:15:00.837357 CGlue-0.2.4/setup.cfg
```

### Comparing `CGlue-0.2.3/CGlue.egg-info/PKG-INFO` & `CGlue-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,247 +1,235 @@
-Metadata-Version: 2.1
-Name: CGlue
-Version: 0.2.3
-Summary: Framework for C software
-Home-page: https://github.com/RevolutionRobotics/CGlue
-Author: Dániel Buga
-Author-email: Dániel Buga <bugadani@gmail.com>
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-CGlue ![Python package](https://github.com/RevolutionRobotics/CGlue/workflows/Python%20package/badge.svg) [![codecov](https://codecov.io/gh/RevolutionRobotics/CGlue/branch/master/graph/badge.svg)](https://codecov.io/gh/RevolutionRobotics/CGlue)
-=====
-
-__CGlue is in its early stages of development. It is not recommended for use in
-production software and every part can change significantly.__
-
-CGlue is a software framework for project written in C. It defines a component-based
-architecture and provides tools to support this architecture.
-
-A CGlue project has two main layers:
-
-- a component layer where you define the boundaries (ports, public types) of your software
-   components
-- and a runtime layer where you define connections between your components
-
-CGlue is capable of generating the skeleton structure of software components
-and the implementation of the runtime layer.
-
-CGlue requires python 3.x (TODO check minimum python version) and chevron.
-
-Got any issues or suggestions? Head on to the issues page and open a ticket!
-
-Running tests
--------------
-
-To set up the required packages, run the following:
-
-```shell
-pip install -r requirements.txt
-pip install -r requirements_tests.txt
-```
-
-Use `python setup.py test` to run the tests.
-
-Create a new project
---------------------
-
-`cglue --new-project ProjectName [--project=project_file.json] [--cleanup]`
-
-This command will create a new CGlue project file and the default directories.
-There is no makefile added to the project - you'll need to write your own
-or use a script to generate based on the CGlue project file.
-
-Create a new software component
--------------------------------
-
-`cglue --new-component ComponentName [--cleanup]`
-
-This will create a new folder in the `SwComponents` folder (by default), create an empty source and
-header file as well as a component configuration json.
-
-Updating a software component
------------------------------
-
-After you edit a component configuration json, you may call the following command to re-generate
-the header and source files:
-
-`cglue --update-component ComponentName [--cleanup]`
-
-Alternatively, if you want to update all components, call `cglue --update-all-components [--cleanup]`
-
-CGlue managed software architecture
------------------------------------
-
-A CGlue project consists of a set of generated components, and a generated runtime that connects
-the components.
-
-__This description is incomplete and CGlue
-may implement features that are not described here__
-
-### Components
-
-Components are independent, isolated pieces of software, connected by the runtime via their ports
-and runnables. Normally, they are singletons and use
-static global memory to manage their state, but CGlue supports components with multiple instances,
-in which case the runtime passes a pointer to the instance's state memory to the generated functions.
-
-Each component has a `config.json` that describes the interface and properties of the component.
-This file contains:
-
-- the set of component dependencies
-- versioning information
-- the set of state variables if the component supports multiple instances.
-
-This file also lists the `*.c` source files
-that implement the component.
-
-#### Ports
-
-```json
-"ports": {
-   "<PortName>": {
-      "port_type": "<PortType>",
-      ... other properties specific to port type ...
-   }
-},
-```
-
-Each port has a name and a type. The current set of port types:
-
-- Constant
-- ConstantArray
-- ReadValue
-- ReadIndexedValue
-- WriteData
-- WriteIndexedData
-- Event
-- ServerCall
-- AsyncServerCall
-
-#### Runnables
-
-Runnables are special ports that always provide some logic or procedure.
-
-```json
-"runnables": {
-   "<RunnableName>": {
-      "port_type": "<PortType>",
-      "arguments": {
-         "<ArgumentName>": {
-            "data_type": "<DataType>",
-            "direction": "<Direction>"
-         }
-      },
-      "return_type": "<ReturnType>",
-   }
-   ...
-}
-```
-
-Runnable types:
-
-- Runnable (default, no need to specify): a normal function.
-  Runnables can be connected to `Event`, `ServerCall` and `AsyncServerCall` ports, or they can be
-  called by runtime callables. If an `AsyncServerCall` port calls a non-async runnable, the
-  runnable's result will be immediately available.
-- AsyncRunnable: A runnable backed by some state machine. Used to represent longer
-  procedures that don't immediately complete. The runtime will periodically poll these runnables.
-  `AsyncRunnable`s can be called by `AsyncServerCall` ports.
-
-Argument directions:
-
-- `in`
-- `out`
-- `inout`
-
-Argument and return types can be any type that is visible to the component. This includes types
-defined by the runtime and other components that are listed as a component's dependency (in the
-`requires` section).
-
-#### Example async runnable definition
-
-```json
-"runnables": {
-   "MyAsyncRunnable": {
-      "port_type": "AsyncRunnable",
-      "arguments": {
-         "double_this": {
-            "data_type": "uint8_t",
-            "direction": "in"
-         }
-      },
-      "return_type": "uint8_t",
-   }
-}
-```
-
-### Runtime
-
-The runtime is generated from a file called `project.json`. This file defines:
-
-- global types
-- the set of components in the project
-- global includes and additional source files not managed by CGlue
-- the top-level runnable functions that users have to call periodically
-- and most importantly, the connections between the components
-
-CGlue defines a number of different connections. Each connection needs two components, and a pair
-of compatible provided and consumed ports.
-
-#### Connecting ports
-
-Only compatible ports can be connected. A provider port may have multiple consumer ports, depending
-on the port type. Currently, CGlue may silently generate incorrect code for incorrect configuration.
-
-```json
-"port_connections": [
-   {
-      "provider": "<ProviderComponent>/<PortName>",
-      "consumer": "<ConsumerComponent>/<PortName1>"
-   }
-]
-```
-
-```json
-"port_connections": [
-   {
-      "provider": "<ProviderComponent>/<PortName>",
-      "consumers": [
-         "<ConsumerComponent>/<PortName1>",
-         "<ConsumerComponent2>/<PortName2>",
-      ]
-   }
-]
-```
-
-Provider ports:
-
-- WriteData - supports multiple consumers
-- WriteIndexedData - supports multiple consumers
-- Constant - supports multiple consumers
-- ConstantArray - supports multiple consumers
-- Event - supports multiple consumers
-- Runnable - does __not__ support multiple consumers
-
-Consumer ports:
-
-- Runnable - provider: Event
-- ReadValue - provider: Contant, WriteData
-- ReadIndexedValue - provider: ConstantArray, WriteIndexedData
-- ServerCall - provider: Runnable
-- AsyncServerCall - provider: Runnable, AsyncRunnable
-
-#### Queues
-
-WriteData and ReadData can be connected using FIFO queues. In this case the runtime will generate
-the queue. This may be useful when the provider runs with a faster loop time than the consumer.
-
-```json
-{
-      "provider": "<ProviderComponent>/<PortName>",
-      "consumer": "<ConsumerComponent>/<PortName1>",
-      "queue_length": 32
-},
-```
+CGlue ![Python package](https://github.com/RevolutionRobotics/CGlue/workflows/Python%20package/badge.svg) [![codecov](https://codecov.io/gh/RevolutionRobotics/CGlue/branch/master/graph/badge.svg)](https://codecov.io/gh/RevolutionRobotics/CGlue)
+=====
+
+__CGlue is in its early stages of development. It is not recommended for use in
+production software and every part can change significantly.__
+
+CGlue is a software framework for project written in C. It defines a component-based
+architecture and provides tools to support this architecture.
+
+A CGlue project has two main layers:
+
+- a component layer where you define the boundaries (ports, public types) of your software
+   components
+- and a runtime layer where you define connections between your components
+
+CGlue is capable of generating the skeleton structure of software components
+and the implementation of the runtime layer.
+
+CGlue requires python 3.x (TODO check minimum python version) and chevron.
+
+Got any issues or suggestions? Head on to the issues page and open a ticket!
+
+Running tests
+-------------
+
+To set up the required packages, run the following:
+
+```shell
+pip install -r requirements.txt
+pip install -r requirements_tests.txt
+```
+
+Use `nose2` to run the tests.
+
+Create a new project
+--------------------
+
+`cglue --new-project ProjectName [--project=project_file.json] [--cleanup]`
+
+This command will create a new CGlue project file and the default directories.
+There is no makefile added to the project - you'll need to write your own
+or use a script to generate based on the CGlue project file.
+
+Create a new software component
+-------------------------------
+
+`cglue --new-component ComponentName [--cleanup]`
+
+This will create a new folder in the `SwComponents` folder (by default), create an empty source and
+header file as well as a component configuration json.
+
+Updating a software component
+-----------------------------
+
+After you edit a component configuration json, you may call the following command to re-generate
+the header and source files:
+
+`cglue --update-component ComponentName [--cleanup]`
+
+Alternatively, if you want to update all components, call `cglue --update-all-components [--cleanup]`
+
+CGlue managed software architecture
+-----------------------------------
+
+A CGlue project consists of a set of generated components, and a generated runtime that connects
+the components.
+
+__This description is incomplete and CGlue
+may implement features that are not described here__
+
+### Components
+
+Components are independent, isolated pieces of software, connected by the runtime via their ports
+and runnables. Normally, they are singletons and use
+static global memory to manage their state, but CGlue supports components with multiple instances,
+in which case the runtime passes a pointer to the instance's state memory to the generated functions.
+
+Each component has a `config.json` that describes the interface and properties of the component.
+This file contains:
+
+- the set of component dependencies
+- versioning information
+- the set of state variables if the component supports multiple instances.
+
+This file also lists the `*.c` source files
+that implement the component.
+
+#### Ports
+
+```json
+"ports": {
+   "<PortName>": {
+      "port_type": "<PortType>",
+      ... other properties specific to port type ...
+   }
+},
+```
+
+Each port has a name and a type. The current set of port types:
+
+- Constant
+- ConstantArray
+- ReadValue
+- ReadIndexedValue
+- WriteData
+- WriteIndexedData
+- Event
+- ServerCall
+- AsyncServerCall
+
+#### Runnables
+
+Runnables are special ports that always provide some logic or procedure.
+
+```json
+"runnables": {
+   "<RunnableName>": {
+      "port_type": "<PortType>",
+      "arguments": {
+         "<ArgumentName>": {
+            "data_type": "<DataType>",
+            "direction": "<Direction>"
+         }
+      },
+      "return_type": "<ReturnType>",
+   }
+   ...
+}
+```
+
+Runnable types:
+
+- Runnable (default, no need to specify): a normal function.
+  Runnables can be connected to `Event`, `ServerCall` and `AsyncServerCall` ports, or they can be
+  called by runtime callables. If an `AsyncServerCall` port calls a non-async runnable, the
+  runnable's result will be immediately available.
+- AsyncRunnable: A runnable backed by some state machine. Used to represent longer
+  procedures that don't immediately complete. The runtime will periodically poll these runnables.
+  `AsyncRunnable`s can be called by `AsyncServerCall` ports.
+
+Argument directions:
+
+- `in`
+- `out`
+- `inout`
+
+Argument and return types can be any type that is visible to the component. This includes types
+defined by the runtime and other components that are listed as a component's dependency (in the
+`requires` section).
+
+#### Example async runnable definition
+
+```json
+"runnables": {
+   "MyAsyncRunnable": {
+      "port_type": "AsyncRunnable",
+      "arguments": {
+         "double_this": {
+            "data_type": "uint8_t",
+            "direction": "in"
+         }
+      },
+      "return_type": "uint8_t",
+   }
+}
+```
+
+### Runtime
+
+The runtime is generated from a file called `project.json`. This file defines:
+
+- global types
+- the set of components in the project
+- global includes and additional source files not managed by CGlue
+- the top-level runnable functions that users have to call periodically
+- and most importantly, the connections between the components
+
+CGlue defines a number of different connections. Each connection needs two components, and a pair
+of compatible provided and consumed ports.
+
+#### Connecting ports
+
+Only compatible ports can be connected. A provider port may have multiple consumer ports, depending
+on the port type. Currently, CGlue may silently generate incorrect code for incorrect configuration.
+
+```json
+"port_connections": [
+   {
+      "provider": "<ProviderComponent>/<PortName>",
+      "consumer": "<ConsumerComponent>/<PortName1>"
+   }
+]
+```
+
+```json
+"port_connections": [
+   {
+      "provider": "<ProviderComponent>/<PortName>",
+      "consumers": [
+         "<ConsumerComponent>/<PortName1>",
+         "<ConsumerComponent2>/<PortName2>",
+      ]
+   }
+]
+```
+
+Provider ports:
+
+- WriteData - supports multiple consumers
+- WriteIndexedData - supports multiple consumers
+- Constant - supports multiple consumers
+- ConstantArray - supports multiple consumers
+- Event - supports multiple consumers
+- Runnable - does __not__ support multiple consumers
+
+Consumer ports:
+
+- Runnable - provider: Event
+- ReadValue - provider: Contant, WriteData
+- ReadIndexedValue - provider: ConstantArray, WriteIndexedData
+- ServerCall - provider: Runnable
+- AsyncServerCall - provider: Runnable, AsyncRunnable
+
+#### Queues
+
+WriteData and ReadData can be connected using FIFO queues. In this case the runtime will generate
+the queue. This may be useful when the provider runs with a faster loop time than the consumer.
+
+```json
+{
+      "provider": "<ProviderComponent>/<PortName>",
+      "consumer": "<ConsumerComponent>/<PortName1>",
+      "queue_length": 32
+},
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `CGlue-0.2.3/CGlue.egg-info/SOURCES.txt` & `CGlue-0.2.4/CGlue.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 CGlue.egg-info/PKG-INFO
 CGlue.egg-info/SOURCES.txt
 CGlue.egg-info/dependency_links.txt
 CGlue.egg-info/entry_points.txt
 CGlue.egg-info/top_level.txt
 cglue/__init__.py
 cglue/cglue.py
@@ -18,26 +17,15 @@
 cglue/plugins/AsyncServerCalls.py
 cglue/plugins/BuiltinDataTypes.py
 cglue/plugins/Locks.py
 cglue/plugins/ProjectConfigCompactor.py
 cglue/plugins/RuntimeEvents.py
 cglue/plugins/UserCodePlugin.py
 cglue/plugins/__init__.py
-cglue/utils/__init__.py
-cglue/utils/common.py
-cglue/utils/dict_processor.py
-cglue/utils/filesystem.py
-cglue/utils/multiple_instance_helpers.py
-cglue/utils/version.py
-cglue/plugins/AsyncServerCalls.py
-cglue/plugins/BuiltinDataTypes.py
-cglue/plugins/Locks.py
-cglue/plugins/ProjectConfigCompactor.py
-cglue/plugins/RuntimeEvents.py
-cglue/plugins/UserCodePlugin.py
-cglue/plugins/__init__.py
+cglue/runtime_generator/__init__.py
+cglue/runtime_generator/context.py
 cglue/utils/__init__.py
 cglue/utils/common.py
 cglue/utils/dict_processor.py
 cglue/utils/filesystem.py
 cglue/utils/multiple_instance_helpers.py
 cglue/utils/version.py
```

### Comparing `CGlue-0.2.3/LICENSE` & `CGlue-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/cglue.py` & `CGlue-0.2.4/cglue/cglue.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 
 {{# types }}
 {{{ . }}}
 {{/ types }}
 
 #endif /* COMPONENT_TYPES_{{ guard_def }}_H_ */
 
+{{# header_decls }}
+{{{ . }}}
+
+{{/ header_decls }}
 {{# function_headers }}
 {{{ . }}};
 {{/ function_headers }}
 
 #endif /* COMPONENT_{{ guard_def }}_H_ */
 '''
 
@@ -142,20 +146,20 @@
             self._load_component_config(component_name)
 
         self.raise_event('project_config_loaded', project_config)
 
     def add_port_type(self, port_type_name, port_type):
         self._port_types[port_type_name] = port_type
 
-    def _component_dir(self, component_name):
+    def component_dir(self, component_name):
         return f'{self._basedir}/{self.settings["components_folder"]}/{component_name}'
 
     def _load_component_config(self, component_name):
         if component_name not in self._components:
-            component_config_file = f'{self._component_dir(component_name)}/config.json'
+            component_config_file = f'{self.component_dir(component_name)}/config.json'
             with open(component_config_file, "r") as file:
                 component_config = json.load(file)
             self.add_component(Component(component_name, component_config, self.types))
 
     def add_component(self, component: Component):
         if component.name not in self._components:
             self._components.add(component)
@@ -196,26 +200,27 @@
                     print(f'Failed to process dependencies of {type_obj}')
                     raise
 
     def update_component(self, component_name):
 
         self._components.check_dependencies()
 
-        component_folder = self._component_dir(component_name)
+        component_folder = self.component_dir(component_name)
         source_file = f'{component_folder}/{component_name}.c'
         header_file = f'{component_folder}/{component_name}.h'
         config_file = f'{component_folder}/config.json'
 
         component_object = self._components[component_name]
         port_short_names = (f'{component_name}/{port_name}' for port_name in component_object.config['ports'])
 
         context = {
             'runtime': self,
             'component_folder': component_folder,
             'declarations': [],
+            'header_declarations': [],
             'files': {
                 config_file: '',
                 source_file: '',
                 header_file: ''
             },
             'folders': [component_name],
             'functions': {short_name: self._ports[short_name].create_component_functions()
@@ -247,14 +252,15 @@
         typedefs = [t.render_typedef() for t in sorted_type_objects]
 
         ctx = {
             'includes': sorted(includes),
             'component_name': component_name,
             'guard_def': to_underscore(component_name).upper(),
             'variables': context['declarations'],
+            'header_decls': context['header_declarations'],
             'types': typedefs,
             'type_includes': sorted(type_includes),
             'functions': function_implementations,
             'function_headers': function_headers
         }
 
         context['files'][config_file] = self.dump_component_config(component_name)
```

### Comparing `CGlue-0.2.3/cglue/cli.py` & `CGlue-0.2.4/cglue/cli.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/component.py` & `CGlue-0.2.4/cglue/component.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/data_types.py` & `CGlue-0.2.4/cglue/data_types.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/function.py` & `CGlue-0.2.4/cglue/function.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/plugins/AsyncServerCalls.py` & `CGlue-0.2.4/cglue/plugins/AsyncServerCalls.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,16 +415,16 @@
                     missing_arguments.add(arg)
 
         return call_arguments, missing_arguments
 
     @staticmethod
     def _get_lock_impl(connection):
         if 'no_locks' not in connection.attributes or not connection.attributes['no_locks']:
-            lock = '__disable_irq();'
-            unlock = '__enable_irq();'
+            lock = 'uint32_t primask = __get_PRIMASK();\n__disable_irq();'
+            unlock = '__set_PRIMASK(primask);'
         else:
             lock = ''
             unlock = ''
         return lock, unlock
 
 
 class AsyncCallPortType(PortType):
```

### Comparing `CGlue-0.2.3/cglue/plugins/BuiltinDataTypes.py` & `CGlue-0.2.4/cglue/plugins/BuiltinDataTypes.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/plugins/Locks.py` & `CGlue-0.2.4/cglue/plugins/Locks.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             if consumer_port['async']:
                 return True
 
     return False
 
 
 def surround_with_lock(signal_impl):
-    lock_impl = '__disable_irq();'
-    unlock_impl = '__enable_irq();'
+    lock_impl = 'uint32_t primask = __get_PRIMASK();\n__disable_irq();'
+    unlock_impl = '__set_PRIMASK(primask);'
 
     if type(signal_impl) is list:
         signal_impl.insert(0, lock_impl)
         signal_impl.append(unlock_impl)
     else:
         signal_impl = f'{lock_impl}\n{signal_impl}\n{unlock_impl}'
```

### Comparing `CGlue-0.2.3/cglue/plugins/ProjectConfigCompactor.py` & `CGlue-0.2.4/cglue/plugins/ProjectConfigCompactor.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/plugins/RuntimeEvents.py` & `CGlue-0.2.4/cglue/plugins/RuntimeEvents.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/plugins/UserCodePlugin.py` & `CGlue-0.2.4/cglue/plugins/UserCodePlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         return indent(create_section(secname, sections.get(secname, '') + '\n'), indent_amt)
 
     return fill_section.sub(repl, source)
 
 
 def add_sections_to_component(owner: CGlue, component_name, context: dict):
     context['declarations'].insert(0, create_section('Declarations', ''))
+    context['header_declarations'].insert(0, create_section('Declarations', ''))
 
     for func_name, functions in context['functions'].items():
         for func_type, function in functions.items():
             name = f'{func_name[func_name.rfind("/") + 1:]}:{func_type}'  # don't need to have the component name
             add_sections_to_function(function, name)
```

### Comparing `CGlue-0.2.3/cglue/ports.py` & `CGlue-0.2.4/cglue/ports.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/signal.py` & `CGlue-0.2.4/cglue/signal.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/utils/common.py` & `CGlue-0.2.4/cglue/utils/common.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/utils/dict_processor.py` & `CGlue-0.2.4/cglue/utils/dict_processor.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/utils/filesystem.py` & `CGlue-0.2.4/cglue/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/utils/multiple_instance_helpers.py` & `CGlue-0.2.4/cglue/utils/multiple_instance_helpers.py`

 * *Files identical despite different names*

### Comparing `CGlue-0.2.3/cglue/utils/version.py` & `CGlue-0.2.4/cglue/utils/version.py`

 * *Files identical despite different names*

