# Comparing `tmp/noelmode-1.0.3.tar.gz` & `tmp/noelmode-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noelmode-1.0.3.tar", last modified: Mon Jul 17 00:21:40 2023, max compression
+gzip compressed data, was "noelmode-1.0.4.tar", last modified: Mon Jul 17 00:26:38 2023, max compression
```

## Comparing `noelmode-1.0.3.tar` & `noelmode-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 00:21:07.000000 noelmode-1.0.3/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 00:21:07.000000 noelmode-1.0.3/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-17 00:21:07.000000 noelmode-1.0.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:21:40.823463 noelmode-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7063 2023-07-17 00:21:07.000000 noelmode-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/noelmode/
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-17 00:21:07.000000 noelmode-1.0.3/noelmode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:21:40.823463 noelmode-1.0.3/noelmode.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:21:40.000000 noelmode-1.0.3/noelmode.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 00:21:40.823463 noelmode-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 00:21:07.000000 noelmode-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:38.975873 noelmode-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 00:21:07.000000 noelmode-1.0.4/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 00:21:07.000000 noelmode-1.0.4/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-17 00:21:07.000000 noelmode-1.0.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:26:38.975873 noelmode-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-07-17 00:21:07.000000 noelmode-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:38.975873 noelmode-1.0.4/noelmode/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-07-17 00:26:30.000000 noelmode-1.0.4/noelmode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:38.975873 noelmode-1.0.4/noelmode.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7892 2023-07-17 00:26:38.000000 noelmode-1.0.4/noelmode.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-17 00:26:38.000000 noelmode-1.0.4/noelmode.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:26:38.000000 noelmode-1.0.4/noelmode.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:26:38.000000 noelmode-1.0.4/noelmode.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 00:26:38.000000 noelmode-1.0.4/noelmode.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 00:26:38.975873 noelmode-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 00:26:30.000000 noelmode-1.0.4/setup.py
```

### Comparing `noelmode-1.0.3/COPYING` & `noelmode-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.3/COPYING.lesser` & `noelmode-1.0.4/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.3/NOTICE` & `noelmode-1.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.3/PKG-INFO` & `noelmode-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.3
+Version: 1.0.4
 Summary: pyromod custom
 Home-page: https://github.com/jokokendi/xmode
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: MIT
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.3.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.4.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `noelmode-1.0.3/README.md` & `noelmode-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.3/noelmode/__init__.py` & `noelmode-1.0.4/noelmode/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with noelmode.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from .listen import *
-from .utils import NoelmodConfig
+from noelmode.listen import *
+from noelmode.utils import NoelmodConfig
```

### Comparing `noelmode-1.0.3/noelmode.egg-info/PKG-INFO` & `noelmode-1.0.4/noelmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.3
+Version: 1.0.4
 Summary: pyromod custom
 Home-page: https://github.com/jokokendi/xmode
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: MIT
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.3.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.4.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `noelmode-1.0.3/setup.py` & `noelmode-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = '1.0.3'
+version = '1.0.4'
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='noelmode',
```

