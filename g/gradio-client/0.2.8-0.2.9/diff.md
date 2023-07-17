# Comparing `tmp/gradio_client-0.2.8.tar.gz` & `tmp/gradio_client-0.2.9.tar.gz`

## Comparing `gradio_client-0.2.8.tar` & `gradio_client-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.8/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.8/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/__init__.py
--rw-r--r--   0        0        0    48736 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/client.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/media_data.py
--rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/types.json
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/version.txt
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 gradio_client-0.2.8/.gitignore
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.9/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.9/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/__init__.py
+-rw-r--r--   0        0        0    48764 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/client.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/types.json
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/version.txt
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 gradio_client-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.9/PKG-INFO
```

### Comparing `gradio_client-0.2.8/README.md` & `gradio_client-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/gradio_client/client.py` & `gradio_client-0.2.9/gradio_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,15 +546,15 @@
             pass
 
     def _infer_fn_index(self, api_name: str | None, fn_index: int | None) -> int:
         inferred_fn_index = None
         if api_name is not None:
             for i, d in enumerate(self.config["dependencies"]):
                 config_api_name = d.get("api_name")
-                if config_api_name is None:
+                if config_api_name is None or config_api_name is False:
                     continue
                 if "/" + config_api_name == api_name:
                     inferred_fn_index = i
                     break
             else:
                 error_message = f"Cannot find a function with `api_name`: {api_name}."
                 if not api_name.startswith("/"):
```

### Comparing `gradio_client-0.2.8/gradio_client/documentation.py` & `gradio_client-0.2.9/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/gradio_client/media_data.py` & `gradio_client-0.2.9/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/gradio_client/serializing.py` & `gradio_client-0.2.9/gradio_client/serializing.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/gradio_client/types.json` & `gradio_client-0.2.9/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/gradio_client/utils.py` & `gradio_client-0.2.9/gradio_client/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/.gitignore` & `gradio_client-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/pyproject.toml` & `gradio_client-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.8/PKG-INFO` & `gradio_client-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

