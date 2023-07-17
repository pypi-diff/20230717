# Comparing `tmp/lognflow-0.7.5.tar.gz` & `tmp/lognflow-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.5.tar", last modified: Tue Jun 27 03:29:02 2023, max compression
+gzip compressed data, was "lognflow-0.7.6.tar", last modified: Mon Jul 17 02:29:51 2023, max compression
```

## Comparing `lognflow-0.7.5.tar` & `lognflow-0.7.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 03:28:52.000000 lognflow-0.7.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-27 03:28:52.000000 lognflow-0.7.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-27 03:28:52.000000 lognflow-0.7.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-27 03:28:52.000000 lognflow-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 03:28:52.000000 lognflow-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-27 03:29:02.686514 lognflow-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 03:28:52.000000 lognflow-0.7.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 03:28:52.000000 lognflow-0.7.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66489 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-27 03:28:52.000000 lognflow-0.7.5/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 03:29:02.000000 lognflow-0.7.5/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-27 03:29:02.686514 lognflow-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-27 03:28:52.000000 lognflow-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:29:02.686514 lognflow-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 03:28:52.000000 lognflow-0.7.5/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 02:29:40.000000 lognflow-0.7.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-17 02:29:40.000000 lognflow-0.7.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-17 02:29:40.000000 lognflow-0.7.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 02:29:40.000000 lognflow-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-17 02:29:40.000000 lognflow-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-17 02:29:51.787692 lognflow-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 02:29:40.000000 lognflow-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.783692 lognflow-0.7.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.783692 lognflow-0.7.6/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67409 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-17 02:29:51.787692 lognflow-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-17 02:29:40.000000 lognflow-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.5/CONTRIBUTING.rst` & `lognflow-0.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/HISTORY.rst` & `lognflow-0.7.6/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -102,10 +102,17 @@
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
 * critical bug fixed in log_imshow
 
-0.7.5 (2023-08-01)
+0.7.5 (2023-06-27)
 ------------------
-* Added complex numbers to log_imshow
+* Added complex numbers to log_imshow
+
+0.7.6 (2023-07-17)
+------------------
+* printprogress can handle up to 99 days
+* log_text takes any save_as
+* If variable name has escape key is alright
+* If variable name is splitable, we replace them with _
```

### Comparing `lognflow-0.7.5/LICENSE` & `lognflow-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/PKG-INFO` & `lognflow-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.5
+Version: 0.7.6
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -195,10 +195,17 @@
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
 * critical bug fixed in log_imshow
 
-0.7.5 (2023-08-01)
+0.7.5 (2023-06-27)
 ------------------
 * Added complex numbers to log_imshow
+
+0.7.6 (2023-07-17)
+------------------
+* printprogress can handle up to 99 days
+* log_text takes any save_as
+* If variable name has escape key is alright
+* If variable name is splitable, we replace them with _
```

### Comparing `lognflow-0.7.5/README.rst` & `lognflow-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/docs/Makefile` & `lognflow-0.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/docs/conf.py` & `lognflow-0.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/docs/installation.rst` & `lognflow-0.7.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/docs/make.bat` & `lognflow-0.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/lognflow/lognflow.py` & `lognflow-0.7.6/lognflow/lognflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 """
 
 import pathlib
 import time
 import itertools
 from   dataclasses import dataclass
+from re import sub as re_sub
+from unicodedata import normalize as unicodedata_normalize
 from   os import sep as os_sep
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from   matplotlib import animation
 
 from .logviewer import logviewer
@@ -62,14 +64,42 @@
     to_be_logged        : str   
     log_fpath           : pathlib.Path         
     log_size_limit      : int 
     log_size            : int     
     last_log_flush_time : float
     log_flush_period    : int
 
+def repr_raw(text):
+    """Returns a raw string representation of a text with escape charachters"""
+    escape_dict={'\a':r'\a',
+                 '\b':r'\b',
+                 '\c':r'\c',
+                 '\f':r'\f',
+                 '\n':r'\n',
+                 '\r':r'\r',
+                 '\t':r'\t',
+                 '\v':r'\v',
+                 '\'':r'\'',
+                 '\"':r'\"'}
+    new_string=''
+    for char in text:
+        try: 
+            new_string += escape_dict[char]
+        except KeyError: 
+            new_string += char
+    return new_string
+
+def replace_all(text, pattern, fill_value):
+    while (len(text.split(pattern)) > 1):
+        text = text.replace(pattern, fill_value)
+    return text
+
+if __name__ == '__main__':
+    name = 'asdfkyt sdyufg%^&*()'
+
 class lognflow:
     """Initialization
         
         lognflow creates a directory/attribute called log_dir and puts all 
         stored data in there, if logs_root is given. Otherwise give it log_dir
         to use. If you type
         
@@ -183,14 +213,17 @@
         self._single_var_call_cnt = 0
 
         self.log_name = main_log_name
         self.log_flush_period = log_flush_period
     
     @property
     def time_stamp(self):
+        """ Current time stamp
+            Gives the time after the start of the lognflow
+        """
         return time.time() - self._init_time
     
     def rename(self, new_name:str, append: bool = False):
         """ renaming the log directory
             It is possible to rename the log directory while logging is going
             on. This is particulary useful when at the end of an experiment,
             it is necessary to put some variables in the name of the directory,
@@ -242,36 +275,28 @@
             self.log_text(None, f'{self.log_dir.name}')
             self.log_text(None, 'into:')
             self.log_text(None, f'{new_name}')
             self.log_text(None, 'Most probably a file was open.')
         return self.log_dir
     
     def _prepare_param_dir(self, parameter_name: str):
-        try:
-            _ = parameter_name.split()
-        except:
-            self.log_text(
-                self.log_name,
-                f'The parameter name {parameter_name} is not a string.' \
-                + f' Its type is {type(parameter_name)}.')
-        assert len(parameter_name.split()) == 1, \
-            self.log_text(self.log_name,\
-                  f'The variable name {parameter_name} you chose, is splitable'\
-                + f' I can split it into {parameter_name.split()}'             \
-                + ' Make sure you dont use space, tab, or backslash with known'\
-                + ' small letters such as f, t, ...'                           \
-                + ' If you are using single backslash, e.g. for windows'       \
-                + ' folders, replace it with \\ or make it a literal string'   \
-                + ' by putting an r before the variable name.')
         
-        is_dir = (parameter_name[-1] == '/') | (parameter_name[-1] == '\\') \
-                 | (parameter_name[-1] == r'/') | (parameter_name[-1] == r'\\')
+        assert isinstance(parameter_name, str), \
+            f'The parameter name {parameter_name} is not a string.' \
+            + f' It is of type {type(parameter_name)}.' \
+            + 'Perhaps you forgot to pass the name of the variable first.'
+        parameter_name = ''.join(
+            [_ for _ in repr(repr_raw(parameter_name))  if _ != '\''])
+        parameter_name = replace_all(parameter_name, ' ', '_')
+        parameter_name = replace_all(parameter_name, '\\', '/')
+        parameter_name = replace_all(parameter_name, '//', '/')
+        
         param_dir = self.log_dir /  parameter_name
         
-        if(is_dir):
+        if(parameter_name[-1] == '/'):
             param_name = ''
         else:
             param_name = param_dir.name
             param_dir = param_dir.parent
         if(not param_dir.is_dir()):
             self.log_text(self.log_name,
                           f'Creating directory: {param_dir.absolute()}')
@@ -289,27 +314,28 @@
         
         if(len(param_name) > 0):
             fname = f'{param_name}'
             if(time_tag):
                 fname += f'_{self.time_stamp:>6.6f}'
         else:
             fname = f'{self.time_stamp:>6.6f}'
-            
+        
         return(param_dir / f'{fname}.{save_as}')
         
     def _log_text_handler(self, log_name = None, 
                          log_size_limit: int = int(1e+7),
                          time_tag: bool = None,
-                         log_flush_period = None):
+                         log_flush_period = None,
+                         save_as = 'txt'):
         
         if (log_flush_period is None):
             log_flush_period = self.log_flush_period
             
         param_dir, param_name = self._prepare_param_dir(log_name)
-        fpath = self._get_fpath(param_dir, param_name, 'txt', time_tag)
+        fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
         self._loggers_dict[log_name] = textinlog(
             to_be_logged=[],      
             log_fpath=fpath,         
             log_size_limit=log_size_limit,    
             log_size=0,          
             last_log_flush_time=0,
             log_flush_period=log_flush_period)  
@@ -347,15 +373,16 @@
                  log_time_stamp = True,
                  print_text = None,
                  log_size_limit: int = int(1e+7),
                  time_tag: bool = None,
                  log_flush_period: int = None,
                  flush = False,
                  end = '\n',
-                 new_file = False):
+                 new_file = False,
+                 save_as = 'txt'):
         """ log a string into a text file
             You can shose a name for the log and give the text to put in it.
             Also you can pass a small numpy array. You can ask it to put time
             stamp in the log and in the log file name, you can disable
             printing the text. You can set the log size limit to split it into
             another file with a new time stamp.
             
@@ -382,14 +409,16 @@
                    force flush into the log file
             :param end: str
                    The last charachter for this call.
             :param new_file: bool
                    if a new file is needed. If time_tag is True, it will make
                    a new file with a new name that has a time tag. If False,
                    it closees the current text file and overwrites on it.
+            :param save_as: str
+                   save_as is the suffix of the text file.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
         log_name = self.log_name if (log_name is None) else log_name
 
         if((print_text is None) | (print_text is True)):
@@ -398,15 +427,16 @@
             if(log_time_stamp):
                 print(f'T:{self.time_stamp:>6.6f}| ', end='')
             print(to_be_logged, end = end)
                 
         if ( (not (log_name in self._loggers_dict)) or new_file):
             self._log_text_handler(log_name, 
                                    log_size_limit = log_size_limit,
-                                   time_tag = time_tag)
+                                   time_tag = time_tag,
+                                   save_as = save_as)
 
         curr_textinlog = self._loggers_dict[log_name]
         _logger = []
         if(log_time_stamp):
             _time_str = f'T:{self.time_stamp:>6.6f}| '
             _logger.append(_time_str)
         if(isinstance(to_be_logged, list)):
@@ -581,53 +611,56 @@
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param parameter_value: np.array
                     An np array whose size doesn't change
             :param save_as: str
                     can be 'npz', 'npy', 'mat', 'torch' for pytorch models
-                    or 'txt' which will save it as text.
+                    or 'txt' or anything else which will save it as text.
+                    This includes 'json', 'pdb', or ...
             :param mat_field: str
                     when saving as 'mat' file, the field can be set.
                     otherwise it will be the parameter_name
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
         if(save_as is None):
-            save_as = 'npy'
+            if isinstance(parameter_value, (np.ndarray, int, float)):
+                save_as = 'npy'
             if (isinstance(parameter_value, dict)):
                 save_as = 'npz'
         save_as = save_as.strip()
         save_as = save_as.strip('.')
 
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
-            
-        if(save_as == 'npy'):
-            np.save(fpath, parameter_value)
-        elif(save_as == 'npz'):
-            np.savez(fpath, **parameter_value)
-        elif((save_as == 'tif') | (save_as == 'tiff')):
-            from tifffile import imwrite
-            imwrite(fpath, parameter_value)
-        elif(save_as == 'txt'):
-            with open(fpath,'a') as fdata: 
-                fdata.write(str(parameter_value))
-        elif(save_as == 'mat'):
-            from scipy.io import savemat
-            if(mat_field is None):
-                mat_field = param_name
-            savemat(fpath, {f'{mat_field}':parameter_value})
-        elif(save_as == 'torch'):
-            from torch import save as torch_save
-            torch_save(parameter_value.state_dict(), fpath)
-        else:
+        
+        try:
+            if(save_as == 'npy'):
+                np.save(fpath, parameter_value)
+            elif(save_as == 'npz'):
+                np.savez(fpath, **parameter_value)
+            elif((save_as == 'tif') | (save_as == 'tiff')):
+                from tifffile import imwrite
+                imwrite(fpath, parameter_value)
+            elif(save_as == 'mat'):
+                from scipy.io import savemat
+                if(mat_field is None):
+                    mat_field = param_name
+                savemat(fpath, {f'{mat_field}':parameter_value})
+            elif(save_as == 'torch'):
+                from torch import save as torch_save
+                torch_save(parameter_value.state_dict(), fpath)
+            else:
+                with open(fpath,'a') as fdata: 
+                    fdata.write(str(parameter_value))
+        except:
             fpath = None
         return fpath
     
     def log_plt(self, 
                 parameter_name: str, 
                 image_format='jpeg', dpi=1200,
                 time_tag: bool = None,
```

### Comparing `lognflow-0.7.5/lognflow/logviewer.py` & `lognflow-0.7.6/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/lognflow/printprogress.py` & `lognflow-0.7.6/lognflow/printprogress.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,23 +112,27 @@
             else:
                 remTimeS = self._calc_ETA() # useful when print_function is None
                 cProg = int(self.numTicks*self.ck/(self.n_steps-1)/3)    
                 #3: because 3 charachters are used
                 while((self.prog < cProg) & (not self.FLAG_ended)):
                     self.prog += 1
                     remTimeS = self._calc_ETA()
-                    if(remTimeS>5940): # less than 99h and more than 99m
+                    if(remTimeS>356400): # less than 99d and more than 99h
+                        progStr = "%02d" % int(ceil(remTimeS/86400))
+                        self._print_func(progStr, end='')
+                        self._print_func('d', end='')
+                    elif(remTimeS>5940): # less than 99h and more than 99m
                         progStr = "%02d" % int(ceil(remTimeS/3600))
                         self._print_func(progStr, end='')
                         self._print_func('h', end='')
                     elif(remTimeS>99): # less than 99m and more than 99s
                         progStr = "%02d" % int(ceil(remTimeS/60))
                         self._print_func(progStr, end='')
                         self._print_func('m', end='')
-                    elif(remTimeS>0): # less than 99s and more than 0
+                    elif(remTimeS>=0): # less than 99s and more than 0
                         progStr = "%02d" % int(ceil(remTimeS))
                         self._print_func(progStr, end='')
                         self._print_func('s', end='')
                     else:
                         self.end()
         return remTimeS
     def end(self):
```

### Comparing `lognflow-0.7.5/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.6/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.5
+Version: 0.7.6
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -195,10 +195,17 @@
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
 
 0.7.4 (2023-06-26)
 ------------------
 * critical bug fixed in log_imshow
 
-0.7.5 (2023-08-01)
+0.7.5 (2023-06-27)
 ------------------
 * Added complex numbers to log_imshow
+
+0.7.6 (2023-07-17)
+------------------
+* printprogress can handle up to 99 days
+* log_text takes any save_as
+* If variable name has escape key is alright
+* If variable name is splitable, we replace them with _
```

### Comparing `lognflow-0.7.5/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.6/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/setup.py` & `lognflow-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.5'
+__version__ = '0.7.6'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.5/tests/test_lognflow.py` & `lognflow-0.7.6/tests/test_lognflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,17 +264,17 @@
     logger.rename(logger.log_dir.name + '_new_name')
     logger('This is another test for test_rename')
     
 def test_log_single_text():
     logger = lognflow(temp_dir)
     logger('This is a test for test_log_single_text', flush = True)
     var = 2
-    logger.log_single('text_log', 'hello\n', save_as='txt', time_tag = False)
-    logger.log_single('text_log', 'bye\n', save_as='txt', time_tag = False)
-    logger.log_single('text_log', var, save_as='txt', time_tag = False)
+    logger.log_single('text_log\a\t/\b/\b//\\/b', 'hello\n', save_as='txt', time_tag = False)
+    logger.log_single('text_log\a', 'bye\n', save_as='json', time_tag = False)
+    logger.log_single('text_log\a', var, save_as='pdb', time_tag = False)
     
 def test_log_imshow_complex():
     logger = lognflow(temp_dir)
     logger('This is a test for test_log_imshow_complex', flush = True)
     
     mat = np.random.rand(100, 100) + 10 * 1j * np.random.rand(100, 100)
     
@@ -283,18 +283,18 @@
     
     
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
+    test_log_single_text()
     test_log_imshow_complex()
     test_log_imshow()
     test_log_text()
-    test_log_single_text()
     test_log_surface()
     test_log_single()
     test_lognflow_conflict_in_names()
     test_rename()
     test_log_plot()
     test_prepare_stack_of_images()
     test_logger()
@@ -304,8 +304,7 @@
     test_log_animation()
     test_log_hist()
     test_log_scatter3()
     test_log_plt()
     test_log_hexbin()
     test_log_canvas()
     test_log_confusion_matrix()
-    exit()
```

### Comparing `lognflow-0.7.5/tests/test_logviewer.py` & `lognflow-0.7.6/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.5/tests/test_printprogress.py` & `lognflow-0.7.6/tests/test_printprogress.py`

 * *Files identical despite different names*

