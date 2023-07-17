# Comparing `tmp/IngeoDash-0.0.21.tar.gz` & `tmp/IngeoDash-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.21.tar", last modified: Fri Jul 14 19:00:10 2023, max compression
+gzip compressed data, was "IngeoDash-0.0.22.tar", last modified: Mon Jul 17 13:44:11 2023, max compression
```

## Comparing `IngeoDash-0.0.21.tar` & `IngeoDash-0.0.22.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.346079 IngeoDash-0.0.21/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.739664 IngeoDash-0.0.22/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 13:44:11.000000 IngeoDash-0.0.22/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:44:11.743664 IngeoDash-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-17 13:42:24.000000 IngeoDash-0.0.22/setup.py
```

### Comparing `IngeoDash-0.0.21/IngeoDash/__init__.py` & `IngeoDash-0.0.22/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.21'
+__version__ = '0.0.22'
```

### Comparing `IngeoDash-0.0.21/IngeoDash/__main__.py` & `IngeoDash-0.0.22/IngeoDash/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import table_next, download, progress, update_row, download_component, table, table_component, table_prev
+from IngeoDash.app import table_next, progress, update_row, table, table_component, table_prev
+from IngeoDash.download import download, download_component
 from IngeoDash.upload import upload, upload_component
 from IngeoDash.config import CONFIG
 from dash import dcc, Output, Input, callback, Dash, State, ctx
 import dash_bootstrap_components as dbc
 
 
 @callback(
```

### Comparing `IngeoDash-0.0.21/IngeoDash/annotate.py` & `IngeoDash-0.0.22/IngeoDash/annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/IngeoDash/app.py` & `IngeoDash-0.0.22/IngeoDash/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import flip_label, label_column, store
 from IngeoDash.config import CONFIG, Config
-from dash import dcc, dash_table, html
-from dash.exceptions import PreventUpdate
+from dash import dash_table, html
 import dash_bootstrap_components as dbc
 from dash import Patch
 import string
 import json
 import numpy as np
 
 
@@ -126,25 +125,8 @@
     data = flip_label(mem, k=table['row'])
     patch = Patch()
     del patch[table['row']]
     patch.insert(table['row'], data)
     return patch
 
 
-def download(mem: Config, filename: str):
-    db = CONFIG.db[mem[mem.username]]
-    permanent = db.get(mem.permanent, list())
-    data = db.get(mem.data, list())
-    _ = [json.dumps(x) for x in permanent + data]
-    return dict(content='\n'.join(_), filename=filename)
-
-
-def download_component():
-    return dbc.InputGroup([dcc.Download(id=CONFIG.download),
-                           dbc.InputGroupText('Filename:'),
-                           dbc.Input(placeholder='output.json',
-                                     value='output.json',
-                                     type='text',
-                                     id=CONFIG.filename),
-                           dbc.Button('Download',
-                                      color='success',
-                                      id=CONFIG.save)])    
+
```

### Comparing `IngeoDash-0.0.21/IngeoDash/config.py` & `IngeoDash-0.0.22/IngeoDash/config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.0.22/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/IngeoDash/tests/test_app.py` & `IngeoDash-0.0.22/IngeoDash/tests/test_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import mock_data, table_next, download, progress, user, update_row, download_component, table_component, table_prev
+from IngeoDash.app import mock_data, table_next, progress, user, update_row, table_component, table_prev
 from IngeoDash.annotate import label_column
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
 from EvoMSA.tests.test_base import TWEETS
 
 
 def test_mock_data():
@@ -72,29 +72,14 @@
                              mem.data: [1] * 10,
                              mem.original: [2] * 10})
     table_prev(mem)    
     assert len(db[mem.permanent]) == 0
     assert len(db[mem.data]) ==  5 and db[mem.data] == [0] * 5
 
 
-def test_download(): 
-    D = mock_data()
-    mem = CONFIG({CONFIG.username: 'xxx'})
-    CONFIG.db['xxx'] = {mem.permanent: D[:11]}
-    _ = download(mem, 'tmp.json')
-    assert _['filename'] == 'tmp.json'
-    assert len(_['content'].split('\n')) == 11
-
-
-def test_download_component():
-    import dash_bootstrap_components as dbc
-    element = download_component()
-    assert isinstance(element, dbc.InputGroup)
-
-
 def test_table_component():
     import dash_bootstrap_components as dbc
     element = table_component()
     assert isinstance(element, dbc.Stack)
 
 
 def test_progress():
```

### Comparing `IngeoDash-0.0.21/IngeoDash/tests/test_config.py` & `IngeoDash-0.0.22/IngeoDash/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/IngeoDash/tests/test_upload.py` & `IngeoDash-0.0.22/IngeoDash/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/IngeoDash/upload.py` & `IngeoDash-0.0.22/IngeoDash/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,20 @@
     mem.text = text
     content_type, content_string = content.split(',')
     decoded = base64.b64decode(content_string)
     data = globals()[f'read_{type}'](mem, decoded)
     username, db = user(mem)
     labels = np.unique([x[mem.label_header]
                         for x in data if _label(x)])
+    permanent = db.get(mem.permanent, list())    
     if labels.shape[0] > 1:
         original = [x for x in data if not _label(x)]
-        permanent = db.get(mem.permanent, list())
         permanent.extend([x for x in data if _label(x)])
     else:
         original = data
-        permanent = []
     db[mem.data] = original[:mem.n_value]
     db[mem.permanent] = permanent
     db[mem.original] = original[mem.n_value:]
     mem.mem.update({mem.lang: lang,
                     mem.size: len(data),
                     mem.username: username})
     if call_next is not None:
```

### Comparing `IngeoDash-0.0.21/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.0.22/IngeoDash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.21
+Version: 0.0.22
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.21/LICENSE` & `IngeoDash-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/PKG-INFO` & `IngeoDash-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.21
+Version: 0.0.22
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.0.21/README.rst` & `IngeoDash-0.0.22/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.21/setup.py` & `IngeoDash-0.0.22/setup.py`

 * *Files identical despite different names*

