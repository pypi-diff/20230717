# Comparing `tmp/quadkey-boosted-1.0.3.tar.gz` & `tmp/quadkey-boosted-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quadkey-boosted-1.0.3.tar", last modified: Sun Jul 16 19:45:08 2023, max compression
+gzip compressed data, was "quadkey-boosted-1.0.4.tar", last modified: Mon Jul 17 11:00:09 2023, max compression
```

## Comparing `quadkey-boosted-1.0.3.tar` & `quadkey-boosted-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/
--rw-rw-r--   0 home      (1000) home      (1000)    11357 2023-07-08 11:45:21.000000 quadkey-boosted-1.0.3/LICENSE
--rw-rw-r--   0 home      (1000) home      (1000)       30 2023-07-16 16:58:10.000000 quadkey-boosted-1.0.3/MANIFEST.in
--rw-rw-r--   0 home      (1000) home      (1000)     4895 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)     3891 2023-07-16 16:42:34.000000 quadkey-boosted-1.0.3/README.md
--rw-rw-r--   0 home      (1000) home      (1000)      387 2023-07-16 19:44:21.000000 quadkey-boosted-1.0.3/pyproject.toml
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-16 19:45:08.898767 quadkey-boosted-1.0.3/quadkey/
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/quadkey/core/
--rw-rw-r--   0 home      (1000) home      (1000)      796 2023-07-16 16:50:30.000000 quadkey-boosted-1.0.3/quadkey/core/__init__.py
--rw-rw-r--   0 home      (1000) home      (1000)     1486 2023-07-16 16:12:37.000000 quadkey-boosted-1.0.3/quadkey/core/test_c_code.py
--rw-rw-r--   0 home      (1000) home      (1000)   385116 2023-07-16 16:58:44.000000 quadkey-boosted-1.0.3/quadkey/core/utils.c
--rw-rw-r--   0 home      (1000) home      (1000)    10934 2023-07-16 16:45:39.000000 quadkey-boosted-1.0.3/quadkey/core/utils.pyx
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/
--rw-rw-r--   0 home      (1000) home      (1000)     4895 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)      459 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/SOURCES.txt
--rw-rw-r--   0 home      (1000) home      (1000)        1 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/dependency_links.txt
--rw-rw-r--   0 home      (1000) home      (1000)       50 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/entry_points.txt
--rw-rw-r--   0 home      (1000) home      (1000)        7 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/requires.txt
--rw-rw-r--   0 home      (1000) home      (1000)       13 2023-07-16 19:45:08.000000 quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/top_level.txt
--rw-rw-r--   0 home      (1000) home      (1000)       38 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/setup.cfg
--rw-rw-r--   0 home      (1000) home      (1000)     1922 2023-07-16 19:44:21.000000 quadkey-boosted-1.0.3/setup.py
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-16 19:45:08.902767 quadkey-boosted-1.0.3/tests/
--rw-rw-r--   0 home      (1000) home      (1000)      688 2023-07-16 16:50:38.000000 quadkey-boosted-1.0.3/tests/test_quadkey_c_.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/
+-rw-rw-r--   0 home      (1000) home      (1000)    11357 2023-07-08 11:45:21.000000 quadkey-boosted-1.0.4/LICENSE
+-rw-rw-r--   0 home      (1000) home      (1000)       30 2023-07-16 16:58:10.000000 quadkey-boosted-1.0.4/MANIFEST.in
+-rw-rw-r--   0 home      (1000) home      (1000)     4880 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)     3881 2023-07-17 10:58:49.000000 quadkey-boosted-1.0.4/README.md
+-rw-rw-r--   0 home      (1000) home      (1000)      387 2023-07-17 10:59:52.000000 quadkey-boosted-1.0.4/pyproject.toml
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-17 11:00:09.654316 quadkey-boosted-1.0.4/quadkey/
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/quadkey/core/
+-rw-rw-r--   0 home      (1000) home      (1000)      796 2023-07-16 16:50:30.000000 quadkey-boosted-1.0.4/quadkey/core/__init__.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1486 2023-07-16 16:12:37.000000 quadkey-boosted-1.0.4/quadkey/core/test_c_code.py
+-rw-rw-r--   0 home      (1000) home      (1000)   385116 2023-07-16 16:58:44.000000 quadkey-boosted-1.0.4/quadkey/core/utils.c
+-rw-rw-r--   0 home      (1000) home      (1000)    10934 2023-07-16 16:45:39.000000 quadkey-boosted-1.0.4/quadkey/core/utils.pyx
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/
+-rw-rw-r--   0 home      (1000) home      (1000)     4880 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)      459 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/SOURCES.txt
+-rw-rw-r--   0 home      (1000) home      (1000)        1 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/dependency_links.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       50 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/entry_points.txt
+-rw-rw-r--   0 home      (1000) home      (1000)        7 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/requires.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       13 2023-07-17 11:00:09.000000 quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/top_level.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       38 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/setup.cfg
+-rw-rw-r--   0 home      (1000) home      (1000)     1917 2023-07-17 10:59:52.000000 quadkey-boosted-1.0.4/setup.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2023-07-17 11:00:09.658316 quadkey-boosted-1.0.4/tests/
+-rw-rw-r--   0 home      (1000) home      (1000)      688 2023-07-16 16:50:38.000000 quadkey-boosted-1.0.4/tests/test_quadkey_c_.py
```

### Comparing `quadkey-boosted-1.0.3/LICENSE` & `quadkey-boosted-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quadkey-boosted-1.0.3/PKG-INFO` & `quadkey-boosted-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: quadkey-boosted
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library that provides a powerful set of tools and functions for working with quadkeys. Built on top of C it offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
-Home-page: https://github.com/ls-da3m0ns/pyquadkey-boosted
+Home-page: https://github.com/ls-da3m0ns/quadkey-boosted
 Author: Prashant Singh
 Author-email: mail.prashantsingh.41@gmail.com
-Project-URL: Documentation, https://github.com/lsda3m0ns/pyquadkey-boosted
-Project-URL: Source Code, https://github.com/lsda3m0ns/pyquadkey-boosted
-Project-URL: Bug Tracker, https://github.com/lsda3m0ns/pyquadkey-boosted/issues
+Project-URL: Documentation, https://github.com/ls-da3m0ns/quadkey-boosted
+Project-URL: Source Code, https://github.com/ls-da3m0ns/quadkey-boosted
+Project-URL: Bug Tracker, https://github.com/ls-da3m0ns/quadkey-boosted/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# pyquadkey-boosted
+# quadkey-boosted
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
 ## Description
-pyquadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, pyquadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
+quadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, quadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
 
 ## Key Features
  * Available API's
    * Conversion
       * lat lng to QuadKey
       * QuadKey to lat lng
       * QuadKey to BingTile
@@ -64,15 +64,15 @@
 
 ## Installation
 ### Requirements
    This library requires **Python 3.6** or higher. To compile it from source, Cython is required in addition.
 
 ### using pip
 ```bash
-pip install pyquadkey-boosted
+pip install quadkey-boosted
 ```
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
 * `python3-devel`
@@ -80,15 +80,15 @@
     * Ubuntu / Debian: `apt install python3-dev`
 
 #### Prerequisites (`Windows`)
 * Visual C++ Build Tools 2015 (with Windows 10 SDK) (see [here](https://devblogs.microsoft.com/python/unable-to-find-vcvarsall-bat/#i-need-a-package-that-has-no-wheel-what-can-i-do))
 #### Build from source
 ```bash
 # Clone  repo
-git clone https://github.com/ls-da3m0ns/pyquadkey-boosted
+git clone https://github.com/ls-da3m0ns/quadkey-boosted
 
 # Create Virtual Environment
 python -m venv ./venv
 source venv/bin/activate
 
 # Install dependencies
 pip install -r requirements.txt
```

### Comparing `quadkey-boosted-1.0.3/README.md` & `quadkey-boosted-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
-# pyquadkey-boosted
+# quadkey-boosted
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
 ## Description
-pyquadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, pyquadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
+quadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, quadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
 
 ## Key Features
  * Available API's
    * Conversion
       * lat lng to QuadKey
       * QuadKey to lat lng
       * QuadKey to BingTile
@@ -45,15 +45,15 @@
 
 ## Installation
 ### Requirements
    This library requires **Python 3.6** or higher. To compile it from source, Cython is required in addition.
 
 ### using pip
 ```bash
-pip install pyquadkey-boosted
+pip install quadkey-boosted
 ```
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
 * `python3-devel`
@@ -61,15 +61,15 @@
     * Ubuntu / Debian: `apt install python3-dev`
 
 #### Prerequisites (`Windows`)
 * Visual C++ Build Tools 2015 (with Windows 10 SDK) (see [here](https://devblogs.microsoft.com/python/unable-to-find-vcvarsall-bat/#i-need-a-package-that-has-no-wheel-what-can-i-do))
 #### Build from source
 ```bash
 # Clone  repo
-git clone https://github.com/ls-da3m0ns/pyquadkey-boosted
+git clone https://github.com/ls-da3m0ns/quadkey-boosted
 
 # Create Virtual Environment
 python -m venv ./venv
 source venv/bin/activate
 
 # Install dependencies
 pip install -r requirements.txt
```

### Comparing `quadkey-boosted-1.0.3/quadkey/core/__init__.py` & `quadkey-boosted-1.0.4/quadkey/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quadkey-boosted-1.0.3/quadkey/core/test_c_code.py` & `quadkey-boosted-1.0.4/quadkey/core/test_c_code.py`

 * *Files identical despite different names*

### Comparing `quadkey-boosted-1.0.3/quadkey/core/utils.c` & `quadkey-boosted-1.0.4/quadkey/core/utils.c`

 * *Files identical despite different names*

### Comparing `quadkey-boosted-1.0.3/quadkey/core/utils.pyx` & `quadkey-boosted-1.0.4/quadkey/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `quadkey-boosted-1.0.3/quadkey/quadkey_boosted.egg-info/PKG-INFO` & `quadkey-boosted-1.0.4/quadkey/quadkey_boosted.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: quadkey-boosted
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library that provides a powerful set of tools and functions for working with quadkeys. Built on top of C it offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
-Home-page: https://github.com/ls-da3m0ns/pyquadkey-boosted
+Home-page: https://github.com/ls-da3m0ns/quadkey-boosted
 Author: Prashant Singh
 Author-email: mail.prashantsingh.41@gmail.com
-Project-URL: Documentation, https://github.com/lsda3m0ns/pyquadkey-boosted
-Project-URL: Source Code, https://github.com/lsda3m0ns/pyquadkey-boosted
-Project-URL: Bug Tracker, https://github.com/lsda3m0ns/pyquadkey-boosted/issues
+Project-URL: Documentation, https://github.com/ls-da3m0ns/quadkey-boosted
+Project-URL: Source Code, https://github.com/ls-da3m0ns/quadkey-boosted
+Project-URL: Bug Tracker, https://github.com/ls-da3m0ns/quadkey-boosted/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# pyquadkey-boosted
+# quadkey-boosted
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
 ## Description
-pyquadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, pyquadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
+quadkey-boosted is a high-performance Python library that provides a powerful set of tools and functions for working with quadkeys, enabling seamless integration of tile-based mapping systems into your Python applications. Built on top of a blazing-fast C implementation, quadkey-boosted offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.
 
 ## Key Features
  * Available API's
    * Conversion
       * lat lng to QuadKey
       * QuadKey to lat lng
       * QuadKey to BingTile
@@ -64,15 +64,15 @@
 
 ## Installation
 ### Requirements
    This library requires **Python 3.6** or higher. To compile it from source, Cython is required in addition.
 
 ### using pip
 ```bash
-pip install pyquadkey-boosted
+pip install quadkey-boosted
 ```
 ### From source
 #### Prerequisites (`Linux`)
 * `gcc`
     * Fedora: `dnf install @development-tools`
     * Ubuntu / Debian: `apt install build-essential`
 * `python3-devel`
@@ -80,15 +80,15 @@
     * Ubuntu / Debian: `apt install python3-dev`
 
 #### Prerequisites (`Windows`)
 * Visual C++ Build Tools 2015 (with Windows 10 SDK) (see [here](https://devblogs.microsoft.com/python/unable-to-find-vcvarsall-bat/#i-need-a-package-that-has-no-wheel-what-can-i-do))
 #### Build from source
 ```bash
 # Clone  repo
-git clone https://github.com/ls-da3m0ns/pyquadkey-boosted
+git clone https://github.com/ls-da3m0ns/quadkey-boosted
 
 # Create Virtual Environment
 python -m venv ./venv
 source venv/bin/activate
 
 # Install dependencies
 pip install -r requirements.txt
```

### Comparing `quadkey-boosted-1.0.3/setup.py` & `quadkey-boosted-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from Cython.Build import cythonize
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="quadkey-boosted",
-    version="1.0.3",
+    version="1.0.4",
     author="Prashant Singh",
     author_email="mail.prashantsingh.41@gmail.com",
     description="Python library that provides a powerful set of tools and functions for working with quadkeys. Built on top of C it offers lightning-fast calculations, ensuring optimal performance even with large-scale datasets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ls-da3m0ns/pyquadkey-boosted",
+    url="https://github.com/ls-da3m0ns/quadkey-boosted",
     ext_modules=cythonize(
         [ 
             Extension("quadkey.core.utils", 
                 sources=["quadkey/core/utils.pyx"], 
                 language="c", optional=False, include_dirs=[get_python_inc()]) ]),
     packages=find_packages('quadkey'),
     include_dirs=[get_python_inc()],
@@ -33,17 +33,17 @@
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires='>=3.6',
     project_urls={
-        'Documentation': 'https://github.com/lsda3m0ns/pyquadkey-boosted',
-        'Source Code': 'https://github.com/lsda3m0ns/pyquadkey-boosted',
-        'Bug Tracker': 'https://github.com/lsda3m0ns/pyquadkey-boosted/issues',
+        'Documentation': 'https://github.com/ls-da3m0ns/quadkey-boosted',
+        'Source Code': 'https://github.com/ls-da3m0ns/quadkey-boosted',
+        'Bug Tracker': 'https://github.com/ls-da3m0ns/quadkey-boosted/issues',
     },
     entry_points={
         'console_scripts': [
             'quadkey = quadkey.__main__:main',
         ],
     },
     ext_package="quadkey",
```

### Comparing `quadkey-boosted-1.0.3/tests/test_quadkey_c_.py` & `quadkey-boosted-1.0.4/tests/test_quadkey_c_.py`

 * *Files identical despite different names*

