# Comparing `tmp/escribalogger-1.0.tar.gz` & `tmp/escribalogger-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escribalogger-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "escribalogger-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `escribalogger-1.0.tar` & `escribalogger-1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3852 2023-07-16 20:17:55.333708 escribalogger-1.0/README.md
--rw-r--r--   0        0        0      734 2023-07-16 20:24:26.500860 escribalogger-1.0/pyproject.toml
--rw-r--r--   0        0        0      267 2023-07-15 23:49:49.033618 escribalogger-1.0/src/EscribaLogger/DPSingleton.py
--rw-r--r--   0        0        0     3606 2023-07-16 18:25:32.945977 escribalogger-1.0/src/EscribaLogger/Log.py
--rw-r--r--   0        0        0       43 2023-07-15 23:53:52.869434 escribalogger-1.0/src/EscribaLogger/__init__.py
--rw-r--r--   0        0        0     1706 2023-07-16 18:27:07.438466 escribalogger-1.0/src/EscribaLogger/drivers.py
--rw-r--r--   0        0        0      286 2023-07-16 15:30:58.059955 escribalogger-1.0/src/EscribaLogger/process_extra_context.py
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 escribalogger-1.0/PKG-INFO
+-rw-r--r--   0        0        0     3852 2023-07-16 20:17:55.333708 escribalogger-1.1/README.md
+-rw-r--r--   0        0        0      902 2023-07-16 22:39:27.743937 escribalogger-1.1/pyproject.toml
+-rw-r--r--   0        0        0      267 2023-07-15 23:49:49.033618 escribalogger-1.1/src/EscribaLogger/DPSingleton.py
+-rw-r--r--   0        0        0     3606 2023-07-16 18:25:32.945977 escribalogger-1.1/src/EscribaLogger/Log.py
+-rw-r--r--   0        0        0       43 2023-07-15 23:53:52.869434 escribalogger-1.1/src/EscribaLogger/__init__.py
+-rw-r--r--   0        0        0     1706 2023-07-16 18:27:07.438466 escribalogger-1.1/src/EscribaLogger/drivers.py
+-rw-r--r--   0        0        0      286 2023-07-16 15:30:58.059955 escribalogger-1.1/src/EscribaLogger/process_extra_context.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 escribalogger-1.1/PKG-INFO
```

### Comparing `escribalogger-1.0/README.md` & `escribalogger-1.1/README.md`

 * *Files identical despite different names*

### Comparing `escribalogger-1.0/src/EscribaLogger/Log.py` & `escribalogger-1.1/src/EscribaLogger/Log.py`

 * *Files identical despite different names*

### Comparing `escribalogger-1.0/src/EscribaLogger/drivers.py` & `escribalogger-1.1/src/EscribaLogger/drivers.py`

 * *Files identical despite different names*

### Comparing `escribalogger-1.0/PKG-INFO` & `escribalogger-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: EscribaLogger
-Version: 1.0
+Version: 1.1
 Summary: A fast 'read to use' Logging system which provides stdout/file/custom stream with easy syntax and operation. It's a very simple approach of Laravel drivers sorts, by the way, handlers ands drivers are both the same
+Keywords: logging,logger,log,logs,drivers
 Author-email: Thiago Santa Clara Pereira <strovsk@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Dist: markdown-it-py==3.0.0
+Requires-Dist: mdurl==0.1.2
+Requires-Dist: Pygments==2.15.1
+Requires-Dist: rich==13.4.2
 Project-URL: Github, https://github.com/Strovsk/EscribaLogger
 
 # Get Started
 
 ## install
 
 `python -m pip install EscribaLogger`
```

