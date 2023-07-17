# Comparing `tmp/typedhttp-0.2.0.tar.gz` & `tmp/typedhttp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhttp-0.2.0.tar", max compression
+gzip compressed data, was "typedhttp-0.3.0.tar", max compression
```

## Comparing `typedhttp-0.2.0.tar` & `typedhttp-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.2.0/README.md
--rw-r--r--   0        0        0      380 2023-07-17 13:50:38.051074 typedhttp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-07-17 13:49:00.751120 typedhttp-0.2.0/src/typedhttp/__init__.py
--rw-r--r--   0        0        0     1504 2023-07-10 18:18:06.546066 typedhttp-0.2.0/src/typedhttp/main.py
--rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.2.0/src/typedhttp/py.typed
--rw-r--r--   0        0        0     2336 2023-07-17 13:50:21.251086 typedhttp-0.2.0/src/typedhttp/requests_hook.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 typedhttp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.3.0/README.md
+-rw-r--r--   0        0        0      481 2023-07-17 15:21:29.738047 typedhttp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-07-17 15:18:47.393340 typedhttp-0.3.0/src/typedhttp/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-17 15:18:47.393340 typedhttp-0.3.0/src/typedhttp/exc.py
+-rw-r--r--   0        0        0     1542 2023-07-17 15:18:47.463340 typedhttp-0.3.0/src/typedhttp/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.3.0/src/typedhttp/py.typed
+-rw-r--r--   0        0        0     2105 2023-07-17 15:21:00.666535 typedhttp-0.3.0/src/typedhttp/requests_hook.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 typedhttp-0.3.0/PKG-INFO
```

### Comparing `typedhttp-0.2.0/src/typedhttp/main.py` & `typedhttp-0.3.0/src/typedhttp/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,37 +30,39 @@
 
     @abstractmethod
     def get_status_code(self) -> int:
         raise NotImplementedError
 
 
 ResponseDecoder = Callable[[ResponseProvider], T]
+ErrorHandler = Callable[[ResponseProvider], None]
 
 
 @dataclass
 class HTTPRequestObject(Generic[T]):
     method: str
     path: str
     response_decoder: ResponseDecoder[T]
     success_status_codes: List[int] = field(
         default_factory=lambda: [200, 201, 202, 203, 204, 205, 206, 207, 208, 226]
     )
-    error_decoders: Dict[int, ResponseDecoder[Exception]] = field(default_factory=dict)
+    error_decoders: Dict[int, ErrorHandler] = field(default_factory=dict)
     as_stream: bool = False
     headers: Optional[List[Tuple[str, str]]] = None
     body: Optional[bytes] = None
     follow_redirects: bool = True
     basic_auth: Optional[Tuple[str, str]] = None
 
 
 class HTTPHandler(ABC):
     @abstractmethod
     def send(self, request: HTTPRequestObject[T]) -> T:
         raise NotImplementedError
 
+
 __all__ = [
     "HTTPHandler",
     "HTTPRequestObject",
     "ResponseDecoder",
     "ResponseProvider",
     "T",
-]
+]
```

### Comparing `typedhttp-0.2.0/src/typedhttp/requests_hook.py` & `typedhttp-0.3.0/src/typedhttp/requests_hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Iterator, List, Tuple, TypeVar
 
 import requests
 
 from typedhttp import HTTPHandler, HTTPRequestObject, ResponseProvider
 
+from typedhttp.exc import NoExceptionProvidedForStatusCode
+
 T = TypeVar("T")
 
+
 class RequestsResponseProvider(ResponseProvider):
     def __init__(self, response: requests.Response) -> None:
         self.response = response
 
     def get_raw_response(self) -> bytes:
         return self.response.content
 
@@ -44,26 +47,18 @@
             auth=request.basic_auth,
         )
 
         response_provider = RequestsResponseProvider(response)
 
         if response.status_code not in request.success_status_codes:
             if response.status_code in request.error_decoders:
-                try:
-                    exc = request.error_decoders[response.status_code](
-                        response_provider
-                    )
-                except Exception as e:
-                    raise Exception(
-                        f"Error decoding response with status code {response.status_code}: {response.text}"
-                    ) from e
+                request.error_decoders[response.status_code](response_provider)
 
-                raise exc
             else:
-                raise Exception(
+                raise NoExceptionProvidedForStatusCode(
                     f"Request failed with status code {response.status_code} and no error decoder: {response.text}"
                 )
 
         return request.response_decoder(response_provider)
 
 
-__all__ = ["RequestsHTTPHandler", "RequestsResponseProvider"]
+__all__ = ["RequestsHTTPHandler", "RequestsResponseProvider"]
```

