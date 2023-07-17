# Comparing `tmp/python_adjudicator-0.3.2.tar.gz` & `tmp/python_adjudicator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.3.2.tar", max compression
+gzip compressed data, was "python_adjudicator-0.4.0.tar", max compression
```

## Comparing `python_adjudicator-0.3.2.tar` & `python_adjudicator-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/LICENSE
--rw-r--r--   0        0        0     3579 2023-06-29 22:15:04.639380 python_adjudicator-0.3.2/README.md
--rw-r--r--   0        0        0     2041 2023-06-29 22:15:59.549824 python_adjudicator-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2119 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3214 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/Executor.py
--rw-r--r--   0        0        0     1530 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     7246 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/Params.py
--rw-r--r--   0        0        0     1054 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     5978 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/RuleEngine.py
--rw-r--r--   0        0        0     2741 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/RuleEngine_test.py
--rw-r--r--   0        0        0     5460 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/RuleGraph.py
--rw-r--r--   0        0        0     3932 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/RuleGraph_test.py
--rw-r--r--   0        0        0      426 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      828 2023-06-29 22:15:59.553824 python_adjudicator-0.3.2/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1462 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/py.typed
--rw-r--r--   0        0        0     6856 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/rule.py
--rw-r--r--   0        0        0      824 2023-06-29 16:54:45.263854 python_adjudicator-0.3.2/src/adjudicator/rule_test.py
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 python_adjudicator-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3579 2023-07-17 15:10:52.894100 python_adjudicator-0.4.0/README.md
+-rw-r--r--   0        0        0     2041 2023-07-17 15:11:19.010444 python_adjudicator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2119 2023-06-21 22:55:41.840466 python_adjudicator-0.4.0/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3214 2023-06-21 22:55:41.841814 python_adjudicator-0.4.0/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-06-21 22:55:41.842426 python_adjudicator-0.4.0/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     7246 2023-06-21 22:55:41.842936 python_adjudicator-0.4.0/src/adjudicator/Params.py
+-rw-r--r--   0        0        0     1054 2023-06-21 22:55:41.843369 python_adjudicator-0.4.0/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     5978 2023-06-21 22:55:41.844148 python_adjudicator-0.4.0/src/adjudicator/RuleEngine.py
+-rw-r--r--   0        0        0     2741 2023-06-21 22:55:41.844722 python_adjudicator-0.4.0/src/adjudicator/RuleEngine_test.py
+-rw-r--r--   0        0        0     5460 2023-06-21 22:55:41.845250 python_adjudicator-0.4.0/src/adjudicator/RuleGraph.py
+-rw-r--r--   0        0        0     3932 2023-06-21 22:55:41.845569 python_adjudicator-0.4.0/src/adjudicator/RuleGraph_test.py
+-rw-r--r--   0        0        0      426 2023-06-21 22:55:41.847616 python_adjudicator-0.4.0/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      828 2023-07-17 15:11:19.010584 python_adjudicator-0.4.0/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-21 22:55:41.848771 python_adjudicator-0.4.0/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-06-21 22:55:41.849105 python_adjudicator-0.4.0/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     6856 2023-06-21 22:56:10.537884 python_adjudicator-0.4.0/src/adjudicator/rule.py
+-rw-r--r--   0        0        0      824 2023-06-21 22:56:15.991531 python_adjudicator-0.4.0/src/adjudicator/rule_test.py
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 python_adjudicator-0.4.0/PKG-INFO
```

### Comparing `python_adjudicator-0.3.2/LICENSE` & `python_adjudicator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/README.md` & `python_adjudicator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/pyproject.toml` & `python_adjudicator-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 # Documentation = ""
 Homepage = "https://github.com/NiklasRosenstein/python-adjudicator"
 Repository = "https://github.com/NiklasRosenstein/python-adjudicator"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 networkx = "^3.1"
-typeapi = "^1.4.2"
+typeapi = "^2.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pycln = "^2.1.3"
```

### Comparing `python_adjudicator-0.3.2/src/adjudicator/Cache.py` & `python_adjudicator-0.4.0/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/Executor.py` & `python_adjudicator-0.4.0/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/HashSupport.py` & `python_adjudicator-0.4.0/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/Params.py` & `python_adjudicator-0.4.0/src/adjudicator/Params.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/Params_test.py` & `python_adjudicator-0.4.0/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/RuleEngine.py` & `python_adjudicator-0.4.0/src/adjudicator/RuleEngine.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/RuleEngine_test.py` & `python_adjudicator-0.4.0/src/adjudicator/RuleEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/RuleGraph.py` & `python_adjudicator-0.4.0/src/adjudicator/RuleGraph.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/RuleGraph_test.py` & `python_adjudicator-0.4.0/src/adjudicator/RuleGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/__init__.py` & `python_adjudicator-0.4.0/src/adjudicator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     "RuleResolveError",
     "RuleTypes",
     "union_rule",
     "union",
     "UnionRule",
 ]
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
```

### Comparing `python_adjudicator-0.3.2/src/adjudicator/errors.py` & `python_adjudicator-0.4.0/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/rule.py` & `python_adjudicator-0.4.0/src/adjudicator/rule.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/src/adjudicator/rule_test.py` & `python_adjudicator-0.4.0/src/adjudicator/rule_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.3.2/PKG-INFO` & `python_adjudicator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: typeapi (>=1.4.2,<2.0.0)
+Requires-Dist: typeapi (>=2.1.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-adjudicator/issues
 Project-URL: Homepage, https://github.com/NiklasRosenstein/python-adjudicator
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-adjudicator
 Description-Content-Type: text/markdown
 
 # adjudicator
```

