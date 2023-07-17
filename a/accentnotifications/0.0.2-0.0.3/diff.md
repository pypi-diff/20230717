# Comparing `tmp/accentnotifications-0.0.2.tar.gz` & `tmp/accentnotifications-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentnotifications-0.0.2.tar", last modified: Wed Oct 12 08:50:43 2022, max compression
+gzip compressed data, was "accentnotifications-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentnotifications-0.0.2.tar` & `accentnotifications-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,14 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.2/.flake8
--rw-r--r--   0        0        0      921 2022-10-05 15:56:51.000000 accentnotifications-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentnotifications-0.0.2/.gitignore
--rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.2/LICENSE
--rw-r--r--   0        0        0      418 2022-10-10 10:41:36.000000 accentnotifications-0.0.2/README.md
--rw-r--r--   0        0        0       81 2022-10-11 14:09:50.000000 accentnotifications-0.0.2/accentnotifications/__init__.py
--rw-r--r--   0        0        0      264 2022-10-11 14:10:19.000000 accentnotifications-0.0.2/accentnotifications/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      667 2022-10-11 13:07:42.000000 accentnotifications-0.0.2/accentnotifications/__pycache__/manager.cpython-310.pyc
--rw-r--r--   0        0        0      963 2022-10-10 08:38:59.000000 accentnotifications-0.0.2/accentnotifications/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.2/accentnotifications/manager.py
--rw-r--r--   0        0        0       48 2022-10-08 14:36:15.000000 accentnotifications-0.0.2/accentnotifications/notifications/__init__.py
--rw-r--r--   0        0        0      256 2022-10-08 14:36:37.000000 accentnotifications-0.0.2/accentnotifications/notifications/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1930 2022-10-11 14:02:43.000000 accentnotifications-0.0.2/accentnotifications/notifications/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3263 2022-10-11 14:02:43.000000 accentnotifications-0.0.2/accentnotifications/notifications/__pycache__/smtp.cpython-310.pyc
--rw-r--r--   0        0        0      848 2022-10-12 08:48:23.000000 accentnotifications-0.0.2/accentnotifications/notifications/base.py
--rw-r--r--   0        0        0     2755 2022-10-12 08:48:23.000000 accentnotifications-0.0.2/accentnotifications/notifications/smtp.py
--rw-r--r--   0        0        0      618 2022-10-10 08:37:39.000000 accentnotifications-0.0.2/accentnotifications/types.py
--rw-r--r--   0        0        0     1279 2022-10-10 11:15:09.000000 accentnotifications-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 accentnotifications-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentnotifications-0.0.3/.flake8
+-rw-r--r--   0        0        0      929 2023-07-17 11:26:35.290624 accentnotifications-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      109 2023-07-17 09:30:14.313081 accentnotifications-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1089 2022-10-07 18:12:15.000000 accentnotifications-0.0.3/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-17 09:30:14.314070 accentnotifications-0.0.3/README.md
+-rw-r--r--   0        0        0       81 2023-07-17 11:28:59.265857 accentnotifications-0.0.3/accentnotifications/__init__.py
+-rw-r--r--   0        0        0      246 2022-10-12 08:48:23.000000 accentnotifications-0.0.3/accentnotifications/manager.py
+-rw-r--r--   0        0        0      112 2023-07-17 09:30:14.314592 accentnotifications-0.0.3/accentnotifications/notifications/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-17 11:16:34.607700 accentnotifications-0.0.3/accentnotifications/notifications/base.py
+-rw-r--r--   0        0        0     2845 2023-07-17 11:16:33.855651 accentnotifications-0.0.3/accentnotifications/notifications/smtp.py
+-rw-r--r--   0        0        0     3038 2023-07-17 11:16:34.605170 accentnotifications-0.0.3/accentnotifications/notifications/twilio_sms.py
+-rw-r--r--   0        0        0     1670 2023-07-17 11:16:15.640920 accentnotifications-0.0.3/accentnotifications/types.py
+-rw-r--r--   0        0        0     1363 2023-07-17 09:34:24.491649 accentnotifications-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 accentnotifications-0.0.3/PKG-INFO
```

### Comparing `accentnotifications-0.0.2/.github/workflows/test.yml` & `accentnotifications-0.0.3/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     types: [opened, synchronize]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `accentnotifications-0.0.2/LICENSE` & `accentnotifications-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accentnotifications-0.0.2/accentnotifications/notifications/smtp.py` & `accentnotifications-0.0.3/accentnotifications/notifications/smtp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from email.message import Message
 from typing import Optional, Type
 
+from pydantic_settings import SettingsConfigDict
+
 try:
     from aiosmtplib import SMTP
 except ImportError:  # pragma: no cover
     SMTP = None
 
 from pydantic import SecretStr
 
@@ -14,28 +15,30 @@
 
 
 class SmtpResponse(BaseResponse):
     success: bool
 
 
 class SmtpNotification(BaseNotification):
+    model_config = SettingsConfigDict(
+        arbitrary_types_allowed=True,
+        env_prefix="notifications_smtp_",
+        # json_encoders={Message: lambda v: v.as_string()}
+    )
+
     host: str
     port: int
     username: Optional[SecretStr] = None
     password: Optional[SecretStr] = None
     use_tls: bool = False
     starttls: bool = False
     timeout: Optional[int] = None
     fail_silently: bool = False
     email: Email
-    response: SmtpResponse = None
-
-    class Config:
-        env_prefix = "notifications_smtp_"
-        json_encoders = {Message: lambda v: v.as_string()}
+    response: Optional[SmtpResponse] = None
 
     @property
     def backend(self) -> Type["SmtpBackend"]:
         return SmtpBackend
 
 
 class SmtpBackend(BaseBackend):
```

### Comparing `accentnotifications-0.0.2/pyproject.toml` & `accentnotifications-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "pydantic",
+    "pydantic>=2.0.1,<2.1.0",
+    "pydantic-settings>=2.0.1,<2.1.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Homepage = "https://github.com/accentdesign/accentnotifications"
 
 [project.optional-dependencies]
@@ -38,14 +39,18 @@
     "autoflake",
     "flake8",
 ]
 smtp = [
     "aiosmtplib"
 ]
 
+twiliosms = [
+    "aiohttp"
+]
+
 [tool.flit.sdist]
 include = [
     "accentnotifications/"
 ]
 exclude = [
     "example/",
     "scripts/",
```

### Comparing `accentnotifications-0.0.2/PKG-INFO` & `accentnotifications-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 Metadata-Version: 2.1
 Name: accentnotifications
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sending various forms of notifications such as smtp
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.0.1,<2.1.0
+Requires-Dist: pydantic-settings>=2.0.1,<2.1.0
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: aiosmtplib ; extra == "smtp"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: isort ; extra == "test"
+Requires-Dist: aiohttp ; extra == "twiliosms"
 Project-URL: Homepage, https://github.com/accentdesign/accentnotifications
 Provides-Extra: dev
 Provides-Extra: smtp
 Provides-Extra: test
+Provides-Extra: twiliosms
 
 [![Test](https://github.com/accentdesign/accentnotifications/actions/workflows/test.yml/badge.svg)](https://github.com/accentdesign/accentnotifications/actions/workflows/test.yml)
 
 ---
 **Source Code**: <a href="https://github.com/accentdesign/accentnotifications" target="_blank">https://github.com/accentdesign/accentnotifications</a>
 ---
 
 ## Installation
 
 For smtp:
 ```bash
 pip install accentnotifications[smtp]
 ```
 
+For twilio sms:
+```bash
+pip install accentnotifications[twiliosms]
+```
+
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.2 Summary: Sending
+Metadata-Version: 2.1 Name: accentnotifications Version: 0.0.3 Summary: Sending
 various forms of notifications such as smtp Author-email: Accent Design Group
 Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Requires-Dist: pydantic Requires-Dist: autoflake ; extra == "dev" Requires-
-Dist: flake8 ; extra == "dev" Requires-Dist: aiosmtplib ; extra == "smtp"
-Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-asyncio ; extra
-== "test" Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: pytest-
-mock ; extra == "test" Requires-Dist: mypy ; extra == "test" Requires-Dist:
-flake8 ; extra == "test" Requires-Dist: black ; extra == "test" Requires-Dist:
-isort ; extra == "test" Project-URL: Homepage, https://github.com/accentdesign/
-accentnotifications Provides-Extra: dev Provides-Extra: smtp Provides-Extra:
-test [![Test](https://github.com/accentdesign/accentnotifications/actions/
-workflows/test.yml/badge.svg)](https://github.com/accentdesign/
-accentnotifications/actions/workflows/test.yml) --- **Source Code**: https://
-github.com/accentdesign/accentnotifications --- ## Installation For smtp:
-```bash pip install accentnotifications[smtp] ```
+Requires-Dist: pydantic>=2.0.1,<2.1.0 Requires-Dist: pydantic-
+settings>=2.0.1,<2.1.0 Requires-Dist: autoflake ; extra == "dev" Requires-Dist:
+flake8 ; extra == "dev" Requires-Dist: aiosmtplib ; extra == "smtp" Requires-
+Dist: pytest ; extra == "test" Requires-Dist: pytest-asyncio ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: pytest-mock ; extra
+== "test" Requires-Dist: mypy ; extra == "test" Requires-Dist: flake8 ; extra
+== "test" Requires-Dist: black ; extra == "test" Requires-Dist: isort ; extra
+== "test" Requires-Dist: aiohttp ; extra == "twiliosms" Project-URL: Homepage,
+https://github.com/accentdesign/accentnotifications Provides-Extra: dev
+Provides-Extra: smtp Provides-Extra: test Provides-Extra: twiliosms [![Test]
+(https://github.com/accentdesign/accentnotifications/actions/workflows/
+test.yml/badge.svg)](https://github.com/accentdesign/accentnotifications/
+actions/workflows/test.yml) --- **Source Code**: https://github.com/
+accentdesign/accentnotifications --- ## Installation For smtp: ```bash pip
+install accentnotifications[smtp] ``` For twilio sms: ```bash pip install
+accentnotifications[twiliosms] ```
```

