# Comparing `tmp/fastapi_authtools-0.3.tar.gz` & `tmp/fastapi_authtools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authtools-0.3.tar", last modified: Sat Jul 15 09:33:23 2023, max compression
+gzip compressed data, was "fastapi_authtools-0.4.tar", last modified: Mon Jul 17 06:23:49 2023, max compression
```

## Comparing `fastapi_authtools-0.3.tar` & `fastapi_authtools-0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.3/LICENSE
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1597 2023-07-14 17:51:40.000000 fastapi_authtools-0.3/README.md
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.480769 fastapi_authtools-0.3/fastapi_authtools/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2660 2023-07-14 18:25:23.000000 fastapi_authtools-0.3/fastapi_authtools/__init__.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1759 2023-07-15 09:32:31.000000 fastapi_authtools-0.3/fastapi_authtools/backend.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      500 2023-07-14 05:43:40.000000 fastapi_authtools-0.3/fastapi_authtools/exceptions.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      966 2023-07-14 18:25:23.000000 fastapi_authtools-0.3/fastapi_authtools/middleware.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.3/fastapi_authtools/models.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      994 2023-07-15 09:32:31.000000 fastapi_authtools-0.3/fastapi_authtools/token.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.3/fastapi_authtools/user.py
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/fastapi_authtools.egg-info/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2262 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      489 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/SOURCES.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/dependency_links.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/not-zip-safe
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       20 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/requires.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       18 2023-07-15 09:33:23.000000 fastapi_authtools-0.3/fastapi_authtools.egg-info/top_level.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      631 2023-07-15 09:33:10.000000 fastapi_authtools-0.3/pyproject.toml
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-07-15 09:33:23.484768 fastapi_authtools-0.3/setup.cfg
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      515 2023-07-15 09:33:10.000000 fastapi_authtools-0.3/setup.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.4/LICENSE
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4351 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3678 2023-07-17 06:19:38.000000 fastapi_authtools-0.4/README.md
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.827398 fastapi_authtools-0.4/fastapi_authtools/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3162 2023-07-16 19:19:10.000000 fastapi_authtools-0.4/fastapi_authtools/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2126 2023-07-16 18:52:36.000000 fastapi_authtools-0.4/fastapi_authtools/backend.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1015 2023-07-16 18:52:36.000000 fastapi_authtools-0.4/fastapi_authtools/exceptions.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1048 2023-07-16 18:35:50.000000 fastapi_authtools-0.4/fastapi_authtools/middleware.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.4/fastapi_authtools/models.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      912 2023-07-15 16:18:33.000000 fastapi_authtools-0.4/fastapi_authtools/token.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.4/fastapi_authtools/user.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/fastapi_authtools.egg-info/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4351 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      489 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/not-zip-safe
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       20 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/requires.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       18 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/top_level.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      639 2023-07-17 06:22:42.000000 fastapi_authtools-0.4/pyproject.toml
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/setup.cfg
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      538 2023-07-17 06:23:22.000000 fastapi_authtools-0.4/setup.py
```

### Comparing `fastapi_authtools-0.3/LICENSE` & `fastapi_authtools-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.3/PKG-INFO` & `fastapi_authtools-0.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: fastapi_authtools
-Version: 0.3
-Summary: A small example package
-Home-page: https://github.com/michael7nightinglae/fastapi_authtools
-Author: Michael Nightingale
-Author-email: Michael Nightingale <suslanchikmopl@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/michael7nightinglae/fastapi_authtools
-Project-URL: Bug Tracker, https://github.com/michael7nightinglae/fastapi_authtools/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FastAPI auth library.
 
 It`s simple to connect to your project. Just make user_data verification, and library will manage JWT-tokens.
 
 ## Installation
 Install package with pip:
 ```commandline
@@ -27,20 +10,21 @@
 
 ...or with poetry:
 ```commandline
 poetry add fastapi-authtools
 ```
 
 ## Usage
+You can you it with JWT-token (default in you headers).
+
 ```python
 from fastapi import FastAPI, Request, Body
-from fastapi import FastAPI, Request, Body
 
 from fastapi_authtools import AuthManager, login_required
-from fastapi_authtools.models import UsernamePasswordToken
+from fastapi_authtools.models import UsernamePasswordToken, UserModel
 
 
 app = FastAPI()
 
 # JWT token settings
 SECRET_KEY = 'secretSERCRET007'
 EXPIRE_MINUTES = 60 * 40
@@ -64,15 +48,86 @@
 async def homepage(request: Request):
     current_user = request.user
     return {"current_user": current_user}
 
 
 @app.post("/auth/token", status_code=201)
 async def get_access_token(request: Request, user_data: UsernamePasswordToken = Body()):
-    # ... here goes db user verification
-    token = request.app.state.auth_manager.create_token(user_data)
+    # ... here goes db user verification and getting user information
+    # user = get_login_user(user_data)
+    user = UserModel(
+        email="suslanchikmol@gmail.con",
+        username="michael7nightingale"
+    )
+    token = request.app.state.auth_manager.create_token(user)
     return {"access_token": token}
 
 ```
 
+But you can still use cookies to save token, just define `user_cookies` as True when initialize AuthManager.
+
+To use templates and form data you should install `jinja2` and `python-multipart`. 
+```python
+from fastapi import FastAPI, Request
+from fastapi.responses import RedirectResponse
+from fastapi.templating import Jinja2Templates
+
+from fastapi_authtools import AuthManager, login_required
+from fastapi_authtools.models import UserModel
+
+
+app = FastAPI()
+templates = Jinja2Templates(directory="templates")
+
+# JWT token settings
+SECRET_KEY = 'secretSERCRET007'
+EXPIRE_MINUTES = 60 * 40
+ALGORITHM = "HS256"
+
+# create login manager
+auth_manager = AuthManager(
+    app=app,
+    use_cookies=True,
+    secret_key=SECRET_KEY,
+    algorithm=ALGORITHM,
+    expire_minutes=EXPIRE_MINUTES
+)
+
+# now you can use login_manager directly or py adding it to the application statement
+# it`s comfortable while dealing with APIRouters
+app.state.auth_manager = auth_manager
+
+
+@app.get("/")
+@login_required  # make this endpoint allowed only for authenticated users
+async def homepage(request: Request):
+    return templates.TemplateResponse(
+        name="homepage.html",
+        context={"request": request, "current_user": request.user}
+    )
+
+
+@app.get('/login')
+async def login_get(request: Request):
+    return templates.TemplateResponse(
+        name='login.html',
+        context={"request": request}
+    )
+
+
+@app.post("/login", status_code=201)
+async def login_post(request: Request):
+    user_data = await request.form()
+    # ... here goes db user verification and getting user information
+    # user = get_login_user(user_data)
+    user = UserModel(
+        email="suslanchikmol@gmail.con",
+        username="michael7nightingale"
+    )
+    response = RedirectResponse(app.url_path_for("homepage"), status_code=303)
+    app.state.auth_manager.login(response, user)
+    return response
+```
+
+
 Auth manager adds authentication middleware to your application instance and uses authentication backends to treat token and
 request user instance.
```

### Comparing `fastapi_authtools-0.3/fastapi_authtools/__init__.py` & `fastapi_authtools-0.4/fastapi_authtools/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fastapi import FastAPI, Request
+from fastapi import FastAPI, Request, Response
 from starlette.middleware import authentication
 from starlette.responses import JSONResponse
 from pydantic import BaseModel
-from typing import Awaitable, List, Callable
+from typing import Awaitable, List, Callable, Type
 from functools import wraps
 
 from .middleware import AuthenticationMiddleware
 from .token import encode_jwt_token
 from .exceptions import raise_credentials_error, raise_data_model_exception
 from .models import UserModel
 
@@ -25,45 +25,59 @@
     """
     def __init__(
             self,
             app: FastAPI,
             secret_key: str,
             algorithm: str,
             expire_minutes: int,
-            user_model: BaseModel = UserModel,
+            use_cookies: bool = False,
+            user_model: Type[BaseModel] = UserModel,
             auth_error_handler: Callable[[Request, authentication.AuthenticationError], JSONResponse] | None = None,
             excluded_urls: List[str] | None = None
     ):
         self._app = app
         self.jwt_config = JWTConfig(
             secret_key=secret_key,
             algorithm=algorithm,
             expire_minutes=expire_minutes
         )
+        self.use_cookies = use_cookies
         self.user_model = user_model
         self.auth_error_handler = auth_error_handler
         self.excluded_urls = excluded_urls
 
         self._configurate_app()
 
     @property
     def app(self) -> FastAPI:
         return self._app
 
+    def login(self, response: Response, user: Type[BaseModel]) -> None:
+        access_token = self.create_token(user)
+        response.set_cookie(
+            key="access-token",
+            value=access_token,
+            max_age=60*24*14
+        )
+
+    def logout(self, response: Response) -> None:
+        response.delete_cookie(key="access-token")
+
     def _configurate_app(self):
         """Configurate application function (adds middleware.)"""
         self.app.add_middleware(
             AuthenticationMiddleware,
             jwt_config=self.jwt_config,
             excluded_urls=self.excluded_urls,
+            use_cookies=self.use_cookies,
             user_model=self.user_model,
             auth_error_handler=self.auth_error_handler
         )
 
-    def create_token(self, data: BaseModel) -> str:
+    def create_token(self, data: Type[BaseModel]) -> str:
         """Create token function to user in token get endpoint."""
         return encode_jwt_token(
             user_data=data,
             secret_key=self.jwt_config.secret_key,
             expire_minutes=self.jwt_config.expire_minutes,
             algorithm=self.jwt_config.algorithm
         )
```

### Comparing `fastapi_authtools-0.3/fastapi_authtools/backend.py` & `fastapi_authtools-0.4/fastapi_authtools/backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 from starlette import authentication
-from starlette.datastructures import Headers
 from starlette.requests import HTTPConnection
 from pydantic import typing, BaseModel
-import typing
+from typing import Type
 
+from .exceptions import invalid_credentials_message
 from .token import decode_jwt_token
-from .user import FastAPIUser
 
 
 class AuthenticationBackend(authentication.AuthenticationBackend):
     def __init__(
             self,
-            jwt_config: BaseModel,
+            jwt_config: Type[BaseModel],
             excluded_urls: list | None,
-            user_model: BaseModel,
+            use_cookies: bool,
+            user_model: Type[BaseModel],
 
     ):
         self.jwt_config = jwt_config
+        self.use_cookies = use_cookies
         self.user_model = user_model
         self.excluded_urls = [] if excluded_urls is None else excluded_urls
 
-    def verify_token(self, headers: dict | Headers):
-        token = headers.get("authorization") or headers.get("Authorization")
+    def verify_token(self, token: str):
         scopes = []
         if token is None:
             return scopes, None
 
         token = token.split()[-1]
         user_data = decode_jwt_token(
             token=token,
             secret_key=self.jwt_config.secret_key,
             algorithm=self.jwt_config.algorithm
         )
         if user_data is None:
             return scopes, None
 
-        user = FastAPIUser(**user_data.dict()) if isinstance(user_data, BaseModel) else FastAPIUser(**user_data)
-        return scopes, user
+        try:
+            user = self.user_model(**user_data)
+        except:
+            raise authentication.AuthenticationError(invalid_credentials_message())
+        else:
+            return scopes, user
+
+    def get_token(self, conn: HTTPConnection) -> str:
+        if self.use_cookies:
+            token = conn.cookies.get("access-token")
+            return token
+        else:
+            token = conn.headers.get("authorization") or conn.headers.get("Authorization")
+            return token
 
     async def authenticate(
         self, conn: HTTPConnection
     ) -> typing.Optional[typing.Tuple[authentication.AuthCredentials, authentication.BaseUser | None]]:
         if conn.url.path in self.excluded_urls:
             return authentication.AuthCredentials([]), None
 
-        response = self.verify_token(conn.headers)
+        token = self.get_token(conn)
+        response = self.verify_token(token)
         if isinstance(response, typing.Awaitable):
             response = await response
 
         scopes, user = response
 
         return authentication.AuthCredentials(scopes=scopes), user
```

### Comparing `fastapi_authtools-0.3/fastapi_authtools/middleware.py` & `fastapi_authtools-0.4/fastapi_authtools/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from fastapi import FastAPI
 from starlette.middleware import authentication
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 from pydantic import BaseModel
-from typing import Callable, List
+from typing import Callable, List, Type
 
 from .backend import AuthenticationBackend
 
 
 def AuthenticationMiddleware(
         app: FastAPI,
-        jwt_config: BaseModel,
-        user_model: BaseModel,
+        jwt_config: Type[BaseModel],
+        use_cookies: bool,
+        user_model: Type[BaseModel],
         auth_error_handler: Callable[[Request, authentication.AuthenticationError], JSONResponse] | None,
         excluded_urls: List[str] | None
 ) -> authentication.AuthenticationMiddleware:
     """
     Fabric function that returns Auth. Middleware instance to insert
     into app middleware stack.
     """
     return authentication.AuthenticationMiddleware(
         app=app,
         backend=AuthenticationBackend(
+            use_cookies=use_cookies,
             jwt_config=jwt_config,
             excluded_urls=excluded_urls,
             user_model=user_model
         ),
         on_error=auth_error_handler
     )
```

### Comparing `fastapi_authtools-0.3/fastapi_authtools/models.py` & `fastapi_authtools-0.4/fastapi_authtools/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.3/fastapi_authtools/user.py` & `fastapi_authtools-0.4/fastapi_authtools/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.3/pyproject.toml` & `fastapi_authtools-0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fastapi_authtools"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="Michael Nightingale", email="suslanchikmopl@gmail.com" },
 ]
-description = "A small example package"
+description = "FastAPI authentication package."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `fastapi_authtools-0.3/setup.py` & `fastapi_authtools-0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapi_authtools',
-    version='0.3',
+    version='0.4',
     url='https://github.com/michael7nightinglae/fastapi_authtools',
     install_requires=[
         "fastapi", "python-jose"
     ],
     license='MIT',
     author='Michael Nightingale',
     author_email='suslanchikmopl@gmail.com',
     description='Simple and comfortable FastAPI JWT authentication.',
-    packages=find_packages(exclude=['tests']),
+    packages=find_packages(exclude=['tests', "templates", "app.py"]),
     long_description=open('README.md').read(),
     zip_safe=False
 )
```

