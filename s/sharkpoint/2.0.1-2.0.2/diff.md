# Comparing `tmp/sharkpoint-2.0.1.tar.gz` & `tmp/sharkpoint-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharkpoint-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sharkpoint-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sharkpoint-2.0.1.tar` & `sharkpoint-2.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2023-07-16 17:27:15.449178 sharkpoint-2.0.1/LICENSE
--rw-r--r--   0        0        0      508 2023-07-16 17:27:15.450181 sharkpoint-2.0.1/README.md
--rw-r--r--   0        0        0      966 2023-07-17 03:06:22.848343 sharkpoint-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      502 2023-07-17 01:11:00.940041 sharkpoint-2.0.1/src/sharkpoint/__init__.py
--rw-r--r--   0        0        0     2832 2023-07-16 17:27:15.451182 sharkpoint-2.0.1/src/sharkpoint/sharepoint.py
--rw-r--r--   0        0        0     6704 2023-07-17 03:03:58.414627 sharkpoint-2.0.1/src/sharkpoint/sharepoint_file.py
--rw-r--r--   0        0        0     8581 2023-07-17 01:19:57.102920 sharkpoint-2.0.1/src/sharkpoint/sharepoint_site.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-2.0.2/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-2.0.2/README.md
+-rw-r--r--   0        0        0      966 2023-07-17 13:31:14.389925 sharkpoint-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-07-17 12:24:18.004073 sharkpoint-2.0.2/src/sharkpoint/__init__.py
+-rw-r--r--   0        0        0     2832 2023-07-14 15:01:59.312373 sharkpoint-2.0.2/src/sharkpoint/sharepoint.py
+-rw-r--r--   0        0        0     9395 2023-07-17 13:28:19.415931 sharkpoint-2.0.2/src/sharkpoint/sharepoint_file.py
+-rw-r--r--   0        0        0     8611 2023-07-17 12:24:18.005070 sharkpoint-2.0.2/src/sharkpoint/sharepoint_site.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.2/PKG-INFO
```

### Comparing `sharkpoint-2.0.1/LICENSE` & `sharkpoint-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sharkpoint-2.0.1/pyproject.toml` & `sharkpoint-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sharkpoint"
-version = "2.0.1"
+version = "2.0.2"
 description = "A small Pythonic library for interacting with SharePoint document libraries"
 authors = [
   { name = "TheOtherOne" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `sharkpoint-2.0.1/src/sharkpoint/sharepoint.py` & `sharkpoint-2.0.2/src/sharkpoint/sharepoint.py`

 * *Files identical despite different names*

### Comparing `sharkpoint-2.0.1/src/sharkpoint/sharepoint_file.py` & `sharkpoint-2.0.2/src/sharkpoint/sharepoint_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import io
 from types import TracebackType
 import requests
 
 
 class SharepointBytesFile(io.BytesIO):
     """
-    SharepointFile(header, sharepoint_site, filepath, checkout)
+    SharepointBytesFile(header, sharepoint_site, filepath, checkout)
 
-    A file-like class used to represent a SharePoint file using the SharePoint REST API v1.
+    A file-like class used to represent a SharePoint binary file using the SharePoint REST API v1.
 
     Methods
     -------
     check_back_in()
         Manually check a file into SharePoint and remove the file lock
     """
 
@@ -48,69 +48,115 @@
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckOut()"
             requests.post(api_url, headers=self._header)
 
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/$value"
         file = requests.get(api_url, headers=self._header)
         return file.content
-
-    def write(self, data):
-        if self._mode not in ("wb", "w+b", "r+b"):
+    
+    def read(self, size: int = -1) -> bytes:
+        if not self.readable():
+            raise IOError("File not open in read mode.")
+        return super().read(size)
+    
+    def write(self, bytes):
+        if not self.writable():
             raise IOError("File not open in write mode.")
-        super().write(data)
+        return super().write(bytes)
+    
+    def truncate(self, __size: int | None = ...) -> int:
+            if not self.seekable():
+                raise IOError("File not open in seekable mode.")
+            return super().truncate(__size)
+    
+    def readline(self, size: int = -1) -> str:
+        if not self.readable():
+            raise IOError("File not open in read mode.")
+        return super().readline(size)
+    
+    def readlines(self, size: int = -1) -> list[str]:
+        if not self.readable():
+            raise IOError("File not open in read mode.")
+        return super().readlines(size)
+    
+    def seek(self, cookie: int, whence: int = 0) -> int:
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().seek(cookie, whence)
+    
+    def tell(self) -> int:
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().tell()
+    
 
     def flush(self):
-        if self._mode not in ("wb", "w+b", "r+b"):
+        if not self.writable():
             raise IOError("File not open in write mode.")
         super().flush()
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files/add(url='{self._filename}', overwrite=true)"
 
         file_size = len(super().getvalue())
         post_request = {
             "Content-Length": str(file_size),
             "X-HTTP-Method": "PUT",
         }
 
         post_request.update(self._header)
         file_content = super().getvalue()
         requests.put(api_url, data=file_content, headers=post_request)
-
-    def read(self, size=-1):
-        if self._mode not in ("rb", "r+b", "w+b"):
-            raise IOError("File not open in read mode.")
-        return super().read(size)
-
+            
     def check_back_in(self):
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckIn(comment='Comment',checkintype=0)"
             requests.post(api_url, headers=self._header)
 
     def close(self):
         self.check_back_in()
-        if self._mode in ("wb", "w+b", "r+b"):
+        
+        if self.writable():
             self.flush()
+        
         super().close()
+    
+    def readable(self) -> bool:
+        if self._mode != "wb":
+            return True
+        else:
+            return False
 
+    def writable(self) -> bool:
+        if self._mode != "rb":
+            return True
+        else:
+            return False
+    
+    def seekable(self) -> bool:
+        if "+" in self._mode:
+            return True
+        else:
+            return False
+    
     def __enter__(self):
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         super().__exit__(exc_type, exc_val, exc_tb)
 
 
 class SharepointTextFile(io.StringIO):
     """
-    SharepointFile(header, sharepoint_site, filepath, checkout)
+    SharepointTextFile(header, sharepoint_site, filepath, checkout)
 
-    A file-like class used to represent a SharePoint file using the SharePoint REST API v1.
+    A file-like class used to represent a SharePoint text file using the SharePoint REST API v1.
 
     Methods
     -------
     check_back_in()
         Manually check a file into SharePoint and remove the file lock
     """
 
@@ -146,21 +192,16 @@
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckOut()"
             requests.post(api_url, headers=self._header)
 
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/$value"
         file = requests.get(api_url, headers=self._header)
         return file.content
 
-    def write(self, data):
-        if self._mode not in ("w", "w+", "r+"):
-            raise IOError("File not open in write mode.")
-        super().write(data)
-
     def flush(self):
-        if self._mode not in ("w", "w+", "r+"):
+        if not self.writable():
             raise IOError("File not open in write mode.")
         super().flush()
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files/add(url='{self._filename}', overwrite=true)"
 
         file_size = len(super().getvalue().encode())
         post_request = {
             "Content-Length": str(file_size),
@@ -168,32 +209,81 @@
         }
 
         post_request.update(self._header)
         file_content = super().getvalue().encode()
         requests.put(api_url, data=file_content, headers=post_request)
 
     def read(self, size=-1):
-        if self._mode not in ("r", "r+", "w+"):
+        if not self.readable():
             raise IOError("File not open in read mode.")
         return super().read(size)
+    
+    def write(self, bytes):
+        if not self.writable():
+            raise IOError("File not open in write mode.")
+        return super().write(bytes)
+    
+    def truncate(self, __size: int | None = ...) -> int:
+            if not self.seekable():
+                raise IOError("File not open in seekable mode.")
+            return super().truncate(__size)
+    
+    def readline(self, size: int = -1) -> str:
+        if not self.readable():
+            raise IOError("File not open in read mode.")
+        return super().readline(size)
+    
+    def readlines(self, size: int = -1) -> list[str]:
+        if not self.readable():
+            raise IOError("File not open in read mode.")
+        return super().readlines(size)
+    
+    def seek(self, cookie: int, whence: int = 0) -> int:
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().seek(cookie, whence)
+    
+    def tell(self) -> int:
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().tell()
 
     def check_back_in(self):
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckIn(comment='Comment',checkintype=0)"
             requests.post(api_url, headers=self._header)
 
     def close(self):
         self.check_back_in()
-        if self._mode in ("w", "w+", "r+"):
+        if self.writable():
             self.flush()
         super().close()
+    
+    def readable(self) -> bool:
+        if self._mode != "w":
+            return True
+        else:
+            return False
+
+    def writable(self) -> bool:
+        if self._mode != "r":
+            return True
+        else:
+            return False
+    
+    def seekable(self) -> bool:
+        if "+" in self._mode:
+            return True
+        else:
+            return False
 
     def __enter__(self):
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        super().__exit__(exc_type, exc_val, exc_tb)
+        super().__exit__(exc_type, exc_val, exc_tb)
+
```

### Comparing `sharkpoint-2.0.1/src/sharkpoint/sharepoint_site.py` & `sharkpoint-2.0.2/src/sharkpoint/sharepoint_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         if "error" in request:
             error_code = request["error"]["code"]
             if error_code == "-2130247139, Microsoft.SharePoint.SPException":
                 raise FileNotFoundError(request["error"]["message"]["value"])
             else:
                 raise Exception(request["error"]["message"]["value"])
 
-    def open(self, filepath: str, checkout: bool = False, mode: str = "r+b"):
+    def open(self, filepath: str, mode: str = "r", checkout: bool = False):
         """Open a file from a SharePoint document library and return a file-like object.
 
         Parameters
         ----------
         filepath : str
             The path of the file to return, relative to the site as a whole. File paths are UNIX-like.
         checkout : bool
@@ -173,15 +173,17 @@
         Returns
         ------
         SharepointFile
             File-like object.
         """
         mode = mode.replace("t", "")
         if mode not in ("w", "w+", "wb", "w+b", "r", "r+", "rb", "r+b"):
-            raise ValueError(f"Invalid mode. Supported modes are 'r', 'r+', 'w', 'w+', 'rb', 'wb', 'r+b', 'w+b'.")
+            raise ValueError(
+                f"Invalid mode. Supported modes are 'r', 'r+', 'w', 'w+', 'rb', 'wb', 'r+b', 'w+b'."
+            )
         if "a" in mode:
             raise NotImplementedError()
         elif "b" in mode:
             return sharepoint_file.SharepointBytesFile(
                 header=self._header,
                 sharepoint_site=self._site_url,
                 filepath=filepath,
```

### Comparing `sharkpoint-2.0.1/PKG-INFO` & `sharkpoint-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharkpoint
-Version: 2.0.1
+Version: 2.0.2
 Summary: A small Pythonic library for interacting with SharePoint document libraries
 Author: TheOtherOne
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

