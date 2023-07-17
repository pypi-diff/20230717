# Comparing `tmp/minimalmodbus-2.1.0.tar.gz` & `tmp/minimalmodbus-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimalmodbus-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "minimalmodbus-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `minimalmodbus-2.1.0.tar` & `minimalmodbus-2.1.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0       57 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/.flake8
--rw-r--r--   0        0        0     1508 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      410 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/.gitignore
--rw-r--r--   0        0        0      624 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/AUTHORS.rst
--rw-r--r--   0        0        0      369 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/CITATION.cff
--rw-r--r--   0        0        0     3843 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     5569 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/HISTORY.rst
--rw-r--r--   0        0        0    10100 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/LICENSE
--rw-r--r--   0        0        0     3231 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/Makefile
--rw-r--r--   0        0        0     2324 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/README.rst
--rw-r--r--   0        0        0     6810 2021-08-05 16:14:45.083858 minimalmodbus-2.1.0/docs/Makefile
--rw-r--r--   0        0        0    13631 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/advancedusage.rst
--rw-r--r--   0        0        0      219 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/apidummyserial.rst
--rw-r--r--   0        0        0      152 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/apiminimalmodbus.rst
--rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/authors.rst
--rwxr-xr-x   0        0        0     3001 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/conf.py
--rw-r--r--   0        0        0       33 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     5248 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/debugmode.rst
--rw-r--r--   0        0        0    27218 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/develop.rst
--rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/history.rst
--rw-r--r--   0        0        0      745 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/index.rst
--rw-r--r--   0        0        0     1312 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/installation.rst
--rw-r--r--   0        0        0      229 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internalminimalmodbus.rst
--rw-r--r--   0        0        0      340 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/internaltestdtb4824.rst
--rw-r--r--   0        0        0      230 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internaltestminimalmodbus.rst
--rw-r--r--   0        0        0      174 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/internaltoc.rst
--rw-r--r--   0        0        0    20566 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/modbusdetails.rst
--rw-r--r--   0        0        0       27 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/readme.rst
--rw-r--r--   0        0        0     1651 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/docs/related.rst
--rw-r--r--   0        0        0     7098 2023-07-17 18:10:01.747841 minimalmodbus-2.1.0/docs/serialcommunication.rst
--rw-r--r--   0        0        0     3786 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/troubleshooting.rst
--rw-r--r--   0        0        0     7976 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/docs/usage.rst
--rw-r--r--   0        0        0   134115 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/minimalmodbus.py
--rw-r--r--   0        0        0     2230 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1257 2021-08-10 20:22:44.985071 minimalmodbus-2.1.0/stubs/serial.pyi
--rwxr-xr-x   0        0        0      708 2021-08-05 16:14:45.087858 minimalmodbus-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     9266 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/dummy_serial.py
--rw-r--r--   0        0        0    13361 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/test_deltaDTB4824.py
--rw-r--r--   0        0        0   240866 2023-07-17 18:10:01.751841 minimalmodbus-2.1.0/tests/test_minimalmodbus.py
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 minimalmodbus-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/.flake8
+-rw-r--r--   0        0        0     1508 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      410 2021-08-05 16:14:45.083858 minimalmodbus-2.1.1/.gitignore
+-rw-r--r--   0        0        0      426 2023-07-17 19:16:25.108128 minimalmodbus-2.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      624 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0      369 2023-07-17 19:37:05.637433 minimalmodbus-2.1.1/CITATION.cff
+-rw-r--r--   0        0        0     3843 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5672 2023-07-17 19:37:05.637433 minimalmodbus-2.1.1/HISTORY.rst
+-rw-r--r--   0        0        0    10100 2021-08-05 16:14:45.083858 minimalmodbus-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3231 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/Makefile
+-rw-r--r--   0        0        0     2324 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/README.rst
+-rw-r--r--   0        0        0     6810 2021-08-05 16:14:45.083858 minimalmodbus-2.1.1/docs/Makefile
+-rw-r--r--   0        0        0    13631 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/advancedusage.rst
+-rw-r--r--   0        0        0      219 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/apidummyserial.rst
+-rw-r--r--   0        0        0      152 2021-08-10 20:22:44.985071 minimalmodbus-2.1.1/docs/apiminimalmodbus.rst
+-rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/authors.rst
+-rwxr-xr-x   0        0        0     3001 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0     5248 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/debugmode.rst
+-rw-r--r--   0        0        0    27218 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/develop.rst
+-rw-r--r--   0        0        0       28 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/history.rst
+-rw-r--r--   0        0        0      745 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/index.rst
+-rw-r--r--   0        0        0     1312 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/installation.rst
+-rw-r--r--   0        0        0      229 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/internalminimalmodbus.rst
+-rw-r--r--   0        0        0      340 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/internaltestdtb4824.rst
+-rw-r--r--   0        0        0      230 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/internaltestminimalmodbus.rst
+-rw-r--r--   0        0        0      174 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/internaltoc.rst
+-rw-r--r--   0        0        0    20566 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/modbusdetails.rst
+-rw-r--r--   0        0        0       27 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/readme.rst
+-rw-r--r--   0        0        0     1651 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/docs/related.rst
+-rw-r--r--   0        0        0       37 2023-07-17 19:16:25.108128 minimalmodbus-2.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0     7098 2023-07-17 18:10:01.747841 minimalmodbus-2.1.1/docs/serialcommunication.rst
+-rw-r--r--   0        0        0     3786 2021-08-10 20:22:44.985071 minimalmodbus-2.1.1/docs/troubleshooting.rst
+-rw-r--r--   0        0        0     7976 2021-08-10 20:22:44.985071 minimalmodbus-2.1.1/docs/usage.rst
+-rw-r--r--   0        0        0   134115 2023-07-17 19:37:05.641433 minimalmodbus-2.1.1/minimalmodbus.py
+-rw-r--r--   0        0        0     2230 2023-07-17 18:10:01.751841 minimalmodbus-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1257 2021-08-10 20:22:44.985071 minimalmodbus-2.1.1/stubs/serial.pyi
+-rwxr-xr-x   0        0        0      708 2021-08-05 16:14:45.087858 minimalmodbus-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     9266 2023-07-17 18:10:01.751841 minimalmodbus-2.1.1/tests/dummy_serial.py
+-rw-r--r--   0        0        0    13361 2023-07-17 18:10:01.751841 minimalmodbus-2.1.1/tests/test_deltaDTB4824.py
+-rw-r--r--   0        0        0   240866 2023-07-17 18:10:01.751841 minimalmodbus-2.1.1/tests/test_minimalmodbus.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 minimalmodbus-2.1.1/PKG-INFO
```

### Comparing `minimalmodbus-2.1.0/.github/workflows/build.yml` & `minimalmodbus-2.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/AUTHORS.rst` & `minimalmodbus-2.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/CONTRIBUTING.rst` & `minimalmodbus-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/HISTORY.rst` & `minimalmodbus-2.1.1/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 History
 =======
 
+Release 2.1.1 (2023-07-17)
+--------------------------
+* Added a .readthedocs.yaml configuration file.
+
 Release 2.1.0 (2023-07-17)
 --------------------------
 New features:
 
 * Support for 64-bit integers in read_long() and write_long().
 * Allow an external serial port object to be used in the Instrument constructor.
```

### Comparing `minimalmodbus-2.1.0/LICENSE` & `minimalmodbus-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/Makefile` & `minimalmodbus-2.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/README.rst` & `minimalmodbus-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/Makefile` & `minimalmodbus-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/advancedusage.rst` & `minimalmodbus-2.1.1/docs/advancedusage.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/conf.py` & `minimalmodbus-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/debugmode.rst` & `minimalmodbus-2.1.1/docs/debugmode.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/develop.rst` & `minimalmodbus-2.1.1/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/index.rst` & `minimalmodbus-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/installation.rst` & `minimalmodbus-2.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/modbusdetails.rst` & `minimalmodbus-2.1.1/docs/modbusdetails.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/related.rst` & `minimalmodbus-2.1.1/docs/related.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/serialcommunication.rst` & `minimalmodbus-2.1.1/docs/serialcommunication.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/troubleshooting.rst` & `minimalmodbus-2.1.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/docs/usage.rst` & `minimalmodbus-2.1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/minimalmodbus.py` & `minimalmodbus-2.1.1/minimalmodbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #   limitations under the License.
 #
 """MinimalModbus: A Python driver for Modbus RTU/ASCII via serial port."""
 
 __author__ = "Jonas Berg"
 __license__ = "Apache License, Version 2.0"
 __url__ = "https://github.com/pyhys/minimalmodbus"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 import sys
 
 if sys.version_info < (3, 8, 0):
     raise ImportError(
         "Your Python version is too old for this version of MinimalModbus"
     )
```

### Comparing `minimalmodbus-2.1.0/pyproject.toml` & `minimalmodbus-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/stubs/serial.pyi` & `minimalmodbus-2.1.1/stubs/serial.pyi`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/tests/__init__.py` & `minimalmodbus-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/tests/dummy_serial.py` & `minimalmodbus-2.1.1/tests/dummy_serial.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/tests/test_deltaDTB4824.py` & `minimalmodbus-2.1.1/tests/test_deltaDTB4824.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/tests/test_minimalmodbus.py` & `minimalmodbus-2.1.1/tests/test_minimalmodbus.py`

 * *Files identical despite different names*

### Comparing `minimalmodbus-2.1.0/PKG-INFO` & `minimalmodbus-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimalmodbus
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easy-to-use Modbus RTU and Modbus ASCII implementation for Python
 Keywords: minimalmodbus,modbus,modbus-serial,modbus-RTU,modbus-ASCII
 Author: Jonas Berg
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

