# Comparing `tmp/st_login-0.0.0.tar.gz` & `tmp/st_login-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_login-0.0.0.tar", last modified: Mon Jul 17 07:12:40 2023, max compression
+gzip compressed data, was "st_login-0.0.1.tar", last modified: Mon Jul 17 07:18:37 2023, max compression
```

## Comparing `st_login-0.0.0.tar` & `st_login-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:12:40.350763 st_login-0.0.0/
--rw-rw-rw-   0        0        0     1087 2023-07-17 06:41:41.000000 st_login-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     6320 2023-07-17 07:12:40.350763 st_login-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5694 2023-07-17 07:11:08.000000 st_login-0.0.0/README.md
--rw-rw-rw-   0        0        0      921 2023-07-17 07:12:40.356762 st_login-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       79 2023-07-17 06:39:35.000000 st_login-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:12:40.312761 st_login-0.0.0/st_login/
--rw-rw-rw-   0        0        0       36 2023-07-17 07:06:31.000000 st_login-0.0.0/st_login/__init__.py
--rw-rw-rw-   0        0        0     6963 2023-07-17 06:41:41.000000 st_login-0.0.0/st_login/utils.py
--rw-rw-rw-   0        0        0    13979 2023-07-17 07:06:23.000000 st_login-0.0.0/st_login/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:12:40.343761 st_login-0.0.0/st_login.egg-info/
--rw-rw-rw-   0        0        0     6320 2023-07-17 07:12:40.000000 st_login-0.0.0/st_login.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-17 07:12:40.000000 st_login-0.0.0/st_login.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:12:40.000000 st_login-0.0.0/st_login.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-17 07:12:40.000000 st_login-0.0.0/st_login.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-17 07:12:40.000000 st_login-0.0.0/st_login.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 07:06:52.000000 st_login-0.0.0/st_login.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-17 07:12:40.346761 st_login-0.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:41:41.000000 st_login-0.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.580529 st_login-0.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-07-17 06:41:41.000000 st_login-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6211 2023-07-17 07:18:37.580529 st_login-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5600 2023-07-17 07:15:36.000000 st_login-0.0.1/README.md
+-rw-rw-rw-   0        0        0      906 2023-07-17 07:18:37.583530 st_login-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       79 2023-07-17 06:39:35.000000 st_login-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.536546 st_login-0.0.1/st_login/
+-rw-rw-rw-   0        0        0       36 2023-07-17 07:06:31.000000 st_login-0.0.1/st_login/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-07-17 06:41:41.000000 st_login-0.0.1/st_login/utils.py
+-rw-rw-rw-   0        0        0    13979 2023-07-17 07:06:23.000000 st_login-0.0.1/st_login/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.572533 st_login-0.0.1/st_login.egg-info/
+-rw-rw-rw-   0        0        0     6211 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.576617 st_login-0.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:41:41.000000 st_login-0.0.1/tests/__init__.py
```

### Comparing `st_login-0.0.0/LICENSE` & `st_login-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_login-0.0.0/PKG-INFO` & `st_login-0.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: st_login
-Version: 0.0.0
-Summary: The streamlit_login_auth_ui library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
+Version: 0.0.1
+Summary: The st_login library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
 Home-page: https://github.com/lijiacaigit/st_login
 Author: Lijiacai
 Author-email: 1050518702@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 The library grants users an option to reset their password, users can click on ```Forgot Password?``` after which an Email is triggered containing a temporary, randomly generated password.
 
 The library also sets encrypted cookies to remember and automatically authenticate the users without password. \
 The users can logout using the ```Logout``` button.
 
 
 ## Authors
-- [@gauriprabhakar](https://github.com/GauriSP10)
+- [@lijiacai](https://github.com/lijiacaigit/)
 
 ## PyPi
 https://pypi.org/project/streamlit-login-auth-ui/
 
 ## The UI:
 ![login_streamlit](https://user-images.githubusercontent.com/75731631/185765909-a70dd7af-240d-4a90-9140-45d6292e76f0.png)
  
@@ -140,16 +140,14 @@
 ![logout_streamlit](https://user-images.githubusercontent.com/75731631/185765879-dbe17dda-93e3-4417-b5fc-5ce1d4dc8ecc.png)
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
 v0.0.0
 
-## License
-[MIT](https://github.com/GauriSP10/streamlit_login_auth_ui/blob/main/LICENSE)
```

### Comparing `st_login-0.0.0/README.md` & `st_login-0.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 The library grants users an option to reset their password, users can click on ```Forgot Password?``` after which an Email is triggered containing a temporary, randomly generated password.
 
 The library also sets encrypted cookies to remember and automatically authenticate the users without password. \
 The users can logout using the ```Logout``` button.
 
 
 ## Authors
-- [@gauriprabhakar](https://github.com/GauriSP10)
+- [@lijiacai](https://github.com/lijiacaigit/)
 
 ## PyPi
 https://pypi.org/project/streamlit-login-auth-ui/
 
 ## The UI:
 ![login_streamlit](https://user-images.githubusercontent.com/75731631/185765909-a70dd7af-240d-4a90-9140-45d6292e76f0.png)
  
@@ -124,15 +124,13 @@
 ![logout_streamlit](https://user-images.githubusercontent.com/75731631/185765879-dbe17dda-93e3-4417-b5fc-5ce1d4dc8ecc.png)
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
 v0.0.0
 
-## License
-[MIT](https://github.com/GauriSP10/streamlit_login_auth_ui/blob/main/LICENSE)
```

### Comparing `st_login-0.0.0/setup.cfg` & `st_login-0.0.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 745f 6c6f 6769 6e0d 0a76 6572   = st_login..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e30 0d0a 6465  sion = 0.0.0..de
+00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6465  sion = 0.0.1..de
 00000030: 7363 7269 7074 696f 6e20 3d20 5468 6520  scription = The 
-00000040: 7374 7265 616d 6c69 745f 6c6f 6769 6e5f  streamlit_login_
-00000050: 6175 7468 5f75 6920 6c69 6272 6172 7920  auth_ui library 
-00000060: 6973 206d 6561 6e74 2066 6f72 2073 7472  is meant for str
-00000070: 6561 6d6c 6974 2061 7070 6c69 6361 7469  eamlit applicati
-00000080: 6f6e 2064 6576 656c 6f70 6572 732e 2049  on developers. I
-00000090: 7420 6c65 7473 2079 6f75 2063 6f6e 6e65  t lets you conne
-000000a0: 6374 2079 6f75 7220 7374 7265 616d 6c69  ct your streamli
-000000b0: 7420 6170 706c 6963 6174 696f 6e20 746f  t application to
-000000c0: 2061 2070 7265 2d62 7569 6c74 2061 6e64   a pre-built and
-000000d0: 2073 6563 7572 6520 4c6f 6769 6e2f 2053   secure Login/ S
-000000e0: 6967 6e2d 5570 2070 6167 650d 0a6c 6f6e  ign-Up page..lon
-000000f0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000100: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000110: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000120: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000130: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000140: 6175 7468 6f72 203d 204c 696a 6961 6361  author = Lijiaca
-00000150: 690d 0a61 7574 686f 725f 656d 6169 6c20  i..author_email 
-00000160: 3d20 3130 3530 3531 3837 3032 4071 712e  = 1050518702@qq.
-00000170: 636f 6d0d 0a75 726c 203d 2068 7474 7073  com..url = https
-00000180: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c69  ://github.com/li
-00000190: 6a69 6163 6169 6769 742f 7374 5f6c 6f67  jiacaigit/st_log
-000001a0: 696e 0d0a 6c69 6365 6e73 655f 6669 6c65  in..license_file
-000001b0: 7320 3d20 4c49 4345 4e53 450d 0a63 6c61  s = LICENSE..cla
-000001c0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001f0: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000200: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000210: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000220: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000230: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000240: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000250: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000260: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000270: 3d20 3e3d 332e 372e 310d 0a7a 6970 5f73  = >=3.7.1..zip_s
-00000280: 6166 6520 3d20 5472 7565 0d0a 696e 636c  afe = True..incl
-00000290: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000002a0: 203d 2054 7275 650d 0a69 6e73 7461 6c6c   = True..install
-000002b0: 5f72 6571 7569 7265 7320 3d20 0d0a 0961  _requires = ...a
-000002c0: 7267 6f6e 322d 6366 6669 0d0a 0961 7267  rgon2-cffi...arg
-000002d0: 6f6e 322d 6366 6669 2d62 696e 6469 6e67  on2-cffi-binding
-000002e0: 730d 0a09 7374 7265 616d 6c69 740d 0a09  s...streamlit...
-000002f0: 7374 7265 616d 6c69 742d 636f 6f6b 6965  streamlit-cookie
-00000300: 732d 6d61 6e61 6765 720d 0a09 7374 7265  s-manager...stre
-00000310: 616d 6c69 742d 6c6f 7474 6965 0d0a 0973  amlit-lottie...s
-00000320: 7472 6561 6d6c 6974 2d6f 7074 696f 6e2d  treamlit-option-
-00000330: 6d65 6e75 0d0a 0d0a 5b6f 7074 696f 6e73  menu....[options
-00000340: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000350: 0a65 7863 6c75 6465 203d 200d 0a09 7465  .exclude = ...te
-00000360: 7374 0d0a 0974 6573 742e 2a0d 0a0d 0a5b  st...test.*....[
-00000370: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000380: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000390: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000040: 7374 5f6c 6f67 696e 206c 6962 7261 7279  st_login library
+00000050: 2069 7320 6d65 616e 7420 666f 7220 7374   is meant for st
+00000060: 7265 616d 6c69 7420 6170 706c 6963 6174  reamlit applicat
+00000070: 696f 6e20 6465 7665 6c6f 7065 7273 2e20  ion developers. 
+00000080: 4974 206c 6574 7320 796f 7520 636f 6e6e  It lets you conn
+00000090: 6563 7420 796f 7572 2073 7472 6561 6d6c  ect your streaml
+000000a0: 6974 2061 7070 6c69 6361 7469 6f6e 2074  it application t
+000000b0: 6f20 6120 7072 652d 6275 696c 7420 616e  o a pre-built an
+000000c0: 6420 7365 6375 7265 204c 6f67 696e 2f20  d secure Login/ 
+000000d0: 5369 676e 2d55 7020 7061 6765 0d0a 6c6f  Sign-Up page..lo
+000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000f0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+00000100: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000110: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000120: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+00000130: 0a61 7574 686f 7220 3d20 4c69 6a69 6163  .author = Lijiac
+00000140: 6169 0d0a 6175 7468 6f72 5f65 6d61 696c  ai..author_email
+00000150: 203d 2031 3035 3035 3138 3730 3240 7171   = 1050518702@qq
+00000160: 2e63 6f6d 0d0a 7572 6c20 3d20 6874 7470  .com..url = http
+00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+00000180: 696a 6961 6361 6967 6974 2f73 745f 6c6f  ijiacaigit/st_lo
+00000190: 6769 6e0d 0a6c 6963 656e 7365 5f66 696c  gin..license_fil
+000001a0: 6573 203d 204c 4943 454e 5345 0d0a 636c  es = LICENSE..cl
+000001b0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001e0: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+000001f0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000200: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000210: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000220: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000230: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000240: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000250: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000260: 203d 203e 3d33 2e37 2e31 0d0a 7a69 705f   = >=3.7.1..zip_
+00000270: 7361 6665 203d 2054 7275 650d 0a69 6e63  safe = True..inc
+00000280: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000290: 6120 3d20 5472 7565 0d0a 696e 7374 616c  a = True..instal
+000002a0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+000002b0: 6172 676f 6e32 2d63 6666 690d 0a09 6172  argon2-cffi...ar
+000002c0: 676f 6e32 2d63 6666 692d 6269 6e64 696e  gon2-cffi-bindin
+000002d0: 6773 0d0a 0973 7472 6561 6d6c 6974 0d0a  gs...streamlit..
+000002e0: 0973 7472 6561 6d6c 6974 2d63 6f6f 6b69  .streamlit-cooki
+000002f0: 6573 2d6d 616e 6167 6572 0d0a 0973 7472  es-manager...str
+00000300: 6561 6d6c 6974 2d6c 6f74 7469 650d 0a09  eamlit-lottie...
+00000310: 7374 7265 616d 6c69 742d 6f70 7469 6f6e  streamlit-option
+00000320: 2d6d 656e 750d 0a0d 0a5b 6f70 7469 6f6e  -menu....[option
+00000330: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000340: 0d0a 6578 636c 7564 6520 3d20 0d0a 0974  ..exclude = ...t
+00000350: 6573 740d 0a09 7465 7374 2e2a 0d0a 0d0a  est...test.*....
+00000360: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000370: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000380: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `st_login-0.0.0/st_login/utils.py` & `st_login-0.0.1/st_login/utils.py`

 * *Files identical despite different names*

### Comparing `st_login-0.0.0/st_login/widgets.py` & `st_login-0.0.1/st_login/widgets.py`

 * *Files identical despite different names*

### Comparing `st_login-0.0.0/st_login.egg-info/PKG-INFO` & `st_login-0.0.1/st_login.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: st-login
-Version: 0.0.0
-Summary: The streamlit_login_auth_ui library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
+Version: 0.0.1
+Summary: The st_login library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
 Home-page: https://github.com/lijiacaigit/st_login
 Author: Lijiacai
 Author-email: 1050518702@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 The library grants users an option to reset their password, users can click on ```Forgot Password?``` after which an Email is triggered containing a temporary, randomly generated password.
 
 The library also sets encrypted cookies to remember and automatically authenticate the users without password. \
 The users can logout using the ```Logout``` button.
 
 
 ## Authors
-- [@gauriprabhakar](https://github.com/GauriSP10)
+- [@lijiacai](https://github.com/lijiacaigit/)
 
 ## PyPi
 https://pypi.org/project/streamlit-login-auth-ui/
 
 ## The UI:
 ![login_streamlit](https://user-images.githubusercontent.com/75731631/185765909-a70dd7af-240d-4a90-9140-45d6292e76f0.png)
  
@@ -140,16 +140,14 @@
 ![logout_streamlit](https://user-images.githubusercontent.com/75731631/185765879-dbe17dda-93e3-4417-b5fc-5ce1d4dc8ecc.png)
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
 v0.0.0
 
-## License
-[MIT](https://github.com/GauriSP10/streamlit_login_auth_ui/blob/main/LICENSE)
```

