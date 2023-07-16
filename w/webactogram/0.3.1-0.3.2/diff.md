# Comparing `tmp/webactogram-0.3.1.tar.gz` & `tmp/webactogram-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webactogram-0.3.1.tar", last modified: Sun Jul 16 22:21:32 2023, max compression
+gzip compressed data, was "webactogram-0.3.2.tar", last modified: Sun Jul 16 22:29:44 2023, max compression
```

## Comparing `webactogram-0.3.1.tar` & `webactogram-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 22:21:32.201626 webactogram-0.3.1/
--rw-rw-rw-   0        0        0     1116 2023-07-16 16:40:22.000000 webactogram-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       95 2023-07-16 21:35:24.000000 webactogram-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4524 2023-07-16 22:19:05.000000 webactogram-0.3.1/Makefile
--rw-rw-rw-   0        0        0     7748 2023-07-16 22:21:32.200629 webactogram-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5482 2023-07-16 22:14:18.000000 webactogram-0.3.1/README.md
--rw-rw-rw-   0        0        0     4876 2023-07-16 22:21:04.000000 webactogram-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 22:21:32.201626 webactogram-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 22:21:32.181621 webactogram-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 22:21:32.189642 webactogram-0.3.1/src/webactogram/
--rw-rw-rw-   0        0        0      121 2023-07-16 21:37:55.000000 webactogram-0.3.1/src/webactogram/__init__.py
--rw-rw-rw-   0        0        0    28193 2023-07-16 22:06:00.000000 webactogram-0.3.1/src/webactogram/webactogram.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:21:32.198629 webactogram-0.3.1/src/webactogram.egg-info/
--rw-rw-rw-   0        0        0     7748 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       99 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 22:21:32.000000 webactogram-0.3.1/src/webactogram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 22:29:44.220374 webactogram-0.3.2/
+-rw-rw-rw-   0        0        0     1116 2023-07-16 16:40:22.000000 webactogram-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       95 2023-07-16 21:35:24.000000 webactogram-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4524 2023-07-16 22:19:05.000000 webactogram-0.3.2/Makefile
+-rw-rw-rw-   0        0        0     8191 2023-07-16 22:29:44.219375 webactogram-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5917 2023-07-16 22:28:22.000000 webactogram-0.3.2/README.md
+-rw-rw-rw-   0        0        0     4876 2023-07-16 22:27:36.000000 webactogram-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:29:44.220374 webactogram-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 22:29:44.199109 webactogram-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 22:29:44.210372 webactogram-0.3.2/src/webactogram/
+-rw-rw-rw-   0        0        0      121 2023-07-16 21:37:55.000000 webactogram-0.3.2/src/webactogram/__init__.py
+-rw-rw-rw-   0        0        0    28193 2023-07-16 22:06:00.000000 webactogram-0.3.2/src/webactogram/webactogram.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:29:44.218373 webactogram-0.3.2/src/webactogram.egg-info/
+-rw-rw-rw-   0        0        0     8191 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       99 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 22:29:44.000000 webactogram-0.3.2/src/webactogram.egg-info/top_level.txt
```

### Comparing `webactogram-0.3.1/LICENSE` & `webactogram-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webactogram-0.3.1/Makefile` & `webactogram-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `webactogram-0.3.1/PKG-INFO` & `webactogram-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webactogram
-Version: 0.3.1
+Version: 0.3.2
 Summary: Actogram from browsers history, may help to screen sleep-wake patterns & disorders!
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <LRQ3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Circadiaware/webactogram
 Project-URL: Documentation, https://github.com/Circadiaware/webactogram/blob/master/README.md
 Project-URL: Source, https://github.com/Circadiaware/webactogram
@@ -38,14 +38,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
 # WebActogram
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
+
 🌐🏃Actogram from browsers history, may help to retrospectively screen 🌙🛌sleep-wake patterns & disorders!
 
 ## Description
 Python 3 tool to generate a web actogram from web browsers history files.
 
 To screen sleep-wake patterns and disorders, all tools require that the user wear an actigraphic device or record themselves a sleep diary.
 
@@ -149,7 +151,13 @@
 
 MIT Public License.
 
 ## Similar projects
 
 Another project, inspired by this one, was written in Javascript using D3, but it cannot fetch browser's history: [Tylian's D3 Browser's History](https://web.archive.org/web/20221207124930/https://tylian.net/d3/history.html).
 How to generate the history.txt file ([source](https://www.reddit.com/r/N24/comments/hxve2w/comment/g30ve2y/?utm_source=share&utm_medium=web2x&context=3)): ```It's a dump of the timestamp column with some manual processing to divide every entry by 1000, since Firefox stores them as a nanosecond epoch for some reason..```
+
+[1]: https://img.shields.io/pypi/v/webactogram.svg
+[2]: https://pypi.org/project/webactogram
+[3]: https://img.shields.io/pypi/pyversions/webactogram.svg?logo=python&logoColor=white
+[4]: https://img.shields.io/pypi/l/webactogram.svg
+[5]: https://img.shields.io/pypi/dm/webactogram.svg?label=pypi%20downloads&logo=python&logoColor=white
```

### Comparing `webactogram-0.3.1/README.md` & `webactogram-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # WebActogram
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
+
 🌐🏃Actogram from browsers history, may help to retrospectively screen 🌙🛌sleep-wake patterns & disorders!
 
 ## Description
 Python 3 tool to generate a web actogram from web browsers history files.
 
 To screen sleep-wake patterns and disorders, all tools require that the user wear an actigraphic device or record themselves a sleep diary.
 
@@ -106,7 +108,13 @@
 
 MIT Public License.
 
 ## Similar projects
 
 Another project, inspired by this one, was written in Javascript using D3, but it cannot fetch browser's history: [Tylian's D3 Browser's History](https://web.archive.org/web/20221207124930/https://tylian.net/d3/history.html).
 How to generate the history.txt file ([source](https://www.reddit.com/r/N24/comments/hxve2w/comment/g30ve2y/?utm_source=share&utm_medium=web2x&context=3)): ```It's a dump of the timestamp column with some manual processing to divide every entry by 1000, since Firefox stores them as a nanosecond epoch for some reason..```
+
+[1]: https://img.shields.io/pypi/v/webactogram.svg
+[2]: https://pypi.org/project/webactogram
+[3]: https://img.shields.io/pypi/pyversions/webactogram.svg?logo=python&logoColor=white
+[4]: https://img.shields.io/pypi/l/webactogram.svg
+[5]: https://img.shields.io/pypi/dm/webactogram.svg?label=pypi%20downloads&logo=python&logoColor=white
```

### Comparing `webactogram-0.3.1/pyproject.toml` & `webactogram-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 # never uppercap requirements unless we have evidence it won't work https://iscinumpy.dev/post/bound-version-constraints/ 
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]  # beware if using setuptools: setup.py still gets executed, and even if pyproject.toml fields take precedence, if there is any code error in setup.py, building will fail!
 name = "webactogram"  # renamed from online-actogram according to PEP 423 https://peps.python.org/pep-0423/#pick-meaningful-names
-version = "0.3.1"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
+version = "0.3.2"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
 description = "Actogram from browsers history, may help to screen sleep-wake patterns & disorders!"
 authors = [
     {name = "Stephen Karl Larroque", email = "LRQ3000@gmail.com"},
     ]
 maintainers = [
     {name = "Stephen Karl Larroque", email = "LRQ3000@gmail.com"},
     ]
```

### Comparing `webactogram-0.3.1/src/webactogram/webactogram.py` & `webactogram-0.3.2/src/webactogram/webactogram.py`

 * *Files identical despite different names*

### Comparing `webactogram-0.3.1/src/webactogram.egg-info/PKG-INFO` & `webactogram-0.3.2/src/webactogram.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webactogram
-Version: 0.3.1
+Version: 0.3.2
 Summary: Actogram from browsers history, may help to screen sleep-wake patterns & disorders!
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <LRQ3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Circadiaware/webactogram
 Project-URL: Documentation, https://github.com/Circadiaware/webactogram/blob/master/README.md
 Project-URL: Source, https://github.com/Circadiaware/webactogram
@@ -38,14 +38,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
 # WebActogram
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
+
 🌐🏃Actogram from browsers history, may help to retrospectively screen 🌙🛌sleep-wake patterns & disorders!
 
 ## Description
 Python 3 tool to generate a web actogram from web browsers history files.
 
 To screen sleep-wake patterns and disorders, all tools require that the user wear an actigraphic device or record themselves a sleep diary.
 
@@ -149,7 +151,13 @@
 
 MIT Public License.
 
 ## Similar projects
 
 Another project, inspired by this one, was written in Javascript using D3, but it cannot fetch browser's history: [Tylian's D3 Browser's History](https://web.archive.org/web/20221207124930/https://tylian.net/d3/history.html).
 How to generate the history.txt file ([source](https://www.reddit.com/r/N24/comments/hxve2w/comment/g30ve2y/?utm_source=share&utm_medium=web2x&context=3)): ```It's a dump of the timestamp column with some manual processing to divide every entry by 1000, since Firefox stores them as a nanosecond epoch for some reason..```
+
+[1]: https://img.shields.io/pypi/v/webactogram.svg
+[2]: https://pypi.org/project/webactogram
+[3]: https://img.shields.io/pypi/pyversions/webactogram.svg?logo=python&logoColor=white
+[4]: https://img.shields.io/pypi/l/webactogram.svg
+[5]: https://img.shields.io/pypi/dm/webactogram.svg?label=pypi%20downloads&logo=python&logoColor=white
```

