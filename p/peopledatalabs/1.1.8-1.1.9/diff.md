# Comparing `tmp/peopledatalabs-1.1.8.tar.gz` & `tmp/peopledatalabs-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-1.1.8.tar", max compression
+gzip compressed data, was "peopledatalabs-1.1.9.tar", max compression
```

## Comparing `peopledatalabs-1.1.8.tar` & `peopledatalabs-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/LICENSE
--rw-r--r--   0        0        0    12222 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/README.md
--rw-r--r--   0        0        0     1637 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      109 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     5754 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     1635 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      762 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2812 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      744 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      984 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5048 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2445 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     2198 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      215 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4349 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      783 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2241 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1139 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      460 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    13628 1970-01-01 00:00:00.000000 peopledatalabs-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-17 18:03:42.940434 peopledatalabs-1.1.9/LICENSE
+-rw-r--r--   0        0        0    12222 2023-07-17 18:03:42.940434 peopledatalabs-1.1.9/README.md
+-rw-r--r--   0        0        0     1637 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     5754 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     1635 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      762 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2812 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      744 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      984 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5048 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2445 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     2198 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      215 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4349 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      783 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2241 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1139 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      460 2023-07-17 18:03:42.944434 peopledatalabs-1.1.9/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    13628 1970-01-01 00:00:00.000000 peopledatalabs-1.1.9/PKG-INFO
```

### Comparing `peopledatalabs-1.1.8/LICENSE` & `peopledatalabs-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/README.md` & `peopledatalabs-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/pyproject.toml` & `peopledatalabs-1.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "1.1.8"
+version = "1.1.9"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
@@ -37,15 +37,15 @@
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7"
 black = "^23.3.0"
 coverage = "^7.2.7"
 docformatter = "^1.7"
 flake8 = "^5.0.4"
 pylint = "^2.17.4"
-pytest = "^7.3.2"
+pytest = "^7.4.0"
 pyupgrade = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-1.1.9/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/logger.py` & `peopledatalabs-1.1.9/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/main.py` & `peopledatalabs-1.1.9/src/peopledatalabs/main.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/models/__init__.py` & `peopledatalabs-1.1.9/src/peopledatalabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/models/company.py` & `peopledatalabs-1.1.9/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/models/person.py` & `peopledatalabs-1.1.9/src/peopledatalabs/models/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/models/school.py` & `peopledatalabs-1.1.9/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/requests.py` & `peopledatalabs-1.1.9/src/peopledatalabs/requests.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/src/peopledatalabs/settings.py` & `peopledatalabs-1.1.9/src/peopledatalabs/settings.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.8/PKG-INFO` & `peopledatalabs-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 1.1.8
+Version: 1.1.9
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.7.2,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.8 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.9 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

