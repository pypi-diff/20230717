# Comparing `tmp/modrinth-0.1.3.tar.gz` & `tmp/modrinth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modrinth-0.1.3.tar", last modified: Sat Aug 27 17:51:05 2022, max compression
+gzip compressed data, was "modrinth-0.1.5.tar", last modified: Sun Jul 16 22:28:34 2023, max compression
```

## Comparing `modrinth-0.1.3.tar` & `modrinth-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:51:05.871821 modrinth-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-08-27 17:51:05.871821 modrinth-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:51:05.871821 modrinth-0.1.3/modrinth/
--rw-r--r--   0 runner    (1001) docker     (121)    13595 2022-08-27 17:50:55.000000 modrinth-0.1.3/modrinth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 17:51:05.871821 modrinth-0.1.3/modrinth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-08-27 17:51:05.000000 modrinth-0.1.3/modrinth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-27 17:51:05.000000 modrinth-0.1.3/modrinth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 17:51:05.000000 modrinth-0.1.3/modrinth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-27 17:51:05.000000 modrinth-0.1.3/modrinth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-27 17:51:05.000000 modrinth-0.1.3/modrinth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-08-27 17:50:55.000000 modrinth-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 17:51:05.871821 modrinth-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:28:34.399990 modrinth-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-16 22:28:34.399990 modrinth-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:28:34.399990 modrinth-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-16 22:28:22.000000 modrinth-0.1.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-16 22:28:22.000000 modrinth-0.1.5/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:28:34.399990 modrinth-0.1.5/modrinth/
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-16 22:28:22.000000 modrinth-0.1.5/modrinth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:28:34.399990 modrinth-0.1.5/modrinth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-16 22:28:34.000000 modrinth-0.1.5/modrinth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-16 22:28:34.000000 modrinth-0.1.5/modrinth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:28:34.000000 modrinth-0.1.5/modrinth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 22:28:34.000000 modrinth-0.1.5/modrinth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 22:28:34.000000 modrinth-0.1.5/modrinth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-16 22:28:22.000000 modrinth-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 22:28:34.399990 modrinth-0.1.5/setup.cfg
```

### Comparing `modrinth-0.1.3/PKG-INFO` & `modrinth-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modrinth
-Version: 0.1.3
+Version: 0.1.5
 Summary:  Interact with Modrinth's Labrinth API through Python.
 Author-email: Beta Pictoris <beta@ozx.me>
 License: The MIT License (MIT)
         =====================
         
         Copyright © `2020` `Daniel`
         
@@ -37,23 +37,14 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Modrinth.py
 Interact with Modrinth's Labrinth API through Python. 
 
-## API Version
-
- Service              | Version
-----------------------|----------
- Modrinth.py version  | v0.1.3
- Labrinth API version | v2.4.4
-
-*Modrinth.py works on the latest Labrinth version!*
-
 ## To-do
  - [x] Search for projects
  - [x] (Un)follow projects
  - [x] Basic authentication
  - [ ] Documentation
  - [ ] Create and delete projects
  - [ ] Modify projects (PATCH requests to `/project/{id|slug}` and `/project/{id|slug}/gallery` requests)
@@ -62,15 +53,15 @@
  - [x] Get project versions
  - [x] Get project details
  - [ ] Create, modify, and delete projects (POST requests to `/version` and PATCH/DELETE to `/version/{id}`)
  - [x] Built-in function to get multiple versions
  - [ ] Upload files to version
  - [ ] Get a version from `sha1` or `sha512`
  - [ ] Delete a file from its hash (DELETE requests to `/version_file`)
- - [ ] Get latest project(s) version(s)
+ - [x] Get latest project(s) version(s)
  - [ ] Get project version from hash
  - [x] Read user(s) data
  - [ ] Delete and modify user data
  - [ ] Read team data 
  - [ ] Add users to teams
  - [ ] Join a team
  - [ ] Modify user roles/perms within a team
```

### Comparing `modrinth-0.1.3/modrinth/__init__.py` & `modrinth-0.1.5/modrinth/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 Modrinth.py - __init__.py 
 
 Developed by Beta Pictoris <beta@ozx.me>
 Modrinth Python API 
 '''
 
 import requests
+from warnings import warn
 
-__version__ = '0.1.3'
+__version__ = '0.1.5'
 
 
 class Users:
     '''
     User data includes their username, name, email, bio, etc. this class hold functions and objects that relate
     to authentication and user data.  
 
@@ -83,15 +84,15 @@
             self.downloads: int = data['downloads']
             self.followers: int = data['followers']
             self.categories: list = data['categories']
             self.versions: list = data['versions']
             self.iconURL: str = data['icon_url']
             self.issuesURL: str = data['issues_url']
             self.sourceURL: str = data['source_url']
-            self.wikiURL: int = data['wiki_url']
+            self.wikiURL: str = data['wiki_url']
             self.discordURL: str = data['discord_url']
             self.donationURLs: list = data['donation_urls']
             self.gallery: list = data['gallery']
 
         def toDict(self) -> dict:
             '''
             Convert the project object to a dictionary.
@@ -146,25 +147,31 @@
             '''
             Unfollow a project, given a user. 
             '''
             url = self.url + '/follow'
             headers = {'Authorization': user.token}
             requests.delete(url, headers=headers)
 
+        def getLatestVersion(self):
+            '''
+            Gets the latest version for the current project.
+            '''
+            return Versions.getLatestVersion(self)
+
         def getVersion(self, version):
             '''
             Shorthand for Versions.ModrinthVersion with no project argument.
             '''
             return Versions.ModrinthVersion(self, version=version)
 
         def getAllVersions(self):
             '''
             Get Versions.getVersions() for all versions found for the project. 
             '''
-            return Versions.getVersions(self.versions)
+            return Versions.getVersions(self, self.versions)
 
     def getProjects(ids: list) -> list:
         '''
         Get a list of projects, given a list of IDs.
         '''
         return [Projects.ModrinthProject(id) for id in ids]
 
@@ -285,19 +292,40 @@
             self.gameVersions: list = rJSON['game_versions']
             self.versionType:   str = rJSON['version_type']
             self.loaders:      list = rJSON['loaders']
             self.featured:     bool = rJSON['featured']
             self.changeLog:     str = rJSON['changelog']
             self.dependencies: list = rJSON['dependencies']
             self.changeLogURL:  str = rJSON['changelog_url']
+        
+        def getFiles(self, hash: str = 'sha1', primary: bool = True, optional: bool = True) -> str:
+            '''
+            Returns the file hashes of the version.
+            '''
+            files = []
+
+            if hash not in ['sha1', 'sha512']:
+                raise ValueError("hash must be either sha1 or sha512")
+            for file in self.files:
+                if file['primary'] and primary:
+                    files.append(file['hashes'][hash])
+                elif not file['primary'] and optional:
+                    files.append(file['hashes'][hash])
+            
+            return files
+
 
         def getPrimaryFile(self, hash: str = 'sha1') -> str:
             '''
             Returns the primary file hash of the version.
+
+            Deprecate: Use getFiles instead, getPrimaryFile may be removed in
+                       a future update.
             '''
+            warn("getPrimaryFile is deprecated, use getFiles instead.")
             if hash not in ['sha1', 'sha512']:
                 raise ValueError("hash must be either sha1 or sha512")
             for file in self.files:
                 if file['primary']:
                     return file['hashes'][hash]
             raise ValueError("No primary file found")
 
@@ -313,7 +341,13 @@
             raise ValueError("No download with that hash was found")
 
     def getVersions(project: Projects.ModrinthProject, ids: list) -> list:
         '''
         Get a list of versions, given a list of IDs.
         '''
         return [Versions.ModrinthVersion(project, id) for id in ids]
+    
+    def getLatestVersion(project: Projects.ModrinthProject) -> ModrinthVersion:
+        '''
+        Gets the latest version, given a project.
+        '''
+        return project.getAllVersions()[-1]
```

### Comparing `modrinth-0.1.3/modrinth.egg-info/PKG-INFO` & `modrinth-0.1.5/modrinth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modrinth
-Version: 0.1.3
+Version: 0.1.5
 Summary:  Interact with Modrinth's Labrinth API through Python.
 Author-email: Beta Pictoris <beta@ozx.me>
 License: The MIT License (MIT)
         =====================
         
         Copyright © `2020` `Daniel`
         
@@ -37,23 +37,14 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Modrinth.py
 Interact with Modrinth's Labrinth API through Python. 
 
-## API Version
-
- Service              | Version
-----------------------|----------
- Modrinth.py version  | v0.1.3
- Labrinth API version | v2.4.4
-
-*Modrinth.py works on the latest Labrinth version!*
-
 ## To-do
  - [x] Search for projects
  - [x] (Un)follow projects
  - [x] Basic authentication
  - [ ] Documentation
  - [ ] Create and delete projects
  - [ ] Modify projects (PATCH requests to `/project/{id|slug}` and `/project/{id|slug}/gallery` requests)
@@ -62,15 +53,15 @@
  - [x] Get project versions
  - [x] Get project details
  - [ ] Create, modify, and delete projects (POST requests to `/version` and PATCH/DELETE to `/version/{id}`)
  - [x] Built-in function to get multiple versions
  - [ ] Upload files to version
  - [ ] Get a version from `sha1` or `sha512`
  - [ ] Delete a file from its hash (DELETE requests to `/version_file`)
- - [ ] Get latest project(s) version(s)
+ - [x] Get latest project(s) version(s)
  - [ ] Get project version from hash
  - [x] Read user(s) data
  - [ ] Delete and modify user data
  - [ ] Read team data 
  - [ ] Add users to teams
  - [ ] Join a team
  - [ ] Modify user roles/perms within a team
```

### Comparing `modrinth-0.1.3/pyproject.toml` & `modrinth-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modrinth"
-version = "0.1.3"
+version = "0.1.5"
 description = " Interact with Modrinth's Labrinth API through Python."
 readme = "docs/readme.md"
 authors = [{ name = "Beta Pictoris", email = "beta@ozx.me" }]
 license = { file = "license.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

