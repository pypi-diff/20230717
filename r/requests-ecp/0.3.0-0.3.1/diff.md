# Comparing `tmp/requests-ecp-0.3.0.tar.gz` & `tmp/requests-ecp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-ecp-0.3.0.tar", last modified: Wed Oct 26 14:16:34 2022, max compression
+gzip compressed data, was "requests-ecp-0.3.1.tar", last modified: Mon Jul 17 20:58:16 2023, max compression
```

## Comparing `requests-ecp-0.3.0.tar` & `requests-ecp-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-12-16 06:26:02.000000 requests-ecp-0.3.0/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2021-03-18 15:37:19.000000 requests-ecp-0.3.0/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3110 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2021-03-19 14:27:03.000000 requests-ecp-0.3.0/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1378 2022-10-26 14:14:57.000000 requests-ecp-0.3.0/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-12-16 06:26:02.000000 requests-ecp-0.3.0/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1035 2021-11-22 09:58:42.000000 requests-ecp-0.3.0/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1048 2020-12-16 06:26:02.000000 requests-ecp-0.3.0/debian/copyright
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      234 2021-11-17 10:00:12.000000 requests-ecp-0.3.0/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-12-16 06:26:02.000000 requests-ecp-0.3.0/debian/source/format
--rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2022-10-26 13:07:44.000000 requests-ecp-0.3.0/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3108 2022-10-26 14:14:57.000000 requests-ecp-0.3.0/requests-ecp.spec
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/requests_ecp/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1188 2022-10-26 14:14:57.000000 requests-ecp-0.3.0/requests_ecp/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9464 2022-10-26 13:07:44.000000 requests-ecp-0.3.0/requests_ecp/auth.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6946 2022-10-24 14:19:14.000000 requests-ecp-0.3.0/requests_ecp/ecp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3976 2022-10-26 13:07:44.000000 requests-ecp-0.3.0/requests_ecp/session.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/requests_ecp/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      782 2022-10-24 09:52:45.000000 requests-ecp-0.3.0/requests_ecp/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9106 2022-10-26 13:07:44.000000 requests-ecp-0.3.0/requests_ecp/tests/test_auth.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6922 2022-10-24 14:19:14.000000 requests-ecp-0.3.0/requests_ecp/tests/test_ecp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2232 2022-10-24 14:19:14.000000 requests-ecp-0.3.0/requests_ecp/tests/test_session.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/requests_ecp.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3110 2022-10-26 14:16:34.000000 requests-ecp-0.3.0/requests_ecp.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      576 2022-10-26 14:16:34.000000 requests-ecp-0.3.0/requests_ecp.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2022-10-26 14:16:34.000000 requests-ecp-0.3.0/requests_ecp.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      184 2022-10-26 14:16:34.000000 requests-ecp-0.3.0/requests_ecp.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       13 2022-10-26 14:16:34.000000 requests-ecp-0.3.0/requests_ecp.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1450 2022-10-26 14:16:34.461630 requests-ecp-0.3.0/setup.cfg
--rw-r--r--   0 duncan    (1000) duncan    (1000)      886 2021-11-22 09:58:42.000000 requests-ecp-0.3.0/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.748123 requests-ecp-0.3.1/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-12-16 06:26:02.000000 requests-ecp-0.3.1/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2021-03-18 15:37:19.000000 requests-ecp-0.3.1/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3214 2023-07-17 20:58:16.748123 requests-ecp-0.3.1/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1876 2023-07-17 16:46:45.000000 requests-ecp-0.3.1/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.738123 requests-ecp-0.3.1/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1525 2023-07-17 20:54:50.000000 requests-ecp-0.3.1/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-12-16 06:26:02.000000 requests-ecp-0.3.1/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1035 2023-06-19 10:35:33.000000 requests-ecp-0.3.1/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1048 2020-12-16 06:26:02.000000 requests-ecp-0.3.1/debian/copyright
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      234 2021-11-17 10:00:12.000000 requests-ecp-0.3.1/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.738123 requests-ecp-0.3.1/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-12-16 06:26:02.000000 requests-ecp-0.3.1/debian/source/format
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3113 2023-07-17 20:54:50.000000 requests-ecp-0.3.1/requests-ecp.spec
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.738123 requests-ecp-0.3.1/requests_ecp/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1188 2023-07-17 20:54:50.000000 requests-ecp-0.3.1/requests_ecp/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9464 2023-06-19 10:35:33.000000 requests-ecp-0.3.1/requests_ecp/auth.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6946 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/ecp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3976 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/session.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.748123 requests-ecp-0.3.1/requests_ecp/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      782 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9106 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/tests/test_auth.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6922 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/tests/test_ecp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2232 2022-11-03 10:02:44.000000 requests-ecp-0.3.1/requests_ecp/tests/test_session.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 20:58:16.738123 requests-ecp-0.3.1/requests_ecp.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3214 2023-07-17 20:58:16.000000 requests-ecp-0.3.1/requests_ecp.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      576 2023-07-17 20:58:16.000000 requests-ecp-0.3.1/requests_ecp.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-07-17 20:58:16.000000 requests-ecp-0.3.1/requests_ecp.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      184 2023-07-17 20:58:16.000000 requests-ecp-0.3.1/requests_ecp.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       13 2023-07-17 20:58:16.000000 requests-ecp-0.3.1/requests_ecp.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1530 2023-07-17 20:58:16.748123 requests-ecp-0.3.1/setup.cfg
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      886 2021-11-22 09:58:42.000000 requests-ecp-0.3.1/setup.py
```

### Comparing `requests-ecp-0.3.0/LICENSE` & `requests-ecp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/PKG-INFO` & `requests-ecp-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-ecp
-Version: 0.3.0
+Version: 0.3.1
 Summary: SAML/ECP authentication handler for python-requests
 Home-page: https://pypi.org/project/requests-ecp/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/requests-ecp/issues
 Project-URL: Documentation, https://requests-ecp.readthedocs.io/
@@ -16,14 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
@@ -38,15 +40,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/requests-ecp.svg)](https://anaconda.org/conda-forge/requests-ecp/)  
 [![DOI](https://zenodo.org/badge/238942798.svg)](https://zenodo.org/badge/latestdoi/238942798)
 [![License](https://img.shields.io/pypi/l/requests-ecp.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/requests-ecp.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml)
 [![Codecov](https://codecov.io/gh/duncanmmacleod/requests-ecp/branch/main/graph/badge.svg?token=PO7lRIPpTm)](https://codecov.io/gh/duncanmmacleod/requests-ecp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9b10bd39e588fd5a34ab/maintainability)](https://codeclimate.com/github/duncanmmacleod/requests-ecp/maintainability)
 [![Documentation](https://readthedocs.org/projects/requests-ecp/badge/?version=latest)](https://requests-ecp.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://requests-ecp.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `requests-ecp-0.3.0/README.md` & `requests-ecp-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/requests-ecp.svg)](https://anaconda.org/conda-forge/requests-ecp/)  
 [![DOI](https://zenodo.org/badge/238942798.svg)](https://zenodo.org/badge/latestdoi/238942798)
 [![License](https://img.shields.io/pypi/l/requests-ecp.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/requests-ecp.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml)
 [![Codecov](https://codecov.io/gh/duncanmmacleod/requests-ecp/branch/main/graph/badge.svg?token=PO7lRIPpTm)](https://codecov.io/gh/duncanmmacleod/requests-ecp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9b10bd39e588fd5a34ab/maintainability)](https://codeclimate.com/github/duncanmmacleod/requests-ecp/maintainability)
 [![Documentation](https://readthedocs.org/projects/requests-ecp/badge/?version=latest)](https://requests-ecp.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://requests-ecp.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `requests-ecp-0.3.0/debian/changelog` & `requests-ecp-0.3.1/debian/changelog`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+requests-ecp (0.3.1-1) unstable; urgency=low
+
+  * update for 0.3.1
+
+ -- Duncan Macleod <duncan.macleod@ligo.org>  Mon, 17 Jul 2023 21:34:00 +0100
+
 requests-ecp (0.3.0-1) unstable; urgency=low
 
   * update for 0.3.0
   * remove unnecessary patches for requests-kerberos, which
     is now optional in the Python metadata
 
  -- Duncan Macleod <duncan.macleod@ligo.org>  Wed, 26 Oct 2022 14:56:00 +0100
```

### Comparing `requests-ecp-0.3.0/debian/control` & `requests-ecp-0.3.1/debian/control`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/debian/copyright` & `requests-ecp-0.3.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests-ecp.spec` & `requests-ecp-0.3.1/requests-ecp.spec`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define name requests-ecp
-%define version 0.3.0
+%define version 0.3.1
 %define release 1
 
 # -- metadata ---------------
 
 BuildArch: noarch
 Group:     Development/Libraries
 License:   GPLv3+
@@ -15,18 +15,15 @@
 Summary:   A SAML/ECP authentication handler for python-requests
 Url:       https://github.com/duncanmmacleod/requests-ecp
 Vendor:    Duncan Macleod <duncan.macleod@ligo.org>
 Version:   %{version}
 
 # -- build requirements -----
 
-BuildRequires: python-srpm-macros
-BuildRequires: python-rpm-macros
-BuildRequires: /usr/bin/python3
-BuildRequires: python3-rpm-macros
+BuildRequires: python%{python3_pkgversion}-devel
 BuildRequires: python%{python3_pkgversion}-lxml
 BuildRequires: python%{python3_pkgversion}-requests
 BuildRequires: python%{python3_pkgversion}-requests-gssapi >= 1.2.2
 BuildRequires: python%{python3_pkgversion}-setuptools >= 30.3.0
 %if 0%{?rhel} == 0 || 0%{?rhel} >= 8
 BuildRequires: python%{python3_pkgversion}-pytest
 BuildRequires: python%{python3_pkgversion}-requests-mock
@@ -77,14 +74,17 @@
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 # -- changelog --------------
 
 %changelog
+* Mon Jul 17 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.3.1-1
+- update for 0.3.1
+
 * Wed Oct 26 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.3.0-1
 - update for 0.3.0
 
 * Mon Nov 22 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.2.3-1
 - update for 0.2.3
 - use python3-gssapi as the kerberos backend
```

### Comparing `requests-ecp-0.3.0/requests_ecp/__init__.py` & `requests-ecp-0.3.1/requests_ecp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     >>> from request_ecp import Session
     >>> with Session(idp="https://idp.example.com/SAML/SOAP/ECP") as sess:
     ...     sess.get("https://private.example.com/data")
 
 """
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 from .auth import HTTPECPAuth
 from .session import (
     ECPAuthSessionMixin,
     Session,
 )
```

### Comparing `requests-ecp-0.3.0/requests_ecp/auth.py` & `requests-ecp-0.3.1/requests_ecp/auth.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/ecp.py` & `requests-ecp-0.3.1/requests_ecp/ecp.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/session.py` & `requests-ecp-0.3.1/requests_ecp/session.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/tests/__init__.py` & `requests-ecp-0.3.1/requests_ecp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/tests/test_auth.py` & `requests-ecp-0.3.1/requests_ecp/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/tests/test_ecp.py` & `requests-ecp-0.3.1/requests_ecp/tests/test_ecp.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp/tests/test_session.py` & `requests-ecp-0.3.1/requests_ecp/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/requests_ecp.egg-info/PKG-INFO` & `requests-ecp-0.3.1/requests_ecp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-ecp
-Version: 0.3.0
+Version: 0.3.1
 Summary: SAML/ECP authentication handler for python-requests
 Home-page: https://pypi.org/project/requests-ecp/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/requests-ecp/issues
 Project-URL: Documentation, https://requests-ecp.readthedocs.io/
@@ -16,14 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
@@ -38,15 +40,15 @@
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/requests-ecp.svg)](https://anaconda.org/conda-forge/requests-ecp/)  
 [![DOI](https://zenodo.org/badge/238942798.svg)](https://zenodo.org/badge/latestdoi/238942798)
 [![License](https://img.shields.io/pypi/l/requests-ecp.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/requests-ecp.svg)
 
 ## Development status
 
-[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/build.yml)
+[![Build status](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/duncanmmacleod/requests-ecp/actions/workflows/python.yml)
 [![Codecov](https://codecov.io/gh/duncanmmacleod/requests-ecp/branch/main/graph/badge.svg?token=PO7lRIPpTm)](https://codecov.io/gh/duncanmmacleod/requests-ecp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9b10bd39e588fd5a34ab/maintainability)](https://codeclimate.com/github/duncanmmacleod/requests-ecp/maintainability)
 [![Documentation](https://readthedocs.org/projects/requests-ecp/badge/?version=latest)](https://requests-ecp.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 See https://requests-ecp.readthedocs.io/en/latest/#installation for installation instructions.
```

### Comparing `requests-ecp-0.3.0/requests_ecp.egg-info/SOURCES.txt` & `requests-ecp-0.3.1/requests_ecp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `requests-ecp-0.3.0/setup.cfg` & `requests-ecp-0.3.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 project_urls = 
 	Bug Tracker = https://github.com/duncanmmacleod/requests-ecp/issues
 	Documentation = https://requests-ecp.readthedocs.io/
 	Source Code = https://github.com/duncanmmacleod/requests-ecp/
 
 [options]
```

### Comparing `requests-ecp-0.3.0/setup.py` & `requests-ecp-0.3.1/setup.py`

 * *Files identical despite different names*

