# Comparing `tmp/hypercli-1.0.0.tar.gz` & `tmp/hypercli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercli-1.0.0.tar", last modified: Mon Jul 17 21:48:23 2023, max compression
+gzip compressed data, was "hypercli-1.0.1.tar", last modified: Mon Jul 17 21:51:16 2023, max compression
```

## Comparing `hypercli-1.0.0.tar` & `hypercli-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 21:48:23.264620 hypercli-1.0.0/
--rw-rw-rw-   0        0        0     1084 2023-07-17 21:35:58.000000 hypercli-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3592 2023-07-17 21:48:23.264620 hypercli-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3296 2023-07-17 21:39:32.000000 hypercli-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 21:48:23.243507 hypercli-1.0.0/hypercli/
--rw-rw-rw-   0        0        0       28 2023-07-17 21:35:58.000000 hypercli-1.0.0/hypercli/__init__.py
--rw-rw-rw-   0        0        0    10350 2023-07-17 21:35:58.000000 hypercli-1.0.0/hypercli/core.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:48:23.262622 hypercli-1.0.0/hypercli.egg-info/
--rw-rw-rw-   0        0        0     3592 2023-07-17 21:48:23.000000 hypercli-1.0.0/hypercli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-17 21:48:23.000000 hypercli-1.0.0/hypercli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 21:48:23.000000 hypercli-1.0.0/hypercli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 21:44:00.000000 hypercli-1.0.0/hypercli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-07-17 21:48:23.000000 hypercli-1.0.0/hypercli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 21:48:23.000000 hypercli-1.0.0/hypercli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-07-17 21:35:58.000000 hypercli-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-07-17 21:48:23.268623 hypercli-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-07-17 21:35:58.000000 hypercli-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:51:16.663425 hypercli-1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-17 21:35:58.000000 hypercli-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3258 2023-07-17 21:51:16.664422 hypercli-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2962 2023-07-17 21:51:05.000000 hypercli-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 21:51:16.649790 hypercli-1.0.1/hypercli/
+-rw-rw-rw-   0        0        0       28 2023-07-17 21:35:58.000000 hypercli-1.0.1/hypercli/__init__.py
+-rw-rw-rw-   0        0        0    10350 2023-07-17 21:35:58.000000 hypercli-1.0.1/hypercli/core.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:51:16.662426 hypercli-1.0.1/hypercli.egg-info/
+-rw-rw-rw-   0        0        0     3258 2023-07-17 21:51:16.000000 hypercli-1.0.1/hypercli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-17 21:51:16.000000 hypercli-1.0.1/hypercli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:51:16.000000 hypercli-1.0.1/hypercli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 21:44:00.000000 hypercli-1.0.1/hypercli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-07-17 21:51:16.000000 hypercli-1.0.1/hypercli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 21:51:16.000000 hypercli-1.0.1/hypercli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-07-17 21:35:58.000000 hypercli-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-07-17 21:51:16.674819 hypercli-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      609 2023-07-17 21:51:10.000000 hypercli-1.0.1/setup.py
```

### Comparing `hypercli-1.0.0/LICENSE` & `hypercli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercli-1.0.0/PKG-INFO` & `hypercli-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,225 +1,186 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2068 7970  : 2.1..Name: hyp
-00000020: 6572 636c 690d 0a56 6572 7369 6f6e 3a20  ercli..Version: 
-00000030: 312e 302e 300d 0a53 756d 6d61 7279 3a20  1.0.0..Summary: 
-00000040: 4765 6e65 7261 7465 2065 6e68 616e 6365  Generate enhance
-00000050: 6420 6d65 6e75 2d64 7269 7665 6e20 434c  d menu-driven CL
-00000060: 4920 7072 6f67 7261 6d73 2077 6974 6820  I programs with 
-00000070: 6561 7365 210d 0a48 6f6d 652d 7061 6765  ease!..Home-page
-00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000090: 2e63 6f6d 2f48 5950 3352 3030 542f 6879  .com/HYP3R00T/hy
-000000a0: 7065 7263 6c69 0d0a 4175 7468 6f72 3a20  percli..Author: 
-000000b0: 4859 5033 5230 3054 0d0a 4175 7468 6f72  HYP3R00T..Author
-000000c0: 2d65 6d61 696c 3a20 6879 7065 726f 6f74  -email: hyperoot
-000000d0: 4070 6d2e 6d65 0d0a 4c69 6365 6e73 653a  @pm.me..License:
-000000e0: 204d 4954 0d0a 4465 7363 7269 7074 696f   MIT..Descriptio
-000000f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000100: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a4c  text/markdown..L
-00000110: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000120: 454e 5345 0d0a 0d0a 6060 600d 0a20 5f20  ENSE....```.. _ 
-00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000140: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
-00000150: 5f0d 0a7c 207c 2020 2020 2020 2020 2020  _..| |          
-00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000170: 2020 207c 2028 5f29 0d0a 7c20 7c5f 5f20     | (_)..| |__ 
-00000180: 205f 2020 205f 205f 205f 5f20 2020 5f5f   _   _ _ __   __
-00000190: 5f20 5f20 5f5f 205f 5f5f 7c20 7c5f 0d0a  _ _ __ ___| |_..
-000001a0: 7c20 275f 205c 7c20 7c20 7c20 7c20 275f  | '_ \| | | | '_
-000001b0: 205c 202f 205f 205c 2027 5f5f 2f20 5f5f   \ / _ \ '__/ __
-000001c0: 7c20 7c20 7c0d 0a7c 207c 207c 207c 207c  | | |..| | | | |
-000001d0: 5f7c 207c 207c 5f29 207c 2020 5f5f 2f20  _| | |_) |  __/ 
-000001e0: 7c20 7c20 285f 5f7c 207c 207c 0d0a 7c5f  | | (__| | |..|_
-000001f0: 7c20 7c5f 7c5c 5f5f 2c20 7c20 2e5f 5f2f  | |_|\__, | .__/
-00000200: 205c 5f5f 5f7c 5f7c 2020 5c5f 5f5f 7c5f   \___|_|  \___|_
-00000210: 7c5f 7c0d 0a20 2020 2020 2020 205f 5f2f  |_|..        __/
-00000220: 207c 207c 0d0a 2020 2020 2020 207c 5f5f   | |..       |__
-00000230: 5f2f 7c5f 7c20 2020 2020 2020 2020 2020  _/|_|           
-00000240: 2020 2020 7620 312e 302e 300d 0a60 6060      v 1.0.0..```
-00000250: 0d0a 0d0a 2320 6879 7065 7263 6c69 0d0a  ....# hypercli..
-00000260: 0d0a 2a2a 6879 7065 7263 6c69 2a2a 2069  ..**hypercli** i
-00000270: 7320 6120 5079 7468 6f6e 2070 6163 6b61  s a Python packa
-00000280: 6765 2074 6861 7420 7072 6f76 6964 6573  ge that provides
-00000290: 2061 6e20 656c 6567 616e 7420 736f 6c75   an elegant solu
-000002a0: 7469 6f6e 2066 6f72 2069 6e74 6572 6163  tion for interac
-000002b0: 7469 6e67 2077 6974 6820 636f 6d6d 616e  ting with comman
-000002c0: 6420 6c69 6e65 2074 6f6f 6c73 2e20 4974  d line tools. It
-000002d0: 206f 6666 6572 7320 6120 6d65 6e75 2d62   offers a menu-b
-000002e0: 6173 6564 2063 6f6d 6d61 6e64 206c 696e  ased command lin
-000002f0: 6520 696e 7465 7266 6163 6520 2843 4c49  e interface (CLI
-00000300: 2920 7468 6174 2061 6c6c 6f77 7320 7573  ) that allows us
-00000310: 6572 7320 746f 206e 6176 6967 6174 6520  ers to navigate 
-00000320: 7468 726f 7567 6820 6469 6666 6572 656e  through differen
-00000330: 7420 6f70 7469 6f6e 7320 616e 6420 6578  t options and ex
-00000340: 6563 7574 6520 6675 6e63 7469 6f6e 7320  ecute functions 
-00000350: 6261 7365 6420 6f6e 2074 6865 6972 2063  based on their c
-00000360: 686f 6963 6573 2e0d 0a0d 0a23 2320 4665  hoices.....## Fe
-00000370: 6174 7572 6573 0d0a 0d0a 2d20 4765 6e65  atures....- Gene
-00000380: 7261 7465 206d 656e 752d 6472 6976 656e  rate menu-driven
-00000390: 2043 4c49 2070 726f 6772 616d 7320 7769   CLI programs wi
-000003a0: 7468 2065 6173 6520 7573 696e 6720 6465  th ease using de
-000003b0: 636f 7261 746f 7273 0d0a 2d20 4375 7374  corators..- Cust
-000003c0: 6f6d 697a 6520 7468 6520 6d65 6e75 732c  omize the menus,
-000003d0: 206f 7074 696f 6e73 2c20 616e 6420 7669   options, and vi
-000003e0: 7375 616c 2073 7479 6c65 7320 6163 636f  sual styles acco
-000003f0: 7264 696e 6720 746f 2079 6f75 7220 7265  rding to your re
-00000400: 7175 6972 656d 656e 7473 0d0a 2d20 5375  quirements..- Su
-00000410: 7070 6f72 7473 206e 6573 7465 6420 6d65  pports nested me
-00000420: 6e75 7320 616e 6420 6e61 7669 6761 7469  nus and navigati
-00000430: 6f6e 2062 6574 7765 656e 206d 656e 7573  on between menus
-00000440: 0d0a 0d0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
-00000450: 696f 6e0d 0a0d 0a59 6f75 2063 616e 2069  ion....You can i
-00000460: 6e73 7461 6c6c 202a 2a68 7970 6572 636c  nstall **hypercl
-00000470: 692a 2a20 7573 696e 6720 7069 702e 204f  i** using pip. O
-00000480: 7065 6e20 796f 7572 2074 6572 6d69 6e61  pen your termina
-00000490: 6c20 616e 6420 7275 6e20 7468 6520 666f  l and run the fo
-000004a0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-000004b0: 0d0a 0d0a 6060 600d 0a70 6970 2069 6e73  ....```..pip ins
-000004c0: 7461 6c6c 2068 7970 6572 636c 690d 0a60  tall hypercli..`
-000004d0: 6060 0d0a 0d0a 2323 2055 7361 6765 0d0a  ``....## Usage..
-000004e0: 0d0a 546f 2075 7365 202a 2a68 7970 6572  ..To use **hyper
-000004f0: 636c 692a 2a2c 2069 6d70 6f72 7420 7468  cli**, import th
-00000500: 6520 6068 7970 6572 636c 6960 206d 6f64  e `hypercli` mod
-00000510: 756c 6520 6672 6f6d 2074 6865 2060 6879  ule from the `hy
-00000520: 7065 7263 6c69 6020 7061 636b 6167 6520  percli` package 
-00000530: 616e 6420 6372 6561 7465 2061 6e20 696e  and create an in
-00000540: 7374 616e 6365 206f 6620 7468 6520 6068  stance of the `h
-00000550: 7970 6572 636c 6960 2063 6c61 7373 2e20  ypercli` class. 
-00000560: 596f 7520 6361 6e20 7468 656e 2064 6566  You can then def
-00000570: 696e 6520 796f 7572 206d 656e 7573 2c20  ine your menus, 
-00000580: 6f70 7469 6f6e 732c 2061 6e64 2066 756e  options, and fun
-00000590: 6374 696f 6e73 2074 6f20 6265 2065 7865  ctions to be exe
-000005a0: 6375 7465 642e 2046 696e 616c 6c79 2c20  cuted. Finally, 
-000005b0: 6361 6c6c 2074 6865 2060 7275 6e28 2960  call the `run()`
-000005c0: 206d 6574 686f 6420 746f 2073 7461 7274   method to start
-000005d0: 2074 6865 2043 4c49 2069 6e74 6572 6661   the CLI interfa
-000005e0: 6365 2e0d 0a0d 0a48 6572 6527 7320 616e  ce.....Here's an
-000005f0: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
-00000600: 746f 2075 7365 202a 2a68 7970 6572 636c  to use **hypercl
-00000610: 692a 2a3a 0d0a 0d0a 6060 6070 7974 686f  i**:....```pytho
-00000620: 6e0d 0a23 2069 6d70 6f72 7420 6879 7065  n..# import hype
-00000630: 7263 6c69 0d0a 6672 6f6d 2068 7970 6572  rcli..from hyper
-00000640: 636c 6920 696d 706f 7274 2068 7970 6572  cli import hyper
-00000650: 636c 690d 0a0d 0a23 2063 7265 6174 6520  cli....# create 
-00000660: 616e 2069 6e73 7461 6e63 6520 6f66 2068  an instance of h
-00000670: 7970 6572 636c 690d 0a63 6c69 203d 2068  ypercli..cli = h
-00000680: 7970 6572 636c 6928 290d 0a0d 0a23 2063  ypercli()....# c
-00000690: 6f6e 6669 6775 7265 2074 6865 2069 6e73  onfigure the ins
-000006a0: 7461 6e63 650d 0a63 6c69 2e63 6f6e 6669  tance..cli.confi
-000006b0: 675b 2262 616e 6e65 725f 7465 7874 225d  g["banner_text"]
-000006c0: 203d 2022 4859 5045 5243 4c49 220d 0a63   = "HYPERCLI"..c
-000006d0: 6c69 2e63 6f6e 6669 675b 2269 6e74 726f  li.config["intro
-000006e0: 5f74 6974 6c65 225d 203d 2022 496e 7472  _title"] = "Intr
-000006f0: 6f22 0d0a 636c 692e 636f 6e66 6967 5b22  o"..cli.config["
-00000700: 696e 7472 6f5f 636f 6e74 656e 7422 5d20  intro_content"] 
-00000710: 3d20 2247 656e 6572 6174 6520 656e 6861  = "Generate enha
-00000720: 6e63 6564 206d 656e 752d 6472 6976 656e  nced menu-driven
-00000730: 2043 4c49 2070 726f 6772 616d 7320 7769   CLI programs wi
-00000740: 7468 2065 6173 6521 220d 0a63 6c69 2e63  th ease!"..cli.c
-00000750: 6f6e 6669 675b 2273 686f 775f 6d65 6e75  onfig["show_menu
-00000760: 5f74 6162 6c65 5f68 6561 6465 7222 5d20  _table_header"] 
-00000770: 3d20 5472 7565 0d0a 0d0a 2320 6164 6420  = True....# add 
-00000780: 6e61 7669 6761 7469 6f6e 206f 7074 696f  navigation optio
-00000790: 6e73 2074 6f20 7468 6520 6d65 6e75 0d0a  ns to the menu..
-000007a0: 636c 692e 6c69 6e6b 2822 4d61 696e 204d  cli.link("Main M
-000007b0: 656e 7522 2c20 224d 6174 6865 6d61 7469  enu", "Mathemati
-000007c0: 6373 204d 656e 7522 290d 0a63 6c69 2e6c  cs Menu")..cli.l
-000007d0: 696e 6b28 224d 6169 6e20 4d65 6e75 222c  ink("Main Menu",
-000007e0: 2022 5374 7269 6e67 204d 656e 7522 290d   "String Menu").
-000007f0: 0a0d 0a0d 0a40 636c 692e 656e 7472 7928  .....@cli.entry(
-00000800: 6d65 6e75 3d22 4d61 696e 204d 656e 7522  menu="Main Menu"
-00000810: 2c20 6f70 7469 6f6e 3d22 4772 6565 7465  , option="Greete
-00000820: 7222 290d 0a64 6566 2067 7265 6574 2829  r")..def greet()
-00000830: 3a0d 0a20 2020 206e 616d 6520 3d20 696e  :..    name = in
-00000840: 7075 7428 2245 6e74 6572 2079 6f75 7220  put("Enter your 
-00000850: 6e61 6d65 3a20 2229 0d0a 2020 2020 7072  name: ")..    pr
-00000860: 696e 7428 6622 4865 6c6c 6f2c 207b 6e61  int(f"Hello, {na
-00000870: 6d65 7d21 2229 0d0a 0d0a 0d0a 4063 6c69  me}!")......@cli
-00000880: 2e65 6e74 7279 286d 656e 753d 224d 6174  .entry(menu="Mat
-00000890: 6865 6d61 7469 6373 204d 656e 7522 2c20  hematics Menu", 
-000008a0: 6f70 7469 6f6e 3d22 4164 6420 7477 6f20  option="Add two 
-000008b0: 6e75 6d62 6572 7322 290d 0a64 6566 2061  numbers")..def a
-000008c0: 6464 286e 756d 313d 312c 206e 756d 323d  dd(num1=1, num2=
-000008d0: 3129 3a0d 0a20 2020 2061 203d 2069 6e74  1):..    a = int
-000008e0: 2869 6e70 7574 2866 2245 6e74 6572 2066  (input(f"Enter f
-000008f0: 6972 7374 206e 756d 6265 7220 2864 6566  irst number (def
-00000900: 6175 6c74 207b 6e75 6d31 7d29 3a20 2229  ault {num1}): ")
-00000910: 206f 7220 6e75 6d31 290d 0a20 2020 2062   or num1)..    b
-00000920: 203d 2069 6e74 2869 6e70 7574 2866 2245   = int(input(f"E
-00000930: 6e74 6572 2073 6563 6f6e 6420 6e75 6d62  nter second numb
-00000940: 6572 2028 6465 6661 756c 7420 7b6e 756d  er (default {num
-00000950: 327d 293a 2022 2920 6f72 206e 756d 3229  2}): ") or num2)
-00000960: 0d0a 2020 2020 7072 696e 7428 6622 7b61  ..    print(f"{a
-00000970: 7d20 2b20 7b62 7d20 3d20 7b61 202b 2062  } + {b} = {a + b
-00000980: 7d22 290d 0a0d 0a0d 0a40 636c 692e 656e  }")......@cli.en
-00000990: 7472 7928 6d65 6e75 3d22 4d61 7468 656d  try(menu="Mathem
-000009a0: 6174 6963 7320 4d65 6e75 222c 206f 7074  atics Menu", opt
-000009b0: 696f 6e3d 2253 7562 7472 6163 7420 7477  ion="Subtract tw
-000009c0: 6f20 6e75 6d62 6572 7322 290d 0a64 6566  o numbers")..def
-000009d0: 2073 7562 286e 756d 313d 312c 206e 756d   sub(num1=1, num
-000009e0: 323d 3129 3a0d 0a20 2020 2061 203d 2069  2=1):..    a = i
-000009f0: 6e74 2869 6e70 7574 2866 2245 6e74 6572  nt(input(f"Enter
-00000a00: 2066 6972 7374 206e 756d 6265 7220 2864   first number (d
-00000a10: 6566 6175 6c74 207b 6e75 6d31 7d29 3a20  efault {num1}): 
-00000a20: 2229 206f 7220 6e75 6d31 290d 0a20 2020  ") or num1)..   
-00000a30: 2062 203d 2069 6e74 2869 6e70 7574 2866   b = int(input(f
-00000a40: 2245 6e74 6572 2073 6563 6f6e 6420 6e75  "Enter second nu
-00000a50: 6d62 6572 2028 6465 6661 756c 7420 7b6e  mber (default {n
-00000a60: 756d 327d 293a 2022 2920 6f72 206e 756d  um2}): ") or num
-00000a70: 3229 0d0a 2020 2020 7072 696e 7428 6622  2)..    print(f"
-00000a80: 7b61 7d20 2d20 7b62 7d20 3d20 7b61 202d  {a} - {b} = {a -
-00000a90: 2062 7d22 290d 0a0d 0a0d 0a40 636c 692e   b}")......@cli.
-00000aa0: 656e 7472 7928 6d65 6e75 3d22 5374 7269  entry(menu="Stri
-00000ab0: 6e67 204d 656e 7522 2c20 6f70 7469 6f6e  ng Menu", option
-00000ac0: 3d22 5265 7665 7273 6520 6120 7374 7269  ="Reverse a stri
-00000ad0: 6e67 2229 0d0a 6465 6620 7265 7665 7273  ng")..def revers
-00000ae0: 6528 293a 0d0a 2020 2020 7374 7269 6e67  e():..    string
-00000af0: 203d 2069 6e70 7574 2822 456e 7465 7220   = input("Enter 
-00000b00: 6120 7374 7269 6e67 3a20 2229 0d0a 2020  a string: ")..  
-00000b10: 2020 7072 696e 7428 7374 7269 6e67 5b3a    print(string[:
-00000b20: 3a2d 315d 290d 0a0d 0a0d 0a40 636c 692e  :-1])......@cli.
-00000b30: 656e 7472 7928 6d65 6e75 3d22 5374 7269  entry(menu="Stri
-00000b40: 6e67 204d 656e 7522 2c20 6f70 7469 6f6e  ng Menu", option
-00000b50: 3d22 5368 6f77 206c 656e 6774 6820 6f66  ="Show length of
-00000b60: 2061 2073 7472 696e 6722 290d 0a64 6566   a string")..def
-00000b70: 2073 7472 5f6c 656e 6774 6828 293a 0d0a   str_length():..
-00000b80: 2020 2020 7374 7269 6e67 203d 2069 6e70      string = inp
-00000b90: 7574 2822 456e 7465 7220 6120 7374 7269  ut("Enter a stri
-00000ba0: 6e67 3a20 2229 0d0a 2020 2020 7072 696e  ng: ")..    prin
-00000bb0: 7428 6622 4c65 6e67 7468 206f 6620 7374  t(f"Length of st
-00000bc0: 7269 6e67 2069 7320 7b6c 656e 2873 7472  ring is {len(str
-00000bd0: 696e 6729 7d22 290d 0a0d 0a0d 0a23 2072  ing)}")......# r
-00000be0: 756e 2074 6865 2063 6c69 0d0a 636c 692e  un the cli..cli.
-00000bf0: 7275 6e28 290d 0a0d 0a60 6060 0d0a 0d0a  run()....```....
-00000c00: 215b 5d28 646f 6373 2f61 7373 6573 7473  ![](docs/assests
-00000c10: 2f65 7861 6d70 6c65 5f64 656d 6f2e 6769  /example_demo.gi
-00000c20: 6629 0d0a 0d0a 5468 6520 6162 6f76 6520  f)....The above 
-00000c30: 7363 7269 7074 2064 656d 6f6e 7374 7261  script demonstra
-00000c40: 7465 7320 7468 6520 7573 6167 6520 6f66  tes the usage of
-00000c50: 202a 2a68 7970 6572 636c 692a 2a2e 2049   **hypercli**. I
-00000c60: 7420 6372 6561 7465 7320 6120 434c 4920  t creates a CLI 
-00000c70: 7769 7468 2074 776f 206d 656e 7573 3a20  with two menus: 
-00000c80: 224d 6169 6e20 4d65 6e75 2220 616e 6420  "Main Menu" and 
-00000c90: 2253 7562 204d 656e 7522 2e20 4561 6368  "Sub Menu". Each
-00000ca0: 206d 656e 7520 6861 7320 6974 7320 6f77   menu has its ow
-00000cb0: 6e20 6f70 7469 6f6e 7320 616e 6420 6675  n options and fu
-00000cc0: 6e63 7469 6f6e 7320 746f 2062 6520 6578  nctions to be ex
-00000cd0: 6563 7574 6564 2e20 596f 7520 6361 6e20  ecuted. You can 
-00000ce0: 6375 7374 6f6d 697a 6520 7468 6520 6d65  customize the me
-00000cf0: 6e75 732c 206f 7074 696f 6e73 2c20 616e  nus, options, an
-00000d00: 6420 7669 7375 616c 2073 7479 6c65 7320  d visual styles 
-00000d10: 6163 636f 7264 696e 6720 746f 2079 6f75  according to you
-00000d20: 7220 7265 7175 6972 656d 656e 7473 2e20  r requirements. 
-00000d30: 546f 2063 6865 636b 206f 7574 206d 6f72  To check out mor
-00000d40: 6520 636f 6d70 6c65 7820 6578 616d 706c  e complex exampl
-00000d50: 652c 2072 6566 6572 2074 6f20 6045 7861  e, refer to `Exa
-00000d60: 6d70 6c65 5f72 6576 616d 7065 642e 7079  mple_revamped.py
-00000d70: 602e 0d0a 0d0a 2323 204c 6963 656e 7365  `.....## License
-00000d80: 0d0a 0d0a 5468 6973 2070 726f 6a65 6374  ....This project
-00000d90: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00000da0: 6572 2074 6865 204d 4954 204c 6963 656e  er the MIT Licen
-00000db0: 7365 2e20 5365 6520 7468 6520 5b4d 4954  se. See the [MIT
-00000dc0: 5d28 6874 7470 733a 2f2f 6368 6f6f 7365  ](https://choose
-00000dd0: 616c 6963 656e 7365 2e63 6f6d 2f6c 6963  alicense.com/lic
-00000de0: 656e 7365 732f 6d69 742f 2920 6669 6c65  enses/mit/) file
-00000df0: 2066 6f72 206d 6f72 6520 696e 666f 726d   for more inform
-00000e00: 6174 696f 6e2e 0d0a                      ation...
+00000000: 6060 600d 0a20 5f20 2020 2020 2020 2020  ```.. _         
+00000010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000020: 2020 2020 2020 5f20 5f0d 0a7c 207c 2020        _ _..| |  
+00000030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000040: 2020 2020 2020 2020 2020 207c 2028 5f29             | (_)
+00000050: 0d0a 7c20 7c5f 5f20 205f 2020 205f 205f  ..| |__  _   _ _
+00000060: 205f 5f20 2020 5f5f 5f20 5f20 5f5f 205f   __   ___ _ __ _
+00000070: 5f5f 7c20 7c5f 0d0a 7c20 275f 205c 7c20  __| |_..| '_ \| 
+00000080: 7c20 7c20 7c20 275f 205c 202f 205f 205c  | | | '_ \ / _ \
+00000090: 2027 5f5f 2f20 5f5f 7c20 7c20 7c0d 0a7c   '__/ __| | |..|
+000000a0: 207c 207c 207c 207c 5f7c 207c 207c 5f29   | | | |_| | |_)
+000000b0: 207c 2020 5f5f 2f20 7c20 7c20 285f 5f7c   |  __/ | | (__|
+000000c0: 207c 207c 0d0a 7c5f 7c20 7c5f 7c5c 5f5f   | |..|_| |_|\__
+000000d0: 2c20 7c20 2e5f 5f2f 205c 5f5f 5f7c 5f7c  , | .__/ \___|_|
+000000e0: 2020 5c5f 5f5f 7c5f 7c5f 7c0d 0a20 2020    \___|_|_|..   
+000000f0: 2020 2020 205f 5f2f 207c 207c 0d0a 2020       __/ | |..  
+00000100: 2020 2020 207c 5f5f 5f2f 7c5f 7c20 2020       |___/|_|   
+00000110: 2020 2020 2020 2020 2020 2020 7620 312e              v 1.
+00000120: 302e 310d 0a60 6060 0d0a 0d0a 2320 6879  0.1..```....# hy
+00000130: 7065 7263 6c69 0d0a 0d0a 2a2a 6879 7065  percli....**hype
+00000140: 7263 6c69 2a2a 2069 7320 6120 5079 7468  rcli** is a Pyth
+00000150: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
+00000160: 7072 6f76 6964 6573 2061 6e20 656c 6567  provides an eleg
+00000170: 616e 7420 736f 6c75 7469 6f6e 2066 6f72  ant solution for
+00000180: 2069 6e74 6572 6163 7469 6e67 2077 6974   interacting wit
+00000190: 6820 636f 6d6d 616e 6420 6c69 6e65 2074  h command line t
+000001a0: 6f6f 6c73 2e20 4974 206f 6666 6572 7320  ools. It offers 
+000001b0: 6120 6d65 6e75 2d62 6173 6564 2063 6f6d  a menu-based com
+000001c0: 6d61 6e64 206c 696e 6520 696e 7465 7266  mand line interf
+000001d0: 6163 6520 2843 4c49 2920 7468 6174 2061  ace (CLI) that a
+000001e0: 6c6c 6f77 7320 7573 6572 7320 746f 206e  llows users to n
+000001f0: 6176 6967 6174 6520 7468 726f 7567 6820  avigate through 
+00000200: 6469 6666 6572 656e 7420 6f70 7469 6f6e  different option
+00000210: 7320 616e 6420 6578 6563 7574 6520 6675  s and execute fu
+00000220: 6e63 7469 6f6e 7320 6261 7365 6420 6f6e  nctions based on
+00000230: 2074 6865 6972 2063 686f 6963 6573 2e0d   their choices..
+00000240: 0a0d 0a23 2320 4665 6174 7572 6573 0d0a  ...## Features..
+00000250: 0d0a 2d20 4765 6e65 7261 7465 206d 656e  ..- Generate men
+00000260: 752d 6472 6976 656e 2043 4c49 2070 726f  u-driven CLI pro
+00000270: 6772 616d 7320 7769 7468 2065 6173 6520  grams with ease 
+00000280: 7573 696e 6720 6465 636f 7261 746f 7273  using decorators
+00000290: 0d0a 2d20 4375 7374 6f6d 697a 6520 7468  ..- Customize th
+000002a0: 6520 6d65 6e75 732c 206f 7074 696f 6e73  e menus, options
+000002b0: 2c20 616e 6420 7669 7375 616c 2073 7479  , and visual sty
+000002c0: 6c65 7320 6163 636f 7264 696e 6720 746f  les according to
+000002d0: 2079 6f75 7220 7265 7175 6972 656d 656e   your requiremen
+000002e0: 7473 0d0a 2d20 5375 7070 6f72 7473 206e  ts..- Supports n
+000002f0: 6573 7465 6420 6d65 6e75 7320 616e 6420  ested menus and 
+00000300: 6e61 7669 6761 7469 6f6e 2062 6574 7765  navigation betwe
+00000310: 656e 206d 656e 7573 0d0a 0d0a 2323 2049  en menus....## I
+00000320: 6e73 7461 6c6c 6174 696f 6e0d 0a0d 0a59  nstallation....Y
+00000330: 6f75 2063 616e 2069 6e73 7461 6c6c 202a  ou can install *
+00000340: 2a68 7970 6572 636c 692a 2a20 7573 696e  *hypercli** usin
+00000350: 6720 7069 702e 204f 7065 6e20 796f 7572  g pip. Open your
+00000360: 2074 6572 6d69 6e61 6c20 616e 6420 7275   terminal and ru
+00000370: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00000380: 636f 6d6d 616e 643a 0d0a 0d0a 6060 600d  command:....```.
+00000390: 0a70 6970 2069 6e73 7461 6c6c 2068 7970  .pip install hyp
+000003a0: 6572 636c 690d 0a60 6060 0d0a 0d0a 2323  ercli..```....##
+000003b0: 2055 7361 6765 0d0a 0d0a 546f 2075 7365   Usage....To use
+000003c0: 202a 2a68 7970 6572 636c 692a 2a2c 2069   **hypercli**, i
+000003d0: 6d70 6f72 7420 7468 6520 6068 7970 6572  mport the `hyper
+000003e0: 636c 6960 206d 6f64 756c 6520 6672 6f6d  cli` module from
+000003f0: 2074 6865 2060 6879 7065 7263 6c69 6020   the `hypercli` 
+00000400: 7061 636b 6167 6520 616e 6420 6372 6561  package and crea
+00000410: 7465 2061 6e20 696e 7374 616e 6365 206f  te an instance o
+00000420: 6620 7468 6520 6068 7970 6572 636c 6960  f the `hypercli`
+00000430: 2063 6c61 7373 2e20 596f 7520 6361 6e20   class. You can 
+00000440: 7468 656e 2064 6566 696e 6520 796f 7572  then define your
+00000450: 206d 656e 7573 2c20 6f70 7469 6f6e 732c   menus, options,
+00000460: 2061 6e64 2066 756e 6374 696f 6e73 2074   and functions t
+00000470: 6f20 6265 2065 7865 6375 7465 642e 2046  o be executed. F
+00000480: 696e 616c 6c79 2c20 6361 6c6c 2074 6865  inally, call the
+00000490: 2060 7275 6e28 2960 206d 6574 686f 6420   `run()` method 
+000004a0: 746f 2073 7461 7274 2074 6865 2043 4c49  to start the CLI
+000004b0: 2069 6e74 6572 6661 6365 2e0d 0a0d 0a48   interface.....H
+000004c0: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
+000004d0: 206f 6620 686f 7720 746f 2075 7365 202a   of how to use *
+000004e0: 2a68 7970 6572 636c 692a 2a3a 0d0a 0d0a  *hypercli**:....
+000004f0: 6060 6070 7974 686f 6e0d 0a23 2069 6d70  ```python..# imp
+00000500: 6f72 7420 6879 7065 7263 6c69 0d0a 6672  ort hypercli..fr
+00000510: 6f6d 2068 7970 6572 636c 6920 696d 706f  om hypercli impo
+00000520: 7274 2068 7970 6572 636c 690d 0a0d 0a23  rt hypercli....#
+00000530: 2063 7265 6174 6520 616e 2069 6e73 7461   create an insta
+00000540: 6e63 6520 6f66 2068 7970 6572 636c 690d  nce of hypercli.
+00000550: 0a63 6c69 203d 2068 7970 6572 636c 6928  .cli = hypercli(
+00000560: 290d 0a0d 0a23 2063 6f6e 6669 6775 7265  )....# configure
+00000570: 2074 6865 2069 6e73 7461 6e63 650d 0a63   the instance..c
+00000580: 6c69 2e63 6f6e 6669 675b 2262 616e 6e65  li.config["banne
+00000590: 725f 7465 7874 225d 203d 2022 4859 5045  r_text"] = "HYPE
+000005a0: 5243 4c49 220d 0a63 6c69 2e63 6f6e 6669  RCLI"..cli.confi
+000005b0: 675b 2269 6e74 726f 5f74 6974 6c65 225d  g["intro_title"]
+000005c0: 203d 2022 496e 7472 6f22 0d0a 636c 692e   = "Intro"..cli.
+000005d0: 636f 6e66 6967 5b22 696e 7472 6f5f 636f  config["intro_co
+000005e0: 6e74 656e 7422 5d20 3d20 2247 656e 6572  ntent"] = "Gener
+000005f0: 6174 6520 656e 6861 6e63 6564 206d 656e  ate enhanced men
+00000600: 752d 6472 6976 656e 2043 4c49 2070 726f  u-driven CLI pro
+00000610: 6772 616d 7320 7769 7468 2065 6173 6521  grams with ease!
+00000620: 220d 0a63 6c69 2e63 6f6e 6669 675b 2273  "..cli.config["s
+00000630: 686f 775f 6d65 6e75 5f74 6162 6c65 5f68  how_menu_table_h
+00000640: 6561 6465 7222 5d20 3d20 5472 7565 0d0a  eader"] = True..
+00000650: 0d0a 2320 6164 6420 6e61 7669 6761 7469  ..# add navigati
+00000660: 6f6e 206f 7074 696f 6e73 2074 6f20 7468  on options to th
+00000670: 6520 6d65 6e75 0d0a 636c 692e 6c69 6e6b  e menu..cli.link
+00000680: 2822 4d61 696e 204d 656e 7522 2c20 224d  ("Main Menu", "M
+00000690: 6174 6865 6d61 7469 6373 204d 656e 7522  athematics Menu"
+000006a0: 290d 0a63 6c69 2e6c 696e 6b28 224d 6169  )..cli.link("Mai
+000006b0: 6e20 4d65 6e75 222c 2022 5374 7269 6e67  n Menu", "String
+000006c0: 204d 656e 7522 290d 0a0d 0a0d 0a40 636c   Menu")......@cl
+000006d0: 692e 656e 7472 7928 6d65 6e75 3d22 4d61  i.entry(menu="Ma
+000006e0: 696e 204d 656e 7522 2c20 6f70 7469 6f6e  in Menu", option
+000006f0: 3d22 4772 6565 7465 7222 290d 0a64 6566  ="Greeter")..def
+00000700: 2067 7265 6574 2829 3a0d 0a20 2020 206e   greet():..    n
+00000710: 616d 6520 3d20 696e 7075 7428 2245 6e74  ame = input("Ent
+00000720: 6572 2079 6f75 7220 6e61 6d65 3a20 2229  er your name: ")
+00000730: 0d0a 2020 2020 7072 696e 7428 6622 4865  ..    print(f"He
+00000740: 6c6c 6f2c 207b 6e61 6d65 7d21 2229 0d0a  llo, {name}!")..
+00000750: 0d0a 0d0a 4063 6c69 2e65 6e74 7279 286d  ....@cli.entry(m
+00000760: 656e 753d 224d 6174 6865 6d61 7469 6373  enu="Mathematics
+00000770: 204d 656e 7522 2c20 6f70 7469 6f6e 3d22   Menu", option="
+00000780: 4164 6420 7477 6f20 6e75 6d62 6572 7322  Add two numbers"
+00000790: 290d 0a64 6566 2061 6464 286e 756d 313d  )..def add(num1=
+000007a0: 312c 206e 756d 323d 3129 3a0d 0a20 2020  1, num2=1):..   
+000007b0: 2061 203d 2069 6e74 2869 6e70 7574 2866   a = int(input(f
+000007c0: 2245 6e74 6572 2066 6972 7374 206e 756d  "Enter first num
+000007d0: 6265 7220 2864 6566 6175 6c74 207b 6e75  ber (default {nu
+000007e0: 6d31 7d29 3a20 2229 206f 7220 6e75 6d31  m1}): ") or num1
+000007f0: 290d 0a20 2020 2062 203d 2069 6e74 2869  )..    b = int(i
+00000800: 6e70 7574 2866 2245 6e74 6572 2073 6563  nput(f"Enter sec
+00000810: 6f6e 6420 6e75 6d62 6572 2028 6465 6661  ond number (defa
+00000820: 756c 7420 7b6e 756d 327d 293a 2022 2920  ult {num2}): ") 
+00000830: 6f72 206e 756d 3229 0d0a 2020 2020 7072  or num2)..    pr
+00000840: 696e 7428 6622 7b61 7d20 2b20 7b62 7d20  int(f"{a} + {b} 
+00000850: 3d20 7b61 202b 2062 7d22 290d 0a0d 0a0d  = {a + b}").....
+00000860: 0a40 636c 692e 656e 7472 7928 6d65 6e75  .@cli.entry(menu
+00000870: 3d22 4d61 7468 656d 6174 6963 7320 4d65  ="Mathematics Me
+00000880: 6e75 222c 206f 7074 696f 6e3d 2253 7562  nu", option="Sub
+00000890: 7472 6163 7420 7477 6f20 6e75 6d62 6572  tract two number
+000008a0: 7322 290d 0a64 6566 2073 7562 286e 756d  s")..def sub(num
+000008b0: 313d 312c 206e 756d 323d 3129 3a0d 0a20  1=1, num2=1):.. 
+000008c0: 2020 2061 203d 2069 6e74 2869 6e70 7574     a = int(input
+000008d0: 2866 2245 6e74 6572 2066 6972 7374 206e  (f"Enter first n
+000008e0: 756d 6265 7220 2864 6566 6175 6c74 207b  umber (default {
+000008f0: 6e75 6d31 7d29 3a20 2229 206f 7220 6e75  num1}): ") or nu
+00000900: 6d31 290d 0a20 2020 2062 203d 2069 6e74  m1)..    b = int
+00000910: 2869 6e70 7574 2866 2245 6e74 6572 2073  (input(f"Enter s
+00000920: 6563 6f6e 6420 6e75 6d62 6572 2028 6465  econd number (de
+00000930: 6661 756c 7420 7b6e 756d 327d 293a 2022  fault {num2}): "
+00000940: 2920 6f72 206e 756d 3229 0d0a 2020 2020  ) or num2)..    
+00000950: 7072 696e 7428 6622 7b61 7d20 2d20 7b62  print(f"{a} - {b
+00000960: 7d20 3d20 7b61 202d 2062 7d22 290d 0a0d  } = {a - b}")...
+00000970: 0a0d 0a40 636c 692e 656e 7472 7928 6d65  ...@cli.entry(me
+00000980: 6e75 3d22 5374 7269 6e67 204d 656e 7522  nu="String Menu"
+00000990: 2c20 6f70 7469 6f6e 3d22 5265 7665 7273  , option="Revers
+000009a0: 6520 6120 7374 7269 6e67 2229 0d0a 6465  e a string")..de
+000009b0: 6620 7265 7665 7273 6528 293a 0d0a 2020  f reverse():..  
+000009c0: 2020 7374 7269 6e67 203d 2069 6e70 7574    string = input
+000009d0: 2822 456e 7465 7220 6120 7374 7269 6e67  ("Enter a string
+000009e0: 3a20 2229 0d0a 2020 2020 7072 696e 7428  : ")..    print(
+000009f0: 7374 7269 6e67 5b3a 3a2d 315d 290d 0a0d  string[::-1])...
+00000a00: 0a0d 0a40 636c 692e 656e 7472 7928 6d65  ...@cli.entry(me
+00000a10: 6e75 3d22 5374 7269 6e67 204d 656e 7522  nu="String Menu"
+00000a20: 2c20 6f70 7469 6f6e 3d22 5368 6f77 206c  , option="Show l
+00000a30: 656e 6774 6820 6f66 2061 2073 7472 696e  ength of a strin
+00000a40: 6722 290d 0a64 6566 2073 7472 5f6c 656e  g")..def str_len
+00000a50: 6774 6828 293a 0d0a 2020 2020 7374 7269  gth():..    stri
+00000a60: 6e67 203d 2069 6e70 7574 2822 456e 7465  ng = input("Ente
+00000a70: 7220 6120 7374 7269 6e67 3a20 2229 0d0a  r a string: ")..
+00000a80: 2020 2020 7072 696e 7428 6622 4c65 6e67      print(f"Leng
+00000a90: 7468 206f 6620 7374 7269 6e67 2069 7320  th of string is 
+00000aa0: 7b6c 656e 2873 7472 696e 6729 7d22 290d  {len(string)}").
+00000ab0: 0a0d 0a0d 0a23 2072 756e 2074 6865 2063  .....# run the c
+00000ac0: 6c69 0d0a 636c 692e 7275 6e28 290d 0a0d  li..cli.run()...
+00000ad0: 0a60 6060 0d0a 0d0a 215b 5d28 646f 6373  .```....![](docs
+00000ae0: 2f61 7373 6573 7473 2f65 7861 6d70 6c65  /assests/example
+00000af0: 5f64 656d 6f2e 6769 6629 0d0a 0d0a 0d0a  _demo.gif)......
+00000b00: 2323 204c 6963 656e 7365 0d0a 0d0a 5468  ## License....Th
+00000b10: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+00000b20: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00000b30: 204d 4954 204c 6963 656e 7365 2e20 5365   MIT License. Se
+00000b40: 6520 7468 6520 5b4d 4954 5d28 6874 7470  e the [MIT](http
+00000b50: 733a 2f2f 6368 6f6f 7365 616c 6963 656e  s://choosealicen
+00000b60: 7365 2e63 6f6d 2f6c 6963 656e 7365 732f  se.com/licenses/
+00000b70: 6d69 742f 2920 6669 6c65 2066 6f72 206d  mit/) file for m
+00000b80: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
+00000b90: 0d0a                                     ..
```

### Comparing `hypercli-1.0.0/hypercli/core.py` & `hypercli-1.0.1/hypercli/core.py`

 * *Files identical despite different names*

### Comparing `hypercli-1.0.0/hypercli.egg-info/PKG-INFO` & `hypercli-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypercli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate enhanced menu-driven CLI programs with ease!
 Home-page: https://github.com/HYP3R00T/hypercli
 Author: HYP3R00T
 Author-email: hyperoot@pm.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
  _                               _ _
 | |                             | (_)
 | |__  _   _ _ __   ___ _ __ ___| |_
 | '_ \| | | | '_ \ / _ \ '__/ __| | |
 | | | | |_| | |_) |  __/ | | (__| | |
 |_| |_|\__, | .__/ \___|_|  \___|_|_|
         __/ | |
-       |___/|_|               v 1.0.0
+       |___/|_|               v 1.0.1
 ```
 
 # hypercli
 
 **hypercli** is a Python package that provides an elegant solution for interacting with command line tools. It offers a menu-based command line interface (CLI) that allows users to navigate through different options and execute functions based on their choices.
 
 ## Features
@@ -97,12 +97,11 @@
 # run the cli
 cli.run()
 
 ```
 
 ![](docs/assests/example_demo.gif)
 
-The above script demonstrates the usage of **hypercli**. It creates a CLI with two menus: "Main Menu" and "Sub Menu". Each menu has its own options and functions to be executed. You can customize the menus, options, and visual styles according to your requirements. To check out more complex example, refer to `Example_revamped.py`.
 
 ## License
 
 This project is licensed under the MIT License. See the [MIT](https://choosealicense.com/licenses/mit/) file for more information.
```

### Comparing `hypercli-1.0.0/setup.py` & `hypercli-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("./README.md", "r") as readme:
     desc = readme.read()
 
 setuptools.setup(
     name="hypercli",
-    version="1.0.0",
+    version="1.0.1",
     author="HYP3R00T",
     author_email="hyperoot@pm.me",
     description="Generate enhanced menu-driven CLI programs with ease!",
     url="https://github.com/HYP3R00T/hypercli",
     long_description=desc,
     long_description_content_type="text/markdown",
     license="MIT",
```

