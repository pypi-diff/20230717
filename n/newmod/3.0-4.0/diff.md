# Comparing `tmp/newmod-3.0.tar.gz` & `tmp/newmod-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newmod-3.0.tar", last modified: Mon Jul 17 16:13:44 2023, max compression
+gzip compressed data, was "newmod-4.0.tar", last modified: Mon Jul 17 16:30:40 2023, max compression
```

## Comparing `newmod-3.0.tar` & `newmod-4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 newmod-3.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 newmod-3.0/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 newmod-3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3066 2023-07-17 16:13:44.865126 newmod-3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 newmod-3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.861126 newmod-3.0/newmod/
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 16:13:17.000000 newmod-3.0/newmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/filters/
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 newmod-3.0/newmod/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 newmod-3.0/newmod/filters/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/helpers/
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 newmod-3.0/newmod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 newmod-3.0/newmod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/listen/
--rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 newmod-3.0/newmod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 newmod-3.0/newmod/listen/listen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/utils/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 newmod-3.0/newmod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 newmod-3.0/newmod/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3066 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:13:44.865126 newmod-3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-17 16:13:17.000000 newmod-3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.762485 newmod-4.0/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 newmod-4.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 newmod-4.0/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 newmod-4.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-17 16:30:40.762485 newmod-4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 newmod-4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.758485 newmod-4.0/newmod/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 16:30:22.000000 newmod-4.0/newmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.762485 newmod-4.0/newmod/filters/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 newmod-4.0/newmod/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 newmod-4.0/newmod/filters/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.762485 newmod-4.0/newmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 newmod-4.0/newmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 newmod-4.0/newmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.762485 newmod-4.0/newmod/listen/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 newmod-4.0/newmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 newmod-4.0/newmod/listen/listen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.762485 newmod-4.0/newmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 newmod-4.0/newmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 newmod-4.0/newmod/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:30:40.758485 newmod-4.0/newmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-17 16:30:40.000000 newmod-4.0/newmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:30:40.000000 newmod-4.0/newmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:30:40.000000 newmod-4.0/newmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:30:40.000000 newmod-4.0/newmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:30:40.000000 newmod-4.0/newmod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:30:40.762485 newmod-4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-07-17 16:30:22.000000 newmod-4.0/setup.py
```

### Comparing `newmod-3.0/COPYING` & `newmod-4.0/COPYING`

 * *Files identical despite different names*

### Comparing `newmod-3.0/COPYING.lesser` & `newmod-4.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `newmod-3.0/NOTICE` & `newmod-4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `newmod-3.0/PKG-INFO` & `newmod-4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 3.0
-Summary: A monkeypatcher add-on for newgram
+Version: 4.0
+Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/pyromod
-Author: Cezar H.
-License: LGPLv3+
+Author: jokokendi
+Author-email: ajual7832@gmail.com
+License: GPLv3
+Download-URL: https://github.com/jokokendi/xmode/archive/v4.0.zip
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # newmod
 A monkeypatcher add-on for Newgram
```

### Comparing `newmod-3.0/README.md` & `newmod-4.0/README.md`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/__init__.py` & `newmod-4.0/newmod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "3.0"
+__version__ = "4.0"
```

### Comparing `newmod-3.0/newmod/filters/__init__.py` & `newmod-4.0/newmod/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/filters/filters.py` & `newmod-4.0/newmod/filters/filters.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/helpers/__init__.py` & `newmod-4.0/newmod/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/helpers/helpers.py` & `newmod-4.0/newmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/listen/__init__.py` & `newmod-4.0/newmod/listen/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/listen/listen.py` & `newmod-4.0/newmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/utils/__init__.py` & `newmod-4.0/newmod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod/utils/utils.py` & `newmod-4.0/newmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `newmod-3.0/newmod.egg-info/PKG-INFO` & `newmod-4.0/newmod.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 3.0
-Summary: A monkeypatcher add-on for newgram
+Version: 4.0
+Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/pyromod
-Author: Cezar H.
-License: LGPLv3+
+Author: jokokendi
+Author-email: ajual7832@gmail.com
+License: GPLv3
+Download-URL: https://github.com/jokokendi/xmode/archive/v4.0.zip
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # newmod
 A monkeypatcher add-on for Newgram
```

