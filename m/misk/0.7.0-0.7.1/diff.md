# Comparing `tmp/misk-0.7.0.tar.gz` & `tmp/misk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misk-0.7.0.tar", last modified: Mon Sep  5 20:23:32 2022, max compression
+gzip compressed data, was "misk-0.7.1.tar", last modified: Mon Jul 17 08:40:55 2023, max compression
```

## Comparing `misk-0.7.0.tar` & `misk-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-05 20:23:32.156205 misk-0.7.0/
--rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1429 2022-09-05 20:23:32.156205 misk-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-05 20:23:32.151195 misk-0.7.0/misk/
--rw-rw-rw-   0        0        0      331 2022-05-08 15:19:38.000000 misk-0.7.0/misk/__init__.py
--rw-rw-rw-   0        0        0    12346 2022-09-05 20:13:50.000000 misk-0.7.0/misk/functions.py
--rw-rw-rw-   0        0        0     1350 2022-05-08 14:12:21.000000 misk-0.7.0/misk/timers.py
-drwxrwxrwx   0        0        0        0 2022-09-05 20:23:32.155195 misk-0.7.0/misk.egg-info/
--rw-rw-rw-   0        0        0     1429 2022-09-05 20:23:31.000000 misk-0.7.0/misk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2022-09-05 20:23:32.000000 misk-0.7.0/misk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-05 20:23:31.000000 misk-0.7.0/misk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-05 20:23:31.000000 misk-0.7.0/misk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-09-05 20:23:31.000000 misk-0.7.0/misk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-05 20:23:32.156205 misk-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1524 2022-09-05 20:08:50.000000 misk-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.800930 misk-0.7.1/
+-rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1562 2023-07-17 08:40:55.800930 misk-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.795930 misk-0.7.1/misk/
+-rw-rw-rw-   0        0        0      331 2023-07-17 08:39:10.000000 misk-0.7.1/misk/__init__.py
+-rw-rw-rw-   0        0        0    12151 2023-07-17 08:39:03.000000 misk-0.7.1/misk/functions.py
+-rw-rw-rw-   0        0        0     1342 2023-07-17 08:39:06.000000 misk-0.7.1/misk/timers.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.799930 misk-0.7.1/misk.egg-info/
+-rw-rw-rw-   0        0        0     1562 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:40:55.800930 misk-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-07-17 08:39:12.000000 misk-0.7.1/setup.py
```

### Comparing `misk-0.7.0/LICENSE.txt` & `misk-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `misk-0.7.0/PKG-INFO` & `misk-0.7.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
 Project-URL: Tracker, https://github.com/marzer/misk/issues
 Keywords: utilities
 Platform: UNKNOWN
-Requires-Python: >=3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # misk
 Miscellaneous useful bits for python 3.
 
 ```
 pip install misk
 ```
 
+<br><br>
+## Changelog
 
-# Changelog
+## v0.7.1 - 2023-07-17
+
+-   Fixed `copy_file()` not following symlinks
 
 ## v0.7.0 - 2022-09-05
-- Added `none` filter to `enumerate_files()`
-- Added `tabify()`
-- Added `untabify()`
-- Added `reindent()`
+
+-   Added `none` filter to `enumerate_files()`
+-   Added `tabify()`
+-   Added `untabify()`
+-   Added `reindent()`
 
 ## v0.6.1 - 2022-08-13
-- Fixed typos in `print_exception()`
+
+-   Fixed typos in `print_exception()`
 
 ## v0.6.0 - 2022-05-08
-- Added `coerce_collection()`
-- Added `coerce_path()`
-- Added `enumerate_files()`
-- Added `enumerate_directories()`
-- Added `check` argument to `run_python_script()`
-- Added function return type annotations
+
+-   Added `coerce_collection()`
+-   Added `coerce_path()`
+-   Added `enumerate_files()`
+-   Added `enumerate_directories()`
+-   Added `check` argument to `run_python_script()`
+-   Added function return type annotations
 
 ## v0.5.0 - 2021-09-11
-- Added `replace_metavar()`
+
+-   Added `replace_metavar()`
 
 ## v0.4.0 - 2021-04-22
-- Fixed `get_all_files()` filtering on full paths instead of filenames only
-- Fixed `print_exception()` output missing a newline
+
+-   Fixed `get_all_files()` filtering on full paths instead of filenames only
+-   Fixed `print_exception()` output missing a newline
 
 ## v0.3.0 - 2021-04-20
-- Decoupled begin and end logger for `ScopeTimer`
+
+-   Decoupled begin and end logger for `ScopeTimer`
 
 ## v0.2.0 - 2021-04-18
-- Fixed incorrect boolean logic in `assert_existing_XXXXX()`
+
+-   Fixed incorrect boolean logic in `assert_existing_XXXXX()`
```

### Comparing `misk-0.7.0/misk/functions.py` & `misk-0.7.1/misk/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,87 @@
 #!/usr/bin/env python3
 # This file is a part of misk and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/misk/blob/master/LICENSE.txt for the full license text.
 # SPDX-License-Identifier: MIT
 
-import sys
-import shutil
 import fnmatch
-import requests
 import hashlib
-import logging
-import traceback
-import subprocess
 import io
-import re
+import logging
 import pathlib
+import re
+import shutil
+import subprocess
+import sys
+import traceback
 from pathlib import Path
 from typing import List, Union
 
-__all__ = []
+import requests
+
+__all__ = [
+	r'is_collection',
+	r'coerce_collection',
+	r'print_exception',
+	r'entry_script_dir',
+	r'coerce_path',
+	r'assert_existing_file',
+	r'assert_existing_directory',
+	r'delete_directory',
+	r'copy_file',
+	r'move_file',
+	r'delete_file',
+	r'enumerate_files',
+	r'get_all_files',
+	r'enumerate_directories',
+	r'read_all_text_from_file',
+	r'run_python_script',
+	r'sha1',
+	r'sha256',
+	r'is_pow2',
+	r'next_pow2',
+	r'replace_metavar',
+	r'tabify',
+	r'untabify',
+	r'reindent',
+]
 
 #=======================================================================================================================
 # shared lib state
 #=======================================================================================================================
 
+
+
 class _State(object):
 
 	def __init__(self):
 		self.entry_script_dir = Path(sys.argv[0]).resolve().parent
 		self.python = 'py' if shutil.which('py') is not None else 'python3'
 
 
 
 __state = None
+
+
+
 def _state() -> _State:
 	global __state
 	if __state is None:
 		__state = _State()
 	return __state
 
 
 
 #=======================================================================================================================
 # functions
 #=======================================================================================================================
 
+
+
 def _log(logger, msg, level=logging.INFO):
 	if logger is None or msg is None:
 		return
 	if isinstance(logger, bool):
 		if logger:
 			print(msg, file=sys.stderr if level >= logging.WARNING else sys.stdout)
 	elif isinstance(logger, logging.Logger):
@@ -56,43 +89,42 @@
 	elif isinstance(logger, io.IOBase):
 		print(msg, file=logger)
 	else:
 		logger(msg)
 
 
 
-__all__.append(r'is_collection')
 def is_collection(val) -> bool:
 	'''
 	Returns true if an object is an instance of one of the python built-in iterable collections.
 	'''
 	if isinstance(val, (list, tuple, dict, set, range)):
 		return True
 	return False
 
-__all__.append(r'coerce_collection')
+
+
 def coerce_collection(val) -> Union[list, tuple, dict, set, range]:
 	'''
 	Returns the input if it already satisfies is_collection(), otherwise returns the input boxed into a tuple.
 	'''
 	assert val is not None
 	if not is_collection(val):
-		val = ( val, )
+		val = (val, )
 	return val
 
 
 
-__all__.append(r'print_exception')
 def print_exception(exc, logger=sys.stderr, include_type=False, include_traceback=False, skip_frames=0):
 	'''
 	Pretty-prints an exception with optional traceback.
 	'''
 	if isinstance(exc, (AssertionError, NameError, TypeError)):
-		include_type=True
-		include_traceback=True
+		include_type = True
+		include_traceback = True
 	with io.StringIO() as buf:
 		if include_traceback:
 			tb = exc.__traceback__
 			while skip_frames > 0 and tb.tb_next is not None:
 				skip_frames = skip_frames - 1
 				tb = tb.tb_next
 			traceback.print_exception(type(exc), exc, tb, file=buf)
@@ -101,115 +133,108 @@
 			if include_type:
 				print(rf'[{type(exc).__name__}] ', file=buf, end='')
 			print(str(exc), file=buf, end='')
 		_log(logger, buf.getvalue(), level=logging.ERROR)
 
 
 
-__all__.append(r'entry_script_dir')
 def entry_script_dir() -> pathlib.Path:
 	'''
 	Returns a pathlib.Path representing the directory of the script used to enter the python process.
 	'''
 	return _state().entry_script_dir
 
 
 
-__all__.append(r'coerce_path')
 def coerce_path(arg, *args) -> pathlib.Path:
 	'''
 	Buildes path from one or more inputs.
 	'''
 	assert arg is not None
 	if args is not None and len(args):
 		return Path(str(arg), *[str(a) for a in args])
 	else:
 		if not isinstance(arg, Path):
 			arg = Path(str(arg))
 		return arg
 
 
 
-__all__.append(r'assert_existing_file')
 def assert_existing_file(path):
 	'''
 	Asserts that a path represents an existing file on disk.
 	'''
 	path = coerce_path(path)
 	if not path.exists() or not path.is_file():
 		raise Exception(rf'{path} did not exist or was not a file')
 
 
 
-__all__.append(r'assert_existing_directory')
 def assert_existing_directory(path):
 	'''
 	Asserts that a path represents an existing directory on disk.
 	'''
 	path = coerce_path(path)
 	if not path.exists() or not path.is_dir():
 		raise Exception(f'{path} did not exist or was not a directory')
 
 
 
-__all__.append(r'delete_directory')
 def delete_directory(path, logger=None):
 	'''
 	Deletes a directory (and all its contents).
 	'''
 	path = coerce_path(path)
 	if path.exists():
 		if not path.is_dir():
 			raise Exception(rf'{path} was not a directory')
 		_log(logger, rf'Deleting {path}')
 		shutil.rmtree(str(path.resolve()))
 
 
 
-__all__.append(r'copy_file')
 def copy_file(source, dest, logger=None):
 	'''
 	Copies a single file.
 	'''
 	source = coerce_path(source)
 	dest = coerce_path(dest)
 	assert_existing_file(source)
 	_log(logger, rf'Copying {source} to {dest}')
-	shutil.copy(str(source), str(dest))
+	shutil.copy(str(source), str(dest), follow_symlinks=True)
+	if (source.is_file() and dest.is_file()):
+		shutil.copymode(str(source), str(dest), follow_symlinks=True)
 
 
 
-__all__.append(r'move_file')
 def move_file(source, dest, logger=None):
 	'''
 	Moves a single file.
 	'''
 	source = coerce_path(source)
 	dest = coerce_path(dest)
 	assert_existing_file(source)
 	_log(logger, rf'Moving {source} to {dest}')
 	shutil.move(str(source), str(dest))
 
 
 
-__all__.append(r'delete_file')
 def delete_file(path, logger=None):
 	'''
 	Deletes a single file.
 	'''
 	path = coerce_path(path)
 	if path.exists():
 		if not path.is_file():
 			raise Exception(rf'{path} was not a file')
 		_log(logger, rf'Deleting {path}')
 		path.unlink()
 
 
 
-__all__.append(r'enumerate_files')
 def enumerate_files(root, all=None, any=None, none=None, recursive=False, sort=True) -> List[pathlib.Path]:
 	'''
 	Collects all files in a directory matching some filename filters.
 	'''
 	root = coerce_path(root)
 	if not root.exists():
 		return []
@@ -255,21 +280,19 @@
 	files = [Path(root, f) for f in files] + child_files
 	if sort:
 		files.sort()
 	return files
 
 
 
-__all__.append(r'get_all_files')
-def get_all_files(path, all=None, any=None, recursive=False, sort=True)-> List[pathlib.Path]:
+def get_all_files(path, all=None, any=None, recursive=False, sort=True) -> List[pathlib.Path]:
 	return enumerate_files(path, all=all, any=any, recursive=recursive, sort=sort)
 
 
 
-__all__.append(r'enumerate_directories')
 def enumerate_directories(root, filter=None, recursive=False, sort=True) -> List[pathlib.Path]:
 	'''
 	Collects all subdirectories in a directory.
 	'''
 	root = coerce_path(root)
 	if not root.exists():
 		return []
@@ -286,15 +309,14 @@
 				subdirs = subdirs + enumerate_directories(p, filter=filter, recursive=True, sort=False)
 	if sort:
 		subdirs.sort()
 	return subdirs
 
 
 
-__all__.append(r'read_all_text_from_file')
 def read_all_text_from_file(path, fallback_url=None, encoding='utf-8', logger=None) -> str:
 	'''
 	Reads all the text from a file, optionally downloading it if the file did not exist on disk or a read error occured.
 	'''
 	path = coerce_path(path)
 	if fallback_url is None:
 		assert_existing_file(path)
@@ -302,42 +324,36 @@
 		_log(logger, rf'Reading {path}')
 		with open(path, 'r', encoding=encoding) as f:
 			text = f.read()
 		return text
 	except:
 		if fallback_url is not None:
 			_log(logger, rf"Couldn't read file locally, downloading from {fallback_url}")
-			response = requests.get(
-				fallback_url,
-				timeout=1
-			)
+			response = requests.get(fallback_url, timeout=1)
 			text = response.text
 			with open(path, 'w', encoding='utf-8', newline='\n') as f:
 				f.write(text)
 			return text
 		else:
 			raise
 
 
 
-__all__.append(r'run_python_script')
 def run_python_script(path, *args, cwd=None, check=True, **kwargs) -> subprocess.CompletedProcess:
 	'''
 	Invokes a python script as a subprocess.
 	'''
 	path = coerce_path(path)
 	if not path.exists():
 		raise Exception(rf'{path} was not an existing directory or file')
 
-	return subprocess.run(
-		[_state().python, str(path)] + [arg for arg in args],
+	return subprocess.run([_state().python, str(path)] + [arg for arg in args],
 		check=check,
 		cwd=path.cwd() if cwd is None else cwd,
-		**kwargs
-	)
+		**kwargs)
 
 
 
 def _do_hash(hasher, obj, *objs) -> str:
 	assert obj is not None
 	append = lambda o: hasher.update(str(o).encode('utf-8'))
 	append(obj)
@@ -345,43 +361,39 @@
 		for o in objs:
 			assert o is not None
 			append(o)
 	return hasher.hexdigest()
 
 
 
-__all__.append(r'sha1')
 def sha1(obj, *objs) -> str:
 	'''
 	Returns an SHA-1 hash of one or more objects.
 	'''
 	return _do_hash(hashlib.sha1(), obj, *objs)
 
 
 
-__all__.append(r'sha256')
 def sha256(obj, *objs) -> str:
 	'''
 	Returns an SHA-256 hash of one or more objects.
 	'''
 	return _do_hash(hashlib.sha256(), obj, *objs)
 
 
 
-__all__.append(r'is_pow2')
 def is_pow2(n) -> bool:
 	'''
 	Returns true if a positive integer is a power of two.
 	'''
 	n = int(n)
 	return n and (n & (n - 1) == 0)
 
 
 
-__all__.append(r'next_pow2')
 def next_pow2(n) -> int:
 	'''
 	Rounds an integer up to the next positive power of two.
 	'''
 	n = int(n)
 	if n <= 0:
 		return 1
@@ -389,15 +401,14 @@
 		return n
 	while n & (n - 1) > 0:
 		n &= (n - 1)
 	return n << 1
 
 
 
-__all__.append(r'replace_metavar')
 def replace_metavar(name, repl, text) -> str:
 	'''
 	Replaces named meta variables in strings. Meta variables can be in any of the following formats:
 	   - {% name %}
 	   - $( name )
 	   - %( name )
 
@@ -428,76 +439,75 @@
 
 
 def _tabify_replace_range(s, start, length, replacement) -> str:
 	assert isinstance(s, str)
 	assert isinstance(replacement, str)
 	assert start >= 0
 	assert length > 0
-	assert start+length <= len(s)
+	assert start + length <= len(s)
 	return rf'{s[:start]}{replacement}{s[start+length:]}'
 
+
+
 def _tabify_count_preceeding_spaces(s, start, tab_width) -> str:
 	spaces = 0
 	for i in range(tab_width):
-		if s[start-i-1] != ' ':
+		if s[start - i - 1] != ' ':
 			break
 		spaces += 1
 	return spaces
 
 
 
-__all__.append(r'tabify')
 def tabify(s, tab_width=4) -> str:
 	'''
 	Replaces spaces with tabs.
 	'''
 	if not isinstance(s, str):
 		s = str(s)
 	i = (len(s) - (len(s) % tab_width)) - tab_width
 	while i >= 0:
-		spaces = _tabify_count_preceeding_spaces(s, i+tab_width, tab_width)
+		spaces = _tabify_count_preceeding_spaces(s, i + tab_width, tab_width)
 		if spaces > 1:
-			s = _tabify_replace_range(s, i+(tab_width-spaces), spaces, '\t')
+			s = _tabify_replace_range(s, i + (tab_width - spaces), spaces, '\t')
 		i -= tab_width
 	return s
 
 
 
-__all__.append(r'untabify')
 def untabify(s, tab_width=4) -> str:
 	'''
 	Replaces tabs with spaces.
 	'''
 	if not isinstance(s, str):
 		s = str(s)
 	i = s.find('\t')
 	while i != -1:
 		spaces = tab_width - (i % tab_width)
-		s = _tabify_replace_range(s, i, 1, ' '*spaces)
+		s = _tabify_replace_range(s, i, 1, ' ' * spaces)
 		i = s.find('\t', i + spaces - 1)
 	return s
 
 
 
-__all__.append(r'reindent')
 def reindent(s, indent='\t', tab_width=4) -> str:
 	'''
 	Re-indents a block of text.
 	'''
 	if not isinstance(s, str):
 		s = str(s)
 
 	if not isinstance(indent, str):
 		indent = str(indent)
 	indent = untabify(indent, tab_width=tab_width)
 
 	lstrip = 9999999999999999
 	s = [untabify(ss, tab_width) for ss in s.splitlines()]
 	for i in range(len(s)):
-		stripped = s[i].lstrip();
+		stripped = s[i].lstrip()
 		if not stripped:
 			s[i] = ''
 			continue
 		lstrip = min(len(s[i]) - len(stripped), lstrip)
 
 	for i in range(len(s)):
 		if s[i]:
```

### Comparing `misk-0.7.0/misk/timers.py` & `misk-0.7.1/misk/timers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/env python3
 # This file is a part of misk and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/misk/blob/master/LICENSE.txt for the full license text.
 # SPDX-License-Identifier: MIT
 
 import time
-from . import functions as fn
 from datetime import timedelta
 
-__all__ = []
+from . import functions as fn
+
+__all__ = [r'ScopeTimer']
 
 
 
-__all__.append(r'ScopeTimer')
 class ScopeTimer(object):
+
 	'''
 	A utility class for scoped timing blocks of code using python's "with" keyword.
 	'''
 
 	def __init__(self, description, print_start=False, print_end=print):
 		self.__description = str(description)
 		self.__print_start = print_start
 		self.__print_end = print_end
 
 	def __enter__(self):
 		self.__start = time.perf_counter_ns()
 		if self.__print_start is not None and (not isinstance(self.__print_start, bool) or self.__print_start):
 			fn._log(self.__print_start, self.__description)
 
-	def __exit__(self ,type, value, traceback):
-		if traceback is not None or self.__print_end is None or (isinstance(self.__print_end, bool) and not self.__print_end):
+	def __exit__(self, type, value, traceback):
+		if traceback is not None or self.__print_end is None or (
+			isinstance(self.__print_end, bool) and not self.__print_end
+		):
 			return
 		nanos = time.perf_counter_ns() - self.__start
 		micros = int(nanos / 1000)
 		nanos = int(nanos % 1000)
 		micros = float(micros) + float(nanos) / 1000.0
 		fn._log(self.__print_end, rf'{self.__description} completed in {timedelta(microseconds=micros)}.')
```

### Comparing `misk-0.7.0/misk.egg-info/PKG-INFO` & `misk-0.7.1/misk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
 Project-URL: Tracker, https://github.com/marzer/misk/issues
 Keywords: utilities
 Platform: UNKNOWN
-Requires-Python: >=3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # misk
 Miscellaneous useful bits for python 3.
 
 ```
 pip install misk
 ```
 
+<br><br>
+## Changelog
 
-# Changelog
+## v0.7.1 - 2023-07-17
+
+-   Fixed `copy_file()` not following symlinks
 
 ## v0.7.0 - 2022-09-05
-- Added `none` filter to `enumerate_files()`
-- Added `tabify()`
-- Added `untabify()`
-- Added `reindent()`
+
+-   Added `none` filter to `enumerate_files()`
+-   Added `tabify()`
+-   Added `untabify()`
+-   Added `reindent()`
 
 ## v0.6.1 - 2022-08-13
-- Fixed typos in `print_exception()`
+
+-   Fixed typos in `print_exception()`
 
 ## v0.6.0 - 2022-05-08
-- Added `coerce_collection()`
-- Added `coerce_path()`
-- Added `enumerate_files()`
-- Added `enumerate_directories()`
-- Added `check` argument to `run_python_script()`
-- Added function return type annotations
+
+-   Added `coerce_collection()`
+-   Added `coerce_path()`
+-   Added `enumerate_files()`
+-   Added `enumerate_directories()`
+-   Added `check` argument to `run_python_script()`
+-   Added function return type annotations
 
 ## v0.5.0 - 2021-09-11
-- Added `replace_metavar()`
+
+-   Added `replace_metavar()`
 
 ## v0.4.0 - 2021-04-22
-- Fixed `get_all_files()` filtering on full paths instead of filenames only
-- Fixed `print_exception()` output missing a newline
+
+-   Fixed `get_all_files()` filtering on full paths instead of filenames only
+-   Fixed `print_exception()` output missing a newline
 
 ## v0.3.0 - 2021-04-20
-- Decoupled begin and end logger for `ScopeTimer`
+
+-   Decoupled begin and end logger for `ScopeTimer`
 
 ## v0.2.0 - 2021-04-18
-- Fixed incorrect boolean logic in `assert_existing_XXXXX()`
+
+-   Fixed incorrect boolean logic in `assert_existing_XXXXX()`
```

### Comparing `misk-0.7.0/setup.py` & `misk-0.7.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 # See https://github.com/marzer/misk/blob/master/LICENSE.txt for the full license text.
 # SPDX-License-Identifier: MIT
 
 # set up based on this: https://thucnc.medium.com/how-to-publish-your-own-python-package-to-pypi-4318868210f9
 # windows:
 # py setup.py sdist bdist_wheel && twine upload dist/* && rmdir /S /Q dist
 
-from setuptools import setup, find_packages
+import re
+
+from setuptools import find_packages, setup
 
 README = ''
-with open('README.md', encoding='utf-8') as file:
+with open(r'README.md', encoding=r'utf-8') as file:
 	README = file.read()
 
 CHANGELOG = ''
-with open('CHANGELOG.md', encoding='utf-8') as file:
-	CHANGELOG = file.read().strip()
-
-setup_args = dict(
-	name=r'misk',
-	version=r'0.7.0',
-	description=r'Miscellaneous useful bits for python 3.',
-	long_description_content_type=r'text/markdown',
-	long_description=f'{README}\n\n{CHANGELOG}'.strip(),
-	license=r'MIT',
-	packages=find_packages(),
-	author=r'Mark Gillard',
-	author_email=r'mark.gillard@outlook.com.au',
-	keywords=['utilities'], # ???
-	url=r'https://github.com/marzer/misk',
-	download_url=r'https://pypi.org/project/misk/',
-	project_urls={
-		r'Source': r'https://github.com/marzer/misk',
-		r'Tracker': r'https://github.com/marzer/misk/issues'
+with open(r'CHANGELOG.md', encoding=r'utf-8') as file:
+	CHANGELOG = f'\n\n{file.read()}\n\n'
+CHANGELOG = re.sub(r'\n#+\s*Changelog\s*?\n', '\n## Changelog\n', CHANGELOG, flags=re.I).strip()
+
+SETUP_ARGS = {
+	r'name': r'misk',
+	r'version': r'0.7.1',
+	r'description': r'Miscellaneous useful bits for python 3.',
+	r'long_description_content_type': r'text/markdown',
+	r'long_description': f'{README}\n<br><br>\n{CHANGELOG}'.strip(),
+	r'license': r'MIT',
+	r'packages': find_packages(),
+	r'author': r'Mark Gillard',
+	r'author_email': r'mark.gillard@outlook.com.au',
+	r'keywords': ['utilities'],  # ???
+	r'url': r'https://github.com/marzer/misk',
+	r'download_url': r'https://pypi.org/project/misk/',
+	r'project_urls': {
+	r'Source': r'https://github.com/marzer/misk',
+	r'Tracker': r'https://github.com/marzer/misk/issues'
 	},
-	python_requires=r'>=3'
-)
+	r'python_requires': r'>=3.7'
+}
 
-install_requires = None
-with open('requirements.txt', encoding='utf-8') as file:
-	install_requires = file.read().strip().split()
+REQUIRES = None
+with open(r'requirements.txt', encoding='utf-8') as file:
+	REQUIRES = file.read().strip().split()
 
 if __name__ == '__main__':
-	setup(**setup_args, install_requires=install_requires)
+	setup(**SETUP_ARGS, install_requires=REQUIRES)
```

