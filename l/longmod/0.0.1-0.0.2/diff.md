# Comparing `tmp/longmod-0.0.1.tar.gz` & `tmp/longmod-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longmod-0.0.1.tar", last modified: Mon Jul 17 16:19:35 2023, max compression
+gzip compressed data, was "longmod-0.0.2.tar", last modified: Mon Jul 17 16:23:49 2023, max compression
```

## Comparing `longmod-0.0.1.tar` & `longmod-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.131305 longmod-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 longmod-0.0.1/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 longmod-0.0.1/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 longmod-0.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3069 2023-07-17 16:19:35.131305 longmod-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 longmod-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.127304 longmod-0.0.1/longmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3069 2023-07-17 16:19:35.000000 longmod-0.0.1/longmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      424 2023-07-17 16:19:35.000000 longmod-0.0.1/longmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:19:35.000000 longmod-0.0.1/longmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:19:35.000000 longmod-0.0.1/longmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:19:35.000000 longmod-0.0.1/longmod.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.127304 longmod-0.0.1/newmod/
--rw-r--r--   0 root         (0) root         (0)      759 2023-07-17 16:19:01.000000 longmod-0.0.1/newmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.131305 longmod-0.0.1/newmod/filters/
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/filters/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.131305 longmod-0.0.1/newmod/helpers/
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.131305 longmod-0.0.1/newmod/listen/
--rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/listen/listen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:35.131305 longmod-0.0.1/newmod/utils/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 longmod-0.0.1/newmod/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:19:35.131305 longmod-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      909 2023-07-17 16:19:01.000000 longmod-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 16:13:17.000000 longmod-0.0.2/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 16:13:17.000000 longmod-0.0.2/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-17 16:13:17.000000 longmod-0.0.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-07-17 16:23:49.354646 longmod-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-17 16:13:17.000000 longmod-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/longmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-07-17 16:23:49.000000 longmod-0.0.2/longmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-17 16:23:49.000000 longmod-0.0.2/longmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:23:49.000000 longmod-0.0.2/longmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 16:23:49.000000 longmod-0.0.2/longmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 16:23:49.000000 longmod-0.0.2/longmod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/newmod/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-07-17 16:23:31.000000 longmod-0.0.2/newmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/newmod/filters/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/filters/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/newmod/helpers/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/newmod/listen/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/listen/listen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:23:49.354646 longmod-0.0.2/newmod/utils/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-17 16:13:17.000000 longmod-0.0.2/newmod/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:23:49.354646 longmod-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-17 16:23:31.000000 longmod-0.0.2/setup.py
```

### Comparing `longmod-0.0.1/COPYING` & `longmod-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/COPYING.lesser` & `longmod-0.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/NOTICE` & `longmod-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/PKG-INFO` & `longmod-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longmod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monkeypatcher add-on for newgram
 Home-page: https://github.com/jokokendi/pyromod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `longmod-0.0.1/README.md` & `longmod-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/longmod.egg-info/PKG-INFO` & `longmod-0.0.2/longmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longmod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monkeypatcher add-on for newgram
 Home-page: https://github.com/jokokendi/pyromod
 Author: Cezar H.
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `longmod-0.0.1/newmod/__init__.py` & `longmod-0.0.2/newmod/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with newmod.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `longmod-0.0.1/newmod/filters/__init__.py` & `longmod-0.0.2/newmod/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/filters/filters.py` & `longmod-0.0.2/newmod/filters/filters.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/helpers/__init__.py` & `longmod-0.0.2/newmod/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/helpers/helpers.py` & `longmod-0.0.2/newmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/listen/__init__.py` & `longmod-0.0.2/newmod/listen/__init__.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/listen/listen.py` & `longmod-0.0.2/newmod/listen/listen.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/utils/__init__.py` & `longmod-0.0.2/newmod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/newmod/utils/utils.py` & `longmod-0.0.2/newmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `longmod-0.0.1/setup.py` & `longmod-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re 
 import setuptools
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
     
-with open('requirements.txt') as fp:
-    requirements = [line.strip() for line in fp]
+with open("requirements.txt", encoding="utf-8") as r:
+    requirements = [i.strip() for i in r]
 
-with open('newmod/__init__.py') as fp:
+with open('newmod/__init__.py', "rt", encoding="utf8") as fp:
     version = re.search('__version__ = "(.+?)"', fp.read())[1]
 
 
 setuptools.setup(
     name="longmod",
     version=version,
     author="Cezar H.",
```

