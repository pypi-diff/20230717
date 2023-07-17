# Comparing `tmp/mortardata-0.1.1.tar.gz` & `tmp/mortardata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mortardata-0.1.1.tar", max compression
+gzip compressed data, was "mortardata-0.1.2.tar", max compression
```

## Comparing `mortardata-0.1.1.tar` & `mortardata-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1370 2023-07-16 20:26:19.400822 mortardata-0.1.1/README.md
--rw-r--r--   0        0        0     5742 2023-07-17 03:07:05.930183 mortardata-0.1.1/mortardata/__init__.py
--rw-r--r--   0        0        0      442 2023-07-17 03:24:43.619004 mortardata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 mortardata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1370 2023-07-16 20:26:19.400822 mortardata-0.1.2/README.md
+-rw-r--r--   0        0        0     5743 2023-07-17 03:27:49.132559 mortardata-0.1.2/mortardata/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-17 03:27:52.568588 mortardata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 mortardata-0.1.2/PKG-INFO
```

### Comparing `mortardata-0.1.1/README.md` & `mortardata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mortardata-0.1.1/mortardata/__init__.py` & `mortardata-0.1.2/mortardata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             return res is not None
         except RuntimeError:
             return False
 
     def sparql(self, query):
         res = requests.post(self._sparql_endpoint, data=query)
         if not res.ok:
-            raise Exception(res.json())
+            raise Exception(res.content)
         b = io.BytesIO(lzma.decompress(base64.urlsafe_b64decode(res.content)))
         res = JSONResultParser().parse(b)
         df = pd.DataFrame.from_records(list(res), columns=[str(c) for c in res.vars])
         return df
 
     def _to_batches(self, sparql, sites=None, start=None, end=None, limit=None):
         res = self.sparql(sparql)
```

### Comparing `mortardata-0.1.1/PKG-INFO` & `mortardata-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mortardata
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: BSD-3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

