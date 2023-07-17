# Comparing `tmp/ploomber-engine-0.0.8.tar.gz` & `tmp/ploomber-engine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-engine-0.0.8.tar", last modified: Sun Aug 21 02:22:13 2022, max compression
+gzip compressed data, was "ploomber-engine-0.0.9.tar", last modified: Tue Aug 23 03:55:51 2022, max compression
```

## Comparing `ploomber-engine-0.0.8.tar` & `ploomber-engine-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-21 02:22:13.815664 ploomber-engine-0.0.8/
--rw-r--r--   0 Edu        (503) staff       (20)     1444 2022-08-21 02:22:11.000000 ploomber-engine-0.0.8/CHANGELOG.md
--rw-r--r--   0 Edu        (503) staff       (20)     1826 2022-08-21 00:14:04.000000 ploomber-engine-0.0.8/LICENSE
--rw-r--r--   0 Edu        (503) staff       (20)      247 2022-07-19 22:24:03.000000 ploomber-engine-0.0.8/MANIFEST.in
--rw-r--r--   0 Edu        (503) staff       (20)      101 2022-08-21 02:22:13.815793 ploomber-engine-0.0.8/PKG-INFO
--rw-r--r--   0 Edu        (503) staff       (20)     3344 2022-08-13 15:26:08.000000 ploomber-engine-0.0.8/README.md
--rw-r--r--   0 Edu        (503) staff       (20)      127 2022-07-21 00:23:47.000000 ploomber-engine-0.0.8/pyproject.toml
--rw-r--r--   0 Edu        (503) staff       (20)      106 2022-08-21 02:22:13.816305 ploomber-engine-0.0.8/setup.cfg
--rw-r--r--   0 Edu        (503) staff       (20)     1430 2022-08-21 00:14:04.000000 ploomber-engine-0.0.8/setup.py
-drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-21 02:22:13.808239 ploomber-engine-0.0.8/src/
-drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-21 02:22:13.813068 ploomber-engine-0.0.8/src/ploomber_engine/
--rw-r--r--   0 Edu        (503) staff       (20)     1317 2022-08-21 02:22:11.000000 ploomber-engine-0.0.8/src/ploomber_engine/__init__.py
--rw-r--r--   0 Edu        (503) staff       (20)    12168 2022-08-21 00:14:04.000000 ploomber-engine-0.0.8/src/ploomber_engine/client.py
--rw-r--r--   0 Edu        (503) staff       (20)     4280 2022-08-13 15:31:24.000000 ploomber-engine-0.0.8/src/ploomber_engine/engine.py
--rw-r--r--   0 Edu        (503) staff       (20)     8755 2022-08-21 02:15:25.000000 ploomber-engine-0.0.8/src/ploomber_engine/ipython.py
-drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-21 02:22:13.815398 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/
--rw-r--r--   0 Edu        (503) staff       (20)      101 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/PKG-INFO
--rw-r--r--   0 Edu        (503) staff       (20)      459 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/SOURCES.txt
--rw-r--r--   0 Edu        (503) staff       (20)        1 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/dependency_links.txt
--rw-r--r--   0 Edu        (503) staff       (20)      216 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/entry_points.txt
--rw-r--r--   0 Edu        (503) staff       (20)      113 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/requires.txt
--rw-r--r--   0 Edu        (503) staff       (20)       16 2022-08-21 02:22:13.000000 ploomber-engine-0.0.8/src/ploomber_engine.egg-info/top_level.txt
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-23 03:55:51.261430 ploomber-engine-0.0.9/
+-rw-r--r--   0 Edu        (503) staff       (20)     1527 2022-08-23 03:55:49.000000 ploomber-engine-0.0.9/CHANGELOG.md
+-rw-r--r--   0 Edu        (503) staff       (20)     1826 2022-08-21 00:14:04.000000 ploomber-engine-0.0.9/LICENSE
+-rw-r--r--   0 Edu        (503) staff       (20)      247 2022-07-19 22:24:03.000000 ploomber-engine-0.0.9/MANIFEST.in
+-rw-r--r--   0 Edu        (503) staff       (20)      101 2022-08-23 03:55:51.261578 ploomber-engine-0.0.9/PKG-INFO
+-rw-r--r--   0 Edu        (503) staff       (20)     3344 2022-08-13 15:26:08.000000 ploomber-engine-0.0.9/README.md
+-rw-r--r--   0 Edu        (503) staff       (20)      127 2022-07-21 00:23:47.000000 ploomber-engine-0.0.9/pyproject.toml
+-rw-r--r--   0 Edu        (503) staff       (20)      106 2022-08-23 03:55:51.262304 ploomber-engine-0.0.9/setup.cfg
+-rw-r--r--   0 Edu        (503) staff       (20)     1474 2022-08-21 05:46:37.000000 ploomber-engine-0.0.9/setup.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-23 03:55:51.254219 ploomber-engine-0.0.9/src/
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-23 03:55:51.259078 ploomber-engine-0.0.9/src/ploomber_engine/
+-rw-r--r--   0 Edu        (503) staff       (20)     1317 2022-08-23 03:55:49.000000 ploomber-engine-0.0.9/src/ploomber_engine/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)    12168 2022-08-21 00:14:04.000000 ploomber-engine-0.0.9/src/ploomber_engine/client.py
+-rw-r--r--   0 Edu        (503) staff       (20)     4280 2022-08-13 15:31:24.000000 ploomber-engine-0.0.9/src/ploomber_engine/engine.py
+-rw-r--r--   0 Edu        (503) staff       (20)    10448 2022-08-23 03:50:29.000000 ploomber-engine-0.0.9/src/ploomber_engine/ipython.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-08-23 03:55:51.261151 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/
+-rw-r--r--   0 Edu        (503) staff       (20)      101 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/PKG-INFO
+-rw-r--r--   0 Edu        (503) staff       (20)      459 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 Edu        (503) staff       (20)        1 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 Edu        (503) staff       (20)      216 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/entry_points.txt
+-rw-r--r--   0 Edu        (503) staff       (20)      136 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/requires.txt
+-rw-r--r--   0 Edu        (503) staff       (20)       16 2022-08-23 03:55:51.000000 ploomber-engine-0.0.9/src/ploomber_engine.egg-info/top_level.txt
```

### Comparing `ploomber-engine-0.0.8/CHANGELOG.md` & `ploomber-engine-0.0.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # CHANGELOG
 
+## 0.0.9 (2022-08-22)
+* Fixes error when notebook called methods in `sys.stdout`
+
 ## 0.0.8 (2022-08-20)
 * Correctly clearing up `PloomberShell` to prevent interfering with IPython terminal singleton
 
 ## 0.0.7 (2022-08-20)
 * Removes `nbclient>0.6.1` requirements (it's only applicable when using the `debug` engine)
 
 ## 0.0.6 (2022-08-13)
@@ -32,8 +35,8 @@
 ## 0.0.2 (2022-07-22)
 * Renames `ploomber-engine` to `debug`
 * Adds `debuglater` engine
 * Adds (experimental) `profiling` engine
 
 ## 0.0.1 (2022-07-20)
 
-* First release
+* First release
```

### Comparing `ploomber-engine-0.0.8/LICENSE` & `ploomber-engine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomber-engine-0.0.8/README.md` & `ploomber-engine-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ploomber-engine-0.0.8/setup.py` & `ploomber-engine-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 REQUIRES = [
     'ploomber-core>=0.0.4',
     'papermill',
     'ipykernel',
     'debuglater',
     'nbclient',
+    'ipython',
+    'parso',
+    'nbformat',
 ]
 
 DEV = [
     'pytest',
     'flake8',
     'invoke',
     'twine',
```

### Comparing `ploomber-engine-0.0.8/src/ploomber_engine/__init__.py` & `ploomber-engine-0.0.9/src/ploomber_engine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This module contains our customizatiosn to nbclient and papermill.
 """
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 import typing as t
 
 # NOTE: fully initialize papermill here to prevent circular import
 import papermill  # noqa
 
 from jupyter_client import KernelManager
```

### Comparing `ploomber-engine-0.0.8/src/ploomber_engine/client.py` & `ploomber-engine-0.0.9/src/ploomber_engine/client.py`

 * *Files identical despite different names*

### Comparing `ploomber-engine-0.0.8/src/ploomber_engine/engine.py` & `ploomber-engine-0.0.9/src/ploomber_engine/engine.py`

 * *Files identical despite different names*

### Comparing `ploomber-engine-0.0.8/src/ploomber_engine/ipython.py` & `ploomber-engine-0.0.9/src/ploomber_engine/ipython.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 import contextlib
 from io import StringIO
-import nbformat
+import itertools
 
+import parso
+import nbformat
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.displaypub import DisplayPublisher
 from IPython.core.displayhook import DisplayHook
 
 
 def _make_stream_output(out, name):
     return nbformat.v4.new_output(output_type='stream',
@@ -70,14 +72,19 @@
         self.shell._current_output.append(out)
 
 
 class PloomberShell(InteractiveShell):
     """
     A subclass of IPython's InteractiveShell to gather all the output
     produced by a code cell
+
+    Notes
+    -----
+    This is intended to be used as a singleton, so either call
+    `.clear_instance()` when you're done or use it as a context manager
     """
 
     def __init__(self):
         super().__init__(display_pub_class=CustomDisplayPublisher,
                          displayhook_class=CustomDisplayHook)
         # no assigning this produces some weird behavior when calling
         # .clear_instance()
@@ -108,34 +115,45 @@
     def enable_matplotlib(self, gui=None):
         # if we don't put this, we'll lose some display_data messages. found
         # about this trick via fastai/execnb
         from matplotlib_inline.backend_inline import configure_inline_support
         configure_inline_support.current_backend = 'unset'
         return super().enable_matplotlib(gui)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.clear_instance()
+
 
 class PloomberClient:
     """
     Partially implements nbclient.client's interface and uses PloomberShell
     to execute cells.
     """
 
     def __init__(self, nb):
         self._nb = nb
         self._shell = None
 
+    @classmethod
+    def from_path(cls, path):
+        nb = nbformat.read(path, as_version=nbformat.NO_CONVERT)
+        return cls(nb)
+
     def execute_cell(self, cell, cell_index, execution_count, store_history):
         if self._shell is None:
             raise RuntimeError('A shell has not been initialized')
 
         # results are published in different places. Here we grab all of them
         # and return them
         with patch_sys_std_out_err() as (stdout_stream, stderr_stream):
             result = self._shell.run_cell(cell['source'])
-            stdout = stdout_stream.getvalue()
+            stdout = stdout_stream.get_separated_values()
             stderr = stderr_stream.getvalue()
 
         output = []
 
         if stdout:
             output.extend(_process_stdout(stdout, result=result))
 
@@ -161,28 +179,65 @@
             result.raise_error()
 
         return output
 
     def execute(self):
         """Execute the notebook
         """
-        # make sure that the current working directory is in the sys.path
-        # in case the user has local modules
         with self:
             self._execute()
 
         return self._nb
 
+    def get_namespace(self):
+        """Run the notebook and return all the variables
+        """
+        with self:
+            existing = set(self._shell.user_ns)
+            self._execute()
+            namespace = {
+                k: v
+                for k, v in self._shell.user_ns.items() if k not in existing
+            }
+
+        return namespace
+
+    def get_definitions(self):
+        """Returns class and function definitions without running the notebook
+        """
+        source = '\n'.join(
+            [c.source for c in self._nb.cells if c.cell_type == 'code'])
+        module = parso.parse(source)
+
+        defs = [
+            def_.get_code() for def_ in itertools.chain(
+                module.iter_classdefs(), module.iter_funcdefs())
+        ]
+
+        defs_source = '\n'.join(defs)
+
+        with self:
+            existing = set(self._shell.user_ns)
+            self._shell.run_cell(defs_source)
+            defs = {
+                k: v
+                for k, v in self._shell.user_ns.items() if k not in existing
+            }
+
+        return defs
+
     def _execute(self):
         """
         Internal method to execute a notebook, assumes the shell has been
         initialized
         """
         execution_count = 1
 
+        # make sure that the current working directory is in the sys.path
+        # in case the user has local modules
         with add_to_sys_path('.'):
             for index, cell in enumerate(self._nb.cells):
                 if cell.cell_type == 'code':
                     self.execute_cell(cell,
                                       cell_index=index,
                                       execution_count=execution_count,
                                       store_history=False)
@@ -235,23 +290,25 @@
                         self._nb_man.cell_complete(self._nb.cells[index],
                                                    cell_index=index)
                         execution_count += 1
 
         return self._nb
 
 
-class IO:
+class IO(StringIO):
 
-    def __init__(self):
+    def __init__(self, initial_value='', newline='\n'):
+        super().__init__(initial_value=initial_value, newline=newline)
         self._values = []
 
     def write(self, s):
         self._values.append(s)
+        super().write(s)
 
-    def getvalue(self):
+    def get_separated_values(self):
         return self._values[:]
 
 
 @contextlib.contextmanager
 def patch_sys_std_out_err():
     """Path sys.{stout, sterr} to capture output
     """
```

