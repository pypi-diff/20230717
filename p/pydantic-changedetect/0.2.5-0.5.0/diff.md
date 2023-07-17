# Comparing `tmp/pydantic_changedetect-0.2.5.tar.gz` & `tmp/pydantic_changedetect-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_changedetect-0.2.5.tar", max compression
+gzip compressed data, was "pydantic_changedetect-0.5.0.tar", max compression
```

## Comparing `pydantic_changedetect-0.2.5.tar` & `pydantic_changedetect-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1078 2022-09-10 19:58:20.449223 pydantic_changedetect-0.2.5/LICENSE
--rw-r--r--   0        0        0     2600 2022-09-09 17:12:19.291926 pydantic_changedetect-0.2.5/README.md
--rw-r--r--   0        0        0       47 2022-08-31 20:08:26.918750 pydantic_changedetect-0.2.5/pydantic_changedetect/__init__.py
--rw-r--r--   0        0        0    11465 2022-09-10 15:38:40.400349 pydantic_changedetect-0.2.5/pydantic_changedetect/changedetect.py
--rw-r--r--   0        0        0        0 2022-09-23 05:50:27.111492 pydantic_changedetect-0.2.5/pydantic_changedetect/py.typed
--rw-r--r--   0        0        0     1172 2022-09-10 15:38:02.543053 pydantic_changedetect-0.2.5/pydantic_changedetect/utils.py
--rw-r--r--   0        0        0      882 2023-03-08 13:43:04.841424 pydantic_changedetect-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 pydantic_changedetect-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-17 07:40:50.942068 pydantic_changedetect-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2827 2023-07-17 07:38:10.198156 pydantic_changedetect-0.5.0/README.md
+-rw-r--r--   0        0        0       47 2022-08-31 20:08:26.918750 pydantic_changedetect-0.5.0/pydantic_changedetect/__init__.py
+-rw-r--r--   0        0        0     1232 2023-07-16 18:05:16.681505 pydantic_changedetect-0.5.0/pydantic_changedetect/_compat.py
+-rw-r--r--   0        0        0    21933 2023-07-17 07:36:59.214165 pydantic_changedetect-0.5.0/pydantic_changedetect/changedetect.py
+-rw-r--r--   0        0        0        0 2022-09-23 05:50:27.111492 pydantic_changedetect-0.5.0/pydantic_changedetect/py.typed
+-rw-r--r--   0        0        0     2621 2023-07-17 07:35:19.623327 pydantic_changedetect-0.5.0/pydantic_changedetect/utils.py
+-rw-r--r--   0        0        0      906 2023-07-17 07:41:48.213670 pydantic_changedetect-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 pydantic_changedetect-0.5.0/PKG-INFO
```

### Comparing `pydantic_changedetect-0.2.5/LICENSE` & `pydantic_changedetect-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
-
```

### Comparing `pydantic_changedetect-0.2.5/README.md` & `pydantic_changedetect-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
+**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
 to any pydantic models. Changes will be detected and stored after the model
 was constructed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic_changedetect-0.2.5/PKG-INFO` & `pydantic_changedetect-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: pydantic-changedetect
-Version: 0.2.5
+Version: 0.5.0
 Summary: Extend pydantic models to also detect and record changes made to the model attributes.
 Home-page: https://github.com/team23/pydantic-changedetect
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.1.0)
 Project-URL: Repository, https://github.com/team23/pydantic-changedetect
 Description-Content-Type: text/markdown
 
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
+**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
 to any pydantic models. Changes will be detected and stored after the model
 was constructed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

