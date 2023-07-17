# Comparing `tmp/mypermobil-0.1.4.tar.gz` & `tmp/mypermobil-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypermobil-0.1.4.tar", last modified: Mon Jul 10 11:52:48 2023, max compression
+gzip compressed data, was "mypermobil-0.1.5.tar", last modified: Mon Jul 17 13:14:44 2023, max compression
```

## Comparing `mypermobil-0.1.4.tar` & `mypermobil-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 11:52:48.173065 mypermobil-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-06-26 13:05:01.000000 mypermobil-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      599 2023-07-10 11:52:48.173065 mypermobil-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-27 12:19:10.000000 mypermobil-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 11:52:48.152072 mypermobil-0.1.4/mypermobil/
--rw-rw-rw-   0        0        0      258 2023-07-10 11:51:54.000000 mypermobil-0.1.4/mypermobil/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-27 11:58:00.000000 mypermobil-0.1.4/mypermobil/const.py
--rw-rw-rw-   0        0        0    15978 2023-07-10 11:47:27.000000 mypermobil-0.1.4/mypermobil/mypermobil.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:52:48.170065 mypermobil-0.1.4/mypermobil.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-10 11:52:48.000000 mypermobil-0.1.4/mypermobil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-07-10 11:52:48.000000 mypermobil-0.1.4/mypermobil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 11:52:48.000000 mypermobil-0.1.4/mypermobil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 11:52:48.000000 mypermobil-0.1.4/mypermobil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 11:52:48.000000 mypermobil-0.1.4/mypermobil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 12:17:06.000000 mypermobil-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      627 2023-07-10 11:52:48.177067 mypermobil-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-07-10 11:52:17.000000 mypermobil-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:14:44.017814 mypermobil-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2023-06-26 13:05:01.000000 mypermobil-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1579 2023-07-17 13:14:44.019819 mypermobil-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-07-12 06:51:54.000000 mypermobil-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:14:43.986817 mypermobil-0.1.5/mypermobil/
+-rw-rw-rw-   0        0        0      258 2023-07-17 13:06:43.000000 mypermobil-0.1.5/mypermobil/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-07-14 11:20:29.000000 mypermobil-0.1.5/mypermobil/const.py
+-rw-rw-rw-   0        0        0    17967 2023-07-17 13:07:15.000000 mypermobil-0.1.5/mypermobil/mypermobil.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:14:44.013814 mypermobil-0.1.5/mypermobil.egg-info/
+-rw-rw-rw-   0        0        0     1579 2023-07-17 13:14:43.000000 mypermobil-0.1.5/mypermobil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-07-17 13:14:43.000000 mypermobil-0.1.5/mypermobil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:14:43.000000 mypermobil-0.1.5/mypermobil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 13:14:43.000000 mypermobil-0.1.5/mypermobil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 13:14:43.000000 mypermobil-0.1.5/mypermobil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 12:17:06.000000 mypermobil-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      627 2023-07-17 13:14:44.022813 mypermobil-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-07-17 13:13:22.000000 mypermobil-0.1.5/setup.py
```

### Comparing `mypermobil-0.1.4/LICENSE` & `mypermobil-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypermobil-0.1.4/mypermobil/mypermobil.py` & `mypermobil-0.1.5/mypermobil/mypermobil.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import aiohttp
 from aiocache import Cache
 
 from .const import (
     ENDPOINT_APPLICATIONAUTHENTICATIONS,
     ENDPOINT_APPLICATIONLINKS,
     ENDPOINT_LOOKUP,
-    ITEM_LOOKUP,
+    ENDPOINT_PRODUCTS,
+    PRODUCTS_ID,
     GET_REGIONS,
     EMAIL_REGEX,
 )
 
 
 class MyPermobilException(Exception):
     """Permobil Exception. Generic Permobil Exception."""
@@ -98,14 +99,16 @@
     return email
 
 
 def validate_code(code: str) -> str:
     """Validates an code."""
     if not code:
         raise MyPermobilClientException("Missing code")
+    if " " in code or "\n" in code:
+        raise MyPermobilClientException("Code cannot contain spaces or newlines")
     if not code.isdigit():
         raise MyPermobilClientException("Code must be a number")
     if len(code) != 6:
         raise MyPermobilClientException("Code must be 6 digits long")
     return code
 
 
@@ -139,42 +142,53 @@
     if not region:
         raise MyPermobilClientException("Missing region")
     if not region.startswith("https://") and not region.startswith("http://"):
         raise MyPermobilClientException("Region missing protocol")
     return region
 
 
+def validate_product_id(product_id: str) -> str:
+    """Validates a product_id."""
+    if not product_id:
+        raise MyPermobilClientException("Missing product id")
+    if len(product_id) != 24:
+        raise MyPermobilClientException("Invalid product id")
+    return product_id
+
+
 async def create_session():
     """Create a client session."""
     return aiohttp.ClientSession()
 
 
 class MyPermobil:
     """Permobil API."""
 
+    request_timeout = 10
+
     def __init__(
         self,
         application: str,
         session: aiohttp.ClientSession,
         email: str = None,
         region: str = None,
         code: str = None,
         token: str = None,
         expiration_date: str = None,
-        request_timeout: int = 10,
+        product_id: str = None,
     ) -> None:
         """Initialize."""
         self.application = application
         self.session = session
         self.email = email
         self.region = region
         self.code = code
         self.token = token
         self.expiration_date = expiration_date
-        self.request_timeout = request_timeout
+        self.product_id = product_id
 
         self.authenticated = False
 
     # Magic methods
     def __str__(self) -> str:
         """str."""
         app, email, region = self.application, self.email, self.region
@@ -215,14 +229,18 @@
 
     def set_expiration_date(self, expiration_date: str):
         """Set expiration date."""
         if self.authenticated:
             raise MyPermobilClientException("Cannot change date after authentication")
         self.expiration_date = validate_expiration_date(expiration_date)
 
+    def set_product_id(self, product_id: str):
+        """Set product id."""
+        self.product_id = validate_product_id(product_id)
+
     def set_application(self, application: str):
         """Set application."""
         if self.authenticated:
             raise MyPermobilClientException("Cannot change app after authentication")
         self.application = application
 
     async def close_session(self):
@@ -249,17 +267,17 @@
         if not self.authenticated:
             raise MyPermobilClientException("Not authenticated")
         # TODO send deauthentication request
 
     # API Methods
     async def get_request(self, *args, **kwargs):
         """Get request."""
-        if "timeout" not in kwargs:
+        if not kwargs.get("timeout"):
             kwargs["timeout"] = self.request_timeout
-        if "headers" not in kwargs and self.authenticated:
+        if not kwargs.get("headers") and self.authenticated:
             kwargs["headers"] = self.headers
 
         try:
             return await self.session.get(*args, **kwargs)
         except aiohttp.ClientConnectorError as err:
             raise MyPermobilConnectionException("Connection error") from err
         except asyncio.TimeoutError as err:
@@ -267,17 +285,17 @@
         except aiohttp.ClientError as err:
             raise MyPermobilConnectionException("Client error") from err
         except Exception as err:
             raise MyPermobilAPIException("Unknown error") from err
 
     async def post_request(self, *args, **kwargs):
         """Post request."""
-        if "timeout" not in kwargs:
+        if not kwargs.get("timeout"):
             kwargs["timeout"] = self.request_timeout
-        if "headers" not in kwargs and self.authenticated:
+        if not kwargs.get("headers") and self.authenticated:
             kwargs["headers"] = self.headers
 
         try:
             return await self.session.post(*args, **kwargs)
         except aiohttp.ClientConnectorError as err:
             raise MyPermobilConnectionException("Connection error") from err
         except asyncio.TimeoutError as err:
@@ -365,81 +383,112 @@
             email = self.email
         if code is None:
             code = self.code
         if region is None:
             region = self.region
         if application is None:
             application = self.application
+        if expiration_date is None:
+            # set expiration date to 1 year from now
+            time_delta = datetime.timedelta(days=365)
+            date = datetime.datetime.now() + time_delta
+            expiration_date = date.strftime("%Y-%m-%d")
 
         if self.authenticated:
             raise MyPermobilClientException("Already authenticated")
         email = validate_email(email)
         region = validate_region(region)
         code = validate_code(code)
+        expiration_date = validate_expiration_date(expiration_date)
 
         url = region + ENDPOINT_APPLICATIONAUTHENTICATIONS
         json = {
             "username": email,
             "code": code,
             "application": application,
             "expirationDate": expiration_date,
         }
         response = await self.post_request(url, json=json)
 
         if response.status == 200:
             json = await response.json()
             token = json.get("token")
-            if expiration_date is None:
-                # set expiration date to 1 year from now
-                time_delta = datetime.timedelta(days=365)
-                date = datetime.datetime.now() + time_delta
-                expiration_date = date.strftime("%Y-%m-%d")
 
         elif response.status == 401:
             raise MyPermobilAPIException("Email not registered for region")
         elif response.status == 403:
             raise MyPermobilAPIException("Incorrect code")
         elif response.status in (400, 500):
             resp = await response.json()
             raise MyPermobilAPIException(resp.get("error", resp))
         else:
             text = await response.text()
             raise MyPermobilAPIException(text)
 
         return token, expiration_date
 
-    async def request_item(
-        self, item: str, endpoint: str = None, headers: dict = None
-    ) -> str | int | float | bool | dict | list:
-        """Takes and item, finds the endpoint and makes the request."""
+    async def request_product_id(self, headers: dict = None) -> str:
+        """Get product id from the API."""
+        # this function is equivalent to request_item(PRODUCTS_ID, ENDPOINT_PRODUCTS)
+        # but it has better error handling
         if headers is None:
             headers = self.headers
 
-        if endpoint not in ENDPOINT_LOOKUP:
-            if endpoint is None:
-                endpoint = ENDPOINT_LOOKUP.get(item)
-            else:
-                raise MyPermobilClientException(f"Invalid endpoint {endpoint}")
-            if endpoint is None:
-                raise MyPermobilClientException(f"No endpoint for item: {item}")
+        response = await self.request_endpoint(ENDPOINT_PRODUCTS, headers)
+        if not isinstance(response, list):
+            raise MyPermobilAPIException("Invalid response")
+        if len(response) != 1:
+            raise MyPermobilAPIException("Wrong number of products found")
 
-        if item not in ITEM_LOOKUP[endpoint]:
-            raise MyPermobilClientException(f"{item} not in endpoint {endpoint}")
+        return response[PRODUCTS_ID[0]][PRODUCTS_ID[1]]
 
-        response = await self.request_endpoint(endpoint, headers)
-        return response.get(item)
+    async def request_item(
+        self, items: str | list[str], endpoint: str = None, **kwargs
+    ) -> str | int | float | bool | dict | list:
+        """Takes a single item or list of items, finds the endpoint and makes the request."""
+        if not items:
+            raise MyPermobilClientException("No item(s) provided")
+
+        if isinstance(items, str):
+            items = [items]
+
+        if endpoint is None:
+            key = str(items)
+            if key in ENDPOINT_LOOKUP:
+                endpoint = ENDPOINT_LOOKUP.get(key)
+            else:
+                raise MyPermobilClientException(f"No endpoint for: {key}")
+
+        # dive into the response for each item in the list
+        response = await self.request_endpoint(endpoint, kwargs)
+        for item in items:
+            if isinstance(response, dict) and item not in response:
+                raise MyPermobilClientException(f"{item} not in response")
+            if isinstance(response, list) and item >= len(response):
+                raise MyPermobilClientException(
+                    f"Too few items in response {item} >= {len(response)}"
+                )
+            response = response[item]
+        return response
 
     @cacheable
-    async def request_endpoint(self, endpoint: str, headers: dict = None) -> dict:
+    async def request_endpoint(
+        self, endpoint: str, headers: dict = None, product_id: str = None
+    ) -> dict:
         """Makes a request to an endpoint."""
         if headers is None:
             headers = self.headers
+        if product_id is None:
+            product_id = self.product_id
 
-        resp = await self.get_request(self.region + endpoint)
+        endpoint = endpoint.format(product_id=product_id)
+        resp = await self.get_request(self.region + endpoint, headers=headers)
         status = resp.status
-        json = await resp.json()
-        if status >= 200 and status < 300:
-            return json
-
-        text = await resp.text()
-        msg = json.get("error", text)
-        raise MyPermobilAPIException(f"Permobil API {status}: {msg}")
+        try:
+            json = await resp.json()
+            if status >= 200 and status < 300:
+                return json
+            text = await resp.text()
+            message = json.get("error", text)
+        except aiohttp.client_exceptions.ContentTypeError:
+            message = await resp.text()
+        raise MyPermobilAPIException(f"{status}: {message}")
```

### Comparing `mypermobil-0.1.4/setup.cfg` & `mypermobil-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7970 6572 6d6f 6269 6c0d 0a76   = mypermobil..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e34 0d0a  ersion = 0.1.4..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e35 0d0a  ersion = 0.1.5..
 00000030: 6175 7468 6f72 203d 2049 7361 6b20 4e79  author = Isak Ny
 00000040: 6265 7267 0d0a 6175 7468 6f72 5f65 6d61  berg..author_ema
 00000050: 696c 203d 2069 7361 6b40 6e79 6265 7267  il = isak@nyberg
 00000060: 2e64 6576 0d0a 6465 7363 7269 7074 696f  .dev..descriptio
 00000070: 6e20 3d20 4120 7079 7468 6f6e 2077 7261  n = A python wra
 00000080: 7070 6572 2066 6f72 2061 2073 7562 7365  pper for a subse
 00000090: 7420 6f66 2074 6865 204d 7950 6572 6d6f  t of the MyPermo
```

### Comparing `mypermobil-0.1.4/setup.py` & `mypermobil-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="mypermobil",
-    version="0.1.4",
+    version="0.1.5",
     description="A Python wrapper for the MyPermobil API",
     url="https://github.com/IsakNyberg/MyPermobil-API",
     author="Isak Nyberg",
     author_email="isak@nyberg.dev",
     license="MIT",
     packages=["mypermobil"],
     install_requires=["aiohttp", "aiocache"],
```

