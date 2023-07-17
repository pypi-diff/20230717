# Comparing `tmp/ProxyPatternPool-5.0.tar.gz` & `tmp/ProxyPatternPool-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyPatternPool-5.0.tar", last modified: Fri Jun 16 10:17:52 2023, max compression
+gzip compressed data, was "ProxyPatternPool-6.0.tar", last modified: Mon Jul 17 05:40:25 2023, max compression
```

## Comparing `ProxyPatternPool-5.0.tar` & `ProxyPatternPool-6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/
--rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:31:46.000000 ProxyPatternPool-5.0/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)     7841 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/PKG-INFO
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     7841 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      251 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       98 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)       17 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/top_level.txt
--rw-------   0 fabien    (1001) fabien    (1001)    14612 2023-06-16 10:13:04.000000 ProxyPatternPool-5.0/ProxyPatternPool.py
--rw-------   0 fabien    (1001) fabien    (1001)     6951 2023-06-16 10:07:28.000000 ProxyPatternPool-5.0/README.md
--rw-------   0 fabien    (1001) fabien    (1001)     1095 2023-06-16 10:05:55.000000 ProxyPatternPool-5.0/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-17 05:40:25.012175 ProxyPatternPool-6.0/
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:31:46.000000 ProxyPatternPool-6.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)     8228 2023-07-17 05:40:25.012175 ProxyPatternPool-6.0/PKG-INFO
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-17 05:40:25.012175 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     8228 2023-07-17 05:40:25.000000 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      251 2023-07-17 05:40:25.000000 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-07-17 05:40:25.000000 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      127 2023-07-17 05:40:25.000000 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       17 2023-07-17 05:40:25.000000 ProxyPatternPool-6.0/ProxyPatternPool.egg-info/top_level.txt
+-rw-------   0 fabien    (1001) fabien    (1001)    15188 2023-07-17 05:18:48.000000 ProxyPatternPool-6.0/ProxyPatternPool.py
+-rw-------   0 fabien    (1001) fabien    (1001)     7338 2023-07-17 05:38:28.000000 ProxyPatternPool-6.0/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1217 2023-07-17 05:38:12.000000 ProxyPatternPool-6.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-07-17 05:40:25.012175 ProxyPatternPool-6.0/setup.cfg
```

### Comparing `ProxyPatternPool-5.0/PKG-INFO` & `ProxyPatternPool-6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProxyPatternPool
-Version: 5.0
+Version: 6.0
 Summary: Generic Proxy and Pool Classes for Python
 Author-email: Fabien Coelho <proxy.pool@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/proxy-pattern-pool
 Project-URL: documentation, https://zx80.github.io/proxy-pattern-pool/
 Project-URL: issues, https://github.com/zx80/proxy-pattern-pool/issues
 Project-URL: package, https://pypi.org/project/ProxyPatternPool/
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 # Proxy Pattern Pool
 
 Generic Proxy and Pool Classes for Python.
 
 ![Status](https://github.com/zx80/proxy-pattern-pool/actions/workflows/ppp.yml/badge.svg?branch=main&style=flat)
-![Tests](https://img.shields.io/badge/tests-8%20✓-success)
+![Tests](https://img.shields.io/badge/tests-9%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/proxy-pattern-pool?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/ProxyPatternPool)
 ![Badges](https://img.shields.io/badge/badges-8-informational)
 ![License](https://img.shields.io/pypi/l/proxypatternpool?style=flat)
 
@@ -74,16 +74,19 @@
 The `Proxy` constructors expects the following parameters:
 
 - `obj` one *single* object `SHARED` between all threads.
 - `fun` one function called for object creation, each time it is needed,
   for `THREAD` and `VERSATILE` scopes.
 - `scope` object scope as defined by `Proxy.Scope`:
   - `SHARED` one shared object (process level)
-  - `THREAD` one object per thread
-  - `VERSATILE` one object per sub-thread (eg greenlets)
+  - `THREAD` one object per thread (`threading` implementation)
+  - `WERKZEUG` one object per greenlet (`werkzeug` implementation)
+  - `EVENTLET` one object per greenlet (`eventlet` implementation)
+  - `GEVENT` one object per greenlet (`gevent` implementation)
+  - `VERSATILE` same as `WERKZEUG`
   default is `SHARED` or `THREAD` depending on whether an object
   of a function was passed for the object.
 - `set_name` the name of a function to set the proxy contents,
   default is `set`. This parameter allows to avoid collisions with
   the proxied methods.
   It is used as a prefix to have `set_obj` and `set_fun` functions
   which allow to reset the internal `obj` or `fun`.
@@ -171,14 +174,16 @@
 run in parallel is moot, thus the point of having a clever pool of stuff to be
 shared by these thread is even mooter!
 
 See Also:
 
 - [Psycopg Pool](https://www.psycopg.org/psycopg3/docs/advanced/pool.html)
   for pooling Postgres database connexions.
+- [Eventlet db_pool](https://eventlet.net/doc/modules/db_pool.html)
+  for pooling MySQL or Postgres database connexions.
 - [Discussion](https://github.com/brettwooldridge/HikariCP/wiki/About-Pool-Sizing)
   about database pool sizing.
 
 ## License
 
 This code is [Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).
 
@@ -187,14 +192,18 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
+### 6.0 on 2023-07-17
+
+Add support for more `local` scopes: `WERKZEUG`, `EVENTLET`, `GEVENT`.
+
 ### 5.0 on 2023-06-16
 
 Use `pyproject.toml` only.
 Require Python *3.10* for simpler code.
 
 ### 4.0 on 2023-02-05
 
@@ -227,11 +236,10 @@
 
 ### 0.1 on 2022-10-28
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
-- greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
 - add an actual timeout feature?
 - how to manage a return automatically?
```

### Comparing `ProxyPatternPool-5.0/ProxyPatternPool.egg-info/PKG-INFO` & `ProxyPatternPool-6.0/ProxyPatternPool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProxyPatternPool
-Version: 5.0
+Version: 6.0
 Summary: Generic Proxy and Pool Classes for Python
 Author-email: Fabien Coelho <proxy.pool@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/proxy-pattern-pool
 Project-URL: documentation, https://zx80.github.io/proxy-pattern-pool/
 Project-URL: issues, https://github.com/zx80/proxy-pattern-pool/issues
 Project-URL: package, https://pypi.org/project/ProxyPatternPool/
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 # Proxy Pattern Pool
 
 Generic Proxy and Pool Classes for Python.
 
 ![Status](https://github.com/zx80/proxy-pattern-pool/actions/workflows/ppp.yml/badge.svg?branch=main&style=flat)
-![Tests](https://img.shields.io/badge/tests-8%20✓-success)
+![Tests](https://img.shields.io/badge/tests-9%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/proxy-pattern-pool?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/ProxyPatternPool)
 ![Badges](https://img.shields.io/badge/badges-8-informational)
 ![License](https://img.shields.io/pypi/l/proxypatternpool?style=flat)
 
@@ -74,16 +74,19 @@
 The `Proxy` constructors expects the following parameters:
 
 - `obj` one *single* object `SHARED` between all threads.
 - `fun` one function called for object creation, each time it is needed,
   for `THREAD` and `VERSATILE` scopes.
 - `scope` object scope as defined by `Proxy.Scope`:
   - `SHARED` one shared object (process level)
-  - `THREAD` one object per thread
-  - `VERSATILE` one object per sub-thread (eg greenlets)
+  - `THREAD` one object per thread (`threading` implementation)
+  - `WERKZEUG` one object per greenlet (`werkzeug` implementation)
+  - `EVENTLET` one object per greenlet (`eventlet` implementation)
+  - `GEVENT` one object per greenlet (`gevent` implementation)
+  - `VERSATILE` same as `WERKZEUG`
   default is `SHARED` or `THREAD` depending on whether an object
   of a function was passed for the object.
 - `set_name` the name of a function to set the proxy contents,
   default is `set`. This parameter allows to avoid collisions with
   the proxied methods.
   It is used as a prefix to have `set_obj` and `set_fun` functions
   which allow to reset the internal `obj` or `fun`.
@@ -171,14 +174,16 @@
 run in parallel is moot, thus the point of having a clever pool of stuff to be
 shared by these thread is even mooter!
 
 See Also:
 
 - [Psycopg Pool](https://www.psycopg.org/psycopg3/docs/advanced/pool.html)
   for pooling Postgres database connexions.
+- [Eventlet db_pool](https://eventlet.net/doc/modules/db_pool.html)
+  for pooling MySQL or Postgres database connexions.
 - [Discussion](https://github.com/brettwooldridge/HikariCP/wiki/About-Pool-Sizing)
   about database pool sizing.
 
 ## License
 
 This code is [Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).
 
@@ -187,14 +192,18 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
+### 6.0 on 2023-07-17
+
+Add support for more `local` scopes: `WERKZEUG`, `EVENTLET`, `GEVENT`.
+
 ### 5.0 on 2023-06-16
 
 Use `pyproject.toml` only.
 Require Python *3.10* for simpler code.
 
 ### 4.0 on 2023-02-05
 
@@ -227,11 +236,10 @@
 
 ### 0.1 on 2022-10-28
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
-- greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
 - add an actual timeout feature?
 - how to manage a return automatically?
```

### Comparing `ProxyPatternPool-5.0/ProxyPatternPool.py` & `ProxyPatternPool-6.0/ProxyPatternPool.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,17 @@
         - VERSATILE: sub-thread-level object (eg greenlet), generated by a function.
         """
 
         AUTO = 0
         SHARED = 1
         THREAD = 2
         VERSATILE = 3
+        WERKZEUG = 3
+        GEVENT = 4
+        EVENTLET = 5
 
     def __init__(
         self,
         obj: Any = None,
         set_name: str = "set",
         fun: Callable[[int], Any] = None,
         max_size: int = 0,
@@ -323,32 +326,46 @@
         self._local.obj = obj
         return self
 
     def _set_fun(self, fun: Callable[[int], Any]):
         """Set current wrapped object generation function."""
         if self._scope == Proxy.Scope.AUTO:
             self._scope = Proxy.Scope.THREAD
-        assert self._scope in (Proxy.Scope.THREAD, Proxy.Scope.VERSATILE)
+        assert self._scope in (Proxy.Scope.THREAD, Proxy.Scope.VERSATILE,
+            Proxy.Scope.WERKZEUG, Proxy.Scope.EVENTLET, Proxy.Scope.GEVENT)
         self._fun = fun
         self._pool = Pool(fun,
                           max_size=self._pool_max_size,
                           min_size=self._pool_min_size,
                           timeout=self._pool_timeout,
                           max_use=self._pool_max_use,
                           max_avail_delay=self._pool_max_avail_delay,
                           max_using_delay=self._pool_max_using_delay,
                           close=self._close) \
             if self._pool_max_size is not None else None  # fmt: skip
         self._nobjs = 0
+
+        # local implementtion
         if self._scope == Proxy.Scope.THREAD:
             self._local = threading.local()
-        else:  # Proxy.Scope.VERSATILE
+        elif self._scope == Proxy.Scope.WERKZEUG:
             from werkzeug.local import Local
 
             self._local = Local()
+        elif self._scope == Proxy.Scope.GEVENT:
+            from gevent.local import local  # type: ignore
+
+            self._local = local()
+        elif self._scope == Proxy.Scope.EVENTLET:
+            from eventlet.corolocal import local  # type: ignore
+
+            self._local = local()
+        else:  # pragma: no cover
+            raise Exception(f"unexpected local scope: {self._scope}")
+
         return self
 
     def _set(
         self,
         obj: Any = None,
         fun: Callable[[int], Any]|None = None,
         mandatory=True,
```

### Comparing `ProxyPatternPool-5.0/README.md` & `ProxyPatternPool-6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Proxy Pattern Pool
 
 Generic Proxy and Pool Classes for Python.
 
 ![Status](https://github.com/zx80/proxy-pattern-pool/actions/workflows/ppp.yml/badge.svg?branch=main&style=flat)
-![Tests](https://img.shields.io/badge/tests-8%20✓-success)
+![Tests](https://img.shields.io/badge/tests-9%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/proxy-pattern-pool?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/ProxyPatternPool)
 ![Badges](https://img.shields.io/badge/badges-8-informational)
 ![License](https://img.shields.io/pypi/l/proxypatternpool?style=flat)
 
@@ -52,16 +52,19 @@
 The `Proxy` constructors expects the following parameters:
 
 - `obj` one *single* object `SHARED` between all threads.
 - `fun` one function called for object creation, each time it is needed,
   for `THREAD` and `VERSATILE` scopes.
 - `scope` object scope as defined by `Proxy.Scope`:
   - `SHARED` one shared object (process level)
-  - `THREAD` one object per thread
-  - `VERSATILE` one object per sub-thread (eg greenlets)
+  - `THREAD` one object per thread (`threading` implementation)
+  - `WERKZEUG` one object per greenlet (`werkzeug` implementation)
+  - `EVENTLET` one object per greenlet (`eventlet` implementation)
+  - `GEVENT` one object per greenlet (`gevent` implementation)
+  - `VERSATILE` same as `WERKZEUG`
   default is `SHARED` or `THREAD` depending on whether an object
   of a function was passed for the object.
 - `set_name` the name of a function to set the proxy contents,
   default is `set`. This parameter allows to avoid collisions with
   the proxied methods.
   It is used as a prefix to have `set_obj` and `set_fun` functions
   which allow to reset the internal `obj` or `fun`.
@@ -149,14 +152,16 @@
 run in parallel is moot, thus the point of having a clever pool of stuff to be
 shared by these thread is even mooter!
 
 See Also:
 
 - [Psycopg Pool](https://www.psycopg.org/psycopg3/docs/advanced/pool.html)
   for pooling Postgres database connexions.
+- [Eventlet db_pool](https://eventlet.net/doc/modules/db_pool.html)
+  for pooling MySQL or Postgres database connexions.
 - [Discussion](https://github.com/brettwooldridge/HikariCP/wiki/About-Pool-Sizing)
   about database pool sizing.
 
 ## License
 
 This code is [Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).
 
@@ -165,14 +170,18 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
+### 6.0 on 2023-07-17
+
+Add support for more `local` scopes: `WERKZEUG`, `EVENTLET`, `GEVENT`.
+
 ### 5.0 on 2023-06-16
 
 Use `pyproject.toml` only.
 Require Python *3.10* for simpler code.
 
 ### 4.0 on 2023-02-05
 
@@ -205,11 +214,10 @@
 
 ### 0.1 on 2022-10-28
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
-- greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
 - add an actual timeout feature?
 - how to manage a return automatically?
```

### Comparing `ProxyPatternPool-5.0/pyproject.toml` & `ProxyPatternPool-6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ProxyPatternPool"
-version = "5.0"
+version = "6.0"
 authors = [ { name = "Fabien Coelho", email = "proxy.pool@coelho.net" } ]
 description = "Generic Proxy and Pool Classes for Python"
 readme = "README.md"
 license = { text = "CC0" }
 requires-python = ">= 3.10"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -24,10 +24,11 @@
 issues = "https://github.com/zx80/proxy-pattern-pool/issues"
 package = "https://pypi.org/project/ProxyPatternPool/"
 
 [tool.setuptools]
 py-modules = [ "ProxyPatternPool" ]
 
 [project.optional-dependencies]
-local = [ "werkzeug" ]
+# NOTE greenlet has strange undeclared dependencies on import, hence "cryptography"
+local = [ "werkzeug", "eventlet", "gevent", "cryptography" ]
 dev = [ "mypy", "flake8", "black", "pytest", "coverage", "pymarkdownlnt" ]
 pub = [ "build", "wheel", "twine" ]
```

