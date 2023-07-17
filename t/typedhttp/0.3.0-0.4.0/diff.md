# Comparing `tmp/typedhttp-0.3.0.tar.gz` & `tmp/typedhttp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhttp-0.3.0.tar", max compression
+gzip compressed data, was "typedhttp-0.4.0.tar", max compression
```

## Comparing `typedhttp-0.3.0.tar` & `typedhttp-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.3.0/README.md
--rw-r--r--   0        0        0      481 2023-07-17 15:21:29.738047 typedhttp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      135 2023-07-17 15:18:47.393340 typedhttp-0.3.0/src/typedhttp/__init__.py
--rw-r--r--   0        0        0      107 2023-07-17 15:18:47.393340 typedhttp-0.3.0/src/typedhttp/exc.py
--rw-r--r--   0        0        0     1542 2023-07-17 15:18:47.463340 typedhttp-0.3.0/src/typedhttp/main.py
--rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.3.0/src/typedhttp/py.typed
--rw-r--r--   0        0        0     2105 2023-07-17 15:21:00.666535 typedhttp-0.3.0/src/typedhttp/requests_hook.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 typedhttp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.4.0/README.md
+-rw-r--r--   0        0        0      481 2023-07-17 15:26:21.010697 typedhttp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-07-17 15:18:47.393340 typedhttp-0.4.0/src/typedhttp/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-17 15:18:47.393340 typedhttp-0.4.0/src/typedhttp/exc.py
+-rw-r--r--   0        0        0     1610 2023-07-17 15:25:43.590096 typedhttp-0.4.0/src/typedhttp/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:18:06.546066 typedhttp-0.4.0/src/typedhttp/py.typed
+-rw-r--r--   0        0        0     2241 2023-07-17 15:25:58.850218 typedhttp-0.4.0/src/typedhttp/requests_hook.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 typedhttp-0.4.0/PKG-INFO
```

### Comparing `typedhttp-0.3.0/src/typedhttp/main.py` & `typedhttp-0.4.0/src/typedhttp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,19 +42,21 @@
     method: str
     path: str
     response_decoder: ResponseDecoder[T]
     success_status_codes: List[int] = field(
         default_factory=lambda: [200, 201, 202, 203, 204, 205, 206, 207, 208, 226]
     )
     error_decoders: Dict[int, ErrorHandler] = field(default_factory=dict)
+    unknown_status_code_decoder: Optional[ErrorHandler] = None
     as_stream: bool = False
     headers: Optional[List[Tuple[str, str]]] = None
     body: Optional[bytes] = None
     follow_redirects: bool = True
     basic_auth: Optional[Tuple[str, str]] = None
+    
 
 
 class HTTPHandler(ABC):
     @abstractmethod
     def send(self, request: HTTPRequestObject[T]) -> T:
         raise NotImplementedError
```

### Comparing `typedhttp-0.3.0/src/typedhttp/requests_hook.py` & `typedhttp-0.4.0/src/typedhttp/requests_hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         )
 
         response_provider = RequestsResponseProvider(response)
 
         if response.status_code not in request.success_status_codes:
             if response.status_code in request.error_decoders:
                 request.error_decoders[response.status_code](response_provider)
-
+            elif request.unknown_status_code_decoder is not None:
+                request.unknown_status_code_decoder(response_provider)
             else:
                 raise NoExceptionProvidedForStatusCode(
                     f"Request failed with status code {response.status_code} and no error decoder: {response.text}"
                 )
 
         return request.response_decoder(response_provider)
```

