# Comparing `tmp/msoffcrypto_tool-5.0.1rc1.tar.gz` & `tmp/msoffcrypto_tool-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msoffcrypto_tool-5.0.1rc1.tar", max compression
+gzip compressed data, was "msoffcrypto_tool-5.1.0.tar", max compression
```

## Comparing `msoffcrypto_tool-5.0.1rc1.tar` & `msoffcrypto_tool-5.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-02-27 20:12:33.110214 msoffcrypto_tool-5.0.1rc1/LICENSE.txt
--rw-r--r--   0        0        0     7232 2023-02-27 20:12:33.110214 msoffcrypto_tool-5.0.1rc1/README.md
--rw-r--r--   0        0        0     2907 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/__init__.py
--rw-r--r--   0        0        0     2469 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/__main__.py
--rw-r--r--   0        0        0      473 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/__init__.py
--rw-r--r--   0        0        0      398 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/base.py
--rw-r--r--   0        0        0     1669 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/common.py
--rw-r--r--   0        0        0    15749 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/doc97.py
--rw-r--r--   0        0        0     9426 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/ooxml.py
--rw-r--r--   0        0        0    28417 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/ppt97.py
--rw-r--r--   0        0        0    18537 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/xls97.py
--rw-r--r--   0        0        0        0 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/__init__.py
--rw-r--r--   0        0        0     7994 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/ecma376_agile.py
--rw-r--r--   0        0        0       62 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/ecma376_extensible.py
--rw-r--r--   0        0        0     3922 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/ecma376_standard.py
--rw-r--r--   0        0        0     3052 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/rc4.py
--rw-r--r--   0        0        0     2500 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/rc4_cryptoapi.py
--rw-r--r--   0        0        0        0 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/xor_obfuscation.py
--rw-r--r--   0        0        0     1016 2023-02-27 20:12:33.114214 msoffcrypto_tool-5.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     8334 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.0.1rc1/setup.py
--rw-r--r--   0        0        0     7991 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     7413 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/README.md
+-rw-r--r--   0        0        0     3056 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/__init__.py
+-rw-r--r--   0        0        0     2469 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/__main__.py
+-rw-r--r--   0        0        0      473 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/base.py
+-rw-r--r--   0        0        0     1669 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/common.py
+-rw-r--r--   0        0        0    15749 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/doc97.py
+-rw-r--r--   0        0        0    11208 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/ooxml.py
+-rw-r--r--   0        0        0    28417 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/ppt97.py
+-rw-r--r--   0        0        0    18537 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/format/xls97.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/__init__.py
+-rw-r--r--   0        0        0     7994 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/ecma376_agile.py
+-rw-r--r--   0        0        0       62 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/ecma376_extensible.py
+-rw-r--r--   0        0        0     3922 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/ecma376_standard.py
+-rw-r--r--   0        0        0     3052 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/rc4.py
+-rw-r--r--   0        0        0     2500 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/rc4_cryptoapi.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/msoffcrypto/method/xor_obfuscation.py
+-rw-r--r--   0        0        0     1012 2023-07-17 09:58:53.058032 msoffcrypto_tool-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8169 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.1.0/PKG-INFO
```

### Comparing `msoffcrypto_tool-5.0.1rc1/LICENSE.txt` & `msoffcrypto_tool-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/README.md` & `msoffcrypto_tool-5.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 * [ ] Isolate parser
 
 ## Resources
 
 * "Backdooring MS Office documents with secret master keys" <http://secuinside.com/archive/2015/2015-1-9.pdf>
 * Technical Documents <https://msdn.microsoft.com/en-us/library/cc313105.aspx>
   * [MS-OFFCRYPTO] Agile Encryption <https://msdn.microsoft.com/en-us/library/dd949735(v=office.12).aspx>
+* [MS-OFFDI] Microsoft Office File Format Documentation Introduction <https://learn.microsoft.com/en-us/openspecs/office_file_formats/ms-offdi/24ed256c-eb5b-494e-b4f6-fb696ad2b4dc>
 * LibreOffice/core <https://github.com/LibreOffice/core>
 * LibreOffice/mso-dumper <https://github.com/LibreOffice/mso-dumper>
 * wvDecrypt <http://www.skynet.ie/~caolan/Packages/wvDecrypt.html>
 * Microsoft Office password protection - Wikipedia <https://en.wikipedia.org/wiki/Microsoft_Office_password_protection#History_of_Microsoft_Encryption_password>
 * office2john.py <https://github.com/magnumripper/JohnTheRipper/blob/bleeding-jumbo/run/office2john.py>
 
 ## Alternatives
```

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/__init__.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-import olefile
+import sys
 import zipfile
-import pkg_resources
+
+import olefile
 
 from msoffcrypto import exceptions
 
-__version__ = pkg_resources.get_distribution("msoffcrypto-tool").version
+if sys.version_info >= (3, 8):
+    from importlib import metadata
+
+    __version__ = metadata.version("msoffcrypto-tool")
+else:
+    import pkg_resources
+
+    __version__ = pkg_resources.get_distribution("msoffcrypto-tool").version
 
 
 def OfficeFile(file):
     """Return an office file object based on the format of given file.
 
     Args:
         file (:obj:`_io.BufferedReader`): Input file.
```

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/__main__.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/__main__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/common.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/format/common.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/doc97.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/format/doc97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/ooxml.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/format/ooxml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,45 @@
+import base64
+import io
 import logging
-import base64, io
+import zipfile
 from struct import unpack
 from xml.dom.minidom import parseString
-import zipfile
 
 import olefile
 
 from msoffcrypto import exceptions
 from msoffcrypto.format import base
 from msoffcrypto.format.common import _parse_encryptionheader, _parse_encryptionverifier
 from msoffcrypto.method.ecma376_agile import ECMA376Agile
 from msoffcrypto.method.ecma376_standard import ECMA376Standard
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
+def _is_ooxml(file):
+    if not zipfile.is_zipfile(file):
+        return False
+    try:
+        zfile = zipfile.ZipFile(file)
+        with zfile.open("[Content_Types].xml") as stream:
+            xml = parseString(stream.read())
+            # Heuristic
+            if (
+                xml.documentElement.tagName == "Types"
+                and xml.documentElement.namespaceURI == "http://schemas.openxmlformats.org/package/2006/content-types"
+            ):
+                return True
+            else:
+                return False
+    except:
+        return False
+
+
 def _parseinfo_standard(ole):
     (headerFlags,) = unpack("<I", ole.read(4))
     (encryptionHeaderSize,) = unpack("<I", ole.read(4))
     block = ole.read(encryptionHeaderSize)
     blob = io.BytesIO(block)
     header = _parse_encryptionheader(blob)
     block = ole.read()
@@ -111,20 +131,26 @@
             if self.type == "agile":
                 # TODO: Support aliases?
                 self.keyTypes = ("password", "private_key", "secret_key")
             elif self.type == "standard":
                 self.keyTypes = ("password", "secret_key")
             elif self.type == "extensible":
                 pass
-        elif zipfile.is_zipfile(file):
-            raise exceptions.FileFormatError("Unencrypted document or unsupported file format")
+        elif _is_ooxml(file):
+            self.type = "plain"
+            self.file = file
         else:
             raise exceptions.FileFormatError("Unsupported file format")
 
     def load_key(self, password=None, private_key=None, secret_key=None, verify_password=False):
+        """
+        >>> with open("tests/outputs/ecma376standard_password_plain.docx", "rb") as f:
+        ...     officefile = OOXMLFile(f)
+        ...     officefile.load_key("1234")
+        """
         if password:
             if self.type == "agile":
                 self.secret_key = ECMA376Agile.makekey_from_password(
                     password,
                     self.info["passwordSalt"],
                     self.info["passwordHashAlgorithm"],
                     self.info["encryptedKeyValue"],
@@ -157,25 +183,37 @@
                     verified = ECMA376Standard.verifykey(
                         self.secret_key, self.info["verifier"]["encryptedVerifier"], self.info["verifier"]["encryptedVerifierHash"]
                     )
                     if not verified:
                         raise exceptions.InvalidKeyError("Key verification failed")
             elif self.type == "extensible":
                 pass
+            elif self.type == "plain":
+                pass
         elif private_key:
             if self.type == "agile":
                 self.secret_key = ECMA376Agile.makekey_from_privkey(private_key, self.info["encryptedKeyValue"])
             else:
                 raise exceptions.DecryptionError("Unsupported key type for the encryption method")
         elif secret_key:
             self.secret_key = secret_key
         else:
             raise exceptions.DecryptionError("No key specified")
 
     def decrypt(self, ofile, verify_integrity=False):
+        """
+        >>> from msoffcrypto import exceptions
+        >>> from io import BytesIO; ofile = BytesIO()
+        >>> with open("tests/outputs/ecma376standard_password_plain.docx", "rb") as f:
+        ...     officefile = OOXMLFile(f)
+        ...     officefile.load_key("1234")
+        ...     officefile.decrypt(ofile)
+        Traceback (most recent call last):
+        msoffcrypto.exceptions.DecryptionError: Unencrypted document
+        """
         if self.type == "agile":
             with self.file.openstream("EncryptedPackage") as stream:
                 if verify_integrity:
                     verified = ECMA376Agile.verify_integrity(
                         self.secret_key,
                         self.info["keyDataSalt"],
                         self.info["keyDataHashAlgorithm"],
@@ -189,20 +227,34 @@
 
                 obuf = ECMA376Agile.decrypt(self.secret_key, self.info["keyDataSalt"], self.info["keyDataHashAlgorithm"], stream)
             ofile.write(obuf)
         elif self.type == "standard":
             with self.file.openstream("EncryptedPackage") as stream:
                 obuf = ECMA376Standard.decrypt(self.secret_key, stream)
             ofile.write(obuf)
+        elif self.type == "plain":
+            raise exceptions.DecryptionError("Unencrypted document")
         else:
             raise exceptions.DecryptionError("Unsupported encryption method")
 
         # If the file is successfully decrypted, there must be a valid OOXML file, i.e. a valid zip file
         if not zipfile.is_zipfile(io.BytesIO(obuf)):
             raise exceptions.InvalidKeyError("The file could not be decrypted with this password")
 
     def is_encrypted(self):
+        """
+        >>> with open("tests/inputs/example_password.docx", "rb") as f:
+        ...     officefile = OOXMLFile(f)
+        ...     officefile.is_encrypted()
+        True
+        >>> with open("tests/outputs/ecma376standard_password_plain.docx", "rb") as f:
+        ...     officefile = OOXMLFile(f)
+        ...     officefile.is_encrypted()
+        False
+        """
         # Heuristic
-        if isinstance(self.file, olefile.OleFileIO):
+        if self.type == "plain":
+            return False
+        elif isinstance(self.file, olefile.OleFileIO):
             return True
         else:
             return False
```

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/ppt97.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/format/ppt97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/format/xls97.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/format/xls97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/ecma376_agile.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/method/ecma376_agile.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/ecma376_standard.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/method/ecma376_standard.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/rc4.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/method/rc4.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/msoffcrypto/method/rc4_cryptoapi.py` & `msoffcrypto_tool-5.1.0/msoffcrypto/method/rc4_cryptoapi.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.0.1rc1/pyproject.toml` & `msoffcrypto_tool-5.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msoffcrypto-tool"
-version = "5.0.1-rc1"
+version = "5.1.0"
 description = "Python tool and library for decrypting MS Office files with passwords or other keys"
 license = "MIT"
 homepage = "https://github.com/nolze/msoffcrypto-tool"
 authors = ["nolze <nolze@archlinux.us>"]
 readme = "README.md"
 packages = [{ include = "msoffcrypto" }]
```

### Comparing `msoffcrypto_tool-5.0.1rc1/setup.py` & `msoffcrypto_tool-5.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,228 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: msoffcrypto-tool
+Version: 5.1.0
+Summary: Python tool and library for decrypting MS Office files with passwords or other keys
+Home-page: https://github.com/nolze/msoffcrypto-tool
+License: MIT
+Author: nolze
+Author-email: nolze@archlinux.us
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=35.0)
+Requires-Dist: olefile (>=0.46)
+Description-Content-Type: text/markdown
 
-packages = \
-['msoffcrypto', 'msoffcrypto.format', 'msoffcrypto.method']
+# msoffcrypto-tool
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/msoffcrypto-tool.svg)](https://pypi.org/project/msoffcrypto-tool/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/msoffcrypto-tool.svg)](https://pypistats.org/packages/msoffcrypto-tool)
+[![build](https://github.com/nolze/msoffcrypto-tool/actions/workflows/ci.yaml/badge.svg)](https://github.com/nolze/msoffcrypto-tool/actions/workflows/ci.yaml)
+[![Coverage Status](https://codecov.io/gh/nolze/msoffcrypto-tool/branch/master/graph/badge.svg)](https://codecov.io/gh/nolze/msoffcrypto-tool)
+[![Documentation Status](https://readthedocs.org/projects/msoffcrypto-tool/badge/?version=latest)](http://msoffcrypto-tool.readthedocs.io/en/latest/?badge=latest)
 
-install_requires = \
-['cryptography>=35.0', 'olefile>=0.46']
-
-entry_points = \
-{'console_scripts': ['msoffcrypto-tool = msoffcrypto.__main__:main']}
-
-setup_kwargs = {
-    'name': 'msoffcrypto-tool',
-    'version': '5.0.1rc1',
-    'description': 'Python tool and library for decrypting MS Office files with passwords or other keys',
-    'long_description': '# msoffcrypto-tool\n\n[![PyPI](https://img.shields.io/pypi/v/msoffcrypto-tool.svg)](https://pypi.org/project/msoffcrypto-tool/)\n[![PyPI downloads](https://img.shields.io/pypi/dm/msoffcrypto-tool.svg)](https://pypistats.org/packages/msoffcrypto-tool)\n[![build](https://github.com/nolze/msoffcrypto-tool/actions/workflows/ci.yaml/badge.svg)](https://github.com/nolze/msoffcrypto-tool/actions/workflows/ci.yaml)\n[![Coverage Status](https://codecov.io/gh/nolze/msoffcrypto-tool/branch/master/graph/badge.svg)](https://codecov.io/gh/nolze/msoffcrypto-tool)\n[![Documentation Status](https://readthedocs.org/projects/msoffcrypto-tool/badge/?version=latest)](http://msoffcrypto-tool.readthedocs.io/en/latest/?badge=latest)\n\nmsoffcrypto-tool (formerly ms-offcrypto-tool) is Python tool and library for decrypting encrypted MS Office files with password, intermediate key, or private key which generated its escrow key.\n\n## Contents\n\n* [Install](#install)\n* [Examples](#examples)\n* [Supported encryption methods](#supported-encryption-methods)\n* [Tests](#tests)\n* [Todo](#todo)\n* [Resources](#resources)\n* [Use cases and mentions](#use-cases-and-mentions)\n* [Contributors](#contributors)\n\n## Install\n\n```\npip install msoffcrypto-tool\n```\n\n## Examples\n\n### As CLI tool (with password)\n\n```\nmsoffcrypto-tool encrypted.docx decrypted.docx -p Passw0rd\n```\n\nPassword is prompted if you omit the password argument value:\n\n```bash\n$ msoffcrypto-tool encrypted.docx decrypted.docx -p\nPassword:\n```\n\nTest if the file is encrypted or not (exit code 0 or 1 is returned):\n\n```\nmsoffcrypto-tool document.doc --test -v\n```\n\n### As library\n\nPassword and more key types are supported with library functions.\n\nBasic usage:\n\n```python\nimport msoffcrypto\n\nencrypted = open("encrypted.docx", "rb")\nfile = msoffcrypto.OfficeFile(encrypted)\n\nfile.load_key(password="Passw0rd")  # Use password\n\nwith open("decrypted.docx", "wb") as f:\n    file.decrypt(f)\n\nencrypted.close()\n```\n\nBasic usage (in-memory):\n\n```python\nimport msoffcrypto\nimport io\nimport pandas as pd\n\ndecrypted = io.BytesIO()\n\nwith open("encrypted.xlsx", "rb") as f:\n    file = msoffcrypto.OfficeFile(f)\n    file.load_key(password="Passw0rd")  # Use password\n    file.decrypt(decrypted)\n\ndf = pd.read_excel(decrypted)\nprint(df)\n```\n\nAdvanced usage:\n\n```python\n# Verify password before decryption (default: False)\n# The ECMA-376 Agile/Standard crypto system allows one to know whether the supplied password is correct before actually decrypting the file\n# Currently, the verify_password option is only meaningful for ECMA-376 Agile/Standard Encryption\nfile.load_key(password="Passw0rd", verify_password=True)\n\n# Use private key\nfile.load_key(private_key=open("priv.pem", "rb"))\n\n# Use intermediate key (secretKey)\nfile.load_key(secret_key=binascii.unhexlify("AE8C36E68B4BB9EA46E5544A5FDB6693875B2FDE1507CBC65C8BCF99E25C2562"))\n\n# Check the HMAC of the data payload before decryption (default: False)\n# Currently, the verify_integrity option is only meaningful for ECMA-376 Agile Encryption\nfile.decrypt(open("decrypted.docx", "wb"), verify_integrity=True)\n```\n\n## Supported encryption methods\n\n### MS-OFFCRYPTO specs\n\n* [x] ECMA-376 (Agile Encryption/Standard Encryption)\n  * [x] MS-DOCX (OOXML) (Word 2007-2016)\n  * [x] MS-XLSX (OOXML) (Excel 2007-2016)\n  * [x] MS-PPTX (OOXML) (PowerPoint 2007-2016)\n* [x] Office Binary Document RC4 CryptoAPI\n  * [x] MS-DOC (Word 2002, 2003, 2004)\n  * [x] MS-XLS (Excel 2002, 2003, 2004) (experimental)\n  * [x] MS-PPT (PowerPoint 2002, 2003, 2004) (partial, experimental)\n* [x] Office Binary Document RC4\n  * [x] MS-DOC (Word 97, 98, 2000)\n  * [x] MS-XLS (Excel 97, 98, 2000) (experimental)\n* [ ] ECMA-376 (Extensible Encryption)\n* [ ] XOR Obfuscation\n\n### Other\n\n* [ ] Word 95 Encryption (Word 95 and prior)\n* [ ] Excel 95 Encryption (Excel 95 and prior)\n* [ ] PowerPoint 95 Encryption (PowerPoint 95 and prior)\n\nPRs are welcome!\n\n## Tests\n\nWith [coverage](https://github.com/nedbat/coveragepy) and [pytest](https://pytest.org/):\n\n```\npoetry install\npoetry run coverage run -m pytest -v\n```\n\n## Todo\n\n* [x] Add tests\n* [x] Support decryption with passwords\n* [x] Support older encryption schemes\n* [x] Add function-level tests\n* [x] Add API documents\n* [x] Publish to PyPI\n* [x] Add decryption tests for various file formats\n* [x] Integrate with more comprehensive projects handling MS Office files (such as [oletools](https://github.com/decalage2/oletools/)?) if possible\n* [x] Add the password prompt mode for CLI\n* [x] Improve error types (v4.12.0)\n* [ ] Redesign APIs (v6.0.0)\n* [ ] Introduce something like `ctypes.Structure`\n* [ ] Support encryption\n* [ ] Isolate parser\n\n## Resources\n\n* "Backdooring MS Office documents with secret master keys" <http://secuinside.com/archive/2015/2015-1-9.pdf>\n* Technical Documents <https://msdn.microsoft.com/en-us/library/cc313105.aspx>\n  * [MS-OFFCRYPTO] Agile Encryption <https://msdn.microsoft.com/en-us/library/dd949735(v=office.12).aspx>\n* LibreOffice/core <https://github.com/LibreOffice/core>\n* LibreOffice/mso-dumper <https://github.com/LibreOffice/mso-dumper>\n* wvDecrypt <http://www.skynet.ie/~caolan/Packages/wvDecrypt.html>\n* Microsoft Office password protection - Wikipedia <https://en.wikipedia.org/wiki/Microsoft_Office_password_protection#History_of_Microsoft_Encryption_password>\n* office2john.py <https://github.com/magnumripper/JohnTheRipper/blob/bleeding-jumbo/run/office2john.py>\n\n## Alternatives\n\n* herumi/msoffice <https://github.com/herumi/msoffice>\n* DocRecrypt <https://blogs.technet.microsoft.com/office_resource_kit/2013/01/23/now-you-can-reset-or-remove-a-password-from-a-word-excel-or-powerpoint-filewith-office-2013/>\n* Apache POI - the Java API for Microsoft Documents <https://poi.apache.org/>\n\n## Use cases and mentions\n\n### General\n\n* <https://repology.org/project/python:msoffcrypto-tool/versions> (kudos to maintainers!)\n* <https://checkroth.com/unlocking-password-protected-files.html>\n\n### Malware/maldoc analysis\n\n* <https://github.com/jbremer/sflock/commit/3f6a96abe1dbb4405e4fb7fd0d16863f634b09fb>\n* <https://isc.sans.edu/forums/diary/Video+Analyzing+Encrypted+Malicious+Office+Documents/24572/>\n\n### CTF\n\n* <https://github.com/shombo/cyberstakes-writeps-2018/tree/master/word_up>\n* <https://github.com/willi123yao/Cyberthon2020_Writeups/blob/master/csit/Lost_Magic>\n\n### In other languages\n\n* <https://github.com/dtjohnson/xlsx-populate>\n* <https://github.com/opendocument-app/OpenDocument.core/blob/233663b039/src/internal/ooxml/ooxml_crypto.h>\n* <https://github.com/jaydadhania08/PHPDecryptXLSXWithPassword>\n\n### In publications\n\n* [Excel、データ整理＆分析、画像処理の自動化ワザを完全網羅！ 超速Python仕事術大全](https://books.google.co.jp/books?id=TBdVEAAAQBAJ&q=msoffcrypto) (伊沢剛, 2022)\n* ["Analyse de documents malveillants en 2021"](https://twitter.com/decalage2/status/1435255507846053889), MISC Hors-série N° 24, "Reverse engineering : apprenez à analyser des binaires" (Lagadec Philippe, 2021)\n* [シゴトがはかどる Python自動処理の教科書](https://books.google.co.jp/books?id=XEYUEAAAQBAJ&q=msoffcrypto) (クジラ飛行机, 2020)\n\n## Contributors\n\n* <https://github.com/nolze/msoffcrypto-tool/graphs/contributors>\n',
-    'author': 'nolze',
-    'author_email': 'nolze@archlinux.us',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nolze/msoffcrypto-tool',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+msoffcrypto-tool (formerly ms-offcrypto-tool) is Python tool and library for decrypting encrypted MS Office files with password, intermediate key, or private key which generated its escrow key.
 
+## Contents
+
+* [Install](#install)
+* [Examples](#examples)
+* [Supported encryption methods](#supported-encryption-methods)
+* [Tests](#tests)
+* [Todo](#todo)
+* [Resources](#resources)
+* [Use cases and mentions](#use-cases-and-mentions)
+* [Contributors](#contributors)
+
+## Install
+
+```
+pip install msoffcrypto-tool
+```
+
+## Examples
+
+### As CLI tool (with password)
+
+```
+msoffcrypto-tool encrypted.docx decrypted.docx -p Passw0rd
+```
+
+Password is prompted if you omit the password argument value:
+
+```bash
+$ msoffcrypto-tool encrypted.docx decrypted.docx -p
+Password:
+```
+
+Test if the file is encrypted or not (exit code 0 or 1 is returned):
+
+```
+msoffcrypto-tool document.doc --test -v
+```
+
+### As library
+
+Password and more key types are supported with library functions.
+
+Basic usage:
+
+```python
+import msoffcrypto
+
+encrypted = open("encrypted.docx", "rb")
+file = msoffcrypto.OfficeFile(encrypted)
+
+file.load_key(password="Passw0rd")  # Use password
+
+with open("decrypted.docx", "wb") as f:
+    file.decrypt(f)
+
+encrypted.close()
+```
+
+Basic usage (in-memory):
+
+```python
+import msoffcrypto
+import io
+import pandas as pd
+
+decrypted = io.BytesIO()
+
+with open("encrypted.xlsx", "rb") as f:
+    file = msoffcrypto.OfficeFile(f)
+    file.load_key(password="Passw0rd")  # Use password
+    file.decrypt(decrypted)
+
+df = pd.read_excel(decrypted)
+print(df)
+```
+
+Advanced usage:
+
+```python
+# Verify password before decryption (default: False)
+# The ECMA-376 Agile/Standard crypto system allows one to know whether the supplied password is correct before actually decrypting the file
+# Currently, the verify_password option is only meaningful for ECMA-376 Agile/Standard Encryption
+file.load_key(password="Passw0rd", verify_password=True)
+
+# Use private key
+file.load_key(private_key=open("priv.pem", "rb"))
+
+# Use intermediate key (secretKey)
+file.load_key(secret_key=binascii.unhexlify("AE8C36E68B4BB9EA46E5544A5FDB6693875B2FDE1507CBC65C8BCF99E25C2562"))
+
+# Check the HMAC of the data payload before decryption (default: False)
+# Currently, the verify_integrity option is only meaningful for ECMA-376 Agile Encryption
+file.decrypt(open("decrypted.docx", "wb"), verify_integrity=True)
+```
+
+## Supported encryption methods
+
+### MS-OFFCRYPTO specs
+
+* [x] ECMA-376 (Agile Encryption/Standard Encryption)
+  * [x] MS-DOCX (OOXML) (Word 2007-2016)
+  * [x] MS-XLSX (OOXML) (Excel 2007-2016)
+  * [x] MS-PPTX (OOXML) (PowerPoint 2007-2016)
+* [x] Office Binary Document RC4 CryptoAPI
+  * [x] MS-DOC (Word 2002, 2003, 2004)
+  * [x] MS-XLS (Excel 2002, 2003, 2004) (experimental)
+  * [x] MS-PPT (PowerPoint 2002, 2003, 2004) (partial, experimental)
+* [x] Office Binary Document RC4
+  * [x] MS-DOC (Word 97, 98, 2000)
+  * [x] MS-XLS (Excel 97, 98, 2000) (experimental)
+* [ ] ECMA-376 (Extensible Encryption)
+* [ ] XOR Obfuscation
+
+### Other
+
+* [ ] Word 95 Encryption (Word 95 and prior)
+* [ ] Excel 95 Encryption (Excel 95 and prior)
+* [ ] PowerPoint 95 Encryption (PowerPoint 95 and prior)
+
+PRs are welcome!
+
+## Tests
+
+With [coverage](https://github.com/nedbat/coveragepy) and [pytest](https://pytest.org/):
+
+```
+poetry install
+poetry run coverage run -m pytest -v
+```
+
+## Todo
+
+* [x] Add tests
+* [x] Support decryption with passwords
+* [x] Support older encryption schemes
+* [x] Add function-level tests
+* [x] Add API documents
+* [x] Publish to PyPI
+* [x] Add decryption tests for various file formats
+* [x] Integrate with more comprehensive projects handling MS Office files (such as [oletools](https://github.com/decalage2/oletools/)?) if possible
+* [x] Add the password prompt mode for CLI
+* [x] Improve error types (v4.12.0)
+* [ ] Redesign APIs (v6.0.0)
+* [ ] Introduce something like `ctypes.Structure`
+* [ ] Support encryption
+* [ ] Isolate parser
+
+## Resources
+
+* "Backdooring MS Office documents with secret master keys" <http://secuinside.com/archive/2015/2015-1-9.pdf>
+* Technical Documents <https://msdn.microsoft.com/en-us/library/cc313105.aspx>
+  * [MS-OFFCRYPTO] Agile Encryption <https://msdn.microsoft.com/en-us/library/dd949735(v=office.12).aspx>
+* [MS-OFFDI] Microsoft Office File Format Documentation Introduction <https://learn.microsoft.com/en-us/openspecs/office_file_formats/ms-offdi/24ed256c-eb5b-494e-b4f6-fb696ad2b4dc>
+* LibreOffice/core <https://github.com/LibreOffice/core>
+* LibreOffice/mso-dumper <https://github.com/LibreOffice/mso-dumper>
+* wvDecrypt <http://www.skynet.ie/~caolan/Packages/wvDecrypt.html>
+* Microsoft Office password protection - Wikipedia <https://en.wikipedia.org/wiki/Microsoft_Office_password_protection#History_of_Microsoft_Encryption_password>
+* office2john.py <https://github.com/magnumripper/JohnTheRipper/blob/bleeding-jumbo/run/office2john.py>
+
+## Alternatives
+
+* herumi/msoffice <https://github.com/herumi/msoffice>
+* DocRecrypt <https://blogs.technet.microsoft.com/office_resource_kit/2013/01/23/now-you-can-reset-or-remove-a-password-from-a-word-excel-or-powerpoint-filewith-office-2013/>
+* Apache POI - the Java API for Microsoft Documents <https://poi.apache.org/>
+
+## Use cases and mentions
+
+### General
+
+* <https://repology.org/project/python:msoffcrypto-tool/versions> (kudos to maintainers!)
+* <https://checkroth.com/unlocking-password-protected-files.html>
+
+### Malware/maldoc analysis
+
+* <https://github.com/jbremer/sflock/commit/3f6a96abe1dbb4405e4fb7fd0d16863f634b09fb>
+* <https://isc.sans.edu/forums/diary/Video+Analyzing+Encrypted+Malicious+Office+Documents/24572/>
+
+### CTF
+
+* <https://github.com/shombo/cyberstakes-writeps-2018/tree/master/word_up>
+* <https://github.com/willi123yao/Cyberthon2020_Writeups/blob/master/csit/Lost_Magic>
+
+### In other languages
+
+* <https://github.com/dtjohnson/xlsx-populate>
+* <https://github.com/opendocument-app/OpenDocument.core/blob/233663b039/src/internal/ooxml/ooxml_crypto.h>
+* <https://github.com/jaydadhania08/PHPDecryptXLSXWithPassword>
+
+### In publications
+
+* [Excel、データ整理＆分析、画像処理の自動化ワザを完全網羅！ 超速Python仕事術大全](https://books.google.co.jp/books?id=TBdVEAAAQBAJ&q=msoffcrypto) (伊沢剛, 2022)
+* ["Analyse de documents malveillants en 2021"](https://twitter.com/decalage2/status/1435255507846053889), MISC Hors-série N° 24, "Reverse engineering : apprenez à analyser des binaires" (Lagadec Philippe, 2021)
+* [シゴトがはかどる Python自動処理の教科書](https://books.google.co.jp/books?id=XEYUEAAAQBAJ&q=msoffcrypto) (クジラ飛行机, 2020)
+
+## Contributors
+
+* <https://github.com/nolze/msoffcrypto-tool/graphs/contributors>
 
-setup(**setup_kwargs)
```

