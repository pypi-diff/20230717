# Comparing `tmp/sharkpoint-2.0.0.tar.gz` & `tmp/sharkpoint-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharkpoint-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sharkpoint-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sharkpoint-2.0.0.tar` & `sharkpoint-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2023-07-16 17:27:15.449178 sharkpoint-2.0.0/LICENSE
--rw-r--r--   0        0        0      508 2023-07-16 17:27:15.450181 sharkpoint-2.0.0/README.md
--rw-r--r--   0        0        0      966 2023-07-17 01:13:59.596232 sharkpoint-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-07-17 01:11:00.940041 sharkpoint-2.0.0/src/sharkpoint/__init__.py
--rw-r--r--   0        0        0     2832 2023-07-16 17:27:15.451182 sharkpoint-2.0.0/src/sharkpoint/sharepoint.py
--rw-r--r--   0        0        0     6709 2023-07-17 01:11:01.081040 sharkpoint-2.0.0/src/sharkpoint/sharepoint_file.py
--rw-r--r--   0        0        0     8393 2023-07-17 01:11:03.425970 sharkpoint-2.0.0/src/sharkpoint/sharepoint_site.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-16 17:27:15.449178 sharkpoint-2.0.1/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-16 17:27:15.450181 sharkpoint-2.0.1/README.md
+-rw-r--r--   0        0        0      966 2023-07-17 03:06:22.848343 sharkpoint-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-07-17 01:11:00.940041 sharkpoint-2.0.1/src/sharkpoint/__init__.py
+-rw-r--r--   0        0        0     2832 2023-07-16 17:27:15.451182 sharkpoint-2.0.1/src/sharkpoint/sharepoint.py
+-rw-r--r--   0        0        0     6704 2023-07-17 03:03:58.414627 sharkpoint-2.0.1/src/sharkpoint/sharepoint_file.py
+-rw-r--r--   0        0        0     8581 2023-07-17 01:19:57.102920 sharkpoint-2.0.1/src/sharkpoint/sharepoint_site.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.1/PKG-INFO
```

### Comparing `sharkpoint-2.0.0/LICENSE` & `sharkpoint-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sharkpoint-2.0.0/pyproject.toml` & `sharkpoint-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sharkpoint"
-version = "2.0.0"
+version = "2.0.1"
 description = "A small Pythonic library for interacting with SharePoint document libraries"
 authors = [
   { name = "TheOtherOne" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `sharkpoint-2.0.0/src/sharkpoint/sharepoint.py` & `sharkpoint-2.0.1/src/sharkpoint/sharepoint.py`

 * *Files identical despite different names*

### Comparing `sharkpoint-2.0.0/src/sharkpoint/sharepoint_file.py` & `sharkpoint-2.0.1/src/sharkpoint/sharepoint_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         }
 
         post_request.update(self._header)
         file_content = super().getvalue().encode()
         requests.put(api_url, data=file_content, headers=post_request)
 
     def read(self, size=-1):
-        if self._mode not in ("rb", "r+b", "w+b"):
+        if self._mode not in ("r", "r+", "w+"):
             raise IOError("File not open in read mode.")
         return super().read(size)
 
     def check_back_in(self):
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckIn(comment='Comment',checkintype=0)"
             requests.post(api_url, headers=self._header)
@@ -192,8 +192,8 @@
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        super().__exit__(exc_type, exc_val, exc_tb)
+        super().__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `sharkpoint-2.0.0/src/sharkpoint/sharepoint_site.py` & `sharkpoint-2.0.1/src/sharkpoint/sharepoint_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,15 +172,16 @@
 
         Returns
         ------
         SharepointFile
             File-like object.
         """
         mode = mode.replace("t", "")
-
+        if mode not in ("w", "w+", "wb", "w+b", "r", "r+", "rb", "r+b"):
+            raise ValueError(f"Invalid mode. Supported modes are 'r', 'r+', 'w', 'w+', 'rb', 'wb', 'r+b', 'w+b'.")
         if "a" in mode:
             raise NotImplementedError()
         elif "b" in mode:
             return sharepoint_file.SharepointBytesFile(
                 header=self._header,
                 sharepoint_site=self._site_url,
                 filepath=filepath,
```

### Comparing `sharkpoint-2.0.0/PKG-INFO` & `sharkpoint-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharkpoint
-Version: 2.0.0
+Version: 2.0.1
 Summary: A small Pythonic library for interacting with SharePoint document libraries
 Author: TheOtherOne
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

