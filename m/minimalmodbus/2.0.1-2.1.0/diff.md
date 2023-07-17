# Comparing `tmp/minimalmodbus-2.0.1.tar.gz` & `tmp/minimalmodbus-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimalmodbus-2.0.1.tar", last modified: Wed Aug 11 19:51:59 2021, max compression
+gzip compressed data, was "minimalmodbus-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `minimalmodbus-2.0.1.tar` & `minimalmodbus-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,40 @@
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      410 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/.gitignore
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      536 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/AUTHORS.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      369 2021-08-11 19:24:27.000000 minimalmodbus-2.0.1/CITATION.cff
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     3843 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     4965 2021-08-11 19:25:23.000000 minimalmodbus-2.0.1/HISTORY.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    10100 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/LICENSE
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      343 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/MANIFEST.in
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     2924 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/Makefile
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     4077 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/PKG-INFO
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     2322 2021-08-11 19:14:11.000000 minimalmodbus-2.0.1/README.rst
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2021-08-11 19:51:59.039386 minimalmodbus-2.0.1/docs/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     6810 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/Makefile
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    12631 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/advancedusage.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      219 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/apidummyserial.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      152 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/apiminimalmodbus.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       28 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/authors.rst
--rwxrwxr-x   0 jonas     (1000) jonas     (1000)     8814 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/conf.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       33 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/contributing.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     5311 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/debugmode.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    28281 2021-08-11 19:14:11.000000 minimalmodbus-2.0.1/docs/develop.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       28 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/history.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      745 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/index.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1304 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/installation.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      229 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/internalminimalmodbus.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      260 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/internaltestdtb4824.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      230 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/internaltestminimalmodbus.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      174 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/internaltoc.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    20088 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/modbusdetails.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       27 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/readme.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1651 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/docs/related.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     7098 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/serialcommunication.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     3786 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/troubleshooting.rst
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     7976 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/docs/usage.rst
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/minimalmodbus.egg-info/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     4077 2021-08-11 19:51:58.000000 minimalmodbus-2.0.1/minimalmodbus.egg-info/PKG-INFO
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      929 2021-08-11 19:51:59.000000 minimalmodbus-2.0.1/minimalmodbus.egg-info/SOURCES.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)        1 2021-08-11 19:51:58.000000 minimalmodbus-2.0.1/minimalmodbus.egg-info/dependency_links.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       14 2021-08-11 19:51:58.000000 minimalmodbus-2.0.1/minimalmodbus.egg-info/requires.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       14 2021-08-11 19:51:58.000000 minimalmodbus-2.0.1/minimalmodbus.egg-info/top_level.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)   137109 2021-08-11 19:24:12.000000 minimalmodbus-2.0.1/minimalmodbus.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      419 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/pyproject.toml
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       13 2021-08-10 20:47:51.000000 minimalmodbus-2.0.1/requirements.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1696 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/setup.cfg
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/stubs/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1257 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/stubs/serial.pyi
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2021-08-11 19:51:59.043387 minimalmodbus-2.0.1/tests/
--rwxrwxr-x   0 jonas     (1000) jonas     (1000)      708 2021-08-05 16:14:45.000000 minimalmodbus-2.0.1/tests/__init__.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     8940 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/tests/dummy_serial.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    12406 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/tests/test_deltaDTB4824.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)   227831 2021-08-10 20:22:44.000000 minimalmodbus-2.0.1/tests/test_minimalmodbus.py
+-rw-r--r--   0        0        0       57 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/.flake8
+-rw-r--r--   0        0        0     1508 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      410 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/.gitignore
+-rw-r--r--   0        0        0      624 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0      369 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/CITATION.cff
+-rw-r--r--   0        0        0     3843 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5569 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/HISTORY.rst
+-rw-r--r--   0        0        0    10100 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3231 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/Makefile
+-rw-r--r--   0        0        0     2324 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/README.rst
+-rw-r--r--   0        0        0     6810 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/docs/Makefile
+-rw-r--r--   0        0        0    13631 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/advancedusage.rst
+-rw-r--r--   0        0        0      219 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/apidummyserial.rst
+-rw-r--r--   0        0        0      152 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/apiminimalmodbus.rst
+-rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/authors.rst
+-rwxr-xr-x   0        0        0     3001 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/contributing.rst
+-rw-r--r--   0        0        0     5248 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/debugmode.rst
+-rw-r--r--   0        0        0    27218 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/develop.rst
+-rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/history.rst
+-rw-r--r--   0        0        0      745 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/index.rst
+-rw-r--r--   0        0        0     1312 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/installation.rst
+-rw-r--r--   0        0        0      229 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internalminimalmodbus.rst
+-rw-r--r--   0        0        0      340 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/internaltestdtb4824.rst
+-rw-r--r--   0        0        0      230 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internaltestminimalmodbus.rst
+-rw-r--r--   0        0        0      174 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internaltoc.rst
+-rw-r--r--   0        0        0    20566 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/modbusdetails.rst
+-rw-r--r--   0        0        0       27 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/readme.rst
+-rw-r--r--   0        0        0     1651 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/related.rst
+-rw-r--r--   0        0        0     7098 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/serialcommunication.rst
+-rw-r--r--   0        0        0     3786 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/troubleshooting.rst
+-rw-r--r--   0        0        0     7976 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/usage.rst
+-rw-r--r--   0        0        0   134115 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/minimalmodbus.py
+-rw-r--r--   0        0        0     2230 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1257 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/stubs/serial.pyi
+-rwxr-xr-x   0        0        0      708 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     9266 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/dummy_serial.py
+-rw-r--r--   0        0        0    13361 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/test_deltaDTB4824.py
+-rw-r--r--   0        0        0   240866 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/test_minimalmodbus.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 minimalmodbus-2.1.0/PKG-INFO
```

### Comparing `minimalmodbus-2.0.1/CONTRIBUTING.rst` & `minimalmodbus-2.1.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -110,10 +110,10 @@
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated.
-3. The pull request should work for currently supported Pyhton versions. Check
+3. The pull request should work for currently supported Python versions. Check
    Github Actions to make sure that the tests pass for all supported Python versions.
```

### Comparing `minimalmodbus-2.0.1/HISTORY.rst` & `minimalmodbus-2.1.0/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 .. :changelog:
 
 History
 =======
 
+Release 2.1.0 (2023-07-17)
+--------------------------
+New features:
+
+* Support for 64-bit integers in read_long() and write_long().
+* Allow an external serial port object to be used in the Instrument constructor.
+
+Other fixes:
+
+* Change internal data representation to Python bytes objects (from bytestrings).
+* Allow integers in write_float(). Fixes github #78.
+* Adapt style to linting tools.
+* Improve Github Action script.
+* Improve scripts for tests on the Delta DTB4824 instrument.
+* Moved the contents of setup.cfg to pyproject.toml.
+* Documentation updates, for example on building with Yocto.
+
+
 Release 2.0.1 (2021-08-11)
 --------------------------
 * Improved documentation
 * Finetuned Github Actions workflow
 
 
 Release 2.0.0 (2021-08-10)
```

### Comparing `minimalmodbus-2.0.1/LICENSE` & `minimalmodbus-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/Makefile` & `minimalmodbus-2.1.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .PHONY: clean-pyc clean-build docs clean clean-docs
 
 help:
 	@echo "devdeps - install dependencies required for development"
-	@echo "lint - check style with flake8"
+	@echo "pylint - check style with pylint"
+	@echo "flake8 - check style with flake8"
+	@echo "ruff - check style with ruff"
+	@echo "pydocstyle - check documentation with pydocstyle"
 	@echo "black - modify code style using the black tool"
+	@echo "mypy - type checking"
 	@echo " "
 	@echo "test - run tests quickly with the default Python"
 	@echo "coverage - check code coverage quickly with the default Python"
 	@echo " "
 	@echo "docs - generate Sphinx HTML documentation"
 	@echo "linkcheck - check documentation html links"
 	@echo " "
@@ -57,34 +61,42 @@
 		coverage[toml] \
 		flake8 \
 		mypy \
 		pip \
 		pycodestyle \
 		pydocstyle \
 		pylint \
+		ruff \
 		setuptools \
-		sphinx_rtd_theme \
 		sphinx \
+		sphinx_rtd_theme \
+		sphinxcontrib-programoutput \
 		twine \
 		wheel
 
-lint:
-	flake8 minimalmodbus.py || true  # Includes pycodestyle
-	@echo " "
-	@echo " "
-	pydocstyle minimalmodbus.py || true
-	@echo " "
-	@echo " "
+pylint:
 	pylint minimalmodbus.py -d C0103 -d C0302 -d C0330 -d C0413 -d R0902 -d R0911 -d R0912 -d R0913 -d R0914 -d R0915 -d W0613 -d W0703 -d W0707 || true
 
+flake8:
+	flake8 minimalmodbus.py tests/dummy_serial.py tests/test_deltaDTB4824.py tests/test_minimalmodbus.py
+
 black:
 	python3 -m black .
 
+ruff:
+	ruff check .
+
+docformatter:
+	docformatter -i --black minimalmodbus.py
+
+pydocstyle:
+	pydocstyle minimalmodbus.py
+
 mypy:
-	python3 -m mypy minimalmodbus.py tests/ --strict
+	python3 -m mypy minimalmodbus.py tests/ --strict --no-warn-unused-ignores
 
 test:
 	python3 tests/test_minimalmodbus.py
 
 coverage:
 	rm -fr htmlcov/
 	coverage3 run tests/test_minimalmodbus.py
@@ -118,14 +130,14 @@
 
 show:
 	pip3 show minimalmodbus
 
 dist: clean
 	@echo "    "
 	@echo "    "
-	python3 -m build
+	flit build
 	@echo "    "
 	@echo "    "
 	ls -l dist
 
 upload:
-	python3 -m twine upload dist/*
+	flit publish
```

### Comparing `minimalmodbus-2.0.1/PKG-INFO` & `minimalmodbus-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 Metadata-Version: 2.1
 Name: minimalmodbus
-Version: 2.0.1
+Version: 2.1.0
 Summary: Easy-to-use Modbus RTU and Modbus ASCII implementation for Python
-Home-page: https://github.com/pyhys/minimalmodbus
-Author: Jonas Berg
-License: Apache License, Version 2.0
-Project-URL: Bug Tracker, https://github.com/pyhys/minimalmodbus/issues
-Project-URL: Documentation, https://minimalmodbus.readthedocs.io
 Keywords: minimalmodbus,modbus,modbus-serial,modbus-RTU,modbus-ASCII
-Platform: UNKNOWN
+Author: Jonas Berg
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Terminals :: Serial
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
+Requires-Dist: pyserial>=3.0
+Project-URL: Changelog, https://github.com/pyhys/minimalmodbus/blob/master/HISTORY.rst
+Project-URL: Documentation, https://minimalmodbus.readthedocs.io
+Project-URL: Homepage, https://github.com/pyhys/minimalmodbus
 
 ===============================
 MinimalModbus
 ===============================
 
 .. image:: https://github.com/pyhys/minimalmodbus/actions/workflows/build.yml/badge.svg
         :target: https://github.com/pyhys/minimalmodbus/actions
@@ -90,12 +88,11 @@
 There are convenience functions to handle floats, strings and long integers
 (in different byte orders).
 
 This software supports the 'Modbus RTU' and 'Modbus ASCII' serial communication
 versions of the protocol, and is intended for use on Linux, OS X and Windows platforms.
 It is open source, and has the Apache License, Version 2.0.
 
-For Python 3.6 and later. Tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10.
+For Python 3.8 and later. Tested with Python 3.8, 3.9, 3.10, 3.11 and 3.12.
 
 This package uses semantic versioning.
 
-
```

### Comparing `minimalmodbus-2.0.1/README.rst` & `minimalmodbus-2.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 There are convenience functions to handle floats, strings and long integers
 (in different byte orders).
 
 This software supports the 'Modbus RTU' and 'Modbus ASCII' serial communication
 versions of the protocol, and is intended for use on Linux, OS X and Windows platforms.
 It is open source, and has the Apache License, Version 2.0.
 
-For Python 3.6 and later. Tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10.
+For Python 3.8 and later. Tested with Python 3.8, 3.9, 3.10, 3.11 and 3.12.
 
 This package uses semantic versioning.
```

### Comparing `minimalmodbus-2.0.1/docs/Makefile` & `minimalmodbus-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/docs/advancedusage.rst` & `minimalmodbus-2.1.0/docs/advancedusage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -306,43 +306,63 @@
 
 
 Including MinimalModbus in a Yocto build
 ----------------------------------------------------------------------------
 It is easy to include MinimalModbus in a Yocto build, which is using Bitbake. Yocto is a
 collaboration with the Open Embedded initiative.
 
-In your layer, create the file
-:file:`recipes-connectivity/minimalmodbus/python-minimalmodbus_0.5.bb`.
-
-It's content should be::
+A Yocto recipe for MinimalModbus looks something like this::
 
     SUMMARY = "Easy-to-use Modbus RTU and Modbus ASCII implementation for Python"
-    SECTION = "devel/python"
+    HOMEPAGE = "https://github.com/pyhys/minimalmodbus"
+    AUTHOR = "Jonas Berg"
     LICENSE = "Apache-2.0"
-    LIC_FILES_CHKSUM = "file://LICENCE.txt;md5=27da4ba4e954f7f4ba8d1e08a2c756c4"
 
-    DEPENDS = "python"
-    RDEPENDS_${PN} = "python-pyserial"
+    PYPI_PACKAGE = "minimalmodbus"
+    LIC_FILES_CHKSUM = "file://LICENSE;md5=27da4ba4e954f7f4ba8d1e08a2c756c4"
+    SRC_URI[md5sum] = "3fe320f7be761b6a2c3373257c431c31"
+    SRC_URI[sha256sum] = "cf873a2530be3f4b86467c3e4d47b5f69fd345d47451baca4adbf59e2ac36d00"
+
+    RDEPENDS:${PN} += "python3-core python3-pyserial"
+
+    inherit pypi setuptools3
+    # TODO Use python_flit_core instead of setuptools3 for newer Yocto releases
+
+    # Handle that there is no setup.py in the project
+    # TODO Remove this once we use python_flit_core
+    do_configure:prepend() {
+    cat > ${S}/setup.py <<-EOF
+    from setuptools import setup
+
+    setup(
+        name="${PYPI_PACKAGE}",
+        version="${PV}",
+        license="${LICENSE}",
+    )
+    EOF
+    }
 
-    PR = "r0"
+Save your recipe to a file :file:`python3-minimalmodbus_2.0.1.bb`.
 
-    SRC_URI = "${SOURCEFORGE_MIRROR}/project/minimalmodbus/${PV}/MinimalModbus-${PV}.tar.gz"
+Put the recipe file in one of your Yocto layers.
 
-    SRC_URI[md5sum] = "1b2ec44e9537e14dcb8a238ea3eda451"
-    SRC_URI[sha256sum] = "d9acf6457bc26d3c784caa5d7589303afe95e980ceff860ec2a4051038bc261e"
+If you need to create a new layer, a brief introduction is given here.
+In the :file:`build` directory, run the *bitbake-layers* command to create a new layer.
+We use the layer name ``meta-minimalmodbustutorial`` in this tutorial::
 
-    S = "${WORKDIR}/MinimalModbus-${PV}"
+    bitbake-layers create-layer ../meta-minimalmodbustutorial
 
-    inherit distutils
+Put the :file:`python3-minimalmodbus_VERSION.bb` recipe file in a subdirectory
+:file:`recipes-devtools/python` within the new layer directory.
 
-You also need to add this to your :file:`local.conf` file::
+Add the layer name to the ``BBLAYERS`` variable in the :file:`build/conf/bblayers.conf`
+file. Note that also the ``meta-openembedded/meta-python`` layer must be present.
 
-    IMAGE_INSTALL_append = " python-minimalmodbus"
+You also need to add this to your :file:`build/conf/local.conf` file::
+
+    IMAGE_INSTALL:append = " python3-minimalmodbus"
 
 When using the recipe for another version of MinimalModbus, change the version
 number in the filename. Bitbake will complain that the md5sum and sha256sum not
 are correct, but Bitbake will print out the correct values so you can change
 the recipe accordingly.
 
-
-
-
```

### Comparing `minimalmodbus-2.0.1/docs/debugmode.rst` & `minimalmodbus-2.1.0/docs/debugmode.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 Similar in interactive mode::
 
     >>> instrument.read_register(4097,1)
     MinimalModbus debug mode. Writing to instrument: '\n\x03\x10\x01\x00\x01\xd0q'
     MinimalModbus debug mode. Response from instrument: '\n\x03\x02\x07\xd0\x1e)'
     200.0
 
-The data is stored internally in this driver as byte strings (representing byte values).
-For example a byte with value 18 (dec) = 12 (hex) = 00010010 (bin) is stored in a string of length one.
-This can be created using the function ``chr(18)``, or by simply typing the
-string ``'\x12'`` (which is a string of length 1). See
+The data is stored internally in this driver as Python ``bytes`` objects.
+For example a byte with value 18 (dec) = 12 (hex) = 00010010 (bin) is stored in a
+``bytes`` object of length one.
+This can be created by typing ``b'\x12'`` (which has the length 1). See
 https://docs.python.org/3/reference/lexical_analysis.html#string-and-bytes-literals
 for details on escape sequences.
 
 For more information about hexadecimal numbers, see https://en.wikipedia.org/wiki/Hexadecimal.
 
 Note that the letter A has the hexadecimal ASCII code 41, why the string ``'\x41'`` prints ``'A'``.
 The Latin-1 encoding is used (on most installations?), and the conversion table is found on
 https://en.wikipedia.org/wiki/Latin_1.
 
-The byte strings can look pretty strange when printed, as values 0 to 31 (dec) are
+The bytes objects can look pretty strange when printed, as values 0 to 31 (dec) are
 ASCII control signs (not corresponding to any letter). For example 'vertical tab'
-and 'line feed' are among those. To make the output easier to understand, print the representation, ``repr()``. Use::
+and 'line feed' are among those. To make the output easier to understand, print
+the representation, ``repr()``. Use::
 
     print(repr(bytestringname))
 
 Registers are 16 bit wide (2 bytes), and the data is sent with the most
 significant byte (MSB) before the least significant byte (LSB). This is
 called big-endian byte order. To find the register data value, multiply the
 MSB by 256 (dec) and add the LSB.
```

### Comparing `minimalmodbus-2.0.1/docs/develop.rst` & `minimalmodbus-2.1.0/docs/develop.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Developer documentation
 =======================
 
 The details printed in debug mode (requests and responses) are very useful
 for using the included dummy_serial port for unit testing purposes.
-For examples, see the file test/test_minimalmodbus.py.
+For examples, see the file :file:`test/test_minimalmodbus.py`.
 
 
 Design considerations
 -----------------------------------------------------------------------------
 My take on the design is that is should be as simple as possible, hence the name MinimalModbus,
 but it should implement the smallest number of functions needed for it to be useful.
 The target audience for this driver simply wants to talk to Modbus clients
@@ -52,71 +52,62 @@
 :meth:`._communicate`       Handles raw bytes for communication via pySerial.
 =========================== ================================================================================
 
 Most of the logic is located in separate (easy to test) functions on module level.
 For a description of them, see :ref:`internalminimalmodbus`.
 
 
-Number conversion to and from bytestrings
------------------------------------------------
-For compability with Python 2, the data is stored internally as strings.
-As this module has dropped support for Python 2, it will be converted gradually to
-use bytes in all internal data storage instead.
-
+Number conversion to and from bytes
+------------------------------------
 The Python module :mod:`struct` is used for conversion. See https://docs.python.org/3/library/struct.html
 
 Several wrapper functions are defined for easy use of the conversion.
 These functions also do argument validity checking.
 
 =========================== =================================== ================================
-Data type                   To bytestring                       From bytestring
+Data type                   To bytes                            From bytes
 =========================== =================================== ================================
-(internal usage)            :meth:`._num_to_onebyte_string`     ``ord()``
-Bit                         :meth:`._bit_to_bytestring`         Same as for bits
-Several bits                :meth:`._bits_to_bytestring`        :meth:`._bytestring_to_bits`
-Integer (char, short)       :meth:`._num_to_twobyte_string`     :meth:`._twobyte_string_to_num`
-Several registers           :meth:`._valuelist_to_bytestring`   :meth:`._bytestring_to_valuelist`
-Long integer                :meth:`._long_to_bytestring`        :meth:`._bytestring_to_long`
-Floating point number       :meth:`._float_to_bytestring`       :meth:`._bytestring_to_float`
-String                      :meth:`._textstring_to_bytestring`  :meth:`._bytestring_to_textstring`
+(internal usage)            :meth:`._num_to_two_bytes`
+Bit                         :meth:`._bit_to_bytes`              Same as for bits
+Several bits                :meth:`._bits_to_bytes`             :meth:`._bytes_to_bits`
+Integer (char, short)       :meth:`._num_to_two_bytes`          :meth:`._two_bytes_to_num`
+Several registers           :meth:`._valuelist_to_bytes`        :meth:`._bytes_to_valuelist`
+Long integer                :meth:`._long_to_bytes`             :meth:`._bytes_to_long`
+Floating point number       :meth:`._float_to_bytes`            :meth:`._bytes_to_float`
+String                      :meth:`._textstring_to_bytes`       :meth:`._bytes_to_textstring`
 =========================== =================================== ================================
 
-Note that the :mod:`struct` module produces byte buffers for Python3, but bytestrings for Python2.
-This is compensated for automatically by using the wrapper functions
-:meth:`._pack` and :meth:`._unpack`.
-
-For a description of them, see :ref:`internalminimalmodbus`.
+For compability with both Python2 and Python3, earlier versions of this module
+did store data internally as bytestrings. Now that Python2 support has been dropped,
+the internal representation of data is using Python *bytes* objects.
 
 
 Unit testing
 ------------------------------------------------------------------------------
 Unit tests are provided in the tests subfolder. To run them::
 
     make test
 
 The unittests uses previosly recorded communication data for the testing.
 
-A dummy/mock/stub for the serial port, dummy_serial, is provided for
+A dummy/mock/stub for the serial port, :mod:`dummy_serial`, is provided for
 test purposes. See :ref:`apidummyserial`.
 
 The test coverage analysis is found
 at https://codecov.io/github/pyhys/minimalmodbus?branch=master.
 
 Hardware tests are performed using a Delta DTB4824 process controller together
 with a USB-to-RS485 converter. See :ref:`testdtb4824` for more information.
 
 Run it with::
 
    python3 tests/test_deltaDTB4824.py
 
-The baudrate, portname and mode can optionally be set from command line::
-
-    python3 tests/test_deltaDTB4824.py -b19200 -D/dev/ttyUSB0 -ascii
-
-For more details on testing with this hardware, see :ref:`testdtb4824`.
+The baudrate, portname and mode can optionally be set from command line. For
+more details on testing with this hardware, see :ref:`testdtb4824`.
 
 
 Making sure that error messages are informative for the user
 ------------------------------------------------------------------------------
 To have a look on the error messages raised during unit testing of :mod:`minimalmodbus`,
 monkey-patch :data:`test_minimalmodbus.SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES` as seen here::
 
@@ -172,15 +163,15 @@
 If necessary::
 
     reload(test_minimalmodbus.minimalmodbus)
 
 
 Recording communication data for unittesting
 -------------------------------------------------------------------------
-With the known data output from an instrument, we can finetune the inner details
+With the known data output from an instrument, we can fine tune the inner details
 of the driver (code refactoring) without worrying that we change the output from the code.
 This data will be the 'golden standard' to which we test the code.
 Use as many as possible of the commands, and paste all the output in a text document.
 From this it is pretty easy to reshuffle it into unittest code.
 
 Here is an example how to record communication data, which then is pasted
 into the test code (for use with a mock/dummy serial port). See for example
@@ -343,15 +334,15 @@
     MinimalModbus debug mode. Writing to instrument: '\x01\x03\x00\x05\x00\x01\x94\x0b'
     MinimalModbus debug mode. Response from instrument: '\x01\x03\x02\x00º9÷'
     18.6
 
 It is possible to use :meth:`_perform_command` directly. You can use any Modbus function code (1-127),
 but you need to generate the payload yourself. Note that the same data is sent::
 
-    >>> instr._perform_command(3, '\x00\x05\x00\x01')
+    >>> instr._perform_command(3, b'\x00\x05\x00\x01')
     MinimalModbus debug mode. Writing to instrument: '\x01\x03\x00\x05\x00\x01\x94\x0b'
     MinimalModbus debug mode. Response from instrument: '\x01\x03\x02\x00º9÷'
     '\x02\x00º'
 
 Use this if you are to implement other Modbus function codes, as it takes care of CRC generation etc.
 
 
@@ -361,21 +352,21 @@
 the :mod:`minimalmodbus` module.
 The module level helper functions can be used without any hardware connected.
 See :ref:`internalminimalmodbus`. These can be handy when developing your
 own Modbus instrument hardware.
 
 For example::
 
-    >>> minimalmodbus._calculate_crc_string('\x01\x03\x00\x05\x00\x01')
-    '\x94\x0b'
+    >>> minimalmodbus._calculate_crc(b'\x01\x03\x00\x05\x00\x01')
+    b'\x94\x0b'
 
-And to embed the payload ``'\x10\x11\x12'`` to slave address 1, with functioncode 16::
+And to embed the payload ``b'\x10\x11\x12'`` to slave address 1, with functioncode 16::
 
-    >>> minimalmodbus._embed_payload(1, MODE_RTU, 16, '\x10\x11\x12')
-    '\x01\x10\x10\x11\x12\x90\x98'
+    >>> minimalmodbus._embed_payload(1, MODE_RTU, 16, b'\x10\x11\x12')
+    b'\x01\x10\x10\x11\x12\x90\x98'
 
 Playing with two's complement::
 
     >>> minimalmodbus._twos_complement(-1, bits=8)
     255
 
 Calculating the minimum silent interval (seconds) at a baudrate of 19200 bits/s::
@@ -397,16 +388,14 @@
     make linkcheck
 
 
 Webpage
 ------------------------------------------------------------------------------
 The HTML theme used is the Sphinx 'sphinx_rtd_theme' theme.
 
-Note that Sphinx version 1.3 or later is required to build the documentation.
-
 
 Codecov.io
 ------------------------------------------------------------------------------
 Log in to https://codecov.io/ using your Github account.
 
 Enable the webhook from GitHub to Codecov.io.
 
@@ -438,29 +427,30 @@
 Change version number etc
 `````````````````````````
 * Manually change the ``__version__`` field in the :file:`minimalmodbus.py` source file.
 * Manually change the release date in :file:`HISTORY.rst`
 * Manually change the date and version in the :file:`CITATION.cff`
 
 (Note that the version number in the Sphinx configuration file :file:`doc/conf.py`
-and in the file :file:`setup.cfg` are changed automatically.
+and in the file :file:`pyproject.toml` are changed automatically.
 Also the copyright year in :file:`doc/conf.py` is changed automatically).
 
 How to number releases are described in :pep:`440`.
 
 Code style checking etc
 ```````````````````````
 
 Automatically modify the formatting of the code::
 
     make black
 
 Check the code::
 
-    make lint
+    make pylint
+    make flake8
 
 Check typing::
 
     make mypy
 
 
 Unittesting
@@ -472,15 +462,15 @@
 Show test coverage report::
 
     make coverage
 
 
 Also make tests using Delta DTB4824 hardware. See :ref:`testdtb4824`.
 
-Test the source distribution generation (look in the :file:`PKG-INFO` file)::
+Test the source distribution generation (look in the resulting :file:`PKG-INFO` file)::
 
     make dist
 
 Also make sure that these are functional (see sections below):
 
   * Documentation generation
   * Test coverage report generation
@@ -518,56 +508,45 @@
 
 Force documentation rebuild on readthedocs
 ``````````````````````````````````````````
 Log in to https://readthedocs.org (using Github credentials) and force rebuild on
 the master branch.
 
 Enable the "master" and "stable" documentation versions. In the advanced settings
-select Python3, and enter the name of the dependency file (a
-``requirements.txt`` file must be available in the repo).
+select Python3.
 
 
 Test the installers
 ```````````````````
 Make sure that the installer works, and the dependencies are handled correctly.
 Try at least Linux and Windows.
 
 On windows you might need to use::
 
     py -m pip install minimalmodbus
 
 
 Test on hardware
 ````````````````
-Test the package on hardware from Linux and Windows. Download the file ``test_deltaDTB4824.py``.
+Test the package on hardware slave via Linux, Windows and Mac OS.
+Download the file ``test_deltaDTB4824.py``.
 
 To run the hardware test on Windows::
 
-    C:\Python27>python.exe C:\Users\jonas\Documents\Pythonprogram\testmodbus\test_deltaDTB4824.py -DCOM7 -b2400 -ascii
+    C:\Python27>python.exe C:\Users\jonas\Documents\Pythonprogram\testmodbus\test_deltaDTB4824.py -d COM7 -b 2400 -a
 
 For python3 you might need to use the ``py`` command.
 
 
 Begin a new development version
 ```````````````````````````````
 Check in a new version on GitHub master branch.
 If the previous release was ``X.Y.Z``, then use ``X.Y.(Z+1)a1``.
 
 
-Backup
-``````
-Burn a CD/DVD with these items:
-
-* Source tree
-* Source distributions
-* Windows installer
-* Generated HTML files
-
-
-
 
 Useful development tools
 ------------------------------------------------------------------------------
 Each of these have some additional information below on this page.
 
 Git
    Version control software. See https://git-scm.com/
@@ -751,23 +730,12 @@
 
 
 TODO
 ----
 
 See also GitHub issues: https://github.com/pyhys/minimalmodbus/issues
 
-* Change internal representation to bytes:
-
-  * Continue with CRC and LRC generation
-  * ``_communicate()``
-  * Better printout of the bytearray in error messages
-  * ``_extract_payload()`` and ``_embed_payload()``
-  * ``_create_payload()``, ``_parse_payload()`` and all related functions
-
-* Logging instead of _print_out()
-* Use flake8, pylint coverage etc on Github Actions
 * Possibly use pytest instead
-* Reduce number of linter deviations (see Makefile)
 * Improve installation troubleshooting
 * Test virtual serial port on Windows using com0com
 * Unittests for measuring the sleep time in ``_communicate()``.
 * Tool for interpretation of Modbus messages
```

### Comparing `minimalmodbus-2.0.1/docs/index.rst` & `minimalmodbus-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/docs/installation.rst` & `minimalmodbus-2.1.0/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 or possibly::
 
     sudo pip3 install -U minimalmodbus
 
 
 Dependencies
 ------------
-Python versions 3.6 and higher are supported. This module is pure Python.
+Python versions 3.8 and higher are supported. This module is pure Python.
 
 This module relies on `pySerial <https://github.com/pyserial/pyserial>`_ (also pure Python)
 to do the heavy lifting, and it is the only dependency. It is BSD-3-Clause licensed.
 You can find it at the Python package index: https://pypi.org/project/pyserial
 The version of pyserial should be 3.0 or later.
 
 .. note:: Since MinimalModbus 1.0 you need to use pySerial version at least 3.0
@@ -32,9 +32,9 @@
 To install a manually downloaded file use the pip tool::
 
     python3 -m pip install filename.tar.gz
 
 
 If everything else fails
 -------------------------
-You can download the raw minimalmodbus.py file from GitHub, and put it in the
+You can download the raw :file:`minimalmodbus.py` file from GitHub, and put it in the
 same directory as your other code. Note that you must have pySerial installed.
```

### Comparing `minimalmodbus-2.0.1/docs/modbusdetails.rst` & `minimalmodbus-2.1.0/docs/modbusdetails.rst`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 **Long integers ('Unsigned INT32' or 'INT32')**
     These require 32 bits, and are implemented as two consecutive 16-bit registers.
     The range is 0 to 4294967295, which is called 'unsigned INT32'. Alternatively
     negative values can be stored if the instrument is defined that way, and is
     then called 'INT32' which has the range -2147483648 to 2147483647. Unfortunately
     the byte order might differ between manufacturers of Modbus instruments.
 
+**Long long integers ('Unsigned INT64' or 'INT64')**
+    These require 64 bits, and are implemented as four consecutive 16-bit registers.
+    The range is 0 to 18446744073709551615, which is called 'unsigned INT64'.
+    Alternatively negative values can be stored if the instrument is defined that way,
+    and is then called 'INT64' which has the range -9223372036854775808
+    to 9223372036854775807. Unfortunately the byte order might differ between
+    manufacturers of Modbus instruments.
+
 **Floats (single or double precision)**
     Single precision floating point values (binary32) are defined by 32 bits (4 bytes),
     and are implemented as two consecutive 16-bit registers.
     Correspondingly, double precision floating point values (binary64) use
     64 bits (8 bytes) and are implemented as four consecutive 16-bit registers.
     How to convert from the bit values to the floating point value is described in
     the standard IEEE 754, as seen in https://en.wikipedia.org/wiki/Floating_point.
@@ -113,38 +121,40 @@
 
 Implemented functions
 ---------------------
 These are the functions to use for reading and writing registers and bits of your instrument. Study the
 documentation of your instrument to find which Modbus function code to use. The function codes (F code) are
 given in decimal in this table.
 
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| Data type in slave                    | Read                    | F code        | Write                    | F code        |
-+=======================================+=========================+===============+==========================+===============+
-| | **Bit**                             | :meth:`.read_bit`       | 2 [or 1]      | :meth:`.write_bit`       | 5 [or 15]     |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **Bits**                            | :meth:`.read_bits`      | 2 [or 1]      | :meth:`.write_bits`      | 15            |
-| | Simultaneous reading                |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **Register**                        | :meth:`.read_register`  | 3 [or 4]      | :meth:`.write_register`  | 16 [or 6]     |
-| | Integer, possibly scaled            |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **Long integer**                    | :meth:`.read_long`      | 3 [or 4]      | :meth:`.write_long`      | 16            |
-| | (32 bits = 2 registers)             |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **Float**                           | :meth:`.read_float`     | 3 [or 4]      | :meth:`.write_float`     | 16            |
-| | (32 or 64 bits =                    |                         |               |                          |               |
-| | 2 or 4 registers)                   |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **String**                          | :meth:`.read_string`    | 3 [or 4]      | :meth:`.write_string`    | 16            |
-| | 2 characters per register           |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
-| | **Registers**                       | :meth:`.read_registers` | 3 [or 4]      | :meth:`.write_registers` | 16            |
-| | Integers                            |                         |               |                          |               |
-+---------------------------------------+-------------------------+---------------+--------------------------+---------------+
+
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+| Data type in slave                  | Read                     | F code    | Write                     | F code     |
++=====================================+==========================+===========+===========================+============+
+| **Bit**                             | :meth:`.read_bit`        | 2 [or 1]  | :meth:`.write_bit`        | 5 [or 15]  |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **Bits**                           || :meth:`.read_bits`      || 2 [or 1] || :meth:`.write_bits`      || 15        |
+|| Simultaneous access                ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **Register**                       || :meth:`.read_register`  || 3 [or 4] || :meth:`.write_register`  || 16 [or 6] |
+|| Integer, possibly scaled           ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **Long integer**                   || :meth:`.read_long`      || 3 [or 4] || :meth:`.write_long`      || 16        |
+|| (32 or 64 bits =                   ||                         ||          ||                          ||           |
+|| 2 or 4 registers)                  ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **Float**                          || :meth:`.read_float`     || 3 [or 4] || :meth:`.write_float`     || 16        |
+|| (32 or 64 bits =                   ||                         ||          ||                          ||           |
+|| 2 or 4 registers)                  ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **String**                         || :meth:`.read_string`    || 3 [or 4] || :meth:`.write_string`    || 16        |
+|| 2 characters per register          ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
+|| **Registers**                      || :meth:`.read_registers` || 3 [or 4] || :meth:`.write_registers` || 16        |
+|| Integers                           ||                         ||          ||                          ||           |
++-------------------------------------+--------------------------+-----------+---------------------------+------------+
 
 See the API for MinimalModbus: :ref:`apiminimalmodbus`.
 
 
 .. _byteorder:
 
 Byte order for data stored in serveral registers
@@ -265,22 +275,23 @@
 This driver also supports Modbus ASCII mode.
 
 Basically, a byte with value 0-255 in Modbus RTU mode will in Modbus ASCII
 mode be sent as two characters corresponding to the hex value of that byte.
 
 For example a value of 76 (dec) = 4C (hex) is sent as the byte 0x4C in Modbus
 RTU mode. This byte happens to correspond to the character 'L' in the ASCII encoding.
-Thus for Modbus RTU this is sent: ``'\x4C'``, which is a string of length 1 and will print as 'L'.
+Thus for Modbus RTU this byte is sent: ``b'\x4C'``, which could be interpreted as a
+string of length 1 and would print as 'L'.
 
 The same value will in Modbus ASCII be sent as the string '4C', which has a length of 2.
 
 The frame format is slightly different for Modbus ASCII. The request message
 is sent from the master in this format:
 
- * Start [1 character]. It is the colon (:).
+ * Start [1 character]. It is the colon ``:``.
  * Slave Address [2 characters]
  * Function code [2 characters]
  * Payload data [0 to 2*252 characters]
  * LRC [2 characters]. The LRC is a Longitudinal Redundancy Check code, for error checking of the message.
  * Stop [2 characters].
    The stop characters are carriage return (``'\r'`` = ``'\x0D'``) and line feed (``'\n'`` = ``'\x0A'``).
```

### Comparing `minimalmodbus-2.0.1/docs/related.rst` & `minimalmodbus-2.1.0/docs/related.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/docs/serialcommunication.rst` & `minimalmodbus-2.1.0/docs/serialcommunication.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 115200     115200 bit/s   8.7 us     95 us           1.75 ms (0.33 ms)
 ========== ============== ========== =============== ======================
 
 
 RS-485 introduction
 -------------------
 Several nodes (instruments) can be connected to one RS485 bus. The bus consists of two lines,
-A and B, carrying differential voltages. In both ends of the bus,
-a 120 Ohm termination resistor is connected between line A and B.
+A and B, carrying a differential voltage. In both ends of the bus is
+a 120 Ohm termination resistor connected between line A and B.
 Most often a common ground line is connected between the nodes as well.
 
 At idle, both line A and B rest at the same voltage (or almost the same voltage).
 When a logic 1 is transmitted, line A is pulled towards lower voltage and
 line B is pulled towards higher voltage.
 Note that the A/B naming is sometimes mixed up by some manufacturers.
```

### Comparing `minimalmodbus-2.0.1/docs/troubleshooting.rst` & `minimalmodbus-2.1.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/docs/usage.rst` & `minimalmodbus-2.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/minimalmodbus.py` & `minimalmodbus-2.1.0/minimalmodbus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 #
-#   Copyright 2021 Jonas Berg
+#   Copyright 2023 Jonas Berg
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-"""MinimalModbus: A Python driver for Modbus RTU/ASCII via serial port (via USB, RS485 or RS232)."""
+"""MinimalModbus: A Python driver for Modbus RTU/ASCII via serial port."""
 
 __author__ = "Jonas Berg"
 __license__ = "Apache License, Version 2.0"
 __url__ = "https://github.com/pyhys/minimalmodbus"
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 
 import sys
 
-if sys.version_info < (3, 6, 0):
+if sys.version_info < (3, 8, 0):
     raise ImportError(
         "Your Python version is too old for this version of MinimalModbus"
     )
 
 import binascii
 import enum
 import os
@@ -44,16 +44,16 @@
 _MAX_NUMBER_OF_BITS_TO_WRITE = 1968  # 0x7B0
 _MAX_NUMBER_OF_BITS_TO_READ = 2000  # 0x7D0
 _MAX_NUMBER_OF_DECIMALS = 10  # Some instrument might store 0.00000154 Ampere as 154 etc
 _MAX_BYTEORDER_VALUE = 3
 _SECONDS_TO_MILLISECONDS = 1000
 _BROADCAST_DELAY: float = 0.2  # seconds
 _BITS_PER_BYTE = 8
-_ASCII_HEADER = ":"
-_ASCII_FOOTER = "\r\n"
+_ASCII_HEADER = b":"
+_ASCII_FOOTER = b"\r\n"
 _BYTEPOSITION_FOR_ASCII_HEADER = 0  # Relative to plain response
 _BYTEPOSITION_FOR_SLAVEADDRESS = 0  # Relative to (stripped) response
 _BYTEPOSITION_FOR_FUNCTIONCODE = 1  # Relative to (stripped) response
 _BYTEPOSITION_FOR_SLAVE_ERROR_CODE = 2  # Relative to (stripped) response
 _BITNUMBER_FUNCTIONCODE_ERRORINDICATION = 7
 _SLAVEADDRESS_BROADCAST = 0
 
@@ -62,26 +62,26 @@
 _latest_read_times: Dict[str, float] = {}  # Key: port name, value: timestamp
 
 # ############### #
 # Named constants #
 # ############### #
 
 MODE_RTU: str = "rtu"
-"""Use Modbus RTU communication"""
+"""Use Modbus RTU communication."""
 MODE_ASCII: str = "ascii"
-"""Use Modbus ASCII communication"""
+"""Use Modbus ASCII communication."""
 
 BYTEORDER_BIG: int = 0
-"""Use big endian byteorder"""
+"""Use big endian byteorder."""
 BYTEORDER_LITTLE: int = 1
-"""Use little endian byteorder"""
+"""Use little endian byteorder."""
 BYTEORDER_BIG_SWAP: int = 2
-"""Use big endian byteorder, with swap"""
+"""Use big endian byteorder, with swap."""
 BYTEORDER_LITTLE_SWAP: int = 3
-"""Use litte endian byteorder, with swap"""
+"""Use litte endian byteorder, with swap."""
 
 
 @enum.unique
 class _Payloadformat(enum.Enum):
     BIT = enum.auto()
     BITS = enum.auto()
     FLOAT = enum.auto()
@@ -100,143 +100,154 @@
     """Instrument class for talking to instruments (slaves).
 
     Uses the Modbus RTU or ASCII protocols (via RS485 or RS232).
 
     Args:
         * port: The serial port name, for example ``/dev/ttyUSB0`` (Linux),
           ``/dev/tty.usbserial`` (OS X) or ``COM4`` (Windows).
-        * slaveaddress: Slave address in the range 0 to 247 (use decimal numbers,
-          not hex). Address 0 is for broadcast, and 248-255 are reserved.
+          It is also possible to pass in an already opened ``serial.Serial``
+          object (new in version 2.1).
+        * slaveaddress: Slave address in the range 0 to 247.
+          Address 0 is for broadcast, and 248-255 are reserved.
         * mode: Mode selection. Can be :data:`minimalmodbus.MODE_RTU` or
           :data:`minimalmodbus.MODE_ASCII`.
         * close_port_after_each_call: If the serial port should be closed after
           each call to the instrument.
         * debug: Set this to :const:`True` to print the communication details
-
     """
 
     def __init__(
         self,
-        port: str,
+        port: Union[str, serial.Serial],
         slaveaddress: int,
         mode: str = MODE_RTU,
         close_port_after_each_call: bool = False,
         debug: bool = False,
     ) -> None:
         """Initialize instrument and open corresponding serial port."""
         self.address = slaveaddress
-        """Slave address (int). Most often set by the constructor
-        (see the class documentation).
+        """Slave address (int). Most often set by the constructor (see the class
+        documentation).
 
-        Slave address 0 is for broadcasting to all slaves (no responses are sent).
-        It is only possible to write infomation (not read) via broadcast. A long
-        delay is added after each transmission to allow the slowest slaves
-        to digest the information.
+        Slave address 0 is for broadcasting to all slaves (no responses are sent). It is
+        only possible to write infomation (not read) via broadcast. A long delay is
+        added after each transmission to allow the slowest slaves to digest the
+        information.
 
         New in version 2.0: Support for broadcast
         """
 
         self.mode = mode
         """Slave mode (str), can be :data:`minimalmodbus.MODE_RTU` or
-        :data:`minimalmodbus.MODE_ASCII`.
-        Most often set by the constructor (see the class documentation). Defaults to RTU.
+        :data:`minimalmodbus.MODE_ASCII`. Most often set by the constructor (see the
+        class documentation). Defaults to RTU.
 
         Changing this will not affect how other instruments use the same serial port.
 
         New in version 0.6.
         """
 
         self.precalculate_read_size = True
-        """If this is :const:`False`, the serial port reads until timeout
-        instead of just reading a specific number of bytes. Defaults to :const:`True`.
+        """If this is :const:`False`, the serial port reads until timeout instead of
+        just reading a specific number of bytes. Defaults to :const:`True`.
 
         Changing this will not affect how other instruments use the same serial port.
 
         New in version 0.5.
         """
 
         self.debug = debug
-        """Set this to :const:`True` to print the communication details.
-        Defaults to :const:`False`.
+        """Set this to :const:`True` to print the communication details. Defaults to
+        :const:`False`.
 
         Most often set by the constructor (see the class documentation).
 
         Changing this will not affect how other instruments use the same serial port.
         """
 
         self.clear_buffers_before_each_transaction = True
-        """If this is :const:`True`, the serial port read and write buffers are
-        cleared before each request to the instrument, to avoid cumulative byte
-        sync errors across multiple messages. Defaults to :const:`True`.
+        """If this is :const:`True`, the serial port read and write buffers are cleared
+        before each request to the instrument, to avoid cumulative byte sync errors
+        across multiple messages. Defaults to :const:`True`.
 
         Changing this will not affect how other instruments use the same serial port.
 
         New in version 1.0.
         """
 
         self.close_port_after_each_call = close_port_after_each_call
-        """If this is :const:`True`, the serial port will be closed after each
-        call. Defaults to :const:`False`.
+        """If this is :const:`True`, the serial port will be closed after each call.
+        Defaults to :const:`False`.
 
         Changing this will not affect how other instruments use the same serial port.
 
         Most often set by the constructor (see the class documentation).
         """
 
         self.handle_local_echo = False
-        """Set to to :const:`True` if your RS-485 adaptor has local echo enabled.
-        Then the transmitted message will immeadiately appear at the receive
-        line of the RS-485 adaptor. MinimalModbus will then read and discard
-        this data, before reading the data from the slave.
-        Defaults to :const:`False`.
+        """Set to to :const:`True` if your RS-485 adaptor has local echo enabled. Then
+        the transmitted message will immeadiately appear at the receive line of the
+        RS-485 adaptor. MinimalModbus will then read and discard this data, before
+        reading the data from the slave. Defaults to :const:`False`.
 
         Changing this will not affect how other instruments use the same serial port.
 
         New in version 0.7.
         """
 
-        self.serial = None
-        """The serial port object as defined by the pySerial module. Created by the constructor.
+        self.serial: Optional[serial.Serial] = None
+        """The serial port object as defined by the pySerial module. Created by the
+        constructor.
 
         Attributes that could be changed after initialisation:
 
             - port (str):      Serial port name.
                 - Most often set by the constructor (see the class documentation).
             - baudrate (int):  Baudrate in Baud.
                 - Defaults to 19200.
-            - parity (use PARITY_xxx constants): Parity. See the pySerial module for documentation.
+            - parity (use PARITY_xxx constants): Parity. See the pySerial module.
                 - Defaults to :const:`serial.PARITY_NONE`.
             - bytesize (int):  Bytesize in bits.
                 - Defaults to 8.
-            - stopbits (use STOPBITS_xxx constants):  The number of stopbits. See pySerial docs.
+            - stopbits (use STOPBITS_xxx constants):  Number of stopbits. See pySerial.
                 - Defaults to :const:`serial.STOPBITS_ONE`.
             - timeout (float): Read timeout value in seconds.
                 - Defaults to 0.05 s.
             - write_timeout (float): Write timeout value in seconds.
                 - Defaults to 2.0 s.
         """
 
-        if port not in _serialports or not _serialports[port]:
+        if _is_serial_object(port):
+            self.serial = port  # type: ignore
+        elif isinstance(port, str) and (
+            port not in _serialports or not _serialports[port]
+        ):
             self._print_debug("Create serial port {}".format(port))
             self.serial = _serialports[port] = serial.Serial(
                 port=port,
                 baudrate=19200,
                 parity=serial.PARITY_NONE,
                 bytesize=8,
                 stopbits=1,
                 timeout=0.05,
                 write_timeout=2.0,
             )
-        else:
+        elif isinstance(port, str):
             self._print_debug("Serial port {} already exists".format(port))
             self.serial = _serialports[port]
             if (self.serial.port is None) or (not self.serial.is_open):
                 self._print_debug("Serial port {} is closed. Opening.".format(port))
                 self.serial.open()
 
+        if self.serial is None or not _is_serial_object(self.serial):
+            raise MasterReportedException("Failed to initialise serial port")
+
+        if not self.serial.is_open:
+            raise MasterReportedException("Failed to open serial port")
+
         if self.close_port_after_each_call:
             self._print_debug("Closing serial port {}".format(port))
             self.serial.close()
 
         self._latest_roundtrip_time: Optional[float] = None
 
     def __repr__(self) -> str:
@@ -276,36 +287,35 @@
 
         New in version 2.0
         """
         return self._latest_roundtrip_time
 
     def _print_debug(self, text: str) -> None:
         if self.debug:
-            _print_out("MinimalModbus debug mode. " + text)
+            print("MinimalModbus debug mode. " + text)
 
     # ################################# #
     #  Methods for talking to the slave #
     # ################################# #
 
     def read_bit(self, registeraddress: int, functioncode: int = 2) -> int:
         """Read one bit from the slave (instrument).
 
         This is for a bit that has its individual address in the instrument.
 
         Args:
-            * registeraddress: The slave register address (use decimal numbers, not hex).
+            * registeraddress: The slave register address.
             * functioncode Modbus function code. Can be 1 or 2.
 
         Returns:
             The bit value 0 or 1.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [1, 2])
         return int(
             self._generic_command(
                 functioncode,
                 registeraddress,
                 number_of_bits=1,
@@ -317,22 +327,21 @@
         self, registeraddress: int, value: int, functioncode: int = 5
     ) -> None:
         """Write one bit to the slave (instrument).
 
         This is for a bit that has its individual address in the instrument.
 
         Args:
-            * registeraddress: The slave register address (use decimal numbers, not hex).
+            * registeraddress: The slave register address.
             * value: 0 or 1, or True or False
             * functioncode: Modbus function code. Can be 5 or 15.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [5, 15])
         _check_int(value, minvalue=0, maxvalue=1, description="input value")
         self._generic_command(
             functioncode,
             registeraddress,
             value,
@@ -344,27 +353,25 @@
         self, registeraddress: int, number_of_bits: int, functioncode: int = 2
     ) -> List[int]:
         """Read multiple bits from the slave (instrument).
 
         This is for bits that have individual addresses in the instrument.
 
         Args:
-            * registeraddress: The slave register start address  (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * number_of_bits: Number of bits to read
             * functioncode: Modbus function code. Can be 1 or 2.
 
         Returns:
             A list of bit values 0 or 1. The first value in the list is for
             the bit at the given address.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [1, 2])
         _check_int(
             number_of_bits,
             minvalue=1,
             maxvalue=_MAX_NUMBER_OF_BITS_TO_READ,
             description="number of bits",
@@ -383,23 +390,21 @@
         """Write multiple bits to the slave (instrument).
 
         This is for bits that have individual addresses in the instrument.
 
         Uses Modbus functioncode 15.
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * values: List of 0 or 1, or True or False. The first
               value in the list is for the bit at the given address.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         if not isinstance(values, list):
             raise TypeError(
                 'The "values parameter" must be a list. Given: {0!r}'.format(values)
             )
         # Note: The content of the list is checked at content conversion.
         _check_int(
@@ -426,15 +431,15 @@
     ) -> Union[int, float]:
         """Read an integer from one 16-bit register in the slave, possibly scaling it.
 
         The slave register can hold integer values in the range 0 to 65535
         ("Unsigned INT16").
 
         Args:
-            * registeraddress: The slave register address (use decimal numbers, not hex).
+            * registeraddress: The slave register address.
             * number_of_decimals: The number of decimals for content conversion.
             * functioncode: Modbus function code. Can be 3 or 4.
             * signed: Whether the data should be interpreted as unsigned or signed.
 
         .. note:: The parameter number_of_decimals was named numberOfDecimals
                   before MinimalModbus 1.0
 
@@ -463,15 +468,14 @@
 
         Returns:
             The register data in numerical value (int or float).
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [3, 4])
         _check_int(
             number_of_decimals,
             minvalue=0,
             maxvalue=_MAX_NUMBER_OF_DECIMALS,
             description="number of decimals",
@@ -499,28 +503,27 @@
     ) -> None:
         """Write an integer to one 16-bit register in the slave, possibly scaling it.
 
         The slave register can hold integer values in the range 0 to
         65535 ("Unsigned INT16").
 
         Args:
-            * registeraddress: The slave register address  (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register address.
             * value (int or float): The value to store in the slave register (might be
               scaled before sending).
             * number_of_decimals: The number of decimals for content conversion.
             * functioncode: Modbus function code. Can be 6 or 16.
             * signed: Whether the data should be interpreted as unsigned or signed.
 
         .. note:: The parameter number_of_decimals was named numberOfDecimals
                   before MinimalModbus 1.0
 
-        To store for example ``value=77.0``, use ``number_of_decimals=1`` if the slave register
-        will hold it as 770 internally. This will multiply ``value`` by 10 before sending it
-        to the slave register.
+        To store for example ``value=77.0``, use ``number_of_decimals=1`` if the
+        slave register will hold it as 770 internally. This will multiply ``value`` by
+        10 before sending it to the slave register.
 
         Similarly ``number_of_decimals=2`` will multiply ``value`` by 100 before sending
         it to the slave register.
 
         As the largest number that can be written to a register is 0xFFFF = 65535,
         the ``value`` and ``number_of_decimals`` should max be 65535 when combined.
         So when using ``number_of_decimals=3`` the maximum ``value`` is 65.535.
@@ -531,15 +534,14 @@
         Use the parameter ``signed=True`` if writing to a register that can hold
         negative values. Then negative input will be automatically converted into
         upper range data (two's complement).
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [6, 16])
         _check_int(
             number_of_decimals,
             minvalue=0,
             maxvalue=_MAX_NUMBER_OF_DECIMALS,
             description="number of decimals",
@@ -559,102 +561,130 @@
 
     def read_long(
         self,
         registeraddress: int,
         functioncode: int = 3,
         signed: bool = False,
         byteorder: int = BYTEORDER_BIG,
+        number_of_registers: int = 2,
     ) -> int:
-        """Read a long integer (32 bits) from the slave.
+        """Read a long integer (32 or 64 bits) from the slave.
 
-        Long integers (32 bits = 4 bytes) are stored in two consecutive 16-bit
-        registers in the slave.
+        Long integers (32 bits = 4 bytes or 64 bits = 8 bytes) are stored in
+        two or four consecutive 16-bit registers in the slave respectively.
 
         Args:
-            * registeraddress: The slave register start address (use decimal numbers,
-              not hex).
+            * registeraddress: The slave register start address.
             * functioncode: Modbus function code. Can be 3 or 4.
             * signed: Whether the data should be interpreted as unsigned or signed.
             * byteorder: How multi-register data should be interpreted.
-              Use the BYTEORDER_xxx constants. Defaults to :data:`minimalmodbus.BYTEORDER_BIG`.
+              Use the BYTEORDER_xxx constants. Defaults to
+              :data:`minimalmodbus.BYTEORDER_BIG`.
+            * number_of_registers: The number of registers allocated for the long.
+              Can be 2 or 4. (New in version 2.1)
 
 
-        ============== ================== ================ ==========================
-        ``signed``     Data type in slave Alternative name Range
-        ============== ================== ================ ==========================
-        :const:`False` Unsigned INT32     Unsigned long    0 to 4294967295
-        :const:`True`  INT32              Long             -2147483648 to 2147483647
-        ============== ================== ================ ==========================
+        ======================= ============== =============== =====================
+        ``number_of_registers`` ``signed``     Slave data type Range
+        ======================= ============== =============== =====================
+        2                       :const:`False` Unsigned INT32  0 to 4294967295
+        2                       :const:`True`  INT32           -2147483648 to 2147483647
+        4                       :const:`False` Unsigned INT64  0 to approx 1.8E19
+        4                       :const:`True`  INT64           Approx -9.2E18 to 9.2E18
+        ======================= ============== =============== =====================
 
         Returns:
             The numerical value.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [3, 4])
         _check_bool(signed, description="signed")
+        _check_int(
+            number_of_registers,
+            minvalue=2,
+            maxvalue=4,
+            description="number of registers",
+        )
         return int(
             self._generic_command(
                 functioncode,
                 registeraddress,
-                number_of_registers=2,
+                number_of_registers=number_of_registers,
                 signed=signed,
                 byteorder=byteorder,
                 payloadformat=_Payloadformat.LONG,
             )
         )
 
     def write_long(
         self,
         registeraddress: int,
         value: int,
         signed: bool = False,
         byteorder: int = BYTEORDER_BIG,
+        number_of_registers: int = 2,
     ) -> None:
-        """Write a long integer (32 bits) to the slave.
+        """Write a long integer (32 or 64 bits) to the slave.
 
-        Long integers (32 bits = 4 bytes) are stored in two consecutive 16-bit
-        registers in the slave.
+        Long integers (32 bits = 4 bytes or 64 bits = 8 bytes) are stored in
+        two or four consecutive 16-bit registers in the slave respectively.
 
         Uses Modbus function code 16.
 
-        For discussion on number of bits, number of registers, the range
-        and on alternative names, see :meth:`.read_long`.
+        For discussion on number of bits, number of registers and the range,
+        see :meth:`.read_long`.
 
         Args:
-            * registeraddress: The slave register start address  (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * value: The value to store in the slave.
             * signed: Whether the data should be interpreted as unsigned or signed.
             * byteorder: How multi-register data should be interpreted.
-              Use the BYTEORDER_xxx constants. Defaults to :data:`minimalmodbus.BYTEORDER_BIG`.
+              Use the BYTEORDER_xxx constants. Defaults to
+              :data:`minimalmodbus.BYTEORDER_BIG`.
+            * number_of_registers: The number of registers allocated for the long.
+              Can be 2 or 4. (New in version 2.1)
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         MAX_VALUE_LONG = 4294967295  # Unsigned INT32
         MIN_VALUE_LONG = -2147483648  # INT32
+        MAX_VALUE_LONG_LONG = 18446744073709551615  # Unsigned INT64
+        MIN_VALUE_LONG_LONG = -9223372036854775808  # INT64
 
         _check_int(
-            value,
-            minvalue=MIN_VALUE_LONG,
-            maxvalue=MAX_VALUE_LONG,
-            description="input value",
+            number_of_registers,
+            minvalue=2,
+            maxvalue=4,
+            description="number of registers",
         )
+        if number_of_registers == 2:
+            _check_int(
+                value,
+                minvalue=MIN_VALUE_LONG,
+                maxvalue=MAX_VALUE_LONG,
+                description="input value",
+            )
+        elif number_of_registers == 4:
+            _check_int(
+                value,
+                minvalue=MIN_VALUE_LONG_LONG,
+                maxvalue=MAX_VALUE_LONG_LONG,
+                description="input value",
+            )
         _check_bool(signed, description="signed")
         self._generic_command(
             16,
             registeraddress,
             value,
-            number_of_registers=2,
+            number_of_registers=number_of_registers,
             signed=signed,
             byteorder=byteorder,
             payloadformat=_Payloadformat.LONG,
         )
 
     def read_float(
         self,
@@ -667,43 +697,43 @@
 
         Floats are stored in two or more consecutive 16-bit registers in the slave.
         The encoding is according to the standard IEEE 754.
 
         There are differences in the byte order used by different manufacturers.
         A floating point value of 1.0 is encoded (in single precision) as 3f800000
         (hex). In this implementation the data will be sent as ``'\x3f\x80'``
-        and ``'\x00\x00'`` to two consecutetive registers by default. Make sure to test that
-        it makes sense for your instrument. If not, change the ``byteorder`` argument.
+        and ``'\x00\x00'`` to two consecutetive registers by default. Make sure to
+        test that it makes sense for your instrument. If not, change the
+        ``byteorder`` argument.
 
         Args:
-            * registeraddress : The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress : The slave register start address.
             * functioncode: Modbus function code. Can be 3 or 4.
             * number_of_registers: The number of registers allocated for the float.
               Can be 2 or 4.
             * byteorder: How multi-register data should be interpreted.
-              Use the BYTEORDER_xxx constants. Defaults to :data:`minimalmodbus.BYTEORDER_BIG`.
+              Use the BYTEORDER_xxx constants. Defaults to
+              :data:`minimalmodbus.BYTEORDER_BIG`.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
-        ====================================== ================= =========== =================
-        Type of floating point number in slave Size              Registers   Range
-        ====================================== ================= =========== =================
-        Single precision (binary32)            32 bits (4 bytes) 2 registers 1.4E-45 to 3.4E38
-        Double precision (binary64)            64 bits (8 bytes) 4 registers 5E-324 to 1.8E308
-        ====================================== ================= =========== =================
+        =============================== ================= =========== =================
+        Type of floating point in slave Size              Registers   Range
+        =============================== ================= =========== =================
+        Single precision (binary32)     32 bits (4 bytes) 2 registers 1.4E-45 to 3.4E38
+        Double precision (binary64)     64 bits (8 bytes) 4 registers 5E-324 to 1.8E308
+        =============================== ================= =========== =================
 
         Returns:
             The numerical value.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [3, 4])
         _check_int(
             number_of_registers,
             minvalue=2,
             maxvalue=4,
             description="number of registers",
@@ -731,29 +761,28 @@
 
         Uses Modbus function code 16.
 
         For discussion on precision, number of registers and on byte order,
         see :meth:`.read_float`.
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * value (float or int): The value to store in the slave
             * number_of_registers: The number of registers allocated for the float.
               Can be 2 or 4.
             * byteorder: How multi-register data should be interpreted.
-              Use the BYTEORDER_xxx constants. Defaults to :data:`minimalmodbus.BYTEORDER_BIG`.
+              Use the BYTEORDER_xxx constants. Defaults to
+              :data:`minimalmodbus.BYTEORDER_BIG`.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_numerical(value, description="input value")
         _check_int(
             number_of_registers,
             minvalue=2,
             maxvalue=4,
             description="number of registers",
@@ -775,29 +804,27 @@
         Each 16-bit register in the slave are interpreted as two characters
         (each 1 byte = 8 bits). For example 16 consecutive registers can hold 32
         characters (32 bytes).
 
         International characters (Unicode/UTF-8) are not supported.
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * number_of_registers: The number of registers allocated for the string.
             * functioncode: Modbus function code. Can be 3 or 4.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
         Returns:
             The string.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [3, 4])
         _check_int(
             number_of_registers,
             minvalue=1,
             maxvalue=_MAX_NUMBER_OF_REGISTERS_TO_READ,
             description="number of registers for read string",
@@ -821,32 +848,30 @@
         characters (32 bytes).
 
         Uses Modbus function code 16.
 
         International characters (Unicode/UTF-8) are not supported.
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * textstring: The string to store in the slave, must be ASCII.
             * number_of_registers: The number of registers allocated for the string.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
-        If the ``textstring`` is longer than the ``2*number_of_registers``, an error is raised.
-        Shorter strings are padded with spaces.
+        If the ``textstring`` is longer than the ``2*number_of_registers``, an
+        error is raised. Shorter strings are padded with spaces.
 
         Returns:
             None
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_int(
             number_of_registers,
             minvalue=1,
             maxvalue=_MAX_NUMBER_OF_REGISTERS_TO_WRITE,
             description="number of registers for write string",
         )
@@ -870,16 +895,15 @@
     ) -> List[int]:
         """Read integers from 16-bit registers in the slave.
 
         The slave registers can hold integer values in the range 0 to
         65535 ("Unsigned INT16").
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * number_of_registers: The number of registers to read, max 125 registers.
             * functioncode: Modbus function code. Can be 3 or 4.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
         Any scaling of the register data, or converting it to negative number
@@ -888,15 +912,14 @@
         Returns:
             The register data. The first value in the list is for
             the register at the given address.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         _check_functioncode(functioncode, [3, 4])
         _check_int(
             number_of_registers,
             minvalue=1,
             maxvalue=_MAX_NUMBER_OF_REGISTERS_TO_READ,
             description="number of registers",
@@ -919,30 +942,28 @@
 
         Uses Modbus function code 16.
 
         The number of registers that will be written is defined by the length of
         the ``values`` list.
 
         Args:
-            * registeraddress: The slave register start address (use decimal
-              numbers, not hex).
+            * registeraddress: The slave register start address.
             * values: The values to store in the slave registers,
               max 123 values. The first value in the list is for the register
               at the given address.
 
         .. note:: The parameter number_of_registers was named numberOfRegisters
                   before MinimalModbus 1.0
 
         Any scaling of the register data, or converting it to negative number
         (two's complement) must be done manually.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         if not isinstance(values, list):
             raise TypeError(
                 'The "values parameter" must be a list. Given: {0!r}'.format(values)
             )
         _check_int(
             len(values),
@@ -976,15 +997,15 @@
         byteorder: int = BYTEORDER_BIG,
         payloadformat: _Payloadformat = _Payloadformat.REGISTER,
     ) -> Any:
         """Perform generic command for reading and writing registers and bits.
 
         Args:
             * functioncode: Modbus function code.
-            * registeraddress: The register address (use decimal numbers, not hex).
+            * registeraddress: The register address.
             * value (numerical or string or None or list of int): The value to store
               in the register. Depends on payloadformat.
             * number_of_decimals: The number of decimals for content conversion.
               Only for a single register.
             * number_of_registers: The number of registers to read/write.
               Only certain values allowed, depends on payloadformat.
             * number_of_bits: The number of bits to read/write.
@@ -1004,15 +1025,14 @@
             1 (int), or a list of int, or ``None``.
 
             Returns ``None`` for all write function codes.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
-
         """
         ALL_ALLOWED_FUNCTIONCODES = [1, 2, 3, 4, 5, 6, 15, 16]
         ALLOWED_FUNCTIONCODES_BROADCAST = [5, 6, 15, 16]
         ALLOWED_FUNCTIONCODES = {}
         ALLOWED_FUNCTIONCODES[_Payloadformat.BIT] = [1, 2, 5, 15]
         ALLOWED_FUNCTIONCODES[_Payloadformat.BITS] = [1, 2, 15]
         ALLOWED_FUNCTIONCODES[_Payloadformat.REGISTER] = [3, 4, 6, 16]
@@ -1050,17 +1070,16 @@
             minvalue=0,
             maxvalue=_MAX_BYTEORDER_VALUE,
             description="byteorder",
         )
 
         if not isinstance(payloadformat, _Payloadformat):
             raise TypeError(
-                "The payload format should be an enum of type _Payloadformat. Given: {!r}".format(
-                    payloadformat
-                )
+                "The payload format should be an enum of type _Payloadformat. "
+                + "Given: {!r}".format(payloadformat)
             )
 
         number_of_register_bytes = number_of_registers * _NUMBER_OF_BYTES_PER_REGISTER
 
         # Check combinations: Payload format and functioncode
         if functioncode not in ALLOWED_FUNCTIONCODES[payloadformat]:
             raise ValueError(
@@ -1085,24 +1104,24 @@
                     + "Given format: {!r}.".format(payloadformat)
                 )
 
         # Check combinations: number_of_decimals
         if number_of_decimals > 0:
             if payloadformat != _Payloadformat.REGISTER:
                 raise ValueError(
-                    'The "number_of_decimals" parameter can not be used for this payload format. '
-                    + "Given format: {0!r}.".format(payloadformat)
+                    'The "number_of_decimals" parameter can not be used for this '
+                    + "payload format. Given format: {0!r}.".format(payloadformat)
                 )
 
         # Check combinations: byteorder
         if byteorder:
             if payloadformat not in [_Payloadformat.FLOAT, _Payloadformat.LONG]:
                 raise ValueError(
-                    'The "byteorder" parameter can not be used for this payload format. '
-                    + "Given format: {0!r}.".format(payloadformat)
+                    'The "byteorder" parameter can not be used for this payload'
+                    + " format. Given format: {0!r}.".format(payloadformat)
                 )
 
         # Check combinations: number of bits
         if payloadformat == _Payloadformat.BIT:
             if number_of_bits != 1:
                 raise ValueError(
                     "For BIT payload format the number of bits should be 1. "
@@ -1146,14 +1165,26 @@
             raise ValueError(
                 "Wrong number_of_registers when writing to a "
                 + "single register. Given {0!r}.".format(number_of_registers)
             )
             # Note: For function code 16 there is checking also in the content
             # conversion functions.
 
+        # Number of registers for float and long
+        if payloadformat == _Payloadformat.FLOAT and number_of_registers not in [2, 4]:
+            raise ValueError(
+                "The number of registers for float must be 2 or 4. "
+                + "Given {0!r}".format(number_of_registers)
+            )
+        if payloadformat == _Payloadformat.LONG and number_of_registers not in [2, 4]:
+            raise ValueError(
+                "The number of registers for long must be 2 or 4. "
+                + "Given {0!r}".format(number_of_registers)
+            )
+
         # Check combinations: Value
         if functioncode in [5, 6, 15, 16] and value is None:
             raise ValueError(
                 "The input value must be given for this function code. "
                 + "Given {0!r} and {1}.".format(value, functioncode)
             )
         if functioncode in [1, 2, 3, 4] and value is not None:
@@ -1262,15 +1293,15 @@
             payloadformat,
         )
 
     # #################################### #
     # Communication implementation details #
     # #################################### #
 
-    def _perform_command(self, functioncode: int, payload_to_slave: str) -> str:
+    def _perform_command(self, functioncode: int, payload_to_slave: bytes) -> bytes:
         """Perform the command having the *functioncode*.
 
         Args:
             * functioncode: The function code for the command to be performed.
               Can for example be 'Write register' = 16.
             * payload_to_slave: Data to be transmitted to the slave (will be
               embedded in slaveaddress, CRC etc)
@@ -1282,23 +1313,22 @@
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
 
         Makes use of the :meth:`_communicate` method. The request is generated
         with the :func:`_embed_payload` function, and the parsing of the
         response is done with the :func:`_extract_payload` function.
-
         """
         DEFAULT_NUMBER_OF_BYTES_TO_READ = 1000
 
         _check_functioncode(functioncode, None)
-        _check_string(payload_to_slave, description="payload")
+        _check_bytes(payload_to_slave, description="payload")
 
         # Build request
-        request = _embed_payload(
+        request_bytes = _embed_payload(
             self.address, self.mode, functioncode, payload_to_slave
         )
 
         # Calculate number of bytes to read
         number_of_bytes_to_read = DEFAULT_NUMBER_OF_BYTES_TO_READ
         if self.address == _SLAVEADDRESS_BROADCAST:
             number_of_bytes_to_read = 0
@@ -1310,37 +1340,37 @@
             except Exception:
                 if self.debug:
                     template = (
                         "Could not precalculate response size for Modbus {} mode. "
                         + "Will read {} bytes. Request: {!r}"
                     )
                     self._print_debug(
-                        template.format(self.mode, number_of_bytes_to_read, request)
+                        template.format(
+                            self.mode, number_of_bytes_to_read, request_bytes
+                        )
                     )
 
         # Communicate
-        request_bytes = bytes(request, encoding="latin1")
         response_bytes = self._communicate(request_bytes, number_of_bytes_to_read)
-        response = str(response_bytes, encoding="latin1")
 
         if number_of_bytes_to_read == 0:
-            return ""
+            return b""
 
         # Extract payload
         payload_from_slave = _extract_payload(
-            response, self.address, self.mode, functioncode
+            response_bytes, self.address, self.mode, functioncode
         )
         return payload_from_slave
 
     def _communicate(self, request: bytes, number_of_bytes_to_read: int) -> bytes:
         """Talk to the slave via a serial port.
 
         Args:
-            request: The raw request that is to be sent to the slave.
-            number_of_bytes_to_read: Number of bytes to read
+            * request: The raw request that is to be sent to the slave.
+            * number_of_bytes_to_read: Number of bytes to read
 
         Returns:
             The raw data returned from the slave.
 
         Raises:
             TypeError, ValueError, ModbusException,
             serial.SerialException (inherited from IOError)
@@ -1350,33 +1380,34 @@
         Will block until reaching *number_of_bytes_to_read* or timeout.
 
         Additional delay will be used after broadcast transmissions (slave address 0).
 
         If the attribute :attr:`Instrument.debug` is :const:`True`, the communication
         details are printed.
 
-        If the attribute :attr:`Instrument.close_port_after_each_call` is :const:`True` the
-        serial port is closed after each call.
+        If the attribute :attr:`Instrument.close_port_after_each_call` is :const:`True`
+        the serial port is closed after each call.
 
         Timing::
 
                             Request from master (Master is writing)
                             |
-                            |                             Response from slave (Master is reading)
+                            |                             Response from slave
+                            |                             (Master is reading)
                             |                             |
-            --------R-------W-----------------------------R-------W-----------------------------
+            --------R-------W-----------------------------R-------W--------------------
                      |     |                               |
                      |     |<------- Roundtrip time ------>|
                      |     |
                   -->|-----|<----- Silent period
 
-        The resolution for Python's time.time() is lower on Windows than on Linux.
+        The resolution for Python's :py:func:`time.time()` is lower on Windows than
+        on Linux.
         It is about 16 ms on Windows according to
-        https://stackoverflow.com/questions/157359/accurate-timestamping-in-python-logging
-
+        stackoverflow.com/questions/157359/accurate-timestamping-in-python-logging
         """
         _check_bytes(request, minlength=1, description="request")
         _check_int(number_of_bytes_to_read)
 
         self._print_debug(
             "Will write to instrument (expecting {} bytes back): {}".format(
                 number_of_bytes_to_read, _describe_bytes(request)
@@ -1418,16 +1449,16 @@
                 )
                 self._print_debug(text)
 
             time.sleep(sleep_time)
 
         elif self.debug:
             template = (
-                "No sleep required before write. "
-                + "Time since previous read: {:.2f} ms, minimum silent period: {:.2f} ms."
+                "No sleep required before write. Time since "
+                + "previous read: {:.2f} ms, minimum silent period: {:.2f} ms."
             )
             text = template.format(
                 time_since_read * _SECONDS_TO_MILLISECONDS,
                 minimum_silent_period * _SECONDS_TO_MILLISECONDS,
             )
             self._print_debug(text)
 
@@ -1556,100 +1587,113 @@
     value: Union[None, str, int, float, List[int]],
     number_of_decimals: int,
     number_of_registers: int,
     number_of_bits: int,
     signed: bool,
     byteorder: int,
     payloadformat: _Payloadformat,
-) -> str:
+) -> bytes:
     """Create the payload.
 
     Error checking should have been done before calling this function.
 
-    For argument descriptions, see the _generic_command() method.
-
+    For argument descriptions, see the :py:meth:`_generic_command` method.
     """
     if functioncode in [1, 2]:
-        return _num_to_twobyte_string(registeraddress) + _num_to_twobyte_string(
-            number_of_bits
-        )
+        return _num_to_two_bytes(registeraddress) + _num_to_two_bytes(number_of_bits)
     if functioncode in [3, 4]:
-        return _num_to_twobyte_string(registeraddress) + _num_to_twobyte_string(
+        return _num_to_two_bytes(registeraddress) + _num_to_two_bytes(
             number_of_registers
         )
     if functioncode == 5:
         assert isinstance(value, int)
-        return _num_to_twobyte_string(registeraddress) + _bit_to_bytestring(value)
+        return _num_to_two_bytes(registeraddress) + _bit_to_bytes(value)
     if functioncode == 6:
         assert isinstance(value, (int, float))
-        return _num_to_twobyte_string(registeraddress) + _num_to_twobyte_string(
+        return _num_to_two_bytes(registeraddress) + _num_to_two_bytes(
             value, number_of_decimals, signed=signed
         )
     if functioncode == 15:
         if payloadformat == _Payloadformat.BIT and isinstance(value, int):
             bitlist = [value]
         elif payloadformat == _Payloadformat.BITS and isinstance(value, list):
             bitlist = value
         else:
             raise ValueError(
-                f"Wrong payloadformat {payloadformat} or type for the value for function code 15"
+                f"Wrong payloadformat {payloadformat} or type "
+                + "for the value for function code 15"
             )
-
+        number_of_bytes_for_bits = _calculate_number_of_bytes_for_bits(number_of_bits)
         return (
-            _num_to_twobyte_string(registeraddress)
-            + _num_to_twobyte_string(number_of_bits)
-            + _num_to_onebyte_string(
-                _calculate_number_of_bytes_for_bits(number_of_bits)
-            )
-            + _bits_to_bytestring(bitlist)
+            _num_to_two_bytes(registeraddress)
+            + _num_to_two_bytes(number_of_bits)
+            + number_of_bytes_for_bits.to_bytes(1, "big")
+            + _bits_to_bytes(bitlist)
         )
     if functioncode == 16:
         if payloadformat == _Payloadformat.REGISTER:
             assert isinstance(value, (int, float))
-            registerdata = _num_to_twobyte_string(
-                value, number_of_decimals, signed=signed
-            )
+            registerdata = _num_to_two_bytes(value, number_of_decimals, signed=signed)
         elif payloadformat == _Payloadformat.STRING:
             assert isinstance(value, str)
-            registerdata = _textstring_to_bytestring(value, number_of_registers)
+            registerdata = _textstring_to_bytes(value, number_of_registers)
         elif payloadformat == _Payloadformat.LONG:
             assert isinstance(value, int)
-            registerdata = _long_to_bytestring(
-                value, signed, number_of_registers, byteorder
-            )
+            registerdata = _long_to_bytes(value, signed, number_of_registers, byteorder)
         elif payloadformat == _Payloadformat.FLOAT:
-            assert isinstance(value, float)
-            registerdata = _float_to_bytestring(value, number_of_registers, byteorder)
+            assert isinstance(value, float) or isinstance(value, int)
+            registerdata = _float_to_bytes(value, number_of_registers, byteorder)
         elif payloadformat == _Payloadformat.REGISTERS:
             assert isinstance(value, list)
-            registerdata = _valuelist_to_bytestring(value, number_of_registers)
-
+            registerdata = _valuelist_to_bytes(value, number_of_registers)
+        else:
+            raise ValueError(
+                f"Wrong payloadformat '{payloadformat}' for function code 16"
+            )
         assert len(registerdata) == number_of_registers * _NUMBER_OF_BYTES_PER_REGISTER
 
+        registerdata_bytecount = len(registerdata)
         return (
-            _num_to_twobyte_string(registeraddress)
-            + _num_to_twobyte_string(number_of_registers)
-            + _num_to_onebyte_string(len(registerdata))
+            _num_to_two_bytes(registeraddress)
+            + _num_to_two_bytes(number_of_registers)
+            + registerdata_bytecount.to_bytes(1, "big")
             + registerdata
         )
     raise ValueError("Wrong function code: " + str(functioncode))
 
 
 def _parse_payload(
-    payload: str,
+    payload: bytes,
     functioncode: int,
     registeraddress: int,
     value: Any,
     number_of_decimals: int,
     number_of_registers: int,
     number_of_bits: int,
     signed: bool,
     byteorder: int,
     payloadformat: _Payloadformat,
 ) -> Union[None, str, int, float, List[int], List[float]]:
+    """Extract the payload data from a response.
+
+    Args:
+        * payload:              Payload to be parsed
+        * functioncode:         Function code
+        * registeraddress:      Register address for error checking
+        * value:                Value in request, for error checking
+        * number_of_decimals:   Number of decimals
+        * number_of_registers:  Number of registers
+        * number_of_bits:       Number of bits
+        * signed:               Signed
+        * byteorder:            Byte order
+        * payloadformat:        Payload format
+
+    Returns:
+        The parsed payload.
+    """
     _check_response_payload(
         payload,
         functioncode,
         registeraddress,
         value,
         number_of_decimals,
         number_of_registers,
@@ -1658,107 +1702,101 @@
         byteorder,
         payloadformat,
     )
 
     if functioncode in [1, 2]:
         registerdata = payload[_NUMBER_OF_BYTES_BEFORE_REGISTERDATA:]
         if payloadformat == _Payloadformat.BIT:
-            return _bytestring_to_bits(registerdata, number_of_bits)[0]
+            return _bytes_to_bits(registerdata, number_of_bits)[0]
         if payloadformat == _Payloadformat.BITS:
-            return _bytestring_to_bits(registerdata, number_of_bits)
+            return _bytes_to_bits(registerdata, number_of_bits)
 
     if functioncode in [3, 4]:
         registerdata = payload[_NUMBER_OF_BYTES_BEFORE_REGISTERDATA:]
         if payloadformat == _Payloadformat.STRING:
-            return _bytestring_to_textstring(registerdata, number_of_registers)
+            return _bytes_to_textstring(registerdata, number_of_registers)
 
         if payloadformat == _Payloadformat.LONG:
-            return _bytestring_to_long(
-                registerdata, signed, number_of_registers, byteorder
-            )
+            return _bytes_to_long(registerdata, signed, number_of_registers, byteorder)
 
         if payloadformat == _Payloadformat.FLOAT:
-            return _bytestring_to_float(registerdata, number_of_registers, byteorder)
+            return _bytes_to_float(registerdata, number_of_registers, byteorder)
 
         if payloadformat == _Payloadformat.REGISTERS:
-            return _bytestring_to_valuelist(registerdata, number_of_registers)
+            return _bytes_to_valuelist(registerdata, number_of_registers)
 
         if payloadformat == _Payloadformat.REGISTER:
-            return _twobyte_string_to_num(
-                registerdata, number_of_decimals, signed=signed
-            )
+            return _two_bytes_to_num(registerdata, number_of_decimals, signed=signed)
 
     if functioncode in [5, 6, 15, 16]:
         # Response to write
         return None
 
     raise ValueError(
-        f"Wrong function code {functioncode} and payloadformat {payloadformat!r} combination"
+        f"Wrong function code {functioncode} and payloadformat {payloadformat!r}"
+        + " combination"
     )
 
 
 def _embed_payload(
-    slaveaddress: int, mode: str, functioncode: int, payloaddata: str
-) -> str:
+    slaveaddress: int, mode: str, functioncode: int, payloaddata: bytes
+) -> bytes:
     """Build a request from the slaveaddress, the function code and the payload data.
 
     Args:
         * slaveaddress: The address of the slave.
         * mode: The modbus protcol mode (MODE_RTU or MODE_ASCII)
         * functioncode: The function code for the command to be performed.
           Can for example be 16 (Write register).
-        * payloaddata: The byte string to be sent to the slave.
+        * payloaddata: The bytes to be sent to the slave.
 
     Returns:
         The built (raw) request for sending to the slave (including CRC etc).
 
     Raises:
         ValueError, TypeError.
 
     The resulting request has the format:
-     * RTU Mode: slaveaddress byte + functioncode byte + payloaddata + CRC (which is two bytes).
-     * ASCII Mode: header (:) + slaveaddress (2 characters) + functioncode
-       (2 characters) + payloaddata + LRC (which is two characters) + footer (CRLF)
+     * RTU Mode: slaveaddress byte + functioncode byte + payloaddata + CRC (two bytes).
+     * ASCII Mode: header (``:``) + slaveaddress (2 characters) + functioncode
+       (2 characters) + payloaddata + LRC (which is two characters) + footer (CR+LF)
 
-    The LRC or CRC is calculated from the byte string made up of slaveaddress +
+    The LRC or CRC is calculated from the bytes made up of slaveaddress +
     functioncode + payloaddata.
     The header, LRC/CRC, and footer are excluded from the calculation.
-
     """
     _check_slaveaddress(slaveaddress)
     _check_mode(mode)
     _check_functioncode(functioncode, None)
-    _check_string(payloaddata, description="payload")
+    _check_bytes(payloaddata, description="payload")
 
     first_part = (
-        _num_to_onebyte_string(slaveaddress)
-        + _num_to_onebyte_string(functioncode)
-        + payloaddata
+        _num_to_one_byte(slaveaddress) + _num_to_one_byte(functioncode) + payloaddata
     )
 
     if mode == MODE_ASCII:
         request = (
             _ASCII_HEADER
             + _hexencode(first_part)
-            + _hexencode(_calculate_lrc_string(first_part))
+            + _hexencode(_calculate_lrc(first_part))
             + _ASCII_FOOTER
         )
     else:
-        request = first_part + _calculate_crc_string(first_part)
+        request = first_part + _calculate_crc(first_part)
 
     return request
 
 
 def _extract_payload(
-    response: str, slaveaddress: int, mode: str, functioncode: int
-) -> str:
+    response: bytes, slaveaddress: int, mode: str, functioncode: int
+) -> bytes:
     """Extract the payload data part from the slave's response.
 
     Args:
-        * response: The raw response byte string from the slave.
+        * response: The raw response bytes from the slave.
           This is different for RTU and ASCII.
         * slaveaddress: The adress of the slave. Used here for error checking only.
         * mode: The modbus protocol mode (MODE_RTU or MODE_ASCII)
         * functioncode: Used here for error checking only.
 
     Returns:
         The payload part of the *response*. Conversion from Modbus ASCII
@@ -1768,92 +1806,91 @@
         ValueError, TypeError, ModbusException (or subclasses).
 
     Raises an exception if there is any problem with the received address,
     the functioncode or the CRC.
 
     The received response should have the format:
 
-    * RTU Mode: slaveaddress byte + functioncode byte + payloaddata + CRC (which is two bytes)
-    * ASCII Mode: header (:) + slaveaddress byte + functioncode byte +
-      payloaddata + LRC (which is two characters) + footer (CRLF)
+    * RTU Mode: slaveaddress byte + functioncode byte + payloaddata + CRC (two bytes)
+    * ASCII Mode: header (``:``) + slaveaddress byte + functioncode byte +
+      payloaddata + LRC (which is two characters) + footer (CR+LF)
 
     For development purposes, this function can also be used to extract the payload
-    from the request sent TO the slave.
-
+    from the request sent **to** the slave.
     """
     # Number of bytes before the response payload (in stripped response)
     NUMBER_OF_RESPONSE_STARTBYTES = 2
 
     NUMBER_OF_CRC_BYTES = 2
     NUMBER_OF_LRC_BYTES = 1
     MINIMAL_RESPONSE_LENGTH_RTU = NUMBER_OF_RESPONSE_STARTBYTES + NUMBER_OF_CRC_BYTES
     MINIMAL_RESPONSE_LENGTH_ASCII = 9
 
     # Argument validity testing (ValueError/TypeError at lib programming error)
-    _check_string(response, description="response")
+    _check_bytes(response, description="response")
     _check_slaveaddress(slaveaddress)
     _check_mode(mode)
     _check_functioncode(functioncode, None)
 
     plainresponse = response
 
     # Validate response length
     if mode == MODE_ASCII:
         if len(response) < MINIMAL_RESPONSE_LENGTH_ASCII:
             raise InvalidResponseError(
-                "Too short Modbus ASCII response (minimum length {} bytes). Response: {!r}".format(
+                "Too short Modbus ASCII response (minimum "
+                + "length {} bytes). Response: {!r}".format(
                     MINIMAL_RESPONSE_LENGTH_ASCII, response
                 )
             )
     elif len(response) < MINIMAL_RESPONSE_LENGTH_RTU:
         raise InvalidResponseError(
-            "Too short Modbus RTU response (minimum length {} bytes). Response: {!r}".format(
+            "Too short Modbus RTU response (minimum "
+            + "length {} bytes). Response: {!r}".format(
                 MINIMAL_RESPONSE_LENGTH_RTU, response
             )
         )
 
     if mode == MODE_ASCII:
-
         # Validate the ASCII header and footer.
-        if response[_BYTEPOSITION_FOR_ASCII_HEADER] != _ASCII_HEADER:
+        if response[_BYTEPOSITION_FOR_ASCII_HEADER].to_bytes(1, "big") != _ASCII_HEADER:
             raise InvalidResponseError(
-                "Did not find header "
-                + "({!r}) as start of ASCII response. The plain response is: {!r}".format(
-                    _ASCII_HEADER, response
-                )
+                "Did not find header ({!r}) as start ".format(_ASCII_HEADER)
+                + "of ASCII response. The plain response is: {!r}".format(response)
             )
         if response[-len(_ASCII_FOOTER) :] != _ASCII_FOOTER:
             raise InvalidResponseError(
                 "Did not find footer "
                 + "({!r}) as end of ASCII response. The plain response is: {!r}".format(
                     _ASCII_FOOTER, response
                 )
             )
 
         # Strip ASCII header and footer
         response = response[1:-2]
 
         if len(response) % 2 != 0:
             template = (
-                "Stripped ASCII frames should have an even number of bytes, but is {} bytes. "
+                "Stripped ASCII frames should have an even "
+                + "number of bytes, but is {} bytes. "
                 + "The stripped response is: {!r} (plain response: {!r})"
             )
             raise InvalidResponseError(
                 template.format(len(response), response, plainresponse)
             )
 
         # Convert the ASCII (stripped) response string to RTU-like response string
         response = _hexdecode(response)
 
     # Validate response checksum
     if mode == MODE_ASCII:
-        calculate_checksum = _calculate_lrc_string
+        calculate_checksum = _calculate_lrc
         number_of_checksum_bytes = NUMBER_OF_LRC_BYTES
     else:
-        calculate_checksum = _calculate_crc_string
+        calculate_checksum = _calculate_crc
         number_of_checksum_bytes = NUMBER_OF_CRC_BYTES
 
     received_checksum = response[-number_of_checksum_bytes:]
     response_without_checksum = response[0 : (len(response) - number_of_checksum_bytes)]
     calculated_checksum = calculate_checksum(response_without_checksum)
 
     if received_checksum != calculated_checksum:
@@ -1863,28 +1900,29 @@
         )
         text = template.format(
             mode, received_checksum, calculated_checksum, response, plainresponse
         )
         raise InvalidResponseError(text)
 
     # Check slave address
-    responseaddress = ord(response[_BYTEPOSITION_FOR_SLAVEADDRESS])
+    responseaddress = response[_BYTEPOSITION_FOR_SLAVEADDRESS]
 
     if responseaddress != slaveaddress:
         raise InvalidResponseError(
-            "Wrong return slave address: {} instead of {}. The response is: {!r}".format(
+            "Wrong return slave "
+            + "address: {} instead of {}. The response is: {!r}".format(
                 responseaddress, slaveaddress, response
             )
         )
 
     # Check if slave indicates error
     _check_response_slaveerrorcode(response)
 
     # Check function code
-    received_functioncode = ord(response[_BYTEPOSITION_FOR_FUNCTIONCODE])
+    received_functioncode = response[_BYTEPOSITION_FOR_FUNCTIONCODE]
     if received_functioncode != functioncode:
         raise InvalidResponseError(
             "Wrong functioncode: {} instead of {}. The response is: {!r}".format(
                 received_functioncode, functioncode, response
             )
         )
 
@@ -1901,29 +1939,30 @@
 
 
 # ###################################### #
 # Serial communication utility functions #
 # ###################################### #
 
 
-def _predict_response_size(mode: str, functioncode: int, payload_to_slave: str) -> int:
+def _predict_response_size(
+    mode: str, functioncode: int, payload_to_slave: bytes
+) -> int:
     """Calculate the number of bytes that should be received from the slave.
 
     Args:
      * mode: The modbus protcol mode (MODE_RTU or MODE_ASCII)
      * functioncode: Modbus function code.
      * payload_to_slave: The raw request that is to be sent to the slave
-       (not hex encoded string)
+       (not hex encoded)
 
     Returns:
         The predicted number of bytes in the response.
 
     Raises:
         ValueError, TypeError.
-
     """
     MIN_PAYLOAD_LENGTH = 4  # For the functioncodes implemented here
     BYTERANGE_FOR_GIVEN_SIZE = slice(2, 4)  # Within the payload
 
     NUMBER_OF_PAYLOAD_BYTES_IN_WRITE_CONFIRMATION = 4
     NUMBER_OF_PAYLOAD_BYTES_FOR_BYTECOUNTFIELD = 1
 
@@ -1933,34 +1972,32 @@
     NUMBER_OF_RTU_RESPONSE_ENDBYTES = 2
     NUMBER_OF_ASCII_RESPONSE_STARTBYTES = 5
     NUMBER_OF_ASCII_RESPONSE_ENDBYTES = 4
 
     # Argument validity testing
     _check_mode(mode)
     _check_functioncode(functioncode, None)
-    _check_string(payload_to_slave, description="payload", minlength=MIN_PAYLOAD_LENGTH)
+    _check_bytes(payload_to_slave, description="payload", minlength=MIN_PAYLOAD_LENGTH)
 
     # Calculate payload size
     if functioncode in [5, 6, 15, 16]:
         response_payload_size = NUMBER_OF_PAYLOAD_BYTES_IN_WRITE_CONFIRMATION
 
     elif functioncode in [1, 2, 3, 4]:
-        given_size = int(
-            _twobyte_string_to_num(payload_to_slave[BYTERANGE_FOR_GIVEN_SIZE])
-        )
+        given_size = int(_two_bytes_to_num(payload_to_slave[BYTERANGE_FOR_GIVEN_SIZE]))
         if functioncode in [1, 2]:
             # Algorithm from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
             number_of_inputs = given_size
             response_payload_size = (
                 NUMBER_OF_PAYLOAD_BYTES_FOR_BYTECOUNTFIELD
                 + number_of_inputs // 8
                 + (1 if number_of_inputs % 8 else 0)
             )
 
-        elif functioncode in [3, 4]:
+        else:
             number_of_registers = given_size
             response_payload_size = (
                 NUMBER_OF_PAYLOAD_BYTES_FOR_BYTECOUNTFIELD
                 + number_of_registers * _NUMBER_OF_BYTES_PER_REGISTER
             )
 
     else:
@@ -1993,15 +2030,14 @@
         baudrate: The baudrate for the serial port
 
     Returns:
         The number of seconds that should pass between each message on the bus.
 
     Raises:
         ValueError, TypeError.
-
     """
     # Avoid division by zero
     _check_numerical(baudrate, minvalue=1, description="baudrate")
 
     BITTIMES_PER_CHARACTERTIME = 11
     MINIMUM_SILENT_CHARACTERTIMES = 3.5
     MINIMUM_SILENT_TIME_SECONDS = 0.00175  # See Modbus standard
@@ -2014,59 +2050,57 @@
 
 
 # ########################## #
 # String and num conversions #
 # ########################## #
 
 
-def _num_to_onebyte_string(inputvalue: int) -> str:
-    """Convert a numerical value to a one-byte string.
+def _num_to_one_byte(inputvalue: int) -> bytes:
+    """Convert a numerical value to one byte.
 
     Args:
         inputvalue: The value to be converted. Should be >=0 and <=255.
 
     Returns:
-        A one-byte string created by chr(inputvalue).
+        One byte representing the inputvalue.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(inputvalue, minvalue=0, maxvalue=0xFF)
 
-    return chr(inputvalue)
+    return inputvalue.to_bytes(1, "big")
 
 
-def _num_to_twobyte_string(
+def _num_to_two_bytes(
     value: Union[int, float],
     number_of_decimals: int = 0,
     lsb_first: bool = False,
     signed: bool = False,
-) -> str:
-    r"""Convert a numerical value to a two-byte string, possibly scaling it.
+) -> bytes:
+    r"""Convert a numerical value to two bytes, possibly scaling it.
 
     Args:
         * value: The numerical value to be converted.
         * number_of_decimals: Number of decimals, 0 or more, for scaling.
         * lsb_first: Whether the least significant byte should be first in
           the resulting string.
         * signed: Whether negative values should be accepted.
 
     Returns:
-        A two-byte string.
+        Two bytes representing the inputvalue.
 
     Raises:
-        TypeError, ValueError. Gives DeprecationWarning instead of ValueError
-        for some values in Python 2.6.
+        TypeError, ValueError.
 
     Use ``number_of_decimals=1`` to multiply ``value`` by 10 before sending it to
     the slave register. Similarly ``number_of_decimals=2`` will multiply ``value``
     by 100 before sending it to the slave register.
 
-    Use the parameter ``signed=True`` if making a bytestring that can hold
+    Use the parameter ``signed=True`` if making a bytes object that can hold
     negative values. Then negative input will be automatically converted into
     upper range data (two's complement).
 
     The byte order is controlled by the ``lsb_first`` parameter, as seen here:
 
     ======================= ============= ====================================
     ``lsb_first`` parameter Endianness    Description
@@ -2075,231 +2109,256 @@
     True                    Little-endian Least significant byte is sent first
     ======================= ============= ====================================
 
     For example:
         To store for example value=77.0, use ``number_of_decimals = 1`` if the
         register will hold it as 770 internally. The value 770 (dec) is 0302 (hex),
         where the most significant byte is 03 (hex) and the least significant byte
-        is 02 (hex). With ``lsb_first = False``, the most significant byte is given first
-        why the resulting string is ``\x03\x02``, which has the length 2.
-
+        is 02 (hex). With ``lsb_first = False``, the most significant byte is
+        given first why the resulting bytes are ``\x03\x02``, which has the length 2.
     """
     _check_numerical(value, description="inputvalue")
     _check_int(
         number_of_decimals,
         minvalue=0,
         maxvalue=_MAX_NUMBER_OF_DECIMALS,
         description="number of decimals",
     )
     _check_bool(lsb_first, description="lsb_first")
     _check_bool(signed, description="signed parameter")
 
-    multiplier = 10 ** number_of_decimals
+    multiplier = 10**number_of_decimals
     integer = int(float(value) * multiplier)
 
     if lsb_first:
         formatcode = "<"  # Little-endian
     else:
         formatcode = ">"  # Big-endian
     if signed:
         formatcode += "h"  # (Signed) short (2 bytes)
     else:
         formatcode += "H"  # Unsigned short (2 bytes)
 
-    outstring = _pack(formatcode, integer)
-    assert len(outstring) == 2
-    return outstring
+    outbytes = _pack_bytes(formatcode, integer)
+    assert len(outbytes) == 2
+    return outbytes
 
 
-def _twobyte_string_to_num(
-    bytestring: str, number_of_decimals: int = 0, signed: bool = False
+def _two_bytes_to_num(
+    inputbytes: bytes, number_of_decimals: int = 0, signed: bool = False
 ) -> Union[int, float]:
-    r"""Convert a two-byte string to a numerical value, possibly scaling it.
+    r"""Convert two bytes to a numerical value, possibly scaling it.
 
     Args:
-        * bytestring: A string of length 2.
+        * inputbytes: Bytes of length 2.
         * number_of_decimals: The number of decimals. Defaults to 0.
         * signed: Whether large positive values should be interpreted as
           negative values.
 
     Returns:
-        The numerical value (int or float) calculated from the ``bytestring``.
+        The numerical value (int or float) calculated from the ``inputbytes``.
 
     Raises:
         TypeError, ValueError
 
-    Use the parameter ``signed=True`` if converting a bytestring that can hold
+    Use the parameter ``signed=True`` if converting bytes that can hold
     negative values. Then upper range data will be automatically converted into
     negative return values (two's complement).
 
     Use ``number_of_decimals=1`` to divide the received data by 10 before returning
     the value. Similarly ``number_of_decimals=2`` will divide the received data by
     100 before returning the value.
 
     The byte order is big-endian, meaning that the most significant byte is sent first.
 
     For example:
-        A string ``\x03\x02`` (which has the length 2) corresponds to 0302 (hex) =
-        770 (dec). If ``number_of_decimals = 1``, then this is converted to 77.0 (float).
-
+        The bytes ``\x03\x02`` (which has the length 2) corresponds to 0302 (hex) =
+        770 (dec). If ``number_of_decimals = 1``, then this is converted
+        to 77.0 (float).
     """
-    _check_string(bytestring, minlength=2, maxlength=2, description="bytestring")
+    _check_bytes(inputbytes, minlength=2, maxlength=2, description="inputbytes")
     _check_int(
         number_of_decimals,
         minvalue=0,
         maxvalue=_MAX_NUMBER_OF_DECIMALS,
         description="number of decimals",
     )
     _check_bool(signed, description="signed parameter")
 
     formatcode = ">"  # Big-endian
     if signed:
         formatcode += "h"  # (Signed) short (2 bytes)
     else:
         formatcode += "H"  # Unsigned short (2 bytes)
 
-    fullregister: int = _unpack(formatcode, bytestring)
+    fullregister: int = _unpack_bytes(formatcode, inputbytes)
 
     if number_of_decimals == 0:
         return fullregister
-    divisor = 10 ** number_of_decimals
+    divisor = 10**number_of_decimals
     return fullregister / float(divisor)
 
 
-def _long_to_bytestring(
+def _long_to_bytes(
     value: int,
     signed: bool = False,
     number_of_registers: int = 2,
     byteorder: int = BYTEORDER_BIG,
-) -> str:
-    """Convert a long integer to a bytestring.
+) -> bytes:
+    """Convert a long integer to bytes.
 
-    Long integers (32 bits = 4 bytes) are stored in two consecutive 16-bit registers
-    in the slave.
+    Long integers (32 bits = 4 bytes or 64 bite = 8 bytes) are stored in two
+    or four consecutive 16-bit registers in the slave respectively.
 
     Args:
         * value: The numerical value to be converted.
         * signed: Whether large positive values should be interpreted as
           negative values.
-        * number_of_registers: Should be 2. For error checking only.
+        * number_of_registers: Should be 2 or 4.
         * byteorder: How multi-register data should be interpreted.
 
     Returns:
-        A bytestring (4 bytes).
+        Four or eight bytes.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(value, description="inputvalue")
     _check_bool(signed, description="signed parameter")
     _check_int(
-        number_of_registers, minvalue=2, maxvalue=2, description="number of registers"
+        number_of_registers, minvalue=2, maxvalue=4, description="number of registers"
     )
     _check_int(
         byteorder, minvalue=0, maxvalue=_MAX_BYTEORDER_VALUE, description="byteorder"
     )
 
     if byteorder in [BYTEORDER_BIG, BYTEORDER_BIG_SWAP]:
         formatcode = ">"
     else:
         formatcode = "<"
-    if signed:
+    if number_of_registers == 2 and signed:
         formatcode += "l"  # (Signed) long (4 bytes)
-    else:
+        lengthtarget = 4
+    elif number_of_registers == 2:
         formatcode += "L"  # Unsigned long (4 bytes)
-
-    outstring = _pack(formatcode, value)
+        lengthtarget = 4
+    elif number_of_registers == 4 and signed:
+        formatcode += "q"  # (Signed) long long (8 bytes)
+        lengthtarget = 8
+    elif number_of_registers == 4:
+        formatcode += "Q"  # Unsigned long long (8 bytes)
+        lengthtarget = 8
+    else:
+        raise ValueError(
+            "Wrong number of registers! Given value is {0!r}".format(
+                number_of_registers
+            )
+        )
+    outputbytes = _pack_bytes(formatcode, value)
     if byteorder in [BYTEORDER_BIG_SWAP, BYTEORDER_LITTLE_SWAP]:
-        outstring = _swap(outstring)
+        outputbytes = _swap(outputbytes)
 
-    assert len(outstring) == 4
-    return outstring
+    assert len(outputbytes) == lengthtarget
+    return outputbytes
 
 
-def _bytestring_to_long(
-    bytestring: str,
+def _bytes_to_long(
+    inputbytes: bytes,
     signed: bool = False,
     number_of_registers: int = 2,
     byteorder: int = BYTEORDER_BIG,
 ) -> int:
-    """Convert a bytestring to a long integer.
+    """Convert bytes to a long integer.
 
-    Long integers (32 bits = 4 bytes) are stored in two consecutive 16-bit registers
-    in the slave.
+    Long integers (32 bits = 4 bytes or 64 bite = 8 bytes) are stored in two
+    or four consecutive 16-bit registers in the slave respectively.
 
     Args:
-        * bytestring: A string of length 4.
+        * inputbytes: Length 4 or 8 bytes.
         * signed: Whether large positive values should be interpreted as
           negative values.
-        * number_of_registers: Should be 2. For error checking only.
+        * number_of_registers: Should be 2 or 4.
         * byteorder: How multi-register data should be interpreted.
 
     Returns:
         The numerical value.
 
     Raises:
         ValueError, TypeError
-
     """
-    _check_string(bytestring, "byte string", minlength=4, maxlength=4)
     _check_bool(signed, description="signed parameter")
     _check_int(
-        number_of_registers, minvalue=2, maxvalue=2, description="number of registers"
+        number_of_registers, minvalue=2, maxvalue=4, description="number of registers"
     )
     _check_int(
         byteorder, minvalue=0, maxvalue=_MAX_BYTEORDER_VALUE, description="byteorder"
     )
 
     if byteorder in [BYTEORDER_BIG, BYTEORDER_BIG_SWAP]:
         formatcode = ">"
     else:
         formatcode = "<"
-    if signed:
+    if number_of_registers == 2 and signed:
         formatcode += "l"  # (Signed) long (4 bytes)
-    else:
+        lengthtarget = 4
+    elif number_of_registers == 2:
         formatcode += "L"  # Unsigned long (4 bytes)
+        lengthtarget = 4
+    elif number_of_registers == 4 and signed:
+        formatcode += "q"  # (Signed) long long (8 bytes)
+        lengthtarget = 8
+    elif number_of_registers == 4:
+        formatcode += "Q"  # Unsigned long long (8 bytes)
+        lengthtarget = 8
+    else:
+        raise ValueError(
+            "Wrong number of registers! Given value is {0!r}".format(
+                number_of_registers
+            )
+        )
+    _check_bytes(
+        inputbytes, "input bytes", minlength=lengthtarget, maxlength=lengthtarget
+    )
 
     if byteorder in [BYTEORDER_BIG_SWAP, BYTEORDER_LITTLE_SWAP]:
-        bytestring = _swap(bytestring)
+        inputbytes = _swap(inputbytes)
 
-    return int(_unpack(formatcode, bytestring))
+    return int(_unpack_bytes(formatcode, inputbytes))
 
 
-def _float_to_bytestring(
+def _float_to_bytes(
     value: Union[int, float],
     number_of_registers: int = 2,
     byteorder: int = BYTEORDER_BIG,
-) -> str:
-    r"""Convert a numerical value to a bytestring.
+) -> bytes:
+    r"""Convert a numerical value to bytes.
 
     Floats are stored in two or more consecutive 16-bit registers in the slave. The
     encoding is according to the standard IEEE 754.
 
-    ====================================== ================= =========== =================
-    Type of floating point number in slave Size              Registers   Range
-    ====================================== ================= =========== =================
-    Single precision (binary32)            32 bits (4 bytes) 2 registers 1.4E-45 to 3.4E38
-    Double precision (binary64)            64 bits (8 bytes) 4 registers 5E-324 to 1.8E308
-    ====================================== ================= =========== =================
+    =============================== ================= =========== =================
+    Type of floating point in slave Size              Registers   Range
+    =============================== ================= =========== =================
+    Single precision (binary32)     32 bits (4 bytes) 2 registers 1.4E-45 to 3.4E38
+    Double precision (binary64)     64 bits (8 bytes) 4 registers 5E-324 to 1.8E308
+    =============================== ================= =========== =================
 
     A floating  point value of 1.0 is encoded (in single precision) as 3f800000 (hex).
-    This will give a byte string ``'\x3f\x80\x00\x00'`` (big endian).
+    This will give the bytes ``'\x3f\x80\x00\x00'`` (big endian).
 
     Args:
         * value (float or int): The numerical value to be converted.
         * number_of_registers: Can be 2 or 4.
         * byteorder: How multi-register data should be interpreted.
 
     Returns:
-        A bytestring (4 or 8 bytes).
+        4 or 8 bytes.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_numerical(value, description="inputvalue")
     _check_int(
         number_of_registers, minvalue=2, maxvalue=4, description="number of registers"
     )
     _check_int(
         byteorder, minvalue=0, maxvalue=_MAX_BYTEORDER_VALUE, description="byteorder"
@@ -2318,44 +2377,43 @@
     else:
         raise ValueError(
             "Wrong number of registers! Given value is {0!r}".format(
                 number_of_registers
             )
         )
 
-    outstring = _pack(formatcode, value)
+    outputbytes = _pack_bytes(formatcode, value)
     if byteorder in [BYTEORDER_BIG_SWAP, BYTEORDER_LITTLE_SWAP]:
-        outstring = _swap(outstring)
-    assert len(outstring) == lengthtarget
-    return outstring
+        outputbytes = _swap(outputbytes)
+    assert len(outputbytes) == lengthtarget
+    return outputbytes
 
 
-def _bytestring_to_float(
-    bytestring: str, number_of_registers: int = 2, byteorder: int = BYTEORDER_BIG
+def _bytes_to_float(
+    inputbytes: bytes, number_of_registers: int = 2, byteorder: int = BYTEORDER_BIG
 ) -> float:
-    """Convert a four-byte string to a float.
+    """Convert four bytes to a float.
 
     Floats are stored in two or more consecutive 16-bit registers in the slave.
 
-    For discussion on precision, number of bits, number of registers, the range, byte order
-    and on alternative names, see :func:`minimalmodbus._float_to_bytestring`.
+    For discussion on precision, number of bits, number of registers, the range,
+    byte order and on alternative names, see :func:`minimalmodbus._float_to_bytes`.
 
     Args:
-        * bytestring: A string of length 4 or 8.
+        * inputbytes: Four or eight bytes
         * number_of_registers: Can be 2 or 4.
         * byteorder: How multi-register data should be interpreted.
 
     Returns:
         A float.
 
     Raises:
         TypeError, ValueError
-
     """
-    _check_string(bytestring, minlength=4, maxlength=8, description="bytestring")
+    _check_bytes(inputbytes, minlength=4, maxlength=8, description="input bytes")
     _check_int(
         number_of_registers, minvalue=2, maxvalue=4, description="number of registers"
     )
     _check_int(
         byteorder, minvalue=0, maxvalue=_MAX_BYTEORDER_VALUE, description="byteorder"
     )
     number_of_bytes = _NUMBER_OF_BYTES_PER_REGISTER * number_of_registers
@@ -2371,114 +2429,112 @@
     else:
         raise ValueError(
             "Wrong number of registers! Given value is {0!r}".format(
                 number_of_registers
             )
         )
 
-    if len(bytestring) != number_of_bytes:
+    if len(inputbytes) != number_of_bytes:
         raise ValueError(
-            "Wrong length of the byte string! Given value is "
+            "Wrong length of the input bytes! Given value is "
             + "{0!r}, and number_of_registers is {1!r}.".format(
-                bytestring, number_of_registers
+                inputbytes, number_of_registers
             )
         )
 
     if byteorder in [BYTEORDER_BIG_SWAP, BYTEORDER_LITTLE_SWAP]:
-        bytestring = _swap(bytestring)
-    return float(_unpack(formatcode, bytestring))
+        inputbytes = _swap(inputbytes)
+    return float(_unpack_bytes(formatcode, inputbytes))
 
 
-def _textstring_to_bytestring(inputstring: str, number_of_registers: int = 16) -> str:
-    """Convert a text string to a bytestring.
+def _textstring_to_bytes(inputstring: str, number_of_registers: int = 16) -> bytes:
+    """Convert a text string to bytes.
 
-    Each 16-bit register in the slave are interpreted as two characters (1 byte = 8 bits).
-    For example 16 consecutive registers can hold 32 characters (32 bytes).
+    Each 16-bit register in the slave are interpreted as two characters (1 byte =
+    8 bits). For example 16 consecutive registers can hold 32 characters (32 bytes).
 
     Not much of conversion is done, mostly error checking and string padding.
-    If the inputstring is shorter that the allocated space, it is padded with
+    If the *inputstring* is shorter that the allocated space, it is padded with
     spaces in the end.
 
     Args:
         * inputstring: The string to be stored in the slave.
-          Max 2*number_of_registers characters.
+          Max 2 * *number_of_registers* characters.
         * number_of_registers: The number of registers allocated for the string.
 
     Returns:
-        A bytestring (str).
+        Bytes.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(
         number_of_registers,
         minvalue=1,
         maxvalue=_MAX_NUMBER_OF_REGISTERS_TO_WRITE,
         description="number of registers",
     )
     max_characters = _NUMBER_OF_BYTES_PER_REGISTER * number_of_registers
     _check_string(inputstring, "input string", minlength=1, maxlength=max_characters)
 
-    bytestring = inputstring.ljust(max_characters)  # Pad with space
-    assert len(bytestring) == max_characters
-    return bytestring
+    padded = inputstring.ljust(max_characters)  # Pad with space
+    outputbytes = bytes(padded, encoding="ascii")
+    assert len(outputbytes) == max_characters
+    return outputbytes
 
 
-def _bytestring_to_textstring(bytestring: str, number_of_registers: int = 16) -> str:
-    """Convert a bytestring to a text string.
+def _bytes_to_textstring(inputbytes: bytes, number_of_registers: int = 16) -> str:
+    """Convert bytes to a text string.
 
-    Each 16-bit register in the slave are interpreted as two characters (1 byte = 8 bits).
-    For example 16 consecutive registers can hold 32 characters (32 bytes).
+    Each 16-bit register in the slave are interpreted as two characters (1 byte =
+    8 bits). For example 16 consecutive registers can hold 32 characters (32 bytes).
 
     Not much of conversion is done, mostly error checking.
 
     Args:
-        * bytestring (str): The string from the slave. Length = 2*number_of_registers
+        * inputbytes: The bytes from the slave. Length = 2 * *number_of_registers*
         * number_of_registers (int): The number of registers allocated for the string.
+          Should be >0.
 
     Returns:
-        A the text string (str).
+        A the text string.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(
         number_of_registers,
         minvalue=1,
         maxvalue=_MAX_NUMBER_OF_REGISTERS_TO_READ,
         description="number of registers",
     )
     max_characters = _NUMBER_OF_BYTES_PER_REGISTER * number_of_registers
-    _check_string(
-        bytestring, "byte string", minlength=max_characters, maxlength=max_characters
+    _check_bytes(
+        inputbytes, "input bytes", minlength=max_characters, maxlength=max_characters
     )
 
-    textstring = bytestring
-    return textstring
+    return inputbytes.decode(encoding="ascii")
 
 
-def _valuelist_to_bytestring(valuelist: List[int], number_of_registers: int) -> str:
-    """Convert a list of numerical values to a bytestring.
+def _valuelist_to_bytes(valuelist: List[int], number_of_registers: int) -> bytes:
+    """Convert a list of numerical values to bytes.
 
     Each element is 'unsigned INT16'.
 
     Args:
         * valuelist: The input list. The elements should be in the
           range 0 to 65535.
         * number_of_registers: The number of registers. For error checking.
-          Should equal the number of elements in valuelist.
+          Should equal the number of elements in *valuelist*.
 
     Returns:
-        A bytestring. Length = 2*number_of_registers
+        Bytes Length = 2 * *number_of_registers*
 
     Raises:
         TypeError, ValueError
-
     """
     MINVALUE = 0
     MAXVALUE = 0xFFFF
 
     _check_int(number_of_registers, minvalue=1, description="number of registers")
 
     if not isinstance(valuelist, list):
@@ -2499,344 +2555,318 @@
         minvalue=number_of_registers,
         maxvalue=number_of_registers,
         description="length of the list",
     )
 
     number_of_bytes = _NUMBER_OF_BYTES_PER_REGISTER * number_of_registers
 
-    bytestring = ""
+    outputbytes = b""
     for value in valuelist:
-        bytestring += _num_to_twobyte_string(value, signed=False)
+        outputbytes += _num_to_two_bytes(value, signed=False)
 
-    assert len(bytestring) == number_of_bytes
-    return bytestring
+    assert len(outputbytes) == number_of_bytes
+    return outputbytes
 
 
-def _bytestring_to_valuelist(bytestring: str, number_of_registers: int) -> List[int]:
-    """Convert a bytestring to a list of numerical values.
+def _bytes_to_valuelist(inputbytes: bytes, number_of_registers: int) -> List[int]:
+    """Convert bytes to a list of numerical values.
 
-    The bytestring is interpreted as 'unsigned INT16'.
+    The bytes are interpreted as 'unsigned INT16'.
 
     Args:
-        * bytestring: The string from the slave. Length = 2*number_of_registers
+        * inputbytes: The bytes from the slave. Length = 2 * *number_of_registers*
         * number_of_registers: The number of registers. For error checking.
 
     Returns:
         A list of integers.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(number_of_registers, minvalue=1, description="number of registers")
     number_of_bytes = _NUMBER_OF_BYTES_PER_REGISTER * number_of_registers
-    _check_string(
-        bytestring, "byte string", minlength=number_of_bytes, maxlength=number_of_bytes
+    _check_bytes(
+        inputbytes, "input bytes", minlength=number_of_bytes, maxlength=number_of_bytes
     )
 
     values = []
     for i in range(number_of_registers):
         offset = _NUMBER_OF_BYTES_PER_REGISTER * i
-        substring = bytestring[offset : (offset + _NUMBER_OF_BYTES_PER_REGISTER)]
-        values.append(int(_twobyte_string_to_num(substring)))
+        sub_bytes = inputbytes[offset : (offset + _NUMBER_OF_BYTES_PER_REGISTER)]
+        values.append(int(_two_bytes_to_num(sub_bytes)))
 
     return values
 
 
-def _pack(formatstring: str, value: Any) -> str:
-    """Pack a value into a bytestring.
+def _pack_bytes(formatstring: str, value: Any) -> bytes:
+    """Pack a value into bytes.
 
-    Uses the built-in :mod:`struct` Python module.
+    Uses the built-in :mod:`struct` Python module, and adds relevant error messages.
 
     Args:
         * formatstring: String for the packing. See the :mod:`struct` module
           for details.
         * value (depends on formatstring): The value to be packed
 
     Returns:
-        A bytestring (str).
+        The packed bytes
 
     Raises:
         ValueError
-
-    Note that the :mod:`struct` module produces byte buffers for Python3,
-    but bytestrings for Python2. This is compensated for automatically.
-
     """
     _check_string(formatstring, description="formatstring", minlength=1)
 
     try:
         result = struct.pack(formatstring, value)
-    except Exception:
-        errortext = (
-            "The value to send is probably out of range, as the num-to-bytestring "
-        )
+    except Exception as exc:
+        errortext = "The value to send is probably out of range, as the num-to-bytes "
         errortext += "conversion failed. Value: {0!r} Struct format code is: {1}"
-        raise ValueError(errortext.format(value, formatstring))
+        raise ValueError(errortext.format(value, formatstring)) from exc
 
-    return str(result, encoding="latin1")
+    return result
 
 
-def _unpack(formatstring: str, packed: str) -> Any:
-    """Unpack a bytestring into a value.
+def _unpack_bytes(formatstring: str, packed_bytes: bytes) -> Any:
+    """Unpack bytes into a value.
 
-    Uses the built-in :mod:`struct` Python module.
+    Uses the built-in :mod:`struct` Python module, and adds relevant error messages.
 
     Args:
         * formatstring: String for the packing. See the :mod:`struct` module
           for details.
-        * packed: The bytestring to be unpacked.
+        * packed_bytes: The bytes to be unpacked.
 
     Returns:
         A value. The type depends on the formatstring.
 
     Raises:
         ValueError
-
-    Note that the :mod:`struct` module wants byte buffers for Python3,
-    but bytestrings for Python2. This is compensated for automatically.
-
     """
     _check_string(formatstring, description="formatstring", minlength=1)
-    _check_string(packed, description="packed string", minlength=1)
-
-    packed_bytes = bytes(packed, encoding="latin1")
+    _check_bytes(packed_bytes, description="packed bytes", minlength=1)
 
     try:
         value = struct.unpack(formatstring, packed_bytes)[0]
     except Exception:
-        errortext = (
-            "The received bytestring is probably wrong, as the bytestring-to-num "
-        )
-        errortext += "conversion failed. Bytestring: {0!r} Struct format code is: {1}"
-        raise InvalidResponseError(errortext.format(packed, formatstring))
+        errortext = "The received bytes is probably wrong, as the bytes-to-num "
+        errortext += "conversion failed. Bytes: {0!r} Struct format code is: {1}"
+        raise InvalidResponseError(errortext.format(packed_bytes, formatstring))
 
     return value
 
 
-def _swap(bytestring: str) -> str:
-    """Swap characters pairwise in a string.
+def _swap(inputbytes: bytes) -> bytes:
+    """Swap bytes pairwise.
 
     This corresponds to a "byte swap".
 
     Args:
-        * bytestring (str): input. The length should be an even number.
-
-    Return the string with characters swapped.
+        * inputbytes: input. The length should be an even number.
 
+    Return the bytes swapped.
     """
-    length = len(bytestring)
+    length = len(inputbytes)
     if length % 2:
         raise ValueError(
-            "The length of the bytestring should be even. Given {!r}.".format(
-                bytestring
+            "The length of the inputbytes should be even. Given {!r}.".format(
+                inputbytes
             )
         )
-    templist = list(bytestring)
+    templist = list(inputbytes)
     templist[1:length:2], templist[:length:2] = (
         templist[:length:2],
         templist[1:length:2],
     )
-    return "".join(templist)
+    return bytes(templist)
 
 
-def _hexencode(bytestring: str, insert_spaces: bool = False) -> str:
-    r"""Convert a byte string to a hex encoded string.
+def _hexencode(inputbytes: bytes, insert_spaces: bool = False) -> bytes:
+    r"""Convert bytes to a hex encoded bytes.
 
-    For example 'J' will return '4A', and ``'\x04'`` will return '04'.
+    For example ``b'J'`` will return ``b'4A'``, and ``b'\x04'`` will return ``b'04'``.
 
     Args:
-        * bytestring (str): Can be for example ``'A\x01B\x45'``.
-        * insert_spaces (bool): Insert space characters between pair of characters
+        * inputbytes: Can be for example ``b'A\x01B\x45'``.
+        * insert_spaces: Insert space characters between pair of characters
           to increase readability.
 
     Returns:
-        A string of twice the length, with characters in the range '0' to '9' and
-        'A' to 'F'. The string will be longer if spaces are inserted.
+        Bytes of twice the length, with characters in the range '0' to '9' and
+        'A' to 'F'. It will be longer if spaces are inserted.
 
     Raises:
         TypeError, ValueError
-
     """
-    _check_string(bytestring, description="byte string")
-
-    separator = "" if not insert_spaces else " "
-
-    # Use plain string formatting instead of binhex.hexlify,
-    # in order to have it Python 2.x and 3.x compatible
+    _check_bytes(inputbytes, description="input bytes")
 
-    byte_representions = []
-    for char in bytestring:
-        byte_representions.append("{0:02X}".format(ord(char)))
-    return separator.join(byte_representions).strip()
+    if insert_spaces:
+        return binascii.hexlify(inputbytes, sep=" ").upper()
+    return binascii.hexlify(inputbytes).upper()
 
 
-def _hexdecode(hexstring: str) -> str:
-    r"""Convert a hex encoded string to a byte string.
+def _hexdecode(hexbytes: bytes) -> bytes:
+    r"""Convert hex encoded bytes to bytes.
 
-    For example '4A' will return 'J', and '04' will return ``'\x04'`` (which has
-    length 1).
+    For example ``b'4A'`` will return ``b'J'``, and ``b'04'`` will
+    return ``b'\x04'`` (which has length 1).
 
     Args:
-        * hexstring: Can be for example 'A3' or 'A3B4'. Must be of even length.
-        * Allowed characters are '0' to '9', 'a' to 'f' and 'A' to 'F' (not space).
+        * hexbytes: Can be for example ``b'A3'`` or ``b'A3B4'``. Must be of even length.
+          Allowed bytes are ``b'0'`` to ``b'9'``, ``b'a'`` to ``b'f'``
+          and ``b'A'`` to ``b'F'`` (not space).
 
     Returns:
-        A string of half the length, with characters corresponding to all 0-255
-        values for each byte.
+        Bytes of half the length, with bytes corresponding to all 0-255 values.
 
     Raises:
         TypeError, ValueError
-
     """
-    # Note: For Python3 the appropriate would be: raise TypeError(new_error_message) from err
+    # TODO Note: For Python3 the appropriate would be:
+    #   raise TypeError(new_error_message) from err
     # but the Python2 interpreter will indicate SyntaxError.
     # Thus we need to live with this warning in Python3:
     # 'During handling of the above exception, another exception occurred'
 
-    _check_string(hexstring, description="hexstring")
+    _check_bytes(hexbytes, description="hex bytes")
 
-    if len(hexstring) % 2 != 0:
+    if len(hexbytes) % 2 != 0:
         raise ValueError(
-            "The input hexstring must be of even length. Given: {!r}".format(hexstring)
+            "The input hex bytes must be of even length. Given: {!r}".format(hexbytes)
         )
 
-    converted_bytes = bytes(hexstring, "latin1")
     try:
-        return str(binascii.unhexlify(converted_bytes), encoding="latin1")
+        return binascii.unhexlify(hexbytes)
     except binascii.Error as err:
         new_error_message = (
-            "Hexdecode reported an error: {!s}. Input hexstring: {}".format(
-                err.args[0], hexstring
+            "Hexdecode reported an error: {!s}. Input hexstring: {!r}".format(
+                err.args[0], hexbytes
             )
         )
         raise TypeError(new_error_message)
 
 
 def _describe_bytes(inputbytes: bytes) -> str:
     r"""Describe bytes in a human friendly way.
 
     Args:
         * inputbytes: Bytes to describe
 
     Returns a space separated descriptive string.
-    For example b'\x01\x02\x03' gives: 01 02 03 (3 bytes)
+    For example ``b'\x01\x02\x03'`` gives: ``01 02 03 (3 bytes)``
     """
     return " ".join([f"{x:02X}" for x in inputbytes]) + " ({} bytes)".format(
         len(inputbytes)
     )
 
 
 def _calculate_number_of_bytes_for_bits(number_of_bits: int) -> int:
     """Calculate number of full bytes required to house a number of bits.
 
     Args:
         * number_of_bits: Number of bits
 
     Error checking should have been done before.
 
-    Algorithm from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
+    For example 9 bits requires 2 bytes.
 
+    Algorithm from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
     """
     result = number_of_bits // _BITS_PER_BYTE  # Integer division in Python2 and 3
     if number_of_bits % _BITS_PER_BYTE:
         result += 1
     return result
 
 
-def _bit_to_bytestring(value: int) -> str:
+def _bit_to_bytes(value: int) -> bytes:
     """Create the bit pattern that is used for writing single bits.
 
     Used for functioncode 5. The same value is sent back in the response
     from the slave.
 
     This is basically a storage of numerical constants.
 
     Args:
         * value: Can be 0 or 1
 
     Returns:
-        The bit pattern (string).
+        The bit pattern.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_int(value, minvalue=0, maxvalue=1, description="inputvalue")
 
     if value == 0:
-        return "\x00\x00"
-    return "\xff\x00"
+        return b"\x00\x00"
+    return b"\xff\x00"
 
 
-def _bits_to_bytestring(valuelist: List[int]) -> str:
-    """Build a bytestring from a list of bits.
+def _bits_to_bytes(valuelist: List[int]) -> bytes:
+    """Build bytes from a list of bits.
 
     This is used for functioncode 15.
 
     Args:
         * valuelist: List of int (0 or 1)
 
-    Returns a bytestring.
-
+    Returns bytes.
     """
     if not isinstance(valuelist, list):
         raise TypeError(
             "The input should be a list. " + "Given: {!r}".format(valuelist)
         )
     for value in valuelist:
         if value not in [0, 1, False, True]:
             raise ValueError(
                 "Wrong value in list of bits. " + "Given: {!r}".format(value)
             )
 
     list_position = 0
-    outputstring = ""
+    outputbytes = b""
     while list_position < len(valuelist):
         sublist = valuelist[list_position : (list_position + _BITS_PER_BYTE)]
 
         bytevalue = 0
         for bitposition, value in enumerate(sublist):
             bytevalue |= value << bitposition
-        outputstring += chr(bytevalue)
+        outputbytes += bytevalue.to_bytes(1, "big")
 
         list_position += _BITS_PER_BYTE
-    return outputstring
+    return outputbytes
 
 
-def _bytestring_to_bits(bytestring: str, number_of_bits: int) -> List[int]:
-    """Parse bits from a bytestring.
+def _bytes_to_bits(inputbytes: bytes, number_of_bits: int) -> List[int]:
+    """Parse bits from bytes.
 
     This is used for parsing the bits in response messages for functioncode 1 and 2.
 
-    The first byte in the bytestring contains info on the addressed bit
+    The first byte in the *inputbytes* contains info on the addressed bit
     (in LSB in that byte). Second bit from right contains info on the bit
     on the next address.
 
-    Next byte in the bytestring contains data on next 8 bits. Might be padded with
+    Next byte in the *inputbytes* contains data on next 8 bits. Might be padded with
     zeros toward MSB.
 
     Args:
-        * bytestring: Input string
+        * inputbytes: Input bytes
         * number_of_bits: Number of bits to extract
 
-    Returns a list of values (0 or 1). The length of the list is equal to number_of_bits.
-
+    Returns a list of values (0 or 1). The length of the list is equal to
+    *number_of_bits*.
     """
     expected_length = _calculate_number_of_bytes_for_bits(number_of_bits)
-    if len(bytestring) != expected_length:
+    if len(inputbytes) != expected_length:
         raise ValueError(
-            "Wrong length of bytestring. Expected is "
+            "Wrong length of input bytes. Expected is "
             + "{} bytes (for {} bits), actual is {} bytes.".format(
-                expected_length, number_of_bits, len(bytestring)
+                expected_length, number_of_bits, len(inputbytes)
             )
         )
     total_list = []
-    for character in bytestring:
-        bytevalue = ord(character)
+    for bytevalue in inputbytes:  # Gives individual bytes as int
         for bitposition in range(_BITS_PER_BYTE):
             bitvalue = (bytevalue & (1 << bitposition)) > 0
             total_list.append(int(bitvalue))
     return total_list[:number_of_bits]
 
 
 # ################### #
@@ -2853,27 +2883,26 @@
     Args:
         * x: Input integer.
         * bits: Number of bits, must be > 0.
 
     Returns:
         The two's complement of the input.
 
-    Example for bits=8:
+    Example for *bits* = 8:
 
     ==== =======
     x    returns
     ==== =======
     0    0
     1    1
     127  127
     -128 128
     -127 129
     -1   255
     ==== =======
-
     """
     _check_int(bits, minvalue=0, description="number of bits")
     _check_int(x, description="input")
     upperlimit: int = 2 ** (bits - 1) - 1
     lowerlimit: int = -(2 ** (bits - 1))
     if x > upperlimit or x < lowerlimit:
         raise ValueError(
@@ -2882,40 +2911,39 @@
                 x, lowerlimit, upperlimit, bits
             )
         )
 
     # Calculate two'2 complement
     if x >= 0:
         return x
-    return int(x + 2 ** bits)
+    return int(x + 2**bits)
 
 
 def _from_twos_complement(x: int, bits: int = 16) -> int:
     """Calculate the inverse(?) of a two's complement of an integer.
 
     Args:
         * x: Input integer.
         * bits: Number of bits, must be > 0.
 
     Returns:
         The inverse(?) of two's complement of the input.
 
-    Example for bits=8:
+     Example for *bits* = 8:
 
     === =======
     x   returns
     === =======
     0   0
     1   1
     127 127
     128 -128
     129 -127
     255 -1
     === =======
-
     """
     _check_int(bits, minvalue=0, description="number of bits")
 
     _check_int(x, description="input")
     upperlimit = 2 ** (bits) - 1
     lowerlimit = 0
     if x > upperlimit or x < lowerlimit:
@@ -2926,56 +2954,55 @@
             )
         )
 
     # Calculate inverse(?) of two'2 complement
     limit = 2 ** (bits - 1) - 1
     if x <= limit:
         return x
-    return int(x - 2 ** bits)
+    return int(x - 2**bits)
 
 
 # ################ #
 # Bit manipulation #
 # ################ #
 
 
 def _set_bit_on(x: int, bit_num: int) -> int:
-    """Set bit 'bit_num' to True.
+    """Set bit *bit_num* to True.
 
     Args:
         * x: The value before.
         * bit_num: The bit number that should be set to True.
 
     Returns:
         The value after setting the bit.
 
     For example:
-        For x = 4 (dec) = 0100 (bin), setting bit number 0 results in 0101 (bin) = 5 (dec).
-
+        For x = 4 (dec) = 0100 (bin), setting bit number 0 results
+        in 0101 (bin) = 5 (dec).
     """
     _check_int(x, minvalue=0, description="input value")
     _check_int(bit_num, minvalue=0, description="bitnumber")
 
     return x | (1 << bit_num)
 
 
 def _check_bit(x: int, bit_num: int) -> bool:
-    """Check if bit 'bit_num' is set the input integer.
+    """Check if bit *bit_num* is set the input integer.
 
     Args:
         * x: The input value.
         * bit_num: The bit number to be checked
 
     Returns:
         True or False
 
     For example:
         For x = 4 (dec) = 0100 (bin), checking bit number 2 results in True, and
         checking bit number 3 results in False.
-
     """
     _check_int(x, minvalue=0, description="input value")
     _check_int(bit_num, minvalue=0, description="bitnumber")
 
     return (x & (1 << bit_num)) > 0
 
 
@@ -3263,105 +3290,110 @@
         if not i%11:
             output += "\n"
         output += "{:5.0f}, ".format(m)
     print output
 """
 
 
-def _calculate_crc_string(inputstring: str) -> str:
-    """Calculate CRC-16 for Modbus.
+def _is_serial_object(obj: Any) -> bool:
+    """Check if an object is serialport-like."""
+    KNOWN_ATTRIBUTES = ["open", "close", "read", "write", "is_open"]
+
+    for attribute_name in KNOWN_ATTRIBUTES:
+        if not hasattr(obj, attribute_name):
+            return False
+    return True
+
+
+def _calculate_crc(inputbytes: bytes) -> bytes:
+    """Calculate CRC-16 for Modbus RTU.
 
     Args:
-        inputstring: An arbitrary-length message (without the CRC).
+        inputbytes: An arbitrary-length message (without the CRC).
 
     Returns:
-        A two-byte CRC string, where the least significant byte is first.
-
+        A two-byte CRC, where the least significant byte is first.
     """
-    _check_string(inputstring, description="input CRC string")
+    _check_bytes(inputbytes, description="CRC input bytes")
 
     # Preload a 16-bit register with ones
     register = 0xFFFF
 
-    for char in inputstring:
-        register = (register >> 8) ^ _CRC16TABLE[(register ^ ord(char)) & 0xFF]
+    for current_byte in inputbytes:
+        register = (register >> 8) ^ _CRC16TABLE[(register ^ current_byte) & 0xFF]
 
-    return _num_to_twobyte_string(register, lsb_first=True)
+    return _num_to_two_bytes(register, lsb_first=True)
 
 
-def _calculate_lrc_string(inputstring: str) -> str:
-    """Calculate LRC for Modbus.
+def _calculate_lrc(inputbytes: bytes) -> bytes:
+    """Calculate LRC for Modbus ASCII.
 
     Args:
-        inputstring: An arbitrary-length message (without the beginning
+        inputbytes: An arbitrary-length message (without the beginning
         colon and terminating CRLF). It should already be decoded from hex-string.
 
     Returns:
-        A one-byte LRC bytestring (not encoded to hex-string)
+        A one-byte LRC (not encoded to hex-string)
 
     Algorithm from the document 'MODBUS over serial line specification and
     implementation guide V1.02'.
 
     The LRC is calculated as 8 bits (one byte).
 
-    For example a LRC 0110 0001 (bin) = 61 (hex) = 97 (dec) = 'a'. This function will
-    then return 'a'.
+    For example a resulting LRC 0110 0001 (bin) = 61 (hex) = 97 (dec) = ``b'a'``.
+    This function will then return ``b'a'``.
 
     In Modbus ASCII mode, this should be transmitted using two characters. This
-    example should be transmitted '61', which is a string of length two. This function
-    does not handle that conversion for transmission.
-
+    example should be transmitted as ``b'61'``, which is a bytes object of length two.
+    This function does not handle that conversion for transmission.
     """
-    _check_string(inputstring, description="input LRC string")
+    _check_bytes(inputbytes, description="LRC input bytes")
 
     register = 0
-    for character in inputstring:
-        register += ord(character)
+    for bytevalue in inputbytes:
+        register += bytevalue
 
     lrc = ((register ^ 0xFF) + 1) & 0xFF
 
-    return _num_to_onebyte_string(lrc)
+    return _num_to_one_byte(lrc)
 
 
 def _check_mode(mode: str) -> None:
     """Check that the Modbus mode is valid.
 
     Args:
         mode: The Modbus mode (MODE_RTU or MODE_ASCII)
 
     Raises:
         TypeError, ValueError
-
     """
     if not isinstance(mode, str):
         raise TypeError("The {0} should be a string. Given: {1!r}".format("mode", mode))
 
     if mode not in [MODE_RTU, MODE_ASCII]:
         raise ValueError(
-            "Unreconized Modbus mode given. Must be 'rtu' or 'ascii' but {0!r} was given.".format(
-                mode
-            )
+            "Unreconized Modbus mode given. Must "
+            + "be 'rtu' or 'ascii' but {0!r} was given.".format(mode)
         )
 
 
 def _check_functioncode(
     functioncode: int, list_of_allowed_values: Optional[List[int]] = None
 ) -> None:
-    """Check that the given functioncode is in the list_of_allowed_values.
+    """Check that the given functioncode is in the *list_of_allowed_values*.
 
     Also verifies that 1 <= function code <= 127.
 
     Args:
         * functioncode: The function code
         * list_of_allowed_values: Allowed values. Use *None* to bypass
           this part of the checking.
 
     Raises:
         TypeError, ValueError
-
     """
     FUNCTIONCODE_MIN = 1
     FUNCTIONCODE_MAX = 127
 
     _check_int(
         functioncode, FUNCTIONCODE_MIN, FUNCTIONCODE_MAX, description="functioncode"
     )
@@ -3389,75 +3421,90 @@
             "Wrong function code: {0}, allowed values are {1!r}".format(
                 functioncode, list_of_allowed_values
             )
         )
 
 
 def _check_slaveaddress(slaveaddress: int) -> None:
-    """Check that the given slaveaddress is valid.
+    """Check that the given *slaveaddress* is valid.
 
     Args:
         slaveaddress: The slave address
 
     Raises:
         TypeError, ValueError
-
     """
     SLAVEADDRESS_MAX = 255  # Allows usage also of reserved addresses
     SLAVEADDRESS_MIN = 0
 
     _check_int(
         slaveaddress, SLAVEADDRESS_MIN, SLAVEADDRESS_MAX, description="slaveaddress"
     )
 
 
 def _check_registeraddress(registeraddress: int) -> None:
-    """Check that the given registeraddress is valid.
+    """Check that the given *registeraddress* is valid.
 
     Args:
         registeraddress: The register address
 
     Raises:
         TypeError, ValueError
-
     """
     REGISTERADDRESS_MAX = 0xFFFF
     REGISTERADDRESS_MIN = 0
 
     _check_int(
         registeraddress,
         REGISTERADDRESS_MIN,
         REGISTERADDRESS_MAX,
         description="registeraddress",
     )
 
 
 def _check_response_payload(
-    payload: str,
+    payload: bytes,
     functioncode: int,
     registeraddress: int,
     value: Any,
     number_of_decimals: int,
     number_of_registers: int,
     number_of_bits: int,
     signed: bool,
-    byteorder: int,  # Not used. For keeping same signature as _parse_payload()
-    payloadformat: _Payloadformat,  # Not used. For keeping same signature as _parse_payload()
+    byteorder: int,  # Not used. For same signature as _parse_payload()
+    payloadformat: _Payloadformat,  # Not used. For same signature as _parse_payload()
 ) -> None:
+    """Check the response payload.
+
+    Args:
+        * payload:              Payload to be checked
+        * functioncode:         Function code
+        * registeraddress:      Register address
+        * value:                Value in request
+        * number_of_decimals:   Number of decimals
+        * number_of_registers:  Number of registers
+        * number_of_bits:       Number of bits
+        * signed:               Signed
+        * byteorder:            Byte order
+        * payloadformat:        Payload format
+
+    Raises:
+        ValueError, TypeError
+    """
     if functioncode in [1, 2, 3, 4]:
         _check_response_bytecount(payload)
 
     if functioncode in [5, 6, 15, 16]:
         _check_response_registeraddress(payload, registeraddress)
 
     if functioncode == 5:
-        _check_response_writedata(payload, _bit_to_bytestring(value))
+        _check_response_writedata(payload, _bit_to_bytes(value))
     elif functioncode == 6:
         _check_response_writedata(
-            payload, _num_to_twobyte_string(value, number_of_decimals, signed=signed)
+            payload, _num_to_two_bytes(value, number_of_decimals, signed=signed)
         )
     elif functioncode == 15:
         # response number of bits
         _check_response_number_of_registers(payload, number_of_bits)
 
     elif functioncode == 16:
         _check_response_number_of_registers(payload, number_of_registers)
@@ -3483,29 +3530,28 @@
                 "The register data length is wrong. "
                 + "Registerdata: {!r} bytes. Expected: {!r}.".format(
                     len(registerdata), number_of_register_bytes
                 )
             )
 
 
-def _check_response_slaveerrorcode(response: str) -> None:
+def _check_response_slaveerrorcode(response: bytes) -> None:
     """Check if the slave indicates an error.
 
     Args:
         * response: Response from the slave
 
     The response is in RTU format, but the checksum might be one or two bytes
     depending on whether it was sent in RTU or ASCII mode.
 
     Checking of type and length of the response should be done before calling
     this functions.
 
     Raises:
         SlaveReportedException or subclass
-
     """
     NON_ERRORS = [5]
     SLAVE_ERRORS = {
         1: IllegalRequestError("Slave reported illegal function"),
         2: IllegalRequestError("Slave reported illegal data address"),
         3: IllegalRequestError("Slave reported illegal data value"),
         4: SlaveReportedException("Slave reported device failure"),
@@ -3517,52 +3563,51 @@
             "Slave reported gateway target device failed to respond"
         ),
     }
 
     if len(response) < _BYTEPOSITION_FOR_SLAVE_ERROR_CODE + 1:
         return  # This check is also done before calling, do not raise exception here.
 
-    received_functioncode = ord(response[_BYTEPOSITION_FOR_FUNCTIONCODE])
+    received_functioncode = response[_BYTEPOSITION_FOR_FUNCTIONCODE]
 
     if _check_bit(received_functioncode, _BITNUMBER_FUNCTIONCODE_ERRORINDICATION):
-        slave_error_code = ord(response[_BYTEPOSITION_FOR_SLAVE_ERROR_CODE])
+        slave_error_code = response[_BYTEPOSITION_FOR_SLAVE_ERROR_CODE]
 
         if slave_error_code in NON_ERRORS:
             return
 
         error = SLAVE_ERRORS.get(
             slave_error_code,
             SlaveReportedException(
                 "Slave reported error code " + str(slave_error_code)
             ),
         )
         raise error
 
 
-def _check_response_bytecount(payload: str) -> None:
+def _check_response_bytecount(payload: bytes) -> None:
     """Check that the number of bytes as given in the response is correct.
 
     The first byte in the payload indicates the length of the payload (first
     byte not counted).
 
     Args:
         payload: The payload
 
     Raises:
         TypeError, ValueError, InvalidResponseError
-
     """
     POSITION_FOR_GIVEN_NUMBER = 0
     NUMBER_OF_BYTES_TO_SKIP = 1
 
-    _check_string(
+    _check_bytes(
         payload, minlength=1, description="payload", exception_type=InvalidResponseError
     )
 
-    given_number_of_databytes = ord(payload[POSITION_FOR_GIVEN_NUMBER])
+    given_number_of_databytes = payload[POSITION_FOR_GIVEN_NUMBER]
     counted_number_of_databytes = len(payload) - NUMBER_OF_BYTES_TO_SKIP
 
     if given_number_of_databytes != counted_number_of_databytes:
         errortemplate = (
             "Wrong given number of bytes in the response: "
             + "{0}, but counted is {1} as data payload length is {2}."
             + " The data payload is: {3!r}"
@@ -3572,106 +3617,104 @@
             counted_number_of_databytes,
             len(payload),
             payload,
         )
         raise InvalidResponseError(errortext)
 
 
-def _check_response_registeraddress(payload: str, registeraddress: int) -> None:
+def _check_response_registeraddress(payload: bytes, registeraddress: int) -> None:
     """Check that the start adress as given in the response is correct.
 
     The first two bytes in the payload holds the address value.
 
     Args:
         * payload: The payload
-        * registeraddress: What the register address actually shoud be
-          (use decimal numbers, not hex).
+        * registeraddress: What the register address actually shoud be.
 
     Raises:
         TypeError, ValueError, InvalidResponseError
-
     """
-    _check_string(
+    _check_bytes(
         payload, minlength=2, description="payload", exception_type=InvalidResponseError
     )
     _check_registeraddress(registeraddress)
 
     BYTERANGE_FOR_STARTADDRESS = slice(0, 2)
 
     bytes_for_startaddress = payload[BYTERANGE_FOR_STARTADDRESS]
-    received_startaddress = _twobyte_string_to_num(bytes_for_startaddress)
+    received_startaddress = _two_bytes_to_num(bytes_for_startaddress)
 
     if received_startaddress != registeraddress:
         raise InvalidResponseError(
             "Wrong given write start adress: "
             + "{0}, but commanded is {1}. The data payload is: {2!r}".format(
                 received_startaddress, registeraddress, payload
             )
         )
 
 
-def _check_response_number_of_registers(payload: str, number_of_registers: int) -> None:
+def _check_response_number_of_registers(
+    payload: bytes, number_of_registers: int
+) -> None:
     """Check that the number of written registers as given in the response is correct.
 
     The bytes 2 and 3 (zero based counting) in the payload holds the value.
 
     Args:
         * payload: The payload
         * number_of_registers: Number of registers that have been written
 
     Raises:
         TypeError, ValueError, InvalidResponseError
-
     """
-    _check_string(
+    _check_bytes(
         payload, minlength=4, description="payload", exception_type=InvalidResponseError
     )
     _check_int(
         number_of_registers,
         minvalue=1,
         maxvalue=max(
             _MAX_NUMBER_OF_REGISTERS_TO_READ, _MAX_NUMBER_OF_REGISTERS_TO_WRITE
         ),
         description="number of registers",
     )
 
     BYTERANGE_FOR_NUMBER_OF_REGISTERS = slice(2, 4)
 
     bytes_for_mumber_of_registers = payload[BYTERANGE_FOR_NUMBER_OF_REGISTERS]
-    received_number_of_written_registers = _twobyte_string_to_num(
+    received_number_of_written_registers = _two_bytes_to_num(
         bytes_for_mumber_of_registers
     )
 
     if received_number_of_written_registers != number_of_registers:
         raise InvalidResponseError(
             "Wrong number of registers to write in the response: "
             + "{0}, but commanded is {1}. The data payload is: {2!r}".format(
                 received_number_of_written_registers, number_of_registers, payload
             )
         )
 
 
-def _check_response_writedata(payload: str, writedata: str) -> None:
+def _check_response_writedata(payload: bytes, writedata: bytes) -> None:
     """Check that the write data as given in the response is correct.
 
     The bytes 2 and 3 (zero based counting) in the payload holds the write data.
 
     Args:
         * payload: The payload
         * writedata: The data that should have been written.
           Length should be 2 bytes.
 
     Raises:
         TypeError, ValueError, InvalidResponseError
-
     """
-    _check_string(
+    _check_bytes(
         payload, minlength=4, description="payload", exception_type=InvalidResponseError
     )
-    _check_string(writedata, minlength=2, maxlength=2, description="writedata")
+    _check_bytes(writedata, minlength=2, maxlength=2, description="writedata")
 
     BYTERANGE_FOR_WRITEDATA = slice(2, 4)
 
     received_writedata = payload[BYTERANGE_FOR_WRITEDATA]
 
     if received_writedata != writedata:
         raise InvalidResponseError(
@@ -3683,16 +3726,25 @@
 
 
 def _check_bytes(
     inputbytes: bytes,
     description: str,
     minlength: int = 0,
     maxlength: Optional[int] = None,
+    exception_type: Type[Exception] = ValueError,
 ) -> None:
-    """Check that the bytes are valid."""
+    """Check that the bytes are valid.
+
+    Args:
+        * inputbytes: The bytes to be checked
+        * description: Used in error messages for the checked inputbytes
+        * minlength: Minimum length of the inputbytes
+        * maxlength: Maximum length of the inputbytes
+        * exception_type: The type of exception to raise for length errors
+    """
     # Type checking
     if not isinstance(description, str):
         raise TypeError(
             "The description should be a string. Given: {0!r}".format(description)
         )
 
     if not isinstance(inputbytes, bytes):
@@ -3705,36 +3757,36 @@
             "The maxlength must be an integer or None. Given: {0!r}".format(maxlength)
         )
 
     # Check values
     _check_int(minlength, minvalue=0, maxvalue=None, description="minlength")
 
     if len(inputbytes) < minlength:
-        raise ValueError(
+        raise exception_type(
             "The {0} is too short: {1}, but minimum value is {2}. Given: {3!r}".format(
                 description, len(inputbytes), minlength, inputbytes
             )
         )
 
     if maxlength is not None:
         if maxlength < 0:
             raise ValueError(
                 "The maxlength must be positive. Given: {0}".format(maxlength)
             )
 
         if maxlength < minlength:
             raise ValueError(
-                "The maxlength must not be smaller than minlength. Given: {0} and {1}".format(
-                    maxlength, minlength
-                )
+                "The maxlength must not be smaller than "
+                + "minlength. Given: {0} and {1}".format(maxlength, minlength)
             )
 
         if len(inputbytes) > maxlength:
-            raise ValueError(
-                "The {0} is too long: {1}, but maximum value is {2}. Given: {3!r}".format(
+            raise exception_type(
+                "The "
+                + "{0} is too long: {1}, but maximum value is {2}. Given: {3!r}".format(
                     description, len(inputbytes), maxlength, inputbytes
                 )
             )
 
 
 def _check_string(
     inputstring: str,
@@ -3744,27 +3796,24 @@
     force_ascii: bool = False,
     exception_type: Type[Exception] = ValueError,
 ) -> None:
     """Check that the given string is valid.
 
     Args:
         * inputstring: The string to be checked
-        * description: Used in error messages for the checked inputstring
+        * description: Used in error messages for the checked *inputstring*
         * minlength: Minimum length of the string
         * maxlength: Maximum length of the string
         * force_ascii: Enforce that the string is ASCII
         * exception_type: The type of exception to raise for length errors
 
-    The force_ascii argument is valid only for Python3, as all strings are ASCII in Python2.
-
     Raises:
         TypeError, ValueError or the one given by exception_type
 
     Uses the function :func:`_check_int` internally.
-
     """
     # Type checking
     if not isinstance(description, str):
         raise TypeError(
             "The description should be a string. Given: {0!r}".format(description)
         )
 
@@ -3805,22 +3854,24 @@
         if maxlength < 0:
             raise ValueError(
                 "The maxlength must be positive. Given: {0}".format(maxlength)
             )
 
         if maxlength < minlength:
             raise ValueError(
-                "The maxlength must not be smaller than minlength. Given: {0} and {1}".format(
+                "The maxlength must "
+                + "not be smaller than minlength. Given: {0} and {1}".format(
                     maxlength, minlength
                 )
             )
 
         if len(inputstring) > maxlength:
             raise exception_type(
-                "The {0} is too long: {1}, but maximum value is {2}. Given: {3!r}".format(
+                "The "
+                + "{0} is too long: {1}, but maximum value is {2}. Given: {3!r}".format(
                     description, len(inputstring), maxlength, inputstring
                 )
             )
 
     if force_ascii and sys.version > "3":
         try:
             inputstring.encode("ascii")
@@ -3845,15 +3896,14 @@
         * description: Used in error messages for the checked inputvalue
 
     Raises:
         TypeError, ValueError
 
     Note: Can not use the function :func:`_check_string`, as that function uses this
     function internally.
-
     """
     if not isinstance(description, str):
         raise TypeError(
             "The description should be a string. Given: {0!r}".format(description)
         )
 
     if not isinstance(inputvalue, (int)):
@@ -3880,24 +3930,23 @@
     maxvalue: Union[None, int, float] = None,
     description: str = "inputvalue",
 ) -> None:
     """Check that the given numerical value is valid.
 
     Args:
         * inputvalue: The value to be checked.
-        * minvalue: Minimum value  Use None to skip this part of the test.
+        * minvalue: Minimum value. Use None to skip this part of the test.
         * maxvalue: Maximum value. Use None to skip this part of the test.
         * description: Used in error messages for the checked inputvalue
 
     Raises:
         TypeError, ValueError
 
     Note: Can not use the function :func:`_check_string`, as it uses this function
     internally.
-
     """
     # Type checking
     if not isinstance(description, str):
         raise TypeError(
             "The description should be a string. Given: {0!r}".format(description)
         )
 
@@ -3939,232 +3988,40 @@
                 "The {0} is too large: {1}, but maximum value is {2}.".format(
                     description, inputvalue, maxvalue
                 )
             )
 
 
 def _check_bool(inputvalue: bool, description: str = "inputvalue") -> None:
-    """Check that the given inputvalue is a boolean.
+    """Check that the given *inputvalue* is a boolean.
 
     Args:
         * inputvalue: The value to be checked.
         * description: Used in error messages for the checked inputvalue.
 
     Raises:
         TypeError, ValueError
-
     """
     _check_string(description, minlength=1, description="description string")
     if not isinstance(inputvalue, bool):
         raise TypeError(
             "The {0} must be boolean. Given: {1!r}".format(description, inputvalue)
         )
 
 
 #####################
 # Development tools #
 #####################
 
 
-def _print_out(inputstring: str) -> None:
-    """Print the inputstring. To make it compatible with Python2 and Python3.
-
-    Args:
-        inputstring (str): The string that should be printed.
-
-    Raises:
-        TypeError
-
-    """
-    _check_string(inputstring, description="string to print")
-
-    sys.stdout.write(inputstring + "\n")
-    sys.stdout.flush()
-
-
-# def _interpretRawMessage(inputstr):
-#     r"""Generate a human readable description of a Modbus bytestring.
-
-#     Args:
-#         inputstr (str): The bytestring that should be interpreted.
-
-#     Returns:
-#         A descriptive string.
-
-#     For example, the string ``'\n\x03\x10\x01\x00\x01\xd0q'`` should give something like::
-
-#         T ODO: update
-
-#         Modbus bytestring decoder
-#         Input string (length 8 characters): '\n\x03\x10\x01\x00\x01\xd0q'
-#         Probably modbus RTU mode.
-#         Slave address: 10 (dec). Function code: 3 (dec).
-#         Valid message. Extracted payload: '\x10\x01\x00\x01'
-
-#         Pos   Character Hex  Dec  Probable interpretation
-#         -------------------------------------------------
-#           0:  '\n'      0A    10  Slave address
-#           1:  '\x03'    03     3  Function code
-#           2:  '\x10'    10    16  Payload
-#           3:  '\x01'    01     1  Payload
-#           4:  '\x00'    00     0  Payload
-#           5:  '\x01'    01     1  Payload
-#           6:  '\xd0'    D0   208  Checksum, CRC LSB
-#           7:  'q'       71   113  Checksum, CRC MSB
-
-#     """
-#     raise NotImplementedError()
-#     output = ""
-#     output += "Modbus bytestring decoder\n"
-#     output += "Input string (length {} characters): {!r} \n".format(
-#         len(inputstr), inputstr
-#     )
-
-#     # Detect modbus type
-#     if inputstr.startswith(_ASCII_HEADER) and inputstr.endswith(_ASCII_FOOTER):
-#         mode = MODE_ASCII
-#     else:
-#         mode = MODE_RTU
-#     output += "Probably Modbus {} mode.\n".format(mode.upper())
-
-#     # Extract slave address and function code
-#     try:
-#         if mode == MODE_ASCII:
-#             slaveaddress = int(inputstr[1:3])
-#             functioncode = int(inputstr[3:5])
-#         else:
-#             slaveaddress = ord(inputstr[0])
-#             functioncode = ord(inputstr[1])
-#         output += "Slave address: {} (dec). Function code: {} (dec).\n".format(
-#             slaveaddress, functioncode
-#         )
-#     except Exception:
-#         output += "\nCould not extract slave address and function code. \n\n"
-
-#     # Check message validity
-#     try:
-#         extractedpayload = _extract_payload(inputstr, slaveaddress, mode, functioncode)
-#         output += "Valid message. Extracted payload: {!r}\n".format(extractedpayload)
-#     except (ValueError, TypeError) as err:
-#         output += "\nThe message does not seem to be valid Modbus {}. ".format(mode.upper())
-#         output += "Error message: \n{}. \n\n".format(err.messages)
-#     except NameError as err:
-#         output += (
-#             "\nNo message validity checking. \n\n"
-#         )  # Slave address or function code not available
-
-#     # Generate table describing the message
-#     if mode == MODE_RTU:
-#         output += "\nPos   Character Hex  Dec  Probable interpretation \n"
-#         output += "------------------------------------------------- \n"
-#         for i, character in enumerate(inputstr):
-#             if i == 0:
-#                 description = "Slave address"
-#             elif i == 1:
-#                 description = "Function code"
-#             elif i == len(inputstr) - 2:
-#                 description = "Checksum, CRC LSB"
-#             elif i == len(inputstr) - 1:
-#                 description = "Checksum, CRC MSB"
-#             else:
-#                 description = "Payload"
-#             output += "{0:3.0f}:  {1!r:<8}  {2:02X}  {2: 4.0f}  {3:<10} \n".format(
-#                 i, character, ord(character), description
-#             )
-
-#     elif mode == MODE_ASCII:
-#         output += "\nPos   Character(s) Converted  Hex  Dec  Probable interpretation \n"
-#         output += "--------------------------------------------------------------- \n"
-
-#         i = 0
-#         while i < len(inputstr):
-
-#             if inputstr[i] in [":", "\r", "\n"]:
-#                 if inputstr[i] == ":":
-#                     description = "Start character"
-#                 else:
-#                     description = "Stop character"
-
-#                 output += "{0:3.0f}:  {1!r:<8}                          {2} \n".format(
-#                     i, inputstr[i], description
-#                 )
-#                 i += 1
-
-#             else:
-#                 if i == 1:
-#                     description = "Slave address"
-#                 elif i == 3:
-#                     description = "Function code"
-#                 elif i == len(inputstr) - 4:
-#                     description = "Checksum (LRC)"
-#                 else:
-#                     description = "Payload"
-
-#                 try:
-#                     hexvalue = _hexdecode(inputstr[i:(i + 2)])
-#                     output += "{0:3.0f}:  {1!r:<8}     {2!r}     {3:02X}  {3: 4.0f}  {4} \n".
-#                               format(
-#                         i, inputstr[i:(i + 2)], hexvalue, ord(hexvalue), description
-#                     )
-#                 except Exception:
-#                     output += "{0:3.0f}:  {1!r:<8}     ?           ?     ?  {2} \n".format(
-#                         i, inputstr[i:(i + 2)], description
-#                     )
-#                 i += 2
-
-#     # Generate description for the payload
-#     output += "\n\n"
-#     try:
-#         output += _interpretPayload(functioncode, extractedpayload)
-#     except Exception:
-#         output += (
-#             "\nCould not interpret the payload. \n\n"
-#         )  # Payload or function code not available
-
-#     return output
-
-
-# def _interpretPayload(functioncode, payload):
-#     r"""Generate a human readable description of a Modbus payload.
-
-#     Args:
-#       * functioncode (int): Function code
-#       * payload (str): The payload that should be interpreted. It should be a
-#         byte string.
-
-#     Returns:
-#         A descriptive string.
-
-#     For example, the payload ``'\x10\x01\x00\x01'`` for functioncode 3 should give
-#         something like::
-
-#             T ODO: Update
-
-#     """
-#     raise NotImplementedError()
-#     output = ""
-#     output += "Modbus payload decoder\n"
-#     output += "Input payload (length {} characters): {!r} \n".format(
-#         len(payload), payload
-#     )
-#     output += "Function code: {} (dec).\n".format(functioncode)
-
-#     if len(payload) == 4:
-#         FourbyteMessageFirstHalfValue = _twobyte_string_to_num(payload[0:2])
-#         FourbyteMessageSecondHalfValue = _twobyte_string_to_num(payload[2:4])
-
-#     return output
-
-
 def _get_diagnostic_string() -> str:
     """Generate a diagnostic string, showing the module version, the platform etc.
 
     Returns:
         A descriptive string.
-
     """
     text = "\n## Diagnostic output from minimalmodbus ## \n\n"
     text += "Minimalmodbus version: " + __version__ + "\n"
     text += "File name (with relative path): " + __file__ + "\n"
     text += "Full file path: " + os.path.abspath(__file__) + "\n\n"
     text += "pySerial version: " + serial.VERSION + "\n"
     text += "pySerial full file path: " + os.path.abspath(serial.__file__) + "\n\n"
```

### Comparing `minimalmodbus-2.0.1/stubs/serial.pyi` & `minimalmodbus-2.1.0/stubs/serial.pyi`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/tests/__init__.py` & `minimalmodbus-2.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.0.1/tests/dummy_serial.py` & `minimalmodbus-2.1.0/tests/dummy_serial.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,73 +23,80 @@
 __author__ = "Jonas Berg"
 __license__ = "Apache License, Version 2.0"
 
 import time
 from typing import Dict, Optional, Union
 
 DEFAULT_TIMEOUT: float = 0.01
-"""The default timeot value in seconds. Used if not set by the constructor."""
+"""The default timeot value in seconds.
+
+Used if not set by the constructor.
+"""
 
 SLEEPTIME_READ: float = 0.001
-"""Simulated read time, in seconds. """
+"""Simulated read time, in seconds."""
 
 SLEEPTIME_WRITE: float = 0.001
-"""Simulated write time, in seconds. """
+"""Simulated write time, in seconds."""
 
 DEFAULT_BAUDRATE: int = 19200
-"""The default baud rate. Used if not set by the constructor."""
+"""The default baud rate.
+
+Used if not set by the constructor.
+"""
 
 VERBOSE: bool = False
-"""Set this to :const:`True` for printing the communication, and also details on the port initialization.
+"""Set this to :const:`True` for printing the communication, and also details on the
+port initialization.
 
 Might be monkey-patched in the calling test module.
 """
 
 RESPONSES: Dict[bytes, bytes] = {}
 """A dictionary of respones from the dummy serial port.
 
-The key is the message (bytes) sent to the dummy serial port, and the item is the response (bytes)
-from the dummy serial port.
+The key is the message (bytes) sent to the dummy serial port, and the item is the
+response (bytes) from the dummy serial port.
 
 Intended to be monkey-patched in the calling test module.
-
 """
 RESPONSES[b"EXAMPLEREQUEST"] = b"EXAMPLERESPONSE"
 
 
 DEFAULT_RESPONSE = b"NotFoundInResponseDictionary"
 """Response when no matching message (key) is found in the look-up dictionary.
 
-Should not be an empty string, as that is interpreted as "no data available on port".
+Should not be an empty bytes object, as that is interpreted as
+"no data available on port".
 
 Might be monkey-patched in the calling test module.
-
 """
 
 NO_DATA_PRESENT = b""
 
 
 def _describe_bytes(inputbytes: bytes) -> str:
     return " ".join([f"{x:02X}" for x in inputbytes]) + " ({} bytes)".format(
         len(inputbytes)
     )
 
 
 class Serial:
     """Dummy (mock) serial port for testing purposes.
 
-    Mimics the behavior of a serial port as defined by the `pySerial <https://github.com/pyserial/pyserial>`_ module.
+    Mimics the behavior of a serial port as defined by
+    the `pySerial <https://github.com/pyserial/pyserial>`_ module.
 
     Args:
         * port:
         * timeout:
 
     Note:
-    As the portname argument not is used properly, only one port on :mod:`dummy_serial` can be used simultaneously.
-
+    As the portname argument not is used properly, only one port
+    on :mod:`dummy_serial` can be used simultaneously.
     """
 
     port: Optional[str]  # Serial port name.
     timeout: float
     baudrate: int
     _initial_port_name: Optional[str]  # Initial name given to the serial port
     _last_written_data: bytes
@@ -105,33 +112,40 @@
         stopbits: Union[int, float] = 1,
         timeout: Optional[float] = None,
         xonxoff: bool = False,
         rtscts: bool = False,
         write_timeout: Optional[float] = None,
         dsrdtr: bool = False,
         inter_byte_timeout: Optional[float] = None,
+        fail_to_open: bool = False,
     ) -> None:
         self._waiting_data = NO_DATA_PRESENT
         self._last_written_data = NO_DATA_PRESENT
-        self._isOpen = True
+        self._fail_to_open = fail_to_open
+        self._isOpen = True if not self._fail_to_open else False
         self.port = port  # Serial port name.
         self._initial_port_name = self.port  # Initial name given to the serial port
 
         self.timeout = timeout if timeout is not None else DEFAULT_TIMEOUT
         self.baudrate = baudrate
 
         if VERBOSE:
             print("\nDummy_serial: Initializing")
             print(
-                f"dummy_serial initialization. Port: {self.port} Baud rate: {self.baudrate} Timeout {self.timeout}"
+                f"dummy_serial initialization. Port: {self.port} "
+                + f"Baud rate: {self.baudrate} Timeout {self.timeout}"
             )
 
     def __repr__(self) -> str:
-        """String representation of the dummy_serial object"""
-        return "{0}.{1}<id=0x{2:x}, open={3}>(port={4!r}, timeout={5!r}, waiting_data={6!r})".format(
+        """String representation of the dummy_serial object."""
+        template = (
+            "{0}.{1}<id=0x{2:x}, open={3}>(port={4!r}, "
+            + "timeout={5!r}, waiting_data={6!r})"
+        )
+        return template.format(
             self.__module__,
             self.__class__.__name__,
             id(self),
             self._isOpen,
             self.port,
             self.timeout,
             self._waiting_data,
@@ -151,45 +165,45 @@
     def reset_output_buffer(self) -> None:
         pass
 
     def flush(self) -> None:
         pass
 
     def open(self) -> None:
-        """Open a (previously initialized) port on dummy_serial."""
+        """Open a (previously initialized) port on :py:mod:`dummy_serial`."""
         if VERBOSE:
             print("\nDummy_serial: Opening port\n")
 
         if self._isOpen:
             raise IOError("Dummy_serial: The port is already open")
 
-        self._isOpen = True
+        if not self._fail_to_open:
+            self._isOpen = True
         self.port = self._initial_port_name
 
     def close(self) -> None:
-        """Close a port on dummy_serial."""
+        """Close a port on :py:mod:`dummy_serial`."""
         if VERBOSE:
             print("\nDummy_serial: Closing port\n")
 
         if not self._isOpen:
             raise IOError("Dummy_serial: The port is already closed")
 
         self._isOpen = False
         self.port = None
 
     def write(self, inputdata: bytes) -> int:
         """Write to a port on dummy_serial.
 
         Args:
-            inputdata: data for sending to the port on dummy_serial. Will affect the response
-            for subsequent read operations.
+            inputdata: data for sending to the port on :py:mod:`dummy_serial`. Will
+            affect the response for subsequent read operations.
 
         Returns:
             Number of bytes written
-
         """
         if VERBOSE:
             print(
                 "\nDummy_serial: Writing to port. Given: "
                 + _describe_bytes(inputdata)
                 + "\n"
             )
@@ -202,63 +216,62 @@
                 "Dummy_serial: Trying to write, but the port is not open. Given:"
                 + repr(inputdata)
             )
 
         # Look up which data that should be waiting for subsequent read commands
         try:
             response = RESPONSES[inputdata]
-        except:
+        except KeyError:
             response = DEFAULT_RESPONSE
         self._last_written_data = inputdata
         self._waiting_data = response
 
         time.sleep(SLEEPTIME_WRITE)
 
         return len(inputdata)
 
     def read(self, size: int) -> bytes:
-        """Read from a port on dummy_serial.
+        """Read from a port on :py:mod:`dummy_serial`.
 
-        The response is dependent on what was written last to the port on dummy_serial,
-        and what is defined in the :data:`RESPONSES` dictionary.
+        The response is dependent on what was written last to the port on
+        :py:mod:`dummy_serial`, and what is defined in the :data:`RESPONSES` dictionary.
 
         Args:
             size (int): For compability with the real function.
 
-        If the response is shorter than size, it will sleep for timeout.
-        If the response is longer than size, it will return only size bytes.
-
+        If the response is shorter than *size*, it will sleep for timeout.
+        If the response is longer than *size*, it will return only *size* bytes.
         """
         if VERBOSE:
             print(
                 "\nDummy_serial: Reading from port (max length {!r} bytes)".format(size)
             )
 
         if size < 0:
             raise IOError(
-                "Dummy_serial: The size to read must not be negative. Given: {!r}".format(
-                    size
-                )
+                "Dummy_serial: The size to read must "
+                + "not be negative. Given: {!r}".format(size)
             )
 
         if not self._isOpen:
             raise IOError("Dummy_serial: Trying to read, but the port is not open.")
 
-        # Do the actual reading from the waiting data, and simulate the influence of size
+        # Do actual reading from the waiting data, and simulate the influence of size
 
         if self._waiting_data == DEFAULT_RESPONSE:
             returnbytes = self._waiting_data
         elif size == len(self._waiting_data):
             returnbytes = self._waiting_data
             self._waiting_data = NO_DATA_PRESENT
         elif size < len(self._waiting_data):
             if VERBOSE:
                 print(
-                    "Dummy_serial: The size to read is smaller than the available data. "
-                    + "Some bytes will be kept for later. Available data: {}, size: {}".format(
+                    "Dummy_serial: The size to read is smaller than the "
+                    + "available data. Some bytes will be kept for later. "
+                    + "Available data: {}, size: {}".format(
                         _describe_bytes(self._waiting_data), size
                     )
                 )
             returnbytes = self._waiting_data[:size]
             self._waiting_data = self._waiting_data[size:]
         else:  # Wait for timeout, as we have asked for more data than available
             if VERBOSE:
```

### Comparing `minimalmodbus-2.0.1/tests/test_deltaDTB4824.py` & `minimalmodbus-2.1.0/tests/test_deltaDTB4824.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-"""
-Hardware testing of MinimalModbus using the Delta DTB temperature controller.
+"""Hardware testing of MinimalModbus using the Delta DTB temperature controller.
 
 For use with Delta DTB4824VR.
 
-Usage
--------------
-
-::
-
-    python3 scriptname [-rtu] [-ascii] [-b38400] [-D/dev/ttyUSB0]
-
-Arguments:
- * -b : baud rate
- * -D : port name
-
-NOTE: There should be no space between the option switch and its argument.
-
-Defaults to RTU mode.
-
 
 Recommended test sequence
 ---------------------------
-Make sure that RUN_VERIFY_EXAMPLES and similar flags are all 'True'.
 
- * Run the tests under Linux and Windows
+ * Run the tests under Linux, Windows and Mac OS
  * Use 2400 bps and 38400 bps
  * Use Modbus ASCII and Modbus RTU
 
  Sequence:
 
   * 38400 bps RTU
   * 38400 bps ASCII
@@ -91,37 +74,41 @@
 
 Manual testing in interactive mode (at the Python prompt)
 ----------------------------------------------------------
 Use a setting of 19200 bps, RTU mode and slave addess 1 for the DTB4824.
 Run these commands::
 
     import minimalmodbus
-    instrument = minimalmodbus.Instrument('/dev/ttyUSB0', 1, debug=True)  # Adjust if necessary.
-    instrument.read_register(4143)  # Read firmware version (address in hex is 0x102F)
-
 
+    # Adjust if necessary.
+    instrument = minimalmodbus.Instrument('/dev/ttyUSB0', 1, debug=True)
+    instrument.read_register(4143)  # Read firmware version (address in hex is 0x102F)
 """
+import argparse
 import os
 import statistics
 import sys
 import time
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, List, Optional, Tuple
+
+import serial
 
 sys.path.insert(0, "..")
-import minimalmodbus
+import minimalmodbus  # noqa: E402
 
 SLAVE_ADDRESS = 1
+ADDRESS_SETPOINT = 0x1001
 TIMEOUT = 0.3  # seconds. At least 0.3 seconds required for 2400 bits/s ASCII mode.
 DEFAULT_PORT_NAME = "/dev/ttyUSB0"
-DEFAULT_BAUDRATE = 38400  # baud (pretty much bits/s). Use 2400 or 38400 bits/s.
+DEFAULT_BAUDRATE = 38400  # baud (pretty much bit/s). Use 2400 or 38400 bit/s.
 
 
 def _box(description: Optional[str] = None, value: Any = None) -> None:
-    """Print a single line in a box"""
-    MAX_WIDTH = 85
+    """Print a single line in a box."""
+    MAX_WIDTH = 100
     DESCR_WIDTH = 30
     if description is None:
         print("#" * MAX_WIDTH)
     else:
         if value is None:
             line = "## {}".format(description)
         else:
@@ -130,34 +117,35 @@
         print(line)
 
 
 def show_test_settings(mode: str, baudrate: int, portname: str) -> None:
     _box()
     _box("Hardware test with Delta DTB4824")
     _box("Minimalmodbus version", minimalmodbus.__version__)
+    _box("Minimalmodbus path", os.path.abspath(minimalmodbus.__file__))
     _box(" ")
     _box("Platform", sys.platform)
     _box(
         "Python version",
         "{}.{}.{}".format(
             sys.version_info[0], sys.version_info[1], sys.version_info[2]
         ),
     )
     _box("Modbus mode", mode)
     _box("Baudrate (-b)", baudrate)
     _box("Port name (-D)", portname)
     _box("Slave address", SLAVE_ADDRESS)
-    _box("Timeout", TIMEOUT)
+    _box("Timeout (s)", TIMEOUT)
     _box("Full file path", os.path.abspath(__file__))
     _box()
     print("")
 
 
 def show_current_values(instr: minimalmodbus.Instrument) -> None:
-    """Read current values via Modbus"""
+    """Read current values via Modbus."""
     _box()
     _box("Current values")
     _box(" ")
     _box("Process value", instr.read_register(0x1000, 1))
     _box("Setpoint", instr.read_register(0x1001, 1))
     _box("Sensor type", instr.read_register(0x1004))
     _box("Heating/cooling selection", instr.read_register(0x1006))
@@ -185,45 +173,51 @@
 
 def verify_value_for_register(instr: minimalmodbus.Instrument, value: int) -> None:
     """Write and read back a value to a register, and validate result.
 
     Also read back several registers.
 
     Args:
-        instr: Instrument instance
-        value: Value to be written
+        * instr: Instrument instance
+        * value: Value to be written
     """
     START_READ_ADDR = 0x1000
-    ADDRESS_SETPOINT = 0x1001
+    NUMBER_OF_REGISTERS = 8
+    assert NUMBER_OF_REGISTERS > ADDRESS_SETPOINT - START_READ_ADDR
 
     instr.write_register(ADDRESS_SETPOINT, value)
     assert value == instr.read_register(ADDRESS_SETPOINT)
 
-    registers = instr.read_registers(START_READ_ADDR, 8)
+    registers = instr.read_registers(START_READ_ADDR, NUMBER_OF_REGISTERS)
     print(registers)
     assert value == registers[ADDRESS_SETPOINT - START_READ_ADDR]
 
 
 def verify_state_for_bits(instr: minimalmodbus.Instrument, state: int) -> None:
     """Write and read back a value to a bit, and validate result.
 
     Also read back several bits.
 
     Args:
-        instr: Instrument instance
-        state: Value to be written (0 or 1)
+        * instr: Instrument instance
+        * state: Value to be written (0 or 1)
     """
     START_READ_ADDR = 0x800
+    NUMBER_OF_BITS = 24
     ADDR_UNITSELECTOR = 0x811
     ADDR_LED_F = 0x804
     ADDR_LED_C = 0x805
+    assert (
+        NUMBER_OF_BITS
+        > max(ADDR_UNITSELECTOR, ADDR_LED_F, ADDR_LED_C) - START_READ_ADDR
+    )
 
     # Write and read selector for Celsius or Farenheit
     instr.write_bit(ADDR_UNITSELECTOR, state)  # 1=deg C, 0=deg F
-    bits = instr.read_bits(START_READ_ADDR, 24)
+    bits = instr.read_bits(START_READ_ADDR, NUMBER_OF_BITS)
     print(repr(bits))
     assert bits[ADDR_UNITSELECTOR - START_READ_ADDR] == state
     assert instr.read_bit(ADDR_UNITSELECTOR) == state
 
     # Read LED for Celcius
     assert bits[ADDR_LED_C - START_READ_ADDR] == state
     assert instr.read_bit(ADDR_LED_C) == state
@@ -233,25 +227,24 @@
     assert instr.read_bit(ADDR_LED_F) != state
 
 
 def verify_bits(instr: minimalmodbus.Instrument) -> None:
     NUMBER_OF_LOOPS = 5
 
     print("Verifying writing and reading bits")
+    print("Contents of 24 bit registers (18th column is temperature unit setting):")
     states = [0, 1] * NUMBER_OF_LOOPS
     for state in states:
         verify_state_for_bits(instr, state)
     print("Passed test for writing and reading bits\n")
 
 
 def verify_readonly_register(instr: minimalmodbus.Instrument) -> None:
-    """Verify that we detect the slave reported error when we
-    write to an read-only register.
-
-    """
+    """Verify that we detect the slave reported error when we write to an read-only
+    register."""
     ADDRESS_FIRMWARE_VERSION = 0x102F
     NEW_FIRMWARE_VERSION = 300
 
     print("Verify detecting a READONLY register (detect slave error)")
     did_report_error = False
     try:
         instr.write_register(ADDRESS_FIRMWARE_VERSION, NEW_FIRMWARE_VERSION)
@@ -261,57 +254,73 @@
     if not did_report_error:
         raise ValueError("Failed to detect READONLY register")
     print("Passed test for READONLY register\n")
 
 
 def verify_register(instr: minimalmodbus.Instrument) -> None:
     print("Verify writing and reading a register (and reading several registers)")
+    print("Contents of 8 registers (second column is setpoint register):")
     for value in range(250, 400, 10):  # Setpoint 25 to 40 deg C
         verify_value_for_register(instr, value)
     print("Passed test for writing and reading a register\n")
 
 
 def verify_two_instrument_instances(
     instr: minimalmodbus.Instrument, portname: str, mode: str, baudrate: int
 ) -> None:
-    ADDRESS_SETPOINT = 0x1001
-
     print("Verify using two instrument instances")
     instr2 = minimalmodbus.Instrument(portname, SLAVE_ADDRESS, mode=mode)
     if instr2.serial is None:
-        print("Failed to instanciate instr2")
-        return
+        raise ValueError("Failed to instanciate instr2")
     instr2.serial.timeout = TIMEOUT
 
     instr.read_register(ADDRESS_SETPOINT)
     instr2.read_register(ADDRESS_SETPOINT)
 
     print("... and verify port closure")
     instr.clear_buffers_before_each_transaction = False
     instr2.close_port_after_each_call = True
     instr.read_register(ADDRESS_SETPOINT)
     instr2.read_register(ADDRESS_SETPOINT)
     instr.read_register(ADDRESS_SETPOINT)
     instr2.read_register(ADDRESS_SETPOINT)
-    print("Passing test for using two instrument instances")
+    print("Passing test for using two instrument instances\n")
+
+
+def verify_external_instrument_instance(
+    portname: str, mode: str, baudrate: int
+) -> None:
+    print("Verify using external serial port instance")
+    extserial = serial.Serial(
+        port=portname,
+        baudrate=baudrate,
+        parity=serial.PARITY_NONE,
+        bytesize=8,
+        stopbits=1,
+        timeout=TIMEOUT,
+        write_timeout=2.0,
+    )
+
+    instr3 = minimalmodbus.Instrument(extserial, SLAVE_ADDRESS, mode=mode)
+    print("Setpoint", instr3.read_register(ADDRESS_SETPOINT))
+    print("Passing test for using external serial port instance\n")
 
 
 def measure_roundtrip_time(instr: minimalmodbus.Instrument) -> None:
     ADDR_SETPOINT = 0x1001
     SECONDS_TO_MILLISECONDS = 1000
     NUMBER_OF_VALUES = 100
     START_VALUE = 200
     STOP_VALUE = 500
     STEPSIZE = 5
     instrument_roundtrip_measurements: List[float] = []
 
     print("Measure request-response round trip time")
     if instr.serial is None:
-        print("Instrument.serial is None")
-        return
+        raise ValueError("Instrument.serial is None")
     print(
         "Setting the setpoint value {} times. Baudrate {} bits/s.".format(
             NUMBER_OF_VALUES, instr.serial.baudrate
         )
     )
 
     value = START_VALUE
@@ -324,72 +333,77 @@
         instr.write_register(ADDR_SETPOINT, value, functioncode=6)
         assert isinstance(instr.roundtrip_time, float)
         instrument_roundtrip_measurements.append(instr.roundtrip_time)
 
     time_per_value = (
         (time.time() - start_time) * float(SECONDS_TO_MILLISECONDS) / NUMBER_OF_VALUES
     )
-    print("Time per loop: {:0.1f} ms.".format(time_per_value))
+    print("Average measured time per loop: {:0.1f} ms.".format(time_per_value))
     print(
-        "Instrument-reported round trip time: {:0.1f} ms. Min {:0.1f} ms Max {:0.1f} ms\n".format(
+        "Instrument-reported round trip "
+        + "time: Mean {:0.1f} ms  Min {:0.1f} ms  Max {:0.1f} ms\n".format(
             statistics.mean(instrument_roundtrip_measurements)
             * SECONDS_TO_MILLISECONDS,
             min(instrument_roundtrip_measurements) * SECONDS_TO_MILLISECONDS,
             max(instrument_roundtrip_measurements) * SECONDS_TO_MILLISECONDS,
         )
     )
 
 
 def parse_commandline(argv: List[str]) -> Tuple[str, str, int]:
-    # TODO Use standard parsing of command line (now that we have dropped Python 2.6)
+    parser = argparse.ArgumentParser(
+        description="Run tests with a Delta DTB4824 instrument"
+    )
+    parser.add_argument("-a", action="store_true", help="Use ASCII mode")
+    parser.add_argument(
+        "-r", action="store_true", help="Use RTU mode (default). Overrides -a flag."
+    )
+    parser.add_argument(
+        "-b",
+        help="Baud rate. Defaults to %(default)s bit/s",
+        default=DEFAULT_BAUDRATE,
+        metavar="BAUD",
+        type=int,
+    )
+    parser.add_argument(
+        "-d",
+        help='Device name. Defaults to "%(default)s"',
+        default=DEFAULT_PORT_NAME,
+        metavar="DEVICE",
+        type=str,
+    )
+    arguments = parser.parse_args(args=argv[1:])
 
     mode = minimalmodbus.MODE_RTU
-    baudrate = DEFAULT_BAUDRATE
-    portname = DEFAULT_PORT_NAME
+    if arguments.a and not arguments.r:
+        mode = minimalmodbus.MODE_ASCII
 
-    for arg in argv:
-        if arg.startswith("-ascii"):
-            mode = minimalmodbus.MODE_ASCII
-
-        elif arg.startswith("-rtu"):
-            mode = minimalmodbus.MODE_RTU
-
-        elif arg.startswith("-b"):
-            if len(arg) < 3:
-                print("Wrong usage of the -b option. Use -b9600")
-                sys.exit()
-            baudrate = int(arg[2:])
-
-        elif arg.startswith("-D"):
-            if len(arg) < 3:
-                print("Wrong usage of the -D option. Use -D/dev/ttyUSB0 or -DCOM4")
-                sys.exit()
-            portname = arg[2:]
-
-    return portname, mode, baudrate
+    return arguments.d, mode, arguments.b
 
 
 def main() -> None:
     portname, mode, baudrate = parse_commandline(sys.argv)
     show_test_settings(mode, baudrate, portname)
 
     inst = minimalmodbus.Instrument(portname, SLAVE_ADDRESS, mode=mode)
     if inst.serial is None:
-        print("Instrument.serial is None")
-        return
+        raise ValueError("Instrument.serial is None")
+
     inst.serial.timeout = TIMEOUT
     inst.serial.baudrate = baudrate
 
     show_instrument_settings(inst)
     show_current_values(inst)
     measure_roundtrip_time(inst)
 
     verify_register(inst)
     verify_readonly_register(inst)
     verify_bits(inst)
     verify_two_instrument_instances(inst, portname, mode, baudrate)
+    verify_external_instrument_instance(portname, mode, baudrate)
+    verify_readonly_register(inst)
     print(" ")
     print("All tests did pass")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `minimalmodbus-2.0.1/tests/test_minimalmodbus.py` & `minimalmodbus-2.1.0/tests/test_minimalmodbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,99 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-#   Copyright 2019 Jonas Berg
+#   Copyright 2023 Jonas Berg
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-
 """
 
 .. moduleauthor:: Jonas Berg
 
 test_minimalmodbus: Unittests for the :mod:`minimalmodbus` module.
 
 For each function are these tests performed:
 
   * Known results
   * Invalid input value
   * Invalid input type
 
 This unittest suite uses a mock/dummy serial port from the module :mod:`dummy_serial`,
-so it is possible to test the functionality using previously recorded communication data.
+so it is possible to test the functionality using previously recorded
+communication data.
 
 With dummy responses, it is also possible to simulate errors in the communication
-from the slave. A few different types of communication errors are tested, as seen in this table.
+from the slave. A few different types of communication errors are tested, as seen
+in this table.
 
-=====================================  ===================== =================================
-Simulated response error               Tested using function Tested using Modbus function code
-=====================================  ===================== =================================
+=====================================  ===================== =========================
+Simulated response error               Tested using function Tested with function code
+=====================================  ===================== =========================
 No response                            read_bit              2
 Wrong CRC in response                  write_register        16
 Wrong slave address in response        write_register        16
 Wrong function code in response        write_register        16
 Slave indicates an error               write_register        16
 Wrong byte count in response           read_bit              2
 Wrong register address in response     write_register        16
 Wrong number of registers in response  write_bit             15
 Wrong number of registers in response  write_register        16
 Wrong write data in response           write_bit             5
 Wrong write data in response           write_register        6
-=====================================  ===================== =================================
+=====================================  ===================== =========================
 
 """
 __author__ = "Jonas Berg"
 __license__ = "Apache License, Version 2.0"
 
 import sys
 import time
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, Tuple, Type, Union
 import unittest
 
 sys.path.append(".")
 
-import tests.dummy_serial as dummy_serial
-import minimalmodbus
-from minimalmodbus import IllegalRequestError
-from minimalmodbus import InvalidResponseError
-from minimalmodbus import LocalEchoError
-from minimalmodbus import MasterReportedException
-from minimalmodbus import ModbusException
-from minimalmodbus import NegativeAcknowledgeError
-from minimalmodbus import NoResponseError
-from minimalmodbus import SlaveDeviceBusyError
-from minimalmodbus import SlaveReportedException
-
-from minimalmodbus import _Payloadformat
-from minimalmodbus import BYTEORDER_BIG
-from minimalmodbus import BYTEORDER_LITTLE
-from minimalmodbus import BYTEORDER_BIG_SWAP
-from minimalmodbus import BYTEORDER_LITTLE_SWAP
+import tests.dummy_serial as dummy_serial  # noqa: E402
+import minimalmodbus  # noqa: E402
+from minimalmodbus import IllegalRequestError  # noqa: E402
+from minimalmodbus import InvalidResponseError  # noqa: E402
+from minimalmodbus import NegativeAcknowledgeError  # noqa: E402
+from minimalmodbus import NoResponseError  # noqa: E402
+from minimalmodbus import SlaveDeviceBusyError  # noqa: E402
+from minimalmodbus import SlaveReportedException  # noqa: E402
+
+from minimalmodbus import _Payloadformat  # noqa: E402
+from minimalmodbus import BYTEORDER_BIG  # noqa: E402
+from minimalmodbus import BYTEORDER_BIG_SWAP  # noqa: E402
+from minimalmodbus import BYTEORDER_LITTLE  # noqa: E402
+from minimalmodbus import BYTEORDER_LITTLE_SWAP  # noqa: E402
 
 VERBOSITY = 0
-"""Verbosity level for the unit testing. Use value 0 or 2. Note that it only has an effect for Python 2.7 and above."""
+"""Verbosity level for the unit testing.
+
+Use value 0 or 2. Note that it only has an effect for Python 2.7 and above.
+"""
 
 SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES = False
 """Set this to :const:`True` for printing the error messages caught by assertRaises().
 
-If set to :const:`True`, any unintentional error messages raised during the processing of the command in :meth:`.assertRaises` are also caught (not counted). It will be printed in the short form, and will show no traceback.  It can also be useful to set :data:`VERBOSITY` = 2.
+If set to :const:`True`, any unintentional error messages raised during the
+processing of the command in :meth:`.assertRaises` are also caught (not counted).
+It will be printed in the short form, and will show no traceback.
+It can also be useful to set :data:`VERBOSITY` = 2.
 """
 
 _LARGE_NUMBER_OF_BYTES = 1000
 
 
 ###########################################################
 # For showing the error messages caught by assertRaises() #
@@ -101,65 +105,68 @@
     pass
 
 
 class ExtendedTestCase(unittest.TestCase):
     """Overriding the assertRaises() method to be able to print the error message.
 
     Use :data:`test_minimalmodbus.SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES` = :const:`True`
-    in order to use this option. It can also be useful to set :data:`test_minimalmodbus.VERBOSITY` = 2.
-
-    Based on https://stackoverflow.com/questions/8672754/how-to-show-the-error-messages-caught-by-assertraises-in-unittest-in-python2-7
+    in order to use this option. It can also be useful to set
+    :data:`test_minimalmodbus.VERBOSITY` = 2.
 
+    Based on https://stackoverflow.com/questions/8672754/
+    how-to-show-the-error-messages-caught-by-assertraises-in-unittest-in-python2-7
     """
 
     def assertRaises(  # type: ignore
         self,
         excClass: Union[Type[BaseException], Tuple[Type[BaseException], ...]],
         callableObj: Callable[..., Any],
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
-        """Prints the caught error message (if :data:`SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES` is :const:`True`)."""
+        """Prints the caught error message
+        (if :data:`SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES` is :const:`True`)."""
         if SHOW_ERROR_MESSAGES_FOR_ASSERTRAISES:
             try:
                 unittest.TestCase.assertRaises(
                     self, _NonexistantError, callableObj, *args, **kwargs
                 )
-            except:
-                minimalmodbus._print_out("\n    " + repr(sys.exc_info()[1]))
+            except Exception:
+                print("\n    " + repr(sys.exc_info()[1]))
         else:
             unittest.TestCase.assertRaises(self, excClass, callableObj, *args, **kwargs)
 
     def assertAlmostEqualRatio(
         self, first: float, second: float, epsilon: float = 1.000001
     ) -> None:
         """A function to compare floats, with ratio instead of "number_of_places".
 
         This is slightly different than the standard unittest.assertAlmostEqual()
 
         Args:
             * first: Input argument for comparison
             * second: Input argument for comparison
-            * epsilon: Largest allowed ratio of largest to smallest of the two input arguments
-
+            * epsilon: Largest allowed ratio of largest to smallest of the two
+              input arguments
         """
         if first == second:
             return
 
         if (first < 0 and second >= 0) or (first >= 0 and second < 0):
             raise AssertionError(
                 "The arguments have different signs: {0!r} and {1!r}".format(
                     first, second
                 )
             )
 
         ratio = max(first, second) / float(min(first, second))
         if ratio > epsilon:
             raise AssertionError(
-                "The arguments are not equal: {0!r} and {1!r}. Epsilon is {2!r}.".format(
+                "The arguments are not "
+                + "equal: {0!r} and {1!r}. Epsilon is {2!r}.".format(
                     first, second, epsilon
                 )
             )
 
 
 ##############################
 # Constants for type testing #
@@ -266,1438 +273,1607 @@
 
 
 class TestCreatePayload(ExtendedTestCase):
     def testKnownValues(self) -> None:
         # read_bit(61, functioncode=2)
         self.assertEqual(
             minimalmodbus._create_payload(
-                2, 61, None, 0, 0, 1, False, False, _Payloadformat.BIT
+                2, 61, None, 0, 0, 1, False, BYTEORDER_BIG, _Payloadformat.BIT
             ),
-            "\x00\x3D\x00\x01",
+            b"\x00\x3D\x00\x01",
         )
 
         # read_bit(62, functioncode=1)
         self.assertEqual(
             minimalmodbus._create_payload(
-                1, 62, None, 0, 0, 1, False, False, _Payloadformat.BIT
+                1, 62, None, 0, 0, 1, False, BYTEORDER_BIG, _Payloadformat.BIT
             ),
-            "\x00\x3E\x00\x01",
+            b"\x00\x3E\x00\x01",
         )
 
         # write_bit(71, 1, functioncode=5)
         self.assertEqual(
             minimalmodbus._create_payload(
-                5, 71, 1, 0, 0, 1, False, False, _Payloadformat.BIT
+                5, 71, 1, 0, 0, 1, False, BYTEORDER_BIG, _Payloadformat.BIT
             ),
-            "\x00\x47\xFF\x00",
+            b"\x00\x47\xFF\x00",
         )
 
         # read_bits(196, 22, functioncode=2)
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._create_payload(
-                2, 196, None, 0, 0, 22, False, False, _Payloadformat.BITS
+                2, 196, None, 0, 0, 22, False, BYTEORDER_BIG, _Payloadformat.BITS
             ),
-            "\x00\xC4\x00\x16",
+            b"\x00\xC4\x00\x16",
         )
 
         # read_bits(19, 19, functioncode=1)
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._create_payload(
-                1, 19, None, 0, 0, 19, False, False, _Payloadformat.BITS
+                1, 19, None, 0, 0, 19, False, BYTEORDER_BIG, _Payloadformat.BITS
             ),
-            "\x00\x13\x00\x13",
+            b"\x00\x13\x00\x13",
         )
 
         # write_bits(19, [1, 0, 1, 1, 0, 0, 1, 1, 1, 0])
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._create_payload(
                 15,
                 19,
                 [1, 0, 1, 1, 0, 0, 1, 1, 1, 0],
                 0,
                 0,
                 10,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.BITS,
             ),
-            "\x00\x13\x00\x0A\x02\xCD\x01",
+            b"\x00\x13\x00\x0A\x02\xCD\x01",
         )
 
         # read_register(289, 0, functioncode=3)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 289, None, 0, 1, 0, False, False, _Payloadformat.REGISTER
+                3, 289, None, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x01\x21\x00\x01",
+            b"\x01\x21\x00\x01",
         )
 
         # read_register(14, 0, functioncode=4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                4, 14, None, 0, 1, 0, False, False, _Payloadformat.REGISTER
+                4, 14, None, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x00\x0E\x00\x01",
+            b"\x00\x0E\x00\x01",
         )
 
         # write_register(35, 20, functioncode = 16)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 35, 20, 0, 1, 0, False, False, _Payloadformat.REGISTER
+                16, 35, 20, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x00\x23\x00\x01\x02\x00\x14",
+            b"\x00\x23\x00\x01\x02\x00\x14",
         )
 
         # write_register(45, 88, functioncode = 6)
         self.assertEqual(
             minimalmodbus._create_payload(
-                6, 45, 88, 0, 1, 0, False, False, _Payloadformat.REGISTER
+                6, 45, 88, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x00\x2D\x00\x58",
+            b"\x00\x2D\x00\x58",
         )
 
         # write_register(101, -5, signed=True)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 101, -5, 0, 1, 0, True, False, _Payloadformat.REGISTER
+                16, 101, -5, 0, 1, 0, True, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x00\x65\x00\x01\x02\xFF\xFB",
+            b"\x00\x65\x00\x01\x02\xFF\xFB",
         )
 
         # write_register(101, -5, 1, signed=True)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 101, -5, 1, 1, 0, True, False, _Payloadformat.REGISTER
+                16, 101, -5, 1, 1, 0, True, BYTEORDER_BIG, _Payloadformat.REGISTER
             ),
-            "\x00\x65\x00\x01\x02\xFF\xCE",
+            b"\x00\x65\x00\x01\x02\xFF\xCE",
         )
 
         # read_long(102)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 102, None, 0, 2, 0, False, False, _Payloadformat.LONG
+                3, 102, None, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x00\x66\x00\x02",
+            b"\x00\x66\x00\x02",
         )
 
         # read_long(102, functioncode=4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                4, 102, None, 0, 2, 0, False, False, _Payloadformat.LONG
+                4, 102, None, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x00\x66\x00\x02",
+            b"\x00\x66\x00\x02",
         )
 
         # read_long(256)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 256, None, 0, 2, 0, False, False, _Payloadformat.LONG
+                3, 256, None, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.LONG
+            ),
+            b"\x01\x00\x00\x02",
+        )
+        # read_long(256, number_of_registers=4)
+        self.assertEqual(
+            minimalmodbus._create_payload(
+                3, 256, None, 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x01\x00\x00\x02",
+            b"\x01\x00\x00\x04",
         )
 
         # write_long(102, 5)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 102, 5, 0, 2, 0, False, False, _Payloadformat.LONG
+                16, 102, 5, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x00\x66\x00\x02\x04\x00\x00\x00\x05",
+            b"\x00\x66\x00\x02\x04\x00\x00\x00\x05",
         )
 
         # write_long(102, 5,  signed=True)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 102, 5, 0, 2, 0, True, False, _Payloadformat.LONG
+                16, 102, 5, 0, 2, 0, True, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x00\x66\x00\x02\x04\x00\x00\x00\x05",
+            b"\x00\x66\x00\x02\x04\x00\x00\x00\x05",
         )
 
         # write_long(102, -5, signed=True)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 102, -5, 0, 2, 0, True, False, _Payloadformat.LONG
+                16, 102, -5, 0, 2, 0, True, BYTEORDER_BIG, _Payloadformat.LONG
+            ),
+            b"\x00\x66\x00\x02\x04\xFF\xFF\xFF\xFB",
+        )
+
+        # write_long(102, -5, signed=True, number_of_registers=4)
+        self.assertEqual(
+            minimalmodbus._create_payload(
+                16, 102, -5, 0, 4, 0, True, BYTEORDER_BIG, _Payloadformat.LONG
             ),
-            "\x00\x66\x00\x02\x04\xFF\xFF\xFF\xFB",
+            b"\x00\x66\x00\x04\x08\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFB",
         )
 
         # read_float(103, functioncode=3, number_of_registers=2)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 103, None, 0, 2, 0, False, False, _Payloadformat.FLOAT
+                3, 103, None, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.FLOAT
             ),
-            "\x00\x67\x00\x02",
+            b"\x00\x67\x00\x02",
         )
 
         # read_float(103, functioncode=3, number_of_registers=4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 103, None, 0, 4, 0, False, False, _Payloadformat.FLOAT
+                3, 103, None, 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.FLOAT
             ),
-            "\x00\x67\x00\x04",
+            b"\x00\x67\x00\x04",
         )
 
         # read_float(103, functioncode=4, number_of_registers=2)
         self.assertEqual(
             minimalmodbus._create_payload(
-                4, 103, None, 0, 2, 0, False, False, _Payloadformat.FLOAT
+                4, 103, None, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.FLOAT
             ),
-            "\x00\x67\x00\x02",
+            b"\x00\x67\x00\x02",
         )
 
         # write_float(103, 1.1, number_of_registers=2)   OK compare to recorded data
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 103, 1.1, 0, 2, 0, False, False, _Payloadformat.FLOAT
+                16, 103, 1.1, 0, 2, 0, False, BYTEORDER_BIG, _Payloadformat.FLOAT
             ),
-            "\x00\x67\x00\x02\x04\x3F\x8C\xCC\xCD",
+            b"\x00\x67\x00\x02\x04\x3F\x8C\xCC\xCD",
         )
 
         # write_float(103, 1.1, number_of_registers=4)   OK compare to recorded data
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 103, 1.1, 0, 4, 0, False, False, _Payloadformat.FLOAT
+                16, 103, 1.1, 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.FLOAT
             ),
-            "\x00\x67\x00\x04\x08\x3F\xF1\x99\x99\x99\x99\x99\x9A",
+            b"\x00\x67\x00\x04\x08\x3F\xF1\x99\x99\x99\x99\x99\x9A",
         )
 
         # read_string(104, 1)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 104, None, 0, 1, 0, False, False, _Payloadformat.STRING
+                3, 104, None, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.STRING
             ),
-            "\x00\x68\x00\x01",
+            b"\x00\x68\x00\x01",
         )
 
         # read_string(104, 4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 104, None, 0, 4, 0, False, False, _Payloadformat.STRING
+                3, 104, None, 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.STRING
             ),
-            "\x00\x68\x00\x04",
+            b"\x00\x68\x00\x04",
         )
 
         # read_string(104, 4, functioncode=4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                4, 104, None, 0, 4, 0, False, False, _Payloadformat.STRING
+                4, 104, None, 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.STRING
             ),
-            "\x00\x68\x00\x04",
+            b"\x00\x68\x00\x04",
         )
 
         # write_string(104, 'A', 1)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 104, "A", 0, 1, 0, False, False, _Payloadformat.STRING
+                16, 104, "A", 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.STRING
             ),
-            "\x00\x68\x00\x01\x02A ",
+            b"\x00\x68\x00\x01\x02A ",
         )
 
         # write_string(104, 'A', 4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 104, "A", 0, 4, 0, False, False, _Payloadformat.STRING
+                16, 104, "A", 0, 4, 0, False, BYTEORDER_BIG, _Payloadformat.STRING
             ),
-            "\x00\x68\x00\x04\x08A       ",
+            b"\x00\x68\x00\x04\x08A       ",
         )
 
         # write_string(104, 'ABCDEFGH', 4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 104, "ABCDEFGH", 0, 4, 0, False, False, _Payloadformat.STRING
+                16,
+                104,
+                "ABCDEFGH",
+                0,
+                4,
+                0,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.STRING,
             ),
-            "\x00\x68\x00\x04\x08ABCDEFGH",
+            b"\x00\x68\x00\x04\x08ABCDEFGH",
         )
 
         # read_registers(105, 1)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 105, None, 0, 1, 0, False, False, _Payloadformat.REGISTERS
+                3, 105, None, 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTERS
             ),
-            "\x00\x69\x00\x01",
+            b"\x00\x69\x00\x01",
         )
 
         # read_registers(105, 3)
         self.assertEqual(
             minimalmodbus._create_payload(
-                3, 105, None, 0, 3, 0, False, False, _Payloadformat.REGISTERS
+                3, 105, None, 0, 3, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTERS
             ),
-            "\x00\x69\x00\x03",
+            b"\x00\x69\x00\x03",
         )
 
         # read_registers(105, 7, functioncode=4)
         self.assertEqual(
             minimalmodbus._create_payload(
-                4, 105, None, 0, 7, 0, False, False, _Payloadformat.REGISTERS
+                4, 105, None, 0, 7, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTERS
             ),
-            "\x00\x69\x00\x07",
+            b"\x00\x69\x00\x07",
         )
 
         # write_registers(105, [2])
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 105, [2], 0, 1, 0, False, False, _Payloadformat.REGISTERS
+                16, 105, [2], 0, 1, 0, False, BYTEORDER_BIG, _Payloadformat.REGISTERS
             ),
-            "\x00\x69\x00\x01\x02\x00\x02",
+            b"\x00\x69\x00\x01\x02\x00\x02",
         )
 
         # write_registers(105, [2, 4, 8])
         self.assertEqual(
             minimalmodbus._create_payload(
-                16, 105, [2, 4, 8], 0, 3, 0, False, False, _Payloadformat.REGISTERS
+                16,
+                105,
+                [2, 4, 8],
+                0,
+                3,
+                0,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.REGISTERS,
             ),
-            "\x00\x69\x00\x03\x06\x00\x02\x00\x04\x00\x08",
+            b"\x00\x69\x00\x03\x06\x00\x02\x00\x04\x00\x08",
         )
 
     def testWrongValues(self) -> None:
         # NOTE: Most of the error checking is done in other methods
         self.assertRaises(
             ValueError,
             minimalmodbus._create_payload,
-            25,
+            25,  # Wrong on purpose
             104,
             "A",
             0,
             4,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.STRING,
         )
 
+        self.assertRaises(
+            ValueError,
+            minimalmodbus._create_payload,
+            15,
+            104,
+            "ABC",  # Wrong on purpose
+            0,
+            4,
+            0,
+            False,
+            BYTEORDER_BIG,
+            _Payloadformat.BITS,
+        )
+
+        self.assertRaises(
+            ValueError,
+            minimalmodbus._create_payload,
+            16,
+            104,
+            [1, 0, 1],  # Wrong on purpose
+            0,
+            1,
+            0,
+            False,
+            BYTEORDER_BIG,
+            _Payloadformat.BITS,  # Wrong on purpose
+        )
+
 
 class TestParsePayload(ExtendedTestCase):
     def testKnownValues(self) -> None:
-
         # read_bit(61, functioncode=2)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x01\x01", 2, 61, None, 0, 0, 1, False, False, _Payloadformat.BIT
+                b"\x01\x01",
+                2,
+                61,
+                None,
+                0,
+                0,
+                1,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.BIT,
             ),
             1,
         )
 
         # read_bit(62, functioncode=1)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x01\x00", 1, 62, None, 0, 0, 1, False, False, _Payloadformat.BIT
+                b"\x01\x00",
+                1,
+                62,
+                None,
+                0,
+                0,
+                1,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.BIT,
             ),
             0,
         )
 
         # write_bit(71, 1, functioncode=5)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00\x47\xff\x00", 5, 71, 1, 0, 0, 1, False, False, _Payloadformat.BIT
+                b"\x00\x47\xff\x00",
+                5,
+                71,
+                1,
+                0,
+                0,
+                1,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.BIT,
             ),
             None,
         )
 
         # write_bit(72, 1, functioncode=15)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00\x48\x00\x01", 15, 72, 1, 0, 0, 1, False, False, _Payloadformat.BIT
+                b"\x00\x48\x00\x01",
+                15,
+                72,
+                1,
+                0,
+                0,
+                1,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.BIT,
             ),
             None,
         )
 
         # read_bits(196, 22, functioncode=2)
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x03\xAC\xDB\x35",
+                b"\x03\xAC\xDB\x35",
                 2,
                 196,
                 None,
                 0,
                 0,
                 22,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.BITS,
             ),
             [0, 0, 1, 1, 0, 1, 0, 1, 1, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 1],
         )
 
         # read_bits(19, 19, functioncode=1)
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x03\xCD\x6B\x05",
+                b"\x03\xCD\x6B\x05",
                 1,
                 19,
                 None,
                 0,
                 0,
                 19,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.BITS,
             ),
             [1, 0, 1, 1, 0, 0, 1, 1, 1, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1],
         )
 
         # write_bits(19, [1, 0, 1, 1, 0, 0, 1, 1, 1, 0])
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00\x13\x00\x0A",
+                b"\x00\x13\x00\x0A",
                 15,
                 19,
                 [1, 0, 1, 1, 0, 0, 1, 1, 1, 0],
                 0,
                 0,
                 10,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.BITS,
             ),
             None,
         )
 
         # read_register(289, 0, functioncode=3)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x02\x03\x02",
+                b"\x02\x03\x02",
                 3,
                 289,
                 None,
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTER,
             ),
             770,
         )
 
         # read_register(14, 0, functioncode=4)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x02\x03\x70",
+                b"\x02\x03\x70",
                 4,
                 14,
                 None,
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTER,
             ),
             880,
         )
 
         # write_register(35, 20, functioncode = 16)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00#\x00\x01",
+                b"\x00#\x00\x01",
                 16,
                 35,
                 20,
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTER,
             ),
             None,
         )
 
         # write_register(45, 88, functioncode = 6)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00\x2d\x00\x58",
+                b"\x00\x2d\x00\x58",
                 6,
                 45,
                 88,
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTER,
             ),
             None,
         )
 
         # write_register(101, -5, signed=True)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00e\x00\x01",
+                b"\x00e\x00\x01",
                 16,
                 101,
                 -5,
                 0,
                 1,
                 0,
                 True,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTER,
             ),
             None,
         )
 
         # read_long(102)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x04\xff\xff\xff\xff",
+                b"\x04\xff\xff\xff\xff",
                 3,
                 102,
                 None,
                 0,
                 2,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.LONG,
             ),
             4294967295,
         )
 
         # read_long(102, signed=True)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x04\xff\xff\xff\xff",
+                b"\x04\xff\xff\xff\xff",
                 3,
                 102,
                 None,
                 0,
                 2,
                 0,
                 True,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.LONG,
             ),
             -1,
         )
 
         # write_long(102, 5)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00f\x00\x02", 16, 102, 5, 0, 2, 0, False, False, _Payloadformat.LONG
+                b"\x00f\x00\x02",
+                16,
+                102,
+                5,
+                0,
+                2,
+                0,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.LONG,
             ),
             None,
         )
 
         # write_long(102, -5, signed=True)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00f\x00\x02", 16, 102, -5, 0, 2, 0, True, False, _Payloadformat.LONG
+                b"\x00f\x00\x02",
+                16,
+                102,
+                -5,
+                0,
+                2,
+                0,
+                True,
+                BYTEORDER_BIG,
+                _Payloadformat.LONG,
             ),
             None,
         )
 
         # read_float(103, functioncode=3, number_of_registers=2)
         parsed_value = minimalmodbus._parse_payload(
-            "\x04\x3f\x80\x00\x00",
+            b"\x04\x3f\x80\x00\x00",
             3,
             103,
             None,
             0,
             2,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.FLOAT,
         )
         assert isinstance(parsed_value, float)
         self.assertAlmostEqual(
             parsed_value,
             1.0,
         )
 
         # read_float(103, functioncode=3, number_of_registers=4)
         parsed_value = minimalmodbus._parse_payload(
-            "\x08\xc0\x00\x00\x00\x00\x00\x00\x00",
+            b"\x08\xc0\x00\x00\x00\x00\x00\x00\x00",
             3,
             103,
             None,
             0,
             4,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.FLOAT,
         )
         assert isinstance(parsed_value, float)
         self.assertAlmostEqual(
             parsed_value,
             -2.0,
         )
 
         # read_float(103, functioncode=4, number_of_registers=2)
         parsed_value = minimalmodbus._parse_payload(
-            "\x04\x72\x38\x47\x25",
+            b"\x04\x72\x38\x47\x25",
             4,
             103,
             None,
             0,
             2,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.FLOAT,
         )
         assert isinstance(parsed_value, float)
         self.assertAlmostEqualRatio(
             parsed_value,
             3.65e30,
         )
 
         # write_float(103, 1.1, number_of_registers=2)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00g\x00\x02",
+                b"\x00g\x00\x02",
                 16,
                 103,
                 1.1,
                 0,
                 2,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.FLOAT,
             ),
             None,
         )
 
         # write_float(103, 1.1, number_of_registers=4)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00g\x00\x04",
+                b"\x00g\x00\x04",
                 16,
                 103,
                 1.1,
                 0,
                 4,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.FLOAT,
             ),
             None,
         )
 
         # read_string(104, 1)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x02AB", 3, 104, None, 0, 1, 0, False, False, _Payloadformat.STRING
+                b"\x02AB",
+                3,
+                104,
+                None,
+                0,
+                1,
+                0,
+                False,
+                BYTEORDER_BIG,
+                _Payloadformat.STRING,
             ),
             "AB",
         )
 
         # read_string(104, 4)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x08ABCDEFGH",
+                b"\x08ABCDEFGH",
                 3,
                 104,
                 None,
                 0,
                 4,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.STRING,
             ),
             "ABCDEFGH",
         )
 
         # write_string(104, 'A', 1)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00h\x00\x01",
+                b"\x00h\x00\x01",
                 16,
                 104,
                 "A",
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.STRING,
             ),
             None,
         )
 
         # write_string(104, 'A', 4)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00h\x00\x04",
+                b"\x00h\x00\x04",
                 16,
                 104,
                 "A",
                 0,
                 4,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.STRING,
             ),
             None,
         )
 
         # write_string(104, 'ABCDEFGH', 4)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00h\x00\x04",
+                b"\x00h\x00\x04",
                 16,
                 104,
                 "ABCDEFGH",
                 0,
                 4,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.STRING,
             ),
             None,
         )
 
         # read_registers(105, 1)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x02\x00\x10",
+                b"\x02\x00\x10",
                 3,
                 105,
                 None,
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTERS,
             ),
             [16],
         )
 
         # read_registers(105, 3)
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x06\x00\x10\x00\x20\x00\x40",
+                b"\x06\x00\x10\x00\x20\x00\x40",
                 3,
                 105,
                 None,
                 0,
                 3,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTERS,
             ),
             [16, 32, 64],
         )
 
         # write_registers(105, [2])
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00i\x00\x01",
+                b"\x00i\x00\x01",
                 16,
                 105,
                 [2],
                 0,
                 1,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTERS,
             ),
             None,
         )
 
         # write_registers(105, [2, 4, 8])
         self.assertEqual(
             minimalmodbus._parse_payload(
-                "\x00i\x00\x03",
+                b"\x00i\x00\x03",
                 16,
                 105,
                 [2, 4, 8],
                 0,
                 3,
                 0,
                 False,
-                False,
+                BYTEORDER_BIG,
                 _Payloadformat.REGISTERS,
             ),
             None,
         )
 
     def testInvalidPayloads(self) -> None:
-
         # read_bit(63, functioncode=2)  # Slave gives wrong byte count
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x02\x01",
+            b"\x02\x01",
             2,
             63,
             None,
             0,
             0,
             1,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.BIT,
         )
 
         # write_bit(73, 1, functioncode=15)  # Slave gives wrong number of registers
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x49\x00\x02",
+            b"\x00\x49\x00\x02",
             15,
             73,
             1,
             0,
             0,
             1,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.BIT,
         )
 
         # write_bit(74, 1, functioncode=5)  # Slave gives wrong write data
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x47\x00\x00",
+            b"\x00\x47\x00\x00",
             5,
             74,
             1,
             0,
             0,
             1,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.BIT,
         )
 
         # write_bit(73, 1, functioncode=15)  # Slave gives wrong number of registers
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x49\x00\x02",
+            b"\x00\x49\x00\x02",
             15,
             73,
             1,
             0,
             0,
             1,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.BIT,
         )
 
         # write_bit(74, 1, functioncode=5)  # Slave gives wrong write data (address)
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x47\x00\x00",
+            b"\x00\x47\x00\x00",
             5,
             74,
             1,
             0,
             0,
             1,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.BIT,
         )
 
         # read_bits(196, 22, functioncode=2)  # Wrong number of bits
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x03\xAC\xDB\x35",
+            b"\x03\xAC\xDB\x35",
             2,
             196,
             None,
             0,
             0,
             7,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
         # read_register(202, 0, functioncode=3)  # Slave gives too long response
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x02\x00\x00\x09",
+            b"\x02\x00\x00\x09",
             3,
             202,
             None,
             0,
             1,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
         # read_register(203, 0, functioncode=3)  # Slave gives too short response
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x02\x09",
+            b"\x02\x09",
             3,
             203,
             None,
             0,
             1,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
-        # write_register(52, 99, functioncode = 16)  # Slave gives wrong number of registers
+        # write_register(52, 99, functioncode = 16)
+        # Slave gives wrong number of registers
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x34\x00\x02",
+            b"\x00\x34\x00\x02",
             16,
             52,
             99,
             0,
             1,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
-        # write_register(53, 99, functioncode = 16)  # Slave gives wrong register address
+        # write_register(53, 99, functioncode = 16)
+        # Slave gives wrong register address
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x36\x00\x01",
+            b"\x00\x36\x00\x01",
             16,
             53,
             99,
             0,
             1,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
         # write_register(55, 99, functioncode = 6)  # Slave gives wrong write data
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x00\x36\x00\x01",
+            b"\x00\x36\x00\x01",
             6,
             55,
             99,
             0,
             1,
             0,
             False,
-            False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTER,
         )
 
         # read_registers(105, 3)  # wrong number of registers
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._parse_payload,
-            "\x06\x00\x10\x00\x20\x00\x40",
+            b"\x06\x00\x10\x00\x20\x00\x40",
             3,
             105,
             None,
             0,
             4,
             0,
             False,
+            BYTEORDER_BIG,
+            _Payloadformat.REGISTERS,
+        )
+
+        # wrong functioncode
+        self.assertRaises(
+            ValueError,
+            minimalmodbus._parse_payload,
+            b"ABC",
+            10,
+            105,
+            None,
+            0,
+            4,
+            0,
             False,
+            BYTEORDER_BIG,
             _Payloadformat.REGISTERS,
         )
 
+        # wrong functioncode and payload combination
+        self.assertRaises(
+            ValueError,
+            minimalmodbus._parse_payload,
+            b"\x01\x01",
+            1,
+            105,
+            None,
+            0,
+            1,
+            1,
+            False,
+            BYTEORDER_BIG,
+            _Payloadformat.REGISTER,  # Wrong on purpose
+        )
+        self.assertRaises(
+            ValueError,
+            minimalmodbus._parse_payload,
+            b"\x02\x00\x01",
+            3,
+            105,
+            None,
+            0,
+            1,
+            0,
+            False,
+            BYTEORDER_BIG,
+            _Payloadformat.BITS,  # Wrong on purpose
+        )
+
 
 class TestEmbedPayload(ExtendedTestCase):
-
-    knownValues = [
-        (2, 2, "rtu", "123", "\x02\x02123X\xc2"),
-        (1, 16, "rtu", "ABC", "\x01\x10ABC<E"),
-        (0, 5, "rtu", "hjl", "\x00\x05hjl\x8b\x9d"),
-        (1, 3, "rtu", "\x01\x02\x03", "\x01\x03\x01\x02\x03\t%"),
-        (1, 3, "ascii", "123", ":010331323366\r\n"),
-        (4, 5, "ascii", "\x01\x02\x03", ":0405010203F1\r\n"),
-        (2, 2, "ascii", "123", ":020231323366\r\n"),
+    known_values = [
+        (2, 2, "rtu", b"123", b"\x02\x02123X\xc2"),
+        (1, 16, "rtu", b"ABC", b"\x01\x10ABC<E"),
+        (0, 5, "rtu", b"hjl", b"\x00\x05hjl\x8b\x9d"),
+        (1, 3, "rtu", b"\x01\x02\x03", b"\x01\x03\x01\x02\x03\t%"),
+        (1, 3, "ascii", b"123", b":010331323366\r\n"),
+        (4, 5, "ascii", b"\x01\x02\x03", b":0405010203F1\r\n"),
+        (2, 2, "ascii", b"123", b":020231323366\r\n"),
     ]
 
     def testKnownValues(self) -> None:
         for (
             slaveaddress,
             functioncode,
             mode,
-            inputstring,
-            knownresult,
-        ) in self.knownValues:
-
+            inputpayload,
+            known_result,
+        ) in self.known_values:
             result = minimalmodbus._embed_payload(
-                slaveaddress, mode, functioncode, inputstring
+                slaveaddress, mode, functioncode, inputpayload
             )
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 256, "rtu", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, 256, "rtu", 16, b"ABC"
         )  # Wrong slave address
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, -1, "rtu", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, -1, "rtu", 16, b"ABC"
         )
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 256, "ascii", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, 256, "ascii", 16, b"ABC"
         )
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, -1, "ascii", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, -1, "ascii", 16, b"ABC"
         )
 
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "rtuu", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "rtuu", 16, b"ABC"
         )  # Wrong Modbus mode
-        self.assertRaises(ValueError, minimalmodbus._embed_payload, 1, "RTU", 16, "ABC")
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "ASCII", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "RTU", 16, b"ABC"
         )
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "asci", 16, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "ASCII", 16, b"ABC"
+        )
+        self.assertRaises(
+            ValueError, minimalmodbus._embed_payload, 1, "asci", 16, b"ABC"
         )
 
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "rtu", 222, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "rtu", 222, b"ABC"
         )  # Wrong function code
-        self.assertRaises(ValueError, minimalmodbus._embed_payload, 1, "rtu", -1, "ABC")
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "ascii", 222, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "rtu", -1, b"ABC"
+        )
+        self.assertRaises(
+            ValueError, minimalmodbus._embed_payload, 1, "ascii", 222, b"ABC"
         )
         self.assertRaises(
-            ValueError, minimalmodbus._embed_payload, 1, "ascii", -1, "ABC"
+            ValueError, minimalmodbus._embed_payload, 1, "ascii", -1, b"ABC"
         )
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._embed_payload, value, "rtu", 16, "ABC"
+                TypeError, minimalmodbus._embed_payload, value, "rtu", 16, b"ABC"
             )
             self.assertRaises(
-                TypeError, minimalmodbus._embed_payload, value, "ascii", 16, "ABC"
+                TypeError, minimalmodbus._embed_payload, value, "ascii", 16, b"ABC"
             )
             self.assertRaises(
-                TypeError, minimalmodbus._embed_payload, 1, "rtu", value, "ABC"
+                TypeError, minimalmodbus._embed_payload, 1, "rtu", value, b"ABC"
             )
             self.assertRaises(
-                TypeError, minimalmodbus._embed_payload, 1, "ascii", value, "ABC"
+                TypeError, minimalmodbus._embed_payload, 1, "ascii", value, b"ABC"
             )
         for value in _NOT_STRINGS:
             self.assertRaises(
-                TypeError, minimalmodbus._embed_payload, 1, value, 16, "ABC"
+                TypeError, minimalmodbus._embed_payload, 1, value, 16, b"ABC"
             )
+        for value in _NOT_BYTES:
             self.assertRaises(
                 TypeError, minimalmodbus._embed_payload, 1, "rtu", 16, value
             )
             self.assertRaises(
                 TypeError, minimalmodbus._embed_payload, 1, "ascii", 16, value
             )
 
 
 class TestExtractPayload(ExtendedTestCase):
-
-    knownValues = TestEmbedPayload.knownValues
+    known_values = TestEmbedPayload.known_values
 
     def testKnownValues(self) -> None:
         for (
             slaveaddress,
             functioncode,
             mode,
-            knownresult,
-            inputstring,
-        ) in self.knownValues:
+            known_result,
+            inputbytes,
+        ) in self.known_values:
             result = minimalmodbus._extract_payload(
-                inputstring, slaveaddress, mode, functioncode
+                inputbytes, slaveaddress, mode, functioncode
             )
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            "\x02\x02123X\xc3",
+            b"\x02\x02123X\xc3",
             2,
             "rtu",
             2,
         )  # Wrong CRC from slave
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":0202313233F1\r\n",
+            b":0202313233F1\r\n",
             2,
             "ascii",
             2,
         )  # Wrong LRC from slave
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._extract_payload,
-            "\x02\x82123q\x02",
+            b"\x02\x82123q\x02",
             2,
             "rtu",
             2,
         )  # Error indication from slave
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._extract_payload,
-            ":0282313233E6\r\n",
+            b":0282313233E6\r\n",
             2,
             "ascii",
             2,
         )
         self.assertRaises(
-            InvalidResponseError, minimalmodbus._extract_payload, "ABC", 2, "rtu", 2
+            InvalidResponseError, minimalmodbus._extract_payload, b"ABC", 2, "rtu", 2
         )  # Too short message from slave
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            "ABCDEFGH",
+            b"ABCDEFGH",
             2,
             "ascii",
             2,
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            "\x02\x72123B\x02",
+            b"\x02\x72123B\x02",
             2,
             "rtu",
             2,
         )  # Wrong functioncode from slave
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":020431323364\r\n",
+            b":020431323364\r\n",
             2,
             "ascii",
             2,
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            "020231323366\r\n",
+            b"020231323366\r\n",
             2,
             "ascii",
             2,
         )  # Missing ASCII header
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":020231323366",
+            b":020231323366",
             2,
             "ascii",
             2,
         )  # Wrong ASCII footer
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":020231323366\r",
+            b":020231323366\r",
             2,
             "ascii",
             2,
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":020231323366\n",
+            b":020231323366\n",
             2,
             "ascii",
             2,
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._extract_payload,
-            ":02023132366\r\n",
+            b":02023132366\r\n",
             2,
             "ascii",
             2,
         )  # Odd number of ASCII payload characters
 
         for value in [256, -1]:
             self.assertRaises(
                 ValueError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 value,
                 "rtu",
                 2,
             )  # Invalid slave address
         for value in [3, 95, 128]:
             self.assertRaises(
                 InvalidResponseError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 value,
                 "rtu",
                 2,
             )  # Wrong slave address
         for value in [128, 256, -1]:
             self.assertRaises(
                 ValueError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 "rtu",
                 value,
             )  # Invalid functioncode
         for value in [3, 95, 127]:
             self.assertRaises(
                 InvalidResponseError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 "rtu",
                 value,
             )  # Wrong functioncode
 
         for value_str in ["RTU", "ASCII", "asc", "", " "]:
             self.assertRaises(
                 ValueError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 value_str,
                 2,
             )  # Wrong mode
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(
                 TypeError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 value,
                 "rtu",
                 2,
             )  # Wrong slaveaddress type
             self.assertRaises(
                 TypeError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 value,
                 "ascii",
                 2,
             )
             self.assertRaises(
                 TypeError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 "rtu",
                 value,
             )  # Wrong functioncode type
             self.assertRaises(
                 TypeError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 "ascii",
                 value,
             )
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(
                 TypeError, minimalmodbus._extract_payload, value, 2, "rtu", 2
             )  # Wrong message
             self.assertRaises(
                 TypeError, minimalmodbus._extract_payload, value, 2, "ascii", 2
             )
+        for value in _NOT_STRINGS:
             self.assertRaises(
                 TypeError,
                 minimalmodbus._extract_payload,
-                "\x02\x02123X\xc2",
+                b"\x02\x02123X\xc2",
                 2,
                 value,
                 2,
             )  # Wrong mode
 
 
 class TestSanityEmbedExtractPayload(ExtendedTestCase):
-
-    knownValues = TestEmbedPayload.knownValues
+    known_values = TestEmbedPayload.known_values
 
     def testKnownValues(self) -> None:
-        for slaveaddress, functioncode, mode, payload, message in self.knownValues:
+        for slaveaddress, functioncode, mode, payload, _ in self.known_values:
             embeddedResult = minimalmodbus._embed_payload(
                 slaveaddress, mode, functioncode, payload
             )
             extractedResult = minimalmodbus._extract_payload(
                 embeddedResult, slaveaddress, mode, functioncode
             )
             self.assertEqual(extractedResult, payload)
 
     def testRange(self) -> None:
         for i in range(110):
-            payload = str(i)
+            payload = str(i).encode("ascii")
 
             embeddedResultRtu = minimalmodbus._embed_payload(2, "rtu", 6, payload)
             extractedResultRtu = minimalmodbus._extract_payload(
                 embeddedResultRtu, 2, "rtu", 6
             )
             self.assertEqual(extractedResultRtu, payload)
 
             embeddedResultAscii = minimalmodbus._embed_payload(2, "ascii", 6, payload)
             extractedResultAscii = minimalmodbus._extract_payload(
                 embeddedResultAscii, 2, "ascii", 6
             )
             self.assertEqual(extractedResultAscii, payload)
 
 
-############################################
-## Serial communication utility functions ##
-############################################
+##########################################
+# Serial communication utility functions #
+##########################################
 
 
 class TestPredictResponseSize(ExtendedTestCase):
-
-    knownValues = [
-        ("rtu", 1, "\x00\x3e\x00\x01", 6),
-        ("rtu", 1, "\x00\x3e\x00\x07", 6),
-        ("rtu", 1, "\x00\x3e\x00\x08", 6),
-        ("rtu", 1, "\x00\x3e\x00\x09", 7),
-        ("rtu", 2, "\x00\x3e\x00\x09", 7),
-        ("rtu", 3, "AB\x00\x07", 19),
-        ("rtu", 4, "AB\x00\x07", 19),
-        ("rtu", 4, "AB\x01\x07", 531),
-        ("rtu", 5, "\x00\x47\xff\x00", 8),
-        ("rtu", 6, "\x00\x47\xFF\xFF", 8),
-        ("rtu", 16, "\x00\x48\x00\x01\x01\x01", 8),
-        ("ascii", 1, "\x00\x3e\x00\x01", 13),
-        ("ascii", 1, "\x00\x3e\x00\x07", 13),
-        ("ascii", 1, "\x00\x3e\x00\x08", 13),
-        ("ascii", 1, "\x00\x3e\x00\x09", 15),
-        ("ascii", 3, "AB\x00\x07", 39),
-        ("ascii", 4, "AB\x00\x07", 39),
-        ("ascii", 4, "AB\x01\x07", 1063),
-        ("ascii", 5, "\x00\x47\xff\x00", 17),
-        ("ascii", 16, "\x00\x48\x00\x01\x01\x01", 17),
+    known_values = [
+        ("rtu", 1, b"\x00\x3e\x00\x01", 6),
+        ("rtu", 1, b"\x00\x3e\x00\x07", 6),
+        ("rtu", 1, b"\x00\x3e\x00\x08", 6),
+        ("rtu", 1, b"\x00\x3e\x00\x09", 7),
+        ("rtu", 2, b"\x00\x3e\x00\x09", 7),
+        ("rtu", 3, b"AB\x00\x07", 19),
+        ("rtu", 4, b"AB\x00\x07", 19),
+        ("rtu", 4, b"AB\x01\x07", 531),
+        ("rtu", 5, b"\x00\x47\xff\x00", 8),
+        ("rtu", 6, b"\x00\x47\xFF\xFF", 8),
+        ("rtu", 16, b"\x00\x48\x00\x01\x01\x01", 8),
+        ("ascii", 1, b"\x00\x3e\x00\x01", 13),
+        ("ascii", 1, b"\x00\x3e\x00\x07", 13),
+        ("ascii", 1, b"\x00\x3e\x00\x08", 13),
+        ("ascii", 1, b"\x00\x3e\x00\x09", 15),
+        ("ascii", 3, b"AB\x00\x07", 39),
+        ("ascii", 4, b"AB\x00\x07", 39),
+        ("ascii", 4, b"AB\x01\x07", 1063),
+        ("ascii", 5, b"\x00\x47\xff\x00", 17),
+        ("ascii", 16, b"\x00\x48\x00\x01\x01\x01", 17),
     ]
 
     def testKnownValues(self) -> None:
-        for mode, functioncode, payload_to_slave, knownvalue in self.knownValues:
+        for mode, functioncode, payload_to_slave, known_value in self.known_values:
             resultvalue = minimalmodbus._predict_response_size(
                 mode, functioncode, payload_to_slave
             )
-            self.assertEqual(resultvalue, knownvalue)
+            self.assertEqual(resultvalue, known_value)
 
     def testRecordedRtuMessages(self) -> None:
-        ## Use the dictionary where the key is the 'message', and the item is the 'response'
+        # Use the dictionary where the key is the 'message', and the
+        # item is the 'response'
         for message in GOOD_RTU_RESPONSES:
             slaveaddress = message[0]
             functioncode = message[1]
-            messagestring = str(message, encoding="latin1")
             payload_to_slave = minimalmodbus._extract_payload(
-                messagestring, slaveaddress, "rtu", functioncode
+                message, slaveaddress, "rtu", functioncode
             )
             result = minimalmodbus._predict_response_size(
                 "rtu", functioncode, payload_to_slave
             )
 
             responseFromSlave = GOOD_RTU_RESPONSES[message]
             self.assertEqual(result, len(responseFromSlave))
 
     def testRecordedAsciiMessages(self) -> None:
-        ## Use the dictionary where the key is the 'message', and the item is the 'response'
+        # Use the dictionary where the key is the 'message', and the item
+        # is the 'response'
         for message in GOOD_ASCII_RESPONSES:
             slaveaddress = int(message[1:3])
             functioncode = int(message[3:5])
-            messagestring = str(message, encoding="latin1")
             payload_to_slave = minimalmodbus._extract_payload(
-                messagestring, slaveaddress, "ascii", functioncode
+                message, slaveaddress, "ascii", functioncode
             )
             result = minimalmodbus._predict_response_size(
                 "ascii", functioncode, payload_to_slave
             )
 
             responseFromSlave = GOOD_ASCII_RESPONSES[message]
             self.assertEqual(result, len(responseFromSlave))
 
     def testWrongInputValue(self) -> None:
         # Wrong mode
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "asciiii", 6, "ABCD"
+            ValueError, minimalmodbus._predict_response_size, "asciiii", 6, b"ABCD"
         )
         # Wrong function code
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "ascii", 35, "ABCD"
+            ValueError, minimalmodbus._predict_response_size, "ascii", 35, b"ABCD"
         )
         # Wrong function code
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "rtu", 35, "ABCD"
+            ValueError, minimalmodbus._predict_response_size, "rtu", 35, b"ABCD"
         )
         # Too short message
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "ascii", 1, "ABC"
+            ValueError, minimalmodbus._predict_response_size, "ascii", 1, b"ABC"
         )
         # Too short message
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "rtu", 1, "ABC"
+            ValueError, minimalmodbus._predict_response_size, "rtu", 1, b"ABC"
         )
         # Too short message
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "ascii", 1, "AB"
+            ValueError, minimalmodbus._predict_response_size, "ascii", 1, b"AB"
         )
         # Too short message
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "ascii", 1, "A"
+            ValueError, minimalmodbus._predict_response_size, "ascii", 1, b"A"
         )
         # Too short message
         self.assertRaises(
-            ValueError, minimalmodbus._predict_response_size, "ascii", 1, ""
+            ValueError, minimalmodbus._predict_response_size, "ascii", 1, b""
         )
 
     def testWrongInputType(self) -> None:
         for value in _NOT_STRINGS:
             self.assertRaises(
-                TypeError, minimalmodbus._predict_response_size, value, 1, "ABCD"
+                TypeError, minimalmodbus._predict_response_size, value, 1, b"ABCD"
             )
+        for value in _NOT_BYTES:
             self.assertRaises(
                 TypeError, minimalmodbus._predict_response_size, "rtu", 1, value
             )
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._predict_response_size, "rtu", value, "ABCD"
+                TypeError, minimalmodbus._predict_response_size, "rtu", value, b"ABCD"
             )
 
 
 class TestCalculateMinimumSilentPeriod(ExtendedTestCase):
-
-    knownValues = [
+    known_values = [
         (2400, 0.016),
         (2400.0, 0.016),
         (4800, 0.008),
         (9600, 0.004),
         (19200, 0.002),
         (38400, 0.00175),
         (57600, 0.00175),
         (115200, 0.00175),
         (128000, 0.00175),
         (230400, 0.00175),
         (4000000, 0.00175),
     ]
 
     def testKnownValues(self) -> None:
-        for baudrate, knownresult in self.knownValues:
+        for baudrate, known_result in self.known_values:
             result = minimalmodbus._calculate_minimum_silent_period(baudrate)
             self.assertAlmostEqualRatio(
-                result, knownresult, 1.02
+                result, known_result, 1.02
             )  # Allow 2% deviation from listed known values
 
     def testWrongInputValue(self) -> None:
         for value in [-2400, -2400.0, -1, -0.5, 0, 0.5, 0.9]:
             self.assertRaises(
                 ValueError, minimalmodbus._calculate_minimum_silent_period, value
             )
@@ -1710,346 +1886,346 @@
 
 
 ##############################
 # String and num conversions #
 ##############################
 
 
-class TestNumToOneByteString(ExtendedTestCase):
-
-    knownValues = [
-        (0, "\x00"),
-        (7, "\x07"),
-        (255, "\xff"),
+class TestNumToOneByte(ExtendedTestCase):
+    known_values = [
+        (0, b"\x00"),
+        (7, b"\x07"),
+        (255, b"\xff"),
     ]
 
     def testKnownValues(self) -> None:
-        for inputvalue, knownstring in self.knownValues:
-            resultstring = minimalmodbus._num_to_onebyte_string(inputvalue)
-            self.assertEqual(resultstring, knownstring)
+        for inputvalue, knownbyte in self.known_values:
+            result = minimalmodbus._num_to_one_byte(inputvalue)
+            self.assertEqual(result, knownbyte)
 
     def testKnownLoop(self) -> None:
         for value in range(256):
-            knownstring = chr(value)
-            resultstring = minimalmodbus._num_to_onebyte_string(value)
-            self.assertEqual(resultstring, knownstring)
+            knownbyte = value.to_bytes(1, "little")
+            result = minimalmodbus._num_to_one_byte(value)
+            self.assertEqual(result, knownbyte)
 
     def testWrongInput(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._num_to_onebyte_string, -1)
-        self.assertRaises(ValueError, minimalmodbus._num_to_onebyte_string, 256)
+        self.assertRaises(ValueError, minimalmodbus._num_to_one_byte, -1)
+        self.assertRaises(ValueError, minimalmodbus._num_to_one_byte, 256)
 
     def testWrongType(self) -> None:
         for value in _NOT_INTERGERS:
-            self.assertRaises(TypeError, minimalmodbus._num_to_onebyte_string, value)
-
+            self.assertRaises(TypeError, minimalmodbus._num_to_one_byte, value)
 
-class TestNumToTwoByteString(ExtendedTestCase):
 
-    knownValues = [
-        (0.0, 0, False, False, "\x00\x00"),  # Range 0-65535
-        (0, 0, False, False, "\x00\x00"),
-        (0, 0, True, False, "\x00\x00"),
-        (77.0, 1, False, False, "\x03\x02"),
-        (77.0, 1, True, False, "\x02\x03"),
-        (770, 0, False, False, "\x03\x02"),
-        (770, 0, True, False, "\x02\x03"),
-        (65535, 0, False, False, "\xff\xff"),
-        (65535, 0, True, False, "\xff\xff"),
-        (770, 0, False, True, "\x03\x02"),  # Range -32768 to 32767
-        (77.0, 1, False, True, "\x03\x02"),
-        (0.0, 0, False, True, "\x00\x00"),
-        (0.0, 3, False, True, "\x00\x00"),
-        (-1, 0, False, True, "\xff\xff"),
-        (-1, 1, False, True, "\xff\xf6"),
-        (-77, 0, False, True, "\xff\xb3"),
-        (-770, 0, False, True, "\xfc\xfe"),
-        (-77, 1, False, True, "\xfc\xfe"),
-        (-32768, 0, False, True, "\x80\x00"),
-        (32767, 0, False, True, "\x7f\xff"),
+class TestNumToTwoBytes(ExtendedTestCase):
+    known_values = [
+        (0.0, 0, False, False, b"\x00\x00"),  # Range 0-65535
+        (0, 0, False, False, b"\x00\x00"),
+        (0, 0, True, False, b"\x00\x00"),
+        (77.0, 1, False, False, b"\x03\x02"),
+        (77.0, 1, True, False, b"\x02\x03"),
+        (770, 0, False, False, b"\x03\x02"),
+        (770, 0, True, False, b"\x02\x03"),
+        (65535, 0, False, False, b"\xff\xff"),
+        (65535, 0, True, False, b"\xff\xff"),
+        (770, 0, False, True, b"\x03\x02"),  # Range -32768 to 32767
+        (77.0, 1, False, True, b"\x03\x02"),
+        (0.0, 0, False, True, b"\x00\x00"),
+        (0.0, 3, False, True, b"\x00\x00"),
+        (-1, 0, False, True, b"\xff\xff"),
+        (-1, 1, False, True, b"\xff\xf6"),
+        (-77, 0, False, True, b"\xff\xb3"),
+        (-770, 0, False, True, b"\xfc\xfe"),
+        (-77, 1, False, True, b"\xfc\xfe"),
+        (-32768, 0, False, True, b"\x80\x00"),
+        (32767, 0, False, True, b"\x7f\xff"),
     ]
 
     def testKnownValues(self) -> None:
         for (
             inputvalue,
             number_of_decimals,
             lsb_first,
             signed,
-            knownstring,
-        ) in self.knownValues:
-            resultstring = minimalmodbus._num_to_twobyte_string(
+            known_bytes,
+        ) in self.known_values:
+            resultbytes = minimalmodbus._num_to_two_bytes(
                 inputvalue, number_of_decimals, lsb_first, signed
             )
-            self.assertEqual(resultstring, knownstring)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
         for lsb_first in [False, True]:
             # Range 0-65535
             self.assertRaises(
-                ValueError, minimalmodbus._num_to_twobyte_string, 77, -1, lsb_first
+                ValueError, minimalmodbus._num_to_two_bytes, 77, -1, lsb_first
             )
             self.assertRaises(
-                ValueError, minimalmodbus._num_to_twobyte_string, 77, 11, lsb_first
+                ValueError, minimalmodbus._num_to_two_bytes, 77, 11, lsb_first
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 77000,
                 0,
                 lsb_first,
             )  # Gives DeprecationWarning instead of ValueError for Python 2.6
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 65536,
                 0,
                 lsb_first,
             )
             self.assertRaises(
-                ValueError, minimalmodbus._num_to_twobyte_string, 77, 4, lsb_first
+                ValueError, minimalmodbus._num_to_two_bytes, 77, 4, lsb_first
             )
             self.assertRaises(
-                ValueError, minimalmodbus._num_to_twobyte_string, -1, 0, lsb_first
+                ValueError, minimalmodbus._num_to_two_bytes, -1, 0, lsb_first
             )
             self.assertRaises(
-                ValueError, minimalmodbus._num_to_twobyte_string, -77, 1, lsb_first
+                ValueError, minimalmodbus._num_to_two_bytes, -77, 1, lsb_first
             )
 
             # Range -32768 to 32767
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 77,
                 -1,
                 lsb_first,
                 True,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 -77000,
                 0,
                 lsb_first,
                 True,
-            )  # Gives DeprecationWarning instead of ValueError for Python 2.6
+            )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 -32769,
                 0,
                 lsb_first,
                 True,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 32768,
                 0,
                 lsb_first,
                 True,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 77000,
                 0,
                 lsb_first,
                 True,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 77,
                 4,
                 lsb_first,
                 True,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._num_to_twobyte_string,
+                minimalmodbus._num_to_two_bytes,
                 -77,
                 4,
                 lsb_first,
                 True,
             )
 
     def testWrongInputType(self) -> None:
+        value: Any = None
         for value in _NOT_NUMERICALS:
             self.assertRaises(
-                TypeError, minimalmodbus._num_to_twobyte_string, value, 1, False, False
+                TypeError, minimalmodbus._num_to_two_bytes, value, 1, False, False
             )
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._num_to_twobyte_string, 77, value, False, False
+                TypeError, minimalmodbus._num_to_two_bytes, 77, value, False, False
             )
         for value in _NOT_BOOLEANS:
             self.assertRaises(
-                TypeError, minimalmodbus._num_to_twobyte_string, 77, 1, value, False
+                TypeError, minimalmodbus._num_to_two_bytes, 77, 1, value, False
             )
             self.assertRaises(
-                TypeError, minimalmodbus._num_to_twobyte_string, 77, 1, False, value
+                TypeError, minimalmodbus._num_to_two_bytes, 77, 1, False, value
             )
 
 
-class TestTwoByteStringToNum(ExtendedTestCase):
-
-    knownValues = TestNumToTwoByteString.knownValues
+class TestTwoBytesToNum(ExtendedTestCase):
+    known_values = TestNumToTwoBytes.known_values
 
     def testKnownValues(self) -> None:
         for (
-            knownvalue,
+            known_value,
             number_of_decimals,
             lsb_first,
             signed,
-            bytestring,
-        ) in self.knownValues:
+            inputbytes,
+        ) in self.known_values:
             if not lsb_first:
-                resultvalue = minimalmodbus._twobyte_string_to_num(
-                    bytestring, number_of_decimals, signed
+                resultvalue = minimalmodbus._two_bytes_to_num(
+                    inputbytes, number_of_decimals, signed
                 )
-                self.assertEqual(resultvalue, knownvalue)
+                self.assertEqual(resultvalue, known_value)
 
     def testWrongInputValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._twobyte_string_to_num, "ABC", 1)
-        self.assertRaises(ValueError, minimalmodbus._twobyte_string_to_num, "A", 1)
-        self.assertRaises(ValueError, minimalmodbus._twobyte_string_to_num, "AB", -1)
-        self.assertRaises(ValueError, minimalmodbus._twobyte_string_to_num, "AB", 11)
+        self.assertRaises(ValueError, minimalmodbus._two_bytes_to_num, b"ABC", 1)
+        self.assertRaises(ValueError, minimalmodbus._two_bytes_to_num, b"A", 1)
+        self.assertRaises(ValueError, minimalmodbus._two_bytes_to_num, b"AB", -1)
+        self.assertRaises(ValueError, minimalmodbus._two_bytes_to_num, b"AB", 11)
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._twobyte_string_to_num, value, 1)
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._two_bytes_to_num, value, 1)
         for value in _NOT_INTERGERS:
-            self.assertRaises(
-                TypeError, minimalmodbus._twobyte_string_to_num, "AB", value
-            )
+            self.assertRaises(TypeError, minimalmodbus._two_bytes_to_num, b"AB", value)
         for value in _NOT_BOOLEANS:
             self.assertRaises(
-                TypeError, minimalmodbus._twobyte_string_to_num, "\x03\x02", 1, value
+                TypeError, minimalmodbus._two_bytes_to_num, b"\x03\x02", 1, value
             )
 
 
-class TestSanityTwoByteString(ExtendedTestCase):
-
-    knownValues = TestNumToTwoByteString.knownValues
+class TestSanityTwoBytes(ExtendedTestCase):
+    known_values = TestNumToTwoBytes.known_values
 
     def testSanity(self) -> None:
         for (
             value,
             number_of_decimals,
             lsb_first,
             signed,
-            bytestring,
-        ) in self.knownValues:
+            _,
+        ) in self.known_values:
             if not lsb_first:
-                resultvalue = minimalmodbus._twobyte_string_to_num(
-                    minimalmodbus._num_to_twobyte_string(
+                resultvalue = minimalmodbus._two_bytes_to_num(
+                    minimalmodbus._num_to_two_bytes(
                         value, number_of_decimals, lsb_first, signed
                     ),
                     number_of_decimals,
                     signed,
                 )
                 self.assertEqual(resultvalue, value)
 
         for value in range(0x10000):
-            resultvalue = minimalmodbus._twobyte_string_to_num(
-                minimalmodbus._num_to_twobyte_string(value)
+            resultvalue = minimalmodbus._two_bytes_to_num(
+                minimalmodbus._num_to_two_bytes(value)
             )
             self.assertEqual(resultvalue, value)
 
 
-class TestBytestringToBits(ExtendedTestCase):
-
-    knownValues = [
-        ("\x00", 1, [0]),
-        ("\x01", 1, [1]),
-        ("\x02", 2, [0, 1]),
-        ("\x04", 3, [0, 0, 1]),
-        ("\x08", 4, [0, 0, 0, 1]),
-        ("\x10", 5, [0, 0, 0, 0, 1]),
-        ("\x20", 6, [0, 0, 0, 0, 0, 1]),
-        ("\x40", 7, [0, 0, 0, 0, 0, 0, 1]),
-        ("\x80", 8, [0, 0, 0, 0, 0, 0, 0, 1]),
-        ("\x00\x01", 9, [0, 0, 0, 0, 0, 0, 0, 0, 1]),
-        ("\x00\x02", 10, [0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
-        ("\x00\x00\x01", 17, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
-        ("\x00\x00\x02", 18, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
-        ("\x00\x00\x02", 19, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0]),
-        ("\x01", 1, [1]),
-        ("\x01", 2, [1, 0]),
-        ("\x01", 3, [1, 0, 0]),
-        ("\x01", 4, [1, 0, 0, 0]),
-        ("\x01", 5, [1, 0, 0, 0, 0]),
-        ("\x01", 6, [1, 0, 0, 0, 0, 0]),
-        ("\x01", 7, [1, 0, 0, 0, 0, 0, 0]),
-        ("\x01", 8, [1, 0, 0, 0, 0, 0, 0, 0]),
-        ("\x01\x00", 9, [1, 0, 0, 0, 0, 0, 0, 0, 0]),
-        ("\x01\x00", 10, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
-        ("\x01\x00", 16, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
-        ("\x01\x00\x00", 17, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
-        ("\x01\x00\x00", 18, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
+class TestBytesToBits(ExtendedTestCase):
+    known_values = [
+        (b"\x00", 1, [0]),
+        (b"\x01", 1, [1]),
+        (b"\x02", 2, [0, 1]),
+        (b"\x03", 2, [1, 1]),
+        (b"\x04", 3, [0, 0, 1]),
+        (b"\x08", 4, [0, 0, 0, 1]),
+        (b"\x10", 5, [0, 0, 0, 0, 1]),
+        (b"\x20", 6, [0, 0, 0, 0, 0, 1]),
+        (b"\x40", 7, [0, 0, 0, 0, 0, 0, 1]),
+        (b"\x80", 8, [0, 0, 0, 0, 0, 0, 0, 1]),
+        (b"\x00\x01", 9, [0, 0, 0, 0, 0, 0, 0, 0, 1]),
+        (b"\x00\x02", 10, [0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
+        (b"\x00\x00\x01", 17, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
+        (b"\x00\x00\x02", 18, [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1]),
+        (
+            b"\x00\x00\x02",
+            19,
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
+        ),
+        (b"\x01", 1, [1]),
+        (b"\x01", 2, [1, 0]),
+        (b"\x01", 3, [1, 0, 0]),
+        (b"\x01", 4, [1, 0, 0, 0]),
+        (b"\x01", 5, [1, 0, 0, 0, 0]),
+        (b"\x01", 6, [1, 0, 0, 0, 0, 0]),
+        (b"\x01", 7, [1, 0, 0, 0, 0, 0, 0]),
+        (b"\x01", 8, [1, 0, 0, 0, 0, 0, 0, 0]),
+        (b"\x01\x00", 9, [1, 0, 0, 0, 0, 0, 0, 0, 0]),
+        (b"\x01\x00", 10, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
+        (b"\x01\x00", 16, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
+        (b"\x01\x00\x00", 17, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
+        (b"\x01\x00\x00", 18, [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]),
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
-        ("\xCD\x6B\x05", 19, [1, 0, 1, 1, 0, 0, 1, 1, 1, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1]),
+        (
+            b"\xCD\x6B\x05",
+            19,
+            [1, 0, 1, 1, 0, 0, 1, 1, 1, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1],
+        ),
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         (
-            "\xAC\xDB\x35",
+            b"\xAC\xDB\x35",
             22,
             [0, 0, 1, 1, 0, 1, 0, 1, 1, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 1],
         ),
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
-        ("\xCD\x01", 10, [1, 0, 1, 1, 0, 0, 1, 1, 1, 0]),
+        (b"\xCD\x01", 10, [1, 0, 1, 1, 0, 0, 1, 1, 1, 0]),
     ]
 
     def testKnownValues(self) -> None:
-        for bytestring, number_of_bits, expected_result in self.knownValues:
+        for inputbytes, number_of_bits, expected_result in self.known_values:
             assert len(expected_result) == number_of_bits
-            result = minimalmodbus._bytestring_to_bits(bytestring, number_of_bits)
+            result = minimalmodbus._bytes_to_bits(inputbytes, number_of_bits)
             self.assertEqual(result, expected_result)
 
     def testWrongValues(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_bits, "\x01\x02", 3)
-
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_bits, b"\x01\x02", 3)
 
-class TestBitsToBytestring(ExtendedTestCase):
 
-    knownValues = TestBytestringToBits.knownValues
+class TestBitsToBytes(ExtendedTestCase):
+    known_values = TestBytesToBits.known_values
 
     def testKnownValues(self) -> None:
-        for knownresult, __, bitlist in self.knownValues:
-            result = minimalmodbus._bits_to_bytestring(bitlist)
-            self.assertEqual(result, knownresult)
+        for known_result, __, bitlist in self.known_values:
+            result = minimalmodbus._bits_to_bytes(bitlist)
+            self.assertEqual(result, known_result)
 
     def testWrongValues(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._bits_to_bytestring, [1, 0, 3])
-        self.assertRaises(TypeError, minimalmodbus._bits_to_bytestring, 1)
+        self.assertRaises(ValueError, minimalmodbus._bits_to_bytes, [1, 0, 3])
+        self.assertRaises(TypeError, minimalmodbus._bits_to_bytes, 1)
 
 
-class TestBitToBytestring(ExtendedTestCase):
-
-    knownValues = [
-        (0, "\x00\x00"),
-        (1, "\xff\x00"),
+class TestBitToBytes(ExtendedTestCase):
+    known_values = [
+        (0, b"\x00\x00"),
+        (1, b"\xff\x00"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, knownresult in self.knownValues:
-            resultvalue = minimalmodbus._bit_to_bytestring(value)
-            self.assertEqual(resultvalue, knownresult)
+        for value, known_result in self.known_values:
+            resultvalue = minimalmodbus._bit_to_bytes(value)
+            self.assertEqual(resultvalue, known_result)
 
     def testWrongValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._bit_to_bytestring, 2)
-        self.assertRaises(ValueError, minimalmodbus._bit_to_bytestring, 222)
-        self.assertRaises(ValueError, minimalmodbus._bit_to_bytestring, -1)
+        self.assertRaises(ValueError, minimalmodbus._bit_to_bytes, 2)
+        self.assertRaises(ValueError, minimalmodbus._bit_to_bytes, 222)
+        self.assertRaises(ValueError, minimalmodbus._bit_to_bytes, -1)
 
     def testValueNotInteger(self) -> None:
         for value in _NOT_INTERGERS:
-            self.assertRaises(TypeError, minimalmodbus._bit_to_bytestring, value)
+            self.assertRaises(TypeError, minimalmodbus._bit_to_bytes, value)
 
 
 class TestCalculateNumberOfBytesForBits(ExtendedTestCase):
-
-    knownValues = [
+    known_values = [
         (0, 0),
         (1, 1),
         (2, 1),
         (3, 1),
         (4, 1),
         (5, 1),
         (6, 1),
@@ -2063,648 +2239,637 @@
         (14, 2),
         (15, 2),
         (16, 2),
         (17, 3),
     ]
 
     def testKnownValues(self) -> None:
-        for bits, knownresult in self.knownValues:
+        for bits, known_result in self.known_values:
             resultvalue = minimalmodbus._calculate_number_of_bytes_for_bits(bits)
-            self.assertEqual(resultvalue, knownresult)
-
+            self.assertEqual(resultvalue, known_result)
 
-class TestLongToBytestring(ExtendedTestCase):
 
-    knownValues = [
-        (0, True, BYTEORDER_BIG, "\x00\x00\x00\x00"),
-        (1, False, BYTEORDER_BIG, "\x00\x00\x00\x01"),
-        (1, True, BYTEORDER_BIG, "\x00\x00\x00\x01"),
-        (2, False, BYTEORDER_BIG, "\x00\x00\x00\x02"),
-        (2, True, BYTEORDER_BIG, "\x00\x00\x00\x02"),
-        (75000, False, BYTEORDER_BIG, "\x00\x01\x24\xf8"),
-        (75000, True, BYTEORDER_BIG, "\x00\x01\x24\xf8"),
-        (1000000, False, BYTEORDER_BIG, "\x00\x0f\x42\x40"),
-        (1000000, True, BYTEORDER_BIG, "\x00\x0f\x42\x40"),
-        (2147483647, False, BYTEORDER_BIG, "\x7f\xff\xff\xff"),
-        (2147483647, True, BYTEORDER_BIG, "\x7f\xff\xff\xff"),
-        (2147483648, False, BYTEORDER_BIG, "\x80\x00\x00\x00"),
-        (4294967295, False, BYTEORDER_BIG, "\xff\xff\xff\xff"),
-        (-1, True, BYTEORDER_BIG, "\xff\xff\xff\xff"),
-        (-2147483648, True, BYTEORDER_BIG, "\x80\x00\x00\x00"),
-        (-200000000, True, BYTEORDER_BIG, "\xf4\x14\x3e\x00"),
+class TestLongToBytes(ExtendedTestCase):
+    known_values = [
+        (0, 2, True, BYTEORDER_BIG, b"\x00\x00\x00\x00"),
+        (1, 2, False, BYTEORDER_BIG, b"\x00\x00\x00\x01"),
+        (1, 2, True, BYTEORDER_BIG, b"\x00\x00\x00\x01"),
+        (2, 2, False, BYTEORDER_BIG, b"\x00\x00\x00\x02"),
+        (2, 2, True, BYTEORDER_BIG, b"\x00\x00\x00\x02"),
+        (75000, 2, False, BYTEORDER_BIG, b"\x00\x01\x24\xf8"),
+        (75000, 2, True, BYTEORDER_BIG, b"\x00\x01\x24\xf8"),
+        (1000000, 2, False, BYTEORDER_BIG, b"\x00\x0f\x42\x40"),
+        (1000000, 2, True, BYTEORDER_BIG, b"\x00\x0f\x42\x40"),
+        (2147483647, 2, False, BYTEORDER_BIG, b"\x7f\xff\xff\xff"),
+        (2147483647, 2, True, BYTEORDER_BIG, b"\x7f\xff\xff\xff"),
+        (2147483648, 2, False, BYTEORDER_BIG, b"\x80\x00\x00\x00"),
+        (4294967295, 2, False, BYTEORDER_BIG, b"\xff\xff\xff\xff"),
+        (-1, 2, True, BYTEORDER_BIG, b"\xff\xff\xff\xff"),
+        (-2147483648, 2, True, BYTEORDER_BIG, b"\x80\x00\x00\x00"),
+        (-200000000, 2, True, BYTEORDER_BIG, b"\xf4\x14\x3e\x00"),
         # Example from https://www.simplymodbus.ca/FAQ.htm
-        (2923517522, False, BYTEORDER_BIG, "\xAE\x41\x56\x52"),
+        (2923517522, 2, False, BYTEORDER_BIG, b"\xAE\x41\x56\x52"),
         # Example from https://www.simplymodbus.ca/FAQ.htm
-        (-1371449774, True, BYTEORDER_BIG, "\xAE\x41\x56\x52"),
+        (-1371449774, 2, True, BYTEORDER_BIG, b"\xAE\x41\x56\x52"),
         # Example from https://www.simplymodbus.ca/FAQ.htm
-        (2923517522, False, BYTEORDER_LITTLE, "\x52\x56\x41\xAE"),
+        (2923517522, 2, False, BYTEORDER_LITTLE, b"\x52\x56\x41\xAE"),
         # Example from https://www.simplymodbus.ca/FAQ.htm (the byteorder is not named)
-        (2923517522, False, BYTEORDER_LITTLE_SWAP, "\x56\x52\xAE\x41"),
+        (2923517522, 2, False, BYTEORDER_LITTLE_SWAP, b"\x56\x52\xAE\x41"),
         # Example from https://www.simplymodbus.ca/FAQ.htm (the byteorder is not named)
-        (2923517522, False, BYTEORDER_BIG_SWAP, "\x41\xAE\x52\x56"),
+        (2923517522, 2, False, BYTEORDER_BIG_SWAP, b"\x41\xAE\x52\x56"),
+        (0, 4, True, BYTEORDER_BIG, b"\x00\x00\x00\x00\x00\x00\x00\x00"),
+        (0, 4, False, BYTEORDER_BIG, b"\x00\x00\x00\x00\x00\x00\x00\x00"),
+        (1, 4, True, BYTEORDER_BIG, b"\x00\x00\x00\x00\x00\x00\x00\x01"),
+        (1, 4, False, BYTEORDER_BIG, b"\x00\x00\x00\x00\x00\x00\x00\x01"),
+        (-1, 4, True, BYTEORDER_BIG, b"\xff\xff\xff\xff\xff\xff\xff\xff"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, signed, byteorder, knownstring in self.knownValues:
-            resultstring = minimalmodbus._long_to_bytestring(
-                value, signed, 2, byteorder
+        for value, num_registers, signed, byteorder, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._long_to_bytes(
+                value, signed, num_registers, byteorder
             )
-            self.assertEqual(resultstring, knownstring)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
-            ValueError, minimalmodbus._long_to_bytestring, -1, False, 2
+            ValueError, minimalmodbus._long_to_bytes, -1, False, 2
         )  # Range 0 to 4294967295
         self.assertRaises(
-            ValueError, minimalmodbus._long_to_bytestring, 4294967296, False, 2
+            ValueError, minimalmodbus._long_to_bytes, 4294967296, False, 2
         )
         self.assertRaises(
-            ValueError, minimalmodbus._long_to_bytestring, -2147483649, True, 2
+            ValueError, minimalmodbus._long_to_bytes, -2147483649, True, 2
         )  # Range -2147483648 to 2147483647
+        self.assertRaises(ValueError, minimalmodbus._long_to_bytes, 2147483648, True, 2)
         self.assertRaises(
-            ValueError, minimalmodbus._long_to_bytestring, 2147483648, True, 2
-        )
-        self.assertRaises(
-            ValueError, minimalmodbus._long_to_bytestring, 222222222222222, True, 2
+            ValueError, minimalmodbus._long_to_bytes, 222222222222222, True, 2
         )
 
-        for number_of_registers in [0, 1, 3, 4, 5, 6, 7, 8, 16]:
+        for number_of_registers in [0, 1, 3, 5, 6, 7, 8, 9, 16]:
             self.assertRaises(
                 ValueError,
-                minimalmodbus._long_to_bytestring,
+                minimalmodbus._long_to_bytes,
                 1,
                 True,
                 number_of_registers,
             )
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
-            self.assertRaises(
-                TypeError, minimalmodbus._long_to_bytestring, value, True, 2
-            )
-            self.assertRaises(
-                TypeError, minimalmodbus._long_to_bytestring, 1, True, value
-            )
+            self.assertRaises(TypeError, minimalmodbus._long_to_bytes, value, True, 2)
+            self.assertRaises(TypeError, minimalmodbus._long_to_bytes, 1, True, value)
         for value in _NOT_BOOLEANS:
-            self.assertRaises(TypeError, minimalmodbus._long_to_bytestring, 1, value, 2)
-
+            self.assertRaises(TypeError, minimalmodbus._long_to_bytes, 1, value, 2)
 
-class TestBytestringToLong(ExtendedTestCase):
 
-    knownValues = TestLongToBytestring.knownValues
+class TestBytesToLong(ExtendedTestCase):
+    known_values = TestLongToBytes.known_values
 
     def testKnownValues(self) -> None:
-        for knownvalue, signed, byteorder, bytestring in self.knownValues:
-            resultvalue = minimalmodbus._bytestring_to_long(
-                bytestring, signed, 2, byteorder
+        for (
+            known_value,
+            num_registers,
+            signed,
+            byteorder,
+            inputbytes,
+        ) in self.known_values:
+            resultvalue = minimalmodbus._bytes_to_long(
+                inputbytes, signed, num_registers, byteorder
             )
-            self.assertEqual(resultvalue, knownvalue)
+            self.assertEqual(resultvalue, known_value)
 
     def testWrongInputValue(self) -> None:
-        for inputstring in ["", "A", "AA", "AAA", "AAAAA"]:
+        for inputbytes in [b"", b"A", b"AA", b"AAA", b"AAAAA"]:
             self.assertRaises(
-                ValueError, minimalmodbus._bytestring_to_long, inputstring, True, 2
+                ValueError, minimalmodbus._bytes_to_long, inputbytes, True, 2
+            )
+        for inputbytes in [
+            b"",
+            b"A",
+            b"AA",
+            b"AAA",
+            b"AAAA",
+            b"AAAAA",
+            b"AAAAA",
+            b"AAAAAAA",
+            b"AAAAAAAAA",
+        ]:
+            self.assertRaises(
+                ValueError, minimalmodbus._bytes_to_long, inputbytes, True, 4
             )
         for number_of_registers in [0, 1, 3, 4, 5, 6, 7, 8, 16]:
             self.assertRaises(
                 ValueError,
-                minimalmodbus._bytestring_to_long,
-                "AAAA",
+                minimalmodbus._bytes_to_long,
+                b"AAAA",
                 True,
                 number_of_registers,
             )
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_long, value, True, 2
-            )
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_long, value, True, 2)
         for value in _NOT_BOOLEANS:
             self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_long, "AAAA", value, 2
+                TypeError, minimalmodbus._bytes_to_long, b"AAAA", value, 2
             )
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_long, "AAAA", True, value
+                TypeError, minimalmodbus._bytes_to_long, b"AAAA", True, value
             )
 
 
 class TestSanityLong(ExtendedTestCase):
-
-    knownValues = TestLongToBytestring.knownValues
+    known_values = TestLongToBytes.known_values
 
     def testSanity(self) -> None:
-        for value, signed, byteorder, bytestring in self.knownValues:
-            resultvalue = minimalmodbus._bytestring_to_long(
-                minimalmodbus._long_to_bytestring(value, signed, 2, byteorder),
+        for value, num_registers, signed, byteorder, _ in self.known_values:
+            resultvalue = minimalmodbus._bytes_to_long(
+                minimalmodbus._long_to_bytes(value, signed, num_registers, byteorder),
                 signed,
-                2,
+                num_registers,
                 byteorder,
             )
             self.assertEqual(resultvalue, value)
 
 
-class TestFloatToBytestring(ExtendedTestCase):
-
+class TestFloatToBytes(ExtendedTestCase):
     # Use this online calculator:
     # https://www.h-schmidt.net/FloatConverter/IEEE754.html
 
     # See also examples in
     # http://en.wikipedia.org/wiki/Single-precision_floating-point_format
     # http://en.wikipedia.org/wiki/Double-precision_floating-point_format
 
-    knownValues = [
-        (1, 2, BYTEORDER_BIG, "\x3f\x80\x00\x00"),
-        (1.0, 2, BYTEORDER_BIG, "\x3f\x80\x00\x00"),  # wikipedia
-        (1.0, 2, BYTEORDER_BIG, "?\x80\x00\x00"),
-        (1.1, 2, BYTEORDER_BIG, "\x3f\x8c\xcc\xcd"),
-        (100, 2, BYTEORDER_BIG, "\x42\xc8\x00\x00"),
-        (100.0, 2, BYTEORDER_BIG, "\x42\xc8\x00\x00"),
-        (1.0e5, 2, BYTEORDER_BIG, "\x47\xc3\x50\x00"),
-        (1.1e9, 2, BYTEORDER_BIG, "\x4e\x83\x21\x56"),
-        (1.0e16, 2, BYTEORDER_BIG, "\x5a\x0e\x1b\xca"),
-        (1.5e16, 2, BYTEORDER_BIG, "\x5a\x55\x29\xaf"),
-        (3.65e30, 2, BYTEORDER_BIG, "\x72\x38\x47\x25"),
-        (-1.1, 2, BYTEORDER_BIG, "\xbf\x8c\xcc\xcd"),
-        (-2, 2, BYTEORDER_BIG, "\xc0\x00\x00\x00"),
-        (-3.6e30, 2, BYTEORDER_BIG, "\xf2\x35\xc0\xe9"),
-        (1.0, 4, BYTEORDER_BIG, "\x3f\xf0\x00\x00\x00\x00\x00\x00"),
-        (2, 4, BYTEORDER_BIG, "\x40\x00\x00\x00\x00\x00\x00\x00"),
-        (1.1e9, 4, BYTEORDER_BIG, "\x41\xd0\x64\x2a\xc0\x00\x00\x00"),
-        (3.65e30, 4, BYTEORDER_BIG, "\x46\x47\x08\xe4\x9e\x2f\x4d\x62"),
-        (2.42e300, 4, BYTEORDER_BIG, "\x7e\x4c\xe8\xa5\x67\x1f\x46\xa0"),
-        (-1.1, 4, BYTEORDER_BIG, "\xbf\xf1\x99\x99\x99\x99\x99\x9a"),
-        (-2, 4, BYTEORDER_BIG, "\xc0\x00\x00\x00\x00\x00\x00\x00"),
-        (-3.6e30, 4, BYTEORDER_BIG, "\xc6\x46\xb8\x1d\x1a\x43\xb2\x06"),
-        (-3.6e30, 4, BYTEORDER_LITTLE, "\x06\xb2\x43\x1a\x1d\xb8\x46\xc6"),
-        (-3.6e30, 4, BYTEORDER_BIG_SWAP, "\x46\xc6\x1d\xb8\x43\x1a\x06\xb2"),
-        (-3.6e30, 4, BYTEORDER_LITTLE_SWAP, "\xb2\x06\x1a\x43\xb8\x1d\xc6\x46"),
+    known_values = [
+        (1, 2, BYTEORDER_BIG, b"\x3f\x80\x00\x00"),
+        (1.0, 2, BYTEORDER_BIG, b"\x3f\x80\x00\x00"),  # wikipedia
+        (1.0, 2, BYTEORDER_BIG, b"?\x80\x00\x00"),
+        (1.1, 2, BYTEORDER_BIG, b"\x3f\x8c\xcc\xcd"),
+        (100, 2, BYTEORDER_BIG, b"\x42\xc8\x00\x00"),
+        (100.0, 2, BYTEORDER_BIG, b"\x42\xc8\x00\x00"),
+        (1.0e5, 2, BYTEORDER_BIG, b"\x47\xc3\x50\x00"),
+        (1.1e9, 2, BYTEORDER_BIG, b"\x4e\x83\x21\x56"),
+        (1.0e16, 2, BYTEORDER_BIG, b"\x5a\x0e\x1b\xca"),
+        (1.5e16, 2, BYTEORDER_BIG, b"\x5a\x55\x29\xaf"),
+        (3.65e30, 2, BYTEORDER_BIG, b"\x72\x38\x47\x25"),
+        (-1.1, 2, BYTEORDER_BIG, b"\xbf\x8c\xcc\xcd"),
+        (-2, 2, BYTEORDER_BIG, b"\xc0\x00\x00\x00"),
+        (-3.6e30, 2, BYTEORDER_BIG, b"\xf2\x35\xc0\xe9"),
+        (1.0, 4, BYTEORDER_BIG, b"\x3f\xf0\x00\x00\x00\x00\x00\x00"),
+        (2, 4, BYTEORDER_BIG, b"\x40\x00\x00\x00\x00\x00\x00\x00"),
+        (1.1e9, 4, BYTEORDER_BIG, b"\x41\xd0\x64\x2a\xc0\x00\x00\x00"),
+        (3.65e30, 4, BYTEORDER_BIG, b"\x46\x47\x08\xe4\x9e\x2f\x4d\x62"),
+        (2.42e300, 4, BYTEORDER_BIG, b"\x7e\x4c\xe8\xa5\x67\x1f\x46\xa0"),
+        (-1.1, 4, BYTEORDER_BIG, b"\xbf\xf1\x99\x99\x99\x99\x99\x9a"),
+        (-2, 4, BYTEORDER_BIG, b"\xc0\x00\x00\x00\x00\x00\x00\x00"),
+        (-3.6e30, 4, BYTEORDER_BIG, b"\xc6\x46\xb8\x1d\x1a\x43\xb2\x06"),
+        (-3.6e30, 4, BYTEORDER_LITTLE, b"\x06\xb2\x43\x1a\x1d\xb8\x46\xc6"),
+        (-3.6e30, 4, BYTEORDER_BIG_SWAP, b"\x46\xc6\x1d\xb8\x43\x1a\x06\xb2"),
+        (-3.6e30, 4, BYTEORDER_LITTLE_SWAP, b"\xb2\x06\x1a\x43\xb8\x1d\xc6\x46"),
         # Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page)
-        (-4.3959787e-11, 2, BYTEORDER_BIG, "\xAE\x41\x56\x52"),
+        (-4.3959787e-11, 2, BYTEORDER_BIG, b"\xAE\x41\x56\x52"),
         # Shifted byte positions manually
-        (-4.3959787e-11, 2, BYTEORDER_LITTLE, "\x52\x56\x41\xAE"),
+        (-4.3959787e-11, 2, BYTEORDER_LITTLE, b"\x52\x56\x41\xAE"),
         # Shifted byte positions manually
-        (-4.3959787e-11, 2, BYTEORDER_BIG_SWAP, "\x41\xAE\x52\x56"),
+        (-4.3959787e-11, 2, BYTEORDER_BIG_SWAP, b"\x41\xAE\x52\x56"),
         # Shifted byte positions manually
-        (-4.3959787e-11, 2, BYTEORDER_LITTLE_SWAP, "\x56\x52\xAE\x41"),
+        (-4.3959787e-11, 2, BYTEORDER_LITTLE_SWAP, b"\x56\x52\xAE\x41"),
         # Calculated by  https://www.h-schmidt.net/FloatConverter/IEEE754.html
-        (123456.00, 2, BYTEORDER_BIG, "\x47\xF1\x20\x00"),
+        (123456.00, 2, BYTEORDER_BIG, b"\x47\xF1\x20\x00"),
         # Example from https://store.chipkin.com/articles/how-real-floating-point-
         #         and-32-bit-data-is-encoded-in-modbus-rtu-messages
         #         Byte order = "No swap"
-        (123456.00, 2, BYTEORDER_LITTLE, "\x00\x20\xF1\x47"),
+        (123456.00, 2, BYTEORDER_LITTLE, b"\x00\x20\xF1\x47"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, number_of_registers, byteorder, knownstring in self.knownValues:
-            resultstring = minimalmodbus._float_to_bytestring(
+        for value, number_of_registers, byteorder, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._float_to_bytes(
                 value, number_of_registers, byteorder
             )
-            self.assertEqual(resultstring, knownstring)
+            self.assertEqual(resultbytes, known_bytes)
         self.assertEqual(
-            minimalmodbus._float_to_bytestring(1.5e999, 2), "\x7f\x80\x00\x00"
+            minimalmodbus._float_to_bytes(1.5e999, 2), b"\x7f\x80\x00\x00"
         )  # +inf
 
     def testWrongInputValue(self) -> None:
-        # Note: Out of range will not necessarily raise any error, instead it will indicate +inf etc.
-        for number_of_registers in [0, 1, 3, 5, 6, 7, 8, 16]:
+        # Note: Out of range will not necessarily raise any error, instead it
+        # will indicate +inf etc.
+        for number_of_registers in [0, 1, 3, 5, 6, 7, 8, 9, 16]:
             self.assertRaises(
-                ValueError, minimalmodbus._float_to_bytestring, 1.1, number_of_registers
+                ValueError, minimalmodbus._float_to_bytes, 1.1, number_of_registers
             )
 
     def testWrongInputType(self) -> None:
+        value: Any = None
         for value in _NOT_NUMERICALS:
-            self.assertRaises(TypeError, minimalmodbus._float_to_bytestring, value, 2)
+            self.assertRaises(TypeError, minimalmodbus._float_to_bytes, value, 2)
         for value in _NOT_INTERGERS:
-            self.assertRaises(TypeError, minimalmodbus._float_to_bytestring, 1.1, value)
-
+            self.assertRaises(TypeError, minimalmodbus._float_to_bytes, 1.1, value)
 
-class TestBytestringToFloat(ExtendedTestCase):
 
-    knownValues = TestFloatToBytestring.knownValues
+class TestBytesToFloat(ExtendedTestCase):
+    known_values = TestFloatToBytes.known_values
 
     def testKnownValues(self) -> None:
-        for knownvalue, number_of_registers, byteorder, bytestring in self.knownValues:
-            resultvalue = minimalmodbus._bytestring_to_float(
-                bytestring, number_of_registers, byteorder
+        for (
+            known_value,
+            number_of_registers,
+            byteorder,
+            inputbytes,
+        ) in self.known_values:
+            resultvalue = minimalmodbus._bytes_to_float(
+                inputbytes, number_of_registers, byteorder
             )
-            self.assertAlmostEqualRatio(resultvalue, knownvalue)
+            self.assertAlmostEqualRatio(resultvalue, known_value)
 
     def testWrongInputValue(self) -> None:
-        for bytestring in [
-            "",
-            "A",
-            "AB",
-            "ABC",
-            "ABCDE",
-            "ABCDEF",
-            "ABCDEFG",
-            "ABCDEFGHI",
+        for inputbytes in [
+            b"",
+            b"A",
+            b"AB",
+            b"ABC",
+            # Not 4 bytes
+            b"ABCDE",
+            b"ABCDEF",
+            b"ABCDEFG",
+            # Not 8 bytes
+            b"ABCDEFGHI",
         ]:
-            self.assertRaises(
-                ValueError, minimalmodbus._bytestring_to_float, bytestring, 2
-            )
-            self.assertRaises(
-                ValueError, minimalmodbus._bytestring_to_float, bytestring, 4
-            )
-        for number_of_registers in [0, 1, 3, 5, 6, 7, 8, 16]:
+            self.assertRaises(ValueError, minimalmodbus._bytes_to_float, inputbytes, 2)
+            self.assertRaises(ValueError, minimalmodbus._bytes_to_float, inputbytes, 4)
+        for number_of_registers in [0, 1, 3, 5, 6, 7, 8, 9, 16]:
             self.assertRaises(
                 ValueError,
-                minimalmodbus._bytestring_to_float,
-                "ABCD",
+                minimalmodbus._bytes_to_float,
+                b"ABCD",
                 number_of_registers,
             )
             self.assertRaises(
                 ValueError,
-                minimalmodbus._bytestring_to_float,
-                "ABCDEFGH",
+                minimalmodbus._bytes_to_float,
+                b"ABCDEFGH",
                 number_of_registers,
             )
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._bytestring_to_float, value, 2)
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_float, value, 2)
         for value in _NOT_INTERGERS:
-            self.assertRaises(TypeError, minimalmodbus._bytestring_to_float, 1.1, value)
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_float, 1.1, value)
 
 
 class TestSanityFloat(ExtendedTestCase):
-
-    knownValues = TestFloatToBytestring.knownValues
+    known_values = TestFloatToBytes.known_values
 
     def testSanity(self) -> None:
-        for value, number_of_registers, byteorder, bytestring in self.knownValues:
-            resultvalue = minimalmodbus._bytestring_to_float(
-                minimalmodbus._float_to_bytestring(
-                    value, number_of_registers, byteorder
-                ),
+        for value, number_of_registers, byteorder, _ in self.known_values:
+            resultvalue = minimalmodbus._bytes_to_float(
+                minimalmodbus._float_to_bytes(value, number_of_registers, byteorder),
                 number_of_registers,
                 byteorder,
             )
             self.assertAlmostEqualRatio(resultvalue, value)
 
 
-class TestValuelistToBytestring(ExtendedTestCase):
-
-    knownValues = [
-        ([1], 1, "\x00\x01"),
-        ([0, 0], 2, "\x00\x00\x00\x00"),
-        ([1, 2], 2, "\x00\x01\x00\x02"),
-        ([1, 256], 2, "\x00\x01\x01\x00"),
-        ([1, 2, 3, 4], 4, "\x00\x01\x00\x02\x00\x03\x00\x04"),
-        ([1, 2, 3, 4, 5], 5, "\x00\x01\x00\x02\x00\x03\x00\x04\x00\x05"),
+class TestValuelistToBytes(ExtendedTestCase):
+    known_values = [
+        ([1], 1, b"\x00\x01"),
+        ([0, 0], 2, b"\x00\x00\x00\x00"),
+        ([1, 2], 2, b"\x00\x01\x00\x02"),
+        ([1, 256], 2, b"\x00\x01\x01\x00"),
+        ([1, 2, 3, 4], 4, b"\x00\x01\x00\x02\x00\x03\x00\x04"),
+        ([1, 2, 3, 4, 5], 5, b"\x00\x01\x00\x02\x00\x03\x00\x04\x00\x05"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, number_of_registers, knownstring in self.knownValues:
-            resultstring = minimalmodbus._valuelist_to_bytestring(
-                value, number_of_registers
-            )
-            self.assertEqual(resultstring, knownstring)
+        for value, number_of_registers, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._valuelist_to_bytes(value, number_of_registers)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
-            ValueError, minimalmodbus._valuelist_to_bytestring, [1, 2, 3, 4], 1
+            ValueError, minimalmodbus._valuelist_to_bytes, [-1, 2, 3, 4], 4
         )
         self.assertRaises(
-            ValueError, minimalmodbus._valuelist_to_bytestring, [1, 2, 3, 4], -4
+            ValueError, minimalmodbus._valuelist_to_bytes, [1, 2, 3, 4], 1
+        )
+        self.assertRaises(
+            ValueError, minimalmodbus._valuelist_to_bytes, [1, 2, 3, 4], -4
         )
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTLISTS:
-            self.assertRaises(
-                TypeError, minimalmodbus._valuelist_to_bytestring, value, 4
-            )
+            self.assertRaises(TypeError, minimalmodbus._valuelist_to_bytes, value, 4)
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._valuelist_to_bytestring, [1, 2, 3, 4], value
+                TypeError, minimalmodbus._valuelist_to_bytes, [1, 2, 3, 4], value
             )
 
 
-class TestBytestringToValuelist(ExtendedTestCase):
-
-    knownValues = TestValuelistToBytestring.knownValues
+class TestBytesToValuelist(ExtendedTestCase):
+    known_values = TestValuelistToBytes.known_values
 
     def testKnownValues(self) -> None:
-        for knownlist, number_of_registers, bytestring in self.knownValues:
-            resultlist = minimalmodbus._bytestring_to_valuelist(
-                bytestring, number_of_registers
+        for knownlist, number_of_registers, inputbytes in self.known_values:
+            resultlist = minimalmodbus._bytes_to_valuelist(
+                inputbytes, number_of_registers
             )
             self.assertEqual(resultlist, knownlist)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
-            ValueError, minimalmodbus._bytestring_to_valuelist, "\x00\x01\x00\x02", 1
-        )
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_valuelist, "", 1)
-        self.assertRaises(
-            ValueError, minimalmodbus._bytestring_to_valuelist, "\x00\x01", 0
+            ValueError, minimalmodbus._bytes_to_valuelist, b"\x00\x01\x00\x02", 1
         )
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_valuelist, b"", 1)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_valuelist, b"\x00\x01", 0)
         self.assertRaises(
-            ValueError, minimalmodbus._bytestring_to_valuelist, "\x00\x01", -1
+            ValueError, minimalmodbus._bytes_to_valuelist, b"\x00\x01", -1
         )
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_valuelist, value, 1
-            )
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_valuelist, value, 1)
         for value in _NOT_INTERGERS:
-            self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_valuelist, "A", value
-            )
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_valuelist, b"A", value)
 
 
 class TestSanityValuelist(ExtendedTestCase):
-
-    knownValues = TestValuelistToBytestring.knownValues
+    known_values = TestValuelistToBytes.known_values
 
     def testSanity(self) -> None:
-        for valuelist, number_of_registers, bytestring in self.knownValues:
-            resultlist = minimalmodbus._bytestring_to_valuelist(
-                minimalmodbus._valuelist_to_bytestring(valuelist, number_of_registers),
+        for valuelist, number_of_registers, _ in self.known_values:
+            resultlist = minimalmodbus._bytes_to_valuelist(
+                minimalmodbus._valuelist_to_bytes(valuelist, number_of_registers),
                 number_of_registers,
             )
             self.assertEqual(resultlist, valuelist)
 
 
-class TestTextstringToBytestring(ExtendedTestCase):
-
-    knownValues = [
-        ("A", 1, "A "),
-        ("AB", 1, "AB"),
-        ("ABC", 2, "ABC "),
-        ("ABCD", 2, "ABCD"),
-        ("A", 16, "A" + " " * 31),
-        ("A", 32, "A" + " " * 63),
-        ("A" * 246, 123, "A" * 246),
+class TestTextstringToBytes(ExtendedTestCase):
+    known_values = [
+        ("A", 1, b"A "),
+        ("AB", 1, b"AB"),
+        ("ABC", 2, b"ABC "),
+        ("ABCD", 2, b"ABCD"),
+        ("A", 16, b"A" + b" " * 31),
+        ("A", 32, b"A" + b" " * 63),
+        ("A" * 246, 123, b"A" * 246),
     ]
 
     def testKnownValues(self) -> None:
-        for textstring, number_of_registers, knownstring in self.knownValues:
-            resultstring = minimalmodbus._textstring_to_bytestring(
+        for textstring, number_of_registers, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._textstring_to_bytes(
                 textstring, number_of_registers
             )
-            self.assertEqual(resultstring, knownstring)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytestring, "ABC", 1)
-        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytestring, "", 1)
-        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytestring, "A", -1)
-        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytestring, "A", 124)
+        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytes, "", 1)  # TODO
+        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytes, "ABC", 1)
+        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytes, "A", -1)
+        self.assertRaises(ValueError, minimalmodbus._textstring_to_bytes, "A", 124)
 
     def testWrongInputType(self) -> None:
         for value in _NOT_STRINGS:
-            self.assertRaises(
-                TypeError, minimalmodbus._textstring_to_bytestring, value, 1
-            )
+            self.assertRaises(TypeError, minimalmodbus._textstring_to_bytes, value, 1)
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._textstring_to_bytestring, "AB", value
+                TypeError, minimalmodbus._textstring_to_bytes, "AB", value
             )
 
 
-class TestBytestringToTextstring(ExtendedTestCase):
-
-    knownValues = TestTextstringToBytestring.knownValues
+class TestBytesToTextstring(ExtendedTestCase):
+    known_values = TestTextstringToBytes.known_values
 
     def testKnownValues(self) -> None:
-        for knownstring, number_of_registers, bytestring in self.knownValues:
-            resultstring = minimalmodbus._bytestring_to_textstring(
-                bytestring, number_of_registers
+        for known_bytes, number_of_registers, inputbytes in self.known_values:
+            resultbytes = minimalmodbus._bytes_to_textstring(
+                inputbytes, number_of_registers
             )
-            self.assertEqual(resultstring.strip(), knownstring)
+            self.assertEqual(resultbytes.strip(), known_bytes)
 
     def testWrongInputValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "A", 1)
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "", 1)
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "", 0)
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "ABC", 1)
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "AB", 0)
-        self.assertRaises(ValueError, minimalmodbus._bytestring_to_textstring, "AB", -1)
-        self.assertRaises(
-            ValueError, minimalmodbus._bytestring_to_textstring, "AB", 126
-        )
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"A", 1)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"", 1)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"", 0)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"ABC", 1)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"AB", 0)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"AB", -1)
+        self.assertRaises(ValueError, minimalmodbus._bytes_to_textstring, b"AB", 126)
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_textstring, value, 1
-            )
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._bytes_to_textstring, value, 1)
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, minimalmodbus._bytestring_to_textstring, "AB", value
+                TypeError, minimalmodbus._bytes_to_textstring, b"AB", value
             )
 
 
 class TestSanityTextstring(ExtendedTestCase):
-
-    knownValues = TestTextstringToBytestring.knownValues
+    known_values = TestTextstringToBytes.known_values
 
     def testSanity(self) -> None:
-        for textstring, number_of_registers, bytestring in self.knownValues:
-            resultstring = minimalmodbus._bytestring_to_textstring(
-                minimalmodbus._textstring_to_bytestring(
-                    textstring, number_of_registers
-                ),
+        for textstring, number_of_registers, _ in self.known_values:
+            resultstring = minimalmodbus._bytes_to_textstring(
+                minimalmodbus._textstring_to_bytes(textstring, number_of_registers),
                 number_of_registers,
             )
             self.assertEqual(resultstring.strip(), textstring)
 
 
 class TestPack(ExtendedTestCase):
-
-    knownValues = [
-        (-77, ">h", "\xff\xb3"),  # (Signed) short (2 bytes)
-        (-1, ">h", "\xff\xff"),
-        (-770, ">h", "\xfc\xfe"),
-        (-32768, ">h", "\x80\x00"),
-        (32767, ">h", "\x7f\xff"),
-        (770, ">H", "\x03\x02"),  # Unsigned short (2 bytes)
-        (65535, ">H", "\xff\xff"),
-        (75000, ">l", "\x00\x01\x24\xf8"),  # (Signed) long (4 bytes)
-        (-1, ">l", "\xff\xff\xff\xff"),
-        (-2147483648, ">l", "\x80\x00\x00\x00"),
-        (-200000000, ">l", "\xf4\x14\x3e\x00"),
-        (1, ">L", "\x00\x00\x00\x01"),  # Unsigned long (4 bytes)
-        (75000, ">L", "\x00\x01\x24\xf8"),
-        (2147483648, ">L", "\x80\x00\x00\x00"),
-        (2147483647, ">L", "\x7f\xff\xff\xff"),
-        (1.0, ">f", "\x3f\x80\x00\x00"),  # Float (4 bytes)
-        (1.0e5, ">f", "\x47\xc3\x50\x00"),
-        (1.0e16, ">f", "\x5a\x0e\x1b\xca"),
-        (3.65e30, ">f", "\x72\x38\x47\x25"),
-        (-2, ">f", "\xc0\x00\x00\x00"),
-        (-3.6e30, ">f", "\xf2\x35\xc0\xe9"),
-        (1.0, ">d", "\x3f\xf0\x00\x00\x00\x00\x00\x00"),  # Double (8 bytes)
-        (2, ">d", "\x40\x00\x00\x00\x00\x00\x00\x00"),
-        (1.1e9, ">d", "\x41\xd0\x64\x2a\xc0\x00\x00\x00"),
-        (3.65e30, ">d", "\x46\x47\x08\xe4\x9e\x2f\x4d\x62"),
-        (2.42e300, ">d", "\x7e\x4c\xe8\xa5\x67\x1f\x46\xa0"),
-        (-1.1, ">d", "\xbf\xf1\x99\x99\x99\x99\x99\x9a"),
-        (-2, ">d", "\xc0\x00\x00\x00\x00\x00\x00\x00"),
+    known_values = [
+        (-77, ">h", b"\xff\xb3"),  # (Signed) short (2 bytes)
+        (-1, ">h", b"\xff\xff"),
+        (-770, ">h", b"\xfc\xfe"),
+        (-32768, ">h", b"\x80\x00"),
+        (32767, ">h", b"\x7f\xff"),
+        (770, ">H", b"\x03\x02"),  # Unsigned short (2 bytes)
+        (65535, ">H", b"\xff\xff"),
+        (75000, ">l", b"\x00\x01\x24\xf8"),  # (Signed) long (4 bytes)
+        (-1, ">l", b"\xff\xff\xff\xff"),
+        (-2147483648, ">l", b"\x80\x00\x00\x00"),
+        (-200000000, ">l", b"\xf4\x14\x3e\x00"),
+        (1, ">L", b"\x00\x00\x00\x01"),  # Unsigned long (4 bytes)
+        (75000, ">L", b"\x00\x01\x24\xf8"),
+        (2147483648, ">L", b"\x80\x00\x00\x00"),
+        (2147483647, ">L", b"\x7f\xff\xff\xff"),
+        (1.0, ">f", b"\x3f\x80\x00\x00"),  # Float (4 bytes)
+        (1.0e5, ">f", b"\x47\xc3\x50\x00"),
+        (1.0e16, ">f", b"\x5a\x0e\x1b\xca"),
+        (3.65e30, ">f", b"\x72\x38\x47\x25"),
+        (-2, ">f", b"\xc0\x00\x00\x00"),
+        (-3.6e30, ">f", b"\xf2\x35\xc0\xe9"),
+        (1.0, ">d", b"\x3f\xf0\x00\x00\x00\x00\x00\x00"),  # Double (8 bytes)
+        (2, ">d", b"\x40\x00\x00\x00\x00\x00\x00\x00"),
+        (1.1e9, ">d", b"\x41\xd0\x64\x2a\xc0\x00\x00\x00"),
+        (3.65e30, ">d", b"\x46\x47\x08\xe4\x9e\x2f\x4d\x62"),
+        (2.42e300, ">d", b"\x7e\x4c\xe8\xa5\x67\x1f\x46\xa0"),
+        (-1.1, ">d", b"\xbf\xf1\x99\x99\x99\x99\x99\x9a"),
+        (-2, ">d", b"\xc0\x00\x00\x00\x00\x00\x00\x00"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, formatstring, knownstring in self.knownValues:
-            resultstring = minimalmodbus._pack(formatstring, value)
-            self.assertEqual(resultstring, knownstring)
+        for value, formatstring, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._pack_bytes(formatstring, value)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._pack, "ABC", 35)
-        self.assertRaises(ValueError, minimalmodbus._pack, "", 35)
-        self.assertRaises(ValueError, minimalmodbus._pack, ">H", -35)
-        self.assertRaises(ValueError, minimalmodbus._pack, ">L", -35)
+        self.assertRaises(ValueError, minimalmodbus._pack_bytes, "ABC", 35)
+        self.assertRaises(ValueError, minimalmodbus._pack_bytes, "", 35)
+        self.assertRaises(ValueError, minimalmodbus._pack_bytes, ">H", -35)
+        self.assertRaises(ValueError, minimalmodbus._pack_bytes, ">L", -35)
 
     def testWrongInputType(self) -> None:
         for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._pack, value, 1)
+            self.assertRaises(TypeError, minimalmodbus._pack_bytes, value, 1)
         for value in ["1", ["1"], [1], ["\x00\x2d\x00\x58"], ["A", "B", "C"], "ABC"]:
-            self.assertRaises(ValueError, minimalmodbus._pack, ">h", value)
+            self.assertRaises(ValueError, minimalmodbus._pack_bytes, ">h", value)
 
 
 class TestUnpack(ExtendedTestCase):
-
-    knownValues = TestPack.knownValues
+    known_values = TestPack.known_values
 
     def testKnownValues(self) -> None:
-        for knownvalue, formatstring, bytestring in self.knownValues:
-            resultvalue = minimalmodbus._unpack(formatstring, bytestring)
-            self.assertAlmostEqualRatio(resultvalue, knownvalue)
+        for known_value, formatstring, inputbytes in self.known_values:
+            resultvalue = minimalmodbus._unpack_bytes(formatstring, inputbytes)
+            self.assertAlmostEqualRatio(resultvalue, known_value)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(
-            InvalidResponseError, minimalmodbus._unpack, "ABC", "\xff\xb3"
+            InvalidResponseError, minimalmodbus._unpack_bytes, "ABC", b"\xff\xb3"
         )
-        self.assertRaises(ValueError, minimalmodbus._unpack, "", "\xff\xb3")
-        self.assertRaises(ValueError, minimalmodbus._unpack, ">h", "")
+        self.assertRaises(ValueError, minimalmodbus._unpack_bytes, "", b"\xff\xb3")
+        self.assertRaises(ValueError, minimalmodbus._unpack_bytes, ">h", b"")
 
     def testWrongInputType(self) -> None:
         for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._unpack, value, "\xff\xb3")
-            self.assertRaises(TypeError, minimalmodbus._unpack, ">h", value)
+            self.assertRaises(
+                TypeError, minimalmodbus._unpack_bytes, value, b"\xff\xb3"
+            )
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._unpack_bytes, ">h", value)
 
 
 class TestSwap(ExtendedTestCase):
-
-    knownValues = [
-        ("", ""),
-        ("AB", "BA"),
-        ("ABCD", "BADC"),
-        ("ABCDEF", "BADCFE"),
-        ("ABCDEFGH", "BADCFEHG"),
-        ("ABCDEFGHIJ", "BADCFEHGJI"),
-        ("ABCDEFGHIJKL", "BADCFEHGJILK"),
+    known_values = [
+        (b"", b""),
+        (b"AB", b"BA"),
+        (b"ABCD", b"BADC"),
+        (b"ABCDEF", b"BADCFE"),
+        (b"ABCDEFGH", b"BADCFEHG"),
+        (b"ABCDEFGHIJ", b"BADCFEHGJI"),
+        (b"ABCDEFGHIJKL", b"BADCFEHGJILK"),
     ]
 
-    wrongValues = ["A", "ABC", "ABCDE", "A" * 123]
+    wrongValues = [b"A", b"ABC", b"ABCDE", b"A" * 123]
 
     def testKnownValues(self) -> None:
-        for inputvalue, knownresult in self.knownValues:
+        for inputvalue, known_result in self.known_values:
             result = minimalmodbus._swap(inputvalue)
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testWrongValues(self) -> None:
         for value in self.wrongValues:
             self.assertRaises(ValueError, minimalmodbus._swap, value)
 
 
 class TestSanityPackUnpack(ExtendedTestCase):
-
-    knownValues = TestPack.knownValues
+    known_values = TestPack.known_values
 
     def testSanity(self) -> None:
-        for value, formatstring, bytestring in self.knownValues:
-            resultstring = minimalmodbus._pack(
-                formatstring, minimalmodbus._unpack(formatstring, bytestring)
+        for _, formatstring, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._pack_bytes(
+                formatstring, minimalmodbus._unpack_bytes(formatstring, known_bytes)
             )
-            self.assertEqual(resultstring, bytestring)
+            self.assertEqual(resultbytes, known_bytes)
 
 
 class TestHexencode(ExtendedTestCase):
-
-    knownValues = [
-        ("", False, ""),
-        ("7", False, "37"),
-        ("J", False, "4A"),
-        ("\x5d", False, "5D"),
-        ("\x04", False, "04"),
-        ("\x04\x5d", False, "045D"),
-        ("mn", False, "6D6E"),
-        ("Katt1", False, "4B61747431"),
-        ("", True, ""),
-        ("7", True, "37"),
-        ("J", True, "4A"),
-        ("\x5d", True, "5D"),
-        ("\x04", True, "04"),
-        ("\x04\x5d", True, "04 5D"),
-        ("mn", True, "6D 6E"),
-        ("Katt1", True, "4B 61 74 74 31"),
+    known_values = [
+        (b"", False, b""),
+        (b"7", False, b"37"),
+        (b"J", False, b"4A"),
+        (b"\x5d", False, b"5D"),
+        (b"\x04", False, b"04"),
+        (b"\x04\x5d", False, b"045D"),
+        (b"mn", False, b"6D6E"),
+        (b"Katt1", False, b"4B61747431"),
+        (b"", True, b""),
+        (b"7", True, b"37"),
+        (b"J", True, b"4A"),
+        (b"\x5d", True, b"5D"),
+        (b"\x04", True, b"04"),
+        (b"\x04\x5d", True, b"04 5D"),
+        (b"mn", True, b"6D 6E"),
+        (b"Katt1", True, b"4B 61 74 74 31"),
     ]
 
     def testKnownValues(self) -> None:
-        for value, insert_spaces, knownstring in self.knownValues:
-            resultstring = minimalmodbus._hexencode(value, insert_spaces)
-            self.assertEqual(resultstring, knownstring)
+        for value, insert_spaces, known_bytes in self.known_values:
+            resultbytes = minimalmodbus._hexencode(value, insert_spaces)
+            self.assertEqual(resultbytes, known_bytes)
 
     def testWrongInputValue(self) -> None:
         pass
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(TypeError, minimalmodbus._hexencode, value)
 
 
 class TestHexdecode(ExtendedTestCase):
-
-    knownValues = TestHexencode.knownValues
+    known_values = TestHexencode.known_values
 
     def testKnownValues(self) -> None:
-        for knownstring, insert_spaces, value in self.knownValues:
+        for known_bytes, insert_spaces, value in self.known_values:
             if not insert_spaces:
-                resultstring = minimalmodbus._hexdecode(value)
-                self.assertEqual(resultstring, knownstring)
+                resultbytes = minimalmodbus._hexdecode(value)
+                self.assertEqual(resultbytes, known_bytes)
 
-        self.assertEqual(minimalmodbus._hexdecode("4A"), "J")
-        self.assertEqual(minimalmodbus._hexdecode("4a"), "J")
+        self.assertEqual(minimalmodbus._hexdecode(b"4A"), b"J")
+        self.assertEqual(minimalmodbus._hexdecode(b"4a"), b"J")
 
     def testAllowLowercase(self) -> None:
-        minimalmodbus._hexdecode("Aa")
-        minimalmodbus._hexdecode("aa23")
+        minimalmodbus._hexdecode(b"Aa")
+        minimalmodbus._hexdecode(b"aa23")
 
     def testWrongInputValue(self) -> None:
-        self.assertRaises(ValueError, minimalmodbus._hexdecode, "A")
-        self.assertRaises(ValueError, minimalmodbus._hexdecode, "AAA")
-        self.assertRaises(TypeError, minimalmodbus._hexdecode, "AG")
+        self.assertRaises(ValueError, minimalmodbus._hexdecode, b"A")
+        self.assertRaises(ValueError, minimalmodbus._hexdecode, b"AAA")
+        self.assertRaises(TypeError, minimalmodbus._hexdecode, b"AG")
 
     def testWrongInputType(self) -> None:
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(TypeError, minimalmodbus._hexdecode, value)
 
 
 class TestSanityHexencodeHexdecode(ExtendedTestCase):
-
-    knownValues = TestHexencode.knownValues
+    known_values = TestHexencode.known_values
 
     def testKnownValues(self) -> None:
-        for value, insert_spaces, knownstring in self.knownValues:
+        for value, insert_spaces, _ in self.known_values:
             if not insert_spaces:
-                resultstring = minimalmodbus._hexdecode(minimalmodbus._hexencode(value))
-                self.assertEqual(resultstring, value)
+                resultbytes = minimalmodbus._hexdecode(minimalmodbus._hexencode(value))
+                self.assertEqual(resultbytes, value)
 
     def testKnownValuesLoop(self) -> None:
-        """Loop through all bytestrings of length two."""
+        """Loop through all bytes objects of length two."""
         RANGE_VALUE = 256
         for i in range(RANGE_VALUE):
             for j in range(RANGE_VALUE):
-                bytestring = chr(i) + chr(j)
-                resultstring = minimalmodbus._hexdecode(
-                    minimalmodbus._hexencode(bytestring)
+                inputbytes = bytes([i, j])
+                resultbytes = minimalmodbus._hexdecode(
+                    minimalmodbus._hexencode(inputbytes)
                 )
-                self.assertEqual(resultstring, bytestring)
+                self.assertEqual(resultbytes, inputbytes)
 
 
 class TestDescribeBytes(ExtendedTestCase):
     def testKnownValues(self) -> None:
         self.assertEqual(
             minimalmodbus._describe_bytes(b"\x01\x02\x03"), "01 02 03 (3 bytes)"
         )
@@ -2712,16 +2877,15 @@
 
 ############################
 # Test number manipulation #
 ############################
 
 
 class TestTwosComplement(ExtendedTestCase):
-
-    knownValues = [
+    known_values = [
         (0, 8, 0),
         (1, 8, 1),
         (127, 8, 127),
         (-128, 8, 128),
         (-127, 8, 129),
         (-1, 8, 255),
         (0, 16, 0),
@@ -2729,18 +2893,17 @@
         (32767, 16, 32767),
         (-32768, 16, 32768),
         (-32767, 16, 32769),
         (-1, 16, 65535),
     ]
 
     def testKnownValues(self) -> None:
-        for x, bits, knownresult in self.knownValues:
-
+        for x, bits, known_result in self.known_values:
             result = minimalmodbus._twos_complement(x, bits)
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testOutOfRange(self) -> None:
         self.assertRaises(ValueError, minimalmodbus._twos_complement, 128, 8)
         self.assertRaises(ValueError, minimalmodbus._twos_complement, 1000000, 8)
         self.assertRaises(ValueError, minimalmodbus._twos_complement, -129, 8)
         self.assertRaises(ValueError, minimalmodbus._twos_complement, 32768, 16)
         self.assertRaises(ValueError, minimalmodbus._twos_complement, 1000000, 16)
@@ -2752,22 +2915,20 @@
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, minimalmodbus._twos_complement, value, 8)
 
 
 class TestFromTwosComplement(ExtendedTestCase):
-
-    knownValues = TestTwosComplement.knownValues
+    known_values = TestTwosComplement.known_values
 
     def testKnownValues(self) -> None:
-        for knownresult, bits, x in self.knownValues:
-
+        for known_result, bits, x in self.known_values:
             result = minimalmodbus._from_twos_complement(x, bits)
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testOutOfRange(self) -> None:
         self.assertRaises(ValueError, minimalmodbus._from_twos_complement, 256, 8)
         self.assertRaises(ValueError, minimalmodbus._from_twos_complement, 1000000, 8)
         self.assertRaises(ValueError, minimalmodbus._from_twos_complement, -1, 8)
         self.assertRaises(ValueError, minimalmodbus._from_twos_complement, 65536, 16)
         self.assertRaises(ValueError, minimalmodbus._from_twos_complement, 1000000, 16)
@@ -2780,58 +2941,54 @@
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, minimalmodbus._from_twos_complement, value, 8)
             self.assertRaises(TypeError, minimalmodbus._from_twos_complement, 1, value)
 
 
 class TestSanityTwosComplement(ExtendedTestCase):
-
-    knownValues = [1, 2, 4, 8, 12, 16]
+    known_values = [1, 2, 4, 8, 12, 16]
 
     def testSanity(self) -> None:
-        for bits in self.knownValues:
-            for x in range(2 ** bits):
+        for bits in self.known_values:
+            for x in range(2**bits):
                 resultvalue = minimalmodbus._twos_complement(
                     minimalmodbus._from_twos_complement(x, bits), bits
                 )
                 self.assertEqual(resultvalue, x)
 
 
 #########################
 # Test bit manipulation #
 #########################
 
 
 class TestSetBitOn(ExtendedTestCase):
-
-    knownValues = [
+    known_values = [
         (4, 0, 5),
         (4, 1, 6),
         (1, 1, 3),
     ]
 
     def testKnownValues(self) -> None:
-        for x, bitnum, knownresult in self.knownValues:
-
+        for x, bitnum, known_result in self.known_values:
             result = minimalmodbus._set_bit_on(x, bitnum)
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(ValueError, minimalmodbus._set_bit_on, 1, -1)
         self.assertRaises(ValueError, minimalmodbus._set_bit_on, -2, 1)
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, minimalmodbus._set_bit_on, value, 1)
             self.assertRaises(TypeError, minimalmodbus._set_bit_on, 1, value)
 
 
 class TestCheckBit(ExtendedTestCase):
-
-    knownValues = [
+    known_values = [
         (0, 0, False),
         (0, 1, False),
         (0, 2, False),
         (0, 3, False),
         (0, 4, False),
         (0, 5, False),
         (0, 6, False),
@@ -2841,18 +2998,17 @@
         (4, 3, False),
         (4, 4, False),
         (4, 5, False),
         (4, 5, False),
     ]
 
     def testKnownValues(self) -> None:
-        for x, bitnum, knownresult in self.knownValues:
-
+        for x, bitnum, known_result in self.known_values:
             result = minimalmodbus._check_bit(x, bitnum)
-            self.assertEqual(result, knownresult)
+            self.assertEqual(result, known_result)
 
     def testWrongInputValue(self) -> None:
         self.assertRaises(ValueError, minimalmodbus._check_bit, 1, -1)
         self.assertRaises(ValueError, minimalmodbus._check_bit, -2, 1)
 
     def testWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
@@ -2861,71 +3017,71 @@
 
 
 ############################
 # Error checking functions #
 ############################
 
 
-class TestCalculateCrcString(ExtendedTestCase):
-
-    knownValues = [
+class TestCalculateCrc(ExtendedTestCase):
+    # Example from MODBUS over Serial Line Specification and Implementation Guide V1.02
+    known_values = [
         (
-            "\x02\x07",
-            "\x41\x12",
-        ),  # Example from MODBUS over Serial Line Specification and Implementation Guide V1.02
-        ("ABCDE", "\x0fP"),
+            b"\x02\x07",
+            b"\x41\x12",
+        ),
+        (b"ABCDE", b"\x0fP"),
     ]
 
     def testKnownValues(self) -> None:
-        for inputstring, knownresult in self.knownValues:
-            resultstring = minimalmodbus._calculate_crc_string(inputstring)
-            self.assertEqual(resultstring, knownresult)
+        for inputbytes, known_result in self.known_values:
+            resultbytes = minimalmodbus._calculate_crc(inputbytes)
+            self.assertEqual(resultbytes, known_result)
 
     def testCalculationTime(self) -> None:
-        teststrings = [minimalmodbus._num_to_twobyte_string(i) for i in range(2 ** 16)]
-        minimalmodbus._print_out(
+        all_byte_variants = [minimalmodbus._num_to_two_bytes(i) for i in range(2**16)]
+        print(
             "\n\n   Measuring CRC calculation time. Running {} calculations ...".format(
-                len(teststrings)
+                len(all_byte_variants)
             )
         )
         start_time = time.time()
-        for teststring in teststrings:
-            minimalmodbus._calculate_crc_string(teststring)
+        for byte_variants in all_byte_variants:
+            minimalmodbus._calculate_crc(byte_variants)
         calculation_time = time.time() - start_time
-        minimalmodbus._print_out(
-            "CRC calculation time: {} calculations took {:.3f} s ({} s per calculation)\n\n".format(
-                len(teststrings),
+        print(
+            "CRC calculation time: "
+            + "{} calculations took {:.3f} s ({} s per calculation)\n\n".format(
+                len(all_byte_variants),
                 calculation_time,
-                calculation_time / float(len(teststrings)),
+                calculation_time / float(len(all_byte_variants)),
             )
         )
 
-    def testNotStringInput(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._calculate_crc_string, value)
-
+    def testNotByteInput(self) -> None:
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._calculate_crc, value)
 
-class TestCalculateLrcString(ExtendedTestCase):
 
-    knownValues = [
-        ("ABCDE", "\xb1"),
+class TestCalculateLrc(ExtendedTestCase):
+    known_values = [
+        (b"ABCDE", b"\xb1"),
         (
-            "\x02\x30\x30\x31\x23\x03",
-            "\x47",
-        ),  # From C# example on http://en.wikipedia.org/wiki/Longitudinal_redundancy_check
+            b"\x02\x30\x30\x31\x23\x03",
+            b"\x47",
+        ),  # From http://en.wikipedia.org/wiki/Longitudinal_redundancy_check
     ]
 
     def testKnownValues(self) -> None:
-        for inputstring, knownresult in self.knownValues:
-            resultstring = minimalmodbus._calculate_lrc_string(inputstring)
-            self.assertEqual(resultstring, knownresult)
+        for inputbytes, known_result in self.known_values:
+            resultbytes = minimalmodbus._calculate_lrc(inputbytes)
+            self.assertEqual(resultbytes, known_result)
 
     def testNotStringInput(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._calculate_lrc_string, value)
+        for value in _NOT_BYTES:
+            self.assertRaises(TypeError, minimalmodbus._calculate_lrc, value)
 
 
 class TestCheckFunctioncode(ExtendedTestCase):
     def testCorrectFunctioncode(self) -> None:
         minimalmodbus._check_functioncode(4, [4, 5])
 
     def testCorrectFunctioncodeNoRange(self) -> None:
@@ -3011,297 +3167,300 @@
     def testWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, minimalmodbus._check_registeraddress, value)
 
 
 class TestCheckResponseSlaveErrorCode(ExtendedTestCase):
     def testResponsesWithoutErrors(self) -> None:
-        minimalmodbus._check_response_slaveerrorcode("\x01\x01\x01\x00Q\x88")
-        minimalmodbus._check_response_slaveerrorcode("\x01\x01\x05")
-        minimalmodbus._check_response_slaveerrorcode("\x01\x81\x05")
+        minimalmodbus._check_response_slaveerrorcode(b"\x01\x01\x01\x00Q\x88")
+        minimalmodbus._check_response_slaveerrorcode(b"\x01\x01\x05")
+        minimalmodbus._check_response_slaveerrorcode(b"\x01\x81\x05")
 
     def testResponsesWithErrors(self) -> None:
         self.assertRaises(
             IllegalRequestError,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x01",
+            b"\x01\x81\x01",
         )
         self.assertRaises(
             IllegalRequestError,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x02",
+            b"\x01\x81\x02",
         )
         self.assertRaises(
             IllegalRequestError,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x03",
+            b"\x01\x81\x03",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x04",
+            b"\x01\x81\x04",
         )
         self.assertRaises(
             SlaveDeviceBusyError,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x06",
+            b"\x01\x81\x06",
         )
         self.assertRaises(
             NegativeAcknowledgeError,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x07",
+            b"\x01\x81\x07",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x08",
+            b"\x01\x81\x08",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x09",
+            b"\x01\x81\x09",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x0A",
+            b"\x01\x81\x0A",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x0B",
+            b"\x01\x81\x0B",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\x0C",
+            b"\x01\x81\x0C",
         )
         self.assertRaises(
             SlaveReportedException,
             minimalmodbus._check_response_slaveerrorcode,
-            "\x01\x81\xFF",
+            b"\x01\x81\xFF",
         )
 
     def testTooShortResponses(self) -> None:
-        minimalmodbus._check_response_slaveerrorcode("")
-        minimalmodbus._check_response_slaveerrorcode("A")
-        minimalmodbus._check_response_slaveerrorcode("AB")
+        minimalmodbus._check_response_slaveerrorcode(b"")
+        minimalmodbus._check_response_slaveerrorcode(b"A")
+        minimalmodbus._check_response_slaveerrorcode(b"AB")
 
 
 class TestCheckResponseNumberOfBytes(ExtendedTestCase):
     def testCorrectNumberOfBytes(self) -> None:
-        minimalmodbus._check_response_bytecount("\x02\x03\x02")
+        minimalmodbus._check_response_bytecount(b"\x02\x03\x02")
         minimalmodbus._check_response_bytecount(
-            "\x0C\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0A\x0B\x0C"
+            b"\x0C\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0A\x0B\x0C"
         )
 
     def testWrongNumberOfBytes(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_bytecount,
-            "\x03\x03\x02",
+            b"\x03\x03\x02",
         )
         self.assertRaises(
-            InvalidResponseError, minimalmodbus._check_response_bytecount, "ABC"
+            InvalidResponseError, minimalmodbus._check_response_bytecount, b"ABC"
         )
         self.assertRaises(
-            InvalidResponseError, minimalmodbus._check_response_bytecount, ""
+            InvalidResponseError, minimalmodbus._check_response_bytecount, b""
         )
 
-    def testNotStringInput(self) -> None:
-        for value in _NOT_STRINGS:
+    def testNotByteInput(self) -> None:
+        for value in _NOT_BYTES:
             self.assertRaises(TypeError, minimalmodbus._check_response_bytecount, value)
 
 
 class TestCheckResponseRegisterAddress(ExtendedTestCase):
     def testCorrectResponseRegisterAddress(self) -> None:
-        minimalmodbus._check_response_registeraddress("\x00\x2d\x00\x58", 45)
-        minimalmodbus._check_response_registeraddress("\x00\x18\x00\x01", 24)
-        minimalmodbus._check_response_registeraddress("\x00\x47\xff\x00", 71)
-        minimalmodbus._check_response_registeraddress("\x00\x48\x00\x01", 72)
+        minimalmodbus._check_response_registeraddress(b"\x00\x2d\x00\x58", 45)
+        minimalmodbus._check_response_registeraddress(b"\x00\x18\x00\x01", 24)
+        minimalmodbus._check_response_registeraddress(b"\x00\x47\xff\x00", 71)
+        minimalmodbus._check_response_registeraddress(b"\x00\x48\x00\x01", 72)
 
     def testTooShortString(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_registeraddress,
-            "\x00",
+            b"\x00",
             46,
         )
 
     def testNotString(self) -> None:
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(
                 TypeError, minimalmodbus._check_response_registeraddress, value, 45
             )
 
     def testWrongResponseRegisterAddress(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_registeraddress,
-            "\x00\x2d\x00\x58",
+            b"\x00\x2d\x00\x58",
             46,
         )
 
     def testInvalidAddress(self) -> None:
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_registeraddress,
-            "\x00\x2d\x00\x58",
+            b"\x00\x2d\x00\x58",
             -2,
         )
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_registeraddress,
-            "\x00\x2d\x00\x58",
+            b"\x00\x2d\x00\x58",
             65536,
         )
 
     def testAddressNotInteger(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(
                 TypeError,
                 minimalmodbus._check_response_registeraddress,
-                "\x00\x2d\x00\x58",
+                b"\x00\x2d\x00\x58",
                 value,
             )
 
 
 class TestCheckResponsenumber_of_registers(ExtendedTestCase):
     def testCorrectResponsenumber_of_registers(self) -> None:
-        minimalmodbus._check_response_number_of_registers("\x00\x18\x00\x01", 1)
-        minimalmodbus._check_response_number_of_registers("\x00#\x00\x01", 1)
-        minimalmodbus._check_response_number_of_registers("\x00\x34\x00\x02", 2)
+        minimalmodbus._check_response_number_of_registers(b"\x00\x18\x00\x01", 1)
+        minimalmodbus._check_response_number_of_registers(b"\x00#\x00\x01", 1)
+        minimalmodbus._check_response_number_of_registers(b"\x00\x34\x00\x02", 2)
 
     def testTooShortString(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_number_of_registers,
-            "\x00",
+            b"\x00",
             1,
         )
 
     def testNotString(self) -> None:
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(
                 TypeError, minimalmodbus._check_response_number_of_registers, value, 1
             )
 
     def testWrongResponsenumber_of_registers(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_number_of_registers,
-            "\x00#\x00\x01",
+            b"\x00#\x00\x01",
             4,
         )
 
     def testInvalidResponsenumber_of_registersRange(self) -> None:
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_number_of_registers,
-            "\x00\x18\x00\x00",
+            b"\x00\x18\x00\x00",
             0,
         )
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_number_of_registers,
-            "\x00\x18\x00\x01",
+            b"\x00\x18\x00\x01",
             -1,
         )
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_number_of_registers,
-            "\x00\x18\x00\x01",
+            b"\x00\x18\x00\x01",
             65536,
         )
 
     def testnumber_of_registersNotInteger(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(
                 TypeError,
                 minimalmodbus._check_response_number_of_registers,
-                "\x00\x18\x00\x01",
+                b"\x00\x18\x00\x01",
                 value,
             )
 
 
 class TestCheckResponseWriteData(ExtendedTestCase):
     def testCorrectResponseWritedata(self) -> None:
-        minimalmodbus._check_response_writedata("\x00\x2d\x00\x58", "\x00\x58")
+        minimalmodbus._check_response_writedata(b"\x00\x2d\x00\x58", b"\x00\x58")
         minimalmodbus._check_response_writedata(
-            "\x00\x2d\x00\x58", minimalmodbus._num_to_twobyte_string(88)
+            b"\x00\x2d\x00\x58", minimalmodbus._num_to_two_bytes(88)
         )
-        minimalmodbus._check_response_writedata("\x00\x47\xff\x00", "\xff\x00")
+        minimalmodbus._check_response_writedata(b"\x00\x47\xff\x00", b"\xff\x00")
         minimalmodbus._check_response_writedata(
-            "\x00\x47\xff\x00", minimalmodbus._num_to_twobyte_string(65280)
+            b"\x00\x47\xff\x00", minimalmodbus._num_to_two_bytes(65280)
         )
         minimalmodbus._check_response_writedata(
-            "\x00\x2d\x00\x58ABCDEFGHIJKLMNOP", "\x00\x58"
+            b"\x00\x2d\x00\x58ABCDEFGHIJKLMNOP", b"\x00\x58"
         )
 
     def testWrongResponseWritedata(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_writedata,
-            "\x00\x2d\x00\x58",
-            "\x00\x59",
+            b"\x00\x2d\x00\x58",
+            b"\x00\x59",
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_writedata,
-            "\x00\x2d\x00\x58",
-            minimalmodbus._num_to_twobyte_string(89),
+            b"\x00\x2d\x00\x58",
+            minimalmodbus._num_to_two_bytes(89),
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_writedata,
-            "\x00\x47\xff\x00",
-            "\xff\x01",
+            b"\x00\x47\xff\x00",
+            b"\xff\x01",
         )
 
     def testNotString(self) -> None:
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(
-                TypeError, minimalmodbus._check_response_writedata, value, "\x00\x58"
+                TypeError, minimalmodbus._check_response_writedata, value, b"\x00\x58"
             )
             self.assertRaises(
                 TypeError,
                 minimalmodbus._check_response_writedata,
-                "\x00\x2d\x00\x58",
+                b"\x00\x2d\x00\x58",
                 value,
             )
 
     def testTooShortPayload(self) -> None:
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_writedata,
-            "\x00\x58",
-            "\x00\x58",
+            b"\x00\x58",
+            b"\x00\x58",
         )
         self.assertRaises(
             InvalidResponseError,
             minimalmodbus._check_response_writedata,
-            "",
-            "\x00\x58",
+            b"",
+            b"\x00\x58",
         )
 
     def testInvalidReferenceData(self) -> None:
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_writedata,
-            "\x00\x2d\x00\x58",
-            "\x00\x58\x00",
+            b"\x00\x2d\x00\x58",
+            b"\x00\x58\x00",
         )
         self.assertRaises(
             ValueError,
             minimalmodbus._check_response_writedata,
-            "\x00\x2d\x00\x58",
-            "\x58",
+            b"\x00\x2d\x00\x58",
+            b"\x58",
         )
         self.assertRaises(
-            ValueError, minimalmodbus._check_response_writedata, "\x00\x2d\x00\x58", ""
+            ValueError,
+            minimalmodbus._check_response_writedata,
+            b"\x00\x2d\x00\x58",
+            b"",
         )
 
 
 class TestCheckString(ExtendedTestCase):
     def testKnownValues(self) -> None:
         minimalmodbus._check_string("DEF", minlength=3, maxlength=3, description="ABC")
         minimalmodbus._check_string(
@@ -3469,24 +3628,42 @@
             ValueError,
             minimalmodbus._check_bytes,
             b"DEF",
             minlength=10,
             maxlength=3,
             description="ABC",
         )
+        self.assertRaises(
+            InvalidResponseError,
+            minimalmodbus._check_bytes,
+            b"DE",
+            minlength=3,
+            maxlength=3,
+            description="ABC",
+            exception_type=InvalidResponseError,
+        )
 
     def testTooLong(self) -> None:
         self.assertRaises(
             ValueError,
             minimalmodbus._check_bytes,
             b"DEFG",
             minlength=1,
             maxlength=3,
             description="ABC",
         )
+        self.assertRaises(
+            InvalidResponseError,
+            minimalmodbus._check_bytes,
+            b"DEFG",
+            minlength=1,
+            maxlength=3,
+            description="ABC",
+            exception_type=InvalidResponseError,
+        )
 
     def testInconsistentLengthlimits(self) -> None:
         self.assertRaises(
             ValueError,
             minimalmodbus._check_bytes,
             b"DEFG",
             minlength=4,
@@ -3759,53 +3936,38 @@
 #####################
 # Development tools #
 #####################
 
 
 class TestGetDiagnosticString(ExtendedTestCase):
     def testReturnsString(self) -> None:
-
         resultstring = minimalmodbus._get_diagnostic_string()
         self.assertTrue(len(resultstring) > 100)  # For Python 2.6 compatibility
 
 
-class TestPrintOut(ExtendedTestCase):
-    def testKnownValues(self) -> None:
-        minimalmodbus._print_out("ABCDEFGHIJKL")
-
-    def testInputNotString(self) -> None:
-        for value in _NOT_STRINGS:
-            self.assertRaises(TypeError, minimalmodbus._print_out, value)
-
-
-# TODO: TestInterpretRawMessage
-
-# TODO: TestInterpretPayload
-
 ###########################################
 # Communication using a dummy serial port #
 ###########################################
 
 
 class TestDummyCommunication(ExtendedTestCase):
-
-    ## Test fixture ##
+    # Test fixture #
 
     def setUp(self) -> None:
-
         # Prepare a dummy serial port to have proper responses,
         # and monkey-patch minimalmodbus to use it
-        # Note that mypy is unhappy about this: https://github.com/python/mypy/issues/1152
+        # Note that mypy is unhappy about this:
+        # https://github.com/python/mypy/issues/1152
         dummy_serial.VERBOSE = False
         dummy_serial.RESPONSES = RTU_RESPONSES
         minimalmodbus.serial.Serial = dummy_serial.Serial  # type: ignore
 
         self.instrument = minimalmodbus.Instrument("DUMMYPORTNAME", 1)
 
-    ## Read bit ##
+    # Read bit #
 
     def testReadBit(self) -> None:
         # Functioncode 2
         self.assertEqual(self.instrument.read_bit(61), 1)
         self.assertEqual(self.instrument.read_bit(61, functioncode=2), 1)
         self.assertEqual(self.instrument.read_bit(61, 2), 1)
         # Functioncode 1
@@ -3830,15 +3992,15 @@
         # Functioncode 2. Slave gives wrong byte count.
         self.assertRaises(InvalidResponseError, self.instrument.read_bit, 63)
 
     def testReadBitWithNoResponse(self) -> None:
         # Functioncode 2. Slave gives no response.
         self.assertRaises(NoResponseError, self.instrument.read_bit, 64)
 
-    ## Write bit ##
+    # Write bit #
 
     def testWriteBit(self) -> None:
         self.instrument.write_bit(71, 0)
         self.instrument.write_bit(71, False)
         self.instrument.write_bit(71, 1)
         self.instrument.write_bit(71, True)
         self.instrument.write_bit(71, 1, 5)
@@ -3873,15 +4035,15 @@
             InvalidResponseError, self.instrument.write_bit, 73, 1, functioncode=15
         )
 
     def testWriteBitWithWrongWritedataResponse(self) -> None:
         # Slave gives wrong write data
         self.assertRaises(InvalidResponseError, self.instrument.write_bit, 74, 1)
 
-    ## Read bits ##
+    # Read bits #
 
     def testReadBits(self) -> None:
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.assertEqual(
             self.instrument.read_bits(196, 22, functioncode=2),
             [0, 0, 1, 1, 0, 1, 0, 1, 1, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 1],
         )
@@ -3897,28 +4059,28 @@
             self.instrument.read_bits(0x800, 16),
             [0, 0, 0, 0, 0, 1, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0],
         )
 
     def testReadBitsWrongValue(self) -> None:
         self.assertRaises(ValueError, self.instrument.read_bits, -1, 4)
 
-    ## Write bits ##
+    # Write bits #
 
     def testWriteBits(self) -> None:
         # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
         self.instrument.write_bits(19, [1, 0, 1, 1, 0, 0, 1, 1, 1, 0])
         self.instrument.write_bits(
             19, [True, False, True, True, False, False, True, True, True, False]
         )
 
     def testWriteBitsWrongValue(self) -> None:
         self.assertRaises(ValueError, self.instrument.write_bits, -1, [0, 1])
         self.assertRaises(TypeError, self.instrument.write_bits, 122, 1)
 
-    ## Read register ##
+    # Read register #
 
     def testReadRegister(self) -> None:
         # functioncode 3
         self.assertEqual(self.instrument.read_register(289), 770)
         self.assertEqual(self.instrument.read_register(5), 184)
         self.assertEqual(self.instrument.read_register(289, 0), 770)
         self.assertEqual(self.instrument.read_register(289, 0, 3), 770)
@@ -3943,15 +4105,15 @@
 
     def testReadRegisterWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.read_register, value, 0, 3)
             self.assertRaises(TypeError, self.instrument.read_register, 289, value)
             self.assertRaises(TypeError, self.instrument.read_register, 289, 0, value)
 
-    ## Write register ##
+    # Write register #
 
     def testWriteRegister(self) -> None:
         self.instrument.write_register(35, 20)
         self.instrument.write_register(35, 20, functioncode=16)
         self.instrument.write_register(35, 20.0)
         self.instrument.write_register(24, 50)
         self.instrument.write_register(45, 88, functioncode=6)
@@ -3999,15 +4161,15 @@
         # Slave gives wrong CRC
         self.assertRaises(InvalidResponseError, self.instrument.write_register, 51, 99)
 
     def testWriteRegisterSuppressErrorMessageAtWrongCRC(self) -> None:
         try:
             self.instrument.write_register(51, 99)  # Slave gives wrong CRC
         except InvalidResponseError:
-            minimalmodbus._print_out("Minimalmodbus: An error was suppressed.")
+            print("Minimalmodbus: An error was suppressed.")
 
     def testWriteRegisterWithWrongSlaveaddressResponse(self) -> None:
         # Slave gives wrong slaveaddress
         self.assertRaises(InvalidResponseError, self.instrument.write_register, 54, 99)
 
     def testWriteRegisterWithWrongFunctioncodeResponse(self) -> None:
         # Slave gives wrong functioncode
@@ -4027,15 +4189,15 @@
 
     def testWriteRegisterWithWrongWritedataResponse(self) -> None:
         # Functioncode 6. Slave gives wrong write data.
         self.assertRaises(
             InvalidResponseError, self.instrument.write_register, 55, 99, functioncode=6
         )
 
-    ## Read Long ##
+    # Read Long #
 
     def testReadLong(self) -> None:
         self.assertEqual(self.instrument.read_long(102), 4294967295)
         self.assertEqual(self.instrument.read_long(102, signed=True), -1)
         self.assertEqual(
             self.instrument.read_long(223, byteorder=BYTEORDER_BIG), 2923517522
         )
@@ -4044,65 +4206,145 @@
         )
         self.assertEqual(
             self.instrument.read_long(225, byteorder=BYTEORDER_LITTLE_SWAP), 2923517522
         )
         self.assertEqual(
             self.instrument.read_long(226, byteorder=BYTEORDER_LITTLE), 2923517522
         )
+        self.assertEqual(
+            self.instrument.read_long(108, signed=True, number_of_registers=4), -2
+        )
+        self.assertEqual(
+            self.instrument.read_long(108, signed=False, number_of_registers=4),
+            18446744073709551614,
+        )
 
     def testReadLongWrongValue(self) -> None:
         # Wrong register address
         self.assertRaises(ValueError, self.instrument.read_long, -1)
         self.assertRaises(ValueError, self.instrument.read_long, 65536)
         # Wrong function code
         self.assertRaises(ValueError, self.instrument.read_long, 102, 1)
         self.assertRaises(ValueError, self.instrument.read_long, 102, -1)
         self.assertRaises(ValueError, self.instrument.read_long, 102, 256)
+        # Wrong number of registers
+        self.assertRaises(
+            ValueError, self.instrument.read_long, 102, 3, False, BYTEORDER_BIG, 3
+        )
 
     def testReadLongWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.read_long, value)
             self.assertRaises(TypeError, self.instrument.read_long, 102, value)
+            self.assertRaises(
+                TypeError, self.instrument.read_long, 102, 3, False, value
+            )
+            self.assertRaises(
+                TypeError,
+                self.instrument.read_long,
+                102,
+                3,
+                False,
+                BYTEORDER_BIG,
+                value,
+            )
         for value in _NOT_BOOLEANS:
-            self.assertRaises(TypeError, self.instrument.read_long, 102, signed=value)
+            self.assertRaises(TypeError, self.instrument.read_long, 102, 3, value)
 
-    ## Write Long ##
+    # Write Long #
 
     def testWriteLong(self) -> None:
         self.instrument.write_long(102, 5)
         self.instrument.write_long(102, 5, signed=True)
         self.instrument.write_long(102, -5, signed=True)
         self.instrument.write_long(102, 3, False)
         self.instrument.write_long(102, -3, True)
         self.instrument.write_long(222, 2923517522)  # BYTEORDER_BIG
         self.instrument.write_long(222, 2923517522, byteorder=BYTEORDER_BIG_SWAP)
         self.instrument.write_long(222, 2923517522, byteorder=BYTEORDER_LITTLE_SWAP)
         self.instrument.write_long(222, 2923517522, byteorder=BYTEORDER_LITTLE)
+        self.instrument.write_long(109, -4, signed=True, number_of_registers=4)
 
     def testWriteLongWrongValue(self) -> None:
         # Wrong register address
         self.assertRaises(ValueError, self.instrument.write_long, -1, 5)
         self.assertRaises(ValueError, self.instrument.write_long, 65536, 5)
         # Wrong value to write to slave
         self.assertRaises(
             ValueError, self.instrument.write_long, 102, 888888888888888888888
         )
         # Wrong value to write to slave
-        self.assertRaises(ValueError, self.instrument.write_long, 102, -5, signed=False)
+        self.assertRaises(ValueError, self.instrument.write_long, 102, -1, False)
+        self.assertRaises(
+            ValueError, self.instrument.write_long, 102, 4294967296, False
+        )
+        self.assertRaises(ValueError, self.instrument.write_long, 102, 2147483648, True)
+        self.assertRaises(
+            ValueError, self.instrument.write_long, 102, -2147483649, True
+        )
+        self.assertRaises(
+            ValueError,
+            self.instrument.write_long,
+            102,
+            18446744073709551616,
+            False,
+            BYTEORDER_BIG,
+            4,
+        )
+        self.assertRaises(
+            ValueError,
+            self.instrument.write_long,
+            102,
+            -1,
+            False,
+            BYTEORDER_BIG,
+            4,
+        )
+        self.assertRaises(
+            ValueError,
+            self.instrument.write_long,
+            102,
+            9223372036854775808,
+            True,
+            BYTEORDER_BIG,
+            4,
+        )
+        self.assertRaises(
+            ValueError,
+            self.instrument.write_long,
+            102,
+            -9223372036854775809,
+            True,
+            BYTEORDER_BIG,
+            4,
+        )
+        # Wrong number of registers
+        self.assertRaises(
+            ValueError, self.instrument.write_long, 102, 5, False, BYTEORDER_BIG, 3
+        )
 
     def testWriteLongWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.write_long, value, 5)
             self.assertRaises(TypeError, self.instrument.write_long, 102, value)
+            self.assertRaises(
+                TypeError,
+                self.instrument.write_long,
+                102,
+                5,
+                False,
+                BYTEORDER_BIG,
+                value,
+            )
         for value in _NOT_BOOLEANS:
             self.assertRaises(
                 TypeError, self.instrument.write_long, 102, 5, signed=value
             )
 
-    ## Read Float ##
+    # Read Float #
 
     def testReadFloat(self) -> None:
         # BYTEORDER_BIG
         self.assertAlmostEqual(self.instrument.read_float(241), -4.3959787e-11)
         self.assertAlmostEqual(
             self.instrument.read_float(242, byteorder=BYTEORDER_BIG_SWAP),
             -4.3959787e-11,
@@ -4130,25 +4372,27 @@
         # Wrong function code
         self.assertRaises(ValueError, self.instrument.read_float, 103, 1)
         self.assertRaises(ValueError, self.instrument.read_float, 103, -1)
         self.assertRaises(ValueError, self.instrument.read_float, 103, 256)
         # Wrong number of registers
         for value in [-1, 0, 1, 5, 6, 7, 8, 16]:
             self.assertRaises(ValueError, self.instrument.read_float, 103, 3, value)
-        self.assertRaises(InvalidResponseError, self.instrument.read_float, 103, 3, 3)
+        self.assertRaises(ValueError, self.instrument.read_float, 103, 3, 3)
 
     def testReadFloatWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.read_float, value, 3, 2)
             self.assertRaises(TypeError, self.instrument.read_float, 103, value, 2)
             self.assertRaises(TypeError, self.instrument.read_float, 103, 3, value)
 
-    ## Write Float ##
+    # Write Float #
 
     def testWriteFloat(self) -> None:
+        self.instrument.write_float(107, 1)
+        self.instrument.write_float(107, 1.0)
         self.instrument.write_float(103, 1.1)
         self.instrument.write_float(103, 1.1, 4)
         self.instrument.write_float(240, -4.3959787e-11)  # BYTEORDER_BIG
         self.instrument.write_float(240, -4.3959787e-11, byteorder=BYTEORDER_BIG_SWAP)
         self.instrument.write_float(
             240, -4.3959787e-11, byteorder=BYTEORDER_LITTLE_SWAP
         )
@@ -4165,15 +4409,15 @@
     def testWriteFloatWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.write_float, value, 1.1)
             self.assertRaises(TypeError, self.instrument.write_float, 103, 1.1, value)
         for value in _NOT_NUMERICALS:
             self.assertRaises(TypeError, self.instrument.write_float, 103, value)
 
-    ## Read String ##
+    # Read String #
 
     def testReadString(self) -> None:
         self.assertEqual(self.instrument.read_string(104, 1), "AB")
         self.assertEqual(self.instrument.read_string(104, 4), "ABCDEFGH")
         self.assertEqual(self.instrument.read_string(104, 4, 3), "ABCDEFGH")
         # TODO test with function code 4
 
@@ -4192,15 +4436,15 @@
     def testReadStringWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.read_string, value, 1)
             self.assertRaises(TypeError, self.instrument.read_string, value, 4)
             self.assertRaises(TypeError, self.instrument.read_string, 104, value)
             self.assertRaises(TypeError, self.instrument.read_string, 104, 4, value)
 
-    ## Write String ##
+    # Write String #
 
     def testWriteString(self) -> None:
         self.instrument.write_string(104, "A", 1)
         self.instrument.write_string(104, "A", 4)
         self.instrument.write_string(104, "ABCDEFGH", 4)
 
     def testWriteStringWrongValue(self) -> None:
@@ -4219,15 +4463,15 @@
     def testWriteStringWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.write_string, value, "A")
             self.assertRaises(TypeError, self.instrument.write_string, 104, "A", value)
         for value in _NOT_STRINGS:
             self.assertRaises(TypeError, self.instrument.write_string, 104, value, 4)
 
-    ## Read Registers ##
+    # Read Registers #
 
     def testReadRegisters(self) -> None:
         self.assertEqual(self.instrument.read_registers(105, 1), [16])
         self.assertEqual(self.instrument.read_registers(105, 3), [16, 32, 64])
         # TODO test with function code 4
 
     def testReadRegistersWrongValue(self) -> None:
@@ -4244,20 +4488,21 @@
 
     def testReadRegistersWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.read_registers, value, 1)
             self.assertRaises(TypeError, self.instrument.read_registers, 105, value)
             self.assertRaises(TypeError, self.instrument.read_registers, 105, 1, value)
 
-    ## Write Registers ##
+    # Write Registers #
 
     def testWriteRegisters(self) -> None:
         self.instrument.write_registers(105, [2])
         self.instrument.write_registers(105, [2, 4, 8])
-        #  self.instrument.write_registers(105, [2]*123)  # Todo create suitable response
+        # Todo create suitable response
+        #  self.instrument.write_registers(105, [2]*123)
 
     def testWriteRegistersWrongValue(self) -> None:
         # Wrong register address
         self.assertRaises(ValueError, self.instrument.write_registers, -1, [2])
         self.assertRaises(ValueError, self.instrument.write_registers, 65536, [2])
         # Wrong list value
         self.assertRaises(ValueError, self.instrument.write_registers, 105, [])
@@ -4267,18 +4512,17 @@
 
     def testWriteRegistersWrongType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(TypeError, self.instrument.write_registers, value, [2])
         for value in _NOT_INTLISTS:
             self.assertRaises(TypeError, self.instrument.write_registers, 105, value)
 
-    ## Generic command ##
+    # Generic command #
 
     def testGenericCommand(self) -> None:
-
         # read_bit(61)
         self.assertEqual(
             self.instrument._generic_command(
                 2, 61, number_of_bits=1, payloadformat=_Payloadformat.BIT
             ),
             1,
         )
@@ -4456,15 +4700,16 @@
             TypeError, self.instrument._generic_command, 3, 289, payloadformat="ABC"
         )
 
     def testGenericCommandWrongType(
         self,
     ) -> None:
         # Detected without looking at parameter combinations
-        # Note: The parameter 'value' type is dependent on the other parameters. See tests above.
+        # Note: The parameter 'value' type is dependent on the other parameters.
+        # See tests above.
         for value in _NOT_INTERGERS:
             # Function code
             self.assertRaises(TypeError, self.instrument._generic_command, value, 289)
             # Register address
             self.assertRaises(TypeError, self.instrument._generic_command, 3, value)
             self.assertRaises(
                 TypeError,
@@ -4719,67 +4964,68 @@
             16,
             123,
             1.0,
             number_of_registers=1,
             payloadformat=_Payloadformat.STRING,
         )
 
-    ## Perform command ##
+    # Perform command #
 
     def testPerformcommandKnownResponse(self) -> None:
         # Total response length should be 8 bytes
-        self.assertEqual(self.instrument._perform_command(16, "TESTCOMMAND"), "TRsp")
+        self.assertEqual(self.instrument._perform_command(16, b"TESTCOMMAND"), b"TRsp")
         self.assertEqual(
-            self.instrument._perform_command(75, "TESTCOMMAND2"), "TESTCOMMANDRESPONSE2"
+            self.instrument._perform_command(75, b"TESTCOMMAND2"),
+            b"TESTCOMMANDRESPONSE2",
         )
         # Read bit register 61 on slave 1 using function code 2.
         self.assertEqual(
-            self.instrument._perform_command(2, "\x00\x3d\x00\x01"), "\x01\x01"
+            self.instrument._perform_command(2, b"\x00\x3d\x00\x01"), b"\x01\x01"
         )
 
     def testPerformcommandWrongSlaveResponse(self) -> None:
         # Wrong slave address in response
         self.assertRaises(
-            InvalidResponseError, self.instrument._perform_command, 1, "TESTCOMMAND"
+            InvalidResponseError, self.instrument._perform_command, 1, b"TESTCOMMAND"
         )
         # Wrong function code in response
         self.assertRaises(
-            InvalidResponseError, self.instrument._perform_command, 2, "TESTCOMMAND"
+            InvalidResponseError, self.instrument._perform_command, 2, b"TESTCOMMAND"
         )
         # Wrong CRC in response
         self.assertRaises(
-            InvalidResponseError, self.instrument._perform_command, 3, "TESTCOMMAND"
+            InvalidResponseError, self.instrument._perform_command, 3, b"TESTCOMMAND"
         )
         # Too short response message from slave
         self.assertRaises(
-            InvalidResponseError, self.instrument._perform_command, 4, "TESTCOMMAND"
+            InvalidResponseError, self.instrument._perform_command, 4, b"TESTCOMMAND"
         )
         # Error indication from slave
         self.assertRaises(
-            InvalidResponseError, self.instrument._perform_command, 5, "TESTCOMMAND"
+            InvalidResponseError, self.instrument._perform_command, 5, b"TESTCOMMAND"
         )
 
     def testPerformcommandWrongInputValue(self) -> None:
         # Wrong function code
         self.assertRaises(
-            ValueError, self.instrument._perform_command, -1, "TESTCOMMAND"
+            ValueError, self.instrument._perform_command, -1, b"TESTCOMMAND"
         )
         self.assertRaises(
-            ValueError, self.instrument._perform_command, 128, "TESTCOMMAND"
+            ValueError, self.instrument._perform_command, 128, b"TESTCOMMAND"
         )
 
     def testPerformcommandWrongInputType(self) -> None:
         for value in _NOT_INTERGERS:
             self.assertRaises(
-                TypeError, self.instrument._perform_command, value, "TESTCOMMAND"
+                TypeError, self.instrument._perform_command, value, b"TESTCOMMAND"
             )
-        for value in _NOT_STRINGS:
+        for value in _NOT_BYTES:
             self.assertRaises(TypeError, self.instrument._perform_command, 16, value)
 
-    ## Communicate ##
+    # Communicate #
 
     def testCommunicateKnownResponse(self) -> None:
         self.assertEqual(
             self.instrument._communicate(b"TESTMESSAGE", _LARGE_NUMBER_OF_BYTES),
             b"TESTRESPONSE",
         )
 
@@ -4790,14 +5036,23 @@
             )
 
     def testCommunicateNoMessage(self) -> None:
         self.assertRaises(
             ValueError, self.instrument._communicate, b"", _LARGE_NUMBER_OF_BYTES
         )
 
+    def testCommunicateNoSerialPort(self) -> None:
+        self.instrument.serial = None
+        self.assertRaises(
+            minimalmodbus.ModbusException,
+            self.instrument._communicate,
+            b"TESTMESSAGE",
+            _LARGE_NUMBER_OF_BYTES,
+        )
+
     def testCommunicateNoResponse(self) -> None:
         self.assertRaises(
             NoResponseError,
             self.instrument._communicate,
             b"MessageForEmptyResponse",
             _LARGE_NUMBER_OF_BYTES,
         )
@@ -4825,33 +5080,36 @@
 
     def testMeasureRoundtriptime(self) -> None:
         self.instrument.debug = True
         self.assertIsNone(self.instrument.roundtrip_time)
         self.instrument.write_bit(71, 1)
         self.assertIsNotNone(self.instrument.roundtrip_time)
         # Measured round trip time in seconds, see dummy_serial
-        self.assertGreater(self.instrument.roundtrip_time, 0.001)
+        self.assertGreater(self.instrument.roundtrip_time, 0.001)  # type: ignore
 
-    ## __repr__ ##
+    # __repr__ #
 
     def testRepresentation(self) -> None:
         representation = repr(self.instrument)
         self.assertTrue("minimalmodbus.Instrument<id=" in representation)
         self.assertTrue(
             ", address=1, mode=rtu, close_port_after_each_call=False, "
             in representation
         )
         self.assertTrue(
-            ", precalculate_read_size=True, clear_buffers_before_each_transaction=True, "
+            (
+                ", precalculate_read_size=True, "
+                + "clear_buffers_before_each_transaction=True, "
+            )
             in representation
         )
         self.assertTrue(", handle_local_echo=False, debug=False, " in representation)
         self.assertTrue(", open=True>(port=" in representation)
 
-    ## Test the dummy serial port itself ##
+    # Test the dummy serial port itself #
 
     def testReadPortClosed(self) -> None:
         assert self.instrument.serial is not None
         self.instrument.serial.close()
         # Error raised by dummy_serial
         self.assertRaises(IOError, self.instrument.serial.read, 1000)
 
@@ -4862,21 +5120,21 @@
 
     def testPortAlreadyClosed(self) -> None:
         assert self.instrument.serial is not None
         self.instrument.serial.close()
         # Error raised by dummy_serial
         self.assertRaises(IOError, self.instrument.serial.close)
 
-    ## Tear down test fixture ##
+    # Tear down test fixture #
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationOmegaSlave1(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -4900,15 +5158,15 @@
         self.instrument.write_register(4097, 700.0, 1)
         self.instrument.write_register(4097, 823.6, 1)
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationOmegaSlave10(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -4932,15 +5190,15 @@
         self.instrument.write_register(4097, 20.0, 1)
         self.instrument.write_register(4097, 200.0, 1)
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationDTB4824_RTU(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -4957,15 +5215,15 @@
     def testWriteBit(self) -> None:
         self.instrument.write_bit(0x0810, 1)  # "Communication write in enabled".
         self.instrument.write_bit(0x0814, 0)  # STOP
         self.instrument.write_bit(0x0814, 1)  # RUN
 
     def testReadBits(self) -> None:
         self.assertEqual(
-            self.instrument._perform_command(2, "\x08\x10\x00\x09"), "\x02\x07\x00"
+            self.instrument._perform_command(2, b"\x08\x10\x00\x09"), b"\x02\x07\x00"
         )
 
     def testReadRegister(self) -> None:
         # Process value (PV)
         self.assertEqual(self.instrument.read_register(0x1000), 64990)
         # Setpoint (SV)
         self.assertAlmostEqual(self.instrument.read_register(0x1001, 1), 80.0)
@@ -4997,15 +5255,15 @@
         self.instrument.write_register(0x1001, 0x0320, functioncode=6)
         self.instrument.write_register(0x1001, 25, 1, functioncode=6)  # Setpoint
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationDTB4824_ASCII(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -5024,15 +5282,15 @@
     def testWriteBit(self) -> None:
         self.instrument.write_bit(0x0810, 1)  # "Communication write in enabled".
         self.instrument.write_bit(0x0814, 0)  # STOP
         self.instrument.write_bit(0x0814, 1)  # RUN
 
     def testReadBits(self) -> None:
         self.assertEqual(
-            self.instrument._perform_command(2, "\x08\x10\x00\x09"), "\x02\x17\x00"
+            self.instrument._perform_command(2, b"\x08\x10\x00\x09"), b"\x02\x17\x00"
         )
 
     def testReadRegister(self) -> None:
         # Process value (PV)
         self.assertEqual(self.instrument.read_register(0x1000), 64990)
         # Setpoint (SV)
         self.assertAlmostEqual(self.instrument.read_register(0x1001, 1), 80.0)
@@ -5064,15 +5322,15 @@
         self.instrument.write_register(0x1001, 0x0320, functioncode=6)
         self.instrument.write_register(0x1001, 25, 1, functioncode=6)  # Setpoint
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationWithPortClosure(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -5095,15 +5353,15 @@
         self.assertEqual(self.instrument.serial.is_open, False)
         self.assertRaises(IOError, self.instrument.serial.close)
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestVerboseDummyCommunicationWithPortClosure(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = True
@@ -5116,15 +5374,55 @@
     def testReadRegister(self) -> None:
         self.assertEqual(self.instrument.read_register(289), 770)
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
+                pass
+        del self.instrument
+
+
+class TestVerboseDummyCommunicationNoBufferClearing(ExtendedTestCase):
+    def setUp(self) -> None:
+        dummy_serial.VERBOSE = True
+        dummy_serial.RESPONSES = RTU_RESPONSES
+        minimalmodbus.serial.Serial = dummy_serial.Serial  # type: ignore
+        self.instrument = minimalmodbus.Instrument("DUMMYPORTNAME", 1, debug=True)
+        self.instrument.clear_buffers_before_each_transaction = False
+
+    def testReadRegister(self) -> None:
+        self.assertEqual(self.instrument.read_register(289), 770)
+
+    def tearDown(self) -> None:
+        if self.instrument.serial is not None:
+            try:
+                self.instrument.serial.close()
+            except Exception:
+                pass
+        del self.instrument
+
+
+class TestVerboseDummyCommunicationNoCalculateReadSize(ExtendedTestCase):
+    def setUp(self) -> None:
+        dummy_serial.VERBOSE = True
+        dummy_serial.RESPONSES = RTU_RESPONSES
+        minimalmodbus.serial.Serial = dummy_serial.Serial  # type: ignore
+        self.instrument = minimalmodbus.Instrument("DUMMYPORTNAME", 1, debug=True)
+        self.instrument.precalculate_read_size = False
+
+    def testReadRegister(self) -> None:
+        self.assertEqual(self.instrument.read_register(289), 770)
+
+    def tearDown(self) -> None:
+        if self.instrument.serial is not None:
+            try:
+                self.instrument.serial.close()
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationBroadcast(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -5149,15 +5447,15 @@
     def testReadingNotAllowed(self) -> None:
         self.assertRaises(ValueError, self.instrument.read_register, 289)
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrument
 
 
 class TestDummyCommunicationThreeInstrumentsPortClosure(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = False
@@ -5186,29 +5484,29 @@
         self.assertEqual(self.instrumentB.read_register(289), 770)
         self.assertEqual(self.instrumentC.read_bit(0x0800), 0)
 
     def tearDown(self) -> None:
         if self.instrumentA.serial is not None:
             try:
                 self.instrumentA.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrumentA
 
         if self.instrumentB.serial is not None:
             try:
                 self.instrumentB.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrumentB
 
         if self.instrumentC.serial is not None:
             try:
                 self.instrumentC.serial.close()
-            except:
+            except Exception:
                 pass
         del self.instrumentC
 
 
 class TestDummyCommunicationHandleLocalEcho(ExtendedTestCase):
     def setUp(self) -> None:
         dummy_serial.VERBOSE = True
@@ -5225,39 +5523,88 @@
             minimalmodbus.LocalEchoError, self.instrument.read_register, 290
         )
 
     def tearDown(self) -> None:
         if self.instrument.serial is not None:
             try:
                 self.instrument.serial.close()
-            except:
+            except Exception:
+                pass
+        del self.instrument
+
+
+class TestDummyCommunicationExternalSerialPort(ExtendedTestCase):
+    def setUp(self) -> None:
+        dummy_serial.VERBOSE = True
+        dummy_serial.RESPONSES = RTU_RESPONSES
+        extserial = dummy_serial.Serial("DUMMYPORTNAME")
+        self.instrument = minimalmodbus.Instrument(extserial, 1)  # type: ignore
+
+    def testReadRegister(self) -> None:
+        self.assertEqual(self.instrument.read_register(289), 770)
+
+    def tearDown(self) -> None:
+        if self.instrument.serial is not None:
+            try:
+                self.instrument.serial.close()
+            except Exception:
                 pass
         del self.instrument
 
 
+class TestDummyCommunicationExternalSerialPortFailsToOpen(ExtendedTestCase):
+    def testInitialise(self) -> None:
+        extserial = dummy_serial.Serial("DUMMYPORTNAME", fail_to_open=True)
+        self.assertRaises(
+            minimalmodbus.MasterReportedException,
+            minimalmodbus.Instrument,
+            extserial,
+            1,
+        )
+
+
+class TestDummyCommunicationExternalSerialPortWrongType(ExtendedTestCase):
+    def testInitialiseSerialPortInteger(self) -> None:
+        extserial = 123
+        self.assertRaises(
+            minimalmodbus.MasterReportedException,
+            minimalmodbus.Instrument,
+            extserial,
+            1,
+        )
+
+    def testInitialiseSerialPortNone(self) -> None:
+        extserial = None
+        self.assertRaises(
+            minimalmodbus.MasterReportedException,
+            minimalmodbus.Instrument,
+            extserial,
+            1,
+        )
+
+
 RTU_RESPONSES: Dict[bytes, bytes] = {}
 GOOD_RTU_RESPONSES: Dict[bytes, bytes] = {}
 WRONG_RTU_RESPONSES: Dict[bytes, bytes] = {}
 ASCII_RESPONSES: Dict[bytes, bytes] = {}
 GOOD_ASCII_RESPONSES: Dict[bytes, bytes] = {}
 WRONG_ASCII_RESPONSES: Dict[bytes, bytes] = {}
 """A dictionary of respones from a dummy instrument.
 
-The key is the message (string) sent to the serial port, and the item is the response (string)
-from the dummy serial port.
-
+The key is the message (string) sent to the serial port, and the item is the response
+(string) from the dummy serial port.
 """
 # Note that the string 'AAAAAAA' might be easier to read if grouped,
 # like 'AA' + 'AAAA' + 'A' for the initial part (address etc) + payload + CRC.
 
 
 #                ##  READ BIT  ##
 
-# Read bit register 61 on slave 1 using function code 2. Also for testing _perform_command() #
-# ----------------------------------------------------------------------------------------- #
+# Read bit register 61 on slave 1 using function code 2. Also for _perform_command() #
+# ---------------------------------------------------------------------------------- #
 # Message:  Slave address 1, function code 2. Register address 61, 1 coil. CRC.
 # Response: Slave address 1, function code 2. 1 byte, value=1. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x02" + b"\x00\x3d\x00\x01" + b"(\x06"] = (
     b"\x01\x02" + b"\x01\x01" + b"`H"
 )
 
 # Read bit register 62 on slave 1 using function code 1 #
@@ -5299,76 +5646,81 @@
 # Response: Slave address 1, function code 5. Register address 71, value 0 (0000). CRC.
 GOOD_RTU_RESPONSES[b"\x01\x05" + b"\x00\x47\x00\x00" + b"}\xDF"] = (
     b"\x01\x05" + b"\x00\x47\x00\x00" + b"}\xDF"
 )
 
 # Write bit register 72 on slave 1 using function code 15 #
 # ------------------------------------------------------ #
-# Message:  Slave address 1, function code 15. Register address 72, 1 bit, 1 byte, value 1 (0100). CRC.
+# Message:  Slave address 1, function code 15. Register address 72, 1 bit, 1 byte,
+#           value 1 (0100). CRC.
 # Response: Slave address 1, function code 15. Register address 72, 1 bit. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x0f" + b"\x00\x48\x00\x01\x01\x01" + b"\x0fY"] = (
     b"\x01\x0f" + b"\x00\x48\x00\x01" + b"\x14\x1d"
 )
 
-# Write bit register 73 on slave 1 using function code 15, slave gives wrong number of registers #
-# ---------------------------------------------------------------------------------------------- #
-# Message:  Slave address 1, function code 15. Register address 73, 1 bit, 1 byte, value 1 (0100). CRC.
+# Write bit register 73 on slave 1 using function code 15, slave gives
+# wrong number of registers #
+# ----------------------------------------------------------------------------------- #
+# Message:  Slave address 1, function code 15. Register address 73, 1 bit, 1 byte,
+#           value 1 (0100). CRC.
 # Response: Slave address 1, function code 15. Register address 73, 2 bits (wrong). CRC.
 WRONG_RTU_RESPONSES[b"\x01\x0f" + b"\x00\x49\x00\x01\x01\x01" + b"2\x99"] = (
     b"\x01\x0f" + b"\x00\x49\x00\x02" + b"\x05\xdc"
 )
 
 # Write bit register 74 on slave 1 using function code 5, slave gives wrong write data #
 # ------------------------------------------------------------------------------------ #
 # Message:  Slave address 1, function code 5. Register address 74, value 1 (FF00). CRC.
-# Response: Slave address 1, function code 5. Register address 74, value 0 (0000, wrong). CRC.
+# Response: Slave address 1, function code 5. Register address 74, value 0 (0000,
+#           wrong). CRC.
 WRONG_RTU_RESPONSES[b"\x01\x05" + b"\x00\x4a\xff\x00" + b"\xad\xec"] = (
     b"\x01\x05" + b"\x00\x47\x00\x00" + b"}\xdf"
 )
 
 
 #                ##  READ BITS  ##
 
 # Read 19 bits starting at address 19 on slave 1 using function code 1.
 # Also for testing _perform_command()
 # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
-# ----------------------------------------------------------------------------------------- #
+# ----------------------------------------------------------------------------------- #
 # Message:  Slave address 1, function code 1. Register address 19, 19 coils. CRC.
 # Response: Slave address 1, function code 1. 3 bytes, values. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x01" + b"\x00\x13\x00\x13" + b"\x8c\x02"] = (
     b"\x01\x01" + b"\x03\xCD\x6B\x05" + b"B\x82"
 )
 
 # Read 22 bits starting at address 196 on slave 1 using function code 2.
 # Also for testing _perform_command()
 # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
-# ----------------------------------------------------------------------------------------- #
+# ----------------------------------------------------------------------------------- #
 # Message:  Slave address 1, function code 2. Register address 196, 22 coils. CRC.
 # Response: Slave address 1, function code 2. 3 bytes, values. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x02" + b"\x00\xC4\x00\x16" + b"\xB89"] = (
     b"\x01\x02" + b"\x03\xAC\xDB\x35" + b'"\x88'
 )
 
 # Read 16 bits starting at address 0x800 on slave 1 using function code 2.
 # Recorded on Delta DTB4824
-# ----------------------------------------------------------------------------------------- #
+# ----------------------------------------------------------------------------------- #
 # Message:  Slave address 1, function code 2. Register address 0x800, 16 coils. CRC.
 # Response: Slave address 1, function code 2. 2 bytes, values. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x02" + b"\x08\x00\x00\x10" + b"\x7B\xA6"] = (
     b"\x01\x02" + b"\x02\x20\x0f" + b"\xE0\x7C"
 )
 
 
 #                ##  WRITE BITS  ##
 
 # Write 10 bits starting at address 19 on slave 1 using function code 15.
 # Also for testing _perform_command()
 # Example from MODBUS APPLICATION PROTOCOL SPECIFICATION V1.1b
-# ----------------------------------------------------------------------------------------- #
-# Message:  Slave address 1, function code 15. Address 19, 10 coils, 2 bytes, values. CRC.
+# ----------------------------------------------------------------------------------- #
+# Message:  Slave address 1, function code 15. Address 19, 10 coils, 2 bytes,
+#           values. CRC.
 # Response: Slave address 1, function code 15. Address 19, 10 coils. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x0f" + b"\x00\x13\x00\x0A\x02\xCD\x01" + b"\x72\xCB"] = (
     b"\x01\x0f" + b"\x00\x13\x00\x0A" + b"$\t"
 )
 
 
 #                ##  READ REGISTER  ##
@@ -5395,16 +5747,17 @@
 # Response: Slave address 1, function code 4. 2 bytes, value=880. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x04" + b"\x00\x0e\x00\x01" + b"P\t"] = (
     b"\x01\x04" + b"\x02\x03\x70" + b"\xb8$"
 )
 
 # Read register 101 on slave 1 using function code 3 #
 # ---------------------------------------------------#
-# Message: Slave address 1, function code 3. Register address 101, 1 register. CRC.
-# Response: Slave address 1, function code 3. 2 bytes, value=-5 or 65531 (depending on interpretation). CRC
+# Message:  Slave address 1, function code 3. Register address 101, 1 register. CRC.
+# Response: Slave address 1, function code 3. 2 bytes, value=-5 or 65531 (depending
+#           on interpretation). CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00e\x00\x01" + b"\x94\x15"] = (
     b"\x01\x03" + b"\x02\xff\xfb" + b"\xb87"
 )
 
 # Read register 201 on slave 1 using function code 3 #
 # ---------------------------------------------------#
 # Message: Slave address 1, function code 3. Register address 201, 1 register. CRC.
@@ -5430,23 +5783,25 @@
 )
 
 
 #                ##  WRITE REGISTER  ##
 
 # Write value 50 in register 24 on slave 1 using function code 16 #
 # ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 24, 1 register, 2 bytes, value=50. CRC.
+# Message:  Slave address 1, function code 16. Register address 24, 1 register,
+#           2 bytes, value=50. CRC.
 # Response: Slave address 1, function code 16. Register address 24, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\x18\x00\x01\x02\x002" + b"$]"] = (
     b"\x01\x10" + b"\x00\x18\x00\x01" + b"\x81\xce"
 )
 
 # Write value 20 in register 35 on slave 1 using function code 16 #
 # ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 35, 1 register, 2 bytes, value=20. CRC.
+# Message:  Slave address 1, function code 16. Register address 35, 1 register,
+#           2 bytes, value=20. CRC.
 # Response: Slave address 1, function code 16. Register address 35, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00#\x00\x01" + b"\x02\x00\x14" + b"\xa1\x0c"] = (
     b"\x01\x10" + b"\x00#\x00\x01" + b"\xf0\x03"
 )
 
 # Write value 88 in register 45 on slave 1 using function code 6 #
 # ---------------------------------------------------------------#
@@ -5454,225 +5809,285 @@
 # Response: Slave address 1, function code 6. Register address 45, value=88. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x06" + b"\x00\x2d\x00\x58" + b"\x189"] = (
     b"\x01\x06" + b"\x00\x2d\x00\x58" + b"\x189"
 )
 
 # Write value 5 in register 101 on slave 1 using function code 16 #
 # ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 101, 1 register, 2 bytes, value=5. CRC.
+# Message:  Slave address 1, function code 16. Register address 101, 1 register,
+#           2 bytes, value=5. CRC.
 # Response: Slave address 1, function code 16. Register address 101, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00e\x00\x01\x02\x00\x05" + b"o\xa6"] = (
     b"\x01\x10" + b"\x00e\x00\x01" + b"\x11\xd6"
 )
 
 # Write value 50 in register 101 on slave 1 using function code 16 #
 # ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 101, 1 register, 2 bytes, value=5. CRC.
+# Message:  Slave address 1, function code 16. Register address 101, 1 register,
+#           2 bytes, value=5. CRC.
 # Response: Slave address 1, function code 16. Register address 101, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00e\x00\x01\x02\x002" + b".p"] = (
     b"\x01\x10" + b"\x00e\x00\x01" + b"\x11\xd6"
 )
 
 # Write value -5 in register 101 on slave 1 using function code 16 #
 # ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 101, 1 register, 2 bytes, value=-5. CRC.
+# Message:  Slave address 1, function code 16. Register address 101, 1 register,
+#           2 bytes, value=-5. CRC.
 # Response: Slave address 1, function code 16. Register address 101, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00e\x00\x01\x02\xff\xfb" + b"\xaf\xd6"] = (
     b"\x01\x10" + b"\x00e\x00\x01" + b"\x11\xd6"
 )
 
 # Write value -50 in register 101 on slave 1 using function code 16 #
-# ----------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 101, 1 register, 2 bytes, value=-50. CRC.
+# ----------------------------------------------------------------- #
+# Message:  Slave address 1, function code 16. Register address 101, 1 register,
+#           2 bytes, value=-50. CRC.
 # Response: Slave address 1, function code 16. Register address 101, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00e\x00\x01\x02\xff\xce" + b"o\xc1"] = (
     b"\x01\x10" + b"\x00e\x00\x01" + b"\x11\xd6"
 )
 
-# Write value 99 in register 51 on slave 1 using function code 16, slave gives wrong CRC #
-# ---------------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 51, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 1, function code 16. Register address 51, 1 register. Wrong CRC.
+# Write value 99 in register 51 on slave 1 using function code 16, slave gives
+# wrong CRC #
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 51, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 1, function code 16. Register address 51, 1 register.
+#           Wrong CRC.
 WRONG_RTU_RESPONSES[
     b"\x01\x10" + b"\x00\x33\x00\x01" + b"\x02\x00\x63" + b"\xe3\xba"
 ] = (b"\x01\x10" + b"\x00\x33\x00\x01" + b"AB")
 
-# Write value 99 in register 52 on slave 1 using function code 16, slave gives wrong number of registers #
-# -------------------------------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 52, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 1, function code 16. Register address 52, 2 registers (wrong). CRC.
+# Write value 99 in register 52 on slave 1 using function code 16, slave
+# gives wrong number of registers #
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 52, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 1, function code 16. Register address 52,
+#           2 registers (wrong). CRC.
 WRONG_RTU_RESPONSES[b"\x01\x10" + b"\x00\x34\x00\x01" + b"\x02\x00\x63" + b"\xe2\r"] = (
     b"\x01\x10" + b"\x00\x34\x00\x02" + b"\x00\x06"
 )
 
-# Write value 99 in register 53 on slave 1 using function code 16, slave gives wrong register address #
-# ----------------------------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 53, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 1, function code 16. Register address 54 (wrong), 1 register. CRC.
+# Write value 99 in register 53 on slave 1 using function code 16, slave
+# gives wrong register address #
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 53, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 1, function code 16. Register address 54 (wrong), 1 register.
+#           CRC.
 WRONG_RTU_RESPONSES[
     b"\x01\x10" + b"\x00\x35\x00\x01" + b"\x02\x00\x63" + b"\xe3\xdc"
 ] = (b"\x01\x10" + b"\x00\x36\x00\x01" + b"\xe1\xc7")
 
-# Write value 99 in register 54 on slave 1 using function code 16, slave gives wrong slave address #
-# ------------------------------------------------------------------------------------------------ #
-# Message:  Slave address 1, function code 16. Register address 54, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 2 (wrong), function code 16. Register address 54, 1 register. CRC.
+# Write value 99 in register 54 on slave 1 using function code 16, slave
+# gives wrong slave address #
+# ----------------------------------------------------------------------------------- #
+# Message:  Slave address 1, function code 16. Register address 54, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 2 (wrong), function code 16. Register address 54, 1 register.
+#           CRC.
 GOOD_RTU_RESPONSES[
     b"\x01\x10" + b"\x00\x36\x00\x01" + b"\x02\x00\x63" + b"\xe3\xef"
 ] = (b"\x02\x10" + b"\x00\x36\x00\x01" + b"\xe1\xf4")
 
-# Write value 99 in register 55 on slave 1 using function code 16, slave gives wrong functioncode #
-# ----------------------------------------------------------------------------------------------- #
-# Message:  Slave address 1, function code 16. Register address 55, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 1, function code 6 (wrong). Register address 55, 1 register. CRC.
+# Write value 99 in register 55 on slave 1 using function code 16, slave
+# gives wrong functioncode #
+# ----------------------------------------------------------------------------------- #
+# Message:  Slave address 1, function code 16. Register address 55, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 1, function code 6 (wrong). Register address 55, 1 register.
+#           CRC.
 WRONG_RTU_RESPONSES[b"\x01\x10" + b"\x00\x37\x00\x01" + b"\x02\x00\x63" + b"\xe2>"] = (
     b"\x01\x06" + b"\x00\x37\x00\x01" + b"\xf9\xc4"
 )
 
-# Write value 99 in register 56 on slave 1 using function code 16, slave gives wrong functioncode (indicates an error) #
-# -------------------------------------------------------------------------------------------------------------------- #
-# Message:  Slave address 1, function code 16. Register address 56, 1 register, 2 bytes, value=99. CRC.
-# Response: Slave address 1, function code 144 (wrong). Register address 56, 1 register. CRC.
+# Write value 99 in register 56 on slave 1 using function code 16, slave
+# gives wrong functioncode (indicates an error) #
+# ----------------------------------------------------------------------------------- #
+# Message:  Slave address 1, function code 16. Register address 56, 1 register,
+#           2 bytes, value=99. CRC.
+# Response: Slave address 1, function code 144 (wrong). Register address 56, 1 register.
+#           CRC.
 WRONG_RTU_RESPONSES[
     b"\x01\x10" + b"\x00\x38\x00\x01" + b"\x02\x00\x63" + b"\xe2\xc1"
 ] = (b"\x01\x90" + b"\x00\x38\x00\x01" + b"\x81\xda")
 
-# Write value 99 in register 55 on slave 1 using function code 6, slave gives wrong write data #
-# -------------------------------------------------------------------------------------------- #
+# Write value 99 in register 55 on slave 1 using function code 6, slave
+# gives wrong write data #
+# ----------------------------------------------------------------------------------- #
 # Message:  Slave address 1, function code 6. Register address 55, value=99. CRC.
-# Response: Slave address 1, function code 6. Register address 55, value=98 (wrong). CRC.
+# Response: Slave address 1, function code 6. Register address 55, value=98 (wrong).
+#           CRC.
 WRONG_RTU_RESPONSES[b"\x01\x06" + b"\x00\x37\x00\x63" + b"x-"] = (
     b"\x01\x06" + b"\x00\x37\x00\x62" + b"\xb9\xed"
 )
 
 #                ##  READ LONG ##
 
 # Read long (2 registers, starting at 102) on slave 1 using function code 3 #
 # --------------------------------------------------------------------------#
-# Message: Slave address 1, function code 3. Register address 289, 2 registers. CRC.
-# Response: Slave address 1, function code 3. 4 bytes, value=-1 or 4294967295 (depending on interpretation). CRC
+# Message:  Slave address 1, function code 3. Register address 102, 2 registers. CRC.
+# Response: Slave address 1, function code 3. 4 bytes, value=-1 or 4294967295
+#           (depending on interpretation). CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00f\x00\x02" + b"$\x14"] = (
     b"\x01\x03" + b"\x04\xff\xff\xff\xff" + b"\xfb\xa7"
 )
 
 # Read long (2 registers, starting at 223) on slave 1 using function code 3 #
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_BIG
-# --------------------------------------------------------------------------------------------#
+# ---------------------------------------------------------------------------------#
 # Message: Slave address 1, function code 3. Register address 223, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, Value 2923517522. CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xDF\x00\x02" + b"\xF5\xF1"] = (
     b"\x01\x03" + b"\x04\xAEAVR" + b"4\x92"
 )
 
 # Read long (2 registers, starting at 224) on slave 1 using function code 3 #
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_BIG_SWAP
-# --------------------------------------------------------------------------------------------#
+# ---------------------------------------------------------------------------------#
 # Message: Slave address 1, function code 3. Register address 224, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, Value 2923517522. CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xE0\x00\x02" + b"\xC5\xFD"] = (
     b"\x01\x03" + b"\x04A\xAERV" + b"2\xB0"
 )
 
 # Read long (2 registers, starting at 225) on slave 1 using function code 3 #
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_LITTLE_SWAP
-# --------------------------------------------------------------------------------------------#
+# --------------------------------------------------------------------------------#
 # Message: Slave address 1, function code 3. Register address 225, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, Value 2923517522. CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xE1\x00\x02" + b"\x94="] = (
     b"\x01\x03" + b"\x04VR\xAEA" + b"\xF6:"
 )
 
 # Read long (2 registers, starting at 226) on slave 1 using function code 3 #
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_LITTLE
-# --------------------------------------------------------------------------------------------#
+# ----------------------------------------------------------------------------------#
 # Message: Slave address 1, function code 3. Register address 226, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, Value 2923517522. CRC
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xE2\x00\x02" + b"\x64\x3D"] = (
     b"\x01\x03" + b"\x04RVA\xAE" + b"\xBBw"
 )
 
+# Read long (4 registers, starting at 108) on slave 1 using function code 3 #
+# --------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 3. Register address 108, 4 registers. CRC.
+# Response: Slave address 1, function code 3. 4 bytes, value=-2 or 18446744073709551614
+#           (depending on interpretation). CRC
+GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\x6c\x00\x04" + b"\x84\x14"] = (
+    b"\x01\x03" + b"\x08\xff\xff\xff\xff\xff\xff\xff\xfe" + b"\x15\x93"
+)
+
 
 #                ##  WRITE LONG ##
 
-# Write long (2 registers, starting at 102) on slave 1 using function code 16, with value 5. #
-# -------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 102, 2 registers, 4 bytes, value=5. CRC.
+# Write long (2 registers, starting at 102) on slave 1 using function code 16, with
+# value 5.
+# -----------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 102, 2 registers,
+#          4 bytes, value=5. CRC.
 # Response: Slave address 1, function code 16. Register address 102, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00f\x00\x02\x04\x00\x00\x00\x05" + b"\xb5\xae"] = (
     b"\x01\x10" + b"\x00f\x00\x02" + b"\xa1\xd7"
 )
 
-# Write long (2 registers, starting at 102) on slave 1 using function code 16, with value -5. #
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 102, 2 registers, 4 bytes, value=-5. CRC.
+# Write long (2 registers, starting at 102) on slave 1 using function code 16, with
+# value -5.
+# ------------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 102, 2 registers,
+#          4 bytes, value=-5. CRC.
 # Response: Slave address 1, function code 16. Register address 102, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00f\x00\x02\x04\xff\xff\xff\xfb" + b"u\xfa"] = (
     b"\x01\x10" + b"\x00f\x00\x02" + b"\xa1\xd7"
 )
 
-# Write long (2 registers, starting at 102) on slave 1 using function code 16, with value 3. #
-# -------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 102, 2 registers, 4 bytes, value=3. CRC.
+# Write long (2 registers, starting at 102) on slave 1 using function code 16, with
+# value 3. #
+# ------------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 102, 2 registers,
+#          4 bytes, value=3. CRC.
 # Response: Slave address 1, function code 16. Register address 102, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00f\x00\x02\x04\x00\x00\x00\x03" + b"5\xac"] = (
     b"\x01\x10" + b"\x00f\x00\x02" + b"\xa1\xd7"
 )
 
-# Write long (2 registers, starting at 102) on slave 1 using function code 16, with value -3. #
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 102, 2 registers, 4 bytes, value=-3. CRC.
+# Write long (2 registers, starting at 102) on slave 1 using function code 16, with
+# value -3. #
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 102, 2 registers,
+#           4 bytes, value=-3. CRC.
 # Response: Slave address 1, function code 16. Register address 102, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00f\x00\x02\x04\xff\xff\xff\xfd" + b"\xf5\xf8"] = (
     b"\x01\x10" + b"\x00f\x00\x02" + b"\xa1\xd7"
 )
 
-# Write long (2 registers, starting at 222) on slave 1 using function code 16, with value 2923517522 #
+# Write long (2 registers, starting at 222) on slave 1 using function code 16, with
+# value 2923517522
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_BIG
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 222, 2 registers, 4 bytes, value. CRC.
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 222, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 222, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xDE\x00\x02\x04\xAEAVR" + b"\xB1\xDE"] = (
     b"\x01\x10" + b"\x00\xDE\x00\x02" + b"\x21\xF2"
 )
 
-# Write long (2 registers, starting at 222) on slave 1 using function code 16, with value 2923517522 #
+# Write long (2 registers, starting at 222) on slave 1 using function code 16, with
+# value 2923517522
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_LITTLE
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 222, 2 registers, 4 bytes, value. CRC.
+# ------------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 222, 2 registers,
+#          4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 222, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xDE\x00\x02\x04RVA\xAE" + b"\x3E\x3B"] = (
     b"\x01\x10" + b"\x00\xDE\x00\x02" + b"\x21\xF2"
 )
 
-# Write long (2 registers, starting at 222) on slave 1 using function code 16, with value 2923517522 #
+# Write long (2 registers, starting at 222) on slave 1 using function code 16, with
+# value 2923517522
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_BIG_SWAP
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 222, 2 registers, 4 bytes, value. CRC.
+# ------------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 222, 2 registers,
+#          4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 222, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xDE\x00\x02\x04A\xAERV" + b"\xB7\xFC"] = (
     b"\x01\x10" + b"\x00\xDE\x00\x02" + b"\x21\xF2"
 )
 
-# Write long (2 registers, starting at 222) on slave 1 using function code 16, with value 2923517522 #
+# Write long (2 registers, starting at 222) on slave 1 using function code 16, with
+# value 2923517522
 # Example from https://www.simplymodbus.ca/FAQ.htm
 # Byte order BYTEORDER_LITTLE_SWAP
-# --------------------------------------------------------------------------------------------#
-# Message: Slave address 1, function code 16. Register address 222, 2 registers, 4 bytes, value. CRC.
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 222, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 222, 2 registers. CRC
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xDE\x00\x02\x04VR\xAEA" + b"sv"] = (
     b"\x01\x10" + b"\x00\xDE\x00\x02" + b"\x21\xF2"
 )
 
+# Write long (4 registers, starting at 109) on slave 1 using function code 16, with
+# value -4.
+# ------------------------------------------------------------------------------------#
+# Message: Slave address 1, function code 16. Register address 109, 4 registers,
+#          8 bytes, value=-4. CRC.
+# Response: Slave address 1, function code 16. Register address 109, 4 registers. CRC
+GOOD_RTU_RESPONSES[
+    b"\x01\x10" + b"\x00m\x00\x04\x08\xff\xff\xff\xff\xff\xff\xff\xfc" + b"\xda\xac"
+] = (b"\x01\x10" + b"\x00m\x00\x04" + b"P\x17")
+
 
 #                ##  READ FLOAT ##
 
 # Read float from address 103 (2 registers) on slave 1 using function code 3 #
 # ---------------------------------------------------------------------------#
 # Message:  Slave address 1, function code 3. Register address 103, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, value=1.0. CRC.
@@ -5703,105 +6118,131 @@
 # Message:  Slave address 1, function code 3. Register address 241, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, value=-4.3959787e-11 CRC.
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xF1\x00\x02" + b"\x95\xF8"] = (
     b"\x01\x03" + b"\x04\xAEAVR" + b"4\x92"
 )
 
 # Read float from address 242 (2 registers) on slave 1 using function code 3 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_BIG_SWAP
 # ---------------------------------------------------------------------------#
 # Message:  Slave address 1, function code 3. Register address 242, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, value=-4.3959787e-11 CRC.
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xF2\x00\x02" + b"\x65\xF8"] = (
     b"\x01\x03" + b"\x04A\xAERV" + b"2\xB0"
 )
 
 # Read float from address 243 (2 registers) on slave 1 using function code 3 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_LITTLE_SWAP
 # ---------------------------------------------------------------------------#
 # Message:  Slave address 1, function code 3. Register address 243, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, value=-4.3959787e-11 CRC.
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xF3\x00\x02" + b"\x34\x38"] = (
     b"\x01\x03" + b"\x04VR\xAEA" + b"\xf6:"
 )
 
 # Read float from address 244 (2 registers) on slave 1 using function code 3 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_LITTLE
 # ---------------------------------------------------------------------------#
 # Message:  Slave address 1, function code 3. Register address 244, 2 registers. CRC.
 # Response: Slave address 1, function code 3. 4 bytes, value=-4.3959787e-11 CRC.
 GOOD_RTU_RESPONSES[b"\x01\x03" + b"\x00\xF4\x00\x02" + b"\x85\xF9"] = (
     b"\x01\x03" + b"\x04RVA\xAE" + b"\xBBw"
 )
 
 
 #                ##  WRITE FLOAT ##
 
+# Write float 1.0 to address 107 (2 registers) on slave 1 using function code 16 #
+# -------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 107, 2 registers,
+#           4 bytes, value=1.1 . CRC.
+# Response: Slave address 1, function code 16. Register address 107, 2 registers. CRC.
+GOOD_RTU_RESPONSES[
+    b"\x01\x10" + b"\x00\x6b\x00\x02\x04\x3F\x80\x00\x00" + b"\xb9\xc8"
+] = (b"\x01\x10" + b"\x00\x6b\x00\x02" + b"0\x14")
+
 # Write float 1.1 to address 103 (2 registers) on slave 1 using function code 16 #
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 103, 2 registers, 4 bytes, value=1.1 . CRC.
+# Message:  Slave address 1, function code 16. Register address 103, 2 registers,
+#           4 bytes, value=1.1 . CRC.
 # Response: Slave address 1, function code 16. Register address 103, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00g\x00\x02\x04?\x8c\xcc\xcd" + b"\xed\x0b"] = (
     b"\x01\x10" + b"\x00g\x00\x02" + b"\xf0\x17"
 )
 
 # Write float 1.1 to address 103 (4 registers) on slave 1 using function code 16 #
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 103, 4 registers, 8 bytes, value=1.1 . CRC.
+# Message:  Slave address 1, function code 16. Register address 103, 4 registers,
+#           8 bytes, value=1.1 . CRC.
 # Response: Slave address 1, function code 16. Register address 103, 4 registers. CRC.
 GOOD_RTU_RESPONSES[
     b"\x01\x10" + b"\x00g\x00\x04\x08?\xf1\x99\x99\x99\x99\x99\x9a" + b"u\xf7"
 ] = (b"\x01\x10" + b"\x00g\x00\x04" + b"p\x15")
 
 # Write float 1.1 to address 103 (4 registers) on slave 1 using function code 16 #
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 103, 4 registers, 8 bytes, value=1.1 . CRC.
+# Message:  Slave address 1, function code 16. Register address 103, 4 registers,
+#           8 bytes, value=1.1 . CRC.
 # Response: Slave address 1, function code 16. Register address 103, 4 registers. CRC.
 GOOD_RTU_RESPONSES[
     b"\x01\x10" + b"\x00g\x00\x04\x08?\xf1\x99\x99\x99\x99\x99\x9a" + b"u\xf7"
 ] = (b"\x01\x10" + b"\x00g\x00\x04" + b"p\x15")
 
-# Write float -4.3959787e-11 to address 240 (42 registers) on slave 1 using function code 16 #
+# Write float -4.3959787e-11 to address 240 (2 registers) on slave 1 using
+# function code 16 #
 # Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page)
 # BYTEORDER_BIG
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 240, 2 registers, 4 bytes, value. CRC.
+# Message:  Slave address 1, function code 16. Register address 240, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 240, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xF0\x00\x02\x04\xAEAVR" + b"2J"] = (
     b"\x01\x10" + b"\x00\xF0\x00\x02" + b"A\xFB"
 )
 
-# Write float -4.3959787e-11 to address 240 (42 registers) on slave 1 using function code 16 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Write float -4.3959787e-11 to address 240 (2 registers) on slave 1 using
+# function code 16 #
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_LITTLE
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 240, 2 registers, 4 bytes, value. CRC.
+# Message:  Slave address 1, function code 16. Register address 240, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 240, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xF0\x00\x02\x04RVA\xAE" + b"\xBD\xAF"] = (
     b"\x01\x10" + b"\x00\xF0\x00\x02" + b"A\xFB"
 )
 
-# Write float -4.3959787e-11 to address 240 (42 registers) on slave 1 using function code 16 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Write float -4.3959787e-11 to address 240 (2 registers) on slave 1 using
+# function code 16 #
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_LITTLE_SWAP
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 240, 2 registers, 4 bytes, value. CRC.
+# Message:  Slave address 1, function code 16. Register address 240, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 240, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xF0\x00\x02\x04VR\xAEA" + b"\xF0\xE2"] = (
     b"\x01\x10" + b"\x00\xF0\x00\x02" + b"A\xFB"
 )
 
-# Write float -4.3959787e-11 to address 240 (42 registers) on slave 1 using function code 16 #
-# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page, manually reshuffled)
+# Write float -4.3959787e-11 to address 240 (2 registers) on slave 1 using
+# function code 16 #
+# Example from https://www.simplymodbus.ca/FAQ.htm (truncated float on page,
+# manually reshuffled)
 # BYTEORDER_BIG_SWAP
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 240, 2 registers, 4 bytes, value. CRC.
+# Message:  Slave address 1, function code 16. Register address 240, 2 registers,
+#           4 bytes, value. CRC.
 # Response: Slave address 1, function code 16. Register address 240, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00\xF0\x00\x02\x04A\xAERV" + b"4h"] = (
     b"\x01\x10" + b"\x00\xF0\x00\x02" + b"A\xFB"
 )
 
 
 #                ##  READ STRING  ##
@@ -5823,31 +6264,35 @@
 )
 
 
 #                ##  WRITE STRING  ##
 
 # Write string 'A' to address 104 (1 register) on slave 1 using function code 16 #
 # -------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 104, 1 register, 2 bytes, value='A ' . CRC.
+# Message:  Slave address 1, function code 16. Register address 104, 1 register,
+#           2 bytes, value='A ' . CRC.
 # Response: Slave address 1, function code 16. Register address 104, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00h\x00\x01\x02A " + b"\x9f0"] = (
     b"\x01\x10" + b"\x00h\x00\x01" + b"\x80\x15"
 )
 
 # Write string 'A' to address 104 (4 registers) on slave 1 using function code 16 #
 # --------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 104, 4 registers, 8 bytes, value='A       ' . CRC.
+# Message:  Slave address 1, function code 16. Register address 104, 4 registers,
+#           8 bytes, value='A       ' . CRC.
 # Response: Slave address 1, function code 16. Register address 104, 2 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00h\x00\x04\x08A       " + b"\xa7\xae"] = (
     b"\x01\x10" + b"\x00h\x00\x04" + b"@\x16"
 )
 
-# Write string 'ABCDEFGH' to address 104 (4 registers) on slave 1 using function code 16 #
-# ---------------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 104, 4 registers, 8 bytes, value='ABCDEFGH' . CRC.
+# Write string 'ABCDEFGH' to address 104 (4 registers) on slave 1 using
+# function code 16
+# ------------------------------------------------------------------------------------#
+# Message:  Slave address 1, function code 16. Register address 104, 4 registers,
+#           8 bytes, value='ABCDEFGH' . CRC.
 # Response: Slave address 1, function code 16. Register address 104, 4 registers. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00h\x00\x04\x08ABCDEFGH" + b"I>"] = (
     b"\x01\x10" + b"\x00h\x00\x04" + b"@\x16"
 )
 
 
 #                ##  READ REGISTERS  ##
@@ -5869,23 +6314,25 @@
 )
 
 
 #                ##  WRITE REGISTERS  ##
 
 # Write value [2] to address 105 (1 register) on slave 1 using function code 16 #
 # ------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 105, 1 register, 2 bytes, value=2 . CRC.
+# Message:  Slave address 1, function code 16. Register address 105, 1 register,
+#           2 bytes, value=2 . CRC.
 # Response: Slave address 1, function code 16. Register address 105, 1 register. CRC.
 GOOD_RTU_RESPONSES[b"\x01\x10" + b"\x00i\x00\x01\x02\x00\x02" + b".\xa8"] = (
     b"\x01\x10" + b"\x00i\x00\x01" + b"\xd1\xd5"
 )
 
 # Write value [2, 4, 8] to address 105 (3 registers) on slave 1 using function code 16 #
 # -------------------------------------------------------------------------------------#
-# Message:  Slave address 1, function code 16. Register address 105, 3 register, 6 bytes, value=2, 4, 8. CRC.
+# Message:  Slave address 1, function code 16. Register address 105, 3 register,
+#           6 bytes, value=2, 4, 8. CRC.
 # Response: Slave address 1, function code 16. Register address 105, 3 registers. CRC.
 GOOD_RTU_RESPONSES[
     b"\x01\x10" + b"\x00i\x00\x03\x06\x00\x02\x00\x04\x00\x08" + b"\x0c\xd6"
 ] = (b"\x01\x10" + b"\x00i\x00\x03" + b"P\x14")
 
 
 #                ##  OTHER RESPONSES  ##
@@ -5949,16 +6396,16 @@
     (b"\x14\x03" + b"\x01\x22\x00\x02" + b"\x27\x39")
     + b"\x14\x03"
     + b"\x02\x03\x02"
     + b"4\xb6"
 )
 
 
-## Recorded data from OmegaCN7500 ##
-####################################
+# Recorded data from OmegaCN7500 #
+##################################
 # (Sorted by slave address, register address)
 
 # Slave address 1, read_bit(2068) Response value 1.
 GOOD_RTU_RESPONSES[b"\x01\x02\x08\x14\x00\x01\xfb\xae"] = b"\x01\x02\x01\x01`H"
 
 # Slave address 1, write_bit(2068, 0)
 GOOD_RTU_RESPONSES[
@@ -6010,16 +6457,16 @@
 
 # Slave address 10, write_register(4097, 200.0, 1)
 GOOD_RTU_RESPONSES[
     b"\n\x10\x10\x01\x00\x01\x02\x07\xd0\xc6\xdc"
 ] = b"\n\x10\x10\x01\x00\x01U\xb2"
 
 
-## Recorded RTU data from Delta DTB4824 ##
-##########################################
+# Recorded RTU data from Delta DTB4824 #
+########################################
 # (Sorted by register number)
 
 # Slave address 7, read_bit(0x0800). This is LED AT.
 # Response value 0
 GOOD_RTU_RESPONSES[b"\x07\x02\x08\x00\x00\x01\xbb\xcc"] = b"\x07\x02\x01\x00\xa1\x00"
 
 # Slave address 7, read_bit(0x0801). This is LED Out1.
@@ -6031,15 +6478,16 @@
 GOOD_RTU_RESPONSES[b"\x07\x02\x08\x02\x00\x01\x1a\x0c"] = b"\x07\x02\x01\x00\xa1\x00"
 
 # Slave address 7, write_bit(0x0810, 1) This is "Communication write in enabled".
 GOOD_RTU_RESPONSES[
     b"\x07\x05\x08\x10\xff\x00\x8f\xf9"
 ] = b"\x07\x05\x08\x10\xff\x00\x8f\xf9"
 
-# Slave address 7, _perform_command(2, '\x08\x10\x00\x09'). This is reading 9 bits starting at 0x0810.
+# Slave address 7, _perform_command(2, '\x08\x10\x00\x09'). This is reading 9 bits
+# starting at 0x0810.
 # Response value '\x02\x07\x00'
 GOOD_RTU_RESPONSES[b"\x07\x02\x08\x10\x00\t\xbb\xcf"] = b"\x07\x02\x02\x07\x003\x88"
 
 # Slave address 7, read_bit(0x0814). This is RUN/STOP setting.
 # Response value 0
 GOOD_RTU_RESPONSES[b"\x07\x02\x08\x14\x00\x01\xfb\xc8"] = b"\x07\x02\x01\x00\xa1\x00"
 
@@ -6047,15 +6495,16 @@
 GOOD_RTU_RESPONSES[
     b"\x07\x05\x08\x14\x00\x00\x8f\xc8"
 ] = b"\x07\x05\x08\x14\x00\x00\x8f\xc8"
 
 # Slave address 7, write_bit(0x0814, 1). This is RUN.
 GOOD_RTU_RESPONSES[b"\x07\x05\x08\x14\xff\x00\xce8"] = b"\x07\x05\x08\x14\xff\x00\xce8"
 
-# Slave address 7, read_registers(0x1000, 2). This is process value (PV) and setpoint (SV).
+# Slave address 7, read_registers(0x1000, 2). This is process value (PV) and
+# setpoint (SV).
 # Response value [64990, 350]
 GOOD_RTU_RESPONSES[
     b"\x07\x03\x10\x00\x00\x02\xc0\xad"
 ] = b"\x07\x03\x04\xfd\xde\x01^M\xcd"
 
 # Slave address 7, read_register(0x1000). This is process value (PV).
 # Response value 64990
@@ -6068,15 +6517,16 @@
 GOOD_RTU_RESPONSES[b"\x07\x03\x10\x01\x00\x01\xd1l"] = b"\x07\x03\x02\x03 1l"
 
 # Slave address 7, write_register(0x1001, 25, 1, functioncode=6)
 GOOD_RTU_RESPONSES[
     b"\x07\x06\x10\x01\x00\xfa\\\xef"
 ] = b"\x07\x06\x10\x01\x00\xfa\\\xef"
 
-# Slave address 7, write_register(0x1001, 0x0320, functioncode=6) # Write value 800 to register 0x1001.
+# Slave address 7, write_register(0x1001, 0x0320, functioncode=6)
+# Write value 800 to register 0x1001.
 # This is a setpoint of 80.0 degrees (Centigrades, dependent on setting).
 GOOD_RTU_RESPONSES[b"\x07\x06\x10\x01\x03 \xdd\x84"] = b"\x07\x06\x10\x01\x03 \xdd\x84"
 
 # Slave address 7, read_register(0x1004). This is sensor type.
 # Response value 14
 GOOD_RTU_RESPONSES[b"\x07\x03\x10\x04\x00\x01\xc1m"] = b"\x07\x03\x02\x00\x0e\xb1\x80"
 
@@ -6111,31 +6561,32 @@
 GOOD_RTU_RESPONSES[b"\x07\x03\x10+\x00\x01\xf0\xa4"] = b"\x07\x03\x02\x00\x0fp@"
 
 # Slave address 7, read_register(0x102F). This is firmware version.
 # Response value 400
 GOOD_RTU_RESPONSES[b"\x07\x03\x10/\x00\x01\xb1e"] = b"\x07\x03\x02\x01\x901\xb8"
 
 
-## Recorded ASCII data from Delta DTB4824 ##
-############################################
+# Recorded ASCII data from Delta DTB4824 #
+##########################################
 # (Sorted by register number)
 
 # Slave address 7, read_bit(0x0800). This is LED AT.
 # Response value 0
 GOOD_ASCII_RESPONSES[b":070208000001EE\r\n"] = b":07020100F6\r\n"
 
 # Slave address 7, read_bit(0x0801). This is LED Out1.
 # Response value 1
 GOOD_ASCII_RESPONSES[b":070208010001ED\r\n"] = b":07020101F5\r\n"
 
 # Slave address 7, read_bit(0x0802). This is LED Out2.
 # Response value 0
 GOOD_ASCII_RESPONSES[b":070208020001EC\r\n"] = b":07020100F6\r\n"
 
-# Slave address 7, _perform_command(2, '\x08\x10\x00\x09'). This is reading 9 bits starting at 0x0810.
+# Slave address 7, _perform_command(2, '\x08\x10\x00\x09').
+# This is reading 9 bits starting at 0x0810.
 # Response value '\x02\x17\x00'
 GOOD_ASCII_RESPONSES[b":070208100009D6\r\n"] = b":0702021700DE\r\n"
 
 # Slave address 7, write_bit(0x0810, 1) This is "Communication write in enabled".
 GOOD_ASCII_RESPONSES[b":07050810FF00DD\r\n"] = b":07050810FF00DD\r\n"
 
 # Slave address 7, read_bit(0x0814). This is RUN/STOP setting.
@@ -6144,30 +6595,32 @@
 
 # Slave address 7, write_bit(0x0814, 0). This is STOP.
 GOOD_ASCII_RESPONSES[b":070508140000D8\r\n"] = b":070508140000D8\r\n"
 
 # Slave address 7, write_bit(0x0814, 1). This is RUN.
 GOOD_ASCII_RESPONSES[b":07050814FF00D9\r\n"] = b":07050814FF00D9\r\n"
 
-# Slave address 7, read_registers(0x1000, 2). This is process value (PV) and setpoint (SV).
+# Slave address 7, read_registers(0x1000, 2).
+# This is process value (PV) and setpoint (SV).
 # Response value [64990, 350]
 GOOD_ASCII_RESPONSES[b":070310000002E4\r\n"] = b":070304FDDE015EB8\r\n"
 
 # Slave address 7, read_register(0x1000). This is process value (PV).
 # Response value 64990
 GOOD_ASCII_RESPONSES[b":070310000001E5\r\n"] = b":070302FDDE19\r\n"
 
 # Slave address 7, read_register(0x1001, 1). This is setpoint (SV).
 # Response value 80.0
 GOOD_ASCII_RESPONSES[b":070310010001E4\r\n"] = b":0703020320D1\r\n"
 
 # Slave address 7, write_register(0x1001, 25, 1, functioncode=6)
 GOOD_ASCII_RESPONSES[b":0706100100FAE8\r\n"] = b":0706100100FAE8\r\n"
 
-# Slave address 7, write_register(0x1001, 0x0320, functioncode=6) # Write value 800 to register 0x1001.
+# Slave address 7, write_register(0x1001, 0x0320, functioncode=6)
+# Write value 800 to register 0x1001.
 # This is a setpoint of 80.0 degrees (Centigrades, dependent on setting).
 GOOD_ASCII_RESPONSES[b":070610010320BF\r\n"] = b":070610010320BF\r\n"
 
 # Slave address 7, read_register(0x1004). This is sensor type.
 # Response value 14
 GOOD_ASCII_RESPONSES[b":070310040001E1\r\n"] = b":070302000EE6\r\n"
 
@@ -6214,33 +6667,40 @@
 ASCII_RESPONSES.update(GOOD_ASCII_RESPONSES)
 
 #################
 # Run the tests #
 #################
 
 if __name__ == "__main__":
-
-    ## Run all tests ##
+    # Run all tests #
 
     unittest.main(verbosity=VERBOSITY)
 
-    ## Run a test class ##
+    # Run a test class #
 
-    # suite = unittest.TestLoader().loadTestsFromTestCase(TestDummyCommunicationHandleLocalEcho)
-    # suite = unittest.TestLoader().loadTestsFromTestCase(TestCalculateCrcString)
-    # suite = unittest.TestLoader().loadTestsFromTestCase(TestHexdecode)
-    # suite = unittest.TestLoader().loadTestsFromTestCase(TestDummyCommunicationBroadcast)
+    # suite = unittest.TestLoader().
+    # loadTestsFromTestCase(TestDummyCommunicationHandleLocalEcho)
+    # suite = unittest.TestLoader().loadTestsFromTestCase(TestCheckBytes)
+    # suite = unittest.TestLoader().loadTestsFromTestCase(TestPredictResponseSize)
+    # suite = unittest.TestLoader().
+    # loadTestsFromTestCase(TestDummyCommunicationBroadcast)
     # unittest.TextTestRunner(verbosity=2).run(suite)
 
-    ## Run a single test ##
+    # Run a single test #
 
     # suite = unittest.TestSuite()
-    # suite.addTest(TestDummyCommunication("testGenericCommand"))
+    # suite.addTest(("testGenericCommand"))
     # suite.addTest(TestDummyCommunication("testWriteBits"))
-    # suite.addTest(TestDummyCommunication("testReadBits"))
+    # suite.addTest(TestDummyCommunication("testReadLongWrongValue"))
     # suite.addTest(TestDummyCommunication("testWriteBit"))
     # suite.addTest(TestDummyCommunication("testWriteFloat"))
     # unittest.TextTestRunner(verbosity=2).run(suite)
 
-    ## Run individual commands ##
+    # Run individual commands #
 
-    # print(repr(minimalmodbus._calculate_crc_string('\x01\x05' + '\x00\x47\x00\x00')))
+    # print(
+    #     repr(
+    #         minimalmodbus._calculate_crc(
+    #             b"\x01\x10" + b"\x00m\x00\x04\x08\xff\xff\xff\xff\xff\xff\xff\xfc"
+    #         )
+    #     )
+    # )
```

