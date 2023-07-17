# Comparing `tmp/sharkpoint-1.1.0.tar.gz` & `tmp/sharkpoint-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharkpoint-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sharkpoint-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sharkpoint-1.1.0.tar` & `sharkpoint-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-1.1.0/LICENSE
--rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-1.1.0/README.md
--rw-r--r--   0        0        0      966 2023-07-14 15:13:47.576074 sharkpoint-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      456 2023-07-14 15:01:59.270829 sharkpoint-1.1.0/src/sharkpoint/__init__.py
--rw-r--r--   0        0        0     2832 2023-07-14 15:01:59.312373 sharkpoint-1.1.0/src/sharkpoint/sharepoint.py
--rw-r--r--   0        0        0     2437 2023-07-14 15:01:59.309381 sharkpoint-1.1.0/src/sharkpoint/sharepoint_file.py
--rw-r--r--   0        0        0     7810 2023-07-14 15:01:59.383631 sharkpoint-1.1.0/src/sharkpoint/sharepoint_site.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-16 17:27:15.449178 sharkpoint-2.0.0/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-16 17:27:15.450181 sharkpoint-2.0.0/README.md
+-rw-r--r--   0        0        0      966 2023-07-17 01:13:59.596232 sharkpoint-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-07-17 01:11:00.940041 sharkpoint-2.0.0/src/sharkpoint/__init__.py
+-rw-r--r--   0        0        0     2832 2023-07-16 17:27:15.451182 sharkpoint-2.0.0/src/sharkpoint/sharepoint.py
+-rw-r--r--   0        0        0     6709 2023-07-17 01:11:01.081040 sharkpoint-2.0.0/src/sharkpoint/sharepoint_file.py
+-rw-r--r--   0        0        0     8393 2023-07-17 01:11:03.425970 sharkpoint-2.0.0/src/sharkpoint/sharepoint_site.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.0/PKG-INFO
```

### Comparing `sharkpoint-1.1.0/LICENSE` & `sharkpoint-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharkpoint-1.1.0/pyproject.toml` & `sharkpoint-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sharkpoint"
-version = "1.1.0"
+version = "2.0.0"
 description = "A small Pythonic library for interacting with SharePoint document libraries"
 authors = [
   { name = "TheOtherOne" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `sharkpoint-1.1.0/src/sharkpoint/sharepoint.py` & `sharkpoint-2.0.0/src/sharkpoint/sharepoint.py`

 * *Files identical despite different names*

### Comparing `sharkpoint-1.1.0/src/sharkpoint/sharepoint_site.py` & `sharkpoint-2.0.0/src/sharkpoint/sharepoint_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 from . import sharepoint_file
 
 
 class SharepointSite:
     """
-    SharePointSite(sharepoint_site_name, sharepoint_site_url, sharepoint_base_url, header)
+    SharePointSite(sharepoint_site_url, sharepoint_base_url, header)
 
     A class used to represent a SharePoint site using the SharePoint REST API v1.
     ...
 
     Parameters
     ----------
     sharepoint_site_url : str
@@ -17,20 +17,22 @@
     sharepoint_base_url : str
         The URL of the Sharepoint instance
     header : dict
         The header for requests made to the API containing the Bearer token
 
     Attributes
     ----------
-    site_name : str
+    name : str
         The user-facing name of the Sharepoint site
     description : str
         The description of the Sharepoint site
-    subsites : dict
+    subsites : list
         A list of dicts of Sharepoint subsites
+    libraries : list
+        A list of strings of Sharepoint document library names
 
     Methods
     -------
     listdir(path)
         Returns a list of directories in a document library
     mkdir(path)
         Creates a new directory in a document library
@@ -45,50 +47,51 @@
         sharepoint_site_url: str,
         sharepoint_base_url: str,
         header,
     ) -> None:
         self._site_url = sharepoint_site_url
         self._base_url = sharepoint_base_url
         self._header = header
-        self._libraries = self._get_libraries()
 
-    def _get_libraries(self):
+    @property
+    def libraries(self):
         api_url = f"{self._site_url}/_api/web/lists?$select=Title,ServerRelativeUrl&$filter=BaseTemplate eq 101 and hidden eq false&$expand=RootFolder"
         request = requests.get(api_url, headers=self._header)
         request = json.loads(request.content)
 
         request = request["d"]["results"]
-        libraries = {}
-
-        for library in request:
-            library_name = library["RootFolder"]["Name"]
-            library_path = library["RootFolder"]["ServerRelativeUrl"]
-            libraries[library_name] = library_path
+        libraries = [library["RootFolder"]["Name"] for library in request]
 
         return libraries
 
     def listdir(self, path: str):
         """List all files in a directory on a SharePoint document library.
 
         Parameters
         ----------
         path : str
             The path of the directory to search, relative to the site as a whole. File paths are UNIX-like.
+
         Raises
         ------
         FileNotFoundError
             If the document library does not exist or if a nonexistent folder is searched.
         Exception
             If an API error has occured that is not otherwise caught.
+
+        Returns
+        -------
+        list
+            List of files and directories
         """
 
         path_list = path.split("/")
         path_list = list(filter(None, path_list))
 
-        if path_list[0] not in self._libraries:
+        if path_list[0] not in self.libraries:
             raise FileNotFoundError(f"Document Library {path_list[0]} Not Found.")
 
         api_url = f"{self._site_url}/_api/web/GetFolderByServerRelativeUrl('{'/'.join(path_list)}')?$expand=Folders,Files"
         request = requests.get(api_url, headers=self._header)
         request = json.loads(request.content)
 
         if "error" in request:
@@ -113,28 +116,29 @@
     def mkdir(self, path: str):
         """Create a new directory on a SharePoint document library.
 
         Parameters
         ----------
         path : str
             The path of the directory to create, relative to the site as a whole. File paths are UNIX-like.
+
         Raises
         ------
         FileExistsError
             If the folder already exists.
         FileNotFoundError
             If the document library does not exist or if a subfolder is attempted to be made in a nonexistent folder.
         Exception
             If an API error has occured that is not otherwise caught.
         """
 
         path_list = path.split("/")
         path_list = list(filter(None, path_list))
 
-        if path_list[0] not in self._libraries:
+        if path_list[0] not in self.libraries:
             raise FileNotFoundError(f"Document Library {path_list[0]} not found.")
 
         if path_list[-1] in self.listdir("/".join(path_list[:-1])):
             raise FileExistsError(f"Folder {path_list[-1]} exists.")
 
         api_url = f"{self._site_url}/_api/web/folders"
         payload = json.dumps(
@@ -150,38 +154,54 @@
         if "error" in request:
             error_code = request["error"]["code"]
             if error_code == "-2130247139, Microsoft.SharePoint.SPException":
                 raise FileNotFoundError(request["error"]["message"]["value"])
             else:
                 raise Exception(request["error"]["message"]["value"])
 
-    def open(self, filepath: str, checkout: bool = False):
+    def open(self, filepath: str, checkout: bool = False, mode: str = "r+b"):
         """Open a file from a SharePoint document library and return a file-like object.
 
         Parameters
         ----------
         filepath : str
             The path of the file to return, relative to the site as a whole. File paths are UNIX-like.
         checkout : bool
             If True, the file will be checked out of Sharepoint and locked.
+        mode : str
+            File mode, append mode is not supported. Default is "r+b".
+
         Returns
         ------
         SharepointFile
             File-like object.
         """
+        mode = mode.replace("t", "")
 
-        return sharepoint_file.SharepointFile(
-            header=self._header,
-            sharepoint_site=self._site_url,
-            filepath=filepath,
-            checkout=checkout,
-        )
+        if "a" in mode:
+            raise NotImplementedError()
+        elif "b" in mode:
+            return sharepoint_file.SharepointBytesFile(
+                header=self._header,
+                sharepoint_site=self._site_url,
+                filepath=filepath,
+                checkout=checkout,
+                mode=mode,
+            )
+        else:
+            return sharepoint_file.SharepointTextFile(
+                header=self._header,
+                sharepoint_site=self._site_url,
+                filepath=filepath,
+                checkout=checkout,
+                mode=mode,
+            )
 
     @property
-    def site_name(self):
+    def name(self):
         api_url = f"{self._site_url}/_api/web/title"
         request = json.loads(requests.get(api_url, headers=self._header).content)
         return request["d"]["Title"]
 
     @property
     def description(self):
         api_url = f"{self._site_url}/_api/web/description"
@@ -200,28 +220,32 @@
                 "Site Name": x["Title"],
                 "Site Path": x["Url"],
             }
             sites.append(site_dict)
         return sites
 
     def get_subsite(self, site_name: str):
-        """Grab a subsite,
+        """Grab a subsite.
 
         Parameters
         ----------
         site_name : str
             The user-facing name of a SharePoint subsite
 
         Raises
         ------
         KeyError
             If the subsite does not exist.
+
+        Returns
+        ------
+        SharepointSite
         """
 
         site_url = next(
-            (item for item in self.sites if item["Site Name"] == site_name), None
+            (item for item in self.subsites if item["Site Name"] == site_name), None
         )
         if site_url is None:
             raise KeyError("Site not found.")
         else:
             site_url = site_url["Site Path"]
-        return SharepointSite(site_url, self.base_url, self._header)
+        return SharepointSite(site_url, self._base_url, self._header)
```

### Comparing `sharkpoint-1.1.0/PKG-INFO` & `sharkpoint-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharkpoint
-Version: 1.1.0
+Version: 2.0.0
 Summary: A small Pythonic library for interacting with SharePoint document libraries
 Author: TheOtherOne
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

