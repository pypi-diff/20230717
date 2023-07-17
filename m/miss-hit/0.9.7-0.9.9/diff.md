# Comparing `tmp/miss_hit-0.9.7.tar.gz` & `tmp/miss_hit-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/miss_hit-0.9.7.tar", last modified: Thu Jul 23 13:23:48 2020, max compression
+gzip compressed data, was "dist/miss_hit-0.9.9.tar", last modified: Thu Jul 30 10:36:22 2020, max compression
```

## Comparing `miss_hit-0.9.7.tar` & `miss_hit-0.9.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-23 13:23:48.000000 miss_hit-0.9.7/
--rw-r--r--   0 flosch    (1000) flosch    (1000)     6618 2020-07-23 13:23:48.000000 miss_hit-0.9.7/PKG-INFO
--rw-r--r--   0 flosch    (1000) flosch    (1000)     4463 2020-07-23 13:07:18.000000 miss_hit-0.9.7/README.md
-drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit/
--rw-r--r--   0 flosch    (1000) flosch    (1000)        0 2020-07-23 11:12:56.000000 miss_hit-0.9.7/miss_hit/__init__.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    10406 2020-07-23 11:16:57.000000 miss_hit-0.9.7/miss_hit/command_line.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     8215 2020-07-20 08:14:53.000000 miss_hit-0.9.7/miss_hit/config.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    16058 2020-07-23 11:17:35.000000 miss_hit-0.9.7/miss_hit/config_files.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    22301 2020-07-20 08:14:53.000000 miss_hit-0.9.7/miss_hit/errors.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     9374 2020-07-23 11:17:57.000000 miss_hit-0.9.7/miss_hit/g_cfg.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     4903 2020-07-23 11:14:36.000000 miss_hit-0.9.7/miss_hit/graph.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    94773 2020-07-23 11:16:17.000000 miss_hit-0.9.7/miss_hit/m_ast.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     3652 2020-07-20 08:14:53.000000 miss_hit-0.9.7/miss_hit/m_language.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    33495 2020-07-20 08:14:53.000000 miss_hit-0.9.7/miss_hit/m_language_builtins.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    58812 2020-07-23 11:18:32.000000 miss_hit-0.9.7/miss_hit/m_lexer.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    75726 2020-07-23 11:56:04.000000 miss_hit-0.9.7/miss_hit/m_parser.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    36510 2020-07-23 12:00:04.000000 miss_hit-0.9.7/miss_hit/mh_metric.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    39937 2020-07-23 11:20:34.000000 miss_hit-0.9.7/miss_hit/mh_style.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     9026 2020-07-23 11:13:28.000000 miss_hit-0.9.7/miss_hit/s_ast.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)    19521 2020-07-23 11:57:08.000000 miss_hit-0.9.7/miss_hit/s_parser.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     2149 2020-07-23 13:14:05.000000 miss_hit-0.9.7/miss_hit/version.py
--rw-r--r--   0 flosch    (1000) flosch    (1000)     6704 2020-07-23 11:16:39.000000 miss_hit-0.9.7/miss_hit/work_package.py
-drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/
--rw-r--r--   0 flosch    (1000) flosch    (1000)     6618 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/PKG-INFO
--rw-r--r--   0 flosch    (1000) flosch    (1000)      577 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/SOURCES.txt
--rw-r--r--   0 flosch    (1000) flosch    (1000)        1 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/dependency_links.txt
--rw-r--r--   0 flosch    (1000) flosch    (1000)       89 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/entry_points.txt
--rw-r--r--   0 flosch    (1000) flosch    (1000)        9 2020-07-23 13:23:48.000000 miss_hit-0.9.7/miss_hit.egg-info/top_level.txt
--rw-r--r--   0 flosch    (1000) flosch    (1000)      103 2020-07-23 13:23:48.000000 miss_hit-0.9.7/setup.cfg
--rw-r--r--   0 flosch    (1000) flosch    (1000)     1559 2020-07-20 14:16:17.000000 miss_hit-0.9.7/setup.py
+drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-30 10:36:22.000000 miss_hit-0.9.9/
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     6618 2020-07-30 10:36:22.000000 miss_hit-0.9.9/PKG-INFO
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     4463 2020-07-23 13:07:18.000000 miss_hit-0.9.9/README.md
+drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit/
+-rw-r--r--   0 flosch    (1000) flosch    (1000)        0 2020-07-23 11:12:56.000000 miss_hit-0.9.9/miss_hit/__init__.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     9306 2020-07-29 14:25:26.000000 miss_hit-0.9.9/miss_hit/cfg_ast.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    16033 2020-07-29 14:29:31.000000 miss_hit-0.9.9/miss_hit/cfg_parser.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    13820 2020-07-30 09:17:16.000000 miss_hit-0.9.9/miss_hit/cfg_tree.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    10428 2020-07-29 15:11:14.000000 miss_hit-0.9.9/miss_hit/command_line.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    14669 2020-07-29 15:10:21.000000 miss_hit-0.9.9/miss_hit/config.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    22301 2020-07-29 13:15:07.000000 miss_hit-0.9.9/miss_hit/errors.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     9374 2020-07-23 11:17:57.000000 miss_hit-0.9.9/miss_hit/g_cfg.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     4903 2020-07-23 11:14:36.000000 miss_hit-0.9.9/miss_hit/graph.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    95644 2020-07-29 13:41:15.000000 miss_hit-0.9.9/miss_hit/m_ast.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     3652 2020-07-20 08:14:53.000000 miss_hit-0.9.9/miss_hit/m_language.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    33495 2020-07-20 08:14:53.000000 miss_hit-0.9.9/miss_hit/m_language_builtins.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    58766 2020-07-29 12:40:48.000000 miss_hit-0.9.9/miss_hit/m_lexer.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    75859 2020-07-29 13:05:45.000000 miss_hit-0.9.9/miss_hit/m_parser.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    36555 2020-07-29 14:11:12.000000 miss_hit-0.9.9/miss_hit/mh_metric.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    40112 2020-07-29 13:32:28.000000 miss_hit-0.9.9/miss_hit/mh_style.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     8935 2020-07-27 12:56:24.000000 miss_hit-0.9.9/miss_hit/s_ast.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)    19486 2020-07-29 13:06:56.000000 miss_hit-0.9.9/miss_hit/s_parser.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     2149 2020-07-30 10:32:07.000000 miss_hit-0.9.9/miss_hit/version.py
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     6692 2020-07-29 12:06:14.000000 miss_hit-0.9.9/miss_hit/work_package.py
+drwxr-xr-x   0 flosch    (1000) flosch    (1000)        0 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     6618 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/PKG-INFO
+-rw-r--r--   0 flosch    (1000) flosch    (1000)      616 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/SOURCES.txt
+-rw-r--r--   0 flosch    (1000) flosch    (1000)        1 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/dependency_links.txt
+-rw-r--r--   0 flosch    (1000) flosch    (1000)       89 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/entry_points.txt
+-rw-r--r--   0 flosch    (1000) flosch    (1000)        9 2020-07-30 10:36:22.000000 miss_hit-0.9.9/miss_hit.egg-info/top_level.txt
+-rw-r--r--   0 flosch    (1000) flosch    (1000)      103 2020-07-30 10:36:22.000000 miss_hit-0.9.9/setup.cfg
+-rw-r--r--   0 flosch    (1000) flosch    (1000)     1559 2020-07-20 14:16:17.000000 miss_hit-0.9.9/setup.py
```

### Comparing `miss_hit-0.9.7/PKG-INFO` & `miss_hit-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss_hit
-Version: 0.9.7
+Version: 0.9.9
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://github.com/florianschanda/miss_hit
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
```

### Comparing `miss_hit-0.9.7/README.md` & `miss_hit-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/command_line.py` & `miss_hit-0.9.9/miss_hit/command_line.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import sys
 import argparse
 import traceback
 import textwrap
 import multiprocessing
 import functools
 
-from miss_hit import config_files
+from miss_hit import cfg_tree
 from miss_hit import errors
 from miss_hit import work_package
 from miss_hit import s_parser
 from miss_hit import s_ast
 
 from miss_hit.version import GITHUB_ISSUES, VERSION, FULL_NAME
 
@@ -61,15 +61,15 @@
                     action="store_true",
                     default=False,
                     help="Do not use multi-threaded analysis")
     ap.add_argument("--ignore-config",
                     action="store_true",
                     default=False,
                     help=("Ignore all %s files." %
-                          " or ".join(config_files.CONFIG_FILENAMES)))
+                          " or ".join(cfg_tree.CONFIG_FILENAMES)))
 
     output_options = ap.add_argument_group("output options")
     rv["output_options"] = output_options
 
     output_options.add_argument("--brief",
                                 action="store_true",
                                 default=False,
@@ -143,15 +143,15 @@
         pass
 
 
 def dispatch_wp(process_fn, wp):
     results = []
 
     try:
-        if not wp.cfg["enable"]:
+        if not wp.cfg.enabled:
             wp.mh.register_exclusion(wp.filename)
             results.append(work_package.Result(wp, False))
 
         elif isinstance(wp, work_package.SIMULINK_File_WP):
             wp.register_file()
             slp = s_parser.Simulink_SLX_Parser(wp.mh, wp.filename, wp.cfg)
             n_content = slp.parse_file()
@@ -181,38 +181,37 @@
     assert isinstance(mh, errors.Message_Handler)
     assert isinstance(back_end, MISS_HIT_Back_End)
 
     process_fn = functools.partial(dispatch_wp, back_end.process_wp)
 
     try:
         for item in options.files:
-            if os.path.isdir(item):
-                config_files.register_tree(mh,
-                                           os.path.abspath(item),
-                                           options)
-
-            elif os.path.isfile(item):
-                config_files.register_tree(
-                    mh,
-                    os.path.dirname(os.path.abspath(item)),
-                    options)
-
-        config_files.build_config_tree(mh,
+            if os.path.isdir(item) or os.path.isfile(item):
+                cfg_tree.register_item(mh,
+                                       os.path.abspath(item),
                                        options)
+        mh.reset_seen()
 
     except errors.Error:
         mh.summary_and_exit()
 
     work_list = []
     for item in options.files:
         if os.path.isdir(item):
             for path, dirs, files in os.walk(item):
+                dirs.sort()
+                for excluded_dir in cfg_tree.get_excluded_directories(path):
+                    dirs.remove(excluded_dir)
+                hidden_dirs = [d for d in dirs if d.startswith(".")]
+                for hidden_dir in hidden_dirs:
+                    dirs.remove(hidden_dir)
+
                 if path == ".":
                     path = ""
-                dirs.sort()
+
                 for f in sorted(files):
                     if f.endswith(".m") or (f.endswith(".slx") and
                                             process_slx):
                         work_list.append(
                             work_package.create(os.path.join(path, f),
                                                 "cp1252",
                                                 mh,
```

### Comparing `miss_hit-0.9.7/miss_hit/config_files.py` & `miss_hit-0.9.9/miss_hit/cfg_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 ##############################################################################
 ##                                                                          ##
 ##          MATLAB Independent, Small & Safe, High Integrity Tools          ##
 ##                                                                          ##
-##              Copyright (C) 2020,      Florian Schanda                    ##
-##              Copyright (C) 2019-2020, Zenuity AB                         ##
+##              Copyright (C) 2020, Florian Schanda                         ##
 ##                                                                          ##
 ##  This file is part of MISS_HIT.                                          ##
 ##                                                                          ##
 ##  MATLAB Independent, Small & Safe, High Integrity Tools (MISS_HIT) is    ##
 ##  free software: you can redistribute it and/or modify it under the       ##
 ##  terms of the GNU General Public License as published by the Free        ##
 ##  Software Foundation, either version 3 of the License, or (at your       ##
@@ -20,48 +19,65 @@
 ##  GNU General Public License for more details.                            ##
 ##                                                                          ##
 ##  You should have received a copy of the GNU General Public License       ##
 ##  along with MISS_HIT. If not, see <http://www.gnu.org/licenses/>.        ##
 ##                                                                          ##
 ##############################################################################
 
-import os
+# Simple parser (based on the MATLAB lexer) for our config file. Some
+# reasoning this is based on the MATLAB lexer:
+#   - increases complexity in the MATLAB lexer a bit, since it adds another
+#     lexing mode
+#   + we don't have to implement a separate lexer
+#   + we don't have to depend on e.g. PLY (which is not a bad thing, I love
+#     PLY, but since we have zero dependencies right now this would be
+#     a bit annoying)
+
 import re
+import difflib
+import os.path
 from copy import deepcopy
 
-from miss_hit import config
 from miss_hit import m_lexer
-
-from miss_hit.errors import ICE, Error, Location
-
-
-CONFIG_FILENAMES = ["miss_hit.cfg", ".miss_hit"]
-
-CONFIG_TREE = {}
+from miss_hit.errors import ICE, Error, Location, Message_Handler
+from miss_hit.config import (STYLE_RULES, STYLE_CONFIGURATION,
+                             METRICS,
+                             Boolean_Style_Configuration,
+                             Integer_Style_Configuration,
+                             Regex_Style_Configuration,
+                             Set_Style_Configuration)
+from miss_hit.cfg_ast import *
 
 
 class Config_Parser:
     def __init__(self, mh, config_file):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(config_file, str)
+
         self.filename = config_file
         self.dirname = os.path.dirname(config_file)
         self.mh = mh
+
         self.mh.register_file(self.filename)
         with open(config_file, "r") as fd:
             content = fd.read()
         self.lexer = m_lexer.MATLAB_Lexer(mh, content, self.filename)
         self.lexer.set_config_file_mode()
 
         # pylint: disable=invalid-name
         self.ct = None
         self.nt = None
         # pylint: enable=invalid-name
 
-        self.next()
+        self.skip()
+
+    ##########################################################################
+    # Generic recursive descent parser support
 
-    def next(self):
+    def skip(self):
         self.ct = self.nt
         self.nt = self.lexer.token()
 
         while self.nt:
             # Skip comments
             while self.nt and self.nt.kind == "COMMENT":
                 self.nt = self.lexer.token()
@@ -72,364 +88,370 @@
                 self.nt.kind == "NEWLINE" and
                 self.ct.kind == "NEWLINE"):
                 self.nt = self.lexer.token()
             else:
                 break
 
     def match(self, kind, value=None):
-        self.next()
+        self.skip()
         if self.ct is None:
             self.mh.error(self.lexer.get_file_loc(),
                           "expected %s, reached EOF instead" % kind)
         elif self.ct.kind != kind:
             self.mh.error(self.ct.location,
                           "expected %s, found %s instead" % (kind,
                                                              self.ct.kind))
         elif value and self.ct.value != value:
             self.mh.error(self.ct.location,
                           "expected %s(%s), found %s(%s) instead" %
                           (kind, value, self.ct.kind, self.ct.value))
 
     def match_eof(self):
-        self.next()
+        self.skip()
         if self.ct is not None:
             self.mh.error(self.ct.location,
                           "expected end of file, found %s instead" %
                           self.ct.kind)
 
     def peek(self, kind, value=None):
         if self.nt and self.nt.kind == kind:
             if value is None:
                 return True
             else:
                 return self.nt.value == value
         else:
             return False
 
-    def parse_generic_entry(self, cfg):
-        self.match("IDENTIFIER")
-        t_key = self.ct
-        key = self.ct.value
-        value = None
-        self.match("COLON")
+    def peek_eof(self):
+        return self.nt is None
 
-        if key == "enable_rule":
-            self.match("STRING")
-            value = self.ct.value
-            if value not in config.STYLE_RULES:
-                self.mh.error(self.ct.location,
-                              "unknown rule")
-                # TODO: Use difflib to find a likely one
+    ##########################################################################
+    # Top-down parsing (main entry point is parse_config_file)
 
-        elif key not in cfg:
-            self.mh.error(t_key.location,
-                          "unknown option %s" % key)
-
-        elif isinstance(cfg[key], int):
-            self.match("NUMBER")
-            try:
-                value = int(self.ct.value)
-            except ValueError:
-                self.mh.error(self.ct.location,
-                              "%s option requires an integer" % key)
+    def parse_config_file(self):
+        n_file = Config_File()
+        has_errors = False
 
-        elif isinstance(cfg[key], bool):
-            self.match("NUMBER")
-            if self.ct.value in ("0", "1"):
-                value = self.ct.value == "1"
+        while not self.peek_eof():
+            if self.peek("NEWLINE"):
+                self.match("NEWLINE")
             else:
-                self.mh.error(self.ct.location,
-                              "boolean option %s requires 0 or 1" %
-                              key)
+                try:
+                    n_item = self.parse_config_item()
+                except Error:
+                    # On errors, we skip tokens until we get to a
+                    # newline
+                    has_errors = True
+                    n_item = None
+                    while not (self.peek_eof() or self.peek("NEWLINE")):
+                        self.skip()
 
-        elif isinstance(cfg[key], set):
-            self.match("STRING")
-            value = self.ct.value
-
-            if key == "exclude_dir":
-                if os.path.basename(value) != value or \
-                   not os.path.isdir(os.path.join(self.dirname,
-                                                  value)):
-                    self.mh.error(self.ct.location,
-                                  "must be a valid local directory")
+                if n_item:
+                    n_file.add_item(n_item)
 
-            elif key == "suppress_rule":
-                if value not in config.STYLE_RULES:
-                    self.mh.error(self.ct.location,
-                                  "unknown rule")
-                    # TODO: Use difflib to find a likely one
+        self.match_eof()
 
-        elif isinstance(cfg[key], str):
-            self.match("STRING")
-            value = self.ct.value
-
-            if key.startswith("regex"):
-                # If this is supposed to be a regex, we can
-                # check in advance if it compiles or not. On
-                # failure we can feed back the error using our
-                # own error system.
-                try:
-                    re.compile(value)
-                except re.error as err:
-                    loc = deepcopy(self.ct.location)
-                    if err.colno is not None:
-                        loc.col_start += err.colno
-                        loc.col_end = loc.col_start
-
-                        self.mh.error(loc, err.msg)
-
-        if key == "enable_rule":
-            if value in cfg["suppress_rule"]:
-                cfg["suppress_rule"].remove(value)
-        elif isinstance(cfg[key], set):
-            cfg[key].add(value)
-        else:
-            cfg[key] = value
+        if has_errors:
+            self.mh.error(Location(self.filename),
+                          "config file contains errors")
+            return None
 
-    def parse_metric_entry(self, cfg):
-        self.match("IDENTIFIER", "metric")
+        return n_file
 
-        if self.peek("OPERATOR", "*"):
-            self.match("OPERATOR", "*")
-            metric_name = None
+    def parse_config_item(self):
+        n_item = None
+
+        if self.peek("IDENTIFIER", "metric"):
+            n_item = self.parse_metric_limit()
+
+        elif self.peek("IDENTIFIER", "enable"):
+            n_item = self.parse_simple_enable()
+
+        elif self.peek("IDENTIFIER", "enable_rule") or \
+             self.peek("IDENTIFIER", "suppress_rule"):
+            n_item = self.parse_style_application()
+
+        elif self.peek("IDENTIFIER", "exclude_dir"):
+            n_item = self.parse_directory_exclusion()
+
+        elif self.peek("IDENTIFIER", "project_root"):
+            n_item = self.parse_project_root()
+
+        elif self.peek("IDENTIFIER", "octave"):
+            n_item = self.parse_octave_mode()
+
+        elif self.peek("IDENTIFIER"):
+            n_item = self.parse_style_configuration()
+
+        else:
+            self.skip()
+            self.mh.error(self.ct.location,
+                          "expected valid config entry, found %s instead" %
+                          (self.ct.kind))
+
+        # Each item is terminated with a newline (or EOF)
+        if self.peek_eof():
+            pass
         else:
-            self.match("STRING")
-            metric_name = self.ct.value
+            self.match("NEWLINE")
+
+        return n_item
 
-            if metric_name in config.METRICS:
-                metric_info = config.METRICS[metric_name]
+    def parse_integer_number(self):
+        self.match("NUMBER")
+        try:
+            value = int(self.ct.value)
+        except ValueError:
+            self.mh.error(self.ct.location, "expected an integer number")
+        return value
+
+    def parse_natural_number(self):
+        value = self.parse_integer_number()
+        if value < 0:
+            self.mh.error(self.ct.location, "expected a natural number (>= 0)")
+        return value
+
+    def parse_string(self):
+        self.match("STRING")
+        return self.ct.value
+
+    def parse_regex(self):
+        value = self.parse_string()
+
+        # We can use the Python regex module to sanity check it
+        try:
+            re.compile(value)
+        except re.error as err:
+            loc = deepcopy(self.ct.location)
+            if err.colno is not None:
+                loc.col_start += err.colno
+                loc.col_end = loc.col_start
+
+                self.mh.error(loc, err.msg)
+
+        return value
+
+    def parse_boolean(self):
+        if self.peek("NUMBER"):
+            value = self.parse_integer_number()
+            if value in (0, 1):
+                return bool(value)
             else:
-                self.mh.error(self.ct.location,
-                              "unknown metric '%s'" % metric_name)
+                self.mh.error(self.ct.location, "expected true or false")
 
+        elif self.peek("IDENTIFIER"):
+            self.match("IDENTIFIER")
+            if self.ct.value == "true":
+                return True
+            elif self.ct.value == "false":
+                return False
+            else:
+                self.mh.error(self.ct.location, "expected true or false")
+
+        else:
+            self.skip()
+            self.mh.error(self.ct.location, "expected true or false")
+
+    def parse_simple_enable(self):
+        self.match("IDENTIFIER", "enable")
         self.match("COLON")
+        value = self.parse_boolean()
+
+        return Activation(value)
 
+    def parse_style_application(self):
         self.match("IDENTIFIER")
-        if self.ct.value == "limit":
-            if metric_name is None:
-                self.mh.error(self.ct.location,
-                              "cannot specify limit for all metrics"
-                              " simultaneously")
+        if self.ct.value == "enable_rule":
+            enabled = True
+        elif self.ct.value == "suppress_rule":
+            enabled = False
+        else:
+            self.mh.error(self.ct.location,
+                          "expected enable_rule or suppress_rule")
 
-            self.match("NUMBER")
-            if metric_info["type"] != "int":
-                raise ICE("logic error: metric that is not an int")
-
-            try:
-                value = int(self.ct.value)
-            except ValueError:
-                self.mh.error(self.ct.location,
-                              "expected positive integer")
-            if value < 0:
-                self.mh.error(self.ct.location,
-                              "expected positive integer")
+        self.match("COLON")
 
-            cfg["metrics"][metric_name] = {"max" : value}
+        self.match("STRING")
+        rule_name = self.ct.value
+        if rule_name not in STYLE_RULES:
+            msg = "expected valid style rule name"
+            suggestions = difflib.get_close_matches(rule_name,
+                                                    list(STYLE_RULES),
+                                                    n=1)
+            if suggestions:
+                msg += " (did you mean %s?)" % suggestions[0]
+            self.mh.error(self.ct.location, msg)
 
-        elif self.ct.value == "disable":
-            if metric_name is None:
-                cfg["metrics"] = {m: {"disable": True}
-                                  for m in config.METRICS}
-            else:
-                cfg["metrics"][metric_name] = {"disable": True}
+        return Style_Application(rule_name, enabled)
 
-        elif self.ct.value == "report":
-            if metric_name is None:
-                cfg["metrics"] = {}
-            else:
-                if metric_name in cfg["metrics"]:
-                    del cfg["metrics"][metric_name]
+    def parse_style_configuration(self):
+        self.match("IDENTIFIER")
+        config_name = self.ct.value
+        if config_name not in STYLE_CONFIGURATION:
+            msg = "expected valid style configuration name"
+            suggestions = difflib.get_close_matches(config_name,
+                                                    list(STYLE_CONFIGURATION),
+                                                    n=1)
+            if suggestions:
+                msg += " (did you mean %s?)" % suggestions[0]
+            self.mh.error(self.ct.location, msg)
+
+        self.match("COLON")
+
+        cfg_item = STYLE_CONFIGURATION[config_name]
+        value = None
+        if isinstance(cfg_item, Integer_Style_Configuration):
+            value = self.parse_integer_number()
+            if cfg_item.lower_limit is not None:
+                if value < cfg_item.lower_limit:
+                    self.mh.error(self.ct.location,
+                                  "%s must be at least %i" %
+                                  (config_name,
+                                   cfg_item.lower_limit))
+            if cfg_item.upper_limit is not None:
+                if value > cfg_item.upper_limit:
+                    self.mh.error(self.ct.location,
+                                  "%s can be at most %i" %
+                                  (config_name,
+                                   cfg_item.upper_limit))
+
+        elif isinstance(cfg_item, Regex_Style_Configuration):
+            value = self.parse_regex()
+
+        elif isinstance(cfg_item, Set_Style_Configuration):
+            value = self.parse_string()
+
+        elif isinstance(cfg_item, Boolean_Style_Configuration):
+            value = self.parse_boolean()
 
         else:
+            raise ICE("unexpected cfg kind %s" % cfg_item.__class__.__name__)
+
+        return Style_Configuration(config_name, value)
+
+    def parse_directory_exclusion(self):
+        self.match("IDENTIFIER", "exclude_dir")
+        self.match("COLON")
+        value = self.parse_string()
+
+        if not os.path.exists(os.path.join(self.dirname, value)):
+            self.mh.error(self.ct.location, "does not exist")
+        elif not os.path.isdir(os.path.join(self.dirname, value)):
+            self.mh.error(self.ct.location,
+                          "is not a directory")
+        elif os.path.basename(value) != value:
             self.mh.error(self.ct.location,
-                          "expected report or limit")
+                          "must local (non-relative) directory")
 
-    def parse_file(self, cfg):
-        while self.nt:
-            if self.nt.kind == "NEWLINE":
-                self.match("NEWLINE")
-                continue
+        # TODO: Allow wildcards (see #5)
 
-            if self.peek("IDENTIFIER", "metric"):
-                self.parse_metric_entry(cfg)
-            else:
-                self.parse_generic_entry(cfg)
+        rv = Directory_Exclusion()
+        rv.add_directory(value)
+        return rv
 
-            # Finished with this thing, now we expect a newline or EOF
-            if self.nt:
-                self.match("NEWLINE")
+    def parse_metric_limit(self):
+        self.match("IDENTIFIER", "metric")
+
+        if self.peek("OPERATOR", "*"):
+            self.match("OPERATOR", "*")
+            metric_name = "*"
+
+        else:
+            metric_name = self.parse_string()
+            if metric_name not in METRICS:
+                msg = "expected valid code metric or '*'"
+                suggestions = difflib.get_close_matches(metric_name,
+                                                        list(METRICS),
+                                                        n=1)
+                if suggestions:
+                    msg += " (did you mean %s?)" % suggestions[0]
+                self.mh.error(self.ct.location, msg)
+
+        self.match("COLON")
+
+        if self.peek("IDENTIFIER", "disable"):
+            self.match("IDENTIFIER", "disable")
+            return Metric_Limit(metric_name, False)
+
+        elif self.peek("IDENTIFIER", "report"):
+            self.match("IDENTIFIER", "report")
+            return Metric_Limit(metric_name, True)
+
+        elif self.peek("IDENTIFIER", "limit"):
+            self.match("IDENTIFIER", "limit")
+            if metric_name == "*":
+                self.mh.error(self.ct.location,
+                              "cannot apply limit to all metrics")
+            value = self.parse_natural_number()
+            return Metric_Limit(metric_name, True, value)
+
+        else:
+            self.skip()
+            if metric_name == "*":
+                self.mh.error(self.ct.location,
+                              "expected disable|report")
             else:
-                self.match_eof()
+                self.mh.error(self.ct.location,
+                              "expected disable|report|limit")
+
+    def parse_project_root(self):
+        self.match("IDENTIFIER", "project_root")
+        return Project_Root()
+
+    def parse_octave_mode(self):
+        self.match("IDENTIFIER", "octave")
+        self.match("COLON")
+        value = self.parse_boolean()
+        return Octave_Mode(value)
+
 
+def load_config(mh, filename):
+    cfg_parser = Config_Parser(mh, os.path.relpath(filename))
+    tree = cfg_parser.parse_config_file()
+    mh.unregister_file(os.path.relpath(filename))
+    return tree
 
-def load_config(mh, cfg_file, cfg):
-    assert isinstance(cfg_file, str)
-    assert os.path.isfile(cfg_file)
-    assert isinstance(cfg, dict)
 
-    rel_name = os.path.relpath(cfg_file)
+def sanity_test(mh, filename, show_bt):
+    # pylint: disable=import-outside-toplevel
+    import traceback
+    # pylint: enable=import-outside-toplevel
 
     try:
-        parser = Config_Parser(mh, rel_name)
-        parser.parse_file(cfg)
-        # Now that we have parsed the file, we should remove it again
-        # from the list of files known to the error handler
-        mh.unregister_file(rel_name)
+        tree = load_config(mh, filename)
+        tree.dump()
+
     except Error:
-        mh.reset_seen()
-        mh.summary_and_exit()
+        if show_bt:
+            traceback.print_exc()
 
-    mh.reset_seen()
+    except ICE as ice:
+        if show_bt:
+            traceback.print_exc()
+        print("ICE:", ice.reason)
 
 
-def register_tree(mh, dirname, options):
-    assert isinstance(dirname, str)
-    assert os.path.isdir(dirname)
-    assert dirname == os.path.abspath(dirname)
+def cfg_parser_main():
+    # pylint: disable=import-outside-toplevel
+    from argparse import ArgumentParser
+    # pylint: enable=import-outside-toplevel
 
-    def register_parent(dirname, find_roots):
-        if dirname in CONFIG_TREE:
-            return
+    ap = ArgumentParser()
+    ap.add_argument("file")
+    ap.add_argument("--no-tb",
+                    action="store_true",
+                    default=False,
+                    help="Do not show debug-style backtrace")
+    options = ap.parse_args()
 
-        # Stop if we reach the root filesystem or a .git directory
-        parent = os.path.dirname(dirname)
-        if find_roots:
-            is_root = parent == dirname
-        else:
-            is_root = False
+    mh = Message_Handler("debug")
+    mh.sort_messages = False
+    mh.colour = False
+
+    sanity_test(mh, options.file,
+                not options.no_tb)
+
+    mh.summary_and_exit()
 
-        if not is_root:
-            register_parent(parent, find_roots)
-            CONFIG_TREE[parent]["children"].add(dirname)
-
-        config_name = None
-        if not options.ignore_config:
-            for filename in CONFIG_FILENAMES:
-                if os.path.isfile(os.path.join(dirname, filename)):
-                    if config_name is None:
-                        config_name = filename
-                    else:
-                        mh.register_file("directory " +
-                                         os.path.relpath(dirname))
-                        mh.error(Location("directory " +
-                                          os.path.relpath(dirname)),
-                                 "cannot have both a %s and %s config file" %
-                                 (config_name, filename))
-
-        CONFIG_TREE[dirname] = {
-            "children"   : set(),
-            "subtree"    : False,
-            "has_config" : config_name,
-            "root"       : is_root,
-            "parent"     : None if is_root else parent
-        }
-
-    def register_subtree(dirname):
-        if CONFIG_TREE[dirname]["subtree"]:
-            return
-
-        CONFIG_TREE[dirname]["children"] = set(
-            os.path.join(dirname, d)
-            for d in os.listdir(dirname)
-            if (os.path.isdir(os.path.join(dirname, d)) and
-                os.access(os.path.join(dirname, d), os.R_OK))
-        )
-
-        for child in CONFIG_TREE[dirname]["children"]:
-            register_parent(child, find_roots=False)
-            register_subtree(child)
-
-        CONFIG_TREE[dirname]["subtree"] = True
-
-    register_parent(dirname, find_roots=True)
-    register_subtree(dirname)
-
-
-def build_config_tree(mh, cmdline_options):
-    # Construct basic default options
-    root_config = deepcopy(config.BASE_CONFIG)
-
-    # Find root of config tree
-    roots = [d for d in CONFIG_TREE if CONFIG_TREE[d]["root"]]
-    if len(roots) == 0:
-        raise ICE("could not find any project or filesystem root")
-    elif len(roots) == 1:
-        project_root = roots[0]
-    elif len(roots) > 1:
-        raise ICE("found multiple roots: %s" % ", ".join(roots))
-
-    parse_config = not cmdline_options.ignore_config
-
-    def merge_command_line(cfg):
-        # Thse options exist for all tools
-        if cmdline_options.octave:
-            cfg["octave"] = cmdline_options.octave
-        if cmdline_options.ignore_pragmas:
-            cfg["ignore_pragmas"] = cmdline_options.ignore_pragmas
-
-        # Overwrite some options from the command-line for style
-        # checking
-        if "line_length" in cmdline_options and \
-           cmdline_options.line_length:
-            cfg["line_length"] = cmdline_options.line_length
-        if "file_length" in cmdline_options and \
-           cmdline_options.file_length:
-            cfg["file_length"] = cmdline_options.file_length
-        if "tab_width" in cmdline_options and \
-           cmdline_options.tab_width:
-            cfg["tab_width"] = cmdline_options.tab_width
-        if "copyright_entity" in cmdline_options and \
-           cmdline_options.copyright_entity:
-            cfg["copyright_entity"] = set(cmdline_options.copyright_entity)
-
-    def build(node, exclude=False):
-        if CONFIG_TREE[node]["root"]:
-            # First we set up basic config. For roots this is a copy
-            # of the default config.
-            CONFIG_TREE[node]["config"] = deepcopy(root_config)
-            merge_command_line(CONFIG_TREE[node]["config"])
-        else:
-            # For non-roots we copy the parent config.
-            parent_node = CONFIG_TREE[node]["parent"]
-            parent_config = CONFIG_TREE[parent_node]["config"]
-            CONFIG_TREE[node]["config"] = deepcopy(parent_config)
-
-            # We reset the exclude_dir field as it makes no sense to
-            # propagate it.
-            CONFIG_TREE[node]["config"]["exclude_dir"] = set()
-
-        # We now have basic configuration for this node. If we're in
-        # exclude mode we just set enable to false for this node.
-        if exclude:
-            CONFIG_TREE[node]["config"]["enable"] = False
-
-        # Otherwise we process any config file
-        elif CONFIG_TREE[node]["has_config"] and parse_config:
-            load_config(mh,
-                        os.path.join(node, CONFIG_TREE[node]["has_config"]),
-                        CONFIG_TREE[node]["config"])
-            merge_command_line(CONFIG_TREE[node]["config"])
-
-        # Finally, loop over all children to continue building the
-        # tree.
-        for child in CONFIG_TREE[node]["children"]:
-            to_exclude = (exclude or
-                          os.path.basename(child) in
-                          CONFIG_TREE[node]["config"]["exclude_dir"])
-            build(child, exclude=to_exclude)
-
-    build(project_root, exclude=False)
-
-
-def get_config(filename):
-    dirname = os.path.dirname(os.path.abspath(filename))
-
-    if dirname not in CONFIG_TREE:
-        if not os.path.isdir(dirname):
-            hint = " (note: this is not a directory)"
-        else:
-            hint = ""
-        raise ICE("%s: expected %s to be in configuration tree%s" % (filename,
-                                                                     dirname,
-                                                                     hint))
 
-    return CONFIG_TREE[dirname]["config"]
+if __name__ == "__main__":
+    cfg_parser_main()
```

### Comparing `miss_hit-0.9.7/miss_hit/errors.py` & `miss_hit-0.9.9/miss_hit/errors.py`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/g_cfg.py` & `miss_hit-0.9.9/miss_hit/g_cfg.py`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/graph.py` & `miss_hit-0.9.9/miss_hit/graph.py`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/m_ast.py` & `miss_hit-0.9.9/miss_hit/m_ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 ##  along with MISS_HIT. If not, see <http://www.gnu.org/licenses/>.        ##
 ##                                                                          ##
 ##############################################################################
 
 import subprocess
 import re
 
-from miss_hit import config
+from miss_hit.config import Config
 from miss_hit.m_language import TOKEN_KINDS
 from miss_hit.m_language_builtins import HIGH_IMPACT_BUILTIN_FUNCTIONS
-from miss_hit.errors import ICE, Location
+from miss_hit.errors import Message_Handler, ICE, Location
 
 
 ##############################################################################
 # Lexical tokens
 ##############################################################################
 
 TOKENS_WITH_IMPLICIT_VALUE = frozenset([
@@ -308,15 +308,16 @@
 
 
 class Name(Expression):
     def is_simple_dotted_name(self):
         return False
 
     def sty_check_builtin_shadow(self, mh, cfg):
-        pass
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
 
 
 class Literal(Expression):
     pass
 
 
 class Definition(Node):
@@ -383,14 +384,16 @@
     def loc(self):
         return self.error_location
 
     def set_parent(self, n_parent):
         raise ICE("compilation unit cannot have a parent")
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
         raise ICE("compilation unit root implements no checks")
 
 
 ##############################################################################
 # Compilation units
 ##############################################################################
 
@@ -434,14 +437,16 @@
     def visit(self, parent, function, relation):
         self._visit(parent, function, relation)
         self.n_statements.visit(self, function, "Statements")
         self._visit_list(self.l_functions, function, "Functions")
         self._visit_end(parent, function, relation)
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
         for n_function in self.l_functions:
             n_function.sty_check_naming(mh, cfg)
 
 
 class Function_File(Compilation_Unit):
     def __init__(self,
                  name, loc, file_length,
@@ -478,14 +483,16 @@
     def visit(self, parent, function, relation):
         self._visit(parent, function, relation)
         self._visit_list(self.l_pragmas, function, "Pragmas")
         self._visit_list(self.l_functions, function, "Functions")
         self._visit_end(parent, function, relation)
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
         for n_function in self.l_functions:
             n_function.sty_check_naming(mh, cfg)
 
 
 class Class_File(Compilation_Unit):
     def __init__(self,
                  name, loc, file_length,
@@ -533,14 +540,16 @@
         self._visit(parent, function, relation)
         self._visit_list(self.l_pragmas, function, "Pragmas")
         self.n_classdef.visit(self, function, "Classdef")
         self._visit_list(self.l_functions, function, "Functions")
         self._visit_end(parent, function, relation)
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
         self.n_classdef.sty_check_naming(mh, cfg)
         for n_function in self.l_functions:
             n_function.sty_check_naming(mh, cfg)
 
 ##############################################################################
 # Definitions
 ##############################################################################
@@ -631,15 +640,17 @@
             self.l_enumerations.append(n_block)
         else:
             raise ICE("unexpected block kind %s" % n_block.kind())
 
         n_block.set_parent(self)
 
     def sty_check_naming(self, mh, cfg):
-        if config.active(cfg, "naming_classes"):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
+        if cfg.active("naming_classes"):
             self.n_name.sty_check_naming(mh, cfg, "class")
         for n_block in self.l_methods:
             for n_function in n_block.l_items:
                 n_function.sty_check_naming(mh, cfg)
 
 
 class Function_Definition(Definition):
@@ -717,14 +728,16 @@
         self.n_sig.visit(self, function, "Signature")
         self._visit_list(self.l_validation, function, "Validation")
         self.n_body.visit(self, function, "Body")
         self._visit_list(self.l_nested, function, "Nested")
         self._visit_end(parent, function, relation)
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
         self.n_sig.sty_check_naming(mh, cfg)
         for n_function in self.l_nested:
             n_function.sty_check_naming(mh, cfg)
 
     def is_class_method(self):
         # We're a class method in two scenarios:
         #
@@ -799,21 +812,24 @@
         self._visit(parent, function, relation)
         self.n_name.visit(self, function, "Name")
         self._visit_list(self.l_inputs, function, "Inputs")
         self._visit_list(self.l_outputs, function, "Outputs")
         self._visit_end(parent, function, relation)
 
     def sty_check_naming(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
+
         # We need to work out what we are. Options are:
         # 1. Ordinary function
         # 2. Nested function
         # 3. Class method (separate or otherwise)
         # 4. Naked signature in class as forward declaration
 
-        if not config.active(cfg, "naming_functions"):
+        if not cfg.active("naming_functions"):
             return
 
         n_fdef = self.n_parent
 
         if isinstance(n_fdef, Special_Block):
             # This is case 4: naked signature. Check as if it's
             # method.
@@ -1363,20 +1379,26 @@
         else:
             return self.t_ident.value
 
     def is_simple_dotted_name(self):
         return self.t_ident.kind == "IDENTIFIER"
 
     def sty_check_naming(self, mh, cfg, kind):
-        regex = cfg["regex_" + kind + "_name"]
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
+
+        regex = cfg.style_config["regex_" + kind + "_name"]
         if not re.match("^(" + regex + ")$", self.t_ident.value):
             mh.style_issue(self.t_ident.location,
                            "violates naming scheme for %s" % kind)
 
     def sty_check_builtin_shadow(self, mh, cfg):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(cfg, Config)
+
         if self.t_ident.value in HIGH_IMPACT_BUILTIN_FUNCTIONS:
             mh.style_issue(self.t_ident.location,
                            "redefining this builtin is very naughty")
 
 
 class Selection(Name):
     def __init__(self, t_selection, n_prefix, n_field):
```

### Comparing `miss_hit-0.9.7/miss_hit/m_language.py` & `miss_hit-0.9.9/miss_hit/m_language.py`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/m_language_builtins.py` & `miss_hit-0.9.9/miss_hit/m_language_builtins.py`

 * *Files identical despite different names*

### Comparing `miss_hit-0.9.7/miss_hit/m_lexer.py` & `miss_hit-0.9.9/miss_hit/m_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ##                                                                          ##
 ##############################################################################
 
 import os
 import re
 from abc import ABCMeta, abstractmethod
 
-from miss_hit import config
+from miss_hit.config import Config
 from miss_hit import m_ast
 
 from miss_hit.errors import Location, Error, Message_Handler, ICE
 from miss_hit.m_language import KEYWORDS, ANNOTATION_KEYWORDS
 
 # The 1999 technical report "The Design and Implementation of a Parser
 # and Scanner for the MATLAB Language in the MATCH Compiler" is a key
@@ -226,29 +226,29 @@
         self.context_line = new_lines
         self.text = "\n".join(new_lines) + "\n"
 
         self.cc = None
         self.nc = self.text[0] if len(self.text) > 0 else "\0"
         self.nnc = self.text[1] if len(self.text) > 1 else "\0"
 
-    def next(self):
+    def skip(self):
         self.lexpos += 1
         if self.cc == "\n":
             self.col_offset = self.lexpos
         self.cc = self.nc
         self.nc = self.nnc
         self.nnc = self.nnnc
         self.nnnc = (self.text[self.lexpos + 3]
                      if len(self.text) > self.lexpos + 3
                      else "\0")
 
     def advance(self, n):
         assert isinstance(n, int) and n >= 0
         for _ in range(n):
-            self.next()
+            self.skip()
 
     def match_re(self, regex):
         match = re.match("^" + regex,
                          self.text[self.lexpos:])
         if match is None:
             return None
         else:
@@ -262,24 +262,20 @@
                                    col_end  =self.lexpos - self.col_offset,
                                    context  =self.context_line[self.line - 1]),
                           (message
                            if message
                            else "unexpected character %s" % repr(self.cc)))
 
     def contains_block_open(self, string):
-        for c in self.comment_char:
-            if c + "{" in string:
-                return True
-        return False
+        return any(c + "{" in string
+                   for c in self.comment_char)
 
     def contains_block_close(self, string):
-        for c in self.comment_char:
-            if c + "}" in string:
-                return True
-        return False
+        return any(c + "}" in string
+                   for c in self.comment_char)
 
     def __token(self):
         # If we've been instructed to add an anonymous comma, we do
         # that and nothing else.
         if self.add_comma:
             self.add_comma = False
             fake_line = self.context_line[self.line - 1]
@@ -302,22 +298,22 @@
             self.last_value = ","
             return token
 
         # First we scan to the next non-whitespace character, unless
         # we're in block comment mode
         preceeding_ws = False
         while not self.block_comment:
-            self.next()
+            self.skip()
             if self.cc in (" ", "\t"):
                 preceeding_ws = True
             else:
                 break
 
         if self.block_comment:
-            self.next()
+            self.skip()
 
         kind = None
         value = None
 
         t_start = self.lexpos
         col_start = t_start - self.col_offset
         contains_quotes = False
@@ -331,44 +327,44 @@
 
         elif self.block_comment:
             if self.cc == "\n":
                 kind = "NEWLINE"
             else:
                 kind = "COMMENT"
                 while self.nc not in ("\n", "\0"):
-                    self.next()
+                    self.skip()
 
         elif self.command_mode:
             # Lexing in command mode
             if self.cc in self.comment_char:
                 # Comments go until the end of the line
                 kind = "COMMENT"
                 while self.nc not in ("\n", "\0"):
-                    self.next()
+                    self.skip()
 
             elif self.cc == "\n":
                 # Newlines are summarised into one token
                 kind = "NEWLINE"
                 while self.nc in ("\n", " ", "\t"):
-                    self.next()
+                    self.skip()
 
             elif self.cc == ";":
                 kind = "SEMICOLON"
 
             elif self.cc == ",":
                 kind = "COMMA"
 
             elif self.cc == "." and \
                  self.nc == "." and \
                  self.nnc == ".":
                 kind = "CONTINUATION"
                 # We now need to eat everything until and including
                 # the next line
                 while self.cc not in ("\n", "\0"):
-                    self.next()
+                    self.skip()
 
             else:
                 # Everything else in command form is converted into a
                 # string. Strings behave in a weird way. They can be
                 # interleaved and joined into text, e.g. "foo'bar'" is
                 # actually "foobar", but "foo 'bar'" is two strings:
                 # "foo" and "bar". This only works with single
@@ -394,15 +390,15 @@
                 while True:
                     if string_mode:
                         if self.nc == "'" and self.nnc == "'":
                             # Double single quotes are escaped to
                             # single quotes. We skip one extra
                             # character ahead.
                             value += "'"
-                            self.next()
+                            self.skip()
 
                         elif self.nc == "'":
                             # Leave string mode
                             string_mode = False
                             open_quote_location = None
 
                         elif self.nc in "\0\n":
@@ -466,67 +462,67 @@
                                          self.context_line[self.line - 1])
 
                         else:
                             # Otherwise, this must be part of our
                             # string, so add the character.
                             value += self.nc
 
-                    self.next()
+                    self.skip()
 
         else:
             # Ordinary lexing
 
             if self.cc in self.comment_char and \
                self.nc == "|" and \
                self.first_in_line and \
                self.process_pragmas:
                 # '%|' on its own in a new line begins an annotation.
                 self.in_annotation = True
                 kind = "ANNOTATION"
-                self.next()
+                self.skip()
 
             elif self.cc in self.comment_char:
                 # Comments go until the end of the line
                 kind = "COMMENT"
                 while self.nc not in ("\n", "\0"):
-                    self.next()
+                    self.skip()
 
             elif self.cc == "\n":
                 # Newlines are summarised into one token, except if
                 # we're in annotation mode
                 kind = "NEWLINE"
                 if self.in_annotation:
                     pass
                 else:
                     while self.nc in ("\n", " ", "\t"):
-                        self.next()
+                        self.skip()
 
             elif self.cc == ";":
                 kind = "SEMICOLON"
 
             elif not self.in_annotation and self.cc == "." and self.nc == ".":
                 # This is a continuation
-                self.next()
+                self.skip()
                 if self.nc == ".":
                     kind = "CONTINUATION"
-                    self.next()
+                    self.skip()
 
                     # We now need to eat everything until and including
                     # the next line
                     while self.cc not in ("\n", "\0"):
-                        self.next()
+                        self.skip()
 
                 else:
                     self.lex_error("expected . to complete continuation token")
 
             elif self.cc.isalpha():
                 # Could be an identifier or keyword
                 kind = "IDENTIFIER"
                 while self.nc.isalnum() or self.nc == "_":
-                    self.next()
+                    self.skip()
 
             elif self.cc.isnumeric() or \
                  self.cc == "." and self.nc.isnumeric():
                 # Its some kind of number
                 kind = "NUMBER"
                 tmp = self.match_re(
                     r"([0-9]+(\.[0-9]*)?([eE][+-]?[0-9]+)?[iIjJ]?)|"
@@ -540,36 +536,36 @@
                    self.nc == "." and self.nnc.isnumeric():
                     self.lex_error()
 
             elif self.cc in ("<", ">", "=", "~"):
                 # This is either a boolean relation, negation, or the
                 # assignment
                 if self.nc == "=":
-                    self.next()
+                    self.skip()
                     kind = "OPERATOR"
                 elif self.cc == "=":
                     kind = "ASSIGNMENT"
                 else:
                     kind = "OPERATOR"
 
             elif self.cc in ("+", "-", "*", "/", "^", "\\"):
                 kind = "OPERATOR"
 
             elif self.cc in ("&", "|"):
                 kind = "OPERATOR"
                 if self.nc == self.cc:
-                    self.next()
+                    self.skip()
 
             elif self.cc == "." and self.nc in ("*", "/", "\\", "^", "'"):
                 kind = "OPERATOR"
-                self.next()
+                self.skip()
 
             elif self.cc == "." and self.nc == "?":
                 kind = "NVP_DELEGATE"
-                self.next()
+                self.skip()
 
             elif self.cc == "'":
                 # This is either a single-quoted string or the
                 # transpose operation. If we had preceeding
                 # whitespace, it is never transpose. Otherwise it
                 # depends on bracket nesting level and/or the previous
                 # token. At this point I'd like to express a heartfelt
@@ -594,29 +590,29 @@
                     contains_quotes = True
                 else:
                     self.lex_error("unable to distinguish between string "
                                    "and transpose operation")
 
                 if kind == "CARRAY":
                     while True:
-                        self.next()
+                        self.skip()
                         if self.cc == "'" and self.nc == "'":
-                            self.next()
+                            self.skip()
                         elif self.cc == "'":
                             break
                         elif self.cc in ("\n", "\0"):
                             self.lex_error()
 
             elif self.cc == '"':
                 kind = "STRING"
                 contains_quotes = True
                 while True:
-                    self.next()
+                    self.skip()
                     if self.cc == '"' and self.nc == '"':
-                        self.next()
+                        self.skip()
                     elif self.cc == '"':
                         break
                     elif self.cc in ("\n", "\0"):
                         self.lex_error()
 
             elif self.cc == ",":
                 kind = "COMMA"
@@ -656,15 +652,15 @@
 
             elif self.cc == "@":
                 kind = "AT"
 
             elif self.cc == "!":
                 # Shell escapes go up to the end of the line
                 while self.nc not in ("\n", "\0"):
-                    self.next()
+                    self.skip()
                 kind = "BANG"
 
             elif self.cc == "?":
                 kind = "METACLASS"
 
             else:
                 self.lex_error()
@@ -1123,15 +1119,15 @@
         tok = self.delay_list.pop(0)
         return tok
 
 
 class Token_Buffer(Token_Generator):
     def __init__(self, lexer, cfg):
         assert isinstance(lexer, MATLAB_Lexer)
-        assert isinstance(cfg, dict)
+        assert isinstance(cfg, Config)
         super().__init__(lexer.filename, lexer.blockname)
 
         self.cfg = cfg
         self.pos = 0
         self.tokens = []
         self.mh = lexer.mh
         self.lines = lexer.line_count()
@@ -1279,19 +1275,19 @@
                     self.fixup_ws(new_tokens[-1], "after")
                     new_tokens[-1].first_in_line = next_token_is_fil
                     new_tokens[-1].first_in_statement = next_token_is_fis
                     token_deleted = False
 
                     # We might have to fix up indentation
                     if new_tokens[-1].first_in_statement and \
-                       config.active(self.cfg, "indentation"):
+                       self.cfg.active("indentation"):
                         if new_tokens[-1].ast_link:
                             new_tokens[-1].fix.correct_indent = (
                                 new_tokens[-1].ast_link.get_indentation() *
-                                self.cfg["tab_width"])
+                                self.cfg.style_config["tab_width"])
 
         # Add newlines
         tmp_tokens = new_tokens
         new_tokens = []
         newline_added = False
         shift_lines = 0
         previous_token = None
@@ -1302,23 +1298,23 @@
             # We've previously added a new-line. This means we need to
             # tidy up this token (specifically we need to indent it
             # correctly).
             if newline_added:
                 newline_added = False
                 token.first_in_line = True
                 token.first_in_statement = True
-                if config.active(self.cfg, "indentation"):
+                if self.cfg.active("indentation"):
                     if token.ast_link:
                         token.fix.correct_indent = (
                             token.ast_link.get_indentation() *
-                            self.cfg["tab_width"])
+                            self.cfg.style_config["tab_width"])
                     else:
                         token.fix.correct_indent = (
                             previous_token.ast_link.get_indentation() *
-                            self.cfg["tab_width"])
+                            self.cfg.style_config["tab_width"])
 
             # This token requires a newline to be inserted.
             if token.fix.add_newline:
                 newline_added = True
                 new_tokens.append(m_ast.MATLAB_Token("NEWLINE", "\n",
                                                      token.location,
                                                      False, False,
@@ -1352,15 +1348,15 @@
                 next_token = None
             if next_token and next_token.location.line == token.location.line:
                 next_in_line = next_token
             else:
                 next_in_line = None
 
             if token.first_in_line:
-                if config.active(self.cfg, "indentation") and \
+                if self.cfg.active("indentation") and \
                    token.fix.correct_indent is not None:
                     rv += " " * token.fix.correct_indent
                 else:
                     rv += " " * token.location.col_start
 
             if token.kind == "NEWLINE":
                 amount = min(2, token.raw_text.count("\n"))
```

### Comparing `miss_hit-0.9.7/miss_hit/m_parser.py` & `miss_hit-0.9.9/miss_hit/m_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 ##  along with MISS_HIT. If not, see <http://www.gnu.org/licenses/>.        ##
 ##                                                                          ##
 ##############################################################################
 
 import os
 import traceback
 
-from miss_hit import config
-
+from miss_hit.config import Config, METRICS
 from miss_hit.errors import ICE, Error, Message_Handler
 from miss_hit.m_ast import *
 from miss_hit.m_lexer import Token_Generator, MATLAB_Lexer, Token_Buffer
 
 
 IGNORED_TOKENS = frozenset(["COMMENT"])
 
@@ -77,15 +76,15 @@
 # 12. Short-circuit OR (||)
 
 
 class MATLAB_Parser:
     def __init__(self, mh, lexer, cfg):
         assert isinstance(mh, Message_Handler)
         assert isinstance(lexer, Token_Generator)
-        assert isinstance(cfg, dict)
+        assert isinstance(cfg, Config)
 
         self.lexer = lexer
         self.mh    = mh
         self.cfg   = cfg
 
         self.context = []
 
@@ -109,16 +108,16 @@
         self.ct  = None
         self.nt  = None
         self.nnt = None
         # pylint: enable=invalid-name
 
         self.debug_tree = False
 
-        self.next()
-        self.next()
+        self.skip()
+        self.skip()
 
     def sc_context(self, enabled):
         assert isinstance(enabled, bool)
 
         class CM:
             def __init__(self, parser, current_value, new_value):
                 self.parser    = parser
@@ -152,29 +151,41 @@
         for k in reversed(self.context):
             if kind == k:
                 return True
             elif k in ("function", "classdef"):
                 return False
         return False
 
-    def next(self):
-        self.ct = self.nt
-        self.nt = self.nnt
-        self.nnt = self.lexer.token()
-
+    def skip(self):
         def should_skip(token):
+            # Returns true iff this token should be completely passed
+            # over by the parser. We do this since the lexer produces
+            # tokens for whitespace and comments (needed for pretty
+            # printing in mh_style).
+
             if not token:
+                # Never skip EOF
                 return False
-            if token.kind in ("COMMENT",
-                              "CONTINUATION",
-                              "ANNOTATION"):
+            elif token.kind in ("COMMENT",
+                                "CONTINUATION",
+                                "ANNOTATION"):
+                # Skip all of these in all cases
                 return True
-            if token.annotation and token.kind == "NEWLINE":
+            elif token.annotation and token.kind == "NEWLINE":
+                # In MATLAB newlines are important. In MISS_HIT
+                # annotations they are not, so if we're in an
+                # annotation we can just ignore them.
                 return True
-            return False
+            else:
+                # Otherwise don't skip
+                return False
+
+        self.ct = self.nt
+        self.nt = self.nnt
+        self.nnt = self.lexer.token()
 
         while self.nnt:
             # Skip comments, continuations and annotation indications
             while should_skip(self.nnt):
                 self.nnt = self.lexer.token()
 
             # Join new-lines
@@ -184,15 +195,15 @@
                 self.nt.kind == "NEWLINE"):
                 self.nnt = self.lexer.token()
             else:
                 break
 
     def match(self, kind, value=None):
         assert kind in TOKEN_KINDS
-        self.next()
+        self.skip()
         if self.ct is None:
             self.mh.error(self.lexer.get_file_loc(),
                           "expected %s, reached EOF instead" % kind)
         elif self.ct.annotation:
             self.mh.error(self.ct.location,
                           "expected %s, "
                           "found miss_hit annotation instead" %
@@ -210,15 +221,15 @@
         elif value and self.ct.value != value:
             self.mh.error(self.ct.location,
                           "expected %s(%s), found %s(%s) instead" %
                           (kind, value, self.ct.kind, self.ct.value))
 
     def amatch(self, kind, value=None):
         assert kind in TOKEN_KINDS
-        self.next()
+        self.skip()
         if self.ct is None:
             self.mh.error(self.lexer.get_file_loc(),
                           "expected %s, reached EOF instead" % kind)
         elif not self.ct.annotation:
             self.mh.error(self.ct.location,
                           "expected %s annotation, "
                           "found normal program text instead" %
@@ -235,15 +246,15 @@
 
         elif value and self.ct.value != value:
             self.mh.error(self.ct.location,
                           "expected %s(%s), found %s(%s) instead" %
                           (kind, value, self.ct.kind, self.ct.value))
 
     def match_eof(self):
-        self.next()
+        self.skip()
         if self.ct is not None:
             if self.ct.annotation:
                 self.mh.error(self.ct.location,
                               "expected end of file, "
                               "found annotation %s instead" %
                               self.ct.kind)
             else:
@@ -304,15 +315,15 @@
 
         n_expr.set_enclosing_brackets(t_open, t_close)
 
     def check_redundant_brackets(self, n_expr):
         assert isinstance(n_expr, Expression), \
             "required expression, not %s" % n_expr.__class__.__name__
 
-        if config.active(self.cfg, "redundant_brackets") and \
+        if self.cfg.active("redundant_brackets") and \
            n_expr.t_bracket_open:
             self.mh.style_issue(n_expr.t_bracket_open.location,
                                 "redundant parenthesis",
                                 True)
             n_expr.t_bracket_open.fix.delete = True
             n_expr.t_bracket_close.fix.delete = True
 
@@ -346,43 +357,43 @@
         # The last token of the previous thing. We might need it later
         # to attach error messages or to record autofix instructions.
 
         # Get all terminator tokens that follow our ending token.
         terminator_tokens = []
         first_newline = None
         while self.peek_eos():
-            self.next()
+            self.skip()
             self.ct.set_ast(n_ast)
             self.ct.fix.statement_terminator = True
             terminator_tokens.append(self.ct)
             if self.ct.kind == "NEWLINE" and first_newline is None:
                 first_newline = len(terminator_tokens) - 1
                 break
         while self.peek_eos():  # and not self.peek("NEWLINE"):
-            self.next()
+            self.skip()
             self.ct.set_ast(n_ast)
             self.ct.fix.statement_terminator = True
             terminator_tokens.append(self.ct)
 
         if not terminator_tokens:
             # We found nothing. This is actually a syntax error in
             # most cases.
             if allow_nothing:
                 ending_token.fix.flag_continuations = True
-                if config.active(self.cfg, "end_of_statements"):
+                if self.cfg.active("end_of_statements"):
                     if semi:
                         ending_token.add_semicolon_after = True
-                        if config.active(self.cfg, "indentation"):
+                        if self.cfg.active("indentation"):
                             ending_token.fix.add_newline = True
                         self.mh.style_issue(ending_token.location,
                                             "end this with a ; and newline",
                                             True)
                     else:
                         fixed = False
-                        if config.active(self.cfg, "indentation"):
+                        if self.cfg.active("indentation"):
                             ending_token.fix.add_newline = True
                             fixed = True
                         self.mh.style_issue(ending_token.location,
                                             "end statement with a newline",
                                             fixed)
                 return
             elif self.peek_eof():
@@ -391,15 +402,15 @@
             else:
                 self.mh.error(self.nt.location,
                               "expected end of statement,"
                               " found %s instead" % self.nt.kind)
             raise ICE("logic error")
         assert len(terminator_tokens) >= 1
 
-        if not config.active(self.cfg, "end_of_statements"):
+        if not self.cfg.active("end_of_statements"):
             return
 
         if semi:
             # Exactly two tokens are required and useful. The first
             # semicolon, and the first new_line.
             if terminator_tokens[0].kind == "SEMICOLON":
                 pass
@@ -416,25 +427,25 @@
                 self.mh.style_issue(ending_token.location,
                                     "end statement with a semicolon",
                                     True)
                 ending_token.fix.add_semicolon_after = True
 
             if first_newline is None:
                 fixed = False
-                if config.active(self.cfg, "indentation"):
+                if self.cfg.active("indentation"):
                     terminator_tokens[0].fix.add_newline = True
                     fixed = True
                 self.mh.style_issue(terminator_tokens[0].location,
                                     "end statement with a newline",
                                     fixed)
 
         else:
             # Exactly one token is required and useful. The first new
             # line.
-            if not config.active(self.cfg, "indentation") and \
+            if not self.cfg.active("indentation") and \
                terminator_tokens[0].kind == "COMMA":
                 # The statement was ended with a comma. Ideally we
                 # just have a newline, but since we're not fixing
                 # indetation we can't fix it. Complain instead about
                 # the comma
                 self.mh.style_issue(ending_token.location,
                                     "end this with just a newline",
@@ -443,15 +454,15 @@
                     terminator_tokens[0].fix.change_to_semicolon = True
 
             elif terminator_tokens[0].kind != "NEWLINE":
                 fixed = False
                 if first_newline is None:
                     # We can only fix a missing newline if indentation
                     # fixing is active.
-                    if config.active(self.cfg, "indentation"):
+                    if self.cfg.active("indentation"):
                         terminator_tokens[0].fix.delete = True
                         ending_token.fix.add_newline = True
                         fixed = True
                 else:
                     terminator_tokens[0].fix.delete = True
                     fixed = True
                 self.mh.style_issue(terminator_tokens[0].location,
@@ -476,27 +487,24 @@
         # class methods called 'end' or 'methods'.
         #
         # The exception to this is 'end', since that is generally
         # allowed since it makes parsing expressions using ranges much
         # easier.
         if self.peek("OPERATOR", "~") and allow_void:
             self.match("OPERATOR")
-            return Identifier(self.ct)
         elif self.peek("KEYWORD", "end"):
             self.match("KEYWORD", "end")
-            return Identifier(self.ct)
         elif allow_some_keywords and self.peek("KEYWORD", "import"):
             self.match("KEYWORD", "import")
-            return Identifier(self.ct)
         elif allow_some_keywords and self.peek("KEYWORD", "arguments"):
             self.match("KEYWORD", "arguments")
-            return Identifier(self.ct)
         else:
             self.match("IDENTIFIER")
-            return Identifier(self.ct)
+
+        return Identifier(self.ct)
 
     def parse_name(self, allow_void):
         # superclass_ref ::= simple_name '@' function_reference
         #
         # simple_name ::= identifier
         #               | simple_name '.' identifier
         #
@@ -593,15 +601,15 @@
 
         # File can start with pragmas or newlines. We need to process
         # them first until we arrive at the first interesting thing
         # that helps us decide.
         l_pragmas = []
         while self.peek("NEWLINE") or self.apeek("KEYWORD", "pragma"):
             if self.peek("NEWLINE"):
-                self.next()
+                self.skip()
             else:
                 l_pragmas.append(self.parse_annotation_pragma())
 
         if self.peek("KEYWORD", "function"):
             l_functions, l_more_pragmas = self.parse_function_list()
             cunit = Function_File(os.path.basename(self.lexer.filename),
                                   self.lexer.get_file_loc(),
@@ -631,36 +639,33 @@
             if self.peek("KEYWORD", "function"):
                 break
             else:
                 statements.append(self.parse_statement())
 
         l_functions, l_more_pragmas = self.parse_function_list()
 
-        rv = Script_File(os.path.basename(self.lexer.filename),
-                         self.lexer.get_file_loc(),
-                         self.lexer.line_count(),
-                         Sequence_Of_Statements(statements),
-                         l_functions,
-                         l_pragmas + l_more_pragmas)
-
-        return rv
+        return Script_File(os.path.basename(self.lexer.filename),
+                           self.lexer.get_file_loc(),
+                           self.lexer.line_count(),
+                           Sequence_Of_Statements(statements),
+                           l_functions,
+                           l_pragmas + l_more_pragmas)
 
     def parse_class_file(self, l_pragmas):
         self.functions_require_end = True
 
         n_classdef                  = self.parse_classdef()
         l_functions, l_more_pragmas = self.parse_function_list()
 
-        rv = Class_File(os.path.basename(self.lexer.filename),
-                        self.lexer.get_file_loc(),
-                        self.lexer.line_count(),
-                        n_classdef,
-                        l_functions,
-                        l_pragmas + l_more_pragmas)
-        return rv
+        return Class_File(os.path.basename(self.lexer.filename),
+                          self.lexer.get_file_loc(),
+                          self.lexer.line_count(),
+                          n_classdef,
+                          l_functions,
+                          l_pragmas + l_more_pragmas)
 
     def parse_function_list(self):
         l_functions = []
         l_pragmas = []
         while self.peek("KEYWORD", "function") or \
               self.apeek("KEYWORD", "pragma"):
             if self.peek("KEYWORD", "function"):
@@ -698,27 +703,26 @@
 
         # Parse returns. Either 'x' or a list '[x, y]'
         l_outputs = []
         if self.peek("A_BRA"):
             out_brackets = True
             self.match("A_BRA")
             self.ct.set_ast(rv)
-            if self.peek("A_KET"):
-                self.match("A_KET")
-                self.ct.set_ast(rv)
-            else:
+
+            if not self.peek("A_KET"):
                 while True:
                     l_outputs.append(self.parse_identifier(allow_void=True))
                     if self.peek("COMMA"):
                         self.match("COMMA")
                         self.ct.set_ast(rv)
                     else:
                         break
-                self.match("A_KET")
-                self.ct.set_ast(rv)
+
+            self.match("A_KET")
+            self.ct.set_ast(rv)
 
         else:
             out_brackets = False
             l_outputs.append(self.parse_simple_name())
 
         if self.peek("BRA") and len(l_outputs) == 1 and not out_brackets:
             # This is a function that doesn't return anything, so
@@ -739,27 +743,26 @@
             self.ct.set_ast(rv)
             n_name = self.parse_simple_name(allow_some_keywords=True)
 
         l_inputs = []
         if self.peek("BRA"):
             self.match("BRA")
             self.ct.set_ast(rv)
-            if self.peek("KET"):
-                self.match("KET")
-                self.ct.set_ast(rv)
-            else:
+
+            if not self.peek("KET"):
                 while True:
                     l_inputs.append(self.parse_identifier(allow_void=True))
                     if self.peek("COMMA"):
                         self.match("COMMA")
                         self.ct.set_ast(rv)
                     else:
                         break
-                self.match("KET")
-                self.ct.set_ast(rv)
+
+            self.match("KET")
+            self.ct.set_ast(rv)
 
         rv.set_name(n_name)
         rv.set_inputs(l_inputs)
         rv.set_outputs(l_outputs)
         self.match_eos(rv)
         return rv
 
@@ -1151,15 +1154,15 @@
 
         self.amatch("COMMA")
         punctuation.append(self.ct)
 
         self.amatch("STRING")
         t_param = self.ct
 
-        if t_param.value not in config.METRICS:
+        if t_param.value not in METRICS:
             self.mh.warning(t_param.location,
                             "unknown metric '%s'" % t_param.value)
 
         self.amatch("COMMA")
         punctuation.append(self.ct)
 
         n_reason = self.parse_annotation_static_string_expression()
@@ -1185,15 +1188,15 @@
                           "expected valid miss_hit annotation statement")
 
     def parse_statement(self):
         if self.in_shortcircuit_context:
             raise ICE("failed to unset sc context")
 
         while self.peek("NEWLINE"):
-            self.next()
+            self.skip()
 
         if self.peek("KEYWORD"):
             if self.nt.value == "for":
                 return self.parse_for_statement()
             elif self.nt.value == "if":
                 return self.parse_if_statement()
             elif self.nt.value == "global":
@@ -1253,15 +1256,15 @@
                 t_eq = self.ct
                 if not isinstance(rv, Name):
                     self.mh.error(t_eq.location,
                                   "left-hand side of assignment must be a"
                                   " Name, found %s instead" %
                                   rv.__class__.__name__)
                 rhs = self.parse_nested_expression()
-                if config.active(self.cfg, "builtin_shadow"):
+                if self.cfg.active("builtin_shadow"):
                     rv.sty_check_builtin_shadow(self.mh, self.cfg)
                 rv = Simple_Assignment_Statement(t_eq, rv, rhs)
 
             elif self.peek("CARRAY"):
                 # Sanity check that the function is a simple name
                 if not isinstance(rv, (Identifier, Selection)):
                     self.mh.error(self.ct.location,
@@ -1306,15 +1309,15 @@
             # There is a special case we need to take care of with
             # ~. There is a MATLAB bug/weirdness with [~ x], which is
             # parsed like [~x], but [x y] is OK for some reason. See
             # issue #70. Hence we enforce commas after any ~.
             if self.peek("OPERATOR", "~"):
                 require_comma = True
             target = self.parse_name(allow_void=True)
-            if config.active(self.cfg, "builtin_shadow"):
+            if self.cfg.active("builtin_shadow"):
                 target.sty_check_builtin_shadow(self.mh, self.cfg)
             lhs.append(target)
             if (self.peek("COMMA") or require_comma) and \
                not self.peek("A_KET"):
                 self.match("COMMA")
                 self.ct.set_ast(rv)
                 require_comma = False
@@ -2082,18 +2085,18 @@
                     cfg.debug_write_dot(node.name)
 
     mh.register_file(filename)
     with open(filename, "r") as fd:
         content = fd.read()
     try:
         lexer = MATLAB_Lexer(mh, content, filename)
-        tbuf = Token_Buffer(lexer, config.BASE_CONFIG)
+        tbuf = Token_Buffer(lexer, Config())
         parser = MATLAB_Parser(mh,
                                tbuf,
-                               config.BASE_CONFIG)
+                               Config())
         parser.debug_tree = show_dot
         tree = parser.parse_file()
         if show_tree:
             print("-" * 70)
             print("--  Parse tree for %s" % os.path.basename(filename))
             tree.pp_node()
             print("-" * 70)
```

### Comparing `miss_hit-0.9.7/miss_hit/mh_metric.py` & `miss_hit-0.9.9/miss_hit/mh_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,24 +293,24 @@
 
 
 ##############################################################################
 # Infrastructure
 ##############################################################################
 
 def check_metric(mh, cfg, loc, metric, metrics, justifications):
-    if not config.metric_enabled(cfg, metric):
+    if not cfg.metric_enabled(metric):
         return
 
-    elif config.metric_check(cfg, metric):
+    elif cfg.metric_check(metric):
         measure = metrics[metric]["measure"]
 
         if measure is None:
             return
 
-        limit = config.metric_upper_limit(cfg, metric)
+        limit = cfg.metric_upper_limit(metric)
         metrics[metric]["limit"] = limit
         if measure > limit:
             if metric in justifications:
                 mh.metric_justifications += 1
                 justifications[metric].applies = True
                 metrics[metric]["reason"] = justifications[metric].reason()
             else:
@@ -365,14 +365,16 @@
                 else:
                     justifications[n_pragma.metric()] = n_pragma
 
     return justifications
 
 
 def get_function_metrics(mh, cfg, tree):
+    assert isinstance(mh, Message_Handler)
+    assert isinstance(cfg, config.Config)
     assert isinstance(tree, Compilation_Unit)
 
     metrics = {}
     justifications = {}
 
     def process_function(n_fdef, naming_stack):
         assert isinstance(n_fdef, Function_Definition)
@@ -380,15 +382,15 @@
         # We need a unique name for the function for this function.
         name = "::".join(map(str, naming_stack + [n_fdef.n_sig.n_name]))
 
         metrics[name] = {m: {"measure" : MEASURE[m](n_fdef),
                              "limit"   : None,
                              "reason"  : None}
                          for m in config.FUNCTION_METRICS
-                         if config.metric_enabled(cfg, m)}
+                         if cfg.metric_enabled(m)}
 
         justifications[name] = get_justifications(mh, n_fdef.n_body)
 
         return name
 
     def process_script(n_script):
         assert isinstance(n_script, Script_File)
@@ -396,15 +398,15 @@
         # We need a unique name for the script
         name = n_script.name.rsplit(".")[0]
 
         metrics[name] = {m: {"measure" : MEASURE[m](n_script),
                              "limit"   : None,
                              "reason"  : None}
                          for m in config.FUNCTION_METRICS
-                         if config.metric_enabled(cfg, m)}
+                         if cfg.metric_enabled(m)}
 
         justifications[name] = get_justifications(mh, n_script.n_statements)
 
         return name
 
     class Function_Visitor(AST_Visitor):
         def __init__(self):
@@ -473,38 +475,38 @@
 
         for file_metric in config.FILE_METRICS:
             if file_metric not in metrics["metrics"]:
                 continue
             results = metrics["metrics"][file_metric]
             if results["measure"] is None:
                 continue
-            fd.write("  %s: %u" % (config.METRICS[file_metric]["name"],
+            fd.write("  %s: %u" % (config.METRICS[file_metric].longname,
                                    results["measure"]))
             if results["reason"]:
                 fd.write(" (%s)\n" % results["reason"])
             elif results["limit"] and results["measure"] > results["limit"]:
                 fd.write(" (!not justified!)\n")
             else:
                 fd.write("\n")
 
         for function in sorted(metrics["functions"]):
             fd.write("\n")
             fd.write("  Code metrics for function %s:\n" % function)
-            max_len = max((len(config.METRICS[m]["name"])
+            max_len = max((len(config.METRICS[m].longname)
                            for m in metrics["functions"][function]),
                           default=0)
             for function_metric in config.FUNCTION_METRICS:
                 if function_metric not in metrics["functions"][function]:
                     continue
                 results = metrics["functions"][function][function_metric]
                 if results["measure"] is None:
                     continue
                 fd.write("    %-*s: %u" %
                          (max_len,
-                          config.METRICS[function_metric]["name"],
+                          config.METRICS[function_metric].longname,
                           results["measure"]))
                 if results["reason"]:
                     fd.write(" (%s)\n" % results["reason"])
                 elif results["limit"] and \
                      results["measure"] > results["limit"]:
                     fd.write(" (!not justified!)\n")
                 else:
@@ -513,28 +515,28 @@
     if worst_offenders:
         fd.write("\n=== Global summary of worst offenders by metric:\n\n")
 
         for file_metric in config.FILE_METRICS:
             if file_metric not in worst_offenders:
                 continue
             fd.write("* File metric '%s':\n" %
-                     config.METRICS[file_metric]["name"])
+                     config.METRICS[file_metric].longname)
             for rank, file_name in enumerate(worst_offenders[file_metric], 1):
                 if file_name:
                     mdata = all_metrics[file_name]["metrics"][file_metric]
                     fd.write("  %u. %u (%s)\n" % (rank,
                                                   mdata["measure"],
                                                   file_name))
             fd.write("\n")
 
         for function_metric in config.FUNCTION_METRICS:
             if function_metric not in worst_offenders:
                 continue
             fd.write("* Function metric '%s':\n" %
-                     config.METRICS[function_metric]["name"])
+                     config.METRICS[function_metric].longname)
             for rank, tup in enumerate(worst_offenders[function_metric], 1):
                 if tup:
                     file_name, function_name = tup
                     mdata = (all_metrics[file_name]["functions"]
                              [function_name][function_metric])
                     fd.write("  %u. %u (%s, function %s)\n" %
                              (rank,
@@ -578,21 +580,21 @@
 
         fd.write("<thead>\n")
         fd.write("<tr>\n")
         fd.write("  <td>Rank</td>\n")
         for file_metric in config.FILE_METRICS:
             if file_metric in worst_offenders:
                 fd.write("  <td class='tip' tip='%s'>%s</td>\n" %
-                         (config.METRICS[file_metric]["help"],
-                          config.METRICS[file_metric]["name"]))
+                         (config.METRICS[file_metric].description,
+                          config.METRICS[file_metric].longname))
         for function_metric in config.FUNCTION_METRICS:
             if function_metric in worst_offenders:
                 fd.write("  <td class='tip' tip='%s'>%s</td>\n" %
-                         (config.METRICS[function_metric]["help"],
-                          config.METRICS[function_metric]["name"]))
+                         (config.METRICS[function_metric].description,
+                          config.METRICS[function_metric].longname))
         fd.write("</tr>\n")
         fd.write("</thead>\n")
         fd.write("<tbody>\n")
 
         count = worst_offender_count(worst_offenders)
         for rank in range(count):
             fd.write("<tr>\n")
@@ -662,22 +664,22 @@
         fd.write("<thead>\n")
         fd.write("<tr>\n")
         fd.write("  <td>Item</td>\n")
         for file_metric in config.FILE_METRICS:
             if file_metric in metrics["disabled"]:
                 continue
             fd.write("  <td class='tip' tip='%s'>%s</td>\n" %
-                     (config.METRICS[file_metric]["help"],
-                      config.METRICS[file_metric]["name"]))
+                     (config.METRICS[file_metric].description,
+                      config.METRICS[file_metric].longname))
         for function_metric in config.FUNCTION_METRICS:
             if function_metric in metrics["disabled"]:
                 continue
             fd.write("  <td class='tip' tip='%s'>%s</td>\n" %
-                     (config.METRICS[function_metric]["help"],
-                      config.METRICS[function_metric]["name"]))
+                     (config.METRICS[function_metric].description,
+                      config.METRICS[function_metric].longname))
         fd.write("</tr>\n")
         fd.write("</thead>\n")
         fd.write("<tbody>\n")
 
         fd.write("<tr>\n")
         fd.write("  <td>%s</td>\n" % os.path.basename(filename))
         for file_metric in config.FILE_METRICS:
@@ -836,26 +838,26 @@
 
         metrics = {
             full_name: {
                 "errors"    : False,
                 "metrics"   : {},
                 "functions" : {},
                 "disabled"  : set(m for m in config.METRICS
-                                  if not config.metric_enabled(wp.cfg, m))
+                                  if not wp.cfg.metric_enabled(m))
             }
         }
         justifications = {}
 
         # Create lexer
 
         lexer = MATLAB_Lexer(wp.mh, wp.get_content(),
                              wp.filename, wp.blockname)
-        if wp.cfg["octave"]:
+        if wp.cfg.octave:
             lexer.set_octave_mode()
-        if wp.cfg["ignore_pragmas"]:
+        if not wp.cfg.pragmas:
             lexer.process_pragmas = False
 
         # We're dealing with an empty file here. Lets just not do anything
 
         if len(lexer.text.strip()) == 0:
             return MH_Metric_Result(wp, metrics)
 
@@ -866,15 +868,15 @@
             parse_tree = parser.parse_file()
         except Error:
             metrics[wp.filename]["errors"] = True
             return MH_Metric_Result(wp, metrics)
 
         # Collect file metrics
 
-        if config.metric_enabled(wp.cfg, "file_length"):
+        if wp.cfg.metric_enabled("file_length"):
             metrics[full_name]["metrics"]["file_length"] = {
                 "measure" : lexer.line_count(),
                 "limit"   : None,
                 "reason"  : None
             }
 
         # Check+justify file metrics
```

### Comparing `miss_hit-0.9.7/miss_hit/mh_style.py` & `miss_hit-0.9.9/miss_hit/mh_style.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,30 +81,31 @@
     """
 
     parameters = {
         "file_length": {
             "type"    : int,
             "metavar" : "N",
             "help"    : ("Maximum lines in a file, %u by default." %
-                         config.BASE_CONFIG["file_length"]),
+                         config.STYLE_CONFIGURATION["file_length"].default)
         }
     }
 
     defaults = {
-        "file_length" : config.BASE_CONFIG["file_length"],
+        "file_length" : config.STYLE_CONFIGURATION["file_length"].default,
     }
 
     def __init__(self):
         super().__init__("file_length")
 
     def apply(self, mh, cfg, filename, full_text, lines):
-        if len(lines) > cfg["file_length"]:
+        if len(lines) > cfg.style_config["file_length"]:
             mh.style_issue(Location(filename,
                                     len(lines)),
-                           "file exceeds %u lines" % cfg["file_length"],
+                           "file exceeds %u lines" %
+                           cfg.style_config["file_length"],
                            self.autofix)
 
 
 class Rule_File_EOF_Lines(Style_Rule_File):
     """Trailing newlines at end of file
 
     This mandatory rule makes sure there is a single trailing newline
@@ -141,33 +142,34 @@
     """
 
     parameters = {
         "line_length": {
             "type"    : int,
             "metavar" : "N",
             "help"    : ("Maximum characters per line, %u by default." %
-                         config.BASE_CONFIG["line_length"]),
+                         config.STYLE_CONFIGURATION["line_length"].default),
         }
     }
 
     defaults = {
-        "line_length" : config.BASE_CONFIG["line_length"],
+        "line_length" : config.STYLE_CONFIGURATION["line_length"].default,
     }
 
     def __init__(self):
         super().__init__("line_length", False)
 
     def apply(self, mh, cfg, filename, line_no, line):
-        if len(line) > cfg["line_length"]:
+        if len(line) > cfg.style_config["line_length"]:
             mh.style_issue(Location(filename,
                                     line_no,
-                                    cfg["line_length"],
+                                    cfg.style_config["line_length"],
                                     len(line),
                                     line),
-                           "line exceeds %u characters" % cfg["line_length"],
+                           "line exceeds %u characters" %
+                           cfg.style_config["line_length"],
                            self.autofix)
 
 
 class Rule_Line_Blank_Lines(Style_Rule_Line):
     """Consecutive blank lines
 
     This rule allows a maximum of one blank line to separate code blocks.
@@ -218,20 +220,20 @@
     """
 
     parameters = {
         "tab_width": {
             "type"    : int,
             "metavar" : "N",
             "help"    : ("Tab-width, by default %u." %
-                         config.BASE_CONFIG["tab_width"]),
+                         config.STYLE_CONFIGURATION["tab_width"].default),
         }
     }
 
     defaults = {
-        "tab_width" : config.BASE_CONFIG["tab_width"],
+        "tab_width" : config.STYLE_CONFIGURATION["tab_width"].default,
     }
 
     def __init__(self):
         super().__init__("tabs", True)
         self.mandatory = True
 
     def apply(self, mh, cfg, filename, line_no, line):
@@ -310,15 +312,15 @@
         "on_line" : [],
         "on_token" : []
     }
 
     for kind in rules:
         for rule in rules[kind]:
             inst = rule()
-            if inst.mandatory or config.active(cfg, inst.name):
+            if inst.mandatory or cfg.active(inst.name):
                 lib[kind].append(inst)
 
     return lib
 
 
 ##############################################################################
 
@@ -345,17 +347,18 @@
 
 
 def stage_3_analysis(mh, cfg, tbuf, is_embedded):
     assert isinstance(mh, Message_Handler)
     assert isinstance(tbuf, Token_Buffer)
     assert isinstance(is_embedded, bool)
 
-    in_copyright_notice = (config.active(cfg, "copyright_notice") and
+    in_copyright_notice = (cfg.active("copyright_notice") and
                            (not is_embedded or
-                            cfg["copyright_in_embedded_code"]))
+                            cfg.style_config["copyright_in_embedded_code"]))
+    entities = cfg.style_config["copyright_entity"]
     company_copyright_found = False
     generic_copyright_found = False
     copyright_token = None
     copyright_notice = []
 
     # Some state needed to fix indentation
     statement_start_token = None
@@ -436,21 +439,21 @@
         if in_copyright_notice:
             if token.kind == "COMMENT":
                 match = re.search(COPYRIGHT_REGEX, token.value)
                 if match:
                     # We have a sane copyright string
                     copyright_token = token
                     generic_copyright_found = True
-                    if match.group("org").strip() in cfg["copyright_entity"]:
+                    if match.group("org").strip() in entities:
                         company_copyright_found = True
 
                 elif copyright_token is None:
                     # We might find something that could look like a
                     # copyright, but is not quite right
-                    for org in cfg["copyright_entity"]:
+                    for org in entities:
                         if org.lower() in token.value.lower():
                             copyright_token = token
                             break
                     for substr in ("(c)", "copyright"):
                         if substr in token.value.lower():
                             copyright_token = token
                             break
@@ -470,18 +473,18 @@
                 elif company_copyright_found:
                     # Everything is fine
                     pass
                 elif generic_copyright_found:
                     # If we have something basic, we only raise an
                     # issue if we're supposed to have something
                     # specific.
-                    if cfg["copyright_entity"]:
+                    if entities:
                         mh.style_issue(copyright_token.location,
                                        "Copyright does not mention one of %s" %
-                                       (" or ".join(cfg["copyright_entity"])))
+                                       (" or ".join(entities)))
                 elif copyright_token:
                     # We found something that might be a copyright,
                     # but is not in a sane format
                     mh.style_issue(copyright_token.location,
                                    "Copyright notice not in right format")
                 else:
                     # We found nothing
@@ -489,27 +492,27 @@
                                    "No copyright notice found in header")
 
         # Corresponds to the old CodeChecker CommaWhitespace
         # rule. CommaLineEndings is now folded into the new
         # end_of_statements rule, which is much more strict and
         # complete.
         if token.kind == "COMMA":
-            if config.active(cfg, "whitespace_comma"):
+            if cfg.active("whitespace_comma"):
                 token.fix.ensure_trim_before = True
                 token.fix.ensure_ws_after = True
 
                 if (next_in_line and ws_after == 0) or \
                    (prev_in_line and ws_before > 0):
                     mh.style_issue(token.location,
                                    "comma cannot be preceeded by whitespace "
                                    "and must be followed by whitespace",
                                    True)
 
         elif token.kind == "COLON":
-            if config.active(cfg, "whitespace_colon"):
+            if cfg.active("whitespace_colon"):
                 if prev_in_line and prev_in_line.kind == "COMMA":
                     pass
                     # We don't deal with this here. If anything it's the
                     # problem of the comma whitespace rules.
                 elif next_in_line and \
                      next_in_line.kind == "CONTINUATION":
                     # Special exception in the rare cases we
@@ -526,15 +529,15 @@
                     mh.style_issue(token.location,
                                    "no whitespace around colon"
                                    " allowed",
                                    True)
 
         # Corresponds to the old CodeChecker EqualSignWhitespace rule
         elif token.kind == "ASSIGNMENT":
-            if config.active(cfg, "whitespace_assignment"):
+            if cfg.active("whitespace_assignment"):
                 token.fix.ensure_ws_before = True
                 token.fix.ensure_ws_after = True
 
                 if prev_in_line and ws_before == 0:
                     mh.style_issue(token.location,
                                    "= must be preceeded by whitespace",
                                    True)
@@ -542,45 +545,45 @@
                     mh.style_issue(token.location,
                                    "= must be succeeded by whitespace",
                                    True)
 
         # Corresponds to the old CodeChecker ParenthesisWhitespace and
         # BracketsWhitespace rules
         elif token.kind in ("BRA", "A_BRA", "M_BRA"):
-            if config.active(cfg, "whitespace_brackets") and \
+            if cfg.active("whitespace_brackets") and \
                next_in_line and ws_after > 0 and \
                next_in_line.kind != "CONTINUATION":
                 mh.style_issue(token.location,
                                "%s must not be followed by whitespace" %
                                token.raw_text,
                                True)
                 token.fix.ensure_trim_after = True
 
         elif token.kind in ("KET", "A_KET", "M_KET"):
-            if config.active(cfg, "whitespace_brackets") and \
+            if cfg.active("whitespace_brackets") and \
                prev_in_line and ws_before > 0:
                 mh.style_issue(token.location,
                                "%s must not be preceeded by whitespace" %
                                token.raw_text,
                                True)
                 token.fix.ensure_trim_before = True
 
         # Corresponds to the old CodeChecker KeywordWhitespace rule
         elif (token.kind == "KEYWORD" and
               token.value in KEYWORDS_WITH_WS):
-            if config.active(cfg, "whitespace_keywords") and \
+            if cfg.active("whitespace_keywords") and \
                next_in_line and ws_after == 0:
                 mh.style_issue(token.location,
                                "keyword must be succeeded by whitespace",
                                True)
                 token.fix.ensure_ws_after = True
 
         # Corresponds to the old CodeChecker CommentWhitespace rule
         elif token.kind == "COMMENT":
-            if config.active(cfg, "whitespace_comments"):
+            if cfg.active("whitespace_comments"):
                 comment_char = token.raw_text[0]
                 comment_body = token.raw_text.lstrip(comment_char)
                 if re.match("^%#[a-zA-Z]", token.raw_text):
                     # Stuff like %#codegen or %#ok are pragmas and should
                     # not be subject to style checks
                     pass
 
@@ -634,47 +637,47 @@
                     mh.style_issue(token.location,
                                    "comment must be preceeded by whitespace",
                                    True)
                     token.fix.ensure_ws_before = True
 
         elif token.kind == "CONTINUATION":
             # Make sure we have whitespace before each line continuation
-            if config.active(cfg, "whitespace_continuation") and \
+            if cfg.active("whitespace_continuation") and \
                prev_in_line and ws_before == 0:
                 mh.style_issue(token.location,
                                "continuation must be preceeded by whitespace",
                                True)
                 token.fix.ensure_ws_before = True
 
-            if config.active(cfg, "operator_after_continuation") and \
+            if cfg.active("operator_after_continuation") and \
                next_token and next_token.first_in_line and \
                next_token.kind == "OPERATOR" and \
                next_token.fix.binary_operator:
                 # Continuations should not start with operators unless
                 # its a unary.
                 mh.style_issue(next_token.location,
                                "continuations should not start with binary "
                                "operators")
 
-            if config.active(cfg, "useless_continuation"):
+            if cfg.active("useless_continuation"):
                 if next_token and next_token.kind in ("NEWLINE", "COMMENT"):
                     # Continuations followed immediately by a new-line
                     # or comment are not actually helpful at all.
                     mh.style_issue(token.location,
                                    "useless line continuation",
                                    True)
                     token.fix.replace_with_newline = True
                 elif prev_token and prev_token.fix.statement_terminator:
                     mh.style_issue(token.location,
                                    "useless line continuation",
                                    True)
                     token.fix.delete = True
 
         elif token.kind == "OPERATOR":
-            if not config.active(cfg, "operator_whitespace"):
+            if not cfg.active("operator_whitespace"):
                 pass
             elif token.fix.unary_operator:
                 if (prev_in_line and ws_before > 0) and \
                    token.value in (".'", "'"):
                     mh.style_issue(token.location,
                                    "suffix operator must not be preceeded by"
                                    " whitespace",
@@ -703,15 +706,15 @@
                         mh.style_issue(token.location,
                                        "non power binary operator"
                                        " must be surrounded by whitespace",
                                        True)
                         token.fix.ensure_ws_before = True
                         token.fix.ensure_ws_after = True
 
-            if config.active(cfg, "implicit_shortcircuit") and \
+            if cfg.active("implicit_shortcircuit") and \
                token.value in ("&", "|") and \
                token.ast_link and \
                isinstance(token.ast_link, Binary_Logical_Operation) and \
                token.ast_link.short_circuit:
                 # This rule is *disabled* for now since it does not
                 # work in all circumstances. Curiously, this bug is
                 # shared by mlint which also mis-classifies & when
@@ -727,45 +730,45 @@
                 #                " expression being contained in "
                 #                " if/while guard",
                 #                True)
                 # token.fix.make_shortcircuit_explicit = True
                 pass
 
         elif token.kind == "ANNOTATION":
-            if config.active(cfg, "annotation_whitespace"):
+            if cfg.active("annotation_whitespace"):
                 token.fix.ensure_ws_after = True
 
                 if next_in_line and ws_after == 0:
                     mh.style_issue(token.location,
                                    "annotation indication must be succeeded"
                                    " by whitespace",
                                    True)
 
         elif token.kind == "NEWLINE":
-            if n == 0 and config.active(cfg, "no_starting_newline"):
+            if n == 0 and cfg.active("no_starting_newline"):
                 # Files should not *start* with newline(s)
                 mh.style_issue(token.location,
                                "files should not start with a newline",
                                True)
                 token.fix.delete = True
 
         # Check some specific problems with continuations
         if token.fix.flag_continuations and \
            next_in_line and next_in_line.kind == "CONTINUATION":
             fixed = False
             token.fix.add_newline = False
-            if config.active(cfg, "dangerous_continuation"):
+            if cfg.active("dangerous_continuation"):
                 next_in_line.fix.replace_with_newline = True
                 fixed = True
             mh.style_issue(next_in_line.location,
                            "this continuation is dangerously misleading",
                            fixed)
 
         # Complain about indentation
-        if config.active(cfg, "indentation") and token.kind != "NEWLINE":
+        if cfg.active("indentation") and token.kind != "NEWLINE":
             if token.first_in_line and not token.block_comment:
                 if token.first_in_statement:
                     if token.ast_link:
                         current_indent = token.ast_link.get_indentation()
                     elif enclosing_ast:
                         current_indent = enclosing_ast.get_indentation() + 1
                     offset = 0
@@ -779,17 +782,19 @@
                         statement_start_token.location.col_start
 
                     # If positive, we can just add it. If 0 or
                     # negative, then we add 1/2 tabs to continue
                     # the line, since previously it was not offset
                     # at all.
                     if offset <= 0:
-                        offset = cfg["tab_width"] // 2
+                        offset = cfg.style_config["tab_width"] // 2
 
-                correct_spaces = cfg["tab_width"] * current_indent + offset
+                correct_spaces = (cfg.style_config["tab_width"] *
+                                  current_indent +
+                                  offset)
                 token.fix.correct_indent = correct_spaces
 
                 if token.location.col_start != correct_spaces:
                     mh.style_issue(token.location,
                                    "indentation not correct, should be"
                                    " %u spaces, not %u" %
                                    (correct_spaces,
@@ -820,17 +825,17 @@
         # Load file content
 
         content = wp.get_content()
 
         # Create lexer
 
         lexer = MATLAB_Lexer(wp.mh, content, wp.filename, wp.blockname)
-        if wp.cfg["octave"]:
+        if wp.cfg.octave:
             lexer.set_octave_mode()
-        if wp.cfg["ignore_pragmas"]:
+        if not wp.cfg.pragmas:
             lexer.process_pragmas = False
 
         # We're dealing with an empty file here. Lets just not do anything
 
         if len(lexer.text.strip()) == 0:
             return MH_Style_Result(wp)
 
@@ -867,15 +872,15 @@
         # This is probably not correct. Fixing this is will require a very
         # different kind of lexing (which I am not in the mood for, I have
         # suffered enough to deal with ') or a 2-pass solution (which is
         # slow): first we lex and then fix up tabs inside tokens; and then
         # we do the global replacement and lex again before we proceed.
 
         if autofix:
-            lexer.correct_tabs(wp.cfg["tab_width"])
+            lexer.correct_tabs(wp.cfg.style_config["tab_width"])
 
         # Create tokenbuffer
 
         try:
             tbuf = Token_Buffer(lexer, wp.cfg)
         except Error:
             # If there are lex errors, we can stop here
```

### Comparing `miss_hit-0.9.7/miss_hit/s_ast.py` & `miss_hit-0.9.9/miss_hit/s_ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,16 +102,15 @@
         assert isinstance(encoding, str)
         self.encoding = encoding
 
     def loc(self):
         return Location(self.filename)
 
     def iter_all_blocks(self):
-        for n_block in self.n_system.iter_all_blocks():
-            yield n_block
+        yield from self.n_system.iter_all_blocks()
 
 
 class Model(Container):
     def dump_hierarchy(self, indent=0):
         print(" " * indent, "Model")
         self.n_system.dump_hierarchy(indent + 1)
 
@@ -143,16 +142,15 @@
     def dump_hierarchy(self, indent=0):
         print(" " * indent, "System")
         for n_block in self.blocks():
             n_block.dump_hierarchy(indent + 1)
 
     def iter_all_blocks(self):
         for n_block in self.d_blocks.values():
-            for item in n_block.iter_all_blocks():
-                yield item
+            yield from n_block.iter_all_blocks()
 
 
 class Block(Node):
     def __init__(self, sid, name, kind):
         assert isinstance(sid, str), "expected string, got %s" % type(sid)
         assert isinstance(name, str)
         assert isinstance(kind, str)
@@ -220,16 +218,15 @@
 
     def dump_hierarchy(self, indent=0):
         print(" " * indent, "Block %s (%s)" % (self.kind, repr(self.name)))
         self.n_system.dump_hierarchy(indent + 1)
 
     def iter_all_blocks(self):
         yield self
-        for n_block in self.n_system.iter_all_blocks():
-            yield n_block
+        yield from self.n_system.iter_all_blocks()
 
 
 class Matlab_Function(Block):
     # In Simulink this is actually a magic Subsystem that you cannot
     # enter, that contains an S-Function block referencing a Stateflow
     # MATLAB function. We hide this as well, but in a different way:
     # we pretend it's a distinct top-level object (and not a special
```

### Comparing `miss_hit-0.9.7/miss_hit/s_parser.py` & `miss_hit-0.9.9/miss_hit/s_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,29 +31,28 @@
 
 import os.path
 import zipfile
 import xml.etree.ElementTree as ET
 
 from abc import ABCMeta, abstractmethod
 
-from miss_hit import config
-
+from miss_hit.config import Config
 from miss_hit.s_ast import *
 from miss_hit.errors import Message_Handler, ICE
 
 # pylint: disable=invalid-name
 anatomy = {}
 # pylint: enable=invalid-name
 
 
 class Simulink_Parser(metaclass=ABCMeta):
     def __init__(self, mh, filename, cfg):
         assert isinstance(mh, Message_Handler)
         assert isinstance(filename, str)
-        assert isinstance(cfg, dict)
+        assert isinstance(cfg, Config)
 
         self.mh       = mh
         self.filename = filename
         self.cfg      = cfg
         # Basic properties
 
     @abstractmethod
@@ -277,19 +276,17 @@
                     self.mh.error(self.loc(),
                                   "Unexpected child %s of eml" % et_item.tag)
                 if et_script and not is_eml:
                     raise ICE("script found, but isEML is not true")
         if et_script is None:
             raise ICE("referenced script for %s not found" % sf_base_name)
 
-        n_block = Matlab_Function(et_block.attrib["SID"],
-                                  et_block.attrib["Name"],
-                                  SLX_Reference(et_script))
-
-        return n_block
+        return Matlab_Function(et_block.attrib["SID"],
+                               et_block.attrib["Name"],
+                               SLX_Reference(et_script))
 
     def parse_block_subsystem(self, et_block):
         assert isinstance(et_block, ET.Element)
         assert et_block.tag == "Block"
         assert et_block.attrib["BlockType"] == "SubSystem"
 
         n_system    = None
@@ -467,15 +464,15 @@
     # pylint: disable=import-outside-toplevel
     from miss_hit import m_lexer
     # pylint: enable=import-outside-toplevel
 
     print("=== Parsing %s ===" % filename)
 
     mh.register_file(filename)
-    slp = Simulink_SLX_Parser(mh, filename, config.BASE_CONFIG)
+    slp = Simulink_SLX_Parser(mh, filename, Config())
 
     if slp.is_external_harness:
         print("   > Ignored external harness")
         return
 
     n_container = slp.parse_file()
```

### Comparing `miss_hit-0.9.7/miss_hit/version.py` & `miss_hit-0.9.9/miss_hit/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 ##                                                                          ##
 ##############################################################################
 
 # Some constants we use for tool version and URLs
 
 GITHUB_ISSUES = "https://github.com/florianschanda/miss_hit/issues"
 
-VERSION_TUPLE = (0, 9, 7)
+VERSION_TUPLE = (0, 9, 9)
 VERSION_SUFFIX = ""
 
 VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
           ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "MISS_HIT %s" % VERSION
```

### Comparing `miss_hit-0.9.7/miss_hit/work_package.py` & `miss_hit-0.9.9/miss_hit/work_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ##  along with MISS_HIT. If not, see <http://www.gnu.org/licenses/>.        ##
 ##                                                                          ##
 ##############################################################################
 
 import os.path
 
 from miss_hit import s_ast
-from miss_hit import config_files
+from miss_hit import cfg_tree
 
 from miss_hit.errors import Message_Handler, ICE, Location
 
 
 class Work_Package:
     def __init__(self, filename, mh, options, extra_options):
         assert isinstance(filename, str)
@@ -48,15 +48,15 @@
 
 
 class SIMULINK_File_WP(Work_Package):
     # This is a SIMULINK model that will in turn spawn multiple
     # Embedded_MATLAB_WP instances.
     def __init__(self, filename, mh, options, extra_options):
         super().__init__(filename, mh, options, extra_options)
-        self.cfg = config_files.get_config(self.filename)
+        self.cfg = cfg_tree.get_config(self.filename)
 
     def write_modified(self, content):
         raise ICE("logic error - must not be called for SL File WP")
 
     def register_file(self):
         self.mh.register_file(self.filename)
 
@@ -87,15 +87,15 @@
     # MATLAB code that is in an m-file somewhere
     def __init__(self, filename,
                  encoding,
                  mh, options, extra_options):
         super().__init__(filename, None,
                          encoding,
                          mh, options, extra_options)
-        self.cfg = config_files.get_config(self.filename)
+        self.cfg = cfg_tree.get_config(self.filename)
 
     def write_modified(self, content):
         assert isinstance(content, str)
         self.modified = True
         with open(self.filename, "w", encoding=self.encoding) as fd:
             fd.write(content)
```

### Comparing `miss_hit-0.9.7/miss_hit.egg-info/PKG-INFO` & `miss_hit-0.9.9/miss_hit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss-hit
-Version: 0.9.7
+Version: 0.9.9
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://github.com/florianschanda/miss_hit
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
```

### Comparing `miss_hit-0.9.7/miss_hit.egg-info/SOURCES.txt` & `miss_hit-0.9.9/miss_hit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 setup.cfg
 setup.py
 miss_hit/__init__.py
+miss_hit/cfg_ast.py
+miss_hit/cfg_parser.py
+miss_hit/cfg_tree.py
 miss_hit/command_line.py
 miss_hit/config.py
-miss_hit/config_files.py
 miss_hit/errors.py
 miss_hit/g_cfg.py
 miss_hit/graph.py
 miss_hit/m_ast.py
 miss_hit/m_language.py
 miss_hit/m_language_builtins.py
 miss_hit/m_lexer.py
```

### Comparing `miss_hit-0.9.7/setup.py` & `miss_hit-0.9.9/setup.py`

 * *Files identical despite different names*

