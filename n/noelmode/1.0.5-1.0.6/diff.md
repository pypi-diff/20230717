# Comparing `tmp/noelmode-1.0.5.tar.gz` & `tmp/noelmode-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noelmode-1.0.5.tar", last modified: Mon Jul 17 03:36:16 2023, max compression
+gzip compressed data, was "noelmode-1.0.6.tar", last modified: Mon Jul 17 04:02:17 2023, max compression
```

## Comparing `noelmode-1.0.5.tar` & `noelmode-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.948681 noelmode-1.0.5/
--rw-rw-rw-   0        0        0    35821 2023-07-17 03:21:44.000000 noelmode-1.0.5/COPYING
--rw-rw-rw-   0        0        0     7815 2023-07-17 03:21:44.000000 noelmode-1.0.5/COPYING.lesser
--rw-rw-rw-   0        0        0       96 2023-07-17 03:21:44.000000 noelmode-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      754 2023-07-17 03:21:44.000000 noelmode-1.0.5/NOTICE
--rw-rw-rw-   0        0        0     8065 2023-07-17 03:36:16.945681 noelmode-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7212 2023-07-17 03:21:44.000000 noelmode-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.783425 noelmode-1.0.5/noelmode/
--rw-rw-rw-   0        0        0     1009 2023-07-17 03:36:13.000000 noelmode-1.0.5/noelmode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.852383 noelmode-1.0.5/noelmode/helpers/
--rw-rw-rw-   0        0        0      841 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/helpers/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.879721 noelmode-1.0.5/noelmode/listen/
--rw-rw-rw-   0        0        0      830 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/listen/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/listen/listen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.910705 noelmode-1.0.5/noelmode/nav/
--rw-rw-rw-   0        0        0      800 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/nav/__init__.py
--rw-rw-rw-   0        0        0     3371 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/nav/pagination.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.941686 noelmode-1.0.5/noelmode/utils/
--rw-rw-rw-   0        0        0      820 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/utils/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-17 03:21:44.000000 noelmode-1.0.5/noelmode/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:36:16.829397 noelmode-1.0.5/noelmode.egg-info/
--rw-rw-rw-   0        0        0     8065 2023-07-17 03:36:16.000000 noelmode-1.0.5/noelmode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-07-17 03:36:16.000000 noelmode-1.0.5/noelmode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:36:16.000000 noelmode-1.0.5/noelmode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-17 03:36:16.000000 noelmode-1.0.5/noelmode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 03:36:16.000000 noelmode-1.0.5/noelmode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       32 2023-07-17 03:21:44.000000 noelmode-1.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 03:36:16.949679 noelmode-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-07-17 03:36:13.000000 noelmode-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.054473 noelmode-1.0.6/
+-rw-rw-rw-   0        0        0    35821 2023-07-17 03:21:44.000000 noelmode-1.0.6/COPYING
+-rw-rw-rw-   0        0        0     7815 2023-07-17 03:21:44.000000 noelmode-1.0.6/COPYING.lesser
+-rw-rw-rw-   0        0        0       96 2023-07-17 03:21:44.000000 noelmode-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      754 2023-07-17 03:21:44.000000 noelmode-1.0.6/NOTICE
+-rw-rw-rw-   0        0        0     8089 2023-07-17 04:02:17.052473 noelmode-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7212 2023-07-17 03:21:44.000000 noelmode-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:16.987515 noelmode-1.0.6/noelmode/
+-rw-rw-rw-   0        0        0     1049 2023-07-17 04:02:06.000000 noelmode-1.0.6/noelmode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.026492 noelmode-1.0.6/noelmode/helpers/
+-rw-rw-rw-   0        0        0      841 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2126 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.040480 noelmode-1.0.6/noelmode/listen/
+-rw-rw-rw-   0        0        0      831 2023-07-17 04:02:06.000000 noelmode-1.0.6/noelmode/listen/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/listen/listen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.045478 noelmode-1.0.6/noelmode/nav/
+-rw-rw-rw-   0        0        0      800 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/nav/__init__.py
+-rw-rw-rw-   0        0        0     3371 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/nav/pagination.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.050476 noelmode-1.0.6/noelmode/utils/
+-rw-rw-rw-   0        0        0      820 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/utils/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-17 03:21:44.000000 noelmode-1.0.6/noelmode/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:02:17.022499 noelmode-1.0.6/noelmode.egg-info/
+-rw-rw-rw-   0        0        0     8089 2023-07-17 04:02:16.000000 noelmode-1.0.6/noelmode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-07-17 04:02:16.000000 noelmode-1.0.6/noelmode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 04:02:16.000000 noelmode-1.0.6/noelmode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-17 04:02:16.000000 noelmode-1.0.6/noelmode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 04:02:16.000000 noelmode-1.0.6/noelmode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       32 2023-07-17 03:21:44.000000 noelmode-1.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 04:02:17.054473 noelmode-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2023-07-17 04:02:06.000000 noelmode-1.0.6/setup.py
```

### Comparing `noelmode-1.0.5/COPYING` & `noelmode-1.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/COPYING.lesser` & `noelmode-1.0.6/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/NOTICE` & `noelmode-1.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/PKG-INFO` & `noelmode-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.5
+Version: 1.0.6
 Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/xmode
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.5.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.6.zip
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # noelmode
 [![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Noelmodechat)
```

### Comparing `noelmode-1.0.5/README.md` & `noelmode-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/__init__.py` & `noelmode-1.0.6/noelmode/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with noelmode.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from noelmode.listen import *
+from noelmode.listen.listen import Client, Chat, MessageHandler, User
 from noelmode.utils import NoelmodConfig
 
 
 __copyright__ = "Copyright (C) 2022-present Noel <https://github.com/jokokendi>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

### Comparing `noelmode-1.0.5/noelmode/helpers/__init__.py` & `noelmode-1.0.6/noelmode/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/helpers/helpers.py` & `noelmode-1.0.6/noelmode/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/listen/__init__.py` & `noelmode-1.0.6/noelmode/nav/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,9 +13,8 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with noelmode.  If not, see <https://www.gnu.org/licenses/>.
 """
-
-from noelmode.listen import Client, MessageHandler, Chat, User
+from .pagination import Pagination
```

### Comparing `noelmode-1.0.5/noelmode/listen/listen.py` & `noelmode-1.0.6/noelmode/listen/listen.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/nav/__init__.py` & `noelmode-1.0.6/noelmode/listen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with noelmode.  If not, see <https://www.gnu.org/licenses/>.
 """
-from .pagination import Pagination
+
+#from noelmode.listen import Client, MessageHandler, Chat, User
```

### Comparing `noelmode-1.0.5/noelmode/nav/pagination.py` & `noelmode-1.0.6/noelmode/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/utils/__init__.py` & `noelmode-1.0.6/noelmode/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode/utils/utils.py` & `noelmode-1.0.6/noelmode/utils/utils.py`

 * *Files identical despite different names*

### Comparing `noelmode-1.0.5/noelmode.egg-info/PKG-INFO` & `noelmode-1.0.6/noelmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: noelmode
-Version: 1.0.5
+Version: 1.0.6
 Summary: Pyromod Custom, Experimental Noel
 Home-page: https://github.com/jokokendi/xmode
-Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.5.zip
+Download-URL: https://github.com/jokokendi/xmode/archive/v1.0.6.zip
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # noelmode
 [![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/Noelmodechat)
```

### Comparing `noelmode-1.0.5/setup.py` & `noelmode-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     download_url='https://github.com/jokokendi/xmode/archive/v{}.zip'.format(
         version
     ),
     license='GPLv3',
 
     packages=find_packages(),
     install_requires=requirements,
-    
+    python_requires="~=3.7",
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

