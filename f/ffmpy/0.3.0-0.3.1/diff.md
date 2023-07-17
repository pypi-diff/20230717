# Comparing `tmp/ffmpy-0.3.0.tar.gz` & `tmp/ffmpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpy-0.3.0.tar", last modified: Wed Jan 13 11:55:30 2021, max compression
+gzip compressed data, was "ffmpy-0.3.1.tar", last modified: Mon Jul 17 08:34:45 2023, max compression
```

## Comparing `ffmpy-0.3.0.tar` & `ffmpy-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2021-01-13 11:55:30.044208 ffmpy-0.3.0/
--rw-rw-r--   0 ay        (1000) ay        (1000)     3077 2021-01-13 11:55:30.044208 ffmpy-0.3.0/PKG-INFO
--rw-rw-r--   0 ay        (1000) ay        (1000)     1554 2021-01-11 20:39:34.000000 ffmpy-0.3.0/README.rst
-drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2021-01-13 11:55:30.044208 ffmpy-0.3.0/ffmpy.egg-info/
--rw-rw-r--   0 ay        (1000) ay        (1000)     3077 2021-01-13 11:55:30.000000 ffmpy-0.3.0/ffmpy.egg-info/PKG-INFO
--rw-rw-r--   0 ay        (1000) ay        (1000)      154 2021-01-13 11:55:30.000000 ffmpy-0.3.0/ffmpy.egg-info/SOURCES.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)        1 2021-01-13 11:55:30.000000 ffmpy-0.3.0/ffmpy.egg-info/dependency_links.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)        6 2021-01-13 11:55:30.000000 ffmpy-0.3.0/ffmpy.egg-info/top_level.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)     8461 2021-01-13 11:43:44.000000 ffmpy-0.3.0/ffmpy.py
--rw-rw-r--   0 ay        (1000) ay        (1000)       89 2021-01-13 11:55:30.044208 ffmpy-0.3.0/setup.cfg
--rw-rw-r--   0 ay        (1000) ay        (1000)     1343 2021-01-11 18:56:33.000000 ffmpy-0.3.0/setup.py
+drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-17 08:34:45.558141 ffmpy-0.3.1/
+-rw-rw-r--   0 ay        (1000) ay        (1000)     1054 2021-01-11 18:14:06.000000 ffmpy-0.3.1/LICENSE
+-rw-rw-r--   0 ay        (1000) ay        (1000)     2778 2023-07-17 08:34:45.558141 ffmpy-0.3.1/PKG-INFO
+-rw-rw-r--   0 ay        (1000) ay        (1000)     1554 2021-01-11 20:39:34.000000 ffmpy-0.3.1/README.rst
+drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-17 08:34:45.558141 ffmpy-0.3.1/ffmpy.egg-info/
+-rw-rw-r--   0 ay        (1000) ay        (1000)     2778 2023-07-17 08:34:45.000000 ffmpy-0.3.1/ffmpy.egg-info/PKG-INFO
+-rw-rw-r--   0 ay        (1000) ay        (1000)      162 2023-07-17 08:34:45.000000 ffmpy-0.3.1/ffmpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)        1 2023-07-17 08:34:45.000000 ffmpy-0.3.1/ffmpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)        6 2023-07-17 08:34:45.000000 ffmpy-0.3.1/ffmpy.egg-info/top_level.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)     8732 2023-07-17 08:28:05.000000 ffmpy-0.3.1/ffmpy.py
+-rw-rw-r--   0 ay        (1000) ay        (1000)       89 2023-07-17 08:34:45.558141 ffmpy-0.3.1/setup.cfg
+-rw-rw-r--   0 ay        (1000) ay        (1000)     1443 2023-07-17 08:28:41.000000 ffmpy-0.3.1/setup.py
```

### Comparing `ffmpy-0.3.0/PKG-INFO` & `ffmpy-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,79 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ffmpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple Python wrapper for ffmpeg
 Home-page: https://github.com/Ch00k/ffmpy
 Author: Andrii Yurchuk
 Author-email: ay@mntw.re
 License: MIT
-Description: .. image:: https://github.com/Ch00k/ffmpy/workflows/test/badge.svg
-            :target: https://github.com/Ch00k/ffmpy/actions
-            :alt: Tests
-        
-        .. image:: https://codecov.io/gh/Ch00k/ffmpy/branch/master/graphs/badge.svg
-            :target: https://codecov.io/github/Ch00k/ffmpy
-            :alt: Coverage
-        
-        .. image:: https://readthedocs.org/projects/ffmpy/badge/?version=latest
-            :target: http://ffmpy.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation
-        
-        .. image:: https://img.shields.io/pypi/v/ffmpy.svg
-            :target: https://pypi.python.org/pypi/ffmpy
-            :alt: Latest version
-        
-        
-        ffmpy
-        =====
-        ffmpy is a simplistic `FFmpeg <http://ffmpeg.org/>`_ command line wrapper. It implements a Pythonic interface for FFmpeg command line compilation and uses Python `subprocess <https://docs.python.org/2/library/subprocess.html>`_ module to execute compiled command line.
-        
-        Installation
-        ------------
-        You guessed it::
-        
-          pip install ffmpy
-        
-        Quick example
-        -------------
-        .. code:: python
-        
-          >>> import ffmpy
-          >>> ff = ffmpy.FFmpeg(
-          ...     inputs={'input.mp4': None},
-          ...     outputs={'output.avi': None}
-          ... )
-          >>> ff.run()
-        
-        This will take ``input.mp4`` file in the current directory as the input, change the video container from MP4 to AVI without changing any other video parameters and create a new output file ``output.avi`` in the current directory.
-        
-        Documentation
-        -------------
-        http://ffmpy.rtfd.io
-        
-        See `Examples <http://ffmpy.readthedocs.io/en/latest/examples.html>`_ section for usage examples.
-        
-        License
-        -------
-        ffmpy is licensed under the terms of MIT license
-        
 Keywords: ffmpeg ffprobe wrapper audio video transcoding
-Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
+License-File: LICENSE
+
+.. image:: https://github.com/Ch00k/ffmpy/workflows/test/badge.svg
+    :target: https://github.com/Ch00k/ffmpy/actions
+    :alt: Tests
+
+.. image:: https://codecov.io/gh/Ch00k/ffmpy/branch/master/graphs/badge.svg
+    :target: https://codecov.io/github/Ch00k/ffmpy
+    :alt: Coverage
+
+.. image:: https://readthedocs.org/projects/ffmpy/badge/?version=latest
+    :target: http://ffmpy.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation
+
+.. image:: https://img.shields.io/pypi/v/ffmpy.svg
+    :target: https://pypi.python.org/pypi/ffmpy
+    :alt: Latest version
+
+
+ffmpy
+=====
+ffmpy is a simplistic `FFmpeg <http://ffmpeg.org/>`_ command line wrapper. It implements a Pythonic interface for FFmpeg command line compilation and uses Python `subprocess <https://docs.python.org/2/library/subprocess.html>`_ module to execute compiled command line.
+
+Installation
+------------
+You guessed it::
+
+  pip install ffmpy
+
+Quick example
+-------------
+.. code:: python
+
+  >>> import ffmpy
+  >>> ff = ffmpy.FFmpeg(
+  ...     inputs={'input.mp4': None},
+  ...     outputs={'output.avi': None}
+  ... )
+  >>> ff.run()
+
+This will take ``input.mp4`` file in the current directory as the input, change the video container from MP4 to AVI without changing any other video parameters and create a new output file ``output.avi`` in the current directory.
+
+Documentation
+-------------
+http://ffmpy.rtfd.io
+
+See `Examples <http://ffmpy.readthedocs.io/en/latest/examples.html>`_ section for usage examples.
+
+License
+-------
+ffmpy is licensed under the terms of MIT license
```

### Comparing `ffmpy-0.3.0/README.rst` & `ffmpy-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ffmpy-0.3.0/ffmpy.egg-info/PKG-INFO` & `ffmpy-0.3.1/ffmpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,79 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ffmpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple Python wrapper for ffmpeg
 Home-page: https://github.com/Ch00k/ffmpy
 Author: Andrii Yurchuk
 Author-email: ay@mntw.re
 License: MIT
-Description: .. image:: https://github.com/Ch00k/ffmpy/workflows/test/badge.svg
-            :target: https://github.com/Ch00k/ffmpy/actions
-            :alt: Tests
-        
-        .. image:: https://codecov.io/gh/Ch00k/ffmpy/branch/master/graphs/badge.svg
-            :target: https://codecov.io/github/Ch00k/ffmpy
-            :alt: Coverage
-        
-        .. image:: https://readthedocs.org/projects/ffmpy/badge/?version=latest
-            :target: http://ffmpy.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation
-        
-        .. image:: https://img.shields.io/pypi/v/ffmpy.svg
-            :target: https://pypi.python.org/pypi/ffmpy
-            :alt: Latest version
-        
-        
-        ffmpy
-        =====
-        ffmpy is a simplistic `FFmpeg <http://ffmpeg.org/>`_ command line wrapper. It implements a Pythonic interface for FFmpeg command line compilation and uses Python `subprocess <https://docs.python.org/2/library/subprocess.html>`_ module to execute compiled command line.
-        
-        Installation
-        ------------
-        You guessed it::
-        
-          pip install ffmpy
-        
-        Quick example
-        -------------
-        .. code:: python
-        
-          >>> import ffmpy
-          >>> ff = ffmpy.FFmpeg(
-          ...     inputs={'input.mp4': None},
-          ...     outputs={'output.avi': None}
-          ... )
-          >>> ff.run()
-        
-        This will take ``input.mp4`` file in the current directory as the input, change the video container from MP4 to AVI without changing any other video parameters and create a new output file ``output.avi`` in the current directory.
-        
-        Documentation
-        -------------
-        http://ffmpy.rtfd.io
-        
-        See `Examples <http://ffmpy.readthedocs.io/en/latest/examples.html>`_ section for usage examples.
-        
-        License
-        -------
-        ffmpy is licensed under the terms of MIT license
-        
 Keywords: ffmpeg ffprobe wrapper audio video transcoding
-Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
+License-File: LICENSE
+
+.. image:: https://github.com/Ch00k/ffmpy/workflows/test/badge.svg
+    :target: https://github.com/Ch00k/ffmpy/actions
+    :alt: Tests
+
+.. image:: https://codecov.io/gh/Ch00k/ffmpy/branch/master/graphs/badge.svg
+    :target: https://codecov.io/github/Ch00k/ffmpy
+    :alt: Coverage
+
+.. image:: https://readthedocs.org/projects/ffmpy/badge/?version=latest
+    :target: http://ffmpy.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation
+
+.. image:: https://img.shields.io/pypi/v/ffmpy.svg
+    :target: https://pypi.python.org/pypi/ffmpy
+    :alt: Latest version
+
+
+ffmpy
+=====
+ffmpy is a simplistic `FFmpeg <http://ffmpeg.org/>`_ command line wrapper. It implements a Pythonic interface for FFmpeg command line compilation and uses Python `subprocess <https://docs.python.org/2/library/subprocess.html>`_ module to execute compiled command line.
+
+Installation
+------------
+You guessed it::
+
+  pip install ffmpy
+
+Quick example
+-------------
+.. code:: python
+
+  >>> import ffmpy
+  >>> ff = ffmpy.FFmpeg(
+  ...     inputs={'input.mp4': None},
+  ...     outputs={'output.avi': None}
+  ... )
+  >>> ff.run()
+
+This will take ``input.mp4`` file in the current directory as the input, change the video container from MP4 to AVI without changing any other video parameters and create a new output file ``output.avi`` in the current directory.
+
+Documentation
+-------------
+http://ffmpy.rtfd.io
+
+See `Examples <http://ffmpy.readthedocs.io/en/latest/examples.html>`_ section for usage examples.
+
+License
+-------
+ffmpy is licensed under the terms of MIT license
```

### Comparing `ffmpy-0.3.0/ffmpy.py` & `ffmpy-0.3.1/ffmpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import errno
 import shlex
 import subprocess
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 class FFmpeg(object):
     """Wrapper for various `FFmpeg <https://www.ffmpeg.org/>`_ related applications (ffmpeg,
     ffprobe).
     """
 
@@ -56,15 +56,15 @@
 
         self.cmd = subprocess.list2cmdline(self._cmd)
         self.process = None
 
     def __repr__(self):
         return "<{0!r} {1!r}>".format(self.__class__.__name__, self.cmd)
 
-    def run(self, input_data=None, stdout=None, stderr=None, env=None):
+    def run(self, input_data=None, stdout=None, stderr=None, env=None, **kwargs):
         """Execute FFmpeg command line.
 
         ``input_data`` can contain input for FFmpeg in case ``pipe`` protocol is used for input.
         ``stdout`` and ``stderr`` specify where to redirect the ``stdout`` and ``stderr`` of the
         process. By default no redirection is done, which means all output goes to running shell
         (this mode should normally only be used for debugging purposes). If FFmpeg ``pipe`` protocol
         is used for output, ``stdout`` must be redirected to a pipe by passing `subprocess.PIPE` as
@@ -80,22 +80,29 @@
         :param str input_data: input data for FFmpeg to deal with (audio, video etc.) as bytes (e.g.
             the result of reading a file in binary mode)
         :param stdout: redirect FFmpeg ``stdout`` there (default is `None` which means no
             redirection)
         :param stderr: redirect FFmpeg ``stderr`` there (default is `None` which means no
             redirection)
         :param env: custom environment for ffmpeg process
+        :param kwargs: any other keyword arguments to be forwarded to `subprocess.Popen
+            <https://docs.python.org/3/library/subprocess.html#subprocess.Popen>`_
         :return: a 2-tuple containing ``stdout`` and ``stderr`` of the process
         :rtype: tuple
         :raise: `FFRuntimeError` in case FFmpeg command exits with a non-zero code;
             `FFExecutableNotFoundError` in case the executable path passed was not valid
         """
         try:
             self.process = subprocess.Popen(
-                self._cmd, stdin=subprocess.PIPE, stdout=stdout, stderr=stderr, env=env
+                self._cmd,
+                stdin=subprocess.PIPE,
+                stdout=stdout,
+                stderr=stderr,
+                env=env,
+                **kwargs
             )
         except OSError as e:
             if e.errno == errno.ENOENT:
                 raise FFExecutableNotFoundError(
                     "Executable '{0}' not found".format(self.executable)
                 )
             else:
```

### Comparing `ffmpy-0.3.0/setup.py` & `ffmpy-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: BSD",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
```

