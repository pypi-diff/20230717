# Comparing `tmp/medialoopster-0.0.8.tar.gz` & `tmp/medialoopster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medialoopster-0.0.8.tar", last modified: Wed Jul 28 14:08:22 2021, max compression
+gzip compressed data, was "medialoopster-0.0.9.tar", last modified: Fri Aug  6 08:13:38 2021, max compression
```

## Comparing `medialoopster-0.0.8.tar` & `medialoopster-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-28 14:08:22.798539 medialoopster-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      873 2021-07-28 14:08:22.798539 medialoopster-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      415 2021-07-28 14:08:13.000000 medialoopster-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-28 14:08:22.796539 medialoopster-0.0.8/medialoopster/
--rw-rw-rw-   0 root         (0) root         (0)      480 2021-07-28 14:08:13.000000 medialoopster-0.0.8/medialoopster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4741 2021-07-28 14:08:13.000000 medialoopster-0.0.8/medialoopster/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-28 14:08:22.797539 medialoopster-0.0.8/medialoopster.egg-info/
--rw-r--r--   0 root         (0) root         (0)      873 2021-07-28 14:08:22.000000 medialoopster-0.0.8/medialoopster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2021-07-28 14:08:22.000000 medialoopster-0.0.8/medialoopster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-28 14:08:22.000000 medialoopster-0.0.8/medialoopster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-07-28 14:08:22.000000 medialoopster-0.0.8/medialoopster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-07-28 14:08:22.000000 medialoopster-0.0.8/medialoopster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-28 14:08:22.798539 medialoopster-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      703 2021-07-28 14:08:13.000000 medialoopster-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-06 08:13:38.769353 medialoopster-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      873 2021-08-06 08:13:38.768352 medialoopster-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      415 2021-08-06 08:13:29.000000 medialoopster-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-06 08:13:38.766352 medialoopster-0.0.9/medialoopster/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2021-08-06 08:13:29.000000 medialoopster-0.0.9/medialoopster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2021-08-06 08:13:29.000000 medialoopster-0.0.9/medialoopster/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-06 08:13:38.768352 medialoopster-0.0.9/medialoopster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      873 2021-08-06 08:13:38.000000 medialoopster-0.0.9/medialoopster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      249 2021-08-06 08:13:38.000000 medialoopster-0.0.9/medialoopster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-06 08:13:38.000000 medialoopster-0.0.9/medialoopster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-08-06 08:13:38.000000 medialoopster-0.0.9/medialoopster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-08-06 08:13:38.000000 medialoopster-0.0.9/medialoopster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-06 08:13:38.769353 medialoopster-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      703 2021-08-06 08:13:29.000000 medialoopster-0.0.9/setup.py
```

### Comparing `medialoopster-0.0.8/PKG-INFO` & `medialoopster-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medialoopster
-Version: 0.0.8
+Version: 0.0.9
 Summary: medialoopster API wrapper for Python
 Home-page: https://gitlab.com/medialoopster/medialoopster_python
 Author: Stéphane Ludwig
 Author-email: gitlab@stephane-ludwig.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `medialoopster-0.0.8/medialoopster/api.py` & `medialoopster-0.0.9/medialoopster/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -143,7 +143,43 @@
             "status_approval": 0
         }
 
         response = self.session.patch(url, json=request)
         response.raise_for_status()
 
         return response.json()
+
+    def disapprove_asset(self, asset_id, asset_type="videoassets"):
+        url = f"{self.get_url(asset_type=asset_type)}{asset_id}/"
+
+        request = {
+            "status_approval": 0
+        }
+
+        response = self.session.patch(url, json=request)
+        response.raise_for_status()
+
+        return response.json()
+
+    def set_date_del_asset(self, asset_id, date_del, asset_type="videoassets"):
+        url = f"{self.get_url(asset_type=asset_type)}{asset_id}/"
+
+        request = {
+            "date_del": date_del
+        }
+
+        response = self.session.patch(url, json=request)
+        response.raise_for_status()
+
+        return response.json()
+
+    def edit_meta_field_store(self, asset_id, meta_field_store, asset_type="videoassets"):
+        url = f"{self.get_url(asset_type=asset_type)}{asset_id}/"
+
+        request = {
+            "meta_field_store": meta_field_store
+        }
+
+        response = self.session.patch(url, json=request)
+        response.raise_for_status()
+
+        return response.json()
```

### Comparing `medialoopster-0.0.8/medialoopster.egg-info/PKG-INFO` & `medialoopster-0.0.9/medialoopster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medialoopster
-Version: 0.0.8
+Version: 0.0.9
 Summary: medialoopster API wrapper for Python
 Home-page: https://gitlab.com/medialoopster/medialoopster_python
 Author: Stéphane Ludwig
 Author-email: gitlab@stephane-ludwig.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `medialoopster-0.0.8/setup.py` & `medialoopster-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="medialoopster",
-    version="0.0.8",
+    version="0.0.9",
     author="Stéphane Ludwig",
     author_email="gitlab@stephane-ludwig.net",
     description="medialoopster API wrapper for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/medialoopster/medialoopster_python",
     packages=setuptools.find_packages(),
```

