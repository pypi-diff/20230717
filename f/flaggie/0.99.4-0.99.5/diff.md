# Comparing `tmp/flaggie-0.99.4.tar.gz` & `tmp/flaggie-0.99.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaggie-0.99.4.tar", last modified: Wed Apr 26 13:12:33 2023, max compression
+gzip compressed data, was "flaggie-0.99.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flaggie-0.99.4.tar` & `flaggie-0.99.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.4/COPYING
--rw-r--r--   0        0        0       84 2023-04-26 13:10:44.388852 flaggie-0.99.4/flaggie/__init__.py
--rw-r--r--   0        0        0    12830 2023-04-26 13:10:43.098826 flaggie-0.99.4/flaggie/__main__.py
--rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.4/flaggie/config.py
--rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.4/flaggie/mangle.py
--rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.4/flaggie/pm.py
--rw-r--r--   0        0        0     1118 2023-04-26 13:10:43.742172 flaggie-0.99.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 07:39:45.200537 flaggie-0.99.4/test/__init__.py
--rw-r--r--   0        0        0     4723 2023-01-15 07:39:45.200537 flaggie-0.99.4/test/test_config.py
--rw-r--r--   0        0        0     1845 2023-01-15 16:47:15.640493 flaggie-0.99.4/test/test_main.py
--rw-r--r--   0        0        0    16203 2023-01-20 19:03:53.062748 flaggie-0.99.4/test/test_mangle.py
--rw-r--r--   0        0        0     7205 2023-02-15 16:46:20.320855 flaggie-0.99.4/test/test_pm.py
--rw-r--r--   0        0        0      464 2023-01-15 07:39:45.200537 flaggie-0.99.4/tox.ini
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.5/COPYING
+-rw-r--r--   0        0        0       84 2023-07-17 09:37:59.888358 flaggie-0.99.5/flaggie/__init__.py
+-rw-r--r--   0        0        0    13202 2023-07-17 09:37:20.610998 flaggie-0.99.5/flaggie/__main__.py
+-rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.5/flaggie/config.py
+-rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.5/flaggie/mangle.py
+-rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.5/flaggie/pm.py
+-rw-r--r--   0        0        0     1118 2023-04-26 13:10:43.742172 flaggie-0.99.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 07:39:45.200537 flaggie-0.99.5/test/__init__.py
+-rw-r--r--   0        0        0     4723 2023-01-15 07:39:45.200537 flaggie-0.99.5/test/test_config.py
+-rw-r--r--   0        0        0     1845 2023-01-15 16:47:15.640493 flaggie-0.99.5/test/test_main.py
+-rw-r--r--   0        0        0    16203 2023-01-20 19:03:53.062748 flaggie-0.99.5/test/test_mangle.py
+-rw-r--r--   0        0        0     7205 2023-02-15 16:46:20.320855 flaggie-0.99.5/test/test_pm.py
+-rw-r--r--   0        0        0      464 2023-01-15 07:39:45.200537 flaggie-0.99.5/tox.ini
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.5/PKG-INFO
```

### Comparing `flaggie-0.99.4/COPYING` & `flaggie-0.99.5/COPYING`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/flaggie/__main__.py` & `flaggie-0.99.5/flaggie/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import sys
 import textwrap
 import typing
 
 from functools import partial
 from pathlib import Path
 
+from flaggie import __version__
 from flaggie.config import (TokenType, find_config_files, read_config_files,
                             save_config_files, ConfigFile,
                             )
 from flaggie.mangle import mangle_flag, remove_flag
 from flaggie.pm import (match_package, get_valid_values, split_use_expand,
                         MatchError,
                         )
@@ -190,14 +191,15 @@
 
     if shutil.which("git"):
         diff_default = "git --no-pager diff --no-index --word-diff --"
     else:
         diff_default = "diff -d -u --"
 
     argp = argparse.ArgumentParser(
+        add_help=False,
         prog=os.path.basename(prog_name),
         usage="%(prog)s [options] request ...",
         epilog=epilog,
         formatter_class=partial(argparse.RawDescriptionHelpFormatter,
                                 width=help_width),
         )
     argp.add_argument("--config-root",
@@ -212,27 +214,34 @@
                       default=diff_default,
                       help="Program used to diff configs "
                            f"(default: {diff_default})")
     argp.add_argument("--force",
                       action="store_true",
                       help="Force performing the action even if arguments "
                            "are invalid")
+    argp.add_argument("--help",
+                      action="help",
+                      help="Print help text and exit")
     argp.add_argument("--no-diff",
                       action="store_const",
                       const=None,
                       dest="diff",
                       help="Do not diff configs")
     argp.add_argument("--no-package-manager",
                       action="store_true",
                       help="Disable package manager interaction and features "
                            "requiring it (category and argument type "
                            "guessing, validation)")
     argp.add_argument("--pretend",
                       action="store_true",
                       help="Do not write any changes to the original files")
+    argp.add_argument("--version",
+                      action="version",
+                      help="Print program version and exit",
+                      version=f"flaggie {__version__}")
     args, request = argp.parse_known_args(argv)
 
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
     if not request:
         argp.error("No request specified")
```

### Comparing `flaggie-0.99.4/flaggie/config.py` & `flaggie-0.99.5/flaggie/config.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/flaggie/mangle.py` & `flaggie-0.99.5/flaggie/mangle.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/flaggie/pm.py` & `flaggie-0.99.5/flaggie/pm.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/pyproject.toml` & `flaggie-0.99.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/test/test_config.py` & `flaggie-0.99.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/test/test_main.py` & `flaggie-0.99.5/test/test_main.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/test/test_mangle.py` & `flaggie-0.99.5/test/test_mangle.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/test/test_pm.py` & `flaggie-0.99.5/test/test_pm.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.4/PKG-INFO` & `flaggie-0.99.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaggie
-Version: 0.99.4
+Version: 0.99.5
 Summary: CLI mangler for Portage package.* configuration files
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: more-itertools
 Requires-Dist: gentoopm >= 0.5 ; extra == "package-manager"
 Requires-Dist: rich ; extra == "pretty-log"
```

