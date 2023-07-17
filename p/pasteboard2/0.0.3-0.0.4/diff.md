# Comparing `tmp/pasteboard2-0.0.3.tar.gz` & `tmp/pasteboard2-0.0.4.tar.gz`

## Comparing `pasteboard2-0.0.3.tar` & `pasteboard2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/.idea/pasteboard.iml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/src/pasteboard2/__init__.py
--rwxr-xr-x   0        0        0     4157 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/src/pasteboard2/pasteboard2.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/tests/test_pasteboard2.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 pasteboard2-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/pasteboard.iml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/src/pasteboard2/__init__.py
+-rwxr-xr-x   0        0        0     4157 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/src/pasteboard2/pasteboard2.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/tests/test_pasteboard2.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/PKG-INFO
```

### Comparing `pasteboard2-0.0.3/src/pasteboard2/pasteboard2.py` & `pasteboard2-0.0.4/src/pasteboard2/pasteboard2.py`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.3/tests/test_pasteboard2.py` & `pasteboard2-0.0.4/tests/test_pasteboard2.py`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.3/.gitignore` & `pasteboard2-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.3/LICENSE.txt` & `pasteboard2-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.3/README.md` & `pasteboard2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.3/pyproject.toml` & `pasteboard2-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "pasteboard2"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Bernhard Wagner", email="pasteboard2@nosuch.biz" },
 ]
 description = "access macOS pasteboard"
 readme = "README.md"
 license = { file = "LICENSE.txt"}
 requires-python = ">=3.7"
@@ -15,13 +15,13 @@
 	"pyobjc",
 	"pytest",
 	"typer",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: MacOS :: MacOS X",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/bwagner/pasteboard2"
 "Bug Tracker" = "https://github.com/bwagner/pasteboard2/issues"
```

### Comparing `pasteboard2-0.0.3/PKG-INFO` & `pasteboard2-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasteboard2
-Version: 0.0.3
+Version: 0.0.4
 Summary: access macOS pasteboard
 Project-URL: Homepage, https://github.com/bwagner/pasteboard2
 Project-URL: Bug Tracker, https://github.com/bwagner/pasteboard2/issues
 Author-email: Bernhard Wagner <pasteboard2@nosuch.biz>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pyobjc
 Requires-Dist: pytest
 Requires-Dist: typer
 Description-Content-Type: text/markdown
```

