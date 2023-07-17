# Comparing `tmp/htruc-1.1.1.tar.gz` & `tmp/htruc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htruc-1.1.1.tar", last modified: Mon Jul 17 05:59:12 2023, max compression
+gzip compressed data, was "htruc-1.1.2.tar", last modified: Mon Jul 17 07:45:13 2023, max compression
```

## Comparing `htruc-1.1.1.tar` & `htruc-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 05:59:12.583822 htruc-1.1.1/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.1.1/LICENSE.md
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-07-17 05:59:12.583822 htruc-1.1.1/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.1.1/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 05:59:12.583822 htruc-1.1.1/htruc/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.1.1/htruc/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11648 2023-07-17 05:57:42.000000 htruc-1.1.1/htruc/catalog.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.1.1/htruc/cli.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 05:59:12.583822 htruc-1.1.1/htruc/repos/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.1.1/htruc/repos/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.1.1/htruc/repos/_generic.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-06-19 07:58:45.000000 htruc-1.1.1/htruc/repos/_github.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 05:59:12.583822 htruc-1.1.1/htruc/schemas/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1375 2023-07-17 05:57:42.000000 htruc-1.1.1/htruc/schemas/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1499 2023-07-17 05:57:42.000000 htruc-1.1.1/htruc/schemas/upgrade_path.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.1.1/htruc/types.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.1.1/htruc/utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.1.1/htruc/validator.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 05:59:12.583822 htruc-1.1.1/htruc.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-07-17 05:59:12.000000 htruc-1.1.1/htruc.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-07-17 05:59:12.583822 htruc-1.1.1/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-07-17 05:58:53.000000 htruc-1.1.1/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 07:45:13.350478 htruc-1.1.2/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.1.2/LICENSE.md
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-07-17 07:45:13.350478 htruc-1.1.2/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.1.2/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 07:45:13.350478 htruc-1.1.2/htruc/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.1.2/htruc/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    11809 2023-07-17 07:43:47.000000 htruc-1.1.2/htruc/catalog.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.1.2/htruc/cli.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 07:45:13.350478 htruc-1.1.2/htruc/repos/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.1.2/htruc/repos/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.1.2/htruc/repos/_generic.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-07-17 07:24:48.000000 htruc-1.1.2/htruc/repos/_github.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 07:45:13.350478 htruc-1.1.2/htruc/schemas/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1375 2023-07-17 05:57:42.000000 htruc-1.1.2/htruc/schemas/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1499 2023-07-17 05:57:42.000000 htruc-1.1.2/htruc/schemas/upgrade_path.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.1.2/htruc/types.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.1.2/htruc/utils.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.1.2/htruc/validator.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-07-17 07:45:13.350478 htruc-1.1.2/htruc.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-07-17 07:45:13.000000 htruc-1.1.2/htruc.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-07-17 07:45:13.350478 htruc-1.1.2/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-07-17 07:44:47.000000 htruc-1.1.2/setup.py
```

### Comparing `htruc-1.1.1/LICENSE.md` & `htruc-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/PKG-INFO` & `htruc-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.1.1
+Version: 1.1.2
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `htruc-1.1.1/README.md` & `htruc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/catalog.py` & `htruc-1.1.2/htruc/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         _upgrade_a_dict(data)
     if citation_cff:
         for key in data:
             up = _get_bibtex_and_apa(data[key], access_token=access_token)
             if up:
                 logger.info(f"Successfully retrieved Bibtex or/and APA for {key}")
                 data[key].update(up)
-    return data
+    return dict(sorted(data.items()))
 
 
 def get_statistics(repositories: Catalog) -> pandas.DataFrame:
     """ Retrieve statistics from a diction of repositories
 
     :param repositories: Dictionary of Repositories records
 
@@ -267,27 +267,29 @@
     else:  # We got a URI
         try:
             req = requests.get(catalog_record["citation-file-link"])
             req.raise_for_status()
             citation_file_content = req.text
             if "</html>" in citation_file_content.lower():
                 raise Exception("CFF File link is wrong, it returns HTML.")
+            elif citation_file_content[0] == "{":
+                raise Exception("Got JSON at the given endpoint instead of YAML")
         except Exception as E:
             logger.error(f"Error retrieving CITATION File for {catalog_record['citation-file-link']}: {str(E)}")
             if "github.com" in catalog_record["url"]:
                 logger.error(f"Trying to reach github directly")
                 return _get_github_citation_file({"url": catalog_record["url"]}, access_token=access_token)
             return {}
 
     try:
         citation = cffconvert.Citation(citation_file_content)
     except Exception as E:
         logger.error(f"Unable to parse CFF for {catalog_record['url']} ({E})")
         nl = "\n"
-        logger.error(f"Content: \n{citation_file_content.replace(nl, nl+'>>>    ')}")
+        logger.error(f"Content: \n>>>    {citation_file_content.replace(nl, nl+'>>>    ')}")
         return {}
     return_obj = {}
     try:
         return_obj["_bibtex"] = citation.as_bibtex()
     except Exception as E:
         logger.error(f"Unable to parse as Bibtex {catalog_record['url']} ({E})")
```

### Comparing `htruc-1.1.1/htruc/cli.py` & `htruc-1.1.2/htruc/cli.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/repos/_github.py` & `htruc-1.1.2/htruc/repos/_github.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/schemas/__init__.py` & `htruc-1.1.2/htruc/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/schemas/upgrade_path.py` & `htruc-1.1.2/htruc/schemas/upgrade_path.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/utils.py` & `htruc-1.1.2/htruc/utils.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc/validator.py` & `htruc-1.1.2/htruc/validator.py`

 * *Files identical despite different names*

### Comparing `htruc-1.1.1/htruc.egg-info/PKG-INFO` & `htruc-1.1.2/htruc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.1.1
+Version: 1.1.2
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `htruc-1.1.1/setup.py` & `htruc-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'htruc'
 DESCRIPTION = 'HTRUC, a toolkit for HTR-United cataloging'
 URL = 'https://github.com/htr-united/htrvc'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

