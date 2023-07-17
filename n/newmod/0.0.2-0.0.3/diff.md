# Comparing `tmp/newmod-0.0.2.tar.gz` & `tmp/newmod-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newmod-0.0.2.tar", last modified: Mon Jul 17 16:44:23 2023, max compression
+gzip compressed data, was "newmod-0.0.3.tar", last modified: Mon Jul 17 16:47:07 2023, max compression
```

## Comparing `newmod-0.0.2.tar` & `newmod-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.202088 newmod-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 newmod-0.0.2/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 newmod-0.0.2/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 newmod-0.0.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3419 2023-07-17 16:44:23.202088 newmod-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 newmod-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.198088 newmod-0.0.2/newmod/
--rw-r--r--   0 root         (0) root         (0)      759 2023-07-17 16:44:07.000000 newmod-0.0.2/newmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.202088 newmod-0.0.2/newmod/filters/
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/filters/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.202088 newmod-0.0.2/newmod/helpers/
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.202088 newmod-0.0.2/newmod/listen/
--rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/listen/listen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.202088 newmod-0.0.2/newmod/utils/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 newmod-0.0.2/newmod/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:44:23.198088 newmod-0.0.2/newmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3419 2023-07-17 16:44:23.000000 newmod-0.0.2/newmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:44:23.000000 newmod-0.0.2/newmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:44:23.000000 newmod-0.0.2/newmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 16:44:23.000000 newmod-0.0.2/newmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:44:23.000000 newmod-0.0.2/newmod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:44:23.202088 newmod-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1321 2023-07-17 16:44:07.000000 newmod-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 newmod-0.0.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 newmod-0.0.3/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 newmod-0.0.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3419 2023-07-17 16:47:07.498799 newmod-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 newmod-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.494799 newmod-0.0.3/newmod/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-07-17 16:47:00.000000 newmod-0.0.3/newmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/newmod/filters/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/filters/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/newmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/newmod/listen/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/listen/listen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/newmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 newmod-0.0.3/newmod/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:47:07.498799 newmod-0.0.3/newmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3419 2023-07-17 16:47:07.000000 newmod-0.0.3/newmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:47:07.000000 newmod-0.0.3/newmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:47:07.000000 newmod-0.0.3/newmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 16:47:07.000000 newmod-0.0.3/newmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:47:07.000000 newmod-0.0.3/newmod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:47:07.498799 newmod-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-17 16:47:00.000000 newmod-0.0.3/setup.py
```

### Comparing `newmod-0.0.2/COPYING` & `newmod-0.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/COPYING.lesser` & `newmod-0.0.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/NOTICE` & `newmod-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/PKG-INFO` & `newmod-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/pyromod
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: GPLv3
-Download-URL: https://github.com/jokokendi/xmode/archive/v0.0.2.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `newmod-0.0.2/README.md` & `newmod-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/__init__.py` & `newmod-0.0.3/newmod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `newmod-0.0.2/newmod/filters/__init__.py` & `newmod-0.0.3/newmod/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/filters/filters.py` & `newmod-0.0.3/newmod/filters/filters.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/helpers/__init__.py` & `newmod-0.0.3/newmod/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/helpers/helpers.py` & `newmod-0.0.3/newmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/listen/__init__.py` & `newmod-0.0.3/newmod/listen/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/listen/listen.py` & `newmod-0.0.3/newmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/utils/__init__.py` & `newmod-0.0.3/newmod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod/utils/utils.py` & `newmod-0.0.3/newmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `newmod-0.0.2/newmod.egg-info/PKG-INFO` & `newmod-0.0.3/newmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/pyromod
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: GPLv3
-Download-URL: https://github.com/jokokendi/xmode/archive/v0.0.2.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `newmod-0.0.2/setup.py` & `newmod-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 # -*- coding: utf-8 -*-
 
 import re
 
 from setuptools import setup, find_packages
 
 
-with open("req.txt") as r:
-    requirements = [i.strip() for i in r]
-
 with open("newmod/__init__.py") as x:
     version = re.search(r'__version__ = "(.*?)"', x.read()).group(1)
 
 with open('README.md') as f:
     long_description = f.read()
 
 
@@ -27,15 +24,15 @@
     long_description_content_type='text/markdown',
 
     download_url='https://github.com/jokokendi/xmode/archive/v{}.zip'.format(
         version
     ),
     license='GPLv3',
     packages=find_packages(),
-    install_requires=requirements,
+    install_requires="Newgram",
     python_requires="~=3.7",
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

