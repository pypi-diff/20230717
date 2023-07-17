# Comparing `tmp/newmod-2.0.tar.gz` & `tmp/newmod-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newmod-2.0.tar", last modified: Mon Jul 17 16:08:10 2023, max compression
+gzip compressed data, was "newmod-3.0.tar", last modified: Mon Jul 17 16:13:44 2023, max compression
```

## Comparing `newmod-2.0.tar` & `newmod-3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.611559 newmod-2.0/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:07:46.000000 newmod-2.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:07:46.000000 newmod-2.0/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:07:46.000000 newmod-2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3065 2023-07-17 16:08:10.611559 newmod-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:07:46.000000 newmod-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 16:07:46.000000 newmod-2.0/newmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/filters/
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:07:46.000000 newmod-2.0/newmod/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:07:46.000000 newmod-2.0/newmod/filters/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/helpers/
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:07:46.000000 newmod-2.0/newmod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:07:46.000000 newmod-2.0/newmod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/listen/
--rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:07:46.000000 newmod-2.0/newmod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:07:46.000000 newmod-2.0/newmod/listen/listen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod/utils/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:07:46.000000 newmod-2.0/newmod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:07:46.000000 newmod-2.0/newmod/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:08:10.607559 newmod-2.0/newmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3065 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:08:10.000000 newmod-2.0/newmod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:08:10.611559 newmod-2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      907 2023-07-17 16:07:46.000000 newmod-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 newmod-3.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 newmod-3.0/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 newmod-3.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-07-17 16:13:44.865126 newmod-3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 newmod-3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.861126 newmod-3.0/newmod/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-17 16:13:17.000000 newmod-3.0/newmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/filters/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 newmod-3.0/newmod/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 newmod-3.0/newmod/filters/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 newmod-3.0/newmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 newmod-3.0/newmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/listen/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 newmod-3.0/newmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 newmod-3.0/newmod/listen/listen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 newmod-3.0/newmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 newmod-3.0/newmod/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:13:44.865126 newmod-3.0/newmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:13:44.000000 newmod-3.0/newmod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:13:44.865126 newmod-3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-17 16:13:17.000000 newmod-3.0/setup.py
```

### Comparing `newmod-2.0/COPYING` & `newmod-3.0/COPYING`

 * *Files identical despite different names*

### Comparing `newmod-2.0/COPYING.lesser` & `newmod-3.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `newmod-2.0/NOTICE` & `newmod-3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `newmod-2.0/PKG-INFO` & `newmod-3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 2.0
+Version: 3.0
 Summary: A monkeypatcher add-on for newgram
-Home-page: https://github.com/jokokendi/newmod
+Home-page: https://github.com/jokokendi/pyromod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `newmod-2.0/README.md` & `newmod-3.0/README.md`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/__init__.py` & `newmod-3.0/newmod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "2.0"
+__version__ = "3.0"
```

### Comparing `newmod-2.0/newmod/filters/__init__.py` & `newmod-3.0/newmod/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/filters/filters.py` & `newmod-3.0/newmod/filters/filters.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/helpers/__init__.py` & `newmod-3.0/newmod/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/helpers/helpers.py` & `newmod-3.0/newmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/listen/__init__.py` & `newmod-3.0/newmod/listen/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/listen/listen.py` & `newmod-3.0/newmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/utils/__init__.py` & `newmod-3.0/newmod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod/utils/utils.py` & `newmod-3.0/newmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `newmod-2.0/newmod.egg-info/PKG-INFO` & `newmod-3.0/newmod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: newmod
-Version: 2.0
+Version: 3.0
 Summary: A monkeypatcher add-on for newgram
-Home-page: https://github.com/jokokendi/newmod
+Home-page: https://github.com/jokokendi/pyromod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `newmod-2.0/setup.py` & `newmod-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     name="newmod",
     version=version,
     author="Cezar H.",
     license="LGPLv3+",
     description="A monkeypatcher add-on for newgram",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/jokokendi/newmod",
+    url="https://github.com/jokokendi/pyromod",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

