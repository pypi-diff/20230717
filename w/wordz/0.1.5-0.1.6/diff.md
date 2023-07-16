# Comparing `tmp/wordz-0.1.5.tar.gz` & `tmp/wordz-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordz-0.1.5.tar", last modified: Sun Jan 15 22:41:07 2023, max compression
+gzip compressed data, was "wordz-0.1.6.tar", last modified: Sun Jul 16 22:30:56 2023, max compression
```

## Comparing `wordz-0.1.5.tar` & `wordz-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-01-15 22:41:07.398630 wordz-0.1.5/
--rw-r--r--   0 robert     (501) staff       (20)     1516 2022-07-14 16:02:29.000000 wordz-0.1.5/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     4980 2023-01-15 22:41:07.398279 wordz-0.1.5/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     4419 2023-01-15 22:40:36.000000 wordz-0.1.5/README.md
--rw-r--r--   0 robert     (501) staff       (20)       38 2023-01-15 22:41:07.398746 wordz-0.1.5/setup.cfg
--rwxr-xr-x   0 robert     (501) staff       (20)     1249 2023-01-12 20:25:50.000000 wordz-0.1.5/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-01-15 22:41:07.388189 wordz-0.1.5/src/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-01-15 22:41:07.394275 wordz-0.1.5/src/wordz/
--rw-r--r--   0 robert     (501) staff       (20)       71 2022-07-15 00:51:31.000000 wordz-0.1.5/src/wordz/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    10865 2023-01-15 22:40:36.000000 wordz-0.1.5/src/wordz/base.py
--rw-r--r--   0 robert     (501) staff       (20)     3239 2023-01-15 21:54:28.000000 wordz-0.1.5/src/wordz/cli.py
--rw-r--r--   0 robert     (501) staff       (20)      431 2022-07-15 11:16:47.000000 wordz-0.1.5/src/wordz/logs.py
--rw-r--r--   0 robert     (501) staff       (20)       62 2023-01-15 22:40:36.000000 wordz-0.1.5/src/wordz/version.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-01-15 22:41:07.397690 wordz-0.1.5/src/wordz.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     4980 2023-01-15 22:41:07.000000 wordz-0.1.5/src/wordz.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      322 2023-01-15 22:41:07.000000 wordz-0.1.5/src/wordz.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2023-01-15 22:41:07.000000 wordz-0.1.5/src/wordz.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       41 2023-01-15 22:41:07.000000 wordz-0.1.5/src/wordz.egg-info/entry_points.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2022-07-14 18:05:20.000000 wordz-0.1.5/src/wordz.egg-info/not-zip-safe
--rw-r--r--   0 robert     (501) staff       (20)        6 2023-01-15 22:41:07.000000 wordz-0.1.5/src/wordz.egg-info/top_level.txt
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.173904 wordz-0.1.6/
+-rw-r--r--   0 robert     (501) staff       (20)     1516 2023-07-05 10:00:48.000000 wordz-0.1.6/LICENSE
+-rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-16 22:30:56.173585 wordz-0.1.6/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     4419 2023-07-05 10:00:49.000000 wordz-0.1.6/README.md
+-rw-r--r--   0 robert     (501) staff       (20)       38 2023-07-16 22:30:56.174000 wordz-0.1.6/setup.cfg
+-rwxr-xr--   0 robert     (501) staff       (20)     1249 2023-05-09 10:42:42.000000 wordz-0.1.6/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.162684 wordz-0.1.6/src/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.168215 wordz-0.1.6/src/wordz/
+-rw-r--r--   0 robert     (501) staff       (20)       71 2023-07-05 10:00:49.000000 wordz-0.1.6/src/wordz/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    11000 2023-07-16 22:20:12.000000 wordz-0.1.6/src/wordz/base.py
+-rw-r--r--   0 robert     (501) staff       (20)     3222 2023-07-16 22:20:13.000000 wordz-0.1.6/src/wordz/cli.py
+-rw-r--r--   0 robert     (501) staff       (20)      431 2023-07-05 10:00:50.000000 wordz-0.1.6/src/wordz/logs.py
+-rw-r--r--   0 robert     (501) staff       (20)       62 2023-07-05 10:00:50.000000 wordz-0.1.6/src/wordz/version.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.171140 wordz-0.1.6/src/wordz.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      365 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       41 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/entry_points.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-16 22:21:33.000000 wordz-0.1.6/src/wordz.egg-info/not-zip-safe
+-rw-r--r--   0 robert     (501) staff       (20)        6 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/top_level.txt
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.172666 wordz-0.1.6/tests/
+-rw-r--r--   0 robert     (501) staff       (20)     2577 2023-07-05 10:00:58.000000 wordz-0.1.6/tests/test_cli.py
+-rw-r--r--   0 robert     (501) staff       (20)     3369 2023-07-16 12:28:58.000000 wordz-0.1.6/tests/test_combinator.py
```

### Comparing `wordz-0.1.5/LICENSE` & `wordz-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wordz-0.1.5/PKG-INFO` & `wordz-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordz
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wordlists builder
 Home-page: https://github.com/tasooshi/wordz
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: BSD License
 Keywords: wordlists,bruteforce,dictionary,generator,hashcat
 Classifier: Development Status :: 4 - Beta
```

### Comparing `wordz-0.1.5/README.md` & `wordz-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wordz-0.1.5/setup.py` & `wordz-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `wordz-0.1.5/src/wordz/base.py` & `wordz-0.1.6/src/wordz/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import datetime
 import functools
 import hashlib
 import os
 import pathlib
 import shutil
 import subprocess
-import sys
 import uuid
 
 from wordz import logs
 
 
 os.environ['LC_ALL'] = 'C'
 
@@ -19,42 +18,42 @@
 
     wordlists = None
     rules = None
 
     LEFT = 1
     BOTH = 2
     RIGHT = 3
+    DEFAULT_EXT = '.txt'
 
     def __init__(self, base_dir, temp_dir, output_dir, min_length, cores, memory, bin_hashcat, bin_combinator, bin_rli2):
         self.checks_ok = True
         if not pathlib.Path.exists(pathlib.Path(temp_dir)):
             logs.logger.error(f'Temporary directory `{temp_dir}` does not exist!')
             self.checks_ok = False
         self.base_dir = base_dir
         self.temp_dir = pathlib.Path(temp_dir).absolute()
         self.output_dir = pathlib.Path(output_dir).absolute()
         self.min_length = min_length
         self.cores = cores
         self.memory = memory
         self.compress_program = '--compress-program=lzop' if shutil.which('lzop') else ''
-        self.sort_snippet = f'sort -f -T {self.temp_dir} {self.compress_program} --parallel={cores} -S {memory}'
+        self.sort_snippet = f'sort -T {self.temp_dir} {self.compress_program} --parallel={cores} -S {memory}'
         self.bin_hashcat = bin_hashcat
         self.bin_combinator = bin_combinator
         self.bin_rli2 = bin_rli2
         self.check_which(self.bin_hashcat)
         self.check_which(self.bin_combinator)
         self.check_which(self.bin_rli2)
         output = subprocess.run('comm --nocheck-order', shell=True, capture_output=True).stderr
         if b'illegal option' in output:
             self.comm_ver = 'comm'
         else:
             self.comm_ver = 'comm --nocheck-order'
         if not self.checks_ok:
             raise Exception('Failed on startup')
-            sys.exit(1)
 
     def check_which(self, name):
         if not shutil.which(pathlib.Path(name)):
             logs.logger.error(f'Binary `{name}` not found - consider adding it to $PATH environment variable')
             self.checks_ok = False
 
     def exist(self, *paths):
@@ -81,30 +80,31 @@
                 with concurrent.futures.ThreadPoolExecutor() as executor:
                     for wordlist in self.wordlists:
                         executor.submit(self.rule, pathlib.Path(self.base_dir, wordlist), pathlib.Path(self.base_dir, rule))
 
     def rule(self, wordlist, rule, dest_dir=None):
         if dest_dir is None:
             dest_dir = self.temp_dir
-        filename = f'{rule.stem}-{wordlist.parts[-2]}-{wordlist.stem}.txt'
-        if not pathlib.Path(dest_dir, filename).is_file():
+        filename = f'{rule.stem}-{wordlist.parts[-2]}-{wordlist.stem}{self.DEFAULT_EXT}'
+        destination = pathlib.Path(dest_dir, filename)
+        if not destination.is_file():
             logs.logger.info(f'Processing `{wordlist}` with rule `{rule}`')
-            self.run_shell(f'{self.bin_hashcat} --stdout --session={uuid.uuid4()} -r {rule} {wordlist} | {self.sort_snippet} | uniq > {dest_dir}/{filename}')
-        return pathlib.Path(f'{dest_dir}/{filename}')
+            self.run_shell(f'{self.bin_hashcat} --stdout --session={uuid.uuid4()} -r {rule} {wordlist} | {self.sort_snippet} | uniq > {destination}')
+        return destination
 
     def sort(self, source, output=None, unique=False):
         cmd = f'{self.sort_snippet} {source}'
         if unique:
             cmd += ' -u'
         if output is None:
-            tmp_output = self.temp(source.stem + '-sort-tmp-replace.txt')
-            cmd += f' -o {tmp_output}'
+            output = self.temp(source.stem + '-sort-tmp-replace' + self.DEFAULT_EXT)
+            cmd += f' -o {output}'
             self.run_shell(cmd)
             self.delete(source)
-            self.move(tmp_output, source)
+            self.move(output, source)
         else:
             cmd += f' -o {output}'
             self.run_shell(cmd)
 
     def copy(self, source, destination):
         logs.logger.debug(f'Copying `{source}` to {destination}')
         self.ensure_path(destination)
@@ -156,62 +156,57 @@
     def left(self, left, right):
         return self.combine(self.LEFT, left, right)
 
     @functools.cache
     def both(self, left, right):
         return self.combine(self.BOTH, left, right)
 
-    def combine(self, method, left, right, destination=None):
-        if destination is None:
-            destination = self.temp_dir
-        self.ensure_path(destination)
+    def combine(self, method, left, right):
         if self.exist(left, right):
-            name = None
             if method is self.RIGHT:
-                name = f'{left.stem}+{right.stem}'
-                if not pathlib.Path(destination, name + '.txt').is_file():
+                destination = pathlib.Path(self.temp_dir, f'{left.stem}+{right.stem}{self.DEFAULT_EXT}')
+                if not destination.is_file():
                     logs.logger.info(f'Combining `{left.stem}` with `{right.stem}`')
-                    self.run_shell(f'{self.bin_combinator} {left} {right} > {destination}/{name}.txt')
+                    self.run_shell(f'{self.bin_combinator} {left} {right} > {destination}')
             elif method is self.LEFT:
-                name = f'{right.stem}+{left.stem}'
-                if not pathlib.Path(destination, name + '.txt').is_file():
+                destination = pathlib.Path(self.temp_dir, f'{right.stem}+{left.stem}{self.DEFAULT_EXT}')
+                if not destination.is_file():
                     logs.logger.info(f'Combining `{right.stem}` with `{left.stem}`')
-                    self.run_shell(f'{self.bin_combinator} {right} {left} > {destination}/{name}.txt')
+                    self.run_shell(f'{self.bin_combinator} {right} {left} > {destination}')
             elif method is self.BOTH:
-                name = f'{right.stem}+{left.stem}+{right.stem}'
-                if not pathlib.Path(destination, f'{right.stem}+{left.stem}' + '.txt').is_file():
-                    self.run_shell(f'{self.bin_combinator} {right} {left} > {destination}/{right.stem}+{left.stem}.txt')
-                if not pathlib.Path(destination, name + '.txt').is_file():
+                if not pathlib.Path(self.temp_dir, f'{right.stem}+{left.stem}{self.DEFAULT_EXT}').is_file():
+                    self.run_shell(f'{self.bin_combinator} {right} {left} > {self.temp_dir}/{right.stem}+{left.stem}{self.DEFAULT_EXT}')
+                destination = pathlib.Path(self.temp_dir, f'{right.stem}+{left.stem}+{right.stem}{self.DEFAULT_EXT}')
+                if not destination.is_file():
                     logs.logger.info(f'Combining `{left.stem}` with `{right.stem}`')
-                    self.run_shell(f'{self.bin_combinator} {destination}/{right.stem}+{left.stem}.txt {right} > {destination}/{name}.txt')
+                    self.run_shell(f'{self.bin_combinator} {self.temp_dir}/{right.stem}+{left.stem}{self.DEFAULT_EXT} {right} > {destination}')
             else:
                 raise NotImplementedError
-            logs.logger.info(f'Combined `{name}`')
-            return pathlib.Path(destination, name + '.txt')
-
+            logs.logger.info(f'Combined `{destination}`')
+            return destination
 
     def merge(self, destination, wordlists, compare=None):
         logs.logger.info(f'Merging: {destination}')
         self.ensure_path(destination)
         wordlists = [words for words in wordlists if words is not None]
         for wordlist in wordlists:
             if wordlist.stat().st_size == 0:
                 raise Exception(f'Wordlist {wordlist} is empty, something is not right. Aborting')
         self.delete(destination)
         job_id = hashlib.md5(str(destination).encode('ASCII')).hexdigest()
         trimmed = list()
         with concurrent.futures.ThreadPoolExecutor() as executor:
             for wordlist in wordlists:
-                trimmed_temp = self.temp(job_id + '-trimmed-' + wordlist.name)
+                trimmed_temp = self.temp(job_id + '-trimmed-' + wordlist.name + self.DEFAULT_EXT)
                 trimmed.append(trimmed_temp)
                 executor.submit(self.run_shell, f'awk "length >= {self.min_length}" {wordlist} > {trimmed_temp}')
         trimmed_joined = ' '.join([str(path) for path in trimmed])
         sort_cmd = f'cat {trimmed_joined} | {self.sort_snippet} | uniq > '
         if compare:
-            output_temp = self.temp(destination.stem + '.txt')
+            output_temp = self.temp(destination.stem + self.DEFAULT_EXT)
             self.run_shell(f'{sort_cmd} {output_temp}')
             self.run_shell(f'{self.bin_rli2} {output_temp} {compare} >> {destination}')
             self.append(destination, compare)
             self.sort(compare)
         else:
             self.run_shell(f'{sort_cmd} {destination}')
         # NOTE: Case when temporary files are really not needed.
@@ -221,19 +216,19 @@
         logs.logger.debug(f'Concatenating: {destination}')
         self.delete(destination)
         self.ensure_path(destination)
         for wordlist in wordlists:
             self.append(wordlist, destination)
 
     def diff(self, path, list_prefix, left='basic', right='extended', output='all'):
-        left_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{left}.txt')
-        right_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{right}.txt')
-        output_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{output}.txt')
-        left_temp = self.temp(f'{list_prefix}-diff-{left}.txt')
-        right_temp = self.temp(f'{list_prefix}-diff-{right}.txt')
+        left_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{left}{self.DEFAULT_EXT}')
+        right_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{right}{self.DEFAULT_EXT}')
+        output_fil = pathlib.Path(self.base_dir, path, f'{list_prefix}-{output}{self.DEFAULT_EXT}')
+        left_temp = self.temp(f'{list_prefix}-diff-{left}{self.DEFAULT_EXT}')
+        right_temp = self.temp(f'{list_prefix}-diff-{right}{self.DEFAULT_EXT}')
         self.sort(left_fil, left_temp)
         self.sort(right_fil, right_temp)
         self.compare(left_temp, right_temp, right_fil)
         self.delete(left_fil)
         self.move(left_temp, left_fil)
         self.concat(output_fil, [left_fil, right_fil])
         self.sort(output_fil)
@@ -247,13 +242,14 @@
         logs.logger.info(f'Using {self.cores} cores')
         logs.logger.info(f'Using {self.memory} of memory')
         self.setup()
         self.process()
         time_total = datetime.datetime.now() - time_start
         logs.logger.info(f'Total time: {time_total}')
         logs.logger.info(f'Done! You may want to clean up the temporary directory yourself: {self.temp_dir}')
+        logs.logger.info(f'Make sure to remove the temporary files used for comparing if you plan to re-run the process.')
 
     def setup(self):
         self.wordlists_process()
 
     def process(self):
         raise NotImplementedError()
```

### Comparing `wordz-0.1.5/src/wordz/cli.py` & `wordz-0.1.6/src/wordz/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import importlib.util
 import multiprocessing
 import pathlib
 import sys
-import tempfile
 
 from wordz import (
     logs,
     version,
 )
 
 
@@ -22,14 +21,15 @@
     try:
         cls = getattr(module, class_name)
     except AttributeError:
         raise Exception(f'Class not found: `{path}`')
     else:
         return cls
 
+
 def get_parser():
     cpu_count = multiprocessing.cpu_count()
     if cpu_count > 1:
         cpu_count = cpu_count - 1
     base_dir = pathlib.Path.cwd()
     parser = argparse.ArgumentParser(
         prog='wordz',
@@ -52,16 +52,16 @@
     verbosity.add_argument('-q', '--quiet', action='store_const', dest='loglevel', const=logs.logging.NOTSET, default=logs.logging.INFO)
     return parser
 
 
 def run(parser, args):
     parsed = parser.parse_args(args)
     logs.init(parsed.loglevel)
-    CombinatorClass = class_import(parsed.path)
-    combinator = CombinatorClass(
+    combinator_cls = class_import(parsed.path)
+    combinator = combinator_cls(
         parsed.base_dir,
         parsed.temp_dir,
         parsed.output_dir,
         parsed.min_length,
         parsed.cores,
         parsed.memory,
         parsed.bin_hashcat,
```

### Comparing `wordz-0.1.5/src/wordz.egg-info/PKG-INFO` & `wordz-0.1.6/src/wordz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordz
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wordlists builder
 Home-page: https://github.com/tasooshi/wordz
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: BSD License
 Keywords: wordlists,bruteforce,dictionary,generator,hashcat
 Classifier: Development Status :: 4 - Beta
```

