# Comparing `tmp/kcfg-0.1.0.tar.gz` & `tmp/kcfg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcfg-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "kcfg-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kcfg-0.1.0.tar` & `kcfg-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     2699 2023-07-15 20:52:33.738840 kcfg-0.1.0/.gitignore
--rw-r--r--   0        0        0    35150 2023-07-15 20:51:52.218637 kcfg-0.1.0/LICENSE
--rw-r--r--   0        0        0      865 2023-07-15 21:35:18.591379 kcfg-0.1.0/README.md
--rw-r--r--   0        0        0       60 2023-07-17 12:27:59.779940 kcfg-0.1.0/TODO
--rwxr-xr-x   0        0        0    10786 2023-07-17 12:41:06.367915 kcfg-0.1.0/kcfg.py
--rw-r--r--   0        0        0      673 2023-07-17 12:46:27.107905 kcfg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1480 1970-01-01 00:00:00.000000 kcfg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-07-15 20:51:52.218637 kcfg-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1695 2023-07-17 13:46:11.187790 kcfg-0.1.1/README.md
+-rwxr-xr-x   0        0        0    10830 2023-07-17 15:08:55.059632 kcfg-0.1.1/kcfg.py
+-rw-r--r--   0        0        0      673 2023-07-17 12:46:27.107905 kcfg-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 kcfg-0.1.1/PKG-INFO
```

### Comparing `kcfg-0.1.0/LICENSE` & `kcfg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kcfg-0.1.0/kcfg.py` & `kcfg-0.1.1/kcfg.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #
 # It should not have any dependencies outside the ones provided by python by
 # default
 # --------------------------------------------------------------------------- #
 """Tool to read and write KDE INI config files, replaces kwriteconfig5 / kreadconfig5
 """
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import sys
 import os
 import configparser
 import argparse
 
 from typing import Tuple, List
@@ -231,15 +231,15 @@
     parser.add_argument('-l', '--list-configs', action=make_final_action(_print_configs), help='lists all known config files then quits')
 
     # positional
     parser.add_argument('path', help='path to use for read/write operation')
 
     args = parser.parse_args(raw_args)
 
-    if args.dry_run and not args.q:
+    if args.dry_run and not args.quiet:
         print("Dry run enabled")
 
     # parse the path
     path, file = _parse_path(args.path)
     file_from_path = True
 
     if file and args.file:
@@ -254,15 +254,15 @@
         file = args.file
         file_from_path = False
 
     # no file is provided so default it is
     if not file:
         file = DEFAULT_FILE
 
-        if not args.q:
+        if not args.quiet:
             print('No file specified, defaulting to kdeglobals')
 
     # only expand if file is specified inside the path
     if file_from_path:
         # lowercase cause some files are just weirdly cased
         file = file.lower()
         if file in PREDEFINED_FILES:
@@ -275,24 +275,24 @@
     key = path.pop()
     section = ']['.join(path)
 
     # the file may not exist
     try:
         data = _read_file(file)
     except FileNotFoundError:
-        data = []
+        data = {}
 
     from io import StringIO
 
     if args.delete:
-        if not args.q:
+        if not args.quiet:
             print(f"Deleting '{args.path}' in '{file}'")
 
         try:
-            if not args.q:
+            if not args.quiet:
                 print(f"Value was '{data[section][key]}'")
 
             del data[section][key]
         except KeyError:
             # exit as there is no need to write to file as either the section
             # or the key do not exist
             exit(0)
@@ -300,19 +300,19 @@
         if not args.dry_run:
             with open(file, 'w') as fp:
                 _write_file(fp, data)
         else:
             buffer = StringIO()
             _write_file(buffer, data)
             print(buffer.getvalue())
-    elif args.write:
-        if not args.q:
+    elif args.write is not None:
+        if not args.quiet:
             print(f"Setting '{args.path}' to '{args.write}' in '{file}'")
 
-            if not args.q:
+            if not args.quiet:
                 # TODO this may be too verbose? make a verbose flag?
                 try:
                     print(f"Value was '{data[section][key]}'")
                 except KeyError:
                     pass
 
             try:
@@ -326,24 +326,24 @@
                 _write_file(fp, data)
         else:
             buffer = StringIO()
             _write_file(buffer, data)
             print(buffer.getvalue())
     else:
         if not data:
-            if not args.q:
+            if not args.quiet:
                 print(f"File '{file}' is empty or does not exist")
 
             exit(0)
 
         try:
             print(data[section][key])
         except KeyError:
             # i am intentionally return with code 0 as it is not an error
-            if not args.q:
+            if not args.quiet:
                 print(f"Path '{args.path}' not found in '{file}'")
 
             exit(0)
 
 if __name__ == '__main__':
     main()
```

### Comparing `kcfg-0.1.0/pyproject.toml` & `kcfg-0.1.1/pyproject.toml`

 * *Files identical despite different names*

