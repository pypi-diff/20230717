# Comparing `tmp/infoblox-discovery-0.1.0.tar.gz` & `tmp/infoblox-discovery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoblox-discovery-0.1.0.tar", last modified: Tue Jul 11 12:37:09 2023, max compression
+gzip compressed data, was "infoblox-discovery-0.1.1.tar", last modified: Mon Jul 17 09:58:54 2023, max compression
```

## Comparing `infoblox-discovery-0.1.0.tar` & `infoblox-discovery-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/infoblox_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/http_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/infoblox_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/infoblox_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/infoblox_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/infoblox_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/infoblox_discovery/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 12:37:09.000000 infoblox-discovery-0.1.0/infoblox_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:37:09.766147 infoblox-discovery-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-11 12:36:34.000000 infoblox-discovery-0.1.0/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/infoblox_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/http_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/tests/test_dummy.py
```

### Comparing `infoblox-discovery-0.1.0/LICENSE` & `infoblox-discovery-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/__init__.py` & `infoblox-discovery-0.1.1/infoblox_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/__main__.py` & `infoblox-discovery-0.1.1/infoblox_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/api.py` & `infoblox-discovery-0.1.1/infoblox_discovery/api.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/cache.py` & `infoblox-discovery-0.1.1/infoblox_discovery/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def put(self, master: str, type: str, data: List[Any]):
         self._expire = time.time() + self._ttl
         if master not in self._cache:
             self._cache[master] = {}
         self._cache[master][type] = data
 
     def get(self, master: str, type: str) -> List[Any]:
-        if time.time() < self._expire:
+        if time.time() < self._expire and type in self._cache[master]:
             log.info_fmt({"operation": "cache", "hit": True})
             return self._cache[master][type]
         log.info_fmt({"operation": "cache", "hit": False})
         return []
 
     def get_all(self) -> Dict[str,Dict[str, List]]:
         return self._cache
```

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/collector.py` & `infoblox-discovery-0.1.1/infoblox_discovery/collector.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/environments.py` & `infoblox-discovery-0.1.1/infoblox_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/exceptions.py` & `infoblox-discovery-0.1.1/infoblox_discovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/file_service_discovery.py` & `infoblox-discovery-0.1.1/infoblox_discovery/file_service_discovery.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/fmglogging.py` & `infoblox-discovery-0.1.1/infoblox_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/http_service_discovery.py` & `infoblox-discovery-0.1.1/infoblox_discovery/http_service_discovery.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/infoblox_dhcp.py` & `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dhcp.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/infoblox_dns.py` & `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dns.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/infoblox_member.py` & `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_member.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/infoblox_node.py` & `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_node.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/metrics.py` & `infoblox-discovery-0.1.1/infoblox_discovery/metrics.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery/transform.py` & `infoblox-discovery-0.1.1/infoblox_discovery/transform.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/infoblox_discovery.egg-info/SOURCES.txt` & `infoblox-discovery-0.1.1/infoblox_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.0/setup.py` & `infoblox-discovery-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "count_commits_from_version_file": False,
         "branch_formatter": None
     },
     setup_requires=['setuptools-git-versioning'],
     packages=find_packages(),
     author='thenodon',
     author_email='aha@ingby.com',
-    url='https://github.com/thenodon/infoblox-discovery',
+    url='https://github.com/thenodon/infoblox_discovery',
     license='GPLv3',
     include_package_data=True,
     zip_safe=False,
     description="A Prometheus file and http discovery for infoblox",
     install_requires=read('requirements.txt').split(),
     python_requires='>=3.8',
 )
```

### Comparing `infoblox-discovery-0.1.0/tests/test_dummy.py` & `infoblox-discovery-0.1.1/tests/test_dummy.py`

 * *Files identical despite different names*

