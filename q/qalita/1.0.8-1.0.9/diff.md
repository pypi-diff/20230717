# Comparing `tmp/qalita-1.0.8.tar.gz` & `tmp/qalita-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.8.tar", max compression
+gzip compressed data, was "qalita-1.0.9.tar", max compression
```

## Comparing `qalita-1.0.8.tar` & `qalita-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-16 19:42:01.762683 qalita-1.0.8/LICENSE
--rw-r--r--   0        0        0     1942 2023-07-16 19:42:01.762683 qalita-1.0.8/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-16 19:42:12.015592 qalita-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 19:42:01.783683 qalita-1.0.8/qalita/__init__.py
--rw-r--r--   0        0        0     4189 2023-07-16 19:42:12.016592 qalita-1.0.8/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-16 19:42:01.784683 qalita-1.0.8/qalita/commands/__init__.py
--rw-r--r--   0        0        0    19666 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/agent.py
--rw-r--r--   0        0        0    14531 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/pack.py
--rw-r--r--   0        0        0     9756 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-16 19:42:01.784683 qalita-1.0.8/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/internal/utils.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-16 19:52:17.634353 qalita-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1942 2023-07-16 19:52:17.635353 qalita-1.0.9/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-16 19:52:28.934563 qalita-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/__init__.py
+-rw-r--r--   0        0        0     4189 2023-07-16 19:52:28.936563 qalita-1.0.9/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    19666 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14531 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9756 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-16 19:52:17.636353 qalita-1.0.9/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-16 19:52:17.636353 qalita-1.0.9/qalita/internal/utils.py
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.9/PKG-INFO
```

### Comparing `qalita-1.0.8/LICENSE` & `qalita-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/docs/README.md` & `qalita-1.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/pyproject.toml` & `qalita-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.8"
+version = "1.0.9"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.8/qalita/cli.py` & `qalita-1.0.9/qalita/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-    logger.info(f"Version : 1.0.8")
+    logger.info(f"Version : 1.0.9")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.8/qalita/commands/agent.py` & `qalita-1.0.9/qalita/commands/agent.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/qalita/commands/pack.py` & `qalita-1.0.9/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/qalita/commands/source.py` & `qalita-1.0.9/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/qalita/internal/logger.py` & `qalita-1.0.9/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/qalita/internal/utils.py` & `qalita-1.0.9/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.8/PKG-INFO` & `qalita-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.8
+Version: 1.0.9
 Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

