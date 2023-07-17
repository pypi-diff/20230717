# Comparing `tmp/quickfix-ch-0.0.8.tar.gz` & `tmp/quickfix-ch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfix-ch-0.0.8.tar", last modified: Fri Jun 16 16:20:05 2023, max compression
+gzip compressed data, was "quickfix-ch-0.0.9.tar", last modified: Mon Jul 17 07:24:51 2023, max compression
```

## Comparing `quickfix-ch-0.0.8.tar` & `quickfix-ch-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,83 @@
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.287624 quickfix-ch-0.0.8/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:20:05.287380 quickfix-ch-0.0.8/PKG-INFO
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.283903 quickfix-ch-0.0.8/quickfix/
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:08:17.000000 quickfix-ch-0.0.8/quickfix/__init__.py
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.13.so
--rwxr-xr-x   0 javierphon   (503) staff       (20)     1000 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.la
--rwxr-xr-x   0 javierphon   (503) staff       (20) 11192092 2023-06-16 07:59:51.000000 quickfix-ch-0.0.8/quickfix/_quickfix.so
--rw-r--r--   0 javierphon   (503) staff       (20)  2064378 2023-06-16 16:08:31.000000 quickfix-ch-0.0.8/quickfix/quickfix.py
--rw-r--r--   0 javierphon   (503) staff       (20)     4839 2023-06-16 16:18:28.000000 quickfix-ch-0.0.8/quickfix/quickfix40.py
--rw-r--r--   0 javierphon   (503) staff       (20)     6246 2023-06-16 16:18:38.000000 quickfix-ch-0.0.8/quickfix/quickfix41.py
--rw-r--r--   0 javierphon   (503) staff       (20)    21594 2023-06-16 16:18:47.000000 quickfix-ch-0.0.8/quickfix/quickfix42.py
--rw-r--r--   0 javierphon   (503) staff       (20)    64755 2023-06-16 16:18:54.000000 quickfix-ch-0.0.8/quickfix/quickfix43.py
--rw-r--r--   0 javierphon   (503) staff       (20)   262998 2023-06-16 16:19:04.000000 quickfix-ch-0.0.8/quickfix/quickfix44.py
--rw-r--r--   0 javierphon   (503) staff       (20)   380012 2023-06-16 16:19:16.000000 quickfix-ch-0.0.8/quickfix/quickfix50.py
--rw-r--r--   0 javierphon   (503) staff       (20)   449416 2023-06-16 16:19:21.000000 quickfix-ch-0.0.8/quickfix/quickfix50sp1.py
--rw-r--r--   0 javierphon   (503) staff       (20)   532358 2023-06-16 16:19:28.000000 quickfix-ch-0.0.8/quickfix/quickfix50sp2.py
--rw-r--r--   0 javierphon   (503) staff       (20)     1237 2023-06-16 16:19:34.000000 quickfix-ch-0.0.8/quickfix/quickfixt11.py
-drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-06-16 16:20:05.286557 quickfix-ch-0.0.8/quickfix_ch.egg-info/
--rw-r--r--   0 javierphon   (503) staff       (20)      576 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/PKG-INFO
--rw-r--r--   0 javierphon   (503) staff       (20)      473 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/SOURCES.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/dependency_links.txt
--rw-r--r--   0 javierphon   (503) staff       (20)        9 2023-06-16 16:20:05.000000 quickfix-ch-0.0.8/quickfix_ch.egg-info/top_level.txt
--rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-06-16 16:20:05.287914 quickfix-ch-0.0.8/setup.cfg
--rw-r--r--   0 javierphon   (503) staff       (20)      951 2023-06-16 16:20:01.000000 quickfix-ch-0.0.8/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-07-17 07:24:51.556954 quickfix-ch-0.0.9/
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-07-17 07:24:51.544887 quickfix-ch-0.0.9/C++/
+-rw-rw-r--   0 javierphon   (503) staff       (20)     6017 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Acceptor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    22902 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/DataDictionary.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2177 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/DataDictionaryProvider.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     4276 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Dictionary.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2840 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/FieldConvertors.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     6486 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/FieldMap.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     1649 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/FieldTypes.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5305 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/FileLog.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     9889 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/FileStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     1676 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Group.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    23438 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/HttpConnection.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5372 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/HttpMessage.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     1326 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/HttpParser.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     3550 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/HttpServer.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7059 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Initiator.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2082 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Log.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    20184 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Message.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2463 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/MessageSorters.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     4333 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/MessageStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7679 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/MySQLLog.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    11615 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/MySQLStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     1319 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/NullStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     6848 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/OdbcLog.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    11551 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/OdbcStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2718 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/PUGIXML_DOMDocument.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2580 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Parser.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7803 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/PostgreSQLLog.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    11770 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/PostgreSQLStore.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20) 11214247 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/C++/QuickfixPython.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    12933 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SSLSocketAcceptor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    12202 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SSLSocketConnection.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    15020 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SSLSocketInitiator.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    45474 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Session.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    10740 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SessionFactory.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5522 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SessionSettings.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     4446 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Settings.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     6084 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketAcceptor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5476 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketConnection.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     3321 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketConnector.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     8014 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketInitiator.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7546 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketMonitor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     4516 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/SocketServer.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    14400 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSSLSocketAcceptor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    11658 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSSLSocketConnection.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    14021 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSSLSocketInitiator.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7079 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSocketAcceptor.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5074 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSocketConnection.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     7694 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/ThreadedSocketInitiator.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     5209 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/TimeRange.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    11744 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/Utility.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)    43883 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/UtilitySSL.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)   277412 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/C++/pugixml.cpp
+-rw-rw-r--   0 javierphon   (503) staff       (20)     2073 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/LICENSE
+-rw-r--r--   0 javierphon   (503) staff       (20)     2813 2023-07-17 07:24:51.556779 quickfix-ch-0.0.9/PKG-INFO
+-rw-rw-r--   0 javierphon   (503) staff       (20)  2059807 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)     4825 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix40.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)     6232 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix41.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)    21580 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix42.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)    64741 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix43.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)   262984 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix44.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)   379998 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix50.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)   449402 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix50sp1.py
+-rw-rw-r--   0 javierphon   (503) staff       (20)   532344 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfix50sp2.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-07-17 07:24:51.546600 quickfix-ch-0.0.9/quickfix_ch.egg-info/
+-rw-r--r--   0 javierphon   (503) staff       (20)     2813 2023-07-17 07:24:51.000000 quickfix-ch-0.0.9/quickfix_ch.egg-info/PKG-INFO
+-rw-r--r--   0 javierphon   (503) staff       (20)     1582 2023-07-17 07:24:51.000000 quickfix-ch-0.0.9/quickfix_ch.egg-info/SOURCES.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)        1 2023-07-17 07:24:51.000000 quickfix-ch-0.0.9/quickfix_ch.egg-info/dependency_links.txt
+-rw-r--r--   0 javierphon   (503) staff       (20)      125 2023-07-17 07:24:51.000000 quickfix-ch-0.0.9/quickfix_ch.egg-info/top_level.txt
+-rw-rw-r--   0 javierphon   (503) staff       (20)     1223 2018-04-16 04:16:16.000000 quickfix-ch-0.0.9/quickfixt11.py
+-rw-r--r--   0 javierphon   (503) staff       (20)       38 2023-07-17 07:24:51.557016 quickfix-ch-0.0.9/setup.cfg
+-rw-r--r--   0 javierphon   (503) staff       (20)     2576 2023-07-17 07:23:50.000000 quickfix-ch-0.0.9/setup.py
+drwxr-xr-x   0 javierphon   (503) staff       (20)        0 2023-07-17 07:24:51.555981 quickfix-ch-0.0.9/spec/
+-rw-rw-r--   0 javierphon   (503) staff       (20)    37498 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX40.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)    58446 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX41.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   130005 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX42.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   209984 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX43.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   320230 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX44.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   396303 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX50.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   468015 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX50SP1.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)   494424 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIX50SP2.xml
+-rw-rw-r--   0 javierphon   (503) staff       (20)    16354 2018-04-16 04:16:17.000000 quickfix-ch-0.0.9/spec/FIXT11.xml
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix.py` & `quickfix-ch-0.0.9/quickfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 3.0.12
+# Version 3.0.10
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
+
+
+
+
 from sys import version_info as _swig_python_version_info
 if _swig_python_version_info >= (2, 7, 0):
     def swig_import_helper():
         import importlib
         pkg = __name__.rpartition('.')[0]
         mname = '.'.join((pkg, '_quickfix')).lstrip('.')
         try:
@@ -22,26 +26,25 @@
         import imp
         fp = None
         try:
             fp, pathname, description = imp.find_module('_quickfix', [dirname(__file__)])
         except ImportError:
             import _quickfix
             return _quickfix
-        try:
-            _mod = imp.load_module('_quickfix', fp, pathname, description)
-        finally:
-            if fp is not None:
+        if fp is not None:
+            try:
+                _mod = imp.load_module('_quickfix', fp, pathname, description)
+            finally:
                 fp.close()
-        return _mod
+            return _mod
     _quickfix = swig_import_helper()
     del swig_import_helper
 else:
     import _quickfix
 del _swig_python_version_info
-
 try:
     _swig_property = property
 except NameError:
     pass  # Python < 2.2 doesn't have 'property'.
 
 try:
     import builtins as __builtin__
@@ -98,78 +101,14 @@
 try:
     import weakref
     weakref_proxy = weakref.proxy
 except __builtin__.Exception:
     weakref_proxy = lambda x: x
 
 
-class SwigPyIterator(_object):
-    __swig_setmethods__ = {}
-    __setattr__ = lambda self, name, value: _swig_setattr(self, SwigPyIterator, name, value)
-    __swig_getmethods__ = {}
-    __getattr__ = lambda self, name: _swig_getattr(self, SwigPyIterator, name)
-
-    def __init__(self, *args, **kwargs):
-        raise AttributeError("No constructor defined - class is abstract")
-    __repr__ = _swig_repr
-    __swig_destroy__ = _quickfix.delete_SwigPyIterator
-    __del__ = lambda self: None
-
-    def value(self):
-        return _quickfix.SwigPyIterator_value(self)
-
-    def incr(self, n=1):
-        return _quickfix.SwigPyIterator_incr(self, n)
-
-    def decr(self, n=1):
-        return _quickfix.SwigPyIterator_decr(self, n)
-
-    def distance(self, x):
-        return _quickfix.SwigPyIterator_distance(self, x)
-
-    def equal(self, x):
-        return _quickfix.SwigPyIterator_equal(self, x)
-
-    def copy(self):
-        return _quickfix.SwigPyIterator_copy(self)
-
-    def next(self):
-        return _quickfix.SwigPyIterator_next(self)
-
-    def __next__(self):
-        return _quickfix.SwigPyIterator___next__(self)
-
-    def previous(self):
-        return _quickfix.SwigPyIterator_previous(self)
-
-    def advance(self, n):
-        return _quickfix.SwigPyIterator_advance(self, n)
-
-    def __eq__(self, x):
-        return _quickfix.SwigPyIterator___eq__(self, x)
-
-    def __ne__(self, x):
-        return _quickfix.SwigPyIterator___ne__(self, x)
-
-    def __iadd__(self, n):
-        return _quickfix.SwigPyIterator___iadd__(self, n)
-
-    def __isub__(self, n):
-        return _quickfix.SwigPyIterator___isub__(self, n)
-
-    def __add__(self, n):
-        return _quickfix.SwigPyIterator___add__(self, n)
-
-    def __sub__(self, *args):
-        return _quickfix.SwigPyIterator___sub__(self, *args)
-    def __iter__(self):
-        return self
-SwigPyIterator_swigregister = _quickfix.SwigPyIterator_swigregister
-SwigPyIterator_swigregister(SwigPyIterator)
-
 class IntArray(_object):
     __swig_setmethods__ = {}
     __setattr__ = lambda self, name, value: _swig_setattr(self, IntArray, name, value)
     __swig_getmethods__ = {}
     __getattr__ = lambda self, name: _swig_getattr(self, IntArray, name)
     __repr__ = _swig_repr
 
@@ -197,106 +136,14 @@
 IntArray_swigregister = _quickfix.IntArray_swigregister
 IntArray_swigregister(IntArray)
 
 def IntArray_frompointer(t):
     return _quickfix.IntArray_frompointer(t)
 IntArray_frompointer = _quickfix.IntArray_frompointer
 
-class SessionIDSet(_object):
-    __swig_setmethods__ = {}
-    __setattr__ = lambda self, name, value: _swig_setattr(self, SessionIDSet, name, value)
-    __swig_getmethods__ = {}
-    __getattr__ = lambda self, name: _swig_getattr(self, SessionIDSet, name)
-    __repr__ = _swig_repr
-
-    def iterator(self):
-        return _quickfix.SessionIDSet_iterator(self)
-    def __iter__(self):
-        return self.iterator()
-
-    def __nonzero__(self):
-        return _quickfix.SessionIDSet___nonzero__(self)
-
-    def __bool__(self):
-        return _quickfix.SessionIDSet___bool__(self)
-
-    def __len__(self):
-        return _quickfix.SessionIDSet___len__(self)
-
-    def append(self, x):
-        return _quickfix.SessionIDSet_append(self, x)
-
-    def __contains__(self, x):
-        return _quickfix.SessionIDSet___contains__(self, x)
-
-    def __getitem__(self, i):
-        return _quickfix.SessionIDSet___getitem__(self, i)
-
-    def add(self, x):
-        return _quickfix.SessionIDSet_add(self, x)
-
-    def discard(self, x):
-        return _quickfix.SessionIDSet_discard(self, x)
-
-    def __init__(self, *args):
-        this = _quickfix.new_SessionIDSet(*args)
-        try:
-            self.this.append(this)
-        except __builtin__.Exception:
-            self.this = this
-
-    def empty(self):
-        return _quickfix.SessionIDSet_empty(self)
-
-    def size(self):
-        return _quickfix.SessionIDSet_size(self)
-
-    def clear(self):
-        return _quickfix.SessionIDSet_clear(self)
-
-    def swap(self, v):
-        return _quickfix.SessionIDSet_swap(self, v)
-
-    def count(self, x):
-        return _quickfix.SessionIDSet_count(self, x)
-
-    def begin(self):
-        return _quickfix.SessionIDSet_begin(self)
-
-    def end(self):
-        return _quickfix.SessionIDSet_end(self)
-
-    def rbegin(self):
-        return _quickfix.SessionIDSet_rbegin(self)
-
-    def rend(self):
-        return _quickfix.SessionIDSet_rend(self)
-
-    def erase(self, *args):
-        return _quickfix.SessionIDSet_erase(self, *args)
-
-    def find(self, x):
-        return _quickfix.SessionIDSet_find(self, x)
-
-    def lower_bound(self, x):
-        return _quickfix.SessionIDSet_lower_bound(self, x)
-
-    def upper_bound(self, x):
-        return _quickfix.SessionIDSet_upper_bound(self, x)
-
-    def equal_range(self, x):
-        return _quickfix.SessionIDSet_equal_range(self, x)
-
-    def insert(self, __x):
-        return _quickfix.SessionIDSet_insert(self, __x)
-    __swig_destroy__ = _quickfix.delete_SessionIDSet
-    __del__ = lambda self: None
-SessionIDSet_swigregister = _quickfix.SessionIDSet_swigregister
-SessionIDSet_swigregister(SessionIDSet)
-
 class FIXException(Exception):
     __swig_setmethods__ = {}
     __setattr__ = lambda self, name, value: _swig_setattr(self, FIXException, name, value)
     __swig_getmethods__ = {}
     __getattr__ = lambda self, name: _swig_getattr(self, FIXException, name)
     __repr__ = _swig_repr
 
@@ -40171,15 +40018,15 @@
     self.settings = settings
     self.logFactory = logFactory
 #endif
 
 # This file is compatible with both classic and new-style classes.
 
 
-from quickfix import quickfix
+import quickfix
 
 class BeginSeqNo(quickfix.IntField):
 	def __init__(self, data = None):
 		if data == None:
 			quickfix.IntField.__init__(self, 7)
 		else:
 			quickfix.IntField.__init__(self, 7, data)
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix40.py` & `quickfix-ch-0.0.9/quickfix40.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.0") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix41.py` & `quickfix-ch-0.0.9/quickfix41.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.1") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix42.py` & `quickfix-ch-0.0.9/quickfix42.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.2") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix43.py` & `quickfix-ch-0.0.9/quickfix43.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.3") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix44.py` & `quickfix-ch-0.0.9/quickfix44.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIX.4.4") )
 
 class Heartbeat(Message):
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix50.py` & `quickfix-ch-0.0.9/quickfix50.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("7") )
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix50sp1.py` & `quickfix-ch-0.0.9/quickfix50sp1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("8") )
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfix50sp2.py` & `quickfix-ch-0.0.9/quickfix50sp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 		self.getHeader().setField( fix.ApplVerID("9") )
```

### Comparing `quickfix-ch-0.0.8/quickfix/quickfixt11.py` & `quickfix-ch-0.0.9/quickfixt11.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quickfix import quickfix as fix
+import quickfix as fix
 
 class Message(fix.Message):
 	def __init__(self):
 		fix.Message.__init__(self)
 		self.getHeader().setField( fix.BeginString("FIXT.1.1") )
 
 class Heartbeat(Message):
```

