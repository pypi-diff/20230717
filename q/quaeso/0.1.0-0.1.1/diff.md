# Comparing `tmp/quaeso-0.1.0.tar.gz` & `tmp/quaeso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quaeso-0.1.0.tar", last modified: Mon Jul 17 18:01:54 2023, max compression
+gzip compressed data, was "quaeso-0.1.1.tar", last modified: Mon Jul 17 18:07:17 2023, max compression
```

## Comparing `quaeso-0.1.0.tar` & `quaeso-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:01:54.775081 quaeso-0.1.0/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2023-04-16 05:21:29.000000 quaeso-0.1.0/LICENSE
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       16 2023-04-16 05:21:29.000000 quaeso-0.1.0/MANIFEST.in
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     4757 2023-07-17 18:01:54.775081 quaeso-0.1.0/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     4352 2023-07-17 17:28:02.000000 quaeso-0.1.0/README.md
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:01:54.775081 quaeso-0.1.0/quaeso/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        0 2023-04-16 05:21:29.000000 quaeso-0.1.0/quaeso/__init__.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      556 2023-07-17 17:48:11.000000 quaeso-0.1.0/quaeso/__main__.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      840 2023-04-16 05:21:29.000000 quaeso-0.1.0/quaeso/colorizer.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1015 2023-04-16 05:21:29.000000 quaeso-0.1.0/quaeso/formatter.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      490 2023-04-16 05:21:29.000000 quaeso-0.1.0/quaeso/reader.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      434 2023-07-17 17:54:25.000000 quaeso-0.1.0/quaeso/writer.py
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     2296 2023-07-17 17:33:51.000000 quaeso-0.1.0/quaeso/yeet.py
-drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:01:54.775081 quaeso-0.1.0/quaeso.egg-info/
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     4757 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/PKG-INFO
--rw-rw-r--   0 zahash    (1000) zahash    (1000)      347 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/SOURCES.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/dependency_links.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       49 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/entry_points.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       50 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/requires.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)        7 2023-07-17 18:01:54.000000 quaeso-0.1.0/quaeso.egg-info/top_level.txt
--rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 18:01:54.775081 quaeso-0.1.0/setup.cfg
--rw-rw-r--   0 zahash    (1000) zahash    (1000)     1004 2023-07-17 18:00:20.000000 quaeso-0.1.0/setup.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:07:17.965665 quaeso-0.1.1/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1063 2023-04-16 05:21:29.000000 quaeso-0.1.1/LICENSE
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       16 2023-04-16 05:21:29.000000 quaeso-0.1.1/MANIFEST.in
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     4784 2023-07-17 18:07:17.965665 quaeso-0.1.1/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     4379 2023-07-17 18:06:03.000000 quaeso-0.1.1/README.md
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:07:17.965665 quaeso-0.1.1/quaeso/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        0 2023-04-16 05:21:29.000000 quaeso-0.1.1/quaeso/__init__.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      556 2023-07-17 17:48:11.000000 quaeso-0.1.1/quaeso/__main__.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      840 2023-04-16 05:21:29.000000 quaeso-0.1.1/quaeso/colorizer.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1015 2023-04-16 05:21:29.000000 quaeso-0.1.1/quaeso/formatter.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      490 2023-04-16 05:21:29.000000 quaeso-0.1.1/quaeso/reader.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      434 2023-07-17 17:54:25.000000 quaeso-0.1.1/quaeso/writer.py
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     2296 2023-07-17 17:33:51.000000 quaeso-0.1.1/quaeso/yeet.py
+drwxrwxr-x   0 zahash    (1000) zahash    (1000)        0 2023-07-17 18:07:17.965665 quaeso-0.1.1/quaeso.egg-info/
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     4784 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/PKG-INFO
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)      347 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/SOURCES.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        1 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/dependency_links.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       49 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/entry_points.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       50 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/requires.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)        7 2023-07-17 18:07:17.000000 quaeso-0.1.1/quaeso.egg-info/top_level.txt
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)       38 2023-07-17 18:07:17.965665 quaeso-0.1.1/setup.cfg
+-rw-rw-r--   0 zahash    (1000) zahash    (1000)     1004 2023-07-17 18:06:45.000000 quaeso-0.1.1/setup.py
```

### Comparing `quaeso-0.1.0/LICENSE` & `quaeso-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quaeso-0.1.0/PKG-INFO` & `quaeso-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,54 @@
-Metadata-Version: 2.1
-Name: quaeso
-Version: 0.1.0
-Summary: python cli program to send requests
-Home-page: https://github.com/zahash/quaeso
-Author: zahash
-Author-email: zahash.z@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # quaeso
 
 > python cli program to send requests
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A Python program that reads a json/yml file for request data and sends the request
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/quaeso.git
+pip3 install quaeso
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/quaeso.git
+pip install quaeso
 ```
 
 ## Usage example
 
-To get help with commandline arguments
+### To get help with commandline arguments
 
 ```sh
 quaeso --help
 ```
 
-Using Command-line Arguments
+### Using Command-line Arguments
 
 ```sh
-quaeso "some/folder/myrequest.yml"
+quaeso -f "some/folder/myrequest.yml"
 ```
 
 (or)
 
 ```sh
-quaeso "some/folder/myrequest.json"
+quaeso -f "some/folder/myrequest.json"
+```
+
+### Colorize Output
+
+```sh
+quaeso -f "some/folder/myrequest.yml" -c
 ```
 
 ### Disclaimer
 
 sometimes the quaeso command doesn't work in windows if the package is installed globally.
 
 to avoid this, install the package in a local virtual env
@@ -77,21 +68,21 @@
 and then pip install. But you will have to activate that env everytime you want to use quaeso.
 
 ## IO Redirection
 
 the response is written to stdout and headers/status are written to stderr so that users can take IO redirection to their advantage. This works on windows, linux and mac.
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2> res_headers.txt
+quaeso -f "some/folder/myrequest.yml" > res.json 2> res_headers.txt
 ```
 
 both stdout and stderr can be redirected to the same file
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2>&1
+quaeso -f "some/folder/myrequest.yml" > res.txt 2>&1
 ```
 
 ## Sample request file (`myrequest.yml`)
 
 ### GET
 
 ```yaml
@@ -102,15 +93,15 @@
   limit: 100
 headers:
   accept: text/xml
   accept-language: en
 timeout: 5000
 ```
 
-#### File Download (`quaeso "some/folder/myrequest.yml" > book.pdf`)
+#### File Download (`quaeso -f "some/folder/myrequest.yml" > book.pdf`)
 
 ```yaml
 url: http://do1.dr-chuck.com/pythonlearn/EN_us/pythonlearn.pdf
 method: get
 ```
 
 ### POST
@@ -224,9 +215,7 @@
 ## Contributing
 
 1. Fork it (<https://github.com/zahash/quaeso/fork>)
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
-
-
```

### Comparing `quaeso-0.1.0/README.md` & `quaeso-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,69 @@
+Metadata-Version: 2.1
+Name: quaeso
+Version: 0.1.1
+Summary: python cli program to send requests
+Home-page: https://github.com/zahash/quaeso
+Author: zahash
+Author-email: zahash.z@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # quaeso
 
 > python cli program to send requests
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A Python program that reads a json/yml file for request data and sends the request
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/quaeso.git
+pip3 install quaeso
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/quaeso.git
+pip install quaeso
 ```
 
 ## Usage example
 
-To get help with commandline arguments
+### To get help with commandline arguments
 
 ```sh
 quaeso --help
 ```
 
-Using Command-line Arguments
+### Using Command-line Arguments
 
 ```sh
-quaeso "some/folder/myrequest.yml"
+quaeso -f "some/folder/myrequest.yml"
 ```
 
 (or)
 
 ```sh
-quaeso "some/folder/myrequest.json"
+quaeso -f "some/folder/myrequest.json"
+```
+
+### Colorize Output
+
+```sh
+quaeso -f "some/folder/myrequest.yml" -c
 ```
 
 ### Disclaimer
 
 sometimes the quaeso command doesn't work in windows if the package is installed globally.
 
 to avoid this, install the package in a local virtual env
@@ -62,21 +83,21 @@
 and then pip install. But you will have to activate that env everytime you want to use quaeso.
 
 ## IO Redirection
 
 the response is written to stdout and headers/status are written to stderr so that users can take IO redirection to their advantage. This works on windows, linux and mac.
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2> res_headers.txt
+quaeso -f "some/folder/myrequest.yml" > res.json 2> res_headers.txt
 ```
 
 both stdout and stderr can be redirected to the same file
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2>&1
+quaeso -f "some/folder/myrequest.yml" > res.txt 2>&1
 ```
 
 ## Sample request file (`myrequest.yml`)
 
 ### GET
 
 ```yaml
@@ -87,15 +108,15 @@
   limit: 100
 headers:
   accept: text/xml
   accept-language: en
 timeout: 5000
 ```
 
-#### File Download (`quaeso "some/folder/myrequest.yml" > book.pdf`)
+#### File Download (`quaeso -f "some/folder/myrequest.yml" > book.pdf`)
 
 ```yaml
 url: http://do1.dr-chuck.com/pythonlearn/EN_us/pythonlearn.pdf
 method: get
 ```
 
 ### POST
@@ -209,7 +230,9 @@
 ## Contributing
 
 1. Fork it (<https://github.com/zahash/quaeso/fork>)
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
+
+
```

### Comparing `quaeso-0.1.0/quaeso/__main__.py` & `quaeso-0.1.1/quaeso/__main__.py`

 * *Files identical despite different names*

### Comparing `quaeso-0.1.0/quaeso/colorizer.py` & `quaeso-0.1.1/quaeso/colorizer.py`

 * *Files identical despite different names*

### Comparing `quaeso-0.1.0/quaeso/formatter.py` & `quaeso-0.1.1/quaeso/formatter.py`

 * *Files identical despite different names*

### Comparing `quaeso-0.1.0/quaeso/yeet.py` & `quaeso-0.1.1/quaeso/yeet.py`

 * *Files identical despite different names*

### Comparing `quaeso-0.1.0/quaeso.egg-info/PKG-INFO` & `quaeso-0.1.1/quaeso.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quaeso
-Version: 0.1.0
+Version: 0.1.1
 Summary: python cli program to send requests
 Home-page: https://github.com/zahash/quaeso
 Author: zahash
 Author-email: zahash.z@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -23,41 +23,47 @@
 
 ## Installation
 
 pip install this repo.
 (Note: Incompatible with Python 2.x)
 
 ```sh
-pip3 install git+https://github.com/zahash/quaeso.git
+pip3 install quaeso
 ```
 
 (or)
 
 ```sh
-pip install git+https://github.com/zahash/quaeso.git
+pip install quaeso
 ```
 
 ## Usage example
 
-To get help with commandline arguments
+### To get help with commandline arguments
 
 ```sh
 quaeso --help
 ```
 
-Using Command-line Arguments
+### Using Command-line Arguments
 
 ```sh
-quaeso "some/folder/myrequest.yml"
+quaeso -f "some/folder/myrequest.yml"
 ```
 
 (or)
 
 ```sh
-quaeso "some/folder/myrequest.json"
+quaeso -f "some/folder/myrequest.json"
+```
+
+### Colorize Output
+
+```sh
+quaeso -f "some/folder/myrequest.yml" -c
 ```
 
 ### Disclaimer
 
 sometimes the quaeso command doesn't work in windows if the package is installed globally.
 
 to avoid this, install the package in a local virtual env
@@ -77,21 +83,21 @@
 and then pip install. But you will have to activate that env everytime you want to use quaeso.
 
 ## IO Redirection
 
 the response is written to stdout and headers/status are written to stderr so that users can take IO redirection to their advantage. This works on windows, linux and mac.
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2> res_headers.txt
+quaeso -f "some/folder/myrequest.yml" > res.json 2> res_headers.txt
 ```
 
 both stdout and stderr can be redirected to the same file
 
 ```sh
-quaeso "some/folder/myrequest.yml" > res.json 2>&1
+quaeso -f "some/folder/myrequest.yml" > res.txt 2>&1
 ```
 
 ## Sample request file (`myrequest.yml`)
 
 ### GET
 
 ```yaml
@@ -102,15 +108,15 @@
   limit: 100
 headers:
   accept: text/xml
   accept-language: en
 timeout: 5000
 ```
 
-#### File Download (`quaeso "some/folder/myrequest.yml" > book.pdf`)
+#### File Download (`quaeso -f "some/folder/myrequest.yml" > book.pdf`)
 
 ```yaml
 url: http://do1.dr-chuck.com/pythonlearn/EN_us/pythonlearn.pdf
 method: get
 ```
 
 ### POST
```

### Comparing `quaeso-0.1.0/setup.py` & `quaeso-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 README = (HERE / "README.md").read_text()
 
 with (HERE / "requirements.txt").open() as f:
     requirements = f.read().splitlines()
 
 setup(
     name="quaeso",
-    version="0.1.0",
+    version="0.1.1",
     description="python cli program to send requests",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/zahash/quaeso",
     author="zahash",
     author_email="zahash.z@gmail.com",
     license="MIT",
```

