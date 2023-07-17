# Comparing `tmp/whop-api-wrapper-1.1.6.tar.gz` & `tmp/whop-api-wrapper-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whop-api-wrapper-1.1.6.tar", last modified: Mon Jul 17 21:13:12 2023, max compression
+gzip compressed data, was "whop-api-wrapper-1.1.7.tar", last modified: Mon Jul 17 21:17:05 2023, max compression
```

## Comparing `whop-api-wrapper-1.1.6.tar` & `whop-api-wrapper-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 21:13:12.272210 whop-api-wrapper-1.1.6/
--rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     2064 2023-07-17 21:13:12.272210 whop-api-wrapper-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 21:13:12.272210 whop-api-wrapper-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-17 21:13:08.000000 whop-api-wrapper-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:13:12.260891 whop-api-wrapper-1.1.6/whop_api_wrapper/
--rw-rw-rw-   0        0        0    15951 2023-07-17 21:12:49.000000 whop-api-wrapper-1.1.6/whop_api_wrapper/Client.py
--rw-rw-rw-   0        0        0      251 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.6/whop_api_wrapper/Endpoints.py
--rw-rw-rw-   0        0        0     5957 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.6/whop_api_wrapper/Objects.py
--rw-rw-rw-   0        0        0      206 2023-07-17 21:12:49.000000 whop-api-wrapper-1.1.6/whop_api_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:13:12.270995 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-07-17 21:13:12.000000 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-17 21:13:12.000000 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 21:13:12.000000 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 21:13:12.000000 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 21:13:12.000000 whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 21:17:05.286945 whop-api-wrapper-1.1.7/
+-rw-rw-rw-   0        0        0     1089 2023-07-17 07:39:09.000000 whop-api-wrapper-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:17:05.286945 whop-api-wrapper-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-07-17 20:25:24.000000 whop-api-wrapper-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 21:17:05.286945 whop-api-wrapper-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-17 21:17:01.000000 whop-api-wrapper-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:17:05.275861 whop-api-wrapper-1.1.7/whop_api_wrapper/
+-rw-rw-rw-   0        0        0    15961 2023-07-17 21:16:30.000000 whop-api-wrapper-1.1.7/whop_api_wrapper/Client.py
+-rw-rw-rw-   0        0        0      251 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.7/whop_api_wrapper/Endpoints.py
+-rw-rw-rw-   0        0        0     5957 2023-07-17 21:02:55.000000 whop-api-wrapper-1.1.7/whop_api_wrapper/Objects.py
+-rw-rw-rw-   0        0        0      206 2023-07-17 21:12:49.000000 whop-api-wrapper-1.1.7/whop_api_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:17:05.285949 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     2064 2023-07-17 21:17:05.000000 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-17 21:17:05.000000 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:17:05.000000 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 21:17:05.000000 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 21:17:05.000000 whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/top_level.txt
```

### Comparing `whop-api-wrapper-1.1.6/LICENSE` & `whop-api-wrapper-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.6/PKG-INFO` & `whop-api-wrapper-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whop-api-wrapper-1.1.6/README.md` & `whop-api-wrapper-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.6/setup.py` & `whop-api-wrapper-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='whop-api-wrapper',
-    version='1.1.6',
+    version='1.1.7',
     author='Jacobfinn123',
     author_email='jacobfinn@bezosproxy.com',
     description='Simple Python Whop API Wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/TheSweeet/Whop-API-Wrapper',
     packages=find_packages(),
```

### Comparing `whop-api-wrapper-1.1.6/whop_api_wrapper/Client.py` & `whop-api-wrapper-1.1.7/whop_api_wrapper/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 
 class Client:
 	def __init__(
 		self,
 		token: str,
 		api_version: str = "v2"
 	):
-		self.token = token.replace("Bearer ", "")
-		self.headers = {"accept": "application/json", "Authorization": f"Bearer {token}"}
-		self.base_url = "https://api.whop.com/api/"
-		self.api_version = api_version
+		self._token = token.replace("Bearer ", "")
+		self._headers = {"accept": "application/json", "Authorization": f"Bearer {token}"}
+		self._base_url = "https://api.whop.com/api/"
+		self._api_version = api_version
 
 		# Test token
 		self._test_token()
 
 	def _test_token(self):
-		url = f"{self.base_url}{self.api_version}"
-		response = requests.get(url, headers=self.headers)
+		url = f"{self._base_url}{self._api_version}"
+		response = requests.get(url, headers=self._headers)
 		status_code = response.status_code
 
 		if status_code == 401:
 			raise Exception("Invalid token. Refer to https://dev.whop.com/reference/authentication", status_code)
 
 	def _make_request(
 		self,
 		endpoint: str,
 		request_method=requests.get,
 		**kwargs
 	) -> dict:
 
-		url = f"{self.base_url}{self.api_version}{endpoint}"
+		url = f"{self._base_url}{self._api_version}{endpoint}"
 		# Ensures at least authentication is being sent
-		headers = kwargs.get('headers') or self.headers
+		headers = kwargs.get('headers') or self._headers
 		kwargs['headers'] = headers
 		response = request_method(url, **kwargs)
 
 		status_code = response.status_code
 		if status_code == 400:
 			raise Exception("Invalid parameters.", status_code)
 		if status_code == 401:
```

### Comparing `whop-api-wrapper-1.1.6/whop_api_wrapper/Objects.py` & `whop-api-wrapper-1.1.7/whop_api_wrapper/Objects.py`

 * *Files identical despite different names*

### Comparing `whop-api-wrapper-1.1.6/whop_api_wrapper.egg-info/PKG-INFO` & `whop-api-wrapper-1.1.7/whop_api_wrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whop-api-wrapper
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple Python Whop API Wrapper
 Home-page: https://github.com/TheSweeet/Whop-API-Wrapper
 Author: Jacobfinn123
 Author-email: jacobfinn@bezosproxy.com
 Keywords: WHOP,API,WRAPPER
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

