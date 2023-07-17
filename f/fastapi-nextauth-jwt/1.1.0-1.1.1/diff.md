# Comparing `tmp/fastapi_nextauth_jwt-1.1.0.tar.gz` & `tmp/fastapi_nextauth_jwt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_nextauth_jwt-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_nextauth_jwt-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_nextauth_jwt-1.1.0.tar` & `fastapi_nextauth_jwt-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,33 @@
--rw-r--r--   0        0        0      985 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      741 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3089 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/LICENSE
--rw-r--r--   0        0        0     1541 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/README.md
--rw-r--r--   0        0        0      563 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/__init__.py
--rw-r--r--   0        0        0      974 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/cookies.py
--rw-r--r--   0        0        0      938 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/csrf.py
--rw-r--r--   0        0        0      873 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/exceptions.py
--rw-r--r--   0        0        0     5850 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
--rw-r--r--   0        0        0      580 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/operations.py
--rw-r--r--   0        0        0      646 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/fastapi/main.py
--rw-r--r--   0        0        0    18051 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/fastapi/test_main.py
--rw-r--r--   0        0        0     1021 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_cookies.py
--rw-r--r--   0        0        0     1654 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_csrf.py
--rw-r--r--   0        0        0      503 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_operations.py
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1541 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/README.md
+-rw-r--r--   0        0        0        6 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/fastapi/.gitignore
+-rw-r--r--   0        0        0      504 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/fastapi/main.py
+-rw-r--r--   0        0        0       53 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/fastapi/requirements.txt
+-rw-r--r--   0        0        0       40 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/.eslintrc.json
+-rw-r--r--   0        0        0      375 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/.gitignore
+-rw-r--r--   0        0        0     1751 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/README.md
+-rw-r--r--   0        0        0      201 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/next-env.d.ts
+-rw-r--r--   0        0        0      254 2023-07-17 16:44:35.043163 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/next.config.js
+-rw-r--r--   0        0        0   288145 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/package-lock.json
+-rw-r--r--   0        0        0      628 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/package.json
+-rw-r--r--   0        0        0       82 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/postcss.config.js
+-rw-r--r--   0        0        0    25931 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/public/next.svg
+-rw-r--r--   0        0        0      629 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/public/vercel.svg
+-rw-r--r--   0        0        0      119 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/middleware.ts
+-rw-r--r--   0        0        0      386 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/pages/_app.tsx
+-rw-r--r--   0        0        0      264 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/pages/_document.tsx
+-rw-r--r--   0        0        0     1356 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/pages/api/auth/[...nextauth].js
+-rw-r--r--   0        0        0      311 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/pages/api/hello.ts
+-rw-r--r--   0        0        0     1662 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/pages/index.tsx
+-rw-r--r--   0        0        0      578 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/src/styles/globals.css
+-rw-r--r--   0        0        0      480 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/tailwind.config.js
+-rw-r--r--   0        0        0      556 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/examples/simple/nextjs/tsconfig.json
+-rw-r--r--   0        0        0      661 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/__init__.py
+-rw-r--r--   0        0        0      974 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/cookies.py
+-rw-r--r--   0        0        0      938 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/csrf.py
+-rw-r--r--   0        0        0      873 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/exceptions.py
+-rw-r--r--   0        0        0     5850 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
+-rw-r--r--   0        0        0      580 2023-07-17 16:44:35.047164 fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/operations.py
+-rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.1.1/PKG-INFO
```

### Comparing `fastapi_nextauth_jwt-1.1.0/LICENSE` & `fastapi_nextauth_jwt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/README.md` & `fastapi_nextauth_jwt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/pyproject.toml` & `fastapi_nextauth_jwt-1.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,16 @@
 test = [
     "pytest >=2.7.3",
     "pytest-cov",
     "httpx"
 ]
 
 [project.urls]
-Home = "https://github.com/TCatshoek/fastapi-nextauth-jwt"
+Home = "https://github.com/TCatshoek/fastapi-nextauth-jwt"
+
+[tool.flit.sdist]
+exclude = [
+    "tests/",
+    ".github/",
+    ".examples/",
+    ".gitignore"
+]
```

### Comparing `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/cookies.py` & `fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/csrf.py` & `fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/csrf.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/exceptions.py` & `fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py` & `fastapi_nextauth_jwt-1.1.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.1.0/PKG-INFO` & `fastapi_nextauth_jwt-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_nextauth_jwt
-Version: 1.1.0
+Version: 1.1.1
 Summary: A fastapi dependency used to decode jwt tokens generated by nextauth,
 Author: Tom Catshoek
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: cryptography
 Requires-Dist: python-jose[cryptography]
```

