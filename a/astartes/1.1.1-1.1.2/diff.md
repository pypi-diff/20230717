# Comparing `tmp/astartes-1.1.1.tar.gz` & `tmp/astartes-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astartes-1.1.1.tar", last modified: Sun Jul  2 10:12:36 2023, max compression
+gzip compressed data, was "astartes-1.1.2.tar", last modified: Mon Jul 17 14:15:07 2023, max compression
```

## Comparing `astartes-1.1.1.tar` & `astartes-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 10:12:27.000000 astartes-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-07-02 10:12:36.902914 astartes-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-07-02 10:12:27.000000 astartes-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.898914 astartes-1.1.1/astartes/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/molecules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/astartes/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/abstract_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/astartes/samplers/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/dbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/optisim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/sphere_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/extrapolation/time_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/astartes/samplers/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/interpolation/kennardstone.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/interpolation/mtsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/interpolation/random_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/samplers/interpolation/spxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/astartes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/array_type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-02 10:12:27.000000 astartes-1.1.1/astartes/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:12:36.902914 astartes-1.1.1/astartes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-07-02 10:12:36.000000 astartes-1.1.1/astartes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-02 10:12:36.000000 astartes-1.1.1/astartes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:12:36.000000 astartes-1.1.1/astartes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 10:12:36.000000 astartes-1.1.1/astartes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 10:12:36.000000 astartes-1.1.1/astartes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-02 10:12:27.000000 astartes-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:12:36.902914 astartes-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 14:14:58.000000 astartes-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-07-17 14:15:07.915574 astartes-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-17 14:14:58.000000 astartes-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.911574 astartes-1.1.2/astartes/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/astartes/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/abstract_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/astartes/samplers/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/optisim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/sphere_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/extrapolation/time_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/astartes/samplers/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/interpolation/kennardstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/interpolation/mtsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/interpolation/random_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/samplers/interpolation/spxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/astartes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/array_type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 14:14:58.000000 astartes-1.1.2/astartes/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:15:07.915574 astartes-1.1.2/astartes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-07-17 14:15:07.000000 astartes-1.1.2/astartes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-17 14:15:07.000000 astartes-1.1.2/astartes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:15:07.000000 astartes-1.1.2/astartes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 14:15:07.000000 astartes-1.1.2/astartes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 14:15:07.000000 astartes-1.1.2/astartes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-17 14:14:59.000000 astartes-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:15:07.915574 astartes-1.1.2/setup.cfg
```

### Comparing `astartes-1.1.1/LICENSE` & `astartes-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/PKG-INFO` & `astartes-1.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6173 7461  : 2.1.Name: asta
 00000020: 7274 6573 0a56 6572 7369 6f6e 3a20 312e  rtes.Version: 1.
-00000030: 312e 310a 5375 6d6d 6172 793a 2054 7261  1.1.Summary: Tra
+00000030: 312e 320a 5375 6d6d 6172 793a 2054 7261  1.2.Summary: Tra
 00000040: 696e 3a54 6573 7420 416c 676f 7269 7468  in:Test Algorith
 00000050: 6d69 6320 5361 6d70 6c69 6e67 2066 6f72  mic Sampling for
 00000060: 204d 6f6c 6563 756c 6573 2061 6e64 2041   Molecules and A
 00000070: 7262 6974 7261 7279 2041 7272 6179 730a  rbitrary Arrays.
 00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 4a61  Author-email: Ja
 00000090: 636b 736f 6e20 4275 726e 7320 3c6a 7762  ckson Burns <jwb
 000000a0: 7572 6e73 406d 6974 2e65 6475 3e2c 2048  urns@mit.edu>, H
@@ -112,1179 +112,1123 @@
 000006f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000700: 4a61 636b 736f 6e42 7572 6e73 2f61 7374  JacksonBurns/ast
 00000710: 6172 7465 732f 6163 7469 6f6e 732f 776f  artes/actions/wo
 00000720: 726b 666c 6f77 732f 7265 7072 6f64 7563  rkflows/reproduc
 00000730: 655f 7061 7065 722e 796d 6c2f 6261 6467  e_paper.yml/badg
 00000740: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
 00000750: 6e26 6576 656e 743d 7363 6865 6475 6c65  n&event=schedule
-00000760: 223e 0a3c 2f70 3e0a 0a23 2320 496e 7374  ">.</p>..## Inst
-00000770: 616c 6c69 6e67 2060 6173 7461 7274 6573  alling `astartes
-00000780: 600a 5765 2072 6563 6f6d 6d65 6e64 2069  `.We recommend i
-00000790: 6e73 7461 6c6c 696e 6720 6061 7374 6172  nstalling `astar
-000007a0: 7465 7360 2077 6974 6869 6e20 6120 7669  tes` within a vi
-000007b0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-000007c0: 742c 2075 7369 6e67 2065 6974 6865 7220  t, using either 
-000007d0: 6076 656e 7660 206f 7220 6063 6f6e 6461  `venv` or `conda
-000007e0: 6020 286f 7220 6f74 6865 7220 746f 6f6c  ` (or other tool
-000007f0: 7329 2074 6f20 7369 6d70 6c69 6679 2064  s) to simplify d
-00000800: 6570 656e 6465 6e63 7920 6d61 6e61 6765  ependency manage
-00000810: 6d65 6e74 2e20 5079 7468 6f6e 2076 6572  ment. Python ver
-00000820: 7369 6f6e 7320 332e 372c 2033 2e38 2c20  sions 3.7, 3.8, 
-00000830: 332e 392c 2033 2e31 302c 2061 6e64 2033  3.9, 3.10, and 3
-00000840: 2e31 3120 6172 6520 7375 7070 6f72 7465  .11 are supporte
-00000850: 6420 6f6e 2061 6c6c 2070 6c61 7466 6f72  d on all platfor
-00000860: 6d73 2e0a 0a60 6173 7461 7274 6573 6020  ms...`astartes` 
-00000870: 6973 2061 7661 696c 6162 6c65 206f 6e20  is available on 
-00000880: 6050 7950 4960 2061 6e64 2063 616e 2062  `PyPI` and can b
-00000890: 6520 696e 7374 616c 6c65 6420 7573 696e  e installed usin
-000008a0: 6720 6070 6970 603a 0a0a 202d 2054 6f20  g `pip`:.. - To 
-000008b0: 696e 636c 7564 6520 7468 6520 6665 6174  include the feat
-000008c0: 7572 697a 6174 696f 6e20 6f70 7469 6f6e  urization option
-000008d0: 7320 666f 7220 6368 656d 6963 616c 2064  s for chemical d
-000008e0: 6174 612c 2075 7365 2060 7069 7020 696e  ata, use `pip in
-000008f0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
-00000900: 6f6c 6563 756c 6573 5d60 2e0a 202d 2054  olecules]`.. - T
-00000910: 6f20 696e 7374 616c 6c20 6f6e 6c79 2074  o install only t
-00000920: 6865 2073 616d 706c 696e 6720 616c 676f  he sampling algo
-00000930: 7269 7468 6d73 2c20 7573 6520 6070 6970  rithms, use `pip
-00000940: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
-00000950: 7360 2028 7468 6973 2069 6e73 7461 6c6c  s` (this install
-00000960: 2077 696c 6c20 6861 7665 2066 6577 6572   will have fewer
-00000970: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
-00000980: 6420 6d61 7920 6265 206d 6f72 6520 7265  d may be more re
-00000990: 6164 696c 7920 636f 6d70 6174 6962 6c65  adily compatible
-000009a0: 2069 6e20 656e 7669 726f 6e6d 656e 7473   in environments
-000009b0: 2077 6974 6820 6578 6973 7469 6e67 2077   with existing w
-000009c0: 6f72 6b66 6c6f 7773 292e 0a0a 5468 6520  orkflows)...The 
-000009d0: 6261 7365 2060 6173 7461 7274 6573 6020  base `astartes` 
-000009e0: 7061 636b 6167 6520 6973 2061 6c73 6f20  package is also 
-000009f0: 6176 6169 6c61 626c 6520 6f6e 2060 636f  available on `co
-00000a00: 6e64 6160 2077 6974 6820 7468 6973 2063  nda` with this c
-00000a10: 6f6d 6d61 6e64 3a20 6063 6f6e 6461 2069  ommand: `conda i
-00000a20: 6e73 7461 6c6c 202d 6320 6a61 636b 736f  nstall -c jackso
-00000a30: 6e62 7572 6e73 2061 7374 6172 7465 7360  nburns astartes`
-00000a40: 2e0a 4e6f 7465 2074 6861 7420 7468 6973  ..Note that this
-00000a50: 2070 6163 6b61 6765 205f 646f 6573 206e   package _does n
-00000a60: 6f74 5f20 696e 636c 7564 6520 6275 696c  ot_ include buil
-00000a70: 742d 696e 2073 7570 706f 7274 2066 6f72  t-in support for
-00000a80: 2066 6561 7475 7269 7a69 6e67 206d 6f6c   featurizing mol
-00000a90: 6563 756c 6573 2c20 7768 6963 6820 6973  ecules, which is
-00000aa0: 2063 7572 7265 6e74 6c79 206f 6e6c 7920   currently only 
-00000ab0: 6176 6169 6c61 626c 6520 6672 6f6d 2074  available from t
-00000ac0: 6865 2050 7950 4920 7061 636b 6167 6520  he PyPI package 
-00000ad0: 6f72 2061 2073 6f75 7263 6520 696e 7374  or a source inst
-00000ae0: 616c 6c2e 0a0a 3e20 2a2a 4e6f 7465 2a2a  all...> **Note**
-00000af0: 0a3e 2057 696e 646f 7773 2050 6f77 6572  .> Windows Power
-00000b00: 7368 656c 6c20 616e 6420 4d61 634f 5320  shell and MacOS 
-00000b10: 4361 7461 6c69 6e61 206f 7220 6e65 7765  Catalina or newe
-00000b20: 7220 6d61 7920 636f 6d70 6c61 696e 2061  r may complain a
-00000b30: 626f 7574 2073 7175 6172 6520 6272 6163  bout square brac
-00000b40: 6b65 7473 2c20 736f 2079 6f75 2077 696c  kets, so you wil
-00000b50: 6c20 6e65 6564 2074 6f20 646f 7562 6c65  l need to double
-00000b60: 2071 756f 7465 2074 6865 2060 6d6f 6c65   quote the `mole
-00000b70: 6375 6c65 7360 2063 6f6d 6d61 6e64 2028  cules` command (
-00000b80: 692e 652e 2060 7069 7020 696e 7374 616c  i.e. `pip instal
-00000b90: 6c20 2261 7374 6172 7465 735b 6d6f 6c65  l "astartes[mole
-00000ba0: 6375 6c65 735d 2260 290a 0a54 6f20 696e  cules]"`)..To in
-00000bb0: 7374 616c 6c20 6061 7374 6172 7465 7360  stall `astartes`
-00000bc0: 2066 726f 6d20 736f 7572 6365 2c20 7365   from source, se
-00000bd0: 6520 7468 6520 5b43 6f6e 7472 6962 7574  e the [Contribut
-00000be0: 696e 6720 2620 4465 7665 6c6f 7065 7220  ing & Developer 
-00000bf0: 4e6f 7465 735d 2823 636f 6e74 7269 6275  Notes](#contribu
-00000c00: 7469 6e67 2d2d 6465 7665 6c6f 7065 722d  ting--developer-
-00000c10: 6e6f 7465 7329 2073 6563 7469 6f6e 2e0a  notes) section..
-00000c20: 0a23 2320 5573 696e 6720 6061 7374 6172  .## Using `astar
-00000c30: 7465 7360 0a60 6173 7461 7274 6573 6020  tes`.`astartes` 
-00000c40: 6973 2064 6573 6967 6e65 6420 6173 2061  is designed as a
-00000c50: 2064 726f 702d 696e 2072 6570 6c61 6365   drop-in replace
-00000c60: 6d65 6e74 2066 6f72 2060 736b 6c65 6172  ment for `sklear
-00000c70: 6e60 2773 2060 7472 6169 6e5f 7465 7374  n`'s `train_test
-00000c80: 5f73 706c 6974 6020 6675 6e63 7469 6f6e  _split` function
-00000c90: 2e20 546f 2073 7769 7463 6820 746f 2060  . To switch to `
-00000ca0: 6173 7461 7274 6573 602c 2063 6861 6e67  astartes`, chang
-00000cb0: 6520 6066 726f 6d20 736b 6c65 6172 6e2e  e `from sklearn.
-00000cc0: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
-00000cd0: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
-00000ce0: 745f 7370 6c69 7460 2074 6f20 6066 726f  t_split` to `fro
-00000cf0: 6d20 6173 7461 7274 6573 2069 6d70 6f72  m astartes impor
-00000d00: 7420 7472 6169 6e5f 7465 7374 5f73 706c  t train_test_spl
-00000d10: 6974 602e 0a0a 4c69 6b65 2060 736b 6c65  it`...Like `skle
-00000d20: 6172 6e60 2c20 6061 7374 6172 7465 7360  arn`, `astartes`
-00000d30: 2061 6363 6570 7473 2061 6e79 2069 7465   accepts any ite
-00000d40: 7261 626c 6520 6f62 6a65 6374 2061 7320  rable object as 
-00000d50: 6058 602c 2060 7960 2c20 616e 6420 606c  `X`, `y`, and `l
-00000d60: 6162 656c 7360 2e0a 4561 6368 2077 696c  abels`..Each wil
-00000d70: 6c20 6265 2063 6f6e 7665 7274 6564 2074  l be converted t
-00000d80: 6f20 6120 606e 756d 7079 6020 6172 7261  o a `numpy` arra
-00000d90: 7920 666f 7220 696e 7465 726e 616c 206f  y for internal o
-00000da0: 7065 7261 7469 6f6e 732c 2061 6e64 2072  perations, and r
-00000db0: 6574 7572 6e65 6420 6173 2061 2060 6e75  eturned as a `nu
-00000dc0: 6d70 7960 2061 7272 6179 2077 6974 6820  mpy` array with 
-00000dd0: 6c69 6d69 7465 6420 6578 6365 7074 696f  limited exceptio
-00000de0: 6e73 3a20 6966 2060 5860 2069 7320 6120  ns: if `X` is a 
-00000df0: 6070 616e 6461 7360 2060 4461 7461 4672  `pandas` `DataFr
-00000e00: 616d 6560 2c20 6079 6020 6973 2061 2060  ame`, `y` is a `
-00000e10: 5365 7269 6573 602c 206f 7220 606c 6162  Series`, or `lab
-00000e20: 656c 7360 2069 7320 6120 6053 6572 6965  els` is a `Serie
-00000e30: 7360 2c20 6061 7374 6172 7465 7360 2077  s`, `astartes` w
-00000e40: 696c 6c20 6361 7374 2069 7420 6261 636b  ill cast it back
-00000e50: 2074 6f20 6974 7320 6f72 6967 696e 616c   to its original
-00000e60: 2074 7970 6520 696e 636c 7564 696e 6720   type including 
-00000e70: 6974 7320 696e 6465 7820 616e 6420 636f  its index and co
-00000e80: 6c75 6d6e 206e 616d 6573 2e0a 0a3e 202a  lumn names...> *
-00000e90: 2a4e 6f74 652a 2a0a 3e20 5468 6520 6465  *Note**.> The de
-00000ea0: 7665 6c6f 7065 7273 2072 6563 6f6d 6d65  velopers recomme
-00000eb0: 6e64 2070 6173 7369 6e67 2060 5860 2c20  nd passing `X`, 
-00000ec0: 6079 602c 2061 6e64 2060 6c61 6265 6c73  `y`, and `labels
-00000ed0: 6020 6173 2060 6e75 6d70 7960 2061 7272  ` as `numpy` arr
-00000ee0: 6179 7320 616e 6420 6861 6e64 6c69 6e67  ays and handling
-00000ef0: 2074 6865 2063 6f6e 7665 7273 696f 6e20   the conversion 
-00000f00: 746f 2061 6e64 2066 726f 6d20 6f74 6865  to and from othe
-00000f10: 7220 7479 7065 7320 6578 706c 6963 6974  r types explicit
-00000f20: 7920 6f6e 2079 6f75 7220 6f77 6e2e 2042  y on your own. B
-00000f30: 6568 696e 642d 7468 652d 7363 656e 6573  ehind-the-scenes
-00000f40: 2074 7970 6520 6361 7374 696e 6720 6361   type casting ca
-00000f50: 6e20 6c65 6164 2074 6f20 756e 6578 7065  n lead to unexpe
-00000f60: 6374 6564 2062 6568 6176 696f 7221 0a0a  cted behavior!..
-00000f70: 4279 2064 6566 6175 6c74 2c20 6061 7374  By default, `ast
-00000f80: 6172 7465 7360 2077 696c 6c20 7370 6c69  artes` will spli
-00000f90: 7420 6461 7461 2072 616e 646f 6d6c 792e  t data randomly.
-00000fa0: 2041 6464 6974 696f 6e61 6c6c 792c 2061   Additionally, a
-00000fb0: 2076 6172 6965 7479 206f 6620 616c 676f   variety of algo
-00000fc0: 7269 7468 6d69 6320 7361 6d70 6c69 6e67  rithmic sampling
-00000fd0: 2061 7070 726f 6163 6865 7320 6361 6e20   approaches can 
-00000fe0: 6265 2075 7365 6420 6279 2073 7065 6369  be used by speci
-00000ff0: 6679 696e 6720 7468 6520 6073 616d 706c  fying the `sampl
-00001000: 6572 6020 6172 6775 6d65 6e74 2074 6f20  er` argument to 
-00001010: 7468 6520 6675 6e63 7469 6f6e 3a0a 0a60  the function:..`
-00001020: 6060 7079 7468 6f6e 0a58 5f74 7261 696e  ``python.X_train
-00001030: 2c20 585f 7465 7374 2c20 795f 7472 6169  , X_test, y_trai
-00001040: 6e2c 2079 5f74 6573 7420 3d20 7472 6169  n, y_test = trai
-00001050: 6e5f 7465 7374 5f73 706c 6974 280a 2020  n_test_split(.  
-00001060: 582c 2020 2320 7072 6566 6572 6162 6c79  X,  # preferably
-00001070: 206e 756d 7079 2061 7272 6179 732c 2062   numpy arrays, b
-00001080: 7574 2061 7374 6172 7465 7320 7769 6c6c  ut astartes will
-00001090: 2063 6173 7420 6974 2066 6f72 2079 6f75   cast it for you
-000010a0: 0a20 2079 2c0a 2020 7361 6d70 6c65 7220  .  y,.  sampler 
-000010b0: 3d20 276b 656e 6e61 7264 5f73 746f 6e65  = 'kennard_stone
-000010c0: 272c 2020 2320 616e 7920 6f66 2074 6865  ',  # any of the
-000010d0: 2073 7570 706f 7274 6564 2073 616d 706c   supported sampl
-000010e0: 6572 730a 290a 6060 600a 0a23 2323 2050  ers.).```..### P
-000010f0: 6170 6572 0a46 6f72 2061 2063 6f6d 7072  aper.For a compr
-00001100: 6568 656e 7369 7665 2077 616c 6b74 6872  ehensive walkthr
-00001110: 6f75 6768 206f 6620 7468 6520 7468 656f  ough of the theo
-00001120: 7279 2061 6e64 2069 6d70 6c65 6d65 6e74  ry and implement
-00001130: 6174 696f 6e20 6f66 2060 6173 7461 7274  ation of `astart
-00001140: 6573 602c 2066 6f6c 6c6f 7720 5b74 6869  es`, follow [thi
-00001150: 7320 6c69 6e6b 5d28 6874 7470 733a 2f2f  s link](https://
-00001160: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
-00001170: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
-00001180: 2f72 6177 2f6a 6f73 732d 7061 7065 722f  /raw/joss-paper/
-00001190: 4275 726e 732d 5370 6965 6b65 726d 616e  Burns-Spiekerman
-000011a0: 6e2d 4268 6174 7461 6368 6172 6a65 655f  n-Bhattacharjee_
-000011b0: 6173 7461 7274 6573 2e70 6466 2920 746f  astartes.pdf) to
-000011c0: 2072 6561 6420 7468 6520 636f 6d70 616e   read the compan
-000011d0: 696f 6e20 7061 7065 722e 0a0a 2323 2320  ion paper...### 
-000011e0: 4578 616d 706c 6520 4e6f 7465 626f 6f6b  Example Notebook
-000011f0: 730a 0a43 6c69 636b 2074 6865 2062 6164  s..Click the bad
-00001200: 6765 7320 696e 2074 6865 2074 6162 6c65  ges in the table
-00001210: 2062 656c 6f77 2074 6f20 6265 2074 616b   below to be tak
-00001220: 656e 2074 6f20 6120 6c69 7665 2c20 696e  en to a live, in
-00001230: 7465 7261 6374 6976 6520 6465 6d6f 206f  teractive demo o
-00001240: 6620 6061 7374 6172 7465 7360 3a0a 0a7c  f `astartes`:..|
-00001250: 2044 656d 6f20 7c20 4c69 6e6b 207c 0a7c   Demo | Link |.|
-00001260: 3a2d 2d2d 3a7c 2d2d 2d7c 0a7c 2055 7369  :---:|---|.| Usi
-00001270: 6e67 2060 7472 6169 6e5f 7661 6c5f 7465  ng `train_val_te
-00001280: 7374 5f73 706c 6974 6020 7769 7468 2074  st_split` with t
-00001290: 6865 2060 736b 6c65 6172 6e60 2065 7861  he `sklearn` exa
-000012a0: 6d70 6c65 2064 6174 6173 6574 7320 7c20  mple datasets | 
-000012b0: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
-000012c0: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-000012d0: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
-000012e0: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
-000012f0: 722e 6f72 672f 7632 2f67 682f 4a61 636b  r.org/v2/gh/Jack
-00001300: 736f 6e42 7572 6e73 2f61 7374 6172 7465  sonBurns/astarte
-00001310: 732f 6d61 696e 3f6c 6162 7061 7468 3d65  s/main?labpath=e
-00001320: 7861 6d70 6c65 7325 3246 7472 6169 6e5f  xamples%2Ftrain_
-00001330: 7661 6c5f 7465 7374 5f73 706c 6974 5f73  val_test_split_s
-00001340: 6b6c 6561 726e 5f65 7861 6d70 6c65 2532  klearn_example%2
-00001350: 4674 7261 696e 5f76 616c 5f74 6573 745f  Ftrain_val_test_
-00001360: 7370 6c69 745f 6578 616d 706c 652e 6970  split_example.ip
-00001370: 796e 6229 207c 0a7c 2043 6f6d 7061 7269  ynb) |.| Compari
-00001380: 6e67 2053 616d 706c 696e 6720 416c 676f  ng Sampling Algo
-00001390: 7269 7468 6d73 2077 6974 6820 4661 7374  rithms with Fast
-000013a0: 2046 6f6f 6420 7c20 5b21 5b42 696e 6465   Food | [![Binde
-000013b0: 725d 2868 7474 7073 3a2f 2f6d 7962 696e  r](https://mybin
-000013c0: 6465 722e 6f72 672f 6261 6467 655f 6c6f  der.org/badge_lo
-000013d0: 676f 2e73 7667 295d 2868 7474 7073 3a2f  go.svg)](https:/
-000013e0: 2f6d 7962 696e 6465 722e 6f72 672f 7632  /mybinder.org/v2
-000013f0: 2f67 682f 4a61 636b 736f 6e42 7572 6e73  /gh/JacksonBurns
-00001400: 2f61 7374 6172 7465 732f 6d61 696e 3f6c  /astartes/main?l
-00001410: 6162 7061 7468 3d65 7861 6d70 6c65 7325  abpath=examples%
-00001420: 3246 7370 6c69 745f 636f 6d70 6172 6973  2Fsplit_comparis
-00001430: 6f6e 7325 3246 7370 6c69 745f 636f 6d70  ons%2Fsplit_comp
-00001440: 6172 6973 6f6e 732e 6970 796e 6229 207c  arisons.ipynb) |
-00001450: 0a7c 2043 6865 6d69 6e66 6f72 6d61 7469  .| Cheminformati
-00001460: 6373 2073 616d 706c 6520 7365 7420 7061  cs sample set pa
-00001470: 7274 6974 696f 6e69 6e67 2077 6974 6820  rtitioning with 
-00001480: 6061 7374 6172 7465 7360 207c 205b 215b  `astartes` | [![
-00001490: 4269 6e64 6572 5d28 6874 7470 733a 2f2f  Binder](https://
-000014a0: 6d79 6269 6e64 6572 2e6f 7267 2f62 6164  mybinder.org/bad
-000014b0: 6765 5f6c 6f67 6f2e 7376 6729 5d28 6874  ge_logo.svg)](ht
-000014c0: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
-000014d0: 7267 2f76 322f 6768 2f4a 6163 6b73 6f6e  rg/v2/gh/Jackson
-000014e0: 4275 726e 732f 6173 7461 7274 6573 2f6d  Burns/astartes/m
-000014f0: 6169 6e3f 6c61 6270 6174 683d 6578 616d  ain?labpath=exam
-00001500: 706c 6573 2532 4662 6172 7269 6572 5f70  ples%2Fbarrier_p
-00001510: 7265 6469 6374 696f 6e5f 7769 7468 5f52  rediction_with_R
-00001520: 4442 3725 3246 5244 4237 5f62 6172 7269  DB7%2FRDB7_barri
-00001530: 6572 5f70 7265 6469 6374 696f 6e5f 6578  er_prediction_ex
-00001540: 616d 706c 652e 6970 796e 6229 207c 0a7c  ample.ipynb) |.|
-00001550: 2043 6f6d 7061 7269 6e67 2070 6172 7469   Comparing parti
-00001560: 7469 6f6e 696e 6720 6170 7072 6f61 6368  tioning approach
-00001570: 6573 2066 6f72 2061 6c6b 616e 6573 207c  es for alkanes |
-00001580: 205b 215b 4269 6e64 6572 5d28 6874 7470   [![Binder](http
-00001590: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
-000015a0: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
-000015b0: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
-000015c0: 6572 2e6f 7267 2f76 322f 6768 2f4a 6163  er.org/v2/gh/Jac
-000015d0: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
-000015e0: 6573 2f6d 6169 6e3f 6c61 6270 6174 683d  es/main?labpath=
-000015f0: 6578 616d 706c 6573 2532 466d 6c70 6473  examples%2Fmlpds
-00001600: 5f32 3032 335f 6173 7461 7274 6573 5f64  _2023_astartes_d
-00001610: 656d 6f25 3246 6d6c 7064 735f 3230 3233  emo%2Fmlpds_2023
-00001620: 5f64 656d 6f2e 6970 796e 6229 207c 0a0a  _demo.ipynb) |..
-00001630: 546f 2065 7865 6375 7465 2074 6865 7365  To execute these
-00001640: 206e 6f74 6562 6f6f 6b73 206c 6f63 616c   notebooks local
-00001650: 6c79 2c20 636c 6f6e 6520 7468 6973 2072  ly, clone this r
-00001660: 6570 6f73 6974 6f72 7920 2869 2e65 2e20  epository (i.e. 
-00001670: 6067 6974 2063 6c6f 6e65 2068 7474 7073  `git clone https
-00001680: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00001690: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-000016a0: 7465 732e 6769 7460 292c 206e 6176 6967  tes.git`), navig
-000016b0: 6174 6520 746f 2074 6865 2060 6173 7461  ate to the `asta
-000016c0: 7274 6573 6020 6469 7265 6374 6f72 792c  rtes` directory,
-000016d0: 2072 756e 2060 7069 7020 696e 7374 616c   run `pip instal
-000016e0: 6c20 2e5b 6465 6d6f 735d 602c 2074 6865  l .[demos]`, the
-000016f0: 6e20 6f70 656e 2061 6e64 2072 756e 2074  n open and run t
-00001700: 6865 206e 6f74 6562 6f6f 6b73 2069 6e20  he notebooks in 
-00001710: 796f 7572 2070 7265 6665 7272 6564 2065  your preferred e
-00001720: 6469 746f 722e 0a0a 2323 2320 5261 7469  ditor...### Rati
-00001730: 6f6e 616c 2053 706c 6974 7469 6e67 2041  onal Splitting A
-00001740: 6c67 6f72 6974 686d 730a 5768 696c 6520  lgorithms.While 
-00001750: 6d75 6368 206d 6163 6869 6e65 206c 6561  much machine lea
-00001760: 726e 696e 6720 6973 2064 6f6e 6520 7769  rning is done wi
-00001770: 7468 2061 2072 616e 646f 6d20 6368 6f69  th a random choi
-00001780: 6365 2062 6574 7765 656e 2074 7261 696e  ce between train
-00001790: 696e 672f 7661 6c69 6461 7469 6f6e 2f74  ing/validation/t
-000017a0: 6573 7420 6461 7461 2c20 616e 2061 6c74  est data, an alt
-000017b0: 6572 6e61 7469 7665 2069 7320 7468 6520  ernative is the 
-000017c0: 7573 6520 6f66 2073 6f2d 6361 6c6c 6564  use of so-called
-000017d0: 2022 7261 7469 6f6e 616c 2220 7370 6c69   "rational" spli
-000017e0: 7474 696e 6720 616c 676f 7269 7468 6d73  tting algorithms
-000017f0: 2e20 5468 6573 6520 6170 7072 6f61 6368  . These approach
-00001800: 6573 2075 7365 2073 6f6d 6520 7369 6d69  es use some simi
-00001810: 6c61 7269 7479 2d62 6173 6564 2061 6c67  larity-based alg
-00001820: 6f72 6974 686d 2074 6f20 6469 7669 6465  orithm to divide
-00001830: 2064 6174 6120 696e 746f 2073 6574 732e   data into sets.
-00001840: 2053 6f6d 6520 6f66 2074 6865 7365 2061   Some of these a
-00001850: 6c67 6f72 6974 686d 7320 696e 636c 7564  lgorithms includ
-00001860: 6520 4b65 6e6e 6172 642d 5374 6f6e 652c  e Kennard-Stone,
-00001870: 206d 696e 696d 616c 2074 6573 7420 7365   minimal test se
-00001880: 7420 6469 7373 696d 696c 6172 6974 792c  t dissimilarity,
-00001890: 2061 6e64 2073 7068 6572 6520 6578 636c   and sphere excl
-000018a0: 7573 696f 6e20 616c 676f 7269 7468 6d73  usion algorithms
-000018b0: 205b 6173 2064 6973 6375 7373 6564 2062   [as discussed b
-000018c0: 7920 5472 6f70 7368 6120 6574 2e20 616c  y Tropsha et. al
-000018d0: 5d28 6874 7470 733a 2f2f 7075 6273 2e61  ](https://pubs.a
-000018e0: 6373 2e6f 7267 2f64 6f69 2f70 6466 2f31  cs.org/doi/pdf/1
-000018f0: 302e 3130 3231 2f63 6933 3030 3333 3877  0.1021/ci300338w
-00001900: 2920 6173 2077 656c 6c20 6173 2074 6865  ) as well as the
-00001910: 204f 7074 6953 696d 2061 7320 6469 7363   OptiSim as disc
-00001920: 7573 7365 6420 696e 205b 4170 706c 6965  ussed in [Applie
-00001930: 6420 4368 656d 6f69 6e66 6f72 6d61 7469  d Chemoinformati
-00001940: 6373 3a20 4163 6869 6576 656d 656e 7473  cs: Achievements
-00001950: 2061 6e64 2046 7574 7572 6520 4f70 706f   and Future Oppo
-00001960: 7274 756e 6974 6965 735d 2868 7474 7073  rtunities](https
-00001970: 3a2f 2f77 7777 2e77 696c 6579 2e63 6f6d  ://www.wiley.com
-00001980: 2f65 6e2d 7573 2f41 7070 6c69 6564 2b43  /en-us/Applied+C
-00001990: 6865 6d6f 696e 666f 726d 6174 6963 7325  hemoinformatics%
-000019a0: 3341 2b41 6368 6965 7665 6d65 6e74 732b  3A+Achievements+
-000019b0: 616e 642b 4675 7475 7265 2b4f 7070 6f72  and+Future+Oppor
-000019c0: 7475 6e69 7469 6573 2d70 2d39 3738 3335  tunities-p-97835
-000019d0: 3237 3830 3635 3436 292e 2053 6f6d 6520  27806546). Some 
-000019e0: 636c 7573 7465 7269 6e67 2d62 6173 6564  clustering-based
-000019f0: 2073 706c 6974 7469 6e67 2074 6563 686e   splitting techn
-00001a00: 6971 7565 7320 6861 7665 2061 6c73 6f20  iques have also 
-00001a10: 6265 656e 2069 6e63 6f72 706f 7261 7465  been incorporate
-00001a20: 642c 2073 7563 6820 6173 205b 4442 5343  d, such as [DBSC
-00001a30: 414e 5d28 6874 7470 3a2f 2f63 6974 6573  AN](http://cites
-00001a40: 6565 7278 2e69 7374 2e70 7375 2e65 6475  eerx.ist.psu.edu
-00001a50: 2f76 6965 7764 6f63 2f64 6f77 6e6c 6f61  /viewdoc/downloa
-00001a60: 643f 646f 693d 3130 2e31 2e31 2e31 3031  d?doi=10.1.1.101
-00001a70: 362e 3839 3026 7265 703d 7265 7031 2674  6.890&rep=rep1&t
-00001a80: 7970 653d 7064 6629 2e0a 0a54 6865 7265  ype=pdf)...There
-00001a90: 2061 7265 2074 776f 2062 726f 6164 2063   are two broad c
-00001aa0: 6174 6567 6f72 6965 7320 6f66 2073 616d  ategories of sam
-00001ab0: 706c 696e 6720 616c 676f 7269 7468 6d73  pling algorithms
-00001ac0: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-00001ad0: 6061 7374 6172 7465 7360 3a20 6578 7472  `astartes`: extr
-00001ae0: 6170 6f6c 6174 6976 6520 616e 6420 696e  apolative and in
-00001af0: 7465 7270 6f6c 6174 6976 652e 2054 6865  terpolative. The
-00001b00: 2066 6f72 6d65 7220 7769 6c6c 2066 6f72   former will for
-00001b10: 6365 2079 6f75 7220 6d6f 6465 6c20 746f  ce your model to
-00001b20: 2070 7265 6469 6374 206f 6e20 6f75 742d   predict on out-
-00001b30: 6f66 2d73 616d 706c 6520 6461 7461 2c20  of-sample data, 
-00001b40: 7768 6963 6820 6372 6561 7465 7320 6120  which creates a 
-00001b50: 6d6f 7265 2063 6861 6c6c 656e 6769 6e67  more challenging
-00001b60: 2074 6173 6b20 7468 616e 2069 6e74 6572   task than inter
-00001b70: 706f 6c61 7469 7665 2073 616d 706c 696e  polative samplin
-00001b80: 672e 2053 6565 2074 6865 2074 6162 6c65  g. See the table
-00001b90: 2062 656c 6f77 2066 6f72 2061 6c6c 206f   below for all o
-00001ba0: 6620 7468 6520 7361 6d70 6c69 6e67 2061  f the sampling a
-00001bb0: 7070 726f 6163 6865 7320 6375 7272 656e  pproaches curren
-00001bc0: 746c 7920 696d 706c 656d 656e 7465 6420  tly implemented 
-00001bd0: 696e 2060 6173 7461 7274 6573 602c 2061  in `astartes`, a
-00001be0: 7320 7765 6c6c 2061 7320 7468 6520 6879  s well as the hy
-00001bf0: 7065 7270 6172 616d 6574 6572 7320 7468  perparameters th
-00001c00: 6174 2065 6163 6820 616c 676f 7269 7468  at each algorith
-00001c10: 6d20 6163 6365 7074 7320 2877 6869 6368  m accepts (which
-00001c20: 2061 7265 2070 6173 7365 6420 696e 2077   are passed in w
-00001c30: 6974 6820 6068 6f70 7473 6029 2061 6e64  ith `hopts`) and
-00001c40: 2061 2068 656c 7066 756c 2072 6566 6572   a helpful refer
-00001c50: 656e 6365 2066 6f72 2075 6e64 6572 7374  ence for underst
-00001c60: 616e 6469 6e67 2068 6f77 2074 6865 2068  anding how the h
-00001c70: 7970 6572 7061 7261 6d65 7465 7273 2077  yperparameters w
-00001c80: 6f72 6b2e 204e 6f74 6520 7468 6174 2060  ork. Note that `
-00001c90: 7261 6e64 6f6d 5f73 7461 7465 6020 6973  random_state` is
-00001ca0: 2064 6566 696e 6564 2061 7320 6120 6b65   defined as a ke
-00001cb0: 7977 6f72 6420 6172 6775 6d65 6e74 2069  yword argument i
-00001cc0: 6e20 6074 7261 696e 5f74 6573 745f 7370  n `train_test_sp
-00001cd0: 6c69 7460 2069 7473 656c 662c 2065 7665  lit` itself, eve
-00001ce0: 6e20 7468 6f75 6768 2074 6865 7365 2061  n though these a
-00001cf0: 6c67 6f72 6974 686d 7320 7769 6c6c 2075  lgorithms will u
-00001d00: 7365 2074 6865 2060 7261 6e64 6f6d 5f73  se the `random_s
-00001d10: 7461 7465 6020 696e 2074 6865 6972 206f  tate` in their o
-00001d20: 776e 2077 6f72 6b2e 2044 6f20 6e6f 7420  wn work. Do not 
-00001d30: 7072 6f76 6964 6520 6120 6072 616e 646f  provide a `rando
-00001d40: 6d5f 7374 6174 6560 2069 6e20 7468 6520  m_state` in the 
-00001d50: 6068 6f70 7473 6020 6469 6374 696f 6e61  `hopts` dictiona
-00001d60: 7279 202d 2069 7420 7769 6c6c 2062 6520  ry - it will be 
-00001d70: 6f76 6572 7772 6974 7465 6e20 6279 2074  overwritten by t
-00001d80: 6865 2060 7261 6e64 6f6d 5f73 7461 7465  he `random_state
-00001d90: 6020 796f 7520 7072 6f76 6964 6520 666f  ` you provide fo
-00001da0: 7220 6074 7261 696e 5f74 6573 745f 7370  r `train_test_sp
-00001db0: 6c69 7460 2028 6f72 2074 6865 2064 6566  lit` (or the def
-00001dc0: 6175 6c74 2069 6620 6e6f 6e65 2069 7320  ault if none is 
-00001dd0: 7072 6f76 6964 6564 292e 0a0a 2323 2323  provided)...####
-00001de0: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
-00001df0: 706c 696e 6720 416c 676f 7269 7468 6d73  pling Algorithms
-00001e00: 0a0a 7c20 5361 6d70 6c65 7220 4e61 6d65  ..| Sampler Name
-00001e10: 207c 2055 7361 6765 2053 7472 696e 6720   | Usage String 
-00001e20: 7c20 5479 7065 207c 2048 7970 6572 7061  | Type | Hyperpa
-00001e30: 7261 6d65 7465 7273 207c 2052 6566 6572  rameters | Refer
-00001e40: 656e 6365 207c 204e 6f74 6573 207c 0a7c  ence | Notes |.|
-00001e50: 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d 2d7c 2d2d  :---:|---|---|--
-00001e60: 2d7c 2d2d 2d7c 2d2d 2d7c 0a7c 2052 616e  -|---|---|.| Ran
-00001e70: 646f 6d20 7c20 2772 616e 646f 6d27 207c  dom | 'random' |
-00001e80: 2049 6e74 6572 706f 6c61 7469 7665 207c   Interpolative |
-00001e90: 2060 7368 7566 666c 6560 207c 205b 6073   `shuffle` | [`s
-00001ea0: 6b6c 6561 726e 2074 7261 696e 5f74 6573  klearn train_tes
-00001eb0: 745f 7370 6c69 7460 5d28 6874 7470 733a  t_split`](https:
-00001ec0: 2f2f 7363 696b 6974 2d6c 6561 726e 2e6f  //scikit-learn.o
-00001ed0: 7267 2f73 7461 626c 652f 6d6f 6475 6c65  rg/stable/module
-00001ee0: 732f 6765 6e65 7261 7465 642f 736b 6c65  s/generated/skle
-00001ef0: 6172 6e2e 6d6f 6465 6c5f 7365 6c65 6374  arn.model_select
-00001f00: 696f 6e2e 7472 6169 6e5f 7465 7374 5f73  ion.train_test_s
-00001f10: 706c 6974 2e68 746d 6c29 207c 2054 6869  plit.html) | Thi
-00001f20: 7320 7361 6d70 6c65 7220 6973 2061 2064  s sampler is a d
-00001f30: 6972 6563 7420 7061 7373 7468 726f 7567  irect passthroug
-00001f40: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
-00001f50: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
-00001f60: 6974 602c 2074 686f 7567 6820 6974 2064  it`, though it d
-00001f70: 6f65 7320 6e6f 7420 6375 7272 656e 746c  oes not currentl
-00001f80: 7920 7265 7072 6f64 7563 6520 7370 6c69  y reproduce spli
-00001f90: 7473 2069 6465 6e74 6963 616c 6c79 2e20  ts identically. 
-00001fa0: 7c0a 7c20 4b65 6e6e 6172 642d 5374 6f6e  |.| Kennard-Ston
-00001fb0: 6520 7c20 276b 656e 6e61 7264 5f73 746f  e | 'kennard_sto
-00001fc0: 6e65 2720 7c20 496e 7465 7270 6f6c 6174  ne' | Interpolat
-00001fd0: 6976 6520 7c20 606d 6574 7269 6360 207c  ive | `metric` |
-00001fe0: 205b 4b65 6e6e 6172 6420 2620 5374 6f6e   [Kennard & Ston
-00001ff0: 655d 2868 7474 7073 3a2f 2f77 7777 2e74  e](https://www.t
-00002000: 616e 6466 6f6e 6c69 6e65 2e63 6f6d 2f64  andfonline.com/d
-00002010: 6f69 2f61 6273 2f31 302e 3130 3830 2f30  oi/abs/10.1080/0
-00002020: 3034 3031 3730 362e 3139 3639 2e31 3034  0401706.1969.104
-00002030: 3930 3636 3629 207c 2045 7563 6c69 6469  90666) | Euclidi
-00002040: 616e 2064 6973 7461 6e63 6520 6973 2075  an distance is u
-00002050: 7365 6420 6279 2064 6566 6175 6c74 2c20  sed by default, 
-00002060: 6173 2064 6573 6372 6962 6564 2069 6e20  as described in 
-00002070: 7468 6520 6f72 6967 696e 616c 2070 6170  the original pap
-00002080: 6572 2e20 7c0a 7c20 5361 6d70 6c65 2073  er. |.| Sample s
-00002090: 6574 2050 6172 7469 7469 6f6e 696e 6720  et Partitioning 
-000020a0: 6261 7365 6420 6f6e 206a 6f69 6e74 2058  based on joint X
-000020b0: 2d59 2064 6973 7461 6e63 6573 2028 5350  -Y distances (SP
-000020c0: 5859 2920 7c20 2773 7078 7927 207c 2049  XY) | 'spxy' | I
-000020d0: 6e74 6572 706f 6c61 7469 7665 207c 2060  nterpolative | `
-000020e0: 6469 7374 616e 6365 5f6d 6574 7269 6360  distance_metric`
-000020f0: 207c 2053 616c 6468 616e 6120 6574 2e20   | Saldhana et. 
-00002100: 616c 205b 6f72 6967 696e 616c 2070 6170  al [original pap
-00002110: 6572 5d28 6874 7470 733a 2f2f 7777 772e  er](https://www.
-00002120: 7363 6965 6e63 6564 6972 6563 742e 636f  sciencedirect.co
-00002130: 6d2f 7363 6965 6e63 652f 6172 7469 636c  m/science/articl
-00002140: 652f 6162 732f 7069 692f 5330 3033 3939  e/abs/pii/S00399
-00002150: 3134 3030 3530 3031 3932 5829 207c 2045  1400500192X) | E
-00002160: 7874 656e 7369 6f6e 206f 6620 4b65 6e6e  xtension of Kenn
-00002170: 6172 6420 5374 6f6e 6520 7468 6174 2061  ard Stone that a
-00002180: 6c73 6f20 696e 636c 7564 6573 2074 6865  lso includes the
-00002190: 2072 6573 706f 6e73 6520 7768 656e 2073   response when s
-000021a0: 616d 706c 696e 6720 6469 7374 616e 6365  ampling distance
-000021b0: 732e 207c 0a7c 2053 6361 6666 6f6c 6420  s. |.| Scaffold 
-000021c0: 7c20 2773 6361 6666 6f6c 6427 207c 2045  | 'scaffold' | E
-000021d0: 7874 7261 706f 6c61 7469 7665 207c 2060  xtrapolative | `
-000021e0: 696e 636c 7564 655f 6368 6972 616c 6974  include_chiralit
-000021f0: 7960 207c 205b 4265 6d69 732d 4d75 7263  y` | [Bemis-Murc
-00002200: 6b6f 2053 6361 6666 6f6c 645d 2868 7474  ko Scaffold](htt
-00002210: 7073 3a2f 2f70 7562 732e 6163 732e 6f72  ps://pubs.acs.or
-00002220: 672f 646f 692f 6675 6c6c 2f31 302e 3130  g/doi/full/10.10
-00002230: 3231 2f6a 6d39 3630 3239 3238 2920 6173  21/jm9602928) as
-00002240: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-00002250: 5244 4b69 7420 7c20 5468 6973 2073 616d  RDKit | This sam
-00002260: 706c 6572 2072 6571 7569 7265 7320 534d  pler requires SM
-00002270: 494c 4553 2073 7472 696e 6773 2061 7320  ILES strings as 
-00002280: 696e 7075 7420 2875 7365 2074 6865 2060  input (use the `
-00002290: 6d6f 6c65 6375 6c65 7360 2073 7562 7061  molecules` subpa
-000022a0: 636b 6167 6529 207c 0a7c 2053 7068 6572  ckage) |.| Spher
-000022b0: 6520 4578 636c 7573 696f 6e20 7c20 2773  e Exclusion | 's
-000022c0: 7068 6572 655f 6578 636c 7573 696f 6e27  phere_exclusion'
-000022d0: 207c 2045 7874 7261 706f 6c61 7469 7665   | Extrapolative
-000022e0: 207c 2060 6d65 7472 6963 602c 2060 6469   | `metric`, `di
-000022f0: 7374 616e 6365 5f63 7574 6f66 6660 207c  stance_cutoff` |
-00002300: 205f 6375 7374 6f6d 2069 6d70 6c65 6d65   _custom impleme
-00002310: 6e74 6174 696f 6e5f 207c 2056 6172 6961  ntation_ | Varia
-00002320: 7469 6f6e 206f 6e20 5370 6865 7265 2045  tion on Sphere E
-00002330: 7863 6c75 7369 6f6e 2066 6f72 2061 7262  xclusion for arb
-00002340: 6974 7261 7279 2d76 616c 7565 6420 7665  itrary-valued ve
-00002350: 6374 6f72 732e 207c 0a7c 2054 696d 6520  ctors. |.| Time 
-00002360: 4261 7365 6420 7c20 2774 696d 655f 6261  Based | 'time_ba
-00002370: 7365 6427 207c 2045 7874 7261 706f 6c61  sed' | Extrapola
-00002380: 7469 7665 207c 205f 6e6f 6e65 5f20 7c20  tive | _none_ | 
-00002390: 5b43 6865 6e20 6574 2061 6c2e 5d28 6874  [Chen et al.](ht
-000023a0: 7470 733a 2f2f 7075 6273 2e61 6373 2e6f  tps://pubs.acs.o
-000023b0: 7267 2f64 6f69 2f66 756c 6c2f 3130 2e31  rg/doi/full/10.1
-000023c0: 3032 312f 6369 3230 3036 3135 6829 2c20  021/ci200615h), 
-000023d0: 5b53 6865 7269 6461 6e2c 2052 2e20 505d  [Sheridan, R. P]
-000023e0: 2868 7474 7073 3a2f 2f70 7562 732e 6163  (https://pubs.ac
-000023f0: 732e 6f72 672f 646f 692f 6675 6c6c 2f31  s.org/doi/full/1
-00002400: 302e 3130 3231 2f63 6934 3030 3038 346b  0.1021/ci400084k
-00002410: 292c 205b 4665 696e 6265 7267 2065 7420  ), [Feinberg et 
-00002420: 616c 2e5d 2868 7474 7073 3a2f 2f70 7562  al.](https://pub
-00002430: 732e 6163 732e 6f72 672f 646f 692f 6675  s.acs.org/doi/fu
-00002440: 6c6c 2f31 302e 3130 3231 2f61 6373 2e6a  ll/10.1021/acs.j
-00002450: 6d65 6463 6865 6d2e 3962 3032 3138 3729  medchem.9b02187)
-00002460: 2c20 5b53 7472 7562 6c65 2065 7420 616c  , [Struble et al
-00002470: 2e5d 2868 7474 7073 3a2f 2f70 7562 732e  .](https://pubs.
-00002480: 7273 632e 6f72 672f 656e 2f63 6f6e 7465  rsc.org/en/conte
-00002490: 6e74 2f61 7274 6963 6c65 6874 6d6c 2f32  nt/articlehtml/2
-000024a0: 3032 302f 7265 2f64 3072 6530 3030 3731  020/re/d0re00071
-000024b0: 6a29 2020 7c20 5468 6973 2073 616d 706c  j)  | This sampl
-000024c0: 6572 2072 6571 7569 7265 7320 606c 6162  er requires `lab
-000024d0: 656c 7360 2074 6f20 6265 2061 6e20 6974  els` to be an it
-000024e0: 6572 6162 6c65 206f 6620 6569 7468 6572  erable of either
-000024f0: 2064 6174 6520 6f72 2064 6174 6574 696d   date or datetim
-00002500: 6520 6f62 6a65 6374 732e 207c 0a7c 204f  e objects. |.| O
-00002510: 7074 696d 697a 6162 6c65 204b 2d44 6973  ptimizable K-Dis
-00002520: 7369 6d69 6c61 7269 7479 2053 656c 6563  similarity Selec
-00002530: 7469 6f6e 2028 4f70 7469 5369 6d29 207c  tion (OptiSim) |
-00002540: 2027 6f70 7469 7369 6d27 207c 2045 7874   'optisim' | Ext
-00002550: 7261 706f 6c61 7469 7665 207c 2060 6e5f  rapolative | `n_
-00002560: 636c 7573 7465 7273 602c 2060 6d61 785f  clusters`, `max_
-00002570: 7375 6273 616d 706c 655f 7369 7a65 602c  subsample_size`,
-00002580: 2060 6469 7374 616e 6365 5f63 7574 6f66   `distance_cutof
-00002590: 6660 207c 205f 6375 7374 6f6d 2069 6d70  f` | _custom imp
-000025a0: 6c65 6d65 6e74 6174 696f 6e5f 207c 2056  lementation_ | V
-000025b0: 6172 6961 7469 6f6e 206f 6e20 5b4f 7074  ariation on [Opt
-000025c0: 6953 696d 5d28 6874 7470 733a 2f2f 7075  iSim](https://pu
-000025d0: 6273 2e61 6373 2e6f 7267 2f64 6f69 2f31  bs.acs.org/doi/1
-000025e0: 302e 3130 3231 2f63 6930 3235 3636 3268  0.1021/ci025662h
-000025f0: 2920 666f 7220 6172 6269 7472 6172 792d  ) for arbitrary-
-00002600: 7661 6c75 6564 2076 6563 746f 7273 2e20  valued vectors. 
-00002610: 7c0a 7c20 4b2d 4d65 616e 7320 7c20 276b  |.| K-Means | 'k
-00002620: 6d65 616e 7327 207c 2045 7874 7261 706f  means' | Extrapo
-00002630: 6c61 7469 7665 207c 2060 6e5f 636c 7573  lative | `n_clus
-00002640: 7465 7273 602c 2060 6e5f 696e 6974 6020  ters`, `n_init` 
-00002650: 7c20 5b60 736b 6c65 6172 6e20 4b4d 6561  | [`sklearn KMea
-00002660: 6e73 605d 2868 7474 7073 3a2f 2f73 6369  ns`](https://sci
-00002670: 6b69 742d 6c65 6172 6e2e 6f72 672f 7374  kit-learn.org/st
-00002680: 6162 6c65 2f6d 6f64 756c 6573 2f67 656e  able/modules/gen
-00002690: 6572 6174 6564 2f73 6b6c 6561 726e 2e63  erated/sklearn.c
-000026a0: 6c75 7374 6572 2e4b 4d65 616e 732e 6874  luster.KMeans.ht
-000026b0: 6d6c 2920 7c20 5061 7373 7468 726f 7567  ml) | Passthroug
-000026c0: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
-000026d0: 2060 4b4d 6561 6e73 602e 207c 0a7c 2044   `KMeans`. |.| D
-000026e0: 656e 7369 7479 2d42 6173 6564 2053 7061  ensity-Based Spa
-000026f0: 7469 616c 2043 6c75 7374 6572 696e 6720  tial Clustering 
-00002700: 6f66 2041 7070 6c69 6361 7469 6f6e 7320  of Applications 
-00002710: 7769 7468 204e 6f69 7365 2028 4442 5343  with Noise (DBSC
-00002720: 414e 2920 7c20 2764 6273 6361 6e27 207c  AN) | 'dbscan' |
-00002730: 2045 7874 7261 706f 6c61 7469 7665 207c   Extrapolative |
-00002740: 2060 6570 7360 2c20 606d 696e 5f73 616d   `eps`, `min_sam
-00002750: 706c 6573 602c 2060 616c 676f 7269 7468  ples`, `algorith
-00002760: 6d60 2c20 606d 6574 7269 6360 2c20 606c  m`, `metric`, `l
-00002770: 6561 665f 7369 7a65 6020 7c20 5b60 736b  eaf_size` | [`sk
-00002780: 6c65 6172 6e20 4442 5343 414e 605d 2868  learn DBSCAN`](h
-00002790: 7474 7073 3a2f 2f73 6369 6b69 742d 6c65  ttps://scikit-le
-000027a0: 6172 6e2e 6f72 672f 7374 6162 6c65 2f6d  arn.org/stable/m
-000027b0: 6f64 756c 6573 2f67 656e 6572 6174 6564  odules/generated
-000027c0: 2f73 6b6c 6561 726e 2e63 6c75 7374 6572  /sklearn.cluster
-000027d0: 2e44 4253 4341 4e2e 6874 6d6c 2920 7c20  .DBSCAN.html) | 
-000027e0: 5061 7373 7468 726f 7567 6820 746f 2060  Passthrough to `
-000027f0: 736b 6c65 6172 6e60 2773 2060 4442 5343  sklearn`'s `DBSC
-00002800: 414e 602e 207c 0a7c 204d 696e 696d 756d  AN`. |.| Minimum
-00002810: 2054 6573 7420 5365 7420 4469 7373 696d   Test Set Dissim
-00002820: 696c 6172 6974 7920 284d 5453 4429 207c  ilarity (MTSD) |
-00002830: 207e 207c 207e 207c 205f 7570 636f 6d69   ~ | ~ | _upcomi
-00002840: 6e67 2069 6e5f 2060 6173 7461 7274 6573  ng in_ `astartes
-00002850: 6020 5f76 312e 785f 207c 207e 207c 207e  ` _v1.x_ | ~ | ~
-00002860: 207c 0a7c 2052 6573 7472 6963 7465 6420   |.| Restricted 
-00002870: 426f 6c74 7a6d 616e 6e20 4d61 6368 696e  Boltzmann Machin
-00002880: 6520 2852 424d 2920 7c20 7e20 7c20 7e20  e (RBM) | ~ | ~ 
-00002890: 7c20 5f75 7063 6f6d 696e 6720 696e 5f20  | _upcoming in_ 
-000028a0: 6061 7374 6172 7465 7360 205f 7631 2e78  `astartes` _v1.x
-000028b0: 5f20 7c20 7e20 7c20 7e20 7c0a 7c20 4b6f  _ | ~ | ~ |.| Ko
-000028c0: 686f 6e65 6e20 5365 6c66 2d4f 7267 616e  honen Self-Organ
-000028d0: 697a 696e 6720 4d61 7020 2853 4f4d 2920  izing Map (SOM) 
-000028e0: 7c20 7e20 7c20 7e20 7c20 5f75 7063 6f6d  | ~ | ~ | _upcom
-000028f0: 696e 6720 696e 5f20 6061 7374 6172 7465  ing in_ `astarte
-00002900: 7360 205f 7631 2e78 5f20 7c20 7e20 7c20  s` _v1.x_ | ~ | 
-00002910: 7e20 7c0a 7c20 5350 6c69 7420 4d65 7468  ~ |.| SPlit Meth
-00002920: 6f64 207c 207e 207c 207e 207c 205f 7570  od | ~ | ~ | _up
-00002930: 636f 6d69 6e67 2069 6e5f 2060 6173 7461  coming in_ `asta
-00002940: 7274 6573 6020 5f76 312e 785f 207c 207e  rtes` _v1.x_ | ~
-00002950: 207c 207e 207c 0a0a 2323 2320 5573 696e   | ~ |..### Usin
-00002960: 6720 7468 6520 6061 7374 6172 7465 732e  g the `astartes.
-00002970: 6d6f 6c65 6375 6c65 7360 2053 7562 7061  molecules` Subpa
-00002980: 636b 6167 650a 4166 7465 7220 696e 7374  ckage.After inst
-00002990: 616c 6c69 6e67 2077 6974 6820 6070 6970  alling with `pip
-000029a0: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
-000029b0: 735b 6d6f 6c65 6375 6c65 735d 6020 6f6e  s[molecules]` on
-000029c0: 6520 6361 6e20 696d 706f 7274 2074 6865  e can import the
-000029d0: 206e 6577 2074 7261 696e 2f74 6573 7420   new train/test 
-000029e0: 7370 6c69 7474 696e 6720 6675 6e63 7469  splitting functi
-000029f0: 6f6e 206c 696b 6520 7468 6973 3a20 6066  on like this: `f
-00002a00: 726f 6d20 6173 7461 7274 6573 2e6d 6f6c  rom astartes.mol
-00002a10: 6563 756c 6573 2069 6d70 6f72 7420 7472  ecules import tr
-00002a20: 6169 6e5f 7465 7374 5f73 706c 6974 5f6d  ain_test_split_m
-00002a30: 6f6c 6563 756c 6573 600a 0a54 6865 2075  olecules`..The u
-00002a40: 7361 6765 206f 6620 7468 6973 2066 756e  sage of this fun
-00002a50: 6374 696f 6e20 6973 2069 6465 6e74 6963  ction is identic
-00002a60: 616c 2074 6f20 6074 7261 696e 5f74 6573  al to `train_tes
-00002a70: 745f 7370 6c69 7460 2062 7574 2077 6974  t_split` but wit
-00002a80: 6820 7468 6520 6164 6469 7469 6f6e 206f  h the addition o
-00002a90: 6620 6e65 7720 6172 6775 6d65 6e74 7320  f new arguments 
-00002aa0: 746f 2063 6f6e 7472 6f6c 2068 6f77 2074  to control how t
-00002ab0: 6865 206d 6f6c 6563 756c 6573 2061 7265  he molecules are
-00002ac0: 2066 6561 7475 7269 7a65 643a 0a0a 6060   featurized:..``
-00002ad0: 6070 7974 686f 6e0a 7472 6169 6e5f 7465  `python.train_te
-00002ae0: 7374 5f73 706c 6974 5f6d 6f6c 6563 756c  st_split_molecul
-00002af0: 6573 280a 2020 2020 6d6f 6c65 6375 6c65  es(.    molecule
-00002b00: 733d 736d 696c 6573 2c0a 2020 2020 793d  s=smiles,.    y=
-00002b10: 792c 0a20 2020 2074 6573 745f 7369 7a65  y,.    test_size
-00002b20: 3d30 2e32 2c0a 2020 2020 7472 6169 6e5f  =0.2,.    train_
-00002b30: 7369 7a65 3d30 2e38 2c0a 2020 2020 6669  size=0.8,.    fi
-00002b40: 6e67 6572 7072 696e 743d 2264 6179 6c69  ngerprint="dayli
-00002b50: 6768 745f 6669 6e67 6572 7072 696e 7422  ght_fingerprint"
-00002b60: 2c0a 2020 2020 6670 7269 6e74 735f 686f  ,.    fprints_ho
-00002b70: 7074 733d 7b0a 2020 2020 2020 2020 226d  pts={.        "m
-00002b80: 696e 5061 7468 223a 2032 2c0a 2020 2020  inPath": 2,.    
-00002b90: 2020 2020 226d 6178 5061 7468 223a 2035      "maxPath": 5
-00002ba0: 2c0a 2020 2020 2020 2020 2266 7053 697a  ,.        "fpSiz
-00002bb0: 6522 3a20 3230 302c 0a20 2020 2020 2020  e": 200,.       
-00002bc0: 2022 6269 7473 5065 7248 6173 6822 3a20   "bitsPerHash": 
-00002bd0: 342c 0a20 2020 2020 2020 2022 7573 6548  4,.        "useH
-00002be0: 7322 3a20 312c 0a20 2020 2020 2020 2022  s": 1,.        "
-00002bf0: 7467 7444 656e 7369 7479 223a 2030 2e34  tgtDensity": 0.4
-00002c00: 2c0a 2020 2020 2020 2020 226d 696e 5369  ,.        "minSi
-00002c10: 7a65 223a 2036 342c 0a20 2020 207d 2c0a  ze": 64,.    },.
-00002c20: 2020 2020 7361 6d70 6c65 723d 2272 616e      sampler="ran
-00002c30: 646f 6d22 2c0a 2020 2020 7261 6e64 6f6d  dom",.    random
-00002c40: 5f73 7461 7465 3d34 322c 0a20 2020 2068  _state=42,.    h
-00002c50: 6f70 7473 3d7b 0a20 2020 2020 2020 2022  opts={.        "
-00002c60: 7368 7566 666c 6522 3a20 5472 7565 2c0a  shuffle": True,.
-00002c70: 2020 2020 7d2c 0a29 0a60 6060 0a0a 546f      },.).```..To
-00002c80: 2073 6565 2061 2063 6f6d 706c 6574 6520   see a complete 
-00002c90: 6578 616d 706c 6520 6f66 2075 7369 6e67  example of using
-00002ca0: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
-00002cb0: 6974 5f6d 6f6c 6563 756c 6573 6020 7769  it_molecules` wi
-00002cc0: 7468 2061 6374 7561 6c20 6368 656d 6963  th actual chemic
-00002cd0: 616c 2064 6174 612c 2074 616b 6520 6120  al data, take a 
-00002ce0: 6c6f 6f6b 2069 6e20 7468 6520 6065 7861  look in the `exa
-00002cf0: 6d70 6c65 7360 2064 6972 6563 746f 7279  mples` directory
-00002d00: 2e0a 0a43 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
-00002d10: 206f 7074 696f 6e73 2066 6f72 2074 6865   options for the
-00002d20: 2066 6561 7475 7269 7a61 7469 6f6e 2073   featurization s
-00002d30: 6368 656d 6520 6361 6e20 6265 2066 6f75  cheme can be fou
-00002d40: 6e64 2069 6e20 7468 6520 646f 6375 6d65  nd in the docume
-00002d50: 6e74 6174 696f 6e20 666f 7220 5b60 4149  ntation for [`AI
-00002d60: 4d53 696d 605d 2868 7474 7073 3a2f 2f76  MSim`](https://v
-00002d70: 6c61 6368 6f73 6772 6f75 702e 6769 7468  lachosgroup.gith
-00002d80: 7562 2e69 6f2f 4149 4d53 696d 2f52 4541  ub.io/AIMSim/REA
-00002d90: 444d 452e 6874 6d6c 2363 7572 7265 6e74  DME.html#current
-00002da0: 6c79 2d69 6d70 6c65 6d65 6e74 6564 2d66  ly-implemented-f
-00002db0: 696e 6765 7270 7269 6e74 7329 2074 686f  ingerprints) tho
-00002dc0: 7567 6820 6d6f 7374 206f 6620 7468 6520  ugh most of the 
-00002dd0: 6372 6974 6963 616c 2063 6f6e 6669 6775  critical configu
-00002de0: 7261 7469 6f6e 206f 7074 696f 6e73 2061  ration options a
-00002df0: 7265 2073 686f 776e 2061 626f 7665 2e0a  re shown above..
-00002e00: 0a23 2323 2052 6570 726f 6475 6369 6269  .### Reproducibi
-00002e10: 6c69 7479 0a60 6173 7461 7274 6573 6020  lity.`astartes` 
-00002e20: 6169 6d73 2074 6f20 6265 2063 6f6d 706c  aims to be compl
-00002e30: 6574 656c 7920 7265 7072 6f64 7563 6962  etely reproducib
-00002e40: 6c65 2061 6372 6f73 7320 6469 6666 6572  le across differ
-00002e50: 656e 7420 706c 6174 666f 726d 732c 2050  ent platforms, P
-00002e60: 7974 686f 6e20 7665 7273 696f 6e73 2c20  ython versions, 
-00002e70: 616e 6420 6465 7065 6e64 656e 6379 2063  and dependency c
-00002e80: 6f6e 6669 6775 7261 7469 6f6e 7320 2d20  onfigurations - 
-00002e90: 616e 7920 7665 7273 696f 6e20 6f66 2060  any version of `
-00002ea0: 6173 7461 7274 6573 6020 7631 2e78 2073  astartes` v1.x s
-00002eb0: 686f 756c 6420 7265 7375 6c74 2069 6e20  hould result in 
-00002ec0: 7468 6520 5f65 7861 6374 5f20 7361 6d65  the _exact_ same
-00002ed0: 2073 706c 6974 732c 2061 6c77 6179 732e   splits, always.
-00002ee0: 0a54 6f20 7468 6174 2065 6e64 2c20 7468  .To that end, th
-00002ef0: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
-00002f00: 6f72 206f 6620 6061 7374 6172 7465 7360  or of `astartes`
-00002f10: 2069 7320 746f 2075 7365 2060 3432 6020   is to use `42` 
-00002f20: 6173 2074 6865 2072 616e 646f 6d20 7365  as the random se
-00002f30: 6564 2061 6e64 205f 616c 7761 7973 5f20  ed and _always_ 
-00002f40: 7365 7420 6974 2e0a 5275 6e6e 696e 6720  set it..Running 
-00002f50: 6061 7374 6172 7465 7360 2077 6974 6820  `astartes` with 
-00002f60: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
-00002f70: 696e 6773 2077 696c 6c20 616c 7761 7973  ings will always
-00002f80: 2070 726f 6475 6365 2074 6865 2065 7861   produce the exa
-00002f90: 6374 2073 616d 6520 7265 7375 6c74 732e  ct same results.
-00002fa0: 0a57 6520 6861 7665 2076 6572 6966 6965  .We have verifie
-00002fb0: 6420 7468 6973 2062 6568 6176 696f 7220  d this behavior 
-00002fc0: 6f6e 2044 6562 6961 6e20 5562 756e 7475  on Debian Ubuntu
-00002fd0: 2c20 5769 6e64 6f77 732c 2061 6e64 2049  , Windows, and I
-00002fe0: 6e74 656c 204d 6163 7320 6672 6f6d 2050  ntel Macs from P
-00002ff0: 7974 686f 6e20 7665 7273 696f 6e73 2033  ython versions 3
-00003000: 2e37 2074 6872 6f75 6768 2033 2e31 3120  .7 through 3.11 
-00003010: 2877 6974 6820 6170 7072 6f70 7269 6174  (with appropriat
-00003020: 6520 6465 7065 6e64 656e 6369 6573 2066  e dependencies f
-00003030: 6f72 2065 6163 6820 7665 7273 696f 6e29  or each version)
-00003040: 2e0a 0a23 2323 2320 4b6e 6f77 6e20 5265  ...#### Known Re
-00003050: 7072 6f64 7563 6962 696c 6974 7920 4c69  producibility Li
-00003060: 6d69 7461 7469 6f6e 730a 0a3e 202a 2a4e  mitations..> **N
-00003070: 6f74 652a 2a0a 3e20 5765 2061 7265 206c  ote**.> We are l
-00003080: 696d 6974 6564 2069 6e20 6f75 7220 6162  imited in our ab
-00003090: 696c 6974 7920 746f 2074 6573 7420 6f6e  ility to test on
-000030a0: 204d 3120 4d61 6373 2c20 6275 7420 6672   M1 Macs, but fr
-000030b0: 6f6d 206f 7572 206c 696d 6974 6564 206d  om our limited m
-000030c0: 616e 7561 6c20 7465 7374 696e 6720 7765  anual testing we
-000030d0: 2061 6368 6965 7665 2070 6572 6665 6374   achieve perfect
-000030e0: 2072 6570 726f 6475 6362 696c 6974 7920   reproducbility 
-000030f0: 696e 2061 6c6c 2063 6173 6573 205f 6578  in all cases _ex
-00003100: 6365 7074 206f 6363 6173 696f 6e61 6c6c  cept occasionall
-00003110: 795f 2077 6974 6820 604b 4d65 616e 7360  y_ with `KMeans`
-00003120: 206f 6e20 4170 706c 6520 7369 6c69 636f   on Apple silico
-00003130: 6e2e 0a49 7420 6861 7320 7072 6f64 7563  n..It has produc
-00003140: 6564 205f 736c 6967 6874 6c79 5f20 6469  ed _slightly_ di
-00003150: 6666 6572 656e 7420 7265 7375 6c74 7320  fferent results 
-00003160: 6265 7477 6565 6e20 706c 6174 666f 726d  between platform
-00003170: 7320 7265 6761 7264 6c65 7373 206f 6620  s regardless of 
-00003180: 6072 616e 646f 6d5f 7374 6174 6560 2c20  `random_state`, 
-00003190: 7769 7468 2075 7020 746f 2074 776f 2063  with up to two c
-000031a0: 6c75 7374 6572 7320 6265 696e 6720 6173  lusters being as
-000031b0: 7369 676e 6564 2064 6966 6665 7265 6e74  signed different
-000031c0: 6c79 2072 6573 756c 7469 6e67 2069 6e20  ly resulting in 
-000031d0: 6461 7461 2073 706c 6974 7320 7768 6963  data splits whic
-000031e0: 6820 6172 6520 3e39 3925 2069 6465 6e74  h are >99% ident
-000031f0: 6963 616c 2e0a 6061 7374 6172 7465 7360  ical..`astartes`
-00003200: 2069 7320 7374 696c 6c20 636f 6e73 6973   is still consis
-00003210: 7465 6e74 2062 6574 7765 656e 2072 756e  tent between run
-00003220: 7320 6f6e 2074 6865 2073 616d 6520 706c  s on the same pl
-00003230: 6174 666f 726d 2069 6e20 616c 6c20 6361  atform in all ca
-00003240: 7365 732c 2061 6e64 206f 7468 6572 2073  ses, and other s
-00003250: 616d 706c 6572 7320 6172 6520 6e6f 7420  amplers are not 
-00003260: 696d 7061 6374 6564 2062 7920 7468 6973  impacted by this
-00003270: 2061 7070 6172 656e 7420 6275 672e 0a0a   apparent bug...
-00003280: 202d 2060 736b 6c65 6172 6e60 2076 312e   - `sklearn` v1.
-00003290: 332e 3020 696e 7472 6f64 7563 6564 2062  3.0 introduced b
-000032a0: 6163 6b77 6172 6473 2d69 6e63 6f6d 7061  ackwards-incompa
-000032b0: 7469 626c 6520 6368 616e 6765 7320 696e  tible changes in
-000032c0: 2074 6865 2060 4b4d 6561 6e73 6020 7361   the `KMeans` sa
-000032d0: 6d70 6c65 7220 7468 6174 2063 6861 6e67  mpler that chang
-000032e0: 6564 2068 6f77 2074 6865 2072 616e 646f  ed how the rando
-000032f0: 6d20 696e 6974 6961 6c69 7a61 7469 6f6e  m initialization
-00003300: 2061 6666 6563 7473 2074 6865 2072 6573   affects the res
-00003310: 756c 7473 2c20 6576 656e 2067 6976 656e  ults, even given
-00003320: 2074 6865 2073 616d 6520 7261 6e64 6f6d   the same random
-00003330: 2073 6565 642e 2044 6966 6665 7265 6e74   seed. Different
-00003340: 2076 6572 7369 6f6e 206f 6620 6073 6b6c   version of `skl
-00003350: 6561 726e 6020 7769 6c6c 2061 6666 6563  earn` will affec
-00003360: 7420 7468 6520 7065 7266 6f72 6d61 6e63  t the performanc
-00003370: 6520 6f66 2060 6173 7461 7274 6573 6020  e of `astartes` 
-00003380: 616e 6420 7765 2072 6563 6f6d 6d65 6e64  and we recommend
-00003390: 2069 6e63 6c75 6469 6e67 2074 6865 2065   including the e
-000033a0: 7861 6374 2076 6572 7369 6f6e 206f 6620  xact version of 
-000033b0: 6073 6369 6b69 742d 6c65 6172 6e60 2061  `scikit-learn` a
-000033c0: 6e64 2060 6173 7461 7274 6573 6020 7573  nd `astartes` us
-000033d0: 6564 2c20 7768 656e 2061 7070 6c69 6361  ed, when applica
-000033e0: 626c 652e 0a0a 2323 2045 7661 6c75 6174  ble...## Evaluat
-000033f0: 6520 7468 6520 496d 7061 6374 206f 6620  e the Impact of 
-00003400: 5370 6c69 7474 696e 6720 416c 676f 7269  Splitting Algori
-00003410: 7468 6d73 0a54 6865 2060 6765 6e65 7261  thms.The `genera
-00003420: 7465 5f72 6567 7265 7373 696f 6e5f 7265  te_regression_re
-00003430: 7375 6c74 735f 6469 6374 6020 6675 6e63  sults_dict` func
-00003440: 7469 6f6e 2061 6c6c 6f77 7320 7573 6572  tion allows user
-00003450: 7320 746f 2071 7569 636b 6c79 2065 7661  s to quickly eva
-00003460: 6c75 6174 6520 7468 6520 696d 7061 6374  luate the impact
-00003470: 206f 6620 6469 6666 6572 656e 7420 7370   of different sp
-00003480: 6c69 7474 696e 6720 7465 6368 6e69 7175  litting techniqu
-00003490: 6573 206f 6e20 616e 7920 6d6f 6465 6c20  es on any model 
-000034a0: 7375 7070 6f72 7465 6420 6279 2060 736b  supported by `sk
-000034b0: 6c65 6172 6e60 2e20 416c 6c20 7265 7375  learn`. All resu
-000034c0: 6c74 7320 6172 6520 7374 6f72 6564 2069  lts are stored i
-000034d0: 6e20 6120 6469 6374 696f 6e61 7279 2066  n a dictionary f
-000034e0: 6f72 6d61 7420 616e 6420 6361 6e20 6265  ormat and can be
-000034f0: 2064 6973 706c 6179 6564 2069 6e20 6120   displayed in a 
-00003500: 6e65 6174 6c79 2066 6f72 6d61 7474 6564  neatly formatted
-00003510: 2074 6162 6c65 2075 7369 6e67 2074 6865   table using the
-00003520: 206f 7074 696f 6e61 6c20 6070 7269 6e74   optional `print
-00003530: 5f72 6573 756c 7473 6020 6172 6775 6d65  _results` argume
-00003540: 6e74 2e0a 0a60 6060 0a66 726f 6d20 736b  nt...```.from sk
-00003550: 6c65 6172 6e2e 7376 6d20 696d 706f 7274  learn.svm import
-00003560: 204c 696e 6561 7253 5652 0a0a 6672 6f6d   LinearSVR..from
-00003570: 2061 7374 6172 7465 732e 7574 696c 7320   astartes.utils 
-00003580: 696d 706f 7274 2067 656e 6572 6174 655f  import generate_
-00003590: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
-000035a0: 7473 5f64 6963 740a 0a73 6b6c 6561 726e  ts_dict..sklearn
-000035b0: 5f6d 6f64 656c 203d 204c 696e 6561 7253  _model = LinearS
-000035c0: 5652 2829 0a72 6573 756c 7473 5f64 6963  VR().results_dic
-000035d0: 7420 3d20 6765 6e65 7261 7465 5f72 6567  t = generate_reg
-000035e0: 7265 7373 696f 6e5f 7265 7375 6c74 735f  ression_results_
-000035f0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00003600: 2020 2020 2020 2020 2020 736b 6c65 6172            sklear
-00003610: 6e5f 6d6f 6465 6c2c 0a20 2020 2020 2020  n_model,.       
-00003620: 2020 2020 2020 2020 2020 2020 2058 2c0a               X,.
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 792c 0a20 2020 2020 2020 2020      y,.         
-00003650: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003660: 5f72 6573 756c 7473 3d54 7275 652c 0a20  _results=True,. 
-00003670: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00003680: 0a20 2020 2020 2020 2020 5472 6169 6e20  .         Train 
-00003690: 2020 2020 2020 5661 6c20 2020 2020 2054        Val      T
-000036a0: 6573 740a 2d2d 2d2d 2020 2d2d 2d2d 2d2d  est.----  ------
-000036b0: 2d2d 2020 2d2d 2d2d 2d2d 2d2d 2020 2d2d  --  --------  --
-000036c0: 2d2d 2d2d 2d2d 0a4d 4145 2020 2031 2e34  ------.MAE   1.4
-000036d0: 3135 3232 2020 2033 2e31 3334 3335 2020  1522   3.13435  
-000036e0: 2032 2e31 3730 3931 0a52 4d53 4520 2032   2.17091.RMSE  2
-000036f0: 2e30 3330 3632 2020 2033 2e37 3337 3231  .03062   3.73721
-00003700: 2020 2032 2e34 3030 3431 0a52 3220 2020     2.40041.R2   
-00003710: 2030 2e39 3037 3435 2020 2030 2e38 3037   0.90745   0.807
-00003720: 3837 2020 2030 2e37 3834 3132 0a0a 6060  87   0.78412..``
-00003730: 600a 0a23 2320 4f6e 6c69 6e65 2044 6f63  `..## Online Doc
-00003740: 756d 656e 7461 7469 6f6e 0a5b 5468 6520  umentation.[The 
-00003750: 6f6e 6c69 6e65 2064 6f63 756d 656e 7461  online documenta
-00003760: 7469 6f6e 5d28 6874 7470 733a 2f2f 4a61  tion](https://Ja
-00003770: 636b 736f 6e42 7572 6e73 2e67 6974 6875  cksonBurns.githu
-00003780: 622e 696f 2f61 7374 6172 7465 732f 2920  b.io/astartes/) 
-00003790: 636f 6e74 6169 6e73 2065 7665 7279 7468  contains everyth
-000037a0: 696e 6720 796f 7520 7365 6520 696e 2074  ing you see in t
-000037b0: 6869 7320 5245 4144 4d45 2077 6974 6820  his README with 
-000037c0: 616e 2061 6464 6974 696f 6e61 6c20 7475  an additional tu
-000037d0: 746f 7269 616c 2066 6f72 205b 6d6f 7669  torial for [movi
-000037e0: 6e67 2066 726f 6d20 6074 7261 696e 5f74  ng from `train_t
-000037f0: 6573 745f 7370 6c69 7460 2069 6e20 6073  est_split` in `s
-00003800: 6b6c 6561 726e 6020 746f 2060 6173 7461  klearn` to `asta
-00003810: 7274 6573 605d 2868 7474 7073 3a2f 2f6a  rtes`](https://j
-00003820: 6163 6b73 6f6e 6275 726e 732e 6769 7468  acksonburns.gith
-00003830: 7562 2e69 6f2f 6173 7461 7274 6573 2f73  ub.io/astartes/s
-00003840: 6b6c 6561 726e 5f74 6f5f 6173 7461 7274  klearn_to_astart
-00003850: 6573 2e68 746d 6c29 2e0a 0a23 2320 486f  es.html)...## Ho
-00003860: 7720 746f 2043 6974 650a 4966 2079 6f75  w to Cite.If you
-00003870: 2075 7365 2060 6173 7461 7274 6573 6020   use `astartes` 
-00003880: 696e 2079 6f75 7220 776f 726b 2070 6c65  in your work ple
-00003890: 6173 6520 7573 6520 7468 6520 6265 6c6f  ase use the belo
-000038a0: 7720 6369 7461 7469 6f6e 206f 7220 7468  w citation or th
-000038b0: 6520 2243 6974 6520 7468 6973 2072 6570  e "Cite this rep
-000038c0: 6f73 6974 6f72 7922 2062 7574 746f 6e20  ository" button 
-000038d0: 6f6e 2047 6974 4875 623a 0a3e 202a 2a42  on GitHub:.> **B
-000038e0: 6962 5465 582a 2a0a 3e20 4073 6f66 7477  ibTeX**.> @softw
-000038f0: 6172 657b 4275 726e 735f 6173 7461 7274  are{Burns_astart
-00003900: 6573 2c0a 3e20 2020 6175 7468 6f72 203d  es,.>   author =
-00003910: 207b 4275 726e 732c 204a 6163 6b73 6f6e   {Burns, Jackson
-00003920: 2061 6e64 2053 7069 656b 6572 6d61 6e6e   and Spiekermann
-00003930: 2c20 4b65 7669 6e20 616e 6420 4268 6174  , Kevin and Bhat
-00003940: 7461 6368 6172 6a65 652c 2048 696d 6167  tacharjee, Himag
-00003950: 686e 6120 616e 6420 566c 6163 686f 732c  hna and Vlachos,
-00003960: 2044 696f 6e69 7369 6f73 2061 6e64 2047   Dionisios and G
-00003970: 7265 656e 2c20 5769 6c6c 6961 6d7d 2c0a  reen, William},.
-00003980: 3e20 2020 6c69 6365 6e73 6520 3d20 7b4d  >   license = {M
-00003990: 4954 7d2c 0a3e 2020 2074 6974 6c65 203d  IT},.>   title =
-000039a0: 207b 7b61 7374 6172 7465 737d 7d2c 0a3e   {{astartes}},.>
-000039b0: 2020 2075 726c 203d 207b 6874 7470 733a     url = {https:
-000039c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4a 6163  //github.com/Jac
-000039d0: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
-000039e0: 6573 7d0a 3e20 7d0a 0a3e 202a 2a41 5041  es}.> }..> **APA
-000039f0: 2a2a 0a3e 2042 7572 6e73 2c20 4a2e 2c20  **.> Burns, J., 
-00003a00: 5370 6965 6b65 726d 616e 6e2c 204b 2e2c  Spiekermann, K.,
-00003a10: 2042 6861 7474 6163 6861 726a 6565 2c20   Bhattacharjee, 
-00003a20: 482e 2c20 566c 6163 686f 732c 2044 2e2c  H., Vlachos, D.,
-00003a30: 2026 2047 7265 656e 2c20 572e 2061 7374   & Green, W. ast
-00003a40: 6172 7465 7320 5b43 6f6d 7075 7465 7220  artes [Computer 
-00003a50: 736f 6674 7761 7265 5d2e 2068 7474 7073  software]. https
-00003a60: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00003a70: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-00003a80: 7465 730a 0a0a 2323 2043 6f6e 7472 6962  tes...## Contrib
-00003a90: 7574 696e 6720 2620 4465 7665 6c6f 7065  uting & Develope
-00003aa0: 7220 4e6f 7465 730a 5075 6c6c 2052 6571  r Notes.Pull Req
-00003ab0: 7565 7374 732c 2042 7567 2052 6570 6f72  uests, Bug Repor
-00003ac0: 7473 2c20 616e 6420 616c 6c20 436f 6e74  ts, and all Cont
-00003ad0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
-00003ae0: 6c63 6f6d 6521 2050 6c65 6173 6520 7573  lcome! Please us
-00003af0: 6520 7468 6520 6170 7072 6f70 7269 6174  e the appropriat
-00003b00: 6520 6973 7375 6520 6f72 2070 756c 6c20  e issue or pull 
-00003b10: 7265 7175 6573 7420 7465 6d70 6c61 7465  request template
-00003b20: 2077 6865 6e20 6d61 6b69 6e67 2061 2063   when making a c
-00003b30: 6f6e 7472 6962 7574 696f 6e2e 0a0a 5765  ontribution...We
-00003b40: 206d 616b 6520 7573 6520 6f66 205b 7468   make use of [th
-00003b50: 6520 4769 7448 7562 2044 6973 6375 7373  e GitHub Discuss
-00003b60: 696f 6e73 2070 6167 655d 2868 7474 7073  ions page](https
-00003b70: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00003b80: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-00003b90: 7465 732f 6469 7363 7573 7369 6f6e 7329  tes/discussions)
-00003ba0: 2074 6f20 676f 206f 7665 7220 706f 7465   to go over pote
-00003bb0: 6e74 6961 6c20 6665 6174 7572 6573 2074  ntial features t
-00003bc0: 6f20 6164 642e 2050 6c65 6173 6520 6665  o add. Please fe
-00003bd0: 656c 2066 7265 6520 746f 2073 746f 7020  el free to stop 
-00003be0: 6279 2069 6620 796f 7520 6172 6520 6c6f  by if you are lo
-00003bf0: 6f6b 696e 6720 666f 7220 736f 6d65 7468  oking for someth
-00003c00: 696e 6720 746f 2064 6576 656c 6f70 206f  ing to develop o
-00003c10: 7220 6861 7665 2061 6e20 6964 6561 2066  r have an idea f
-00003c20: 6f72 2061 2075 7365 6675 6c20 6665 6174  or a useful feat
-00003c30: 7572 6521 0a0a 5768 656e 2073 7562 6d69  ure!..When submi
-00003c40: 7474 696e 6720 6120 5052 2c20 706c 6561  tting a PR, plea
-00003c50: 7365 206d 6172 6b20 796f 7572 2050 5220  se mark your PR 
-00003c60: 7769 7468 2074 6865 2022 5052 2052 6561  with the "PR Rea
-00003c70: 6479 2066 6f72 2052 6576 6965 7722 206c  dy for Review" l
-00003c80: 6162 656c 2077 6865 6e20 796f 7520 6172  abel when you ar
-00003c90: 6520 6669 6e69 7368 6564 206d 616b 696e  e finished makin
-00003ca0: 6720 6368 616e 6765 7320 736f 2074 6861  g changes so tha
-00003cb0: 7420 7468 6520 4769 7448 7562 2061 6374  t the GitHub act
-00003cc0: 696f 6e73 2062 6f74 7320 6361 6e20 776f  ions bots can wo
-00003cd0: 726b 2074 6865 6972 206d 6167 6963 210a  rk their magic!.
-00003ce0: 0a23 2323 2044 6576 656c 6f70 6572 2049  .### Developer I
-00003cf0: 6e73 7461 6c6c 0a0a 546f 2063 6f6e 7472  nstall..To contr
-00003d00: 6962 7574 6520 746f 2074 6865 2060 6173  ibute to the `as
-00003d10: 7461 7274 6573 6020 736f 7572 6365 2063  tartes` source c
-00003d20: 6f64 652c 2073 7461 7274 2062 7920 636c  ode, start by cl
-00003d30: 6f6e 696e 6720 7468 6520 7265 706f 7369  oning the reposi
-00003d40: 746f 7279 2028 692e 652e 2060 6769 7420  tory (i.e. `git 
-00003d50: 636c 6f6e 6520 6769 7440 6769 7468 7562  clone git@github
-00003d60: 2e63 6f6d 3a4a 6163 6b73 6f6e 4275 726e  .com:JacksonBurn
-00003d70: 732f 6173 7461 7274 6573 2e67 6974 6029  s/astartes.git`)
-00003d80: 2061 6e64 2074 6865 6e20 696e 7369 6465   and then inside
-00003d90: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00003da0: 7275 6e20 6070 6970 2069 6e73 7461 6c6c  run `pip install
-00003db0: 202d 6520 2e5b 6d6f 6c65 6375 6c65 732c   -e .[molecules,
-00003dc0: 6465 765d 602e 2054 6869 7320 7769 6c6c  dev]`. This will
-00003dd0: 2073 6574 2079 6f75 2075 7020 7769 7468   set you up with
-00003de0: 2061 6c6c 2074 6865 2072 6571 7569 7265   all the require
-00003df0: 6420 6465 7065 6e64 656e 6369 6573 2074  d dependencies t
-00003e00: 6f20 7275 6e20 6061 7374 6172 7465 7360  o run `astartes`
-00003e10: 2061 6e64 2063 6f6e 666f 726d 2074 6f20   and conform to 
-00003e20: 6f75 7220 666f 726d 6174 7469 6e67 2073  our formatting s
-00003e30: 7461 6e64 6172 6473 2028 6062 6c61 636b  tandards (`black
-00003e40: 6020 616e 6420 6069 736f 7274 6029 2c20  ` and `isort`), 
-00003e50: 7768 6963 6820 796f 7520 6361 6e20 636f  which you can co
-00003e60: 6e66 6967 7572 6520 746f 2072 756e 2061  nfigure to run a
-00003e70: 7574 6f6d 6174 6963 616c 6c79 2069 6e20  utomatically in 
-00003e80: 7673 636f 6465 205b 6c69 6b65 2074 6869  vscode [like thi
-00003e90: 735d 2868 7474 7073 3a2f 2f6d 6172 636f  s](https://marco
-00003ea0: 6265 6c6f 2e6d 6564 6975 6d2e 636f 6d2f  belo.medium.com/
-00003eb0: 7365 7474 696e 672d 7570 2d70 7974 686f  setting-up-pytho
-00003ec0: 6e2d 626c 6163 6b2d 6f6e 2d76 6973 7561  n-black-on-visua
-00003ed0: 6c2d 7374 7564 696f 2d63 6f64 652d 3533  l-studio-code-53
-00003ee0: 3138 6562 6134 6364 3030 233a 7e3a 7465  18eba4cd00#:~:te
-00003ef0: 7874 3d47 6f25 3230 746f 2532 3073 6574  xt=Go%20to%20set
-00003f00: 7469 6e67 7325 3230 696e 2532 3079 6f75  tings%20in%20you
-00003f10: 722c 2545 3225 3830 2539 4425 3230 616e  r,%E2%80%9D%20an
-00003f20: 6425 3230 7365 6c65 6374 2532 3025 4532  d%20select%20%E2
-00003f30: 2538 3025 3943 626c 6163 6b25 4532 2538  %80%9Cblack%E2%8
-00003f40: 3025 3944 2e29 2e0a 0a3e 202a 2a4e 6f74  0%9D.)...> **Not
-00003f50: 652a 2a0a 3e20 5769 6e64 6f77 7320 506f  e**.> Windows Po
-00003f60: 7765 7273 6865 6c6c 2061 6e64 204d 6163  wershell and Mac
-00003f70: 4f53 2043 6174 616c 696e 6120 6f72 206e  OS Catalina or n
-00003f80: 6577 6572 206d 6179 2063 6f6d 706c 6169  ewer may complai
-00003f90: 6e20 6162 6f75 7420 7371 7561 7265 2062  n about square b
-00003fa0: 7261 636b 6574 732c 2073 6f20 796f 7520  rackets, so you 
-00003fb0: 7769 6c6c 206e 6565 6420 746f 2064 6f75  will need to dou
-00003fc0: 626c 6520 7175 6f74 6520 7468 6520 606d  ble quote the `m
-00003fd0: 6f6c 6563 756c 6573 6020 636f 6d6d 616e  olecules` comman
-00003fe0: 6420 2869 2e65 2e20 6070 6970 2069 6e73  d (i.e. `pip ins
-00003ff0: 7461 6c6c 2022 6173 7461 7274 6573 5b6d  tall "astartes[m
-00004000: 6f6c 6563 756c 6573 2c64 6576 5d22 6029  olecules,dev]"`)
-00004010: 0a0a 2323 2320 556e 6974 2054 6573 7469  ..### Unit Testi
-00004020: 6e67 0a41 6c6c 206f 6620 7468 6520 7465  ng.All of the te
-00004030: 7374 7320 696e 2060 6173 7461 7274 6573  sts in `astartes
-00004040: 6020 6172 6520 7772 6974 7465 6e20 7573  ` are written us
-00004050: 696e 6720 7468 6520 6275 696c 742d 696e  ing the built-in
-00004060: 2070 7974 686f 6e20 6075 6e69 7474 6573   python `unittes
-00004070: 7460 206d 6f64 756c 6520 2874 6f20 616c  t` module (to al
-00004080: 6c6f 7720 7275 6e6e 696e 6720 7769 7468  low running with
-00004090: 6f75 7420 6070 7974 6573 7460 2920 6275  out `pytest`) bu
-000040a0: 7420 7765 205f 6869 6768 6c79 5f20 7265  t we _highly_ re
-000040b0: 636f 6d6d 656e 6420 7573 696e 6720 6070  commend using `p
-000040c0: 7974 6573 7460 2e20 546f 2065 7865 6375  ytest`. To execu
-000040d0: 7465 2074 6865 2074 6573 7473 2066 726f  te the tests fro
-000040e0: 6d20 7468 6520 6061 7374 6172 7465 7360  m the `astartes`
-000040f0: 2072 6570 6f73 6974 6f72 792c 2073 696d   repository, sim
-00004100: 706c 7920 7479 7065 2060 7079 7465 7374  ply type `pytest
-00004110: 6020 6166 7465 7220 7275 6e6e 696e 6720  ` after running 
-00004120: 7468 6520 6465 7665 6c6f 7065 7220 696e  the developer in
-00004130: 7374 616c 6c20 286f 7220 616c 7465 726e  stall (or altern
-00004140: 6174 656c 792c 2060 7079 7465 7374 202d  ately, `pytest -
-00004150: 7660 2066 6f72 2061 206d 6f72 6520 6865  v` for a more he
-00004160: 6c70 6675 6c20 6f75 7470 7574 292e 0a0a  lpful output)...
-00004170: 2323 2320 4164 6469 6e67 204e 6577 2053  ### Adding New S
-00004180: 616d 706c 6572 730a 4164 6469 6e67 2061  amplers.Adding a
-00004190: 206e 6577 2073 616d 706c 6572 2073 686f   new sampler sho
-000041a0: 756c 6420 6578 7465 6e64 2074 6865 2060  uld extend the `
-000041b0: 6162 7374 7261 6374 5f73 616d 706c 6572  abstract_sampler
-000041c0: 2e70 7960 2061 6273 7472 6163 7420 6261  .py` abstract ba
-000041d0: 7365 2063 6c61 7373 2e0a 0a49 7420 6361  se class...It ca
-000041e0: 6e20 6265 2061 7320 7369 6d70 6c65 2061  n be as simple a
-000041f0: 7320 6120 7061 7373 7468 726f 7567 6820  s a passthrough 
-00004200: 746f 2061 2061 6e6f 7468 6572 2060 7472  to a another `tr
-00004210: 6169 6e5f 7465 7374 5f73 706c 6974 602c  ain_test_split`,
-00004220: 206f 7220 6974 2063 616e 2062 6520 616e   or it can be an
-00004230: 206f 7269 6769 6e61 6c20 696d 706c 656d   original implem
-00004240: 656e 7461 7469 6f6e 2074 6861 7420 7265  entation that re
-00004250: 7375 6c74 7320 696e 2058 2061 6e64 2079  sults in X and y
-00004260: 2062 6569 6e67 2073 706c 6974 2069 6e74   being split int
-00004270: 6f20 7477 6f20 6c69 7374 732e 2054 616b  o two lists. Tak
-00004280: 6520 6120 6c6f 6f6b 2061 7420 6061 7374  e a look at `ast
-00004290: 6172 7465 732f 7361 6d70 6c65 7273 2f72  artes/samplers/r
-000042a0: 616e 646f 6d5f 7370 6c69 742e 7079 6020  andom_split.py` 
-000042b0: 666f 7220 6120 6261 7369 6320 6578 616d  for a basic exam
-000042c0: 706c 6521 0a0a 4166 7465 7220 7468 6520  ple!..After the 
-000042d0: 7361 6d70 6c65 7220 6861 7320 6265 656e  sampler has been
-000042e0: 2069 6d70 6c65 6d65 6e74 6564 2c20 6164   implemented, ad
-000042f0: 6420 6974 2074 6f20 605f 5f69 6e69 745f  d it to `__init_
-00004300: 5f2e 7079 6020 696e 2069 6e20 6061 7374  _.py` in in `ast
-00004310: 6172 7465 732f 7361 6d70 6c65 7273 6020  artes/samplers` 
-00004320: 616e 6420 6974 2077 696c 6c20 6175 746f  and it will auto
-00004330: 6d61 7469 6361 6c6c 7920 6265 2075 6e69  matically be uni
-00004340: 7420 7465 7374 6564 2e20 4164 6469 7469  t tested. Additi
-00004350: 6f6e 616c 2075 6e69 7420 7465 7374 7320  onal unit tests 
-00004360: 746f 2076 6572 6966 7920 7468 6174 2068  to verify that h
-00004370: 7970 6572 7061 7261 6d65 7465 7273 2063  yperparameters c
-00004380: 616e 2062 6520 7072 6f70 6572 6c79 2070  an be properly p
-00004390: 6173 7365 642c 2065 7463 2e20 6172 6520  assed, etc. are 
-000043a0: 616c 736f 2072 6563 6f6d 6d65 6e64 6564  also recommended
-000043b0: 2e0a 0a46 6f72 2068 6973 746f 7269 6361  ...For historica
-000043c0: 6c20 7265 6173 6f6e 732c 2061 6e64 2061  l reasons, and a
-000043d0: 7320 6120 6775 6964 6520 666f 7220 616e  s a guide for an
-000043e0: 7920 6465 7665 6c6f 7065 7273 2077 686f  y developers who
-000043f0: 2077 6f75 6c64 206c 696b 6520 6164 6420   would like add 
-00004400: 6e65 7720 7361 6d70 6c65 7273 2c20 6265  new samplers, be
-00004410: 6c6f 7720 6973 2061 2072 756e 6e69 6e67  low is a running
-00004420: 206c 6973 7420 6f66 2073 616d 706c 6572   list of sampler
-00004430: 7320 7768 6963 6820 6861 7665 2062 6565  s which have bee
-00004440: 6e20 5f63 6f6e 7369 6465 7265 645f 2066  n _considered_ f
-00004450: 6f72 2061 6464 6974 696f 6e20 746f 2060  or addition to `
-00004460: 6173 6172 7465 7360 2062 7574 2075 6c74  asartes` but ult
-00004470: 696d 6174 656c 7920 6e6f 7420 6164 6465  imately not adde
-00004480: 6420 666f 7220 7661 7269 6f75 7320 7265  d for various re
-00004490: 6173 6f6e 732e 0a0a 2323 2323 204e 6f74  asons...#### Not
-000044a0: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
-000044b0: 706c 696e 6720 416c 676f 7269 7468 6d73  pling Algorithms
-000044c0: 0a0a 7c20 5361 6d70 6c65 7220 4e61 6d65  ..| Sampler Name
-000044d0: 207c 2052 6561 736f 6e69 6e67 207c 2052   | Reasoning | R
-000044e0: 656c 6576 616e 7420 4c69 6e6b 2873 2920  elevant Link(s) 
-000044f0: 7c0a 7c3a 2d2d 2d3a 7c2d 2d2d 7c2d 2d2d  |.|:---:|---|---
-00004500: 7c0a 7c20 442d 4f70 7469 6d61 6c20 7c20  |.| D-Optimal | 
-00004510: 5265 7175 6972 6573 205f 612d 7072 696f  Requires _a-prio
-00004520: 7269 5f20 6b6e 6f77 6c65 6467 6520 6f66  ri_ knowledge of
-00004530: 2074 6865 2074 6573 7420 616e 6420 7472   the test and tr
-00004540: 6169 6e20 7369 7a65 2077 6869 6368 2064  ain size which d
-00004550: 6f65 7320 6e6f 7420 6669 7420 696e 2074  oes not fit in t
-00004560: 6865 2060 6173 7461 7274 6573 6020 6672  he `astartes` fr
-00004570: 616d 6577 6f72 6b20 2873 616d 706c 6572  amework (sampler
-00004580: 7320 6172 6520 616c 6c20 6167 6e6f 7374  s are all agnost
-00004590: 6963 2074 6f20 7468 6520 7369 7a65 206f  ic to the size o
-000045a0: 6620 7468 6520 7365 7473 2920 616e 6420  f the sets) and 
-000045b0: 6974 2069 7320 7175 6573 7469 6f6e 6162  it is questionab
-000045c0: 6c65 2069 6620 7468 6520 7573 6520 6f66  le if the use of
-000045d0: 2074 6865 2046 6973 6368 6572 2069 6e66   the Fischer inf
-000045e0: 6f72 6d61 7469 6f6e 206d 6174 7269 7820  ormation matrix 
-000045f0: 6973 2061 6374 7561 6c6c 7920 6d65 616e  is actually mean
-00004600: 696e 6766 756c 2069 6e20 7468 6520 636f  ingful in the co
-00004610: 6e74 6578 7420 6f66 2073 616d 706c 696e  ntext of samplin
-00004620: 6720 6578 6973 7469 6e67 2064 6174 6120  g existing data 
-00004630: 7261 7468 6572 2074 6861 6e20 7475 6e69  rather than tuni
-00004640: 6e67 2066 6f72 2069 6465 616c 2064 6174  ng for ideal dat
-00004650: 612e 207c 2054 6865 205b 5769 6b69 7065  a. | The [Wikipe
-00004660: 6469 6120 6172 7469 636c 6520 666f 7220  dia article for 
-00004670: 6f70 7469 6d61 6c20 6465 7369 676e 5d28  optimal design](
-00004680: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00004690: 6564 6961 2e6f 7267 2f77 696b 692f 4f70  edia.org/wiki/Op
-000046a0: 7469 6d61 6c5f 6465 7369 676e 233a 7e3a  timal_design#:~:
-000046b0: 7465 7874 3d4f 6625 3230 636f 7572 7365  text=Of%20course
-000046c0: 2532 4325 3230 6669 7869 6e67 2532 3074  %2C%20fixing%20t
-000046d0: 6865 2532 306e 756d 6265 7225 3230 6f66  he%20number%20of
-000046e0: 2532 3065 7870 6572 696d 656e 7461 6c25  %20experimental%
-000046f0: 3230 7275 6e73 2532 3061 2532 3070 7269  20runs%20a%20pri
-00004700: 6f72 6925 3230 776f 756c 6425 3230 6265  ori%20would%20be
-00004710: 2532 3069 6d70 7261 6374 6963 616c 2e29  %20impractical.)
-00004720: 2064 6f65 7320 6120 676f 6f64 206a 6f62   does a good job
-00004730: 2065 7870 6c61 696e 696e 6720 7768 7920   explaining why 
-00004740: 7468 6973 2069 7320 6469 6666 6963 756c  this is difficul
-00004750: 742c 2061 6e64 2070 6f69 6e74 7320 6174  t, and points at
-00004760: 2073 6f6d 6520 706f 7465 6e74 6961 6c20   some potential 
-00004770: 616c 7465 726e 6174 6976 6573 2e20 7c0a  alternatives. |.
-00004780: 7c20 4475 706c 6578 207c 2052 6571 7569  | Duplex | Requi
-00004790: 7265 7320 6b6e 6f77 696e 6720 7465 7374  res knowing test
-000047a0: 2061 6e64 2074 7261 696e 2073 697a 6520   and train size 
-000047b0: 6265 666f 7265 2065 7865 6375 7469 6f6e  before execution
-000047c0: 2c20 616e 6420 6361 6e20 6f6e 6c79 2070  , and can only p
-000047d0: 6172 7469 7469 6f6e 2064 6174 6120 696e  artition data in
-000047e0: 746f 2074 776f 2073 6574 7320 7768 6963  to two sets whic
-000047f0: 6820 776f 756c 6420 6d61 6b65 2069 7420  h would make it 
-00004800: 696e 636f 6d70 6174 6962 6c65 2077 6974  incompatible wit
-00004810: 6820 6074 7261 696e 5f76 616c 5f74 6573  h `train_val_tes
-00004820: 745f 7370 6c69 7460 2e20 7c20 5468 6973  t_split`. | This
-00004830: 205b 696d 706c 656d 656e 7461 7469 6f6e   [implementation
-00004840: 2069 6e20 525d 2868 7474 7073 3a2f 2f73   in R](https://s
-00004850: 6561 7263 682e 722d 7072 6f6a 6563 742e  earch.r-project.
-00004860: 6f72 672f 4352 414e 2f72 6566 6d61 6e73  org/CRAN/refmans
-00004870: 2f70 726f 7370 6563 7472 2f68 746d 6c2f  /prospectr/html/
-00004880: 6475 706c 6578 2e68 746d 6c23 3a7e 3a74  duplex.html#:~:t
-00004890: 6578 743d 5468 6525 3230 4455 504c 4558  ext=The%20DUPLEX
-000048a0: 2532 3061 6c67 6f72 6974 686d 2532 3069  %20algorithm%20i
-000048b0: 7325 3230 7369 6d69 6c61 722c 7468 6174  s%20similar,that
-000048c0: 2532 3061 7265 2532 3074 6865 2532 3066  %20are%20the%20f
-000048d0: 6172 7468 6573 7425 3230 6170 6172 742e  arthest%20apart.
-000048e0: 2920 696e 636c 7564 6573 2068 656c 7066  ) includes helpf
-000048f0: 756c 2072 6566 6572 656e 6365 7320 616e  ul references an
-00004900: 6420 6120 7265 6665 7265 6e63 6520 696d  d a reference im
-00004910: 706c 656d 656e 7461 7469 6f6e 2e20 7c0a  plementation. |.
-00004920: 0a23 2323 2041 6464 696e 6720 4e65 7720  .### Adding New 
-00004930: 4665 6174 7572 697a 6174 696f 6e20 5363  Featurization Sc
-00004940: 6865 6d65 730a 416c 6c20 6f66 2074 6865  hemes.All of the
-00004950: 2073 616d 706c 696e 6720 6d65 7468 6f64   sampling method
-00004960: 7320 696d 706c 656d 656e 7465 6420 696e  s implemented in
-00004970: 2060 6173 7461 7274 6573 6020 6163 6365   `astartes` acce
-00004980: 7074 2061 7262 6974 7261 7279 2061 7272  pt arbitrary arr
-00004990: 6179 7320 6f66 206e 756d 6265 7273 2061  ays of numbers a
-000049a0: 6e64 2072 6574 7572 6e20 7468 6520 7361  nd return the sa
-000049b0: 6d70 6c65 6420 6772 6f75 7073 2028 7769  mpled groups (wi
-000049c0: 7468 2074 6865 2065 7863 6570 7469 6f6e  th the exception
-000049d0: 206f 6620 6053 6361 6666 6f6c 642e 7079   of `Scaffold.py
-000049e0: 6029 2e20 4966 2079 6f75 2068 6176 6520  `). If you have 
-000049f0: 616e 2065 7869 7374 696e 6720 6665 6174  an existing feat
-00004a00: 7572 697a 6174 696f 6e20 7363 6865 6d65  urization scheme
-00004a10: 2028 692e 652e 2074 616b 6520 616e 2061   (i.e. take an a
-00004a20: 7262 6974 7261 7279 2069 6e70 7574 2061  rbitrary input a
-00004a30: 6e64 2074 7572 6e20 6974 2069 6e74 6f20  nd turn it into 
-00004a40: 616e 2061 7272 6179 206f 6620 6e75 6d62  an array of numb
-00004a50: 6572 7329 2c20 7765 2077 6f75 6c64 2062  ers), we would b
-00004a60: 6520 7468 7269 6c6c 6564 2074 6f20 696e  e thrilled to in
-00004a70: 636c 7564 6520 6974 2069 6e20 6061 7374  clude it in `ast
-00004a80: 6172 7465 7360 2e0a 0a41 6464 696e 6720  artes`...Adding 
-00004a90: 6120 6e65 7720 696e 7465 7266 6163 6520  a new interface 
-00004aa0: 7368 6f75 6c64 2074 616b 6520 6f6e 2074  should take on t
-00004ab0: 6869 7320 666f 726d 6174 3a0a 0a60 6060  his format:..```
-00004ac0: 7079 7468 6f6e 0a66 726f 6d20 6173 7461  python.from asta
-00004ad0: 7274 6573 2069 6d70 6f72 7420 7472 6169  rtes import trai
-00004ae0: 6e5f 7465 7374 5f73 706c 6974 0a0a 6465  n_test_split..de
-00004af0: 6620 7472 6169 6e5f 7465 7374 5f73 706c  f train_test_spl
-00004b00: 6974 5f49 4e54 4552 4641 4345 280a 2020  it_INTERFACE(.  
-00004b10: 2020 494e 5445 5246 4143 455f 696e 7075    INTERFACE_inpu
-00004b20: 742c 0a20 2020 2049 4e54 4552 4641 4345  t,.    INTERFACE
-00004b30: 5f41 5247 532c 0a20 2020 2079 3a20 6e70  _ARGS,.    y: np
-00004b40: 2e61 7272 6179 203d 204e 6f6e 652c 0a20  .array = None,. 
-00004b50: 2020 206c 6162 656c 733a 206e 702e 6172     labels: np.ar
-00004b60: 7261 7920 3d20 4e6f 6e65 2c0a 2020 2020  ray = None,.    
-00004b70: 7465 7374 5f73 697a 653a 2066 6c6f 6174  test_size: float
-00004b80: 203d 2030 2e32 352c 0a20 2020 2074 7261   = 0.25,.    tra
-00004b90: 696e 5f73 697a 653a 2066 6c6f 6174 203d  in_size: float =
-00004ba0: 2030 2e37 352c 0a20 2020 2073 706c 6974   0.75,.    split
-00004bb0: 7465 723a 2073 7472 203d 2027 7261 6e64  ter: str = 'rand
-00004bc0: 6f6d 272c 0a20 2020 2068 6f70 7473 3a20  om',.    hopts: 
-00004bd0: 6469 6374 203d 207b 7d2c 0a20 2020 2049  dict = {},.    I
-00004be0: 4e54 4552 4641 4345 5f68 6f70 7473 3a20  NTERFACE_hopts: 
-00004bf0: 6469 6374 203d 207b 7d2c 0a29 3a0a 2020  dict = {},.):.  
-00004c00: 2020 2320 7475 726e 2074 6865 2049 4e54    # turn the INT
-00004c10: 4552 4641 4345 5f69 6e70 7574 2069 6e74  ERFACE_input int
-00004c20: 6f20 616e 2069 6e70 7574 2058 0a20 2020  o an input X.   
-00004c30: 2023 2062 6173 6564 206f 6e20 494e 5445   # based on INTE
-00004c40: 5246 4143 4520 4152 4753 2077 6865 7265  RFACE ARGS where
-00004c50: 2049 4e54 4552 4641 4345 5f68 6f70 7473   INTERFACE_hopts
-00004c60: 0a20 2020 2023 2073 7065 6369 6669 6573  .    # specifies
-00004c70: 2061 6464 6974 696f 6e61 6c20 6265 6861   additional beha
-00004c80: 7669 6f72 0a20 2020 2058 203d 205b 5d0a  vior.    X = [].
-00004c90: 2020 2020 0a20 2020 2023 2063 616c 6c20      .    # call 
-00004ca0: 7472 6169 6e20 7465 7374 2073 706c 6974  train test split
-00004cb0: 2077 6974 6820 7468 6973 2069 6e70 7574   with this input
-00004cc0: 0a20 2020 2072 6574 7572 6e20 7472 6169  .    return trai
-00004cd0: 6e5f 7465 7374 5f73 706c 6974 280a 2020  n_test_split(.  
-00004ce0: 2020 2020 2020 582c 0a20 2020 2020 2020        X,.       
-00004cf0: 2079 3d79 2c0a 2020 2020 2020 2020 6c61   y=y,.        la
-00004d00: 6265 6c73 3d6c 6162 656c 732c 0a20 2020  bels=labels,.   
-00004d10: 2020 2020 2074 6573 745f 7369 7a65 3d74       test_size=t
-00004d20: 6573 745f 7369 7a65 2c0a 2020 2020 2020  est_size,.      
-00004d30: 2020 7472 6169 6e5f 7369 7a65 3d74 7261    train_size=tra
-00004d40: 696e 5f73 697a 652c 0a20 2020 2020 2020  in_size,.       
-00004d50: 2073 706c 6974 7465 723d 7370 6c69 7474   splitter=splitt
-00004d60: 6572 2c0a 2020 2020 2020 2020 686f 7074  er,.        hopt
-00004d70: 733d 686f 7074 732c 0a20 2020 2029 0a60  s=hopts,.    ).`
-00004d80: 6060 0a0a 4966 2070 6f73 7369 626c 652c  ``..If possible,
-00004d90: 2077 6520 776f 756c 6420 6c69 6b65 2074   we would like t
-00004da0: 6f20 616c 736f 2061 6464 2061 6e20 6578  o also add an ex
-00004db0: 616d 706c 6520 4a75 7079 7465 7220 4e6f  ample Jupyter No
-00004dc0: 7465 626f 6f6b 2077 6974 6820 616e 7920  tebook with any 
-00004dd0: 6e65 7720 696e 7465 7266 6163 6520 746f  new interface to
-00004de0: 2064 656d 6f6e 7374 7261 7465 2074 6f20   demonstrate to 
-00004df0: 6e65 7720 7573 6572 7320 686f 7720 6974  new users how it
-00004e00: 2066 756e 6374 696f 6e73 2e20 5365 6520   functions. See 
-00004e10: 6f75 7220 6f74 6865 7220 6578 616d 706c  our other exampl
-00004e20: 6573 2069 6e20 7468 6520 6065 7861 6d70  es in the `examp
-00004e30: 6c65 7360 2064 6972 6563 746f 7279 2e0a  les` directory..
-00004e40: 0a43 6f6e 7461 6374 205b 404a 6163 6b73  .Contact [@Jacks
-00004e50: 6f6e 4275 726e 735d 2868 7474 7073 3a2f  onBurns](https:/
-00004e60: 2f67 6974 6875 622e 636f 6d2f 4a61 636b  /github.com/Jack
-00004e70: 736f 6e42 7572 6e73 2920 6966 2079 6f75  sonBurns) if you
-00004e80: 206e 6565 6420 6173 7369 7374 616e 6365   need assistance
-00004e90: 2061 6464 696e 6720 616e 2065 7869 7374   adding an exist
-00004ea0: 696e 6720 776f 726b 666c 6f77 2074 6f20  ing workflow to 
-00004eb0: 6061 7374 6172 7465 7360 2e20 4966 2074  `astartes`. If t
-00004ec0: 6869 7320 6665 6174 7572 697a 6174 696f  his featurizatio
-00004ed0: 6e20 7363 6865 6d65 2072 6571 7569 7265  n scheme require
-00004ee0: 7320 6164 6469 7469 6f6e 616c 2064 6570  s additional dep
-00004ef0: 656e 6465 6e63 6965 7320 746f 2066 756e  endencies to fun
-00004f00: 6374 696f 6e2c 2077 6520 6d61 7920 6164  ction, we may ad
-00004f10: 6420 6974 2061 7320 616e 2061 6464 6974  d it as an addit
-00004f20: 696f 6e61 6c20 5f65 7874 7261 5f20 7061  ional _extra_ pa
-00004f30: 636b 6167 6520 696e 2074 6865 2073 616d  ckage in the sam
-00004f40: 6520 7761 7920 7468 6174 2060 6d6f 6c65  e way that `mole
-00004f50: 6375 6c65 7360 2069 6e20 696e 7374 616c  cules` in instal
-00004f60: 6c65 642e 0a0a 2323 204a 4f53 5320 4272  led...## JOSS Br
-00004f70: 616e 6368 0a0a 6061 7374 6172 7465 7360  anch..`astartes`
-00004f80: 2063 6f72 7265 7370 6f6e 6469 6e67 204a   corresponding J
-00004f90: 4f53 5320 7061 7065 7220 6973 2073 746f  OSS paper is sto
-00004fa0: 7265 6420 696e 2074 6869 7320 7265 706f  red in this repo
-00004fb0: 7369 746f 7279 206f 6e20 6120 7365 7061  sitory on a sepa
-00004fc0: 7261 7465 2062 7261 6e63 682e 2059 6f75  rate branch. You
-00004fd0: 2063 616e 2066 696e 6420 6070 6170 6572   can find `paper
-00004fe0: 2e6d 6460 206f 6e20 7468 6520 6170 746c  .md` on the aptl
-00004ff0: 7920 6e61 6d65 6420 606a 6f73 732d 7061  y named `joss-pa
-00005000: 7065 7260 2062 7261 6e63 682e 200a 0a5f  per` branch. .._
-00005010: 4e6f 7465 2066 6f72 204d 6169 6e74 6169  Note for Maintai
-00005020: 6e65 7273 5f3a 2054 6f20 7075 7368 2063  ners_: To push c
-00005030: 6861 6e67 6573 2066 726f 6d20 7468 6520  hanges from the 
-00005040: 606d 6169 6e60 2062 7261 6e63 6820 696e  `main` branch in
-00005050: 746f 2074 6865 2060 6a6f 7373 2d70 6170  to the `joss-pap
-00005060: 6572 6020 6272 616e 6368 2c20 7275 6e20  er` branch, run 
-00005070: 7468 6520 6055 7064 6174 6520 4a4f 5353  the `Update JOSS
-00005080: 2042 7261 6e63 6860 2077 6f72 6b66 6c6f   Branch` workflo
-00005090: 772e 0a0a                                w...
+00000760: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000770: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00000780: 2e35 3238 312f 7a65 6e6f 646f 2e38 3134  .5281/zenodo.814
+00000790: 3732 3035 223e 3c69 6d67 2073 7263 3d22  7205"><img src="
+000007a0: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+000007b0: 7267 2f62 6164 6765 2f44 4f49 2f31 302e  rg/badge/DOI/10.
+000007c0: 3532 3831 2f7a 656e 6f64 6f2e 3831 3437  5281/zenodo.8147
+000007d0: 3230 352e 7376 6722 2061 6c74 3d22 444f  205.svg" alt="DO
+000007e0: 4922 3e3c 2f61 3e0a 3c2f 703e 0a0a 2323  I"></a>.</p>..##
+000007f0: 204f 6e6c 696e 6520 446f 6375 6d65 6e74   Online Document
+00000800: 6174 696f 6e0a 466f 6c6c 6f77 205b 7468  ation.Follow [th
+00000810: 6973 206c 696e 6b5d 2868 7474 7073 3a2f  is link](https:/
+00000820: 2f4a 6163 6b73 6f6e 4275 726e 732e 6769  /JacksonBurns.gi
+00000830: 7468 7562 2e69 6f2f 6173 7461 7274 6573  thub.io/astartes
+00000840: 2f29 2066 6f72 2061 206e 6963 656c 792d  /) for a nicely-
+00000850: 7265 6e64 6572 6564 2076 6572 7369 6f6e  rendered version
+00000860: 206f 6620 7468 6973 2052 4541 444d 4520   of this README 
+00000870: 616c 6f6e 6720 7769 7468 2061 6464 6974  along with addit
+00000880: 696f 6e61 6c20 7475 746f 7269 616c 7320  ional tutorials 
+00000890: 666f 7220 5b6d 6f76 696e 6720 6672 6f6d  for [moving from
+000008a0: 2074 7261 696e 5f74 6573 745f 7370 6c69   train_test_spli
+000008b0: 7420 696e 2073 6b6c 6561 726e 2074 6f20  t in sklearn to 
+000008c0: 6173 7461 7274 6573 5d28 6874 7470 733a  astartes](https:
+000008d0: 2f2f 6a61 636b 736f 6e62 7572 6e73 2e67  //jacksonburns.g
+000008e0: 6974 6875 622e 696f 2f61 7374 6172 7465  ithub.io/astarte
+000008f0: 732f 736b 6c65 6172 6e5f 746f 5f61 7374  s/sklearn_to_ast
+00000900: 6172 7465 732e 6874 6d6c 292e 0a4b 6565  artes.html)..Kee
+00000910: 7020 7265 6164 696e 6720 666f 7220 6120  p reading for a 
+00000920: 696e 7374 616c 6c61 7469 6f6e 2067 7569  installation gui
+00000930: 6465 2061 6e64 206c 696e 6b73 2074 6f20  de and links to 
+00000940: 7475 746f 7269 616c 7321 0a0a 2323 2049  tutorials!..## I
+00000950: 6e73 7461 6c6c 696e 6720 6061 7374 6172  nstalling `astar
+00000960: 7465 7360 0a57 6520 7265 636f 6d6d 656e  tes`.We recommen
+00000970: 6420 696e 7374 616c 6c69 6e67 2060 6173  d installing `as
+00000980: 7461 7274 6573 6020 7769 7468 696e 2061  tartes` within a
+00000990: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+000009a0: 6d65 6e74 2c20 7573 696e 6720 6569 7468  ment, using eith
+000009b0: 6572 2060 7665 6e76 6020 6f72 2060 636f  er `venv` or `co
+000009c0: 6e64 6160 2028 6f72 206f 7468 6572 2074  nda` (or other t
+000009d0: 6f6f 6c73 2920 746f 2073 696d 706c 6966  ools) to simplif
+000009e0: 7920 6465 7065 6e64 656e 6379 206d 616e  y dependency man
+000009f0: 6167 656d 656e 742e 2050 7974 686f 6e20  agement. Python 
+00000a00: 7665 7273 696f 6e73 2033 2e37 2c20 332e  versions 3.7, 3.
+00000a10: 382c 2033 2e39 2c20 332e 3130 2c20 616e  8, 3.9, 3.10, an
+00000a20: 6420 332e 3131 2061 7265 2073 7570 706f  d 3.11 are suppo
+00000a30: 7274 6564 206f 6e20 616c 6c20 706c 6174  rted on all plat
+00000a40: 666f 726d 732e 0a0a 6061 7374 6172 7465  forms...`astarte
+00000a50: 7360 2069 7320 6176 6169 6c61 626c 6520  s` is available 
+00000a60: 6f6e 2060 5079 5049 6020 616e 6420 6361  on `PyPI` and ca
+00000a70: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
+00000a80: 7369 6e67 2060 7069 7060 3a0a 0a20 2d20  sing `pip`:.. - 
+00000a90: 546f 2069 6e63 6c75 6465 2074 6865 2066  To include the f
+00000aa0: 6561 7475 7269 7a61 7469 6f6e 206f 7074  eaturization opt
+00000ab0: 696f 6e73 2066 6f72 2063 6865 6d69 6361  ions for chemica
+00000ac0: 6c20 6461 7461 2c20 7573 6520 6070 6970  l data, use `pip
+00000ad0: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
+00000ae0: 735b 6d6f 6c65 6375 6c65 735d 602e 0a20  s[molecules]`.. 
+00000af0: 2d20 546f 2069 6e73 7461 6c6c 206f 6e6c  - To install onl
+00000b00: 7920 7468 6520 7361 6d70 6c69 6e67 2061  y the sampling a
+00000b10: 6c67 6f72 6974 686d 732c 2075 7365 2060  lgorithms, use `
+00000b20: 7069 7020 696e 7374 616c 6c20 6173 7461  pip install asta
+00000b30: 7274 6573 6020 2874 6869 7320 696e 7374  rtes` (this inst
+00000b40: 616c 6c20 7769 6c6c 2068 6176 6520 6665  all will have fe
+00000b50: 7765 7220 6465 7065 6e64 656e 6369 6573  wer dependencies
+00000b60: 2061 6e64 206d 6179 2062 6520 6d6f 7265   and may be more
+00000b70: 2072 6561 6469 6c79 2063 6f6d 7061 7469   readily compati
+00000b80: 626c 6520 696e 2065 6e76 6972 6f6e 6d65  ble in environme
+00000b90: 6e74 7320 7769 7468 2065 7869 7374 696e  nts with existin
+00000ba0: 6720 776f 726b 666c 6f77 7329 2e0a 0a54  g workflows)...T
+00000bb0: 6865 2062 6173 6520 6061 7374 6172 7465  he base `astarte
+00000bc0: 7360 2070 6163 6b61 6765 2069 7320 616c  s` package is al
+00000bd0: 736f 2061 7661 696c 6162 6c65 206f 6e20  so available on 
+00000be0: 6063 6f6e 6461 6020 7769 7468 2074 6869  `conda` with thi
+00000bf0: 7320 636f 6d6d 616e 643a 2060 636f 6e64  s command: `cond
+00000c00: 6120 696e 7374 616c 6c20 2d63 206a 6163  a install -c jac
+00000c10: 6b73 6f6e 6275 726e 7320 6173 7461 7274  ksonburns astart
+00000c20: 6573 602e 0a4e 6f74 6520 7468 6174 2074  es`..Note that t
+00000c30: 6869 7320 7061 636b 6167 6520 5f64 6f65  his package _doe
+00000c40: 7320 6e6f 745f 2069 6e63 6c75 6465 2062  s not_ include b
+00000c50: 7569 6c74 2d69 6e20 7375 7070 6f72 7420  uilt-in support 
+00000c60: 666f 7220 6665 6174 7572 697a 696e 6720  for featurizing 
+00000c70: 6d6f 6c65 6375 6c65 732c 2077 6869 6368  molecules, which
+00000c80: 2069 7320 6375 7272 656e 746c 7920 6f6e   is currently on
+00000c90: 6c79 2061 7661 696c 6162 6c65 2066 726f  ly available fro
+00000ca0: 6d20 7468 6520 5079 5049 2070 6163 6b61  m the PyPI packa
+00000cb0: 6765 206f 7220 6120 736f 7572 6365 2069  ge or a source i
+00000cc0: 6e73 7461 6c6c 2e0a 0a3e 202a 2a4e 6f74  nstall...> **Not
+00000cd0: 652a 2a0a 3e20 5769 6e64 6f77 7320 506f  e**.> Windows Po
+00000ce0: 7765 7273 6865 6c6c 2061 6e64 204d 6163  wershell and Mac
+00000cf0: 4f53 2043 6174 616c 696e 6120 6f72 206e  OS Catalina or n
+00000d00: 6577 6572 206d 6179 2063 6f6d 706c 6169  ewer may complai
+00000d10: 6e20 6162 6f75 7420 7371 7561 7265 2062  n about square b
+00000d20: 7261 636b 6574 732c 2073 6f20 796f 7520  rackets, so you 
+00000d30: 7769 6c6c 206e 6565 6420 746f 2064 6f75  will need to dou
+00000d40: 626c 6520 7175 6f74 6520 7468 6520 606d  ble quote the `m
+00000d50: 6f6c 6563 756c 6573 6020 636f 6d6d 616e  olecules` comman
+00000d60: 6420 2869 2e65 2e20 6070 6970 2069 6e73  d (i.e. `pip ins
+00000d70: 7461 6c6c 2022 6173 7461 7274 6573 5b6d  tall "astartes[m
+00000d80: 6f6c 6563 756c 6573 5d22 6029 0a0a 546f  olecules]"`)..To
+00000d90: 2069 6e73 7461 6c6c 2060 6173 7461 7274   install `astart
+00000da0: 6573 6020 6672 6f6d 2073 6f75 7263 652c  es` from source,
+00000db0: 2073 6565 2074 6865 205b 436f 6e74 7269   see the [Contri
+00000dc0: 6275 7469 6e67 2026 2044 6576 656c 6f70  buting & Develop
+00000dd0: 6572 204e 6f74 6573 5d28 2363 6f6e 7472  er Notes](#contr
+00000de0: 6962 7574 696e 672d 2d64 6576 656c 6f70  ibuting--develop
+00000df0: 6572 2d6e 6f74 6573 2920 7365 6374 696f  er-notes) sectio
+00000e00: 6e2e 0a0a 2323 2051 7569 636b 2053 7461  n...## Quick Sta
+00000e10: 7274 0a60 6173 7461 7274 6573 6020 6973  rt.`astartes` is
+00000e20: 2064 6573 6967 6e65 6420 6173 2061 2064   designed as a d
+00000e30: 726f 702d 696e 2072 6570 6c61 6365 6d65  rop-in replaceme
+00000e40: 6e74 2066 6f72 2060 736b 6c65 6172 6e60  nt for `sklearn`
+00000e50: 2773 2060 7472 6169 6e5f 7465 7374 5f73  's `train_test_s
+00000e60: 706c 6974 6020 6675 6e63 7469 6f6e 2028  plit` function (
+00000e70: 7365 6520 7468 6520 5b73 6b6c 6561 726e  see the [sklearn
+00000e80: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00000e90: 6874 7470 733a 2f2f 7363 696b 6974 2d6c  https://scikit-l
+00000ea0: 6561 726e 2e6f 7267 2f73 7461 626c 652f  earn.org/stable/
+00000eb0: 6d6f 6475 6c65 732f 6765 6e65 7261 7465  modules/generate
+00000ec0: 642f 736b 6c65 6172 6e2e 6d6f 6465 6c5f  d/sklearn.model_
+00000ed0: 7365 6c65 6374 696f 6e2e 7472 6169 6e5f  selection.train_
+00000ee0: 7465 7374 5f73 706c 6974 2e68 746d 6c29  test_split.html)
+00000ef0: 292e 2054 6f20 7377 6974 6368 2074 6f20  ). To switch to 
+00000f00: 6061 7374 6172 7465 7360 2c20 6368 616e  `astartes`, chan
+00000f10: 6765 2060 6672 6f6d 2073 6b6c 6561 726e  ge `from sklearn
+00000f20: 2e6d 6f64 656c 5f73 656c 6563 7469 6f6e  .model_selection
+00000f30: 2069 6d70 6f72 7420 7472 6169 6e5f 7465   import train_te
+00000f40: 7374 5f73 706c 6974 6020 746f 2060 6672  st_split` to `fr
+00000f50: 6f6d 2061 7374 6172 7465 7320 696d 706f  om astartes impo
+00000f60: 7274 2074 7261 696e 5f74 6573 745f 7370  rt train_test_sp
+00000f70: 6c69 7460 2e0a 0a4c 696b 6520 6073 6b6c  lit`...Like `skl
+00000f80: 6561 726e 602c 2060 6173 7461 7274 6573  earn`, `astartes
+00000f90: 6020 6163 6365 7074 7320 616e 7920 6974  ` accepts any it
+00000fa0: 6572 6162 6c65 206f 626a 6563 7420 6173  erable object as
+00000fb0: 2060 5860 2c20 6079 602c 2061 6e64 2060   `X`, `y`, and `
+00000fc0: 6c61 6265 6c73 602e 0a45 6163 6820 7769  labels`..Each wi
+00000fd0: 6c6c 2062 6520 636f 6e76 6572 7465 6420  ll be converted 
+00000fe0: 746f 2061 2060 6e75 6d70 7960 2061 7272  to a `numpy` arr
+00000ff0: 6179 2066 6f72 2069 6e74 6572 6e61 6c20  ay for internal 
+00001000: 6f70 6572 6174 696f 6e73 2c20 616e 6420  operations, and 
+00001010: 7265 7475 726e 6564 2061 7320 6120 606e  returned as a `n
+00001020: 756d 7079 6020 6172 7261 7920 7769 7468  umpy` array with
+00001030: 206c 696d 6974 6564 2065 7863 6570 7469   limited excepti
+00001040: 6f6e 733a 2069 6620 6058 6020 6973 2061  ons: if `X` is a
+00001050: 2060 7061 6e64 6173 6020 6044 6174 6146   `pandas` `DataF
+00001060: 7261 6d65 602c 2060 7960 2069 7320 6120  rame`, `y` is a 
+00001070: 6053 6572 6965 7360 2c20 6f72 2060 6c61  `Series`, or `la
+00001080: 6265 6c73 6020 6973 2061 2060 5365 7269  bels` is a `Seri
+00001090: 6573 602c 2060 6173 7461 7274 6573 6020  es`, `astartes` 
+000010a0: 7769 6c6c 2063 6173 7420 6974 2062 6163  will cast it bac
+000010b0: 6b20 746f 2069 7473 206f 7269 6769 6e61  k to its origina
+000010c0: 6c20 7479 7065 2069 6e63 6c75 6469 6e67  l type including
+000010d0: 2069 7473 2069 6e64 6578 2061 6e64 2063   its index and c
+000010e0: 6f6c 756d 6e20 6e61 6d65 732e 0a0a 3e20  olumn names...> 
+000010f0: 2a2a 4e6f 7465 2a2a 0a3e 2054 6865 2064  **Note**.> The d
+00001100: 6576 656c 6f70 6572 7320 7265 636f 6d6d  evelopers recomm
+00001110: 656e 6420 7061 7373 696e 6720 6058 602c  end passing `X`,
+00001120: 2060 7960 2c20 616e 6420 606c 6162 656c   `y`, and `label
+00001130: 7360 2061 7320 606e 756d 7079 6020 6172  s` as `numpy` ar
+00001140: 7261 7973 2061 6e64 2068 616e 646c 696e  rays and handlin
+00001150: 6720 7468 6520 636f 6e76 6572 7369 6f6e  g the conversion
+00001160: 2074 6f20 616e 6420 6672 6f6d 206f 7468   to and from oth
+00001170: 6572 2074 7970 6573 2065 7870 6c69 6369  er types explici
+00001180: 7479 206f 6e20 796f 7572 206f 776e 2e20  ty on your own. 
+00001190: 4265 6869 6e64 2d74 6865 2d73 6365 6e65  Behind-the-scene
+000011a0: 7320 7479 7065 2063 6173 7469 6e67 2063  s type casting c
+000011b0: 616e 206c 6561 6420 746f 2075 6e65 7870  an lead to unexp
+000011c0: 6563 7465 6420 6265 6861 7669 6f72 210a  ected behavior!.
+000011d0: 0a42 7920 6465 6661 756c 742c 2060 6173  .By default, `as
+000011e0: 7461 7274 6573 6020 7769 6c6c 2073 706c  tartes` will spl
+000011f0: 6974 2064 6174 6120 7261 6e64 6f6d 6c79  it data randomly
+00001200: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
+00001210: 6120 7661 7269 6574 7920 6f66 2061 6c67  a variety of alg
+00001220: 6f72 6974 686d 6963 2073 616d 706c 696e  orithmic samplin
+00001230: 6720 6170 7072 6f61 6368 6573 2063 616e  g approaches can
+00001240: 2062 6520 7573 6564 2062 7920 7370 6563   be used by spec
+00001250: 6966 7969 6e67 2074 6865 2060 7361 6d70  ifying the `samp
+00001260: 6c65 7260 2061 7267 756d 656e 7420 746f  ler` argument to
+00001270: 2074 6865 2066 756e 6374 696f 6e20 2873   the function (s
+00001280: 6565 2074 6865 205b 5461 626c 6520 6f66  ee the [Table of
+00001290: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
+000012a0: 706c 6572 735d 2823 696d 706c 656d 656e  plers](#implemen
+000012b0: 7465 642d 7361 6d70 6c69 6e67 2d61 6c67  ted-sampling-alg
+000012c0: 6f72 6974 686d 7329 2066 6f72 2061 2063  orithms) for a c
+000012d0: 6f6d 706c 6574 206c 6973 7420 6f66 206f  omplet list of o
+000012e0: 7074 696f 6e73 2061 6e64 2074 6865 6972  ptions and their
+000012f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2072   corresponding r
+00001300: 6566 6572 656e 6365 7329 3a0a 0a60 6060  eferences):..```
+00001310: 7079 7468 6f6e 0a58 5f74 7261 696e 2c20  python.X_train, 
+00001320: 585f 7465 7374 2c20 795f 7472 6169 6e2c  X_test, y_train,
+00001330: 2079 5f74 6573 7420 3d20 7472 6169 6e5f   y_test = train_
+00001340: 7465 7374 5f73 706c 6974 280a 2020 582c  test_split(.  X,
+00001350: 2020 2320 7072 6566 6572 6162 6c79 206e    # preferably n
+00001360: 756d 7079 2061 7272 6179 732c 2062 7574  umpy arrays, but
+00001370: 2061 7374 6172 7465 7320 7769 6c6c 2063   astartes will c
+00001380: 6173 7420 6974 2066 6f72 2079 6f75 0a20  ast it for you. 
+00001390: 2079 2c0a 2020 7361 6d70 6c65 7220 3d20   y,.  sampler = 
+000013a0: 276b 656e 6e61 7264 5f73 746f 6e65 272c  'kennard_stone',
+000013b0: 2020 2320 616e 7920 6f66 2074 6865 2073    # any of the s
+000013c0: 7570 706f 7274 6564 2073 616d 706c 6572  upported sampler
+000013d0: 730a 290a 6060 600a 0a54 6861 7427 7320  s.).```..That's 
+000013e0: 616c 6c20 796f 7520 6e65 6564 2074 6f20  all you need to 
+000013f0: 6765 7420 7374 6172 7465 6420 7769 7468  get started with
+00001400: 2060 6173 7461 7274 6573 6021 2054 6865   `astartes`! The
+00001410: 206e 6578 7420 7365 6374 696f 6e73 2069   next sections i
+00001420: 6e63 6c75 6465 206d 6f72 6520 6578 616d  nclude more exam
+00001430: 706c 6573 2061 6e64 2073 6f6d 6520 6465  ples and some de
+00001440: 6d6f 206e 6f74 6562 6f6f 6b73 2079 6f75  mo notebooks you
+00001450: 2063 616e 2074 7279 2069 6e20 796f 7572   can try in your
+00001460: 2062 726f 7773 6572 2e0a 0a23 2323 2045   browser...### E
+00001470: 7861 6d70 6c65 204e 6f74 6562 6f6f 6b73  xample Notebooks
+00001480: 0a0a 436c 6963 6b20 7468 6520 6261 6467  ..Click the badg
+00001490: 6573 2069 6e20 7468 6520 7461 626c 6520  es in the table 
+000014a0: 6265 6c6f 7720 746f 2062 6520 7461 6b65  below to be take
+000014b0: 6e20 746f 2061 206c 6976 652c 2069 6e74  n to a live, int
+000014c0: 6572 6163 7469 7665 2064 656d 6f20 6f66  eractive demo of
+000014d0: 2060 6173 7461 7274 6573 603a 0a0a 7c20   `astartes`:..| 
+000014e0: 4465 6d6f 207c 2054 6f70 6963 207c 204c  Demo | Topic | L
+000014f0: 696e 6b20 7c0a 7c3a 2d2d 2d3a 7c2d 2d2d  ink |.|:---:|---
+00001500: 7c2d 2d2d 7c0a 7c20 436f 6d70 6172 696e  |---|.| Comparin
+00001510: 6720 5361 6d70 6c69 6e67 2041 6c67 6f72  g Sampling Algor
+00001520: 6974 686d 7320 7769 7468 2046 6173 7420  ithms with Fast 
+00001530: 466f 6f64 207c 2056 6973 7561 6c20 7265  Food | Visual re
+00001540: 7072 6573 656e 7461 7469 6f6e 7320 6f66  presentations of
+00001550: 2068 6f77 2064 6966 6665 7265 6e74 2073   how different s
+00001560: 616d 706c 6572 7320 6166 6665 6374 2064  amplers affect d
+00001570: 6174 6120 7061 7274 6974 696f 6e69 6e67  ata partitioning
+00001580: 207c 205b 215b 436f 6c61 625d 2868 7474   | [![Colab](htt
+00001590: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000015a0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000015b0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000015c0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000015d0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+000015e0: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+000015f0: 2f4a 6163 6b73 6f6e 4275 726e 732f 6173  /JacksonBurns/as
+00001600: 7461 7274 6573 2f62 6c6f 622f 6d61 696e  tartes/blob/main
+00001610: 2f65 7861 6d70 6c65 732f 7370 6c69 745f  /examples/split_
+00001620: 636f 6d70 6172 6973 6f6e 732f 7370 6c69  comparisons/spli
+00001630: 745f 636f 6d70 6172 6973 6f6e 732e 6970  t_comparisons.ip
+00001640: 796e 6229 207c 0a7c 2055 7369 6e67 2060  ynb) |.| Using `
+00001650: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001660: 706c 6974 6020 7769 7468 2074 6865 2060  plit` with the `
+00001670: 736b 6c65 6172 6e60 2065 7861 6d70 6c65  sklearn` example
+00001680: 2064 6174 6173 6574 7320 7c20 4465 6d6f   datasets | Demo
+00001690: 6e73 7472 6174 696e 6720 686f 7720 7769  nstrating how wi
+000016a0: 7468 6f6c 6469 6e67 2061 2074 6573 7420  tholding a test 
+000016b0: 7365 7420 7769 7468 2060 7472 6169 6e5f  set with `train_
+000016c0: 7661 6c5f 7465 7374 5f73 706c 6974 6020  val_test_split` 
+000016d0: 6361 6e20 696d 7061 6374 2070 6572 666f  can impact perfo
+000016e0: 726d 616e 6365 207c 205b 215b 436f 6c61  rmance | [![Cola
+000016f0: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
+00001700: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001710: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+00001720: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
+00001730: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+00001740: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+00001750: 6769 7468 7562 2f4a 6163 6b73 6f6e 4275  github/JacksonBu
+00001760: 726e 732f 6173 7461 7274 6573 2f62 6c6f  rns/astartes/blo
+00001770: 622f 6d61 696e 2f65 7861 6d70 6c65 732f  b/main/examples/
+00001780: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001790: 706c 6974 5f73 6b6c 6561 726e 5f65 7861  plit_sklearn_exa
+000017a0: 6d70 6c65 2f74 7261 696e 5f76 616c 5f74  mple/train_val_t
+000017b0: 6573 745f 7370 6c69 745f 6578 616d 706c  est_split_exampl
+000017c0: 652e 6970 796e 6229 207c 0a7c 2043 6865  e.ipynb) |.| Che
+000017d0: 6d69 6e66 6f72 6d61 7469 6373 2073 616d  minformatics sam
+000017e0: 706c 6520 7365 7420 7061 7274 6974 696f  ple set partitio
+000017f0: 6e69 6e67 2077 6974 6820 6061 7374 6172  ning with `astar
+00001800: 7465 7360 207c 2045 7874 7261 706f 6c61  tes` | Extrapola
+00001810: 7469 6f6e 2076 732e 2049 6e74 6572 706f  tion vs. Interpo
+00001820: 6c61 7469 6f6e 2069 6d70 6163 7420 6f6e  lation impact on
+00001830: 2063 6865 6d69 6e66 6f72 6d61 7469 6373   cheminformatics
+00001840: 206d 6f64 656c 2061 6363 7572 6163 7920   model accuracy 
+00001850: 7c20 5b21 5b43 6f6c 6162 5d28 6874 7470  | [![Colab](http
+00001860: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001870: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
+00001880: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
+00001890: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+000018a0: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+000018b0: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+000018c0: 4a61 636b 736f 6e42 7572 6e73 2f61 7374  JacksonBurns/ast
+000018d0: 6172 7465 732f 626c 6f62 2f6d 6169 6e2f  artes/blob/main/
+000018e0: 6578 616d 706c 6573 2f62 6172 7269 6572  examples/barrier
+000018f0: 5f70 7265 6469 6374 696f 6e5f 7769 7468  _prediction_with
+00001900: 5f52 4442 372f 5244 4237 5f62 6172 7269  _RDB7/RDB7_barri
+00001910: 6572 5f70 7265 6469 6374 696f 6e5f 6578  er_prediction_ex
+00001920: 616d 706c 652e 6970 796e 6229 207c 0a7c  ample.ipynb) |.|
+00001930: 2043 6f6d 7061 7269 6e67 2070 6172 7469   Comparing parti
+00001940: 7469 6f6e 696e 6720 6170 7072 6f61 6368  tioning approach
+00001950: 6573 2066 6f72 2061 6c6b 616e 6573 207c  es for alkanes |
+00001960: 2056 6973 7561 6c69 7a69 6e67 2068 6f77   Visualizing how
+00001970: 2073 616d 706c 6572 2069 6d70 6163 7420   sampler impact 
+00001980: 6d6f 6465 6c20 7065 7266 6f72 6d61 6e63  model performanc
+00001990: 6520 7769 7468 2073 696d 706c 6520 6368  e with simple ch
+000019a0: 656d 6963 616c 7320 7c20 5b21 5b43 6f6c  emicals | [![Col
+000019b0: 6162 5d28 6874 7470 733a 2f2f 636f 6c61  ab](https://cola
+000019c0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+000019d0: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
+000019e0: 6162 2d62 6164 6765 2e73 7667 295d 2868  ab-badge.svg)](h
+000019f0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00001a00: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00001a10: 2f67 6974 6875 622f 4a61 636b 736f 6e42  /github/JacksonB
+00001a20: 7572 6e73 2f61 7374 6172 7465 732f 626c  urns/astartes/bl
+00001a30: 6f62 2f6d 6169 6e2f 6578 616d 706c 6573  ob/main/examples
+00001a40: 2f6d 6c70 6473 5f32 3032 335f 6173 7461  /mlpds_2023_asta
+00001a50: 7274 6573 5f64 656d 6f6e 7374 7261 7469  rtes_demonstrati
+00001a60: 6f6e 2f6d 6c70 6473 5f32 3032 335f 6465  on/mlpds_2023_de
+00001a70: 6d6f 2e69 7079 6e62 2920 7c0a 0a54 6f20  mo.ipynb) |..To 
+00001a80: 6578 6563 7574 6520 7468 6573 6520 6e6f  execute these no
+00001a90: 7465 626f 6f6b 7320 6c6f 6361 6c6c 792c  tebooks locally,
+00001aa0: 2063 6c6f 6e65 2074 6869 7320 7265 706f   clone this repo
+00001ab0: 7369 746f 7279 2028 692e 652e 2060 6769  sitory (i.e. `gi
+00001ac0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00001ad0: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
+00001ae0: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
+00001af0: 2e67 6974 6029 2c20 6e61 7669 6761 7465  .git`), navigate
+00001b00: 2074 6f20 7468 6520 6061 7374 6172 7465   to the `astarte
+00001b10: 7360 2064 6972 6563 746f 7279 2c20 7275  s` directory, ru
+00001b20: 6e20 6070 6970 2069 6e73 7461 6c6c 202e  n `pip install .
+00001b30: 5b64 656d 6f73 5d60 2c20 7468 656e 206f  [demos]`, then o
+00001b40: 7065 6e20 616e 6420 7275 6e20 7468 6520  pen and run the 
+00001b50: 6e6f 7465 626f 6f6b 7320 696e 2079 6f75  notebooks in you
+00001b60: 7220 7072 6566 6572 7265 6420 6564 6974  r preferred edit
+00001b70: 6f72 2e0a 596f 7520 646f 205f 6e6f 745f  or..You do _not_
+00001b80: 206e 6565 6420 746f 2065 7865 6375 7465   need to execute
+00001b90: 2074 6865 2063 656c 6c73 2070 7265 6669   the cells prefi
+00001ba0: 7865 6420 7769 7468 2060 2525 6361 7074  xed with `%%capt
+00001bb0: 7572 6560 202d 2074 6865 7920 6172 6520  ure` - they are 
+00001bc0: 6f6e 6c79 2070 7265 7365 6e74 2066 6f72  only present for
+00001bd0: 2063 6f6d 7061 7469 6269 6c69 7479 2077   compatibility w
+00001be0: 6974 6820 476f 6f67 6c65 2043 6f6c 6162  ith Google Colab
+00001bf0: 2e0a 0a23 2323 2057 6974 6868 6f6c 6420  ...### Withhold 
+00001c00: 5465 7374 696e 6720 4461 7461 2077 6974  Testing Data wit
+00001c10: 6820 6074 7261 696e 5f76 616c 5f74 6573  h `train_val_tes
+00001c20: 745f 7370 6c69 7460 0a46 6f72 2072 6967  t_split`.For rig
+00001c30: 6f72 6f75 7320 4d4c 2072 6573 6561 7263  orous ML researc
+00001c40: 682c 2069 7420 6973 2063 7269 7469 6361  h, it is critica
+00001c50: 6c20 746f 2077 6974 6868 6f6c 6420 736f  l to withhold so
+00001c60: 6d65 2064 6174 6120 6475 7269 6e67 2074  me data during t
+00001c70: 7261 696e 696e 6720 746f 2075 7365 2061  raining to use a
+00001c80: 2060 7465 7374 6020 7365 742e 0a54 6865   `test` set..The
+00001c90: 206d 6f64 656c 2073 686f 756c 6420 5f6e   model should _n
+00001ca0: 6576 6572 5f20 7365 6520 7468 6973 2064  ever_ see this d
+00001cb0: 6174 6120 6475 7269 6e67 2074 7261 696e  ata during train
+00001cc0: 696e 6720 2875 6e6c 696b 6520 7468 6520  ing (unlike the 
+00001cd0: 7661 6c69 6461 7469 6f6e 2073 6574 2920  validation set) 
+00001ce0: 736f 2074 6861 7420 7765 2063 616e 2067  so that we can g
+00001cf0: 6574 2061 6e20 6163 6375 7261 7465 206d  et an accurate m
+00001d00: 6561 7375 7265 6d65 6e74 206f 6620 6974  easurement of it
+00001d10: 7320 7065 7266 6f72 6d61 6e63 652e 0a0a  s performance...
+00001d20: 5769 7468 2060 6173 7461 7274 6573 6020  With `astartes` 
+00001d30: 7065 7266 6f72 6d69 6e67 2074 6869 7320  performing this 
+00001d40: 7468 7265 652d 7761 7920 6461 7461 2073  three-way data s
+00001d50: 706c 6974 2069 7320 7265 6164 696c 7920  plit is readily 
+00001d60: 6176 6169 6c61 626c 6520 7769 7468 2060  available with `
+00001d70: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001d80: 706c 6974 603a 0a60 6060 7079 7468 6f6e  plit`:.```python
+00001d90: 0a66 726f 6d20 6173 7461 7274 6573 2069  .from astartes i
+00001da0: 6d70 6f72 7420 7472 6169 6e5f 7661 6c5f  mport train_val_
+00001db0: 7465 7374 5f73 706c 6974 0a0a 585f 7472  test_split..X_tr
+00001dc0: 6169 6e2c 2058 5f76 616c 2c20 585f 7465  ain, X_val, X_te
+00001dd0: 7374 203d 2074 7261 696e 5f76 616c 5f74  st = train_val_t
+00001de0: 6573 745f 7370 6c69 7428 582c 2073 616d  est_split(X, sam
+00001df0: 706c 6572 203d 2027 7370 6865 7265 5f65  pler = 'sphere_e
+00001e00: 7863 6c75 7369 6f6e 2729 0a60 6060 0a59  xclusion').```.Y
+00001e10: 6f75 2063 616e 206e 6f77 2074 7261 696e  ou can now train
+00001e20: 2079 6f75 7220 6d6f 6465 6c20 7769 7468   your model with
+00001e30: 2060 585f 7472 6169 6e60 2c20 6f70 7469   `X_train`, opti
+00001e40: 6d69 7a65 2079 6f75 7220 6d6f 6465 6c20  mize your model 
+00001e50: 7769 7468 2060 585f 7661 6c60 2c20 616e  with `X_val`, an
+00001e60: 6420 6d65 6173 7572 6520 6974 7320 7065  d measure its pe
+00001e70: 7266 6f72 6d61 6e63 6520 7769 7468 2060  rformance with `
+00001e80: 585f 7465 7374 602e 0a0a 2323 2320 4576  X_test`...### Ev
+00001e90: 616c 7561 7465 2074 6865 2049 6d70 6163  aluate the Impac
+00001ea0: 7420 6f66 2053 706c 6974 7469 6e67 2041  t of Splitting A
+00001eb0: 6c67 6f72 6974 686d 730a 466f 7220 6461  lgorithms.For da
+00001ec0: 7461 2077 6974 6820 6d61 6e79 2066 6561  ta with many fea
+00001ed0: 7475 7265 7320 6974 2063 616e 2062 6520  tures it can be 
+00001ee0: 6469 6666 6963 756c 7420 746f 2076 6973  difficult to vis
+00001ef0: 7561 6c69 7a65 2068 6f77 2064 6966 6665  ualize how diffe
+00001f00: 7265 6e74 2073 616d 706c 696e 6720 616c  rent sampling al
+00001f10: 676f 7269 7468 6d73 2063 6861 6e67 6520  gorithms change 
+00001f20: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+00001f30: 206f 6620 6461 7461 2069 6e74 6f20 7472   of data into tr
+00001f40: 6169 6e69 6e67 2c20 7661 6c69 6461 7469  aining, validati
+00001f50: 6f6e 2c20 616e 6420 7465 7374 696e 6720  on, and testing 
+00001f60: 6c69 6b65 2077 6520 646f 2069 6e20 736f  like we do in so
+00001f70: 6d65 206f 6620 7468 6520 6465 6d6f 206e  me of the demo n
+00001f80: 6f74 6562 6f6f 6b73 2e0a 546f 2061 6964  otebooks..To aid
+00001f90: 2069 6e20 616e 616c 797a 696e 6720 7468   in analyzing th
+00001fa0: 6520 696d 7061 6374 206f 6620 7468 6520  e impact of the 
+00001fb0: 616c 676f 7269 7468 6d73 2c20 6061 7374  algorithms, `ast
+00001fc0: 6172 7465 7360 2070 726f 7669 6465 7320  artes` provides 
+00001fd0: 6067 656e 6572 6174 655f 7265 6772 6573  `generate_regres
+00001fe0: 7369 6f6e 5f72 6573 756c 7473 5f64 6963  sion_results_dic
+00001ff0: 7460 2e0a 5468 6973 2066 756e 6374 696f  t`..This functio
+00002000: 6e20 616c 6c6f 7773 2075 7365 7273 2074  n allows users t
+00002010: 6f20 7175 6963 6b6c 7920 6576 616c 7561  o quickly evalua
+00002020: 7465 2074 6865 2069 6d70 6163 7420 6f66  te the impact of
+00002030: 2064 6966 6665 7265 6e74 2073 706c 6974   different split
+00002040: 7469 6e67 2074 6563 686e 6971 7565 7320  ting techniques 
+00002050: 6f6e 2061 6e79 206d 6f64 656c 2073 7570  on any model sup
+00002060: 706f 7274 6564 2062 7920 6073 6b6c 6561  ported by `sklea
+00002070: 726e 602e 2041 6c6c 2072 6573 756c 7473  rn`. All results
+00002080: 2061 7265 2073 746f 7265 6420 696e 2061   are stored in a
+00002090: 2064 6963 7469 6f6e 6172 7920 666f 726d   dictionary form
+000020a0: 6174 2061 6e64 2063 616e 2062 6520 6469  at and can be di
+000020b0: 7370 6c61 7965 6420 696e 2061 206e 6561  splayed in a nea
+000020c0: 746c 7920 666f 726d 6174 7465 6420 7461  tly formatted ta
+000020d0: 626c 6520 7573 696e 6720 7468 6520 6f70  ble using the op
+000020e0: 7469 6f6e 616c 2060 7072 696e 745f 7265  tional `print_re
+000020f0: 7375 6c74 7360 2061 7267 756d 656e 742e  sults` argument.
+00002100: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00002110: 2073 6b6c 6561 726e 2e73 766d 2069 6d70   sklearn.svm imp
+00002120: 6f72 7420 4c69 6e65 6172 5356 520a 0a66  ort LinearSVR..f
+00002130: 726f 6d20 6173 7461 7274 6573 2e75 7469  rom astartes.uti
+00002140: 6c73 2069 6d70 6f72 7420 6765 6e65 7261  ls import genera
+00002150: 7465 5f72 6567 7265 7373 696f 6e5f 7265  te_regression_re
+00002160: 7375 6c74 735f 6469 6374 0a0a 736b 6c65  sults_dict..skle
+00002170: 6172 6e5f 6d6f 6465 6c20 3d20 4c69 6e65  arn_model = Line
+00002180: 6172 5356 5228 290a 7265 7375 6c74 735f  arSVR().results_
+00002190: 6469 6374 203d 2067 656e 6572 6174 655f  dict = generate_
+000021a0: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
+000021b0: 7473 5f64 6963 7428 0a20 2020 2073 6b6c  ts_dict(.    skl
+000021c0: 6561 726e 5f6d 6f64 656c 2c0a 2020 2020  earn_model,.    
+000021d0: 582c 0a20 2020 2079 2c0a 2020 2020 7072  X,.    y,.    pr
+000021e0: 696e 745f 7265 7375 6c74 733d 5472 7565  int_results=True
+000021f0: 2c0a 290a 0a20 2020 2020 2020 2020 5472  ,.)..         Tr
+00002200: 6169 6e20 2020 2020 2020 5661 6c20 2020  ain       Val   
+00002210: 2020 2054 6573 740a 2d2d 2d2d 2020 2d2d     Test.----  --
+00002220: 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2d2d 2d2d  ------  --------
+00002230: 2020 2d2d 2d2d 2d2d 2d2d 0a4d 4145 2020    --------.MAE  
+00002240: 2031 2e34 3135 3232 2020 2033 2e31 3334   1.41522   3.134
+00002250: 3335 2020 2032 2e31 3730 3931 0a52 4d53  35   2.17091.RMS
+00002260: 4520 2032 2e30 3330 3632 2020 2033 2e37  E  2.03062   3.7
+00002270: 3337 3231 2020 2032 2e34 3030 3431 0a52  3721   2.40041.R
+00002280: 3220 2020 2030 2e39 3037 3435 2020 2030  2    0.90745   0
+00002290: 2e38 3037 3837 2020 2030 2e37 3834 3132  .80787   0.78412
+000022a0: 0a0a 6060 600a 0a23 2323 2041 6363 6573  ..```..### Acces
+000022b0: 7320 5361 6d70 6c69 6e67 2041 6c67 6f72  s Sampling Algor
+000022c0: 6974 686d 7320 4469 7265 6374 6c79 0a54  ithms Directly.T
+000022d0: 6865 2073 616d 706c 696e 6720 616c 676f  he sampling algo
+000022e0: 7269 7468 6d73 2069 6d70 6c65 6d65 6e74  rithms implement
+000022f0: 6564 2069 6e20 6061 7374 6172 7465 7360  ed in `astartes`
+00002300: 2063 616e 2061 6c73 6f20 6265 2064 6972   can also be dir
+00002310: 6563 746c 7920 6163 6365 7373 6564 2061  ectly accessed a
+00002320: 6e64 2072 756e 2069 6620 6974 2069 7320  nd run if it is 
+00002330: 6d6f 7265 2075 7365 6675 6c20 666f 7220  more useful for 
+00002340: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
+00002350: 732e 0a49 6e20 7468 6520 6265 6c6f 7720  s..In the below 
+00002360: 6578 616d 706c 652c 2077 6520 696d 706f  example, we impo
+00002370: 7274 2074 6865 204b 656e 6e61 7264 2053  rt the Kennard S
+00002380: 746f 6e65 2073 616d 706c 6572 2c20 7573  tone sampler, us
+00002390: 6520 6974 2074 6f20 7061 7274 6974 696f  e it to partitio
+000023a0: 6e20 6120 7369 6d70 6c65 2061 7272 6179  n a simple array
+000023b0: 2c20 616e 6420 7468 656e 2072 6574 7269  , and then retri
+000023c0: 6576 6520 6120 7361 6d70 6c65 2e0a 6060  eve a sample..``
+000023d0: 6070 7974 686f 6e0a 6672 6f6d 2061 7374  `python.from ast
+000023e0: 6172 7465 732e 7361 6d70 6c65 7273 2e69  artes.samplers.i
+000023f0: 6e74 6572 706f 6c61 7469 6f6e 2069 6d70  nterpolation imp
+00002400: 6f72 7420 4b65 6e6e 6172 6453 746f 6e65  ort KennardStone
+00002410: 0a0a 6b65 6e6e 6172 645f 7374 6f6e 6520  ..kennard_stone 
+00002420: 3d20 4b65 6e6e 6172 6453 746f 6e65 285b  = KennardStone([
+00002430: 5b31 2c20 325d 2c20 5b33 2c20 345d 2c20  [1, 2], [3, 4], 
+00002440: 5b35 2c20 365d 5d29 0a66 6972 7374 5f32  [5, 6]]).first_2
+00002450: 5f73 616d 706c 6573 203d 206b 656e 6e61  _samples = kenna
+00002460: 7264 5f73 746f 6e65 2e67 6574 5f73 616d  rd_stone.get_sam
+00002470: 706c 655f 6964 7873 2832 290a 6060 600a  ple_idxs(2).```.
+00002480: 416c 6c20 7361 6d70 6c65 7273 2069 6e20  All samplers in 
+00002490: 6061 7374 6172 7465 7360 2069 6d70 6c65  `astartes` imple
+000024a0: 6d65 6e74 2061 2060 5f73 616d 706c 6528  ment a `_sample(
+000024b0: 2960 206d 6574 686f 6420 7468 6174 2069  )` method that i
+000024c0: 7320 6361 6c6c 6564 2062 7920 7468 6520  s called by the 
+000024d0: 636f 6e73 7472 7563 746f 7220 2869 2e65  constructor (i.e
+000024e0: 2e20 6772 6565 6469 6c79 2920 616e 6420  . greedily) and 
+000024f0: 6569 7468 6572 2061 2060 6765 745f 7361  either a `get_sa
+00002500: 6d70 6c65 725f 6964 7873 6020 6f72 2060  mpler_idxs` or `
+00002510: 6765 745f 636c 7573 7465 725f 6964 7873  get_cluster_idxs
+00002520: 6020 666f 7220 696e 7465 7270 6f6c 6174  ` for interpolat
+00002530: 6976 6520 616e 6420 6578 7472 6170 6f6c  ive and extrapol
+00002540: 6174 6976 6520 7361 6d70 6c65 7273 2c20  ative samplers, 
+00002550: 7265 7370 6563 7469 7665 6c79 2e0a 466f  respectively..Fo
+00002560: 7220 6d6f 7265 2064 6574 6169 6c20 6f6e  r more detail on
+00002570: 2074 6865 2069 6d70 6c65 6d65 6e74 6169   the implementai
+00002580: 746f 6e20 616e 6420 6465 7369 676e 206f  ton and design o
+00002590: 6620 7361 6d70 6c65 7273 2069 6e20 6061  f samplers in `a
+000025a0: 7374 6172 7465 7360 2c20 7365 6520 7468  startes`, see th
+000025b0: 6520 5b44 6576 656c 6f70 6572 204e 6f74  e [Developer Not
+000025c0: 6573 5d28 2363 6f6e 7472 6962 7574 696e  es](#contributin
+000025d0: 672d 2d64 6576 656c 6f70 6572 2d6e 6f74  g--developer-not
+000025e0: 6573 2920 7365 6374 696f 6e2e 0a0a 2323  es) section...##
+000025f0: 2054 6865 6f72 7920 616e 6420 4170 706c   Theory and Appl
+00002600: 6963 6174 696f 6e20 6f66 2060 6173 7461  ication of `asta
+00002610: 7274 6573 600a 5468 6973 2073 6563 7469  rtes`.This secti
+00002620: 6f6e 206f 6620 7468 6520 5245 4144 4d45  on of the README
+00002630: 2064 6574 6169 6c73 2073 6f6d 6520 6f66   details some of
+00002640: 2074 6865 2074 6865 6f72 7920 6265 6869   the theory behi
+00002650: 6e64 2077 6879 2074 6865 2061 6c67 6f72  nd why the algor
+00002660: 6974 686d 7320 696d 706c 656d 656e 7465  ithms implemente
+00002670: 6420 696e 2060 6173 7461 7274 6573 6020  d in `astartes` 
+00002680: 6172 6520 696d 706f 7274 616e 7420 616e  are important an
+00002690: 6420 736f 6d65 206d 6f74 6976 6174 696e  d some motivatin
+000026a0: 6720 6578 616d 706c 6573 2e0a 466f 7220  g examples..For 
+000026b0: 6120 636f 6d70 7265 6865 6e73 6976 6520  a comprehensive 
+000026c0: 7761 6c6b 7468 726f 7567 6820 6f66 2074  walkthrough of t
+000026d0: 6865 2074 6865 6f72 7920 616e 6420 696d  he theory and im
+000026e0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+000026f0: 6061 7374 6172 7465 7360 2c20 666f 6c6c  `astartes`, foll
+00002700: 6f77 205b 7468 6973 206c 696e 6b5d 2868  ow [this link](h
+00002710: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002720: 6d2f 4a61 636b 736f 6e42 7572 6e73 2f61  m/JacksonBurns/a
+00002730: 7374 6172 7465 732f 7261 772f 6a6f 7373  startes/raw/joss
+00002740: 2d70 6170 6572 2f42 7572 6e73 2d53 7069  -paper/Burns-Spi
+00002750: 656b 6572 6d61 6e6e 2d42 6861 7474 6163  ekermann-Bhattac
+00002760: 6861 726a 6565 5f61 7374 6172 7465 732e  harjee_astartes.
+00002770: 7064 6629 2074 6f20 7265 6164 2074 6865  pdf) to read the
+00002780: 2063 6f6d 7061 6e69 6f6e 2070 6170 6572   companion paper
+00002790: 2028 6672 6565 6c79 2061 7661 696c 6162   (freely availab
+000027a0: 6c65 2061 6e64 2068 6f73 7465 6420 6865  le and hosted he
+000027b0: 7265 206f 6e20 4769 7448 7562 292e 0a0a  re on GitHub)...
+000027c0: 3e20 2a2a 4e6f 7465 2a2a 0a3e 2057 6520  > **Note**.> We 
+000027d0: 7265 6665 7265 6e63 6520 6f70 656e 2d61  reference open-a
+000027e0: 6363 6573 7320 7075 626c 6963 6174 696f  ccess publicatio
+000027f0: 6e73 2077 6865 7265 7665 7220 706f 7373  ns wherever poss
+00002800: 6962 6c65 2e20 466f 7220 6172 7469 636c  ible. For articl
+00002810: 6573 206c 6f63 6b65 6420 6265 6869 6e64  es locked behind
+00002820: 2061 2070 6179 7761 6c6c 2028 6465 6e6f   a paywall (deno
+00002830: 7465 6420 7769 7468 203a 736d 616c 6c5f  ted with :small_
+00002840: 626c 7565 5f64 6961 6d6f 6e64 3a29 2c20  blue_diamond:), 
+00002850: 7765 2069 6e73 7465 6164 2073 7567 6765  we instead sugge
+00002860: 7374 2072 6561 6469 6e67 205b 7468 6973  st reading [this
+00002870: 2057 696b 6970 6564 6961 2070 6167 655d   Wikipedia page]
+00002880: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+00002890: 7065 6469 612e 6f72 672f 7769 6b69 2f53  pedia.org/wiki/S
+000028a0: 6369 2d48 7562 2920 616e 6420 6162 736f  ci-Hub) and abso
+000028b0: 6c75 7465 6c79 205f 5f6e 6f74 5f5f 2061  lutely __not__ a
+000028c0: 7474 656d 7074 696e 6720 746f 2062 7970  ttempting to byp
+000028d0: 6173 7320 7468 6520 7061 7977 616c 6c2e  ass the paywall.
+000028e0: 0a0a 2323 2320 5261 7469 6f6e 616c 2053  ..### Rational S
+000028f0: 706c 6974 7469 6e67 2041 6c67 6f72 6974  plitting Algorit
+00002900: 686d 730a 5768 696c 6520 6d75 6368 206d  hms.While much m
+00002910: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+00002920: 6973 2064 6f6e 6520 7769 7468 2061 2072  is done with a r
+00002930: 616e 646f 6d20 6368 6f69 6365 2062 6574  andom choice bet
+00002940: 7765 656e 2074 7261 696e 696e 672f 7661  ween training/va
+00002950: 6c69 6461 7469 6f6e 2f74 6573 7420 6461  lidation/test da
+00002960: 7461 2c20 616e 2061 6c74 6572 6e61 7469  ta, an alternati
+00002970: 7665 2069 7320 7468 6520 7573 6520 6f66  ve is the use of
+00002980: 2073 6f2d 6361 6c6c 6564 2022 7261 7469   so-called "rati
+00002990: 6f6e 616c 2220 7370 6c69 7474 696e 6720  onal" splitting 
+000029a0: 616c 676f 7269 7468 6d73 2e0a 5468 6573  algorithms..Thes
+000029b0: 6520 6170 7072 6f61 6368 6573 2075 7365  e approaches use
+000029c0: 2073 6f6d 6520 7369 6d69 6c61 7269 7479   some similarity
+000029d0: 2d62 6173 6564 2061 6c67 6f72 6974 686d  -based algorithm
+000029e0: 2074 6f20 6469 7669 6465 2064 6174 6120   to divide data 
+000029f0: 696e 746f 2073 6574 732e 0a53 6f6d 6520  into sets..Some 
+00002a00: 6f66 2074 6865 7365 2061 6c67 6f72 6974  of these algorit
+00002a10: 686d 7320 696e 636c 7564 6520 4b65 6e6e  hms include Kenn
+00002a20: 6172 642d 5374 6f6e 6520 285b 4b65 6e6e  ard-Stone ([Kenn
+00002a30: 6172 6420 2620 5374 6f6e 655d 2868 7474  ard & Stone](htt
+00002a40: 7073 3a2f 2f77 7777 2e74 616e 6466 6f6e  ps://www.tandfon
+00002a50: 6c69 6e65 2e63 6f6d 2f64 6f69 2f61 6273  line.com/doi/abs
+00002a60: 2f31 302e 3130 3830 2f30 3034 3031 3730  /10.1080/0040170
+00002a70: 362e 3139 3639 2e31 3034 3930 3636 3629  6.1969.10490666)
+00002a80: 203a 736d 616c 6c5f 626c 7565 5f64 6961   :small_blue_dia
+00002a90: 6d6f 6e64 3a29 2c20 5370 6865 7265 2045  mond:), Sphere E
+00002aa0: 7863 6c75 7369 6f6e 2028 5b54 726f 7073  xclusion ([Trops
+00002ab0: 6861 2065 742e 2061 6c5d 2868 7474 7073  ha et. al](https
+00002ac0: 3a2f 2f70 7562 732e 6163 732e 6f72 672f  ://pubs.acs.org/
+00002ad0: 646f 692f 7064 662f 3130 2e31 3032 312f  doi/pdf/10.1021/
+00002ae0: 6369 3330 3033 3338 7729 203a 736d 616c  ci300338w) :smal
+00002af0: 6c5f 626c 7565 5f64 6961 6d6f 6e64 3a29  l_blue_diamond:)
+00002b00: 2c61 7320 7765 6c6c 2061 7320 7468 6520  ,as well as the 
+00002b10: 4f70 7469 5369 6d20 6173 2064 6973 6375  OptiSim as discu
+00002b20: 7373 6564 2069 6e20 5b41 7070 6c69 6564  ssed in [Applied
+00002b30: 2043 6865 6d6f 696e 666f 726d 6174 6963   Chemoinformatic
+00002b40: 733a 2041 6368 6965 7665 6d65 6e74 7320  s: Achievements 
+00002b50: 616e 6420 4675 7475 7265 204f 7070 6f72  and Future Oppor
+00002b60: 7475 6e69 7469 6573 5d28 6874 7470 733a  tunities](https:
+00002b70: 2f2f 7777 772e 7769 6c65 792e 636f 6d2f  //www.wiley.com/
+00002b80: 656e 2d75 732f 4170 706c 6965 642b 4368  en-us/Applied+Ch
+00002b90: 656d 6f69 6e66 6f72 6d61 7469 6373 2533  emoinformatics%3
+00002ba0: 412b 4163 6869 6576 656d 656e 7473 2b61  A+Achievements+a
+00002bb0: 6e64 2b46 7574 7572 652b 4f70 706f 7274  nd+Future+Opport
+00002bc0: 756e 6974 6965 732d 702d 3937 3833 3532  unities-p-978352
+00002bd0: 3738 3036 3534 3629 203a 736d 616c 6c5f  7806546) :small_
+00002be0: 626c 7565 5f64 6961 6d6f 6e64 3a2e 0a53  blue_diamond:..S
+00002bf0: 6f6d 6520 636c 7573 7465 7269 6e67 2d62  ome clustering-b
+00002c00: 6173 6564 2073 706c 6974 7469 6e67 2074  ased splitting t
+00002c10: 6563 686e 6971 7565 7320 6861 7665 2061  echniques have a
+00002c20: 6c73 6f20 6265 656e 2069 6e63 6f72 706f  lso been incorpo
+00002c30: 7261 7465 642c 2073 7563 6820 6173 205b  rated, such as [
+00002c40: 4442 5343 414e 5d28 6874 7470 3a2f 2f63  DBSCAN](http://c
+00002c50: 6974 6573 6565 7278 2e69 7374 2e70 7375  iteseerx.ist.psu
+00002c60: 2e65 6475 2f76 6965 7764 6f63 2f64 6f77  .edu/viewdoc/dow
+00002c70: 6e6c 6f61 643f 646f 693d 3130 2e31 2e31  nload?doi=10.1.1
+00002c80: 2e31 3031 362e 3839 3026 7265 703d 7265  .1016.890&rep=re
+00002c90: 7031 2674 7970 653d 7064 6629 2e0a 0a54  p1&type=pdf)...T
+00002ca0: 6865 7265 2061 7265 2074 776f 2062 726f  here are two bro
+00002cb0: 6164 2063 6174 6567 6f72 6965 7320 6f66  ad categories of
+00002cc0: 2073 616d 706c 696e 6720 616c 676f 7269   sampling algori
+00002cd0: 7468 6d73 2069 6d70 6c65 6d65 6e74 6564  thms implemented
+00002ce0: 2069 6e20 6061 7374 6172 7465 7360 3a20   in `astartes`: 
+00002cf0: 6578 7472 6170 6f6c 6174 6976 6520 616e  extrapolative an
+00002d00: 6420 696e 7465 7270 6f6c 6174 6976 652e  d interpolative.
+00002d10: 0a54 6865 2066 6f72 6d65 7220 7769 6c6c  .The former will
+00002d20: 2066 6f72 6365 2079 6f75 7220 6d6f 6465   force your mode
+00002d30: 6c20 746f 2070 7265 6469 6374 206f 6e20  l to predict on 
+00002d40: 6f75 742d 6f66 2d73 616d 706c 6520 6461  out-of-sample da
+00002d50: 7461 2c20 7768 6963 6820 6372 6561 7465  ta, which create
+00002d60: 7320 6120 6d6f 7265 2063 6861 6c6c 656e  s a more challen
+00002d70: 6769 6e67 2074 6173 6b20 7468 616e 2069  ging task than i
+00002d80: 6e74 6572 706f 6c61 7469 7665 2073 616d  nterpolative sam
+00002d90: 706c 696e 672e 0a53 6565 2074 6865 2074  pling..See the t
+00002da0: 6162 6c65 2062 656c 6f77 2066 6f72 2061  able below for a
+00002db0: 6c6c 206f 6620 7468 6520 7361 6d70 6c69  ll of the sampli
+00002dc0: 6e67 2061 7070 726f 6163 6865 7320 6375  ng approaches cu
+00002dd0: 7272 656e 746c 7920 696d 706c 656d 656e  rrently implemen
+00002de0: 7465 6420 696e 2060 6173 7461 7274 6573  ted in `astartes
+00002df0: 602c 2061 7320 7765 6c6c 2061 7320 7468  `, as well as th
+00002e00: 6520 6879 7065 7270 6172 616d 6574 6572  e hyperparameter
+00002e10: 7320 7468 6174 2065 6163 6820 616c 676f  s that each algo
+00002e20: 7269 7468 6d20 6163 6365 7074 7320 2877  rithm accepts (w
+00002e30: 6869 6368 2061 7265 2070 6173 7365 6420  hich are passed 
+00002e40: 696e 2077 6974 6820 6068 6f70 7473 6029  in with `hopts`)
+00002e50: 2061 6e64 2061 2068 656c 7066 756c 2072   and a helpful r
+00002e60: 6566 6572 656e 6365 2066 6f72 2075 6e64  eference for und
+00002e70: 6572 7374 616e 6469 6e67 2068 6f77 2074  erstanding how t
+00002e80: 6865 2068 7970 6572 7061 7261 6d65 7465  he hyperparamete
+00002e90: 7273 2077 6f72 6b2e 0a4e 6f74 6520 7468  rs work..Note th
+00002ea0: 6174 2060 7261 6e64 6f6d 5f73 7461 7465  at `random_state
+00002eb0: 6020 6973 2064 6566 696e 6564 2061 7320  ` is defined as 
+00002ec0: 6120 6b65 7977 6f72 6420 6172 6775 6d65  a keyword argume
+00002ed0: 6e74 2069 6e20 6074 7261 696e 5f74 6573  nt in `train_tes
+00002ee0: 745f 7370 6c69 7460 2069 7473 656c 662c  t_split` itself,
+00002ef0: 2065 7665 6e20 7468 6f75 6768 2074 6865   even though the
+00002f00: 7365 2061 6c67 6f72 6974 686d 7320 7769  se algorithms wi
+00002f10: 6c6c 2075 7365 2074 6865 2060 7261 6e64  ll use the `rand
+00002f20: 6f6d 5f73 7461 7465 6020 696e 2074 6865  om_state` in the
+00002f30: 6972 206f 776e 2077 6f72 6b2e 0a44 6f20  ir own work..Do 
+00002f40: 6e6f 7420 7072 6f76 6964 6520 6120 6072  not provide a `r
+00002f50: 616e 646f 6d5f 7374 6174 6560 2069 6e20  andom_state` in 
+00002f60: 7468 6520 6068 6f70 7473 6020 6469 6374  the `hopts` dict
+00002f70: 696f 6e61 7279 202d 2069 7420 7769 6c6c  ionary - it will
+00002f80: 2062 6520 6f76 6572 7772 6974 7465 6e20   be overwritten 
+00002f90: 6279 2074 6865 2060 7261 6e64 6f6d 5f73  by the `random_s
+00002fa0: 7461 7465 6020 796f 7520 7072 6f76 6964  tate` you provid
+00002fb0: 6520 666f 7220 6074 7261 696e 5f74 6573  e for `train_tes
+00002fc0: 745f 7370 6c69 7460 2028 6f72 2074 6865  t_split` (or the
+00002fd0: 2064 6566 6175 6c74 2069 6620 6e6f 6e65   default if none
+00002fe0: 2069 7320 7072 6f76 6964 6564 292e 0a0a   is provided)...
+00002ff0: 2323 2323 2049 6d70 6c65 6d65 6e74 6564  #### Implemented
+00003000: 2053 616d 706c 696e 6720 416c 676f 7269   Sampling Algori
+00003010: 7468 6d73 0a0a 7c20 5361 6d70 6c65 7220  thms..| Sampler 
+00003020: 4e61 6d65 207c 2055 7361 6765 2053 7472  Name | Usage Str
+00003030: 696e 6720 7c20 5479 7065 207c 2048 7970  ing | Type | Hyp
+00003040: 6572 7061 7261 6d65 7465 7273 207c 2052  erparameters | R
+00003050: 6566 6572 656e 6365 207c 204e 6f74 6573  eference | Notes
+00003060: 207c 0a7c 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d   |.|:---:|---|--
+00003070: 2d7c 2d2d 2d7c 2d2d 2d7c 2d2d 2d7c 0a7c  -|---|---|---|.|
+00003080: 2052 616e 646f 6d20 7c20 2772 616e 646f   Random | 'rando
+00003090: 6d27 207c 2049 6e74 6572 706f 6c61 7469  m' | Interpolati
+000030a0: 7665 207c 2060 7368 7566 666c 6560 207c  ve | `shuffle` |
+000030b0: 205b 736b 6c65 6172 6e20 7472 6169 6e5f   [sklearn train_
+000030c0: 7465 7374 5f73 706c 6974 5d28 6874 7470  test_split](http
+000030d0: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
+000030e0: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
+000030f0: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
+00003100: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
+00003110: 6374 696f 6e2e 7472 6169 6e5f 7465 7374  ction.train_test
+00003120: 5f73 706c 6974 2e68 746d 6c29 2044 6f63  _split.html) Doc
+00003130: 756d 656e 7461 7469 6f6e 207c 2054 6869  umentation | Thi
+00003140: 7320 7361 6d70 6c65 7220 6973 2061 2064  s sampler is a d
+00003150: 6972 6563 7420 7061 7373 7468 726f 7567  irect passthroug
+00003160: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
+00003170: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
+00003180: 6974 602e 207c 0a7c 204b 656e 6e61 7264  it`. |.| Kennard
+00003190: 2d53 746f 6e65 207c 2027 6b65 6e6e 6172  -Stone | 'kennar
+000031a0: 645f 7374 6f6e 6527 207c 2049 6e74 6572  d_stone' | Inter
+000031b0: 706f 6c61 7469 7665 207c 2060 6d65 7472  polative | `metr
+000031c0: 6963 6020 7c20 4f72 6967 696e 616c 2050  ic` | Original P
+000031d0: 6170 6572 2062 7920 5b4b 656e 6e61 7264  aper by [Kennard
+000031e0: 2026 2053 746f 6e65 5d28 6874 7470 733a   & Stone](https:
+000031f0: 2f2f 7777 772e 7461 6e64 666f 6e6c 696e  //www.tandfonlin
+00003200: 652e 636f 6d2f 646f 692f 6162 732f 3130  e.com/doi/abs/10
+00003210: 2e31 3038 302f 3030 3430 3137 3036 2e31  .1080/00401706.1
+00003220: 3936 392e 3130 3439 3036 3636 2920 3a73  969.10490666) :s
+00003230: 6d61 6c6c 5f62 6c75 655f 6469 616d 6f6e  mall_blue_diamon
+00003240: 643a 207c 2045 7563 6c69 6469 616e 2064  d: | Euclidian d
+00003250: 6973 7461 6e63 6520 6973 2075 7365 6420  istance is used 
+00003260: 6279 2064 6566 6175 6c74 2c20 6173 2064  by default, as d
+00003270: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+00003280: 6f72 6967 696e 616c 2070 6170 6572 2e20  original paper. 
+00003290: 7c0a 7c20 5361 6d70 6c65 2073 6574 2050  |.| Sample set P
+000032a0: 6172 7469 7469 6f6e 696e 6720 6261 7365  artitioning base
+000032b0: 6420 6f6e 206a 6f69 6e74 2058 2d59 2064  d on joint X-Y d
+000032c0: 6973 7461 6e63 6573 2028 5350 5859 2920  istances (SPXY) 
+000032d0: 7c20 2773 7078 7927 207c 2049 6e74 6572  | 'spxy' | Inter
+000032e0: 706f 6c61 7469 7665 207c 2060 6469 7374  polative | `dist
+000032f0: 616e 6365 5f6d 6574 7269 6360 207c 2053  ance_metric` | S
+00003300: 616c 6468 616e 6120 6574 2e20 616c 205b  aldhana et. al [
+00003310: 6f72 6967 696e 616c 2070 6170 6572 5d28  original paper](
+00003320: 6874 7470 733a 2f2f 7777 772e 7363 6965  https://www.scie
+00003330: 6e63 6564 6972 6563 742e 636f 6d2f 7363  ncedirect.com/sc
+00003340: 6965 6e63 652f 6172 7469 636c 652f 6162  ience/article/ab
+00003350: 732f 7069 692f 5330 3033 3939 3134 3030  s/pii/S003991400
+00003360: 3530 3031 3932 5829 203a 736d 616c 6c5f  500192X) :small_
+00003370: 626c 7565 5f64 6961 6d6f 6e64 3a20 7c20  blue_diamond: | 
+00003380: 4578 7465 6e73 696f 6e20 6f66 204b 656e  Extension of Ken
+00003390: 6e61 7264 2053 746f 6e65 2074 6861 7420  nard Stone that 
+000033a0: 616c 736f 2069 6e63 6c75 6465 7320 7468  also includes th
+000033b0: 6520 7265 7370 6f6e 7365 2077 6865 6e20  e response when 
+000033c0: 7361 6d70 6c69 6e67 2064 6973 7461 6e63  sampling distanc
+000033d0: 6573 2e20 7c0a 7c20 5363 6166 666f 6c64  es. |.| Scaffold
+000033e0: 207c 2027 7363 6166 666f 6c64 2720 7c20   | 'scaffold' | 
+000033f0: 4578 7472 6170 6f6c 6174 6976 6520 7c20  Extrapolative | 
+00003400: 6069 6e63 6c75 6465 5f63 6869 7261 6c69  `include_chirali
+00003410: 7479 6020 7c20 5b42 656d 6973 2d4d 7572  ty` | [Bemis-Mur
+00003420: 636b 6f20 5363 6166 666f 6c64 5d28 6874  cko Scaffold](ht
+00003430: 7470 733a 2f2f 7075 6273 2e61 6373 2e6f  tps://pubs.acs.o
+00003440: 7267 2f64 6f69 2f66 756c 6c2f 3130 2e31  rg/doi/full/10.1
+00003450: 3032 312f 6a6d 3936 3032 3932 3829 203a  021/jm9602928) :
+00003460: 736d 616c 6c5f 626c 7565 5f64 6961 6d6f  small_blue_diamo
+00003470: 6e64 3a20 6173 2069 6d70 6c65 6d65 6e74  nd: as implement
+00003480: 6564 2069 6e20 5244 4b69 7420 7c20 5468  ed in RDKit | Th
+00003490: 6973 2073 616d 706c 6572 2072 6571 7569  is sampler requi
+000034a0: 7265 7320 534d 494c 4553 2073 7472 696e  res SMILES strin
+000034b0: 6773 2061 7320 696e 7075 7420 2875 7365  gs as input (use
+000034c0: 2074 6865 2060 6d6f 6c65 6375 6c65 7360   the `molecules`
+000034d0: 2073 7562 7061 636b 6167 6529 207c 0a7c   subpackage) |.|
+000034e0: 2053 7068 6572 6520 4578 636c 7573 696f   Sphere Exclusio
+000034f0: 6e20 7c20 2773 7068 6572 655f 6578 636c  n | 'sphere_excl
+00003500: 7573 696f 6e27 207c 2045 7874 7261 706f  usion' | Extrapo
+00003510: 6c61 7469 7665 207c 2060 6d65 7472 6963  lative | `metric
+00003520: 602c 2060 6469 7374 616e 6365 5f63 7574  `, `distance_cut
+00003530: 6f66 6660 207c 205f 6375 7374 6f6d 2069  off` | _custom i
+00003540: 6d70 6c65 6d65 6e74 6174 696f 6e5f 207c  mplementation_ |
+00003550: 2056 6172 6961 7469 6f6e 206f 6e20 5370   Variation on Sp
+00003560: 6865 7265 2045 7863 6c75 7369 6f6e 2066  here Exclusion f
+00003570: 6f72 2061 7262 6974 7261 7279 2d76 616c  or arbitrary-val
+00003580: 7565 6420 7665 6374 6f72 732e 207c 0a7c  ued vectors. |.|
+00003590: 2054 696d 6520 4261 7365 6420 7c20 2774   Time Based | 't
+000035a0: 696d 655f 6261 7365 6427 207c 2045 7874  ime_based' | Ext
+000035b0: 7261 706f 6c61 7469 7665 207c 205f 6e6f  rapolative | _no
+000035c0: 6e65 5f20 7c20 5061 7065 7273 2075 7369  ne_ | Papers usi
+000035d0: 6e67 2054 696d 6520 6261 7365 6420 7370  ng Time based sp
+000035e0: 6c69 7474 696e 673a 205b 4368 656e 2065  litting: [Chen e
+000035f0: 7420 616c 2e5d 2868 7474 7073 3a2f 2f70  t al.](https://p
+00003600: 7562 732e 6163 732e 6f72 672f 646f 692f  ubs.acs.org/doi/
+00003610: 6675 6c6c 2f31 302e 3130 3231 2f63 6932  full/10.1021/ci2
+00003620: 3030 3631 3568 2920 3a73 6d61 6c6c 5f62  00615h) :small_b
+00003630: 6c75 655f 6469 616d 6f6e 643a 2c20 5b53  lue_diamond:, [S
+00003640: 6865 7269 6461 6e2c 2052 2e20 505d 2868  heridan, R. P](h
+00003650: 7474 7073 3a2f 2f70 7562 732e 6163 732e  ttps://pubs.acs.
+00003660: 6f72 672f 646f 692f 6675 6c6c 2f31 302e  org/doi/full/10.
+00003670: 3130 3231 2f63 6934 3030 3038 346b 2920  1021/ci400084k) 
+00003680: 3a73 6d61 6c6c 5f62 6c75 655f 6469 616d  :small_blue_diam
+00003690: 6f6e 643a 2c20 5b46 6569 6e62 6572 6720  ond:, [Feinberg 
+000036a0: 6574 2061 6c2e 5d28 6874 7470 733a 2f2f  et al.](https://
+000036b0: 7075 6273 2e61 6373 2e6f 7267 2f64 6f69  pubs.acs.org/doi
+000036c0: 2f66 756c 6c2f 3130 2e31 3032 312f 6163  /full/10.1021/ac
+000036d0: 732e 6a6d 6564 6368 656d 2e39 6230 3231  s.jmedchem.9b021
+000036e0: 3837 2920 3a73 6d61 6c6c 5f62 6c75 655f  87) :small_blue_
+000036f0: 6469 616d 6f6e 643a 2c20 5b53 7472 7562  diamond:, [Strub
+00003700: 6c65 2065 7420 616c 2e5d 2868 7474 7073  le et al.](https
+00003710: 3a2f 2f70 7562 732e 7273 632e 6f72 672f  ://pubs.rsc.org/
+00003720: 656e 2f63 6f6e 7465 6e74 2f61 7274 6963  en/content/artic
+00003730: 6c65 6874 6d6c 2f32 3032 302f 7265 2f64  lehtml/2020/re/d
+00003740: 3072 6530 3030 3731 6a29 207c 2054 6869  0re00071j) | Thi
+00003750: 7320 7361 6d70 6c65 7220 7265 7175 6972  s sampler requir
+00003760: 6573 2060 6c61 6265 6c73 6020 746f 2062  es `labels` to b
+00003770: 6520 616e 2069 7465 7261 626c 6520 6f66  e an iterable of
+00003780: 2065 6974 6865 7220 6461 7465 206f 7220   either date or 
+00003790: 6461 7465 7469 6d65 206f 626a 6563 7473  datetime objects
+000037a0: 2e20 7c0a 7c20 4f70 7469 6d69 7a61 626c  . |.| Optimizabl
+000037b0: 6520 4b2d 4469 7373 696d 696c 6172 6974  e K-Dissimilarit
+000037c0: 7920 5365 6c65 6374 696f 6e20 284f 7074  y Selection (Opt
+000037d0: 6953 696d 2920 7c20 276f 7074 6973 696d  iSim) | 'optisim
+000037e0: 2720 7c20 4578 7472 6170 6f6c 6174 6976  ' | Extrapolativ
+000037f0: 6520 7c20 606e 5f63 6c75 7374 6572 7360  e | `n_clusters`
+00003800: 2c20 606d 6178 5f73 7562 7361 6d70 6c65  , `max_subsample
+00003810: 5f73 697a 6560 2c20 6064 6973 7461 6e63  _size`, `distanc
+00003820: 655f 6375 746f 6666 6020 7c20 5f63 7573  e_cutoff` | _cus
+00003830: 746f 6d20 696d 706c 656d 656e 7461 7469  tom implementati
+00003840: 6f6e 5f20 7c20 5661 7269 6174 696f 6e20  on_ | Variation 
+00003850: 6f6e 205b 4f70 7469 5369 6d5d 2868 7474  on [OptiSim](htt
+00003860: 7073 3a2f 2f70 7562 732e 6163 732e 6f72  ps://pubs.acs.or
+00003870: 672f 646f 692f 3130 2e31 3032 312f 6369  g/doi/10.1021/ci
+00003880: 3032 3536 3632 6829 2066 6f72 2061 7262  025662h) for arb
+00003890: 6974 7261 7279 2d76 616c 7565 6420 7665  itrary-valued ve
+000038a0: 6374 6f72 732e 207c 0a7c 204b 2d4d 6561  ctors. |.| K-Mea
+000038b0: 6e73 207c 2027 6b6d 6561 6e73 2720 7c20  ns | 'kmeans' | 
+000038c0: 4578 7472 6170 6f6c 6174 6976 6520 7c20  Extrapolative | 
+000038d0: 606e 5f63 6c75 7374 6572 7360 2c20 606e  `n_clusters`, `n
+000038e0: 5f69 6e69 7460 207c 205b 6073 6b6c 6561  _init` | [`sklea
+000038f0: 726e 204b 4d65 616e 7360 5d28 6874 7470  rn KMeans`](http
+00003900: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
+00003910: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
+00003920: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
+00003930: 6c65 6172 6e2e 636c 7573 7465 722e 4b4d  learn.cluster.KM
+00003940: 6561 6e73 2e68 746d 6c29 207c 2050 6173  eans.html) | Pas
+00003950: 7374 6872 6f75 6768 2074 6f20 6073 6b6c  sthrough to `skl
+00003960: 6561 726e 6027 7320 604b 4d65 616e 7360  earn`'s `KMeans`
+00003970: 2e20 7c0a 7c20 4465 6e73 6974 792d 4261  . |.| Density-Ba
+00003980: 7365 6420 5370 6174 6961 6c20 436c 7573  sed Spatial Clus
+00003990: 7465 7269 6e67 206f 6620 4170 706c 6963  tering of Applic
+000039a0: 6174 696f 6e73 2077 6974 6820 4e6f 6973  ations with Nois
+000039b0: 6520 2844 4253 4341 4e29 207c 2027 6462  e (DBSCAN) | 'db
+000039c0: 7363 616e 2720 7c20 4578 7472 6170 6f6c  scan' | Extrapol
+000039d0: 6174 6976 6520 7c20 6065 7073 602c 2060  ative | `eps`, `
+000039e0: 6d69 6e5f 7361 6d70 6c65 7360 2c20 6061  min_samples`, `a
+000039f0: 6c67 6f72 6974 686d 602c 2060 6d65 7472  lgorithm`, `metr
+00003a00: 6963 602c 2060 6c65 6166 5f73 697a 6560  ic`, `leaf_size`
+00003a10: 207c 205b 6073 6b6c 6561 726e 2044 4253   | [`sklearn DBS
+00003a20: 4341 4e60 5d28 6874 7470 733a 2f2f 7363  CAN`](https://sc
+00003a30: 696b 6974 2d6c 6561 726e 2e6f 7267 2f73  ikit-learn.org/s
+00003a40: 7461 626c 652f 6d6f 6475 6c65 732f 6765  table/modules/ge
+00003a50: 6e65 7261 7465 642f 736b 6c65 6172 6e2e  nerated/sklearn.
+00003a60: 636c 7573 7465 722e 4442 5343 414e 2e68  cluster.DBSCAN.h
+00003a70: 746d 6c29 2044 6f63 756d 656e 7461 7469  tml) Documentati
+00003a80: 6f6e 7c20 5061 7373 7468 726f 7567 6820  on| Passthrough 
+00003a90: 746f 2060 736b 6c65 6172 6e60 2773 2060  to `sklearn`'s `
+00003aa0: 4442 5343 414e 602e 207c 0a7c 204d 696e  DBSCAN`. |.| Min
+00003ab0: 696d 756d 2054 6573 7420 5365 7420 4469  imum Test Set Di
+00003ac0: 7373 696d 696c 6172 6974 7920 284d 5453  ssimilarity (MTS
+00003ad0: 4429 207c 207e 207c 207e 207c 205f 7570  D) | ~ | ~ | _up
+00003ae0: 636f 6d69 6e67 2069 6e5f 2060 6173 7461  coming in_ `asta
+00003af0: 7274 6573 6020 5f76 312e 785f 207c 207e  rtes` _v1.x_ | ~
+00003b00: 207c 207e 207c 0a7c 2052 6573 7472 6963   | ~ |.| Restric
+00003b10: 7465 6420 426f 6c74 7a6d 616e 6e20 4d61  ted Boltzmann Ma
+00003b20: 6368 696e 6520 2852 424d 2920 7c20 7e20  chine (RBM) | ~ 
+00003b30: 7c20 7e20 7c20 5f75 7063 6f6d 696e 6720  | ~ | _upcoming 
+00003b40: 696e 5f20 6061 7374 6172 7465 7360 205f  in_ `astartes` _
+00003b50: 7631 2e78 5f20 7c20 7e20 7c20 7e20 7c0a  v1.x_ | ~ | ~ |.
+00003b60: 7c20 4b6f 686f 6e65 6e20 5365 6c66 2d4f  | Kohonen Self-O
+00003b70: 7267 616e 697a 696e 6720 4d61 7020 2853  rganizing Map (S
+00003b80: 4f4d 2920 7c20 7e20 7c20 7e20 7c20 5f75  OM) | ~ | ~ | _u
+00003b90: 7063 6f6d 696e 6720 696e 5f20 6061 7374  pcoming in_ `ast
+00003ba0: 6172 7465 7360 205f 7631 2e78 5f20 7c20  artes` _v1.x_ | 
+00003bb0: 7e20 7c20 7e20 7c0a 7c20 5350 6c69 7420  ~ | ~ |.| SPlit 
+00003bc0: 4d65 7468 6f64 207c 207e 207c 207e 207c  Method | ~ | ~ |
+00003bd0: 205f 7570 636f 6d69 6e67 2069 6e5f 2060   _upcoming in_ `
+00003be0: 6173 7461 7274 6573 6020 5f76 312e 785f  astartes` _v1.x_
+00003bf0: 207c 207e 207c 207e 207c 0a0a 2323 2320   | ~ | ~ |..### 
+00003c00: 446f 6d61 696e 2d53 7065 6369 6669 6320  Domain-Specific 
+00003c10: 4170 706c 6963 6174 696f 6e73 0a42 656c  Applications.Bel
+00003c20: 6f77 2061 7265 2073 6f6d 6520 6669 656c  ow are some fiel
+00003c30: 6420 7370 6563 6966 6963 2061 7070 6c69  d specific appli
+00003c40: 6361 7469 6f6e 7320 6f66 2060 6173 7461  cations of `asta
+00003c50: 7274 6573 602e 2049 6e74 6572 6573 7465  rtes`. Intereste
+00003c60: 6420 696e 2061 6464 696e 6720 6120 6e65  d in adding a ne
+00003c70: 7720 7361 6d70 6c69 6e67 2061 6c67 6f72  w sampling algor
+00003c80: 6974 686d 206f 7220 6665 6174 7572 697a  ithm or featuriz
+00003c90: 6174 696f 6e20 6170 7072 6f61 6368 3f20  ation approach? 
+00003ca0: 5365 6520 5b60 434f 4e54 5249 4255 5449  See [`CONTRIBUTI
+00003cb0: 4e47 2e6d 6460 5d28 2e2f 434f 4e54 5249  NG.md`](./CONTRI
+00003cc0: 4255 5449 4e47 2e6d 6429 2e0a 0a23 2323  BUTING.md)...###
+00003cd0: 2320 4368 656d 6963 616c 2044 6174 6120  # Chemical Data 
+00003ce0: 616e 6420 7468 6520 6061 7374 6172 7465  and the `astarte
+00003cf0: 732e 6d6f 6c65 6375 6c65 7360 2053 7562  s.molecules` Sub
+00003d00: 7061 636b 6167 650a 4d61 6368 696e 6520  package.Machine 
+00003d10: 4c65 6172 6e69 6e67 2069 7320 656e 6f72  Learning is enor
+00003d20: 6d6f 7573 6c79 2075 7365 6675 6c20 696e  mously useful in
+00003d30: 2063 6865 6d69 7374 7279 2d72 656c 6174   chemistry-relat
+00003d40: 6564 2066 6965 6c64 7320 6475 6520 746f  ed fields due to
+00003d50: 2074 6865 2068 6967 682d 6469 6d65 6e73   the high-dimens
+00003d60: 696f 6e61 6c20 6665 6174 7572 6520 7370  ional feature sp
+00003d70: 6163 6520 6f66 2063 6865 6d69 6361 6c20  ace of chemical 
+00003d80: 6461 7461 2e0a 546f 2070 726f 7065 726c  data..To properl
+00003d90: 7920 6170 706c 7920 4d4c 2074 6f20 6368  y apply ML to ch
+00003da0: 656d 6963 616c 2064 6174 6120 666f 7220  emical data for 
+00003db0: 696e 6665 7265 6e63 6520 5f6f 725f 2064  inference _or_ d
+00003dc0: 6973 636f 7665 7279 2c20 6974 2069 7320  iscovery, it is 
+00003dd0: 696d 706f 7274 616e 7420 746f 206b 6e6f  important to kno
+00003de0: 7720 6120 6d6f 6465 6c27 7320 6163 6375  w a model's accu
+00003df0: 7261 6379 2075 6e64 6572 2074 6865 2074  racy under the t
+00003e00: 776f 2064 6f6d 6169 6e73 2e0a 546f 2073  wo domains..To s
+00003e10: 696d 706c 6966 7920 7468 6520 7072 6f63  implify the proc
+00003e20: 6573 7320 6f66 2070 6172 7469 7469 6f6e  ess of partition
+00003e30: 696e 6720 6368 656d 6963 616c 2064 6174  ing chemical dat
+00003e40: 612c 2060 6173 7461 7274 6573 6020 696d  a, `astartes` im
+00003e50: 706c 656d 656e 7473 2061 2070 7265 2d62  plements a pre-b
+00003e60: 7569 6c74 2066 6561 7475 7269 7a65 7220  uilt featurizer 
+00003e70: 666f 7220 636f 6d6d 6f6e 2063 6865 6d69  for common chemi
+00003e80: 7374 7279 2064 6174 6120 666f 726d 6174  stry data format
+00003e90: 732e 0a41 6674 6572 2069 6e73 7461 6c6c  s..After install
+00003ea0: 696e 6720 7769 7468 2060 7069 7020 696e  ing with `pip in
+00003eb0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
+00003ec0: 6f6c 6563 756c 6573 5d60 206f 6e65 2063  olecules]` one c
+00003ed0: 616e 2069 6d70 6f72 7420 7468 6520 6e65  an import the ne
+00003ee0: 7720 7472 6169 6e2f 7465 7374 2073 706c  w train/test spl
+00003ef0: 6974 7469 6e67 2066 756e 6374 696f 6e20  itting function 
+00003f00: 6c69 6b65 2074 6869 733a 2060 6672 6f6d  like this: `from
+00003f10: 2061 7374 6172 7465 732e 6d6f 6c65 6375   astartes.molecu
+00003f20: 6c65 7320 696d 706f 7274 2074 7261 696e  les import train
+00003f30: 5f74 6573 745f 7370 6c69 745f 6d6f 6c65  _test_split_mole
+00003f40: 6375 6c65 7360 0a0a 5468 6520 7573 6167  cules`..The usag
+00003f50: 6520 6f66 2074 6869 7320 6675 6e63 7469  e of this functi
+00003f60: 6f6e 2069 7320 6964 656e 7469 6361 6c20  on is identical 
+00003f70: 746f 2060 7472 6169 6e5f 7465 7374 5f73  to `train_test_s
+00003f80: 706c 6974 6020 6275 7420 7769 7468 2074  plit` but with t
+00003f90: 6865 2061 6464 6974 696f 6e20 6f66 206e  he addition of n
+00003fa0: 6577 2061 7267 756d 656e 7473 2074 6f20  ew arguments to 
+00003fb0: 636f 6e74 726f 6c20 686f 7720 7468 6520  control how the 
+00003fc0: 6d6f 6c65 6375 6c65 7320 6172 6520 6665  molecules are fe
+00003fd0: 6174 7572 697a 6564 3a0a 0a60 6060 7079  aturized:..```py
+00003fe0: 7468 6f6e 0a74 7261 696e 5f74 6573 745f  thon.train_test_
+00003ff0: 7370 6c69 745f 6d6f 6c65 6375 6c65 7328  split_molecules(
+00004000: 0a20 2020 206d 6f6c 6563 756c 6573 3d73  .    molecules=s
+00004010: 6d69 6c65 732c 0a20 2020 2079 3d79 2c0a  miles,.    y=y,.
+00004020: 2020 2020 7465 7374 5f73 697a 653d 302e      test_size=0.
+00004030: 322c 0a20 2020 2074 7261 696e 5f73 697a  2,.    train_siz
+00004040: 653d 302e 382c 0a20 2020 2066 696e 6765  e=0.8,.    finge
+00004050: 7270 7269 6e74 3d22 6461 796c 6967 6874  rprint="daylight
+00004060: 5f66 696e 6765 7270 7269 6e74 222c 0a20  _fingerprint",. 
+00004070: 2020 2066 7072 696e 7473 5f68 6f70 7473     fprints_hopts
+00004080: 3d7b 0a20 2020 2020 2020 2022 6d69 6e50  ={.        "minP
+00004090: 6174 6822 3a20 322c 0a20 2020 2020 2020  ath": 2,.       
+000040a0: 2022 6d61 7850 6174 6822 3a20 352c 0a20   "maxPath": 5,. 
+000040b0: 2020 2020 2020 2022 6670 5369 7a65 223a         "fpSize":
+000040c0: 2032 3030 2c0a 2020 2020 2020 2020 2262   200,.        "b
+000040d0: 6974 7350 6572 4861 7368 223a 2034 2c0a  itsPerHash": 4,.
+000040e0: 2020 2020 2020 2020 2275 7365 4873 223a          "useHs":
+000040f0: 2031 2c0a 2020 2020 2020 2020 2274 6774   1,.        "tgt
+00004100: 4465 6e73 6974 7922 3a20 302e 342c 0a20  Density": 0.4,. 
+00004110: 2020 2020 2020 2022 6d69 6e53 697a 6522         "minSize"
+00004120: 3a20 3634 2c0a 2020 2020 7d2c 0a20 2020  : 64,.    },.   
+00004130: 2073 616d 706c 6572 3d22 7261 6e64 6f6d   sampler="random
+00004140: 222c 0a20 2020 2072 616e 646f 6d5f 7374  ",.    random_st
+00004150: 6174 653d 3432 2c0a 2020 2020 686f 7074  ate=42,.    hopt
+00004160: 733d 7b0a 2020 2020 2020 2020 2273 6875  s={.        "shu
+00004170: 6666 6c65 223a 2054 7275 652c 0a20 2020  ffle": True,.   
+00004180: 207d 2c0a 290a 6060 600a 0a54 6f20 7365   },.).```..To se
+00004190: 6520 6120 636f 6d70 6c65 7465 2065 7861  e a complete exa
+000041a0: 6d70 6c65 206f 6620 7573 696e 6720 6074  mple of using `t
+000041b0: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
+000041c0: 6d6f 6c65 6375 6c65 7360 2077 6974 6820  molecules` with 
+000041d0: 6163 7475 616c 2063 6865 6d69 6361 6c20  actual chemical 
+000041e0: 6461 7461 2c20 7461 6b65 2061 206c 6f6f  data, take a loo
+000041f0: 6b20 696e 2074 6865 2060 6578 616d 706c  k in the `exampl
+00004200: 6573 6020 6469 7265 6374 6f72 7920 616e  es` directory an
+00004210: 6420 7468 6520 6272 6965 6620 5b63 6f6d  d the brief [com
+00004220: 7061 6e69 6f6e 2070 6170 6572 5d28 6874  panion paper](ht
+00004230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004240: 2f4a 6163 6b73 6f6e 4275 726e 732f 6173  /JacksonBurns/as
+00004250: 7461 7274 6573 2f72 6177 2f6a 6f73 732d  tartes/raw/joss-
+00004260: 7061 7065 722f 4275 726e 732d 5370 6965  paper/Burns-Spie
+00004270: 6b65 726d 616e 6e2d 4268 6174 7461 6368  kermann-Bhattach
+00004280: 6172 6a65 655f 6173 7461 7274 6573 2e70  arjee_astartes.p
+00004290: 6466 292e 0a0a 436f 6e66 6967 7572 6174  df)...Configurat
+000042a0: 696f 6e20 6f70 7469 6f6e 7320 666f 7220  ion options for 
+000042b0: 7468 6520 6665 6174 7572 697a 6174 696f  the featurizatio
+000042c0: 6e20 7363 6865 6d65 2063 616e 2062 6520  n scheme can be 
+000042d0: 666f 756e 6420 696e 2074 6865 2064 6f63  found in the doc
+000042e0: 756d 656e 7461 7469 6f6e 2066 6f72 205b  umentation for [
+000042f0: 4149 4d53 696d 5d28 6874 7470 733a 2f2f  AIMSim](https://
+00004300: 766c 6163 686f 7367 726f 7570 2e67 6974  vlachosgroup.git
+00004310: 6875 622e 696f 2f41 494d 5369 6d2f 5245  hub.io/AIMSim/RE
+00004320: 4144 4d45 2e68 746d 6c23 6375 7272 656e  ADME.html#curren
+00004330: 746c 792d 696d 706c 656d 656e 7465 642d  tly-implemented-
+00004340: 6669 6e67 6572 7072 696e 7473 2920 7468  fingerprints) th
+00004350: 6f75 6768 206d 6f73 7420 6f66 2074 6865  ough most of the
+00004360: 2063 7269 7469 6361 6c20 636f 6e66 6967   critical config
+00004370: 7572 6174 696f 6e20 6f70 7469 6f6e 7320  uration options 
+00004380: 6172 6520 7368 6f77 6e20 6162 6f76 652e  are shown above.
+00004390: 0a0a 2323 2052 6570 726f 6475 6369 6269  ..## Reproducibi
+000043a0: 6c69 7479 0a60 6173 7461 7274 6573 6020  lity.`astartes` 
+000043b0: 6169 6d73 2074 6f20 6265 2063 6f6d 706c  aims to be compl
+000043c0: 6574 656c 7920 7265 7072 6f64 7563 6962  etely reproducib
+000043d0: 6c65 2061 6372 6f73 7320 6469 6666 6572  le across differ
+000043e0: 656e 7420 706c 6174 666f 726d 732c 2050  ent platforms, P
+000043f0: 7974 686f 6e20 7665 7273 696f 6e73 2c20  ython versions, 
+00004400: 616e 6420 6465 7065 6e64 656e 6379 2063  and dependency c
+00004410: 6f6e 6669 6775 7261 7469 6f6e 7320 2d20  onfigurations - 
+00004420: 616e 7920 7665 7273 696f 6e20 6f66 2060  any version of `
+00004430: 6173 7461 7274 6573 6020 7631 2e78 2073  astartes` v1.x s
+00004440: 686f 756c 6420 7265 7375 6c74 2069 6e20  hould result in 
+00004450: 7468 6520 5f65 7861 6374 5f20 7361 6d65  the _exact_ same
+00004460: 2073 706c 6974 732c 2061 6c77 6179 732e   splits, always.
+00004470: 0a54 6f20 7468 6174 2065 6e64 2c20 7468  .To that end, th
+00004480: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
+00004490: 6f72 206f 6620 6061 7374 6172 7465 7360  or of `astartes`
+000044a0: 2069 7320 746f 2075 7365 2060 3432 6020   is to use `42` 
+000044b0: 6173 2074 6865 2072 616e 646f 6d20 7365  as the random se
+000044c0: 6564 2061 6e64 205f 616c 7761 7973 5f20  ed and _always_ 
+000044d0: 7365 7420 6974 2e0a 5275 6e6e 696e 6720  set it..Running 
+000044e0: 6061 7374 6172 7465 7360 2077 6974 6820  `astartes` with 
+000044f0: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
+00004500: 696e 6773 2077 696c 6c20 616c 7761 7973  ings will always
+00004510: 2070 726f 6475 6365 2074 6865 2065 7861   produce the exa
+00004520: 6374 2073 616d 6520 7265 7375 6c74 732e  ct same results.
+00004530: 0a57 6520 6861 7665 2076 6572 6966 6965  .We have verifie
+00004540: 6420 7468 6973 2062 6568 6176 696f 7220  d this behavior 
+00004550: 6f6e 2044 6562 6961 6e20 5562 756e 7475  on Debian Ubuntu
+00004560: 2c20 5769 6e64 6f77 732c 2061 6e64 2049  , Windows, and I
+00004570: 6e74 656c 204d 6163 7320 6672 6f6d 2050  ntel Macs from P
+00004580: 7974 686f 6e20 7665 7273 696f 6e73 2033  ython versions 3
+00004590: 2e37 2074 6872 6f75 6768 2033 2e31 3120  .7 through 3.11 
+000045a0: 2877 6974 6820 6170 7072 6f70 7269 6174  (with appropriat
+000045b0: 6520 6465 7065 6e64 656e 6369 6573 2066  e dependencies f
+000045c0: 6f72 2065 6163 6820 7665 7273 696f 6e29  or each version)
+000045d0: 2e0a 0a23 2323 204b 6e6f 776e 2052 6570  ...### Known Rep
+000045e0: 726f 6475 6369 6269 6c69 7479 204c 696d  roducibility Lim
+000045f0: 6974 6174 696f 6e73 0a49 6e65 7669 7461  itations.Inevita
+00004600: 626c 7920 6578 7465 726e 616c 2064 6570  bly external dep
+00004610: 656e 6465 6e63 6965 7320 6f66 2060 6173  endencies of `as
+00004620: 7461 7274 6573 6020 7769 6c6c 2069 6e74  tartes` will int
+00004630: 726f 6475 6365 2062 6163 6b77 6172 6473  roduce backwards
+00004640: 2d69 6e63 6f6d 7061 7469 626c 6520 6368  -incompatible ch
+00004650: 616e 6765 732e 0a57 6520 636f 6e74 696e  anges..We contin
+00004660: 7561 6c6c 7920 7275 6e20 7265 6772 6573  ually run regres
+00004670: 7369 6f6e 2074 6573 7473 2074 6f20 6361  sion tests to ca
+00004680: 7463 6820 7468 6573 652c 2061 6e64 2077  tch these, and w
+00004690: 696c 6c20 6c69 7374 2061 6c6c 205f 6b6e  ill list all _kn
+000046a0: 6f77 6e5f 206c 696d 6974 6174 696f 6e73  own_ limitations
+000046b0: 2068 6572 653a 0a20 2d20 6073 6b6c 6561   here:. - `sklea
+000046c0: 726e 6020 7631 2e33 2e30 2069 6e74 726f  rn` v1.3.0 intro
+000046d0: 6475 6365 6420 6261 636b 7761 7264 732d  duced backwards-
+000046e0: 696e 636f 6d70 6174 6962 6c65 2063 6861  incompatible cha
+000046f0: 6e67 6573 2069 6e20 7468 6520 604b 4d65  nges in the `KMe
+00004700: 616e 7360 2073 616d 706c 6572 2074 6861  ans` sampler tha
+00004710: 7420 6368 616e 6765 6420 686f 7720 7468  t changed how th
+00004720: 6520 7261 6e64 6f6d 2069 6e69 7469 616c  e random initial
+00004730: 697a 6174 696f 6e20 6166 6665 6374 7320  ization affects 
+00004740: 7468 6520 7265 7375 6c74 732c 2065 7665  the results, eve
+00004750: 6e20 6769 7665 6e20 7468 6520 7361 6d65  n given the same
+00004760: 2072 616e 646f 6d20 7365 6564 2e20 4469   random seed. Di
+00004770: 6666 6572 656e 7420 7665 7273 696f 6e20  fferent version 
+00004780: 6f66 2060 736b 6c65 6172 6e60 2077 696c  of `sklearn` wil
+00004790: 6c20 6166 6665 6374 2074 6865 2070 6572  l affect the per
+000047a0: 666f 726d 616e 6365 206f 6620 6061 7374  formance of `ast
+000047b0: 6172 7465 7360 2061 6e64 2077 6520 7265  artes` and we re
+000047c0: 636f 6d6d 656e 6420 696e 636c 7564 696e  commend includin
+000047d0: 6720 7468 6520 6578 6163 7420 7665 7273  g the exact vers
+000047e0: 696f 6e20 6f66 2060 7363 696b 6974 2d6c  ion of `scikit-l
+000047f0: 6561 726e 6020 616e 6420 6061 7374 6172  earn` and `astar
+00004800: 7465 7360 2075 7365 642c 2077 6865 6e20  tes` used, when 
+00004810: 6170 706c 6963 6162 6c65 2e0a 0a3e 202a  applicable...> *
+00004820: 2a4e 6f74 652a 2a0a 3e20 5765 2061 7265  *Note**.> We are
+00004830: 206c 696d 6974 6564 2069 6e20 6f75 7220   limited in our 
+00004840: 6162 696c 6974 7920 746f 2074 6573 7420  ability to test 
+00004850: 6f6e 204d 3120 4d61 6373 2c20 6275 7420  on M1 Macs, but 
+00004860: 6672 6f6d 206f 7572 206c 696d 6974 6564  from our limited
+00004870: 206d 616e 7561 6c20 7465 7374 696e 6720   manual testing 
+00004880: 7765 2061 6368 6965 7665 2070 6572 6665  we achieve perfe
+00004890: 6374 2072 6570 726f 6475 6362 696c 6974  ct reproducbilit
+000048a0: 7920 696e 2061 6c6c 2063 6173 6573 205f  y in all cases _
+000048b0: 6578 6365 7074 206f 6363 6173 696f 6e61  except occasiona
+000048c0: 6c6c 795f 2077 6974 6820 604b 4d65 616e  lly_ with `KMean
+000048d0: 7360 206f 6e20 4170 706c 6520 7369 6c69  s` on Apple sili
+000048e0: 636f 6e2e 0a60 6173 7461 7274 6573 6020  con..`astartes` 
+000048f0: 6973 2073 7469 6c6c 2063 6f6e 7369 7374  is still consist
+00004900: 656e 7420 6265 7477 6565 6e20 7275 6e73  ent between runs
+00004910: 206f 6e20 7468 6520 7361 6d65 2070 6c61   on the same pla
+00004920: 7466 6f72 6d20 696e 2061 6c6c 2063 6173  tform in all cas
+00004930: 6573 2c20 616e 6420 6f74 6865 7220 7361  es, and other sa
+00004940: 6d70 6c65 7273 2061 7265 206e 6f74 2069  mplers are not i
+00004950: 6d70 6163 7465 6420 6279 2074 6869 7320  mpacted by this 
+00004960: 6170 7061 7265 6e74 2062 7567 2e0a 0a23  apparent bug...#
+00004970: 2320 486f 7720 746f 2043 6974 650a 4966  # How to Cite.If
+00004980: 2079 6f75 2075 7365 2060 6173 7461 7274   you use `astart
+00004990: 6573 6020 696e 2079 6f75 7220 776f 726b  es` in your work
+000049a0: 2070 6c65 6173 6520 7573 6520 7468 6520   please use the 
+000049b0: 6265 6c6f 7720 6369 7461 7469 6f6e 206f  below citation o
+000049c0: 7220 7468 6520 2243 6974 6520 7468 6973  r the "Cite this
+000049d0: 2072 6570 6f73 6974 6f72 7922 2062 7574   repository" but
+000049e0: 746f 6e20 6f6e 2047 6974 4875 623a 0a3e  ton on GitHub:.>
+000049f0: 202a 2a42 6962 5465 582a 2a0a 3e20 4073   **BibTeX**.> @s
+00004a00: 6f66 7477 6172 657b 6275 726e 735f 6a61  oftware{burns_ja
+00004a10: 636b 736f 6e5f 3230 3233 5f38 3134 3732  ckson_2023_81472
+00004a20: 3035 2c0a 3e20 2020 6175 7468 6f72 2020  05,.>   author  
+00004a30: 2020 2020 203d 207b 4275 726e 732c 204a       = {Burns, J
+00004a40: 6163 6b73 6f6e 2061 6e64 0a3e 2020 2020  ackson and.>    
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00004a60: 7069 656b 6572 6d61 6e6e 2c20 4b65 7669  piekermann, Kevi
+00004a70: 6e20 616e 640a 3e20 2020 2020 2020 2020  n and.>         
+00004a80: 2020 2020 2020 2020 2020 4268 6174 7461            Bhatta
+00004a90: 6368 6172 6a65 652c 2048 696d 6167 686e  charjee, Himaghn
+00004aa0: 6120 616e 640a 3e20 2020 2020 2020 2020  a and.>         
+00004ab0: 2020 2020 2020 2020 2020 566c 6163 686f            Vlacho
+00004ac0: 732c 2044 696f 6e69 7369 6f73 2061 6e64  s, Dionisios and
+00004ad0: 0a3e 2020 2020 2020 2020 2020 2020 2020  .>              
+00004ae0: 2020 2020 2047 7265 656e 2c20 5769 6c6c       Green, Will
+00004af0: 6961 6d7d 2c0a 3e20 2020 7469 746c 6520  iam},.>   title 
+00004b00: 2020 2020 2020 203d 207b 7b4d 6163 6869         = {{Machi
+00004b10: 6e65 204c 6561 726e 696e 6720 5661 6c69  ne Learning Vali
+00004b20: 6461 7469 6f6e 2076 6961 2052 6174 696f  dation via Ratio
+00004b30: 6e61 6c20 4461 7461 7365 7420 0a3e 2020  nal Dataset .>  
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 5361 6d70 6c69 6e67 2077 6974 6820    Sampling with 
+00004b60: 6173 7461 7274 6573 7d7d 2c0a 3e20 2020  astartes}},.>   
+00004b70: 6d6f 6e74 6820 2020 2020 2020 203d 206d  month        = m
+00004b80: 6179 2c0a 3e20 2020 7965 6172 2020 2020  ay,.>   year    
+00004b90: 2020 2020 203d 2032 3032 332c 0a3e 2020       = 2023,.>  
+00004ba0: 2070 7562 6c69 7368 6572 2020 2020 3d20   publisher    = 
+00004bb0: 7b5a 656e 6f64 6f7d 2c0a 3e20 2020 7665  {Zenodo},.>   ve
+00004bc0: 7273 696f 6e20 2020 2020 203d 207b 312e  rsion      = {1.
+00004bd0: 312e 317d 2c0a 3e20 2020 646f 6920 2020  1.1},.>   doi   
+00004be0: 2020 2020 2020 203d 207b 3130 2e35 3238         = {10.528
+00004bf0: 312f 7a65 6e6f 646f 2e38 3134 3732 3035  1/zenodo.8147205
+00004c00: 7d2c 0a3e 2020 2075 726c 2020 2020 2020  },.>   url      
+00004c10: 2020 2020 3d20 7b68 7474 7073 3a2f 2f64      = {https://d
+00004c20: 6f69 2e6f 7267 2f31 302e 3532 3831 2f7a  oi.org/10.5281/z
+00004c30: 656e 6f64 6f2e 3831 3437 3230 357d 0a3e  enodo.8147205}.>
+00004c40: 207d 0a0a 2323 2043 6f6e 7472 6962 7574   }..## Contribut
+00004c50: 696e 6720 2620 4465 7665 6c6f 7065 7220  ing & Developer 
+00004c60: 4e6f 7465 730a 5365 6520 5b43 4f4e 5452  Notes.See [CONTR
+00004c70: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
+00004c80: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00004c90: 6f72 2069 6e73 7472 7563 7469 6f6e 7320  or instructions 
+00004ca0: 6f6e 2069 6e73 7461 6c6c 696e 6720 6061  on installing `a
+00004cb0: 7374 6172 7465 7360 2066 6f72 2064 6576  startes` for dev
+00004cc0: 656c 6f70 6d65 6e74 2c20 6d61 6b69 6e67  elopment, making
+00004cd0: 2061 2063 6f6e 7472 6962 7574 696f 6e2c   a contribution,
+00004ce0: 2061 6e64 2067 656e 6572 616c 2067 7569   and general gui
+00004cf0: 6461 6e63 6520 6f6e 2074 6865 2064 6573  dance on the des
+00004d00: 6967 6e20 6f66 2060 6173 7461 7274 6573  ign of `astartes
+00004d10: 602e 0a0a                                `...
```

### Comparing `astartes-1.1.1/README.md` & `astartes-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -66,1179 +66,1123 @@
 00000410: 2f2f 6769 7468 7562 2e63 6f6d 2f4a 6163  //github.com/Jac
 00000420: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
 00000430: 6573 2f61 6374 696f 6e73 2f77 6f72 6b66  es/actions/workf
 00000440: 6c6f 7773 2f72 6570 726f 6475 6365 5f70  lows/reproduce_p
 00000450: 6170 6572 2e79 6d6c 2f62 6164 6765 2e73  aper.yml/badge.s
 00000460: 7667 3f62 7261 6e63 683d 6d61 696e 2665  vg?branch=main&e
 00000470: 7665 6e74 3d73 6368 6564 756c 6522 3e0a  vent=schedule">.
-00000480: 3c2f 703e 0a0a 2323 2049 6e73 7461 6c6c  </p>..## Install
-00000490: 696e 6720 6061 7374 6172 7465 7360 0a57  ing `astartes`.W
-000004a0: 6520 7265 636f 6d6d 656e 6420 696e 7374  e recommend inst
-000004b0: 616c 6c69 6e67 2060 6173 7461 7274 6573  alling `astartes
-000004c0: 6020 7769 7468 696e 2061 2076 6972 7475  ` within a virtu
-000004d0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2c20  al environment, 
-000004e0: 7573 696e 6720 6569 7468 6572 2060 7665  using either `ve
-000004f0: 6e76 6020 6f72 2060 636f 6e64 6160 2028  nv` or `conda` (
-00000500: 6f72 206f 7468 6572 2074 6f6f 6c73 2920  or other tools) 
-00000510: 746f 2073 696d 706c 6966 7920 6465 7065  to simplify depe
-00000520: 6e64 656e 6379 206d 616e 6167 656d 656e  ndency managemen
-00000530: 742e 2050 7974 686f 6e20 7665 7273 696f  t. Python versio
-00000540: 6e73 2033 2e37 2c20 332e 382c 2033 2e39  ns 3.7, 3.8, 3.9
-00000550: 2c20 332e 3130 2c20 616e 6420 332e 3131  , 3.10, and 3.11
-00000560: 2061 7265 2073 7570 706f 7274 6564 206f   are supported o
-00000570: 6e20 616c 6c20 706c 6174 666f 726d 732e  n all platforms.
-00000580: 0a0a 6061 7374 6172 7465 7360 2069 7320  ..`astartes` is 
-00000590: 6176 6169 6c61 626c 6520 6f6e 2060 5079  available on `Py
-000005a0: 5049 6020 616e 6420 6361 6e20 6265 2069  PI` and can be i
-000005b0: 6e73 7461 6c6c 6564 2075 7369 6e67 2060  nstalled using `
-000005c0: 7069 7060 3a0a 0a20 2d20 546f 2069 6e63  pip`:.. - To inc
-000005d0: 6c75 6465 2074 6865 2066 6561 7475 7269  lude the featuri
-000005e0: 7a61 7469 6f6e 206f 7074 696f 6e73 2066  zation options f
-000005f0: 6f72 2063 6865 6d69 6361 6c20 6461 7461  or chemical data
-00000600: 2c20 7573 6520 6070 6970 2069 6e73 7461  , use `pip insta
-00000610: 6c6c 2061 7374 6172 7465 735b 6d6f 6c65  ll astartes[mole
-00000620: 6375 6c65 735d 602e 0a20 2d20 546f 2069  cules]`.. - To i
-00000630: 6e73 7461 6c6c 206f 6e6c 7920 7468 6520  nstall only the 
-00000640: 7361 6d70 6c69 6e67 2061 6c67 6f72 6974  sampling algorit
-00000650: 686d 732c 2075 7365 2060 7069 7020 696e  hms, use `pip in
-00000660: 7374 616c 6c20 6173 7461 7274 6573 6020  stall astartes` 
-00000670: 2874 6869 7320 696e 7374 616c 6c20 7769  (this install wi
-00000680: 6c6c 2068 6176 6520 6665 7765 7220 6465  ll have fewer de
-00000690: 7065 6e64 656e 6369 6573 2061 6e64 206d  pendencies and m
-000006a0: 6179 2062 6520 6d6f 7265 2072 6561 6469  ay be more readi
-000006b0: 6c79 2063 6f6d 7061 7469 626c 6520 696e  ly compatible in
-000006c0: 2065 6e76 6972 6f6e 6d65 6e74 7320 7769   environments wi
-000006d0: 7468 2065 7869 7374 696e 6720 776f 726b  th existing work
-000006e0: 666c 6f77 7329 2e0a 0a54 6865 2062 6173  flows)...The bas
-000006f0: 6520 6061 7374 6172 7465 7360 2070 6163  e `astartes` pac
-00000700: 6b61 6765 2069 7320 616c 736f 2061 7661  kage is also ava
-00000710: 696c 6162 6c65 206f 6e20 6063 6f6e 6461  ilable on `conda
-00000720: 6020 7769 7468 2074 6869 7320 636f 6d6d  ` with this comm
-00000730: 616e 643a 2060 636f 6e64 6120 696e 7374  and: `conda inst
-00000740: 616c 6c20 2d63 206a 6163 6b73 6f6e 6275  all -c jacksonbu
-00000750: 726e 7320 6173 7461 7274 6573 602e 0a4e  rns astartes`..N
-00000760: 6f74 6520 7468 6174 2074 6869 7320 7061  ote that this pa
-00000770: 636b 6167 6520 5f64 6f65 7320 6e6f 745f  ckage _does not_
-00000780: 2069 6e63 6c75 6465 2062 7569 6c74 2d69   include built-i
-00000790: 6e20 7375 7070 6f72 7420 666f 7220 6665  n support for fe
-000007a0: 6174 7572 697a 696e 6720 6d6f 6c65 6375  aturizing molecu
-000007b0: 6c65 732c 2077 6869 6368 2069 7320 6375  les, which is cu
-000007c0: 7272 656e 746c 7920 6f6e 6c79 2061 7661  rrently only ava
-000007d0: 696c 6162 6c65 2066 726f 6d20 7468 6520  ilable from the 
-000007e0: 5079 5049 2070 6163 6b61 6765 206f 7220  PyPI package or 
-000007f0: 6120 736f 7572 6365 2069 6e73 7461 6c6c  a source install
-00000800: 2e0a 0a3e 202a 2a4e 6f74 652a 2a0a 3e20  ...> **Note**.> 
-00000810: 5769 6e64 6f77 7320 506f 7765 7273 6865  Windows Powershe
-00000820: 6c6c 2061 6e64 204d 6163 4f53 2043 6174  ll and MacOS Cat
-00000830: 616c 696e 6120 6f72 206e 6577 6572 206d  alina or newer m
-00000840: 6179 2063 6f6d 706c 6169 6e20 6162 6f75  ay complain abou
-00000850: 7420 7371 7561 7265 2062 7261 636b 6574  t square bracket
-00000860: 732c 2073 6f20 796f 7520 7769 6c6c 206e  s, so you will n
-00000870: 6565 6420 746f 2064 6f75 626c 6520 7175  eed to double qu
-00000880: 6f74 6520 7468 6520 606d 6f6c 6563 756c  ote the `molecul
-00000890: 6573 6020 636f 6d6d 616e 6420 2869 2e65  es` command (i.e
-000008a0: 2e20 6070 6970 2069 6e73 7461 6c6c 2022  . `pip install "
-000008b0: 6173 7461 7274 6573 5b6d 6f6c 6563 756c  astartes[molecul
-000008c0: 6573 5d22 6029 0a0a 546f 2069 6e73 7461  es]"`)..To insta
-000008d0: 6c6c 2060 6173 7461 7274 6573 6020 6672  ll `astartes` fr
-000008e0: 6f6d 2073 6f75 7263 652c 2073 6565 2074  om source, see t
-000008f0: 6865 205b 436f 6e74 7269 6275 7469 6e67  he [Contributing
-00000900: 2026 2044 6576 656c 6f70 6572 204e 6f74   & Developer Not
-00000910: 6573 5d28 2363 6f6e 7472 6962 7574 696e  es](#contributin
-00000920: 672d 2d64 6576 656c 6f70 6572 2d6e 6f74  g--developer-not
-00000930: 6573 2920 7365 6374 696f 6e2e 0a0a 2323  es) section...##
-00000940: 2055 7369 6e67 2060 6173 7461 7274 6573   Using `astartes
-00000950: 600a 6061 7374 6172 7465 7360 2069 7320  `.`astartes` is 
-00000960: 6465 7369 676e 6564 2061 7320 6120 6472  designed as a dr
-00000970: 6f70 2d69 6e20 7265 706c 6163 656d 656e  op-in replacemen
-00000980: 7420 666f 7220 6073 6b6c 6561 726e 6027  t for `sklearn`'
-00000990: 7320 6074 7261 696e 5f74 6573 745f 7370  s `train_test_sp
-000009a0: 6c69 7460 2066 756e 6374 696f 6e2e 2054  lit` function. T
-000009b0: 6f20 7377 6974 6368 2074 6f20 6061 7374  o switch to `ast
-000009c0: 6172 7465 7360 2c20 6368 616e 6765 2060  artes`, change `
-000009d0: 6672 6f6d 2073 6b6c 6561 726e 2e6d 6f64  from sklearn.mod
-000009e0: 656c 5f73 656c 6563 7469 6f6e 2069 6d70  el_selection imp
-000009f0: 6f72 7420 7472 6169 6e5f 7465 7374 5f73  ort train_test_s
-00000a00: 706c 6974 6020 746f 2060 6672 6f6d 2061  plit` to `from a
-00000a10: 7374 6172 7465 7320 696d 706f 7274 2074  startes import t
-00000a20: 7261 696e 5f74 6573 745f 7370 6c69 7460  rain_test_split`
-00000a30: 2e0a 0a4c 696b 6520 6073 6b6c 6561 726e  ...Like `sklearn
-00000a40: 602c 2060 6173 7461 7274 6573 6020 6163  `, `astartes` ac
-00000a50: 6365 7074 7320 616e 7920 6974 6572 6162  cepts any iterab
-00000a60: 6c65 206f 626a 6563 7420 6173 2060 5860  le object as `X`
-00000a70: 2c20 6079 602c 2061 6e64 2060 6c61 6265  , `y`, and `labe
-00000a80: 6c73 602e 0a45 6163 6820 7769 6c6c 2062  ls`..Each will b
-00000a90: 6520 636f 6e76 6572 7465 6420 746f 2061  e converted to a
-00000aa0: 2060 6e75 6d70 7960 2061 7272 6179 2066   `numpy` array f
-00000ab0: 6f72 2069 6e74 6572 6e61 6c20 6f70 6572  or internal oper
-00000ac0: 6174 696f 6e73 2c20 616e 6420 7265 7475  ations, and retu
-00000ad0: 726e 6564 2061 7320 6120 606e 756d 7079  rned as a `numpy
-00000ae0: 6020 6172 7261 7920 7769 7468 206c 696d  ` array with lim
-00000af0: 6974 6564 2065 7863 6570 7469 6f6e 733a  ited exceptions:
-00000b00: 2069 6620 6058 6020 6973 2061 2060 7061   if `X` is a `pa
-00000b10: 6e64 6173 6020 6044 6174 6146 7261 6d65  ndas` `DataFrame
-00000b20: 602c 2060 7960 2069 7320 6120 6053 6572  `, `y` is a `Ser
-00000b30: 6965 7360 2c20 6f72 2060 6c61 6265 6c73  ies`, or `labels
-00000b40: 6020 6973 2061 2060 5365 7269 6573 602c  ` is a `Series`,
-00000b50: 2060 6173 7461 7274 6573 6020 7769 6c6c   `astartes` will
-00000b60: 2063 6173 7420 6974 2062 6163 6b20 746f   cast it back to
-00000b70: 2069 7473 206f 7269 6769 6e61 6c20 7479   its original ty
-00000b80: 7065 2069 6e63 6c75 6469 6e67 2069 7473  pe including its
-00000b90: 2069 6e64 6578 2061 6e64 2063 6f6c 756d   index and colum
-00000ba0: 6e20 6e61 6d65 732e 0a0a 3e20 2a2a 4e6f  n names...> **No
-00000bb0: 7465 2a2a 0a3e 2054 6865 2064 6576 656c  te**.> The devel
-00000bc0: 6f70 6572 7320 7265 636f 6d6d 656e 6420  opers recommend 
-00000bd0: 7061 7373 696e 6720 6058 602c 2060 7960  passing `X`, `y`
-00000be0: 2c20 616e 6420 606c 6162 656c 7360 2061  , and `labels` a
-00000bf0: 7320 606e 756d 7079 6020 6172 7261 7973  s `numpy` arrays
-00000c00: 2061 6e64 2068 616e 646c 696e 6720 7468   and handling th
-00000c10: 6520 636f 6e76 6572 7369 6f6e 2074 6f20  e conversion to 
-00000c20: 616e 6420 6672 6f6d 206f 7468 6572 2074  and from other t
-00000c30: 7970 6573 2065 7870 6c69 6369 7479 206f  ypes explicity o
-00000c40: 6e20 796f 7572 206f 776e 2e20 4265 6869  n your own. Behi
-00000c50: 6e64 2d74 6865 2d73 6365 6e65 7320 7479  nd-the-scenes ty
-00000c60: 7065 2063 6173 7469 6e67 2063 616e 206c  pe casting can l
-00000c70: 6561 6420 746f 2075 6e65 7870 6563 7465  ead to unexpecte
-00000c80: 6420 6265 6861 7669 6f72 210a 0a42 7920  d behavior!..By 
-00000c90: 6465 6661 756c 742c 2060 6173 7461 7274  default, `astart
-00000ca0: 6573 6020 7769 6c6c 2073 706c 6974 2064  es` will split d
-00000cb0: 6174 6120 7261 6e64 6f6d 6c79 2e20 4164  ata randomly. Ad
-00000cc0: 6469 7469 6f6e 616c 6c79 2c20 6120 7661  ditionally, a va
-00000cd0: 7269 6574 7920 6f66 2061 6c67 6f72 6974  riety of algorit
-00000ce0: 686d 6963 2073 616d 706c 696e 6720 6170  hmic sampling ap
-00000cf0: 7072 6f61 6368 6573 2063 616e 2062 6520  proaches can be 
-00000d00: 7573 6564 2062 7920 7370 6563 6966 7969  used by specifyi
-00000d10: 6e67 2074 6865 2060 7361 6d70 6c65 7260  ng the `sampler`
-00000d20: 2061 7267 756d 656e 7420 746f 2074 6865   argument to the
-00000d30: 2066 756e 6374 696f 6e3a 0a0a 6060 6070   function:..```p
-00000d40: 7974 686f 6e0a 585f 7472 6169 6e2c 2058  ython.X_train, X
-00000d50: 5f74 6573 742c 2079 5f74 7261 696e 2c20  _test, y_train, 
-00000d60: 795f 7465 7374 203d 2074 7261 696e 5f74  y_test = train_t
-00000d70: 6573 745f 7370 6c69 7428 0a20 2058 2c20  est_split(.  X, 
-00000d80: 2023 2070 7265 6665 7261 626c 7920 6e75   # preferably nu
-00000d90: 6d70 7920 6172 7261 7973 2c20 6275 7420  mpy arrays, but 
-00000da0: 6173 7461 7274 6573 2077 696c 6c20 6361  astartes will ca
-00000db0: 7374 2069 7420 666f 7220 796f 750a 2020  st it for you.  
-00000dc0: 792c 0a20 2073 616d 706c 6572 203d 2027  y,.  sampler = '
-00000dd0: 6b65 6e6e 6172 645f 7374 6f6e 6527 2c20  kennard_stone', 
-00000de0: 2023 2061 6e79 206f 6620 7468 6520 7375   # any of the su
-00000df0: 7070 6f72 7465 6420 7361 6d70 6c65 7273  pported samplers
-00000e00: 0a29 0a60 6060 0a0a 2323 2320 5061 7065  .).```..### Pape
-00000e10: 720a 466f 7220 6120 636f 6d70 7265 6865  r.For a comprehe
-00000e20: 6e73 6976 6520 7761 6c6b 7468 726f 7567  nsive walkthroug
-00000e30: 6820 6f66 2074 6865 2074 6865 6f72 7920  h of the theory 
-00000e40: 616e 6420 696d 706c 656d 656e 7461 7469  and implementati
-00000e50: 6f6e 206f 6620 6061 7374 6172 7465 7360  on of `astartes`
-00000e60: 2c20 666f 6c6c 6f77 205b 7468 6973 206c  , follow [this l
-00000e70: 696e 6b5d 2868 7474 7073 3a2f 2f67 6974  ink](https://git
-00000e80: 6875 622e 636f 6d2f 4a61 636b 736f 6e42  hub.com/JacksonB
-00000e90: 7572 6e73 2f61 7374 6172 7465 732f 7261  urns/astartes/ra
-00000ea0: 772f 6a6f 7373 2d70 6170 6572 2f42 7572  w/joss-paper/Bur
-00000eb0: 6e73 2d53 7069 656b 6572 6d61 6e6e 2d42  ns-Spiekermann-B
-00000ec0: 6861 7474 6163 6861 726a 6565 5f61 7374  hattacharjee_ast
-00000ed0: 6172 7465 732e 7064 6629 2074 6f20 7265  artes.pdf) to re
-00000ee0: 6164 2074 6865 2063 6f6d 7061 6e69 6f6e  ad the companion
-00000ef0: 2070 6170 6572 2e0a 0a23 2323 2045 7861   paper...### Exa
-00000f00: 6d70 6c65 204e 6f74 6562 6f6f 6b73 0a0a  mple Notebooks..
-00000f10: 436c 6963 6b20 7468 6520 6261 6467 6573  Click the badges
-00000f20: 2069 6e20 7468 6520 7461 626c 6520 6265   in the table be
-00000f30: 6c6f 7720 746f 2062 6520 7461 6b65 6e20  low to be taken 
-00000f40: 746f 2061 206c 6976 652c 2069 6e74 6572  to a live, inter
-00000f50: 6163 7469 7665 2064 656d 6f20 6f66 2060  active demo of `
-00000f60: 6173 7461 7274 6573 603a 0a0a 7c20 4465  astartes`:..| De
-00000f70: 6d6f 207c 204c 696e 6b20 7c0a 7c3a 2d2d  mo | Link |.|:--
-00000f80: 2d3a 7c2d 2d2d 7c0a 7c20 5573 696e 6720  -:|---|.| Using 
-00000f90: 6074 7261 696e 5f76 616c 5f74 6573 745f  `train_val_test_
-00000fa0: 7370 6c69 7460 2077 6974 6820 7468 6520  split` with the 
-00000fb0: 6073 6b6c 6561 726e 6020 6578 616d 706c  `sklearn` exampl
-00000fc0: 6520 6461 7461 7365 7473 207c 205b 215b  e datasets | [![
-00000fd0: 4269 6e64 6572 5d28 6874 7470 733a 2f2f  Binder](https://
-00000fe0: 6d79 6269 6e64 6572 2e6f 7267 2f62 6164  mybinder.org/bad
-00000ff0: 6765 5f6c 6f67 6f2e 7376 6729 5d28 6874  ge_logo.svg)](ht
-00001000: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
-00001010: 7267 2f76 322f 6768 2f4a 6163 6b73 6f6e  rg/v2/gh/Jackson
-00001020: 4275 726e 732f 6173 7461 7274 6573 2f6d  Burns/astartes/m
-00001030: 6169 6e3f 6c61 6270 6174 683d 6578 616d  ain?labpath=exam
-00001040: 706c 6573 2532 4674 7261 696e 5f76 616c  ples%2Ftrain_val
-00001050: 5f74 6573 745f 7370 6c69 745f 736b 6c65  _test_split_skle
-00001060: 6172 6e5f 6578 616d 706c 6525 3246 7472  arn_example%2Ftr
-00001070: 6169 6e5f 7661 6c5f 7465 7374 5f73 706c  ain_val_test_spl
-00001080: 6974 5f65 7861 6d70 6c65 2e69 7079 6e62  it_example.ipynb
-00001090: 2920 7c0a 7c20 436f 6d70 6172 696e 6720  ) |.| Comparing 
-000010a0: 5361 6d70 6c69 6e67 2041 6c67 6f72 6974  Sampling Algorit
-000010b0: 686d 7320 7769 7468 2046 6173 7420 466f  hms with Fast Fo
-000010c0: 6f64 207c 205b 215b 4269 6e64 6572 5d28  od | [![Binder](
-000010d0: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-000010e0: 2e6f 7267 2f62 6164 6765 5f6c 6f67 6f2e  .org/badge_logo.
-000010f0: 7376 6729 5d28 6874 7470 733a 2f2f 6d79  svg)](https://my
-00001100: 6269 6e64 6572 2e6f 7267 2f76 322f 6768  binder.org/v2/gh
-00001110: 2f4a 6163 6b73 6f6e 4275 726e 732f 6173  /JacksonBurns/as
-00001120: 7461 7274 6573 2f6d 6169 6e3f 6c61 6270  tartes/main?labp
-00001130: 6174 683d 6578 616d 706c 6573 2532 4673  ath=examples%2Fs
-00001140: 706c 6974 5f63 6f6d 7061 7269 736f 6e73  plit_comparisons
-00001150: 2532 4673 706c 6974 5f63 6f6d 7061 7269  %2Fsplit_compari
-00001160: 736f 6e73 2e69 7079 6e62 2920 7c0a 7c20  sons.ipynb) |.| 
-00001170: 4368 656d 696e 666f 726d 6174 6963 7320  Cheminformatics 
-00001180: 7361 6d70 6c65 2073 6574 2070 6172 7469  sample set parti
-00001190: 7469 6f6e 696e 6720 7769 7468 2060 6173  tioning with `as
-000011a0: 7461 7274 6573 6020 7c20 5b21 5b42 696e  tartes` | [![Bin
-000011b0: 6465 725d 2868 7474 7073 3a2f 2f6d 7962  der](https://myb
-000011c0: 696e 6465 722e 6f72 672f 6261 6467 655f  inder.org/badge_
-000011d0: 6c6f 676f 2e73 7667 295d 2868 7474 7073  logo.svg)](https
-000011e0: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-000011f0: 7632 2f67 682f 4a61 636b 736f 6e42 7572  v2/gh/JacksonBur
-00001200: 6e73 2f61 7374 6172 7465 732f 6d61 696e  ns/astartes/main
-00001210: 3f6c 6162 7061 7468 3d65 7861 6d70 6c65  ?labpath=example
-00001220: 7325 3246 6261 7272 6965 725f 7072 6564  s%2Fbarrier_pred
-00001230: 6963 7469 6f6e 5f77 6974 685f 5244 4237  iction_with_RDB7
-00001240: 2532 4652 4442 375f 6261 7272 6965 725f  %2FRDB7_barrier_
-00001250: 7072 6564 6963 7469 6f6e 5f65 7861 6d70  prediction_examp
-00001260: 6c65 2e69 7079 6e62 2920 7c0a 7c20 436f  le.ipynb) |.| Co
-00001270: 6d70 6172 696e 6720 7061 7274 6974 696f  mparing partitio
-00001280: 6e69 6e67 2061 7070 726f 6163 6865 7320  ning approaches 
-00001290: 666f 7220 616c 6b61 6e65 7320 7c20 5b21  for alkanes | [!
-000012a0: 5b42 696e 6465 725d 2868 7474 7073 3a2f  [Binder](https:/
-000012b0: 2f6d 7962 696e 6465 722e 6f72 672f 6261  /mybinder.org/ba
-000012c0: 6467 655f 6c6f 676f 2e73 7667 295d 2868  dge_logo.svg)](h
-000012d0: 7474 7073 3a2f 2f6d 7962 696e 6465 722e  ttps://mybinder.
-000012e0: 6f72 672f 7632 2f67 682f 4a61 636b 736f  org/v2/gh/Jackso
-000012f0: 6e42 7572 6e73 2f61 7374 6172 7465 732f  nBurns/astartes/
-00001300: 6d61 696e 3f6c 6162 7061 7468 3d65 7861  main?labpath=exa
-00001310: 6d70 6c65 7325 3246 6d6c 7064 735f 3230  mples%2Fmlpds_20
-00001320: 3233 5f61 7374 6172 7465 735f 6465 6d6f  23_astartes_demo
-00001330: 2532 466d 6c70 6473 5f32 3032 335f 6465  %2Fmlpds_2023_de
-00001340: 6d6f 2e69 7079 6e62 2920 7c0a 0a54 6f20  mo.ipynb) |..To 
-00001350: 6578 6563 7574 6520 7468 6573 6520 6e6f  execute these no
-00001360: 7465 626f 6f6b 7320 6c6f 6361 6c6c 792c  tebooks locally,
-00001370: 2063 6c6f 6e65 2074 6869 7320 7265 706f   clone this repo
-00001380: 7369 746f 7279 2028 692e 652e 2060 6769  sitory (i.e. `gi
-00001390: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-000013a0: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
-000013b0: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
-000013c0: 2e67 6974 6029 2c20 6e61 7669 6761 7465  .git`), navigate
-000013d0: 2074 6f20 7468 6520 6061 7374 6172 7465   to the `astarte
-000013e0: 7360 2064 6972 6563 746f 7279 2c20 7275  s` directory, ru
-000013f0: 6e20 6070 6970 2069 6e73 7461 6c6c 202e  n `pip install .
-00001400: 5b64 656d 6f73 5d60 2c20 7468 656e 206f  [demos]`, then o
-00001410: 7065 6e20 616e 6420 7275 6e20 7468 6520  pen and run the 
-00001420: 6e6f 7465 626f 6f6b 7320 696e 2079 6f75  notebooks in you
-00001430: 7220 7072 6566 6572 7265 6420 6564 6974  r preferred edit
-00001440: 6f72 2e0a 0a23 2323 2052 6174 696f 6e61  or...### Rationa
-00001450: 6c20 5370 6c69 7474 696e 6720 416c 676f  l Splitting Algo
-00001460: 7269 7468 6d73 0a57 6869 6c65 206d 7563  rithms.While muc
-00001470: 6820 6d61 6368 696e 6520 6c65 6172 6e69  h machine learni
-00001480: 6e67 2069 7320 646f 6e65 2077 6974 6820  ng is done with 
-00001490: 6120 7261 6e64 6f6d 2063 686f 6963 6520  a random choice 
-000014a0: 6265 7477 6565 6e20 7472 6169 6e69 6e67  between training
-000014b0: 2f76 616c 6964 6174 696f 6e2f 7465 7374  /validation/test
-000014c0: 2064 6174 612c 2061 6e20 616c 7465 726e   data, an altern
-000014d0: 6174 6976 6520 6973 2074 6865 2075 7365  ative is the use
-000014e0: 206f 6620 736f 2d63 616c 6c65 6420 2272   of so-called "r
-000014f0: 6174 696f 6e61 6c22 2073 706c 6974 7469  ational" splitti
-00001500: 6e67 2061 6c67 6f72 6974 686d 732e 2054  ng algorithms. T
-00001510: 6865 7365 2061 7070 726f 6163 6865 7320  hese approaches 
-00001520: 7573 6520 736f 6d65 2073 696d 696c 6172  use some similar
-00001530: 6974 792d 6261 7365 6420 616c 676f 7269  ity-based algori
-00001540: 7468 6d20 746f 2064 6976 6964 6520 6461  thm to divide da
-00001550: 7461 2069 6e74 6f20 7365 7473 2e20 536f  ta into sets. So
-00001560: 6d65 206f 6620 7468 6573 6520 616c 676f  me of these algo
-00001570: 7269 7468 6d73 2069 6e63 6c75 6465 204b  rithms include K
-00001580: 656e 6e61 7264 2d53 746f 6e65 2c20 6d69  ennard-Stone, mi
-00001590: 6e69 6d61 6c20 7465 7374 2073 6574 2064  nimal test set d
-000015a0: 6973 7369 6d69 6c61 7269 7479 2c20 616e  issimilarity, an
-000015b0: 6420 7370 6865 7265 2065 7863 6c75 7369  d sphere exclusi
-000015c0: 6f6e 2061 6c67 6f72 6974 686d 7320 5b61  on algorithms [a
-000015d0: 7320 6469 7363 7573 7365 6420 6279 2054  s discussed by T
-000015e0: 726f 7073 6861 2065 742e 2061 6c5d 2868  ropsha et. al](h
-000015f0: 7474 7073 3a2f 2f70 7562 732e 6163 732e  ttps://pubs.acs.
-00001600: 6f72 672f 646f 692f 7064 662f 3130 2e31  org/doi/pdf/10.1
-00001610: 3032 312f 6369 3330 3033 3338 7729 2061  021/ci300338w) a
-00001620: 7320 7765 6c6c 2061 7320 7468 6520 4f70  s well as the Op
-00001630: 7469 5369 6d20 6173 2064 6973 6375 7373  tiSim as discuss
-00001640: 6564 2069 6e20 5b41 7070 6c69 6564 2043  ed in [Applied C
-00001650: 6865 6d6f 696e 666f 726d 6174 6963 733a  hemoinformatics:
-00001660: 2041 6368 6965 7665 6d65 6e74 7320 616e   Achievements an
-00001670: 6420 4675 7475 7265 204f 7070 6f72 7475  d Future Opportu
-00001680: 6e69 7469 6573 5d28 6874 7470 733a 2f2f  nities](https://
-00001690: 7777 772e 7769 6c65 792e 636f 6d2f 656e  www.wiley.com/en
-000016a0: 2d75 732f 4170 706c 6965 642b 4368 656d  -us/Applied+Chem
-000016b0: 6f69 6e66 6f72 6d61 7469 6373 2533 412b  oinformatics%3A+
-000016c0: 4163 6869 6576 656d 656e 7473 2b61 6e64  Achievements+and
-000016d0: 2b46 7574 7572 652b 4f70 706f 7274 756e  +Future+Opportun
-000016e0: 6974 6965 732d 702d 3937 3833 3532 3738  ities-p-97835278
-000016f0: 3036 3534 3629 2e20 536f 6d65 2063 6c75  06546). Some clu
-00001700: 7374 6572 696e 672d 6261 7365 6420 7370  stering-based sp
-00001710: 6c69 7474 696e 6720 7465 6368 6e69 7175  litting techniqu
-00001720: 6573 2068 6176 6520 616c 736f 2062 6565  es have also bee
-00001730: 6e20 696e 636f 7270 6f72 6174 6564 2c20  n incorporated, 
-00001740: 7375 6368 2061 7320 5b44 4253 4341 4e5d  such as [DBSCAN]
-00001750: 2868 7474 703a 2f2f 6369 7465 7365 6572  (http://citeseer
-00001760: 782e 6973 742e 7073 752e 6564 752f 7669  x.ist.psu.edu/vi
-00001770: 6577 646f 632f 646f 776e 6c6f 6164 3f64  ewdoc/download?d
-00001780: 6f69 3d31 302e 312e 312e 3130 3136 2e38  oi=10.1.1.1016.8
-00001790: 3930 2672 6570 3d72 6570 3126 7479 7065  90&rep=rep1&type
-000017a0: 3d70 6466 292e 0a0a 5468 6572 6520 6172  =pdf)...There ar
-000017b0: 6520 7477 6f20 6272 6f61 6420 6361 7465  e two broad cate
-000017c0: 676f 7269 6573 206f 6620 7361 6d70 6c69  gories of sampli
-000017d0: 6e67 2061 6c67 6f72 6974 686d 7320 696d  ng algorithms im
-000017e0: 706c 656d 656e 7465 6420 696e 2060 6173  plemented in `as
-000017f0: 7461 7274 6573 603a 2065 7874 7261 706f  tartes`: extrapo
-00001800: 6c61 7469 7665 2061 6e64 2069 6e74 6572  lative and inter
-00001810: 706f 6c61 7469 7665 2e20 5468 6520 666f  polative. The fo
-00001820: 726d 6572 2077 696c 6c20 666f 7263 6520  rmer will force 
-00001830: 796f 7572 206d 6f64 656c 2074 6f20 7072  your model to pr
-00001840: 6564 6963 7420 6f6e 206f 7574 2d6f 662d  edict on out-of-
-00001850: 7361 6d70 6c65 2064 6174 612c 2077 6869  sample data, whi
-00001860: 6368 2063 7265 6174 6573 2061 206d 6f72  ch creates a mor
-00001870: 6520 6368 616c 6c65 6e67 696e 6720 7461  e challenging ta
-00001880: 736b 2074 6861 6e20 696e 7465 7270 6f6c  sk than interpol
-00001890: 6174 6976 6520 7361 6d70 6c69 6e67 2e20  ative sampling. 
-000018a0: 5365 6520 7468 6520 7461 626c 6520 6265  See the table be
-000018b0: 6c6f 7720 666f 7220 616c 6c20 6f66 2074  low for all of t
-000018c0: 6865 2073 616d 706c 696e 6720 6170 7072  he sampling appr
-000018d0: 6f61 6368 6573 2063 7572 7265 6e74 6c79  oaches currently
-000018e0: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-000018f0: 6061 7374 6172 7465 7360 2c20 6173 2077  `astartes`, as w
-00001900: 656c 6c20 6173 2074 6865 2068 7970 6572  ell as the hyper
-00001910: 7061 7261 6d65 7465 7273 2074 6861 7420  parameters that 
-00001920: 6561 6368 2061 6c67 6f72 6974 686d 2061  each algorithm a
-00001930: 6363 6570 7473 2028 7768 6963 6820 6172  ccepts (which ar
-00001940: 6520 7061 7373 6564 2069 6e20 7769 7468  e passed in with
-00001950: 2060 686f 7074 7360 2920 616e 6420 6120   `hopts`) and a 
-00001960: 6865 6c70 6675 6c20 7265 6665 7265 6e63  helpful referenc
-00001970: 6520 666f 7220 756e 6465 7273 7461 6e64  e for understand
-00001980: 696e 6720 686f 7720 7468 6520 6879 7065  ing how the hype
-00001990: 7270 6172 616d 6574 6572 7320 776f 726b  rparameters work
-000019a0: 2e20 4e6f 7465 2074 6861 7420 6072 616e  . Note that `ran
-000019b0: 646f 6d5f 7374 6174 6560 2069 7320 6465  dom_state` is de
-000019c0: 6669 6e65 6420 6173 2061 206b 6579 776f  fined as a keywo
-000019d0: 7264 2061 7267 756d 656e 7420 696e 2060  rd argument in `
-000019e0: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
-000019f0: 6020 6974 7365 6c66 2c20 6576 656e 2074  ` itself, even t
-00001a00: 686f 7567 6820 7468 6573 6520 616c 676f  hough these algo
-00001a10: 7269 7468 6d73 2077 696c 6c20 7573 6520  rithms will use 
-00001a20: 7468 6520 6072 616e 646f 6d5f 7374 6174  the `random_stat
-00001a30: 6560 2069 6e20 7468 6569 7220 6f77 6e20  e` in their own 
-00001a40: 776f 726b 2e20 446f 206e 6f74 2070 726f  work. Do not pro
-00001a50: 7669 6465 2061 2060 7261 6e64 6f6d 5f73  vide a `random_s
-00001a60: 7461 7465 6020 696e 2074 6865 2060 686f  tate` in the `ho
-00001a70: 7074 7360 2064 6963 7469 6f6e 6172 7920  pts` dictionary 
-00001a80: 2d20 6974 2077 696c 6c20 6265 206f 7665  - it will be ove
-00001a90: 7277 7269 7474 656e 2062 7920 7468 6520  rwritten by the 
-00001aa0: 6072 616e 646f 6d5f 7374 6174 6560 2079  `random_state` y
-00001ab0: 6f75 2070 726f 7669 6465 2066 6f72 2060  ou provide for `
-00001ac0: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
-00001ad0: 6020 286f 7220 7468 6520 6465 6661 756c  ` (or the defaul
-00001ae0: 7420 6966 206e 6f6e 6520 6973 2070 726f  t if none is pro
-00001af0: 7669 6465 6429 2e0a 0a23 2323 2320 496d  vided)...#### Im
-00001b00: 706c 656d 656e 7465 6420 5361 6d70 6c69  plemented Sampli
-00001b10: 6e67 2041 6c67 6f72 6974 686d 730a 0a7c  ng Algorithms..|
-00001b20: 2053 616d 706c 6572 204e 616d 6520 7c20   Sampler Name | 
-00001b30: 5573 6167 6520 5374 7269 6e67 207c 2054  Usage String | T
-00001b40: 7970 6520 7c20 4879 7065 7270 6172 616d  ype | Hyperparam
-00001b50: 6574 6572 7320 7c20 5265 6665 7265 6e63  eters | Referenc
-00001b60: 6520 7c20 4e6f 7465 7320 7c0a 7c3a 2d2d  e | Notes |.|:--
-00001b70: 2d3a 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c2d  -:|---|---|---|-
-00001b80: 2d2d 7c2d 2d2d 7c0a 7c20 5261 6e64 6f6d  --|---|.| Random
-00001b90: 207c 2027 7261 6e64 6f6d 2720 7c20 496e   | 'random' | In
-00001ba0: 7465 7270 6f6c 6174 6976 6520 7c20 6073  terpolative | `s
-00001bb0: 6875 6666 6c65 6020 7c20 5b60 736b 6c65  huffle` | [`skle
-00001bc0: 6172 6e20 7472 6169 6e5f 7465 7374 5f73  arn train_test_s
-00001bd0: 706c 6974 605d 2868 7474 7073 3a2f 2f73  plit`](https://s
-00001be0: 6369 6b69 742d 6c65 6172 6e2e 6f72 672f  cikit-learn.org/
-00001bf0: 7374 6162 6c65 2f6d 6f64 756c 6573 2f67  stable/modules/g
-00001c00: 656e 6572 6174 6564 2f73 6b6c 6561 726e  enerated/sklearn
-00001c10: 2e6d 6f64 656c 5f73 656c 6563 7469 6f6e  .model_selection
-00001c20: 2e74 7261 696e 5f74 6573 745f 7370 6c69  .train_test_spli
-00001c30: 742e 6874 6d6c 2920 7c20 5468 6973 2073  t.html) | This s
-00001c40: 616d 706c 6572 2069 7320 6120 6469 7265  ampler is a dire
-00001c50: 6374 2070 6173 7374 6872 6f75 6768 2074  ct passthrough t
-00001c60: 6f20 6073 6b6c 6561 726e 6027 7320 6074  o `sklearn`'s `t
-00001c70: 7261 696e 5f74 6573 745f 7370 6c69 7460  rain_test_split`
-00001c80: 2c20 7468 6f75 6768 2069 7420 646f 6573  , though it does
-00001c90: 206e 6f74 2063 7572 7265 6e74 6c79 2072   not currently r
-00001ca0: 6570 726f 6475 6365 2073 706c 6974 7320  eproduce splits 
-00001cb0: 6964 656e 7469 6361 6c6c 792e 207c 0a7c  identically. |.|
-00001cc0: 204b 656e 6e61 7264 2d53 746f 6e65 207c   Kennard-Stone |
-00001cd0: 2027 6b65 6e6e 6172 645f 7374 6f6e 6527   'kennard_stone'
-00001ce0: 207c 2049 6e74 6572 706f 6c61 7469 7665   | Interpolative
-00001cf0: 207c 2060 6d65 7472 6963 6020 7c20 5b4b   | `metric` | [K
-00001d00: 656e 6e61 7264 2026 2053 746f 6e65 5d28  ennard & Stone](
-00001d10: 6874 7470 733a 2f2f 7777 772e 7461 6e64  https://www.tand
-00001d20: 666f 6e6c 696e 652e 636f 6d2f 646f 692f  fonline.com/doi/
-00001d30: 6162 732f 3130 2e31 3038 302f 3030 3430  abs/10.1080/0040
-00001d40: 3137 3036 2e31 3936 392e 3130 3439 3036  1706.1969.104906
-00001d50: 3636 2920 7c20 4575 636c 6964 6961 6e20  66) | Euclidian 
-00001d60: 6469 7374 616e 6365 2069 7320 7573 6564  distance is used
-00001d70: 2062 7920 6465 6661 756c 742c 2061 7320   by default, as 
-00001d80: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
-00001d90: 206f 7269 6769 6e61 6c20 7061 7065 722e   original paper.
-00001da0: 207c 0a7c 2053 616d 706c 6520 7365 7420   |.| Sample set 
-00001db0: 5061 7274 6974 696f 6e69 6e67 2062 6173  Partitioning bas
-00001dc0: 6564 206f 6e20 6a6f 696e 7420 582d 5920  ed on joint X-Y 
-00001dd0: 6469 7374 616e 6365 7320 2853 5058 5929  distances (SPXY)
-00001de0: 207c 2027 7370 7879 2720 7c20 496e 7465   | 'spxy' | Inte
-00001df0: 7270 6f6c 6174 6976 6520 7c20 6064 6973  rpolative | `dis
-00001e00: 7461 6e63 655f 6d65 7472 6963 6020 7c20  tance_metric` | 
-00001e10: 5361 6c64 6861 6e61 2065 742e 2061 6c20  Saldhana et. al 
-00001e20: 5b6f 7269 6769 6e61 6c20 7061 7065 725d  [original paper]
-00001e30: 2868 7474 7073 3a2f 2f77 7777 2e73 6369  (https://www.sci
-00001e40: 656e 6365 6469 7265 6374 2e63 6f6d 2f73  encedirect.com/s
-00001e50: 6369 656e 6365 2f61 7274 6963 6c65 2f61  cience/article/a
-00001e60: 6273 2f70 6969 2f53 3030 3339 3931 3430  bs/pii/S00399140
-00001e70: 3035 3030 3139 3258 2920 7c20 4578 7465  0500192X) | Exte
-00001e80: 6e73 696f 6e20 6f66 204b 656e 6e61 7264  nsion of Kennard
-00001e90: 2053 746f 6e65 2074 6861 7420 616c 736f   Stone that also
-00001ea0: 2069 6e63 6c75 6465 7320 7468 6520 7265   includes the re
-00001eb0: 7370 6f6e 7365 2077 6865 6e20 7361 6d70  sponse when samp
-00001ec0: 6c69 6e67 2064 6973 7461 6e63 6573 2e20  ling distances. 
-00001ed0: 7c0a 7c20 5363 6166 666f 6c64 207c 2027  |.| Scaffold | '
-00001ee0: 7363 6166 666f 6c64 2720 7c20 4578 7472  scaffold' | Extr
-00001ef0: 6170 6f6c 6174 6976 6520 7c20 6069 6e63  apolative | `inc
-00001f00: 6c75 6465 5f63 6869 7261 6c69 7479 6020  lude_chirality` 
-00001f10: 7c20 5b42 656d 6973 2d4d 7572 636b 6f20  | [Bemis-Murcko 
-00001f20: 5363 6166 666f 6c64 5d28 6874 7470 733a  Scaffold](https:
-00001f30: 2f2f 7075 6273 2e61 6373 2e6f 7267 2f64  //pubs.acs.org/d
-00001f40: 6f69 2f66 756c 6c2f 3130 2e31 3032 312f  oi/full/10.1021/
-00001f50: 6a6d 3936 3032 3932 3829 2061 7320 696d  jm9602928) as im
-00001f60: 706c 656d 656e 7465 6420 696e 2052 444b  plemented in RDK
-00001f70: 6974 207c 2054 6869 7320 7361 6d70 6c65  it | This sample
-00001f80: 7220 7265 7175 6972 6573 2053 4d49 4c45  r requires SMILE
-00001f90: 5320 7374 7269 6e67 7320 6173 2069 6e70  S strings as inp
-00001fa0: 7574 2028 7573 6520 7468 6520 606d 6f6c  ut (use the `mol
-00001fb0: 6563 756c 6573 6020 7375 6270 6163 6b61  ecules` subpacka
-00001fc0: 6765 2920 7c0a 7c20 5370 6865 7265 2045  ge) |.| Sphere E
-00001fd0: 7863 6c75 7369 6f6e 207c 2027 7370 6865  xclusion | 'sphe
-00001fe0: 7265 5f65 7863 6c75 7369 6f6e 2720 7c20  re_exclusion' | 
-00001ff0: 4578 7472 6170 6f6c 6174 6976 6520 7c20  Extrapolative | 
-00002000: 606d 6574 7269 6360 2c20 6064 6973 7461  `metric`, `dista
-00002010: 6e63 655f 6375 746f 6666 6020 7c20 5f63  nce_cutoff` | _c
-00002020: 7573 746f 6d20 696d 706c 656d 656e 7461  ustom implementa
-00002030: 7469 6f6e 5f20 7c20 5661 7269 6174 696f  tion_ | Variatio
-00002040: 6e20 6f6e 2053 7068 6572 6520 4578 636c  n on Sphere Excl
-00002050: 7573 696f 6e20 666f 7220 6172 6269 7472  usion for arbitr
-00002060: 6172 792d 7661 6c75 6564 2076 6563 746f  ary-valued vecto
-00002070: 7273 2e20 7c0a 7c20 5469 6d65 2042 6173  rs. |.| Time Bas
-00002080: 6564 207c 2027 7469 6d65 5f62 6173 6564  ed | 'time_based
-00002090: 2720 7c20 4578 7472 6170 6f6c 6174 6976  ' | Extrapolativ
-000020a0: 6520 7c20 5f6e 6f6e 655f 207c 205b 4368  e | _none_ | [Ch
-000020b0: 656e 2065 7420 616c 2e5d 2868 7474 7073  en et al.](https
-000020c0: 3a2f 2f70 7562 732e 6163 732e 6f72 672f  ://pubs.acs.org/
-000020d0: 646f 692f 6675 6c6c 2f31 302e 3130 3231  doi/full/10.1021
-000020e0: 2f63 6932 3030 3631 3568 292c 205b 5368  /ci200615h), [Sh
-000020f0: 6572 6964 616e 2c20 522e 2050 5d28 6874  eridan, R. P](ht
-00002100: 7470 733a 2f2f 7075 6273 2e61 6373 2e6f  tps://pubs.acs.o
-00002110: 7267 2f64 6f69 2f66 756c 6c2f 3130 2e31  rg/doi/full/10.1
-00002120: 3032 312f 6369 3430 3030 3834 6b29 2c20  021/ci400084k), 
-00002130: 5b46 6569 6e62 6572 6720 6574 2061 6c2e  [Feinberg et al.
-00002140: 5d28 6874 7470 733a 2f2f 7075 6273 2e61  ](https://pubs.a
-00002150: 6373 2e6f 7267 2f64 6f69 2f66 756c 6c2f  cs.org/doi/full/
-00002160: 3130 2e31 3032 312f 6163 732e 6a6d 6564  10.1021/acs.jmed
-00002170: 6368 656d 2e39 6230 3231 3837 292c 205b  chem.9b02187), [
-00002180: 5374 7275 626c 6520 6574 2061 6c2e 5d28  Struble et al.](
-00002190: 6874 7470 733a 2f2f 7075 6273 2e72 7363  https://pubs.rsc
-000021a0: 2e6f 7267 2f65 6e2f 636f 6e74 656e 742f  .org/en/content/
-000021b0: 6172 7469 636c 6568 746d 6c2f 3230 3230  articlehtml/2020
-000021c0: 2f72 652f 6430 7265 3030 3037 316a 2920  /re/d0re00071j) 
-000021d0: 207c 2054 6869 7320 7361 6d70 6c65 7220   | This sampler 
-000021e0: 7265 7175 6972 6573 2060 6c61 6265 6c73  requires `labels
-000021f0: 6020 746f 2062 6520 616e 2069 7465 7261  ` to be an itera
-00002200: 626c 6520 6f66 2065 6974 6865 7220 6461  ble of either da
-00002210: 7465 206f 7220 6461 7465 7469 6d65 206f  te or datetime o
-00002220: 626a 6563 7473 2e20 7c0a 7c20 4f70 7469  bjects. |.| Opti
-00002230: 6d69 7a61 626c 6520 4b2d 4469 7373 696d  mizable K-Dissim
-00002240: 696c 6172 6974 7920 5365 6c65 6374 696f  ilarity Selectio
-00002250: 6e20 284f 7074 6953 696d 2920 7c20 276f  n (OptiSim) | 'o
-00002260: 7074 6973 696d 2720 7c20 4578 7472 6170  ptisim' | Extrap
-00002270: 6f6c 6174 6976 6520 7c20 606e 5f63 6c75  olative | `n_clu
-00002280: 7374 6572 7360 2c20 606d 6178 5f73 7562  sters`, `max_sub
-00002290: 7361 6d70 6c65 5f73 697a 6560 2c20 6064  sample_size`, `d
-000022a0: 6973 7461 6e63 655f 6375 746f 6666 6020  istance_cutoff` 
-000022b0: 7c20 5f63 7573 746f 6d20 696d 706c 656d  | _custom implem
-000022c0: 656e 7461 7469 6f6e 5f20 7c20 5661 7269  entation_ | Vari
-000022d0: 6174 696f 6e20 6f6e 205b 4f70 7469 5369  ation on [OptiSi
-000022e0: 6d5d 2868 7474 7073 3a2f 2f70 7562 732e  m](https://pubs.
-000022f0: 6163 732e 6f72 672f 646f 692f 3130 2e31  acs.org/doi/10.1
-00002300: 3032 312f 6369 3032 3536 3632 6829 2066  021/ci025662h) f
-00002310: 6f72 2061 7262 6974 7261 7279 2d76 616c  or arbitrary-val
-00002320: 7565 6420 7665 6374 6f72 732e 207c 0a7c  ued vectors. |.|
-00002330: 204b 2d4d 6561 6e73 207c 2027 6b6d 6561   K-Means | 'kmea
-00002340: 6e73 2720 7c20 4578 7472 6170 6f6c 6174  ns' | Extrapolat
-00002350: 6976 6520 7c20 606e 5f63 6c75 7374 6572  ive | `n_cluster
-00002360: 7360 2c20 606e 5f69 6e69 7460 207c 205b  s`, `n_init` | [
-00002370: 6073 6b6c 6561 726e 204b 4d65 616e 7360  `sklearn KMeans`
-00002380: 5d28 6874 7470 733a 2f2f 7363 696b 6974  ](https://scikit
-00002390: 2d6c 6561 726e 2e6f 7267 2f73 7461 626c  -learn.org/stabl
-000023a0: 652f 6d6f 6475 6c65 732f 6765 6e65 7261  e/modules/genera
-000023b0: 7465 642f 736b 6c65 6172 6e2e 636c 7573  ted/sklearn.clus
-000023c0: 7465 722e 4b4d 6561 6e73 2e68 746d 6c29  ter.KMeans.html)
-000023d0: 207c 2050 6173 7374 6872 6f75 6768 2074   | Passthrough t
-000023e0: 6f20 6073 6b6c 6561 726e 6027 7320 604b  o `sklearn`'s `K
-000023f0: 4d65 616e 7360 2e20 7c0a 7c20 4465 6e73  Means`. |.| Dens
-00002400: 6974 792d 4261 7365 6420 5370 6174 6961  ity-Based Spatia
-00002410: 6c20 436c 7573 7465 7269 6e67 206f 6620  l Clustering of 
-00002420: 4170 706c 6963 6174 696f 6e73 2077 6974  Applications wit
-00002430: 6820 4e6f 6973 6520 2844 4253 4341 4e29  h Noise (DBSCAN)
-00002440: 207c 2027 6462 7363 616e 2720 7c20 4578   | 'dbscan' | Ex
-00002450: 7472 6170 6f6c 6174 6976 6520 7c20 6065  trapolative | `e
-00002460: 7073 602c 2060 6d69 6e5f 7361 6d70 6c65  ps`, `min_sample
-00002470: 7360 2c20 6061 6c67 6f72 6974 686d 602c  s`, `algorithm`,
-00002480: 2060 6d65 7472 6963 602c 2060 6c65 6166   `metric`, `leaf
-00002490: 5f73 697a 6560 207c 205b 6073 6b6c 6561  _size` | [`sklea
-000024a0: 726e 2044 4253 4341 4e60 5d28 6874 7470  rn DBSCAN`](http
-000024b0: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
-000024c0: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
-000024d0: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
-000024e0: 6c65 6172 6e2e 636c 7573 7465 722e 4442  learn.cluster.DB
-000024f0: 5343 414e 2e68 746d 6c29 207c 2050 6173  SCAN.html) | Pas
-00002500: 7374 6872 6f75 6768 2074 6f20 6073 6b6c  sthrough to `skl
-00002510: 6561 726e 6027 7320 6044 4253 4341 4e60  earn`'s `DBSCAN`
-00002520: 2e20 7c0a 7c20 4d69 6e69 6d75 6d20 5465  . |.| Minimum Te
-00002530: 7374 2053 6574 2044 6973 7369 6d69 6c61  st Set Dissimila
-00002540: 7269 7479 2028 4d54 5344 2920 7c20 7e20  rity (MTSD) | ~ 
-00002550: 7c20 7e20 7c20 5f75 7063 6f6d 696e 6720  | ~ | _upcoming 
-00002560: 696e 5f20 6061 7374 6172 7465 7360 205f  in_ `astartes` _
-00002570: 7631 2e78 5f20 7c20 7e20 7c20 7e20 7c0a  v1.x_ | ~ | ~ |.
-00002580: 7c20 5265 7374 7269 6374 6564 2042 6f6c  | Restricted Bol
-00002590: 747a 6d61 6e6e 204d 6163 6869 6e65 2028  tzmann Machine (
-000025a0: 5242 4d29 207c 207e 207c 207e 207c 205f  RBM) | ~ | ~ | _
-000025b0: 7570 636f 6d69 6e67 2069 6e5f 2060 6173  upcoming in_ `as
-000025c0: 7461 7274 6573 6020 5f76 312e 785f 207c  tartes` _v1.x_ |
-000025d0: 207e 207c 207e 207c 0a7c 204b 6f68 6f6e   ~ | ~ |.| Kohon
-000025e0: 656e 2053 656c 662d 4f72 6761 6e69 7a69  en Self-Organizi
-000025f0: 6e67 204d 6170 2028 534f 4d29 207c 207e  ng Map (SOM) | ~
-00002600: 207c 207e 207c 205f 7570 636f 6d69 6e67   | ~ | _upcoming
-00002610: 2069 6e5f 2060 6173 7461 7274 6573 6020   in_ `astartes` 
-00002620: 5f76 312e 785f 207c 207e 207c 207e 207c  _v1.x_ | ~ | ~ |
-00002630: 0a7c 2053 506c 6974 204d 6574 686f 6420  .| SPlit Method 
-00002640: 7c20 7e20 7c20 7e20 7c20 5f75 7063 6f6d  | ~ | ~ | _upcom
-00002650: 696e 6720 696e 5f20 6061 7374 6172 7465  ing in_ `astarte
-00002660: 7360 205f 7631 2e78 5f20 7c20 7e20 7c20  s` _v1.x_ | ~ | 
-00002670: 7e20 7c0a 0a23 2323 2055 7369 6e67 2074  ~ |..### Using t
-00002680: 6865 2060 6173 7461 7274 6573 2e6d 6f6c  he `astartes.mol
-00002690: 6563 756c 6573 6020 5375 6270 6163 6b61  ecules` Subpacka
-000026a0: 6765 0a41 6674 6572 2069 6e73 7461 6c6c  ge.After install
-000026b0: 696e 6720 7769 7468 2060 7069 7020 696e  ing with `pip in
-000026c0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
-000026d0: 6f6c 6563 756c 6573 5d60 206f 6e65 2063  olecules]` one c
-000026e0: 616e 2069 6d70 6f72 7420 7468 6520 6e65  an import the ne
-000026f0: 7720 7472 6169 6e2f 7465 7374 2073 706c  w train/test spl
-00002700: 6974 7469 6e67 2066 756e 6374 696f 6e20  itting function 
-00002710: 6c69 6b65 2074 6869 733a 2060 6672 6f6d  like this: `from
-00002720: 2061 7374 6172 7465 732e 6d6f 6c65 6375   astartes.molecu
-00002730: 6c65 7320 696d 706f 7274 2074 7261 696e  les import train
-00002740: 5f74 6573 745f 7370 6c69 745f 6d6f 6c65  _test_split_mole
-00002750: 6375 6c65 7360 0a0a 5468 6520 7573 6167  cules`..The usag
-00002760: 6520 6f66 2074 6869 7320 6675 6e63 7469  e of this functi
-00002770: 6f6e 2069 7320 6964 656e 7469 6361 6c20  on is identical 
-00002780: 746f 2060 7472 6169 6e5f 7465 7374 5f73  to `train_test_s
-00002790: 706c 6974 6020 6275 7420 7769 7468 2074  plit` but with t
-000027a0: 6865 2061 6464 6974 696f 6e20 6f66 206e  he addition of n
-000027b0: 6577 2061 7267 756d 656e 7473 2074 6f20  ew arguments to 
-000027c0: 636f 6e74 726f 6c20 686f 7720 7468 6520  control how the 
-000027d0: 6d6f 6c65 6375 6c65 7320 6172 6520 6665  molecules are fe
-000027e0: 6174 7572 697a 6564 3a0a 0a60 6060 7079  aturized:..```py
-000027f0: 7468 6f6e 0a74 7261 696e 5f74 6573 745f  thon.train_test_
-00002800: 7370 6c69 745f 6d6f 6c65 6375 6c65 7328  split_molecules(
-00002810: 0a20 2020 206d 6f6c 6563 756c 6573 3d73  .    molecules=s
-00002820: 6d69 6c65 732c 0a20 2020 2079 3d79 2c0a  miles,.    y=y,.
-00002830: 2020 2020 7465 7374 5f73 697a 653d 302e      test_size=0.
-00002840: 322c 0a20 2020 2074 7261 696e 5f73 697a  2,.    train_siz
-00002850: 653d 302e 382c 0a20 2020 2066 696e 6765  e=0.8,.    finge
-00002860: 7270 7269 6e74 3d22 6461 796c 6967 6874  rprint="daylight
-00002870: 5f66 696e 6765 7270 7269 6e74 222c 0a20  _fingerprint",. 
-00002880: 2020 2066 7072 696e 7473 5f68 6f70 7473     fprints_hopts
-00002890: 3d7b 0a20 2020 2020 2020 2022 6d69 6e50  ={.        "minP
-000028a0: 6174 6822 3a20 322c 0a20 2020 2020 2020  ath": 2,.       
-000028b0: 2022 6d61 7850 6174 6822 3a20 352c 0a20   "maxPath": 5,. 
-000028c0: 2020 2020 2020 2022 6670 5369 7a65 223a         "fpSize":
-000028d0: 2032 3030 2c0a 2020 2020 2020 2020 2262   200,.        "b
-000028e0: 6974 7350 6572 4861 7368 223a 2034 2c0a  itsPerHash": 4,.
-000028f0: 2020 2020 2020 2020 2275 7365 4873 223a          "useHs":
-00002900: 2031 2c0a 2020 2020 2020 2020 2274 6774   1,.        "tgt
-00002910: 4465 6e73 6974 7922 3a20 302e 342c 0a20  Density": 0.4,. 
-00002920: 2020 2020 2020 2022 6d69 6e53 697a 6522         "minSize"
-00002930: 3a20 3634 2c0a 2020 2020 7d2c 0a20 2020  : 64,.    },.   
-00002940: 2073 616d 706c 6572 3d22 7261 6e64 6f6d   sampler="random
-00002950: 222c 0a20 2020 2072 616e 646f 6d5f 7374  ",.    random_st
-00002960: 6174 653d 3432 2c0a 2020 2020 686f 7074  ate=42,.    hopt
-00002970: 733d 7b0a 2020 2020 2020 2020 2273 6875  s={.        "shu
-00002980: 6666 6c65 223a 2054 7275 652c 0a20 2020  ffle": True,.   
-00002990: 207d 2c0a 290a 6060 600a 0a54 6f20 7365   },.).```..To se
-000029a0: 6520 6120 636f 6d70 6c65 7465 2065 7861  e a complete exa
-000029b0: 6d70 6c65 206f 6620 7573 696e 6720 6074  mple of using `t
-000029c0: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
-000029d0: 6d6f 6c65 6375 6c65 7360 2077 6974 6820  molecules` with 
-000029e0: 6163 7475 616c 2063 6865 6d69 6361 6c20  actual chemical 
-000029f0: 6461 7461 2c20 7461 6b65 2061 206c 6f6f  data, take a loo
-00002a00: 6b20 696e 2074 6865 2060 6578 616d 706c  k in the `exampl
-00002a10: 6573 6020 6469 7265 6374 6f72 792e 0a0a  es` directory...
-00002a20: 436f 6e66 6967 7572 6174 696f 6e20 6f70  Configuration op
-00002a30: 7469 6f6e 7320 666f 7220 7468 6520 6665  tions for the fe
-00002a40: 6174 7572 697a 6174 696f 6e20 7363 6865  aturization sche
-00002a50: 6d65 2063 616e 2062 6520 666f 756e 6420  me can be found 
-00002a60: 696e 2074 6865 2064 6f63 756d 656e 7461  in the documenta
-00002a70: 7469 6f6e 2066 6f72 205b 6041 494d 5369  tion for [`AIMSi
-00002a80: 6d60 5d28 6874 7470 733a 2f2f 766c 6163  m`](https://vlac
-00002a90: 686f 7367 726f 7570 2e67 6974 6875 622e  hosgroup.github.
-00002aa0: 696f 2f41 494d 5369 6d2f 5245 4144 4d45  io/AIMSim/README
-00002ab0: 2e68 746d 6c23 6375 7272 656e 746c 792d  .html#currently-
-00002ac0: 696d 706c 656d 656e 7465 642d 6669 6e67  implemented-fing
-00002ad0: 6572 7072 696e 7473 2920 7468 6f75 6768  erprints) though
-00002ae0: 206d 6f73 7420 6f66 2074 6865 2063 7269   most of the cri
-00002af0: 7469 6361 6c20 636f 6e66 6967 7572 6174  tical configurat
-00002b00: 696f 6e20 6f70 7469 6f6e 7320 6172 6520  ion options are 
-00002b10: 7368 6f77 6e20 6162 6f76 652e 0a0a 2323  shown above...##
-00002b20: 2320 5265 7072 6f64 7563 6962 696c 6974  # Reproducibilit
-00002b30: 790a 6061 7374 6172 7465 7360 2061 696d  y.`astartes` aim
-00002b40: 7320 746f 2062 6520 636f 6d70 6c65 7465  s to be complete
-00002b50: 6c79 2072 6570 726f 6475 6369 626c 6520  ly reproducible 
-00002b60: 6163 726f 7373 2064 6966 6665 7265 6e74  across different
-00002b70: 2070 6c61 7466 6f72 6d73 2c20 5079 7468   platforms, Pyth
-00002b80: 6f6e 2076 6572 7369 6f6e 732c 2061 6e64  on versions, and
-00002b90: 2064 6570 656e 6465 6e63 7920 636f 6e66   dependency conf
-00002ba0: 6967 7572 6174 696f 6e73 202d 2061 6e79  igurations - any
-00002bb0: 2076 6572 7369 6f6e 206f 6620 6061 7374   version of `ast
-00002bc0: 6172 7465 7360 2076 312e 7820 7368 6f75  artes` v1.x shou
-00002bd0: 6c64 2072 6573 756c 7420 696e 2074 6865  ld result in the
-00002be0: 205f 6578 6163 745f 2073 616d 6520 7370   _exact_ same sp
-00002bf0: 6c69 7473 2c20 616c 7761 7973 2e0a 546f  lits, always..To
-00002c00: 2074 6861 7420 656e 642c 2074 6865 2064   that end, the d
-00002c10: 6566 6175 6c74 2062 6568 6176 696f 7220  efault behavior 
-00002c20: 6f66 2060 6173 7461 7274 6573 6020 6973  of `astartes` is
-00002c30: 2074 6f20 7573 6520 6034 3260 2061 7320   to use `42` as 
-00002c40: 7468 6520 7261 6e64 6f6d 2073 6565 6420  the random seed 
-00002c50: 616e 6420 5f61 6c77 6179 735f 2073 6574  and _always_ set
-00002c60: 2069 742e 0a52 756e 6e69 6e67 2060 6173   it..Running `as
-00002c70: 7461 7274 6573 6020 7769 7468 2074 6865  tartes` with the
-00002c80: 2064 6566 6175 6c74 2073 6574 7469 6e67   default setting
-00002c90: 7320 7769 6c6c 2061 6c77 6179 7320 7072  s will always pr
-00002ca0: 6f64 7563 6520 7468 6520 6578 6163 7420  oduce the exact 
-00002cb0: 7361 6d65 2072 6573 756c 7473 2e0a 5765  same results..We
-00002cc0: 2068 6176 6520 7665 7269 6669 6564 2074   have verified t
-00002cd0: 6869 7320 6265 6861 7669 6f72 206f 6e20  his behavior on 
-00002ce0: 4465 6269 616e 2055 6275 6e74 752c 2057  Debian Ubuntu, W
-00002cf0: 696e 646f 7773 2c20 616e 6420 496e 7465  indows, and Inte
-00002d00: 6c20 4d61 6373 2066 726f 6d20 5079 7468  l Macs from Pyth
-00002d10: 6f6e 2076 6572 7369 6f6e 7320 332e 3720  on versions 3.7 
-00002d20: 7468 726f 7567 6820 332e 3131 2028 7769  through 3.11 (wi
-00002d30: 7468 2061 7070 726f 7072 6961 7465 2064  th appropriate d
-00002d40: 6570 656e 6465 6e63 6965 7320 666f 7220  ependencies for 
-00002d50: 6561 6368 2076 6572 7369 6f6e 292e 0a0a  each version)...
-00002d60: 2323 2323 204b 6e6f 776e 2052 6570 726f  #### Known Repro
-00002d70: 6475 6369 6269 6c69 7479 204c 696d 6974  ducibility Limit
-00002d80: 6174 696f 6e73 0a0a 3e20 2a2a 4e6f 7465  ations..> **Note
-00002d90: 2a2a 0a3e 2057 6520 6172 6520 6c69 6d69  **.> We are limi
-00002da0: 7465 6420 696e 206f 7572 2061 6269 6c69  ted in our abili
-00002db0: 7479 2074 6f20 7465 7374 206f 6e20 4d31  ty to test on M1
-00002dc0: 204d 6163 732c 2062 7574 2066 726f 6d20   Macs, but from 
-00002dd0: 6f75 7220 6c69 6d69 7465 6420 6d61 6e75  our limited manu
-00002de0: 616c 2074 6573 7469 6e67 2077 6520 6163  al testing we ac
-00002df0: 6869 6576 6520 7065 7266 6563 7420 7265  hieve perfect re
-00002e00: 7072 6f64 7563 6269 6c69 7479 2069 6e20  producbility in 
-00002e10: 616c 6c20 6361 7365 7320 5f65 7863 6570  all cases _excep
-00002e20: 7420 6f63 6361 7369 6f6e 616c 6c79 5f20  t occasionally_ 
-00002e30: 7769 7468 2060 4b4d 6561 6e73 6020 6f6e  with `KMeans` on
-00002e40: 2041 7070 6c65 2073 696c 6963 6f6e 2e0a   Apple silicon..
-00002e50: 4974 2068 6173 2070 726f 6475 6365 6420  It has produced 
-00002e60: 5f73 6c69 6768 746c 795f 2064 6966 6665  _slightly_ diffe
-00002e70: 7265 6e74 2072 6573 756c 7473 2062 6574  rent results bet
-00002e80: 7765 656e 2070 6c61 7466 6f72 6d73 2072  ween platforms r
-00002e90: 6567 6172 646c 6573 7320 6f66 2060 7261  egardless of `ra
-00002ea0: 6e64 6f6d 5f73 7461 7465 602c 2077 6974  ndom_state`, wit
-00002eb0: 6820 7570 2074 6f20 7477 6f20 636c 7573  h up to two clus
-00002ec0: 7465 7273 2062 6569 6e67 2061 7373 6967  ters being assig
-00002ed0: 6e65 6420 6469 6666 6572 656e 746c 7920  ned differently 
-00002ee0: 7265 7375 6c74 696e 6720 696e 2064 6174  resulting in dat
-00002ef0: 6120 7370 6c69 7473 2077 6869 6368 2061  a splits which a
-00002f00: 7265 203e 3939 2520 6964 656e 7469 6361  re >99% identica
-00002f10: 6c2e 0a60 6173 7461 7274 6573 6020 6973  l..`astartes` is
-00002f20: 2073 7469 6c6c 2063 6f6e 7369 7374 656e   still consisten
-00002f30: 7420 6265 7477 6565 6e20 7275 6e73 206f  t between runs o
-00002f40: 6e20 7468 6520 7361 6d65 2070 6c61 7466  n the same platf
-00002f50: 6f72 6d20 696e 2061 6c6c 2063 6173 6573  orm in all cases
-00002f60: 2c20 616e 6420 6f74 6865 7220 7361 6d70  , and other samp
-00002f70: 6c65 7273 2061 7265 206e 6f74 2069 6d70  lers are not imp
-00002f80: 6163 7465 6420 6279 2074 6869 7320 6170  acted by this ap
-00002f90: 7061 7265 6e74 2062 7567 2e0a 0a20 2d20  parent bug... - 
-00002fa0: 6073 6b6c 6561 726e 6020 7631 2e33 2e30  `sklearn` v1.3.0
-00002fb0: 2069 6e74 726f 6475 6365 6420 6261 636b   introduced back
-00002fc0: 7761 7264 732d 696e 636f 6d70 6174 6962  wards-incompatib
-00002fd0: 6c65 2063 6861 6e67 6573 2069 6e20 7468  le changes in th
-00002fe0: 6520 604b 4d65 616e 7360 2073 616d 706c  e `KMeans` sampl
-00002ff0: 6572 2074 6861 7420 6368 616e 6765 6420  er that changed 
-00003000: 686f 7720 7468 6520 7261 6e64 6f6d 2069  how the random i
-00003010: 6e69 7469 616c 697a 6174 696f 6e20 6166  nitialization af
-00003020: 6665 6374 7320 7468 6520 7265 7375 6c74  fects the result
-00003030: 732c 2065 7665 6e20 6769 7665 6e20 7468  s, even given th
-00003040: 6520 7361 6d65 2072 616e 646f 6d20 7365  e same random se
-00003050: 6564 2e20 4469 6666 6572 656e 7420 7665  ed. Different ve
-00003060: 7273 696f 6e20 6f66 2060 736b 6c65 6172  rsion of `sklear
-00003070: 6e60 2077 696c 6c20 6166 6665 6374 2074  n` will affect t
-00003080: 6865 2070 6572 666f 726d 616e 6365 206f  he performance o
-00003090: 6620 6061 7374 6172 7465 7360 2061 6e64  f `astartes` and
-000030a0: 2077 6520 7265 636f 6d6d 656e 6420 696e   we recommend in
-000030b0: 636c 7564 696e 6720 7468 6520 6578 6163  cluding the exac
-000030c0: 7420 7665 7273 696f 6e20 6f66 2060 7363  t version of `sc
-000030d0: 696b 6974 2d6c 6561 726e 6020 616e 6420  ikit-learn` and 
-000030e0: 6061 7374 6172 7465 7360 2075 7365 642c  `astartes` used,
-000030f0: 2077 6865 6e20 6170 706c 6963 6162 6c65   when applicable
-00003100: 2e0a 0a23 2320 4576 616c 7561 7465 2074  ...## Evaluate t
-00003110: 6865 2049 6d70 6163 7420 6f66 2053 706c  he Impact of Spl
-00003120: 6974 7469 6e67 2041 6c67 6f72 6974 686d  itting Algorithm
-00003130: 730a 5468 6520 6067 656e 6572 6174 655f  s.The `generate_
-00003140: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
-00003150: 7473 5f64 6963 7460 2066 756e 6374 696f  ts_dict` functio
-00003160: 6e20 616c 6c6f 7773 2075 7365 7273 2074  n allows users t
-00003170: 6f20 7175 6963 6b6c 7920 6576 616c 7561  o quickly evalua
-00003180: 7465 2074 6865 2069 6d70 6163 7420 6f66  te the impact of
-00003190: 2064 6966 6665 7265 6e74 2073 706c 6974   different split
-000031a0: 7469 6e67 2074 6563 686e 6971 7565 7320  ting techniques 
-000031b0: 6f6e 2061 6e79 206d 6f64 656c 2073 7570  on any model sup
-000031c0: 706f 7274 6564 2062 7920 6073 6b6c 6561  ported by `sklea
-000031d0: 726e 602e 2041 6c6c 2072 6573 756c 7473  rn`. All results
-000031e0: 2061 7265 2073 746f 7265 6420 696e 2061   are stored in a
-000031f0: 2064 6963 7469 6f6e 6172 7920 666f 726d   dictionary form
-00003200: 6174 2061 6e64 2063 616e 2062 6520 6469  at and can be di
-00003210: 7370 6c61 7965 6420 696e 2061 206e 6561  splayed in a nea
-00003220: 746c 7920 666f 726d 6174 7465 6420 7461  tly formatted ta
-00003230: 626c 6520 7573 696e 6720 7468 6520 6f70  ble using the op
-00003240: 7469 6f6e 616c 2060 7072 696e 745f 7265  tional `print_re
-00003250: 7375 6c74 7360 2061 7267 756d 656e 742e  sults` argument.
-00003260: 0a0a 6060 600a 6672 6f6d 2073 6b6c 6561  ..```.from sklea
-00003270: 726e 2e73 766d 2069 6d70 6f72 7420 4c69  rn.svm import Li
-00003280: 6e65 6172 5356 520a 0a66 726f 6d20 6173  nearSVR..from as
-00003290: 7461 7274 6573 2e75 7469 6c73 2069 6d70  tartes.utils imp
-000032a0: 6f72 7420 6765 6e65 7261 7465 5f72 6567  ort generate_reg
-000032b0: 7265 7373 696f 6e5f 7265 7375 6c74 735f  ression_results_
-000032c0: 6469 6374 0a0a 736b 6c65 6172 6e5f 6d6f  dict..sklearn_mo
-000032d0: 6465 6c20 3d20 4c69 6e65 6172 5356 5228  del = LinearSVR(
-000032e0: 290a 7265 7375 6c74 735f 6469 6374 203d  ).results_dict =
-000032f0: 2067 656e 6572 6174 655f 7265 6772 6573   generate_regres
-00003300: 7369 6f6e 5f72 6573 756c 7473 5f64 6963  sion_results_dic
-00003310: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00003320: 2020 2020 2020 2073 6b6c 6561 726e 5f6d         sklearn_m
-00003330: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
-00003340: 2020 2020 2020 2020 2020 582c 0a20 2020            X,.   
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2079 2c0a 2020 2020 2020 2020 2020 2020   y,.            
-00003370: 2020 2020 2020 2020 7072 696e 745f 7265          print_re
-00003380: 7375 6c74 733d 5472 7565 2c0a 2020 2020  sults=True,.    
-00003390: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000033a0: 2020 2020 2020 2054 7261 696e 2020 2020         Train    
-000033b0: 2020 2056 616c 2020 2020 2020 5465 7374     Val      Test
-000033c0: 0a2d 2d2d 2d20 202d 2d2d 2d2d 2d2d 2d20  .----  -------- 
-000033d0: 202d 2d2d 2d2d 2d2d 2d20 202d 2d2d 2d2d   --------  -----
-000033e0: 2d2d 2d0a 4d41 4520 2020 312e 3431 3532  ---.MAE   1.4152
-000033f0: 3220 2020 332e 3133 3433 3520 2020 322e  2   3.13435   2.
-00003400: 3137 3039 310a 524d 5345 2020 322e 3033  17091.RMSE  2.03
-00003410: 3036 3220 2020 332e 3733 3732 3120 2020  062   3.73721   
-00003420: 322e 3430 3034 310a 5232 2020 2020 302e  2.40041.R2    0.
-00003430: 3930 3734 3520 2020 302e 3830 3738 3720  90745   0.80787 
-00003440: 2020 302e 3738 3431 320a 0a60 6060 0a0a    0.78412..```..
-00003450: 2323 204f 6e6c 696e 6520 446f 6375 6d65  ## Online Docume
-00003460: 6e74 6174 696f 6e0a 5b54 6865 206f 6e6c  ntation.[The onl
-00003470: 696e 6520 646f 6375 6d65 6e74 6174 696f  ine documentatio
-00003480: 6e5d 2868 7474 7073 3a2f 2f4a 6163 6b73  n](https://Jacks
-00003490: 6f6e 4275 726e 732e 6769 7468 7562 2e69  onBurns.github.i
-000034a0: 6f2f 6173 7461 7274 6573 2f29 2063 6f6e  o/astartes/) con
-000034b0: 7461 696e 7320 6576 6572 7974 6869 6e67  tains everything
-000034c0: 2079 6f75 2073 6565 2069 6e20 7468 6973   you see in this
-000034d0: 2052 4541 444d 4520 7769 7468 2061 6e20   README with an 
-000034e0: 6164 6469 7469 6f6e 616c 2074 7574 6f72  additional tutor
-000034f0: 6961 6c20 666f 7220 5b6d 6f76 696e 6720  ial for [moving 
-00003500: 6672 6f6d 2060 7472 6169 6e5f 7465 7374  from `train_test
-00003510: 5f73 706c 6974 6020 696e 2060 736b 6c65  _split` in `skle
-00003520: 6172 6e60 2074 6f20 6061 7374 6172 7465  arn` to `astarte
-00003530: 7360 5d28 6874 7470 733a 2f2f 6a61 636b  s`](https://jack
-00003540: 736f 6e62 7572 6e73 2e67 6974 6875 622e  sonburns.github.
-00003550: 696f 2f61 7374 6172 7465 732f 736b 6c65  io/astartes/skle
-00003560: 6172 6e5f 746f 5f61 7374 6172 7465 732e  arn_to_astartes.
-00003570: 6874 6d6c 292e 0a0a 2323 2048 6f77 2074  html)...## How t
-00003580: 6f20 4369 7465 0a49 6620 796f 7520 7573  o Cite.If you us
-00003590: 6520 6061 7374 6172 7465 7360 2069 6e20  e `astartes` in 
-000035a0: 796f 7572 2077 6f72 6b20 706c 6561 7365  your work please
-000035b0: 2075 7365 2074 6865 2062 656c 6f77 2063   use the below c
-000035c0: 6974 6174 696f 6e20 6f72 2074 6865 2022  itation or the "
-000035d0: 4369 7465 2074 6869 7320 7265 706f 7369  Cite this reposi
-000035e0: 746f 7279 2220 6275 7474 6f6e 206f 6e20  tory" button on 
-000035f0: 4769 7448 7562 3a0a 3e20 2a2a 4269 6254  GitHub:.> **BibT
-00003600: 6558 2a2a 0a3e 2040 736f 6674 7761 7265  eX**.> @software
-00003610: 7b42 7572 6e73 5f61 7374 6172 7465 732c  {Burns_astartes,
-00003620: 0a3e 2020 2061 7574 686f 7220 3d20 7b42  .>   author = {B
-00003630: 7572 6e73 2c20 4a61 636b 736f 6e20 616e  urns, Jackson an
-00003640: 6420 5370 6965 6b65 726d 616e 6e2c 204b  d Spiekermann, K
-00003650: 6576 696e 2061 6e64 2042 6861 7474 6163  evin and Bhattac
-00003660: 6861 726a 6565 2c20 4869 6d61 6768 6e61  harjee, Himaghna
-00003670: 2061 6e64 2056 6c61 6368 6f73 2c20 4469   and Vlachos, Di
-00003680: 6f6e 6973 696f 7320 616e 6420 4772 6565  onisios and Gree
-00003690: 6e2c 2057 696c 6c69 616d 7d2c 0a3e 2020  n, William},.>  
-000036a0: 206c 6963 656e 7365 203d 207b 4d49 547d   license = {MIT}
-000036b0: 2c0a 3e20 2020 7469 746c 6520 3d20 7b7b  ,.>   title = {{
-000036c0: 6173 7461 7274 6573 7d7d 2c0a 3e20 2020  astartes}},.>   
-000036d0: 7572 6c20 3d20 7b68 7474 7073 3a2f 2f67  url = {https://g
-000036e0: 6974 6875 622e 636f 6d2f 4a61 636b 736f  ithub.com/Jackso
-000036f0: 6e42 7572 6e73 2f61 7374 6172 7465 737d  nBurns/astartes}
-00003700: 0a3e 207d 0a0a 3e20 2a2a 4150 412a 2a0a  .> }..> **APA**.
-00003710: 3e20 4275 726e 732c 204a 2e2c 2053 7069  > Burns, J., Spi
-00003720: 656b 6572 6d61 6e6e 2c20 4b2e 2c20 4268  ekermann, K., Bh
-00003730: 6174 7461 6368 6172 6a65 652c 2048 2e2c  attacharjee, H.,
-00003740: 2056 6c61 6368 6f73 2c20 442e 2c20 2620   Vlachos, D., & 
-00003750: 4772 6565 6e2c 2057 2e20 6173 7461 7274  Green, W. astart
-00003760: 6573 205b 436f 6d70 7574 6572 2073 6f66  es [Computer sof
-00003770: 7477 6172 655d 2e20 6874 7470 733a 2f2f  tware]. https://
-00003780: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
-00003790: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
-000037a0: 0a0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-000037b0: 6e67 2026 2044 6576 656c 6f70 6572 204e  ng & Developer N
-000037c0: 6f74 6573 0a50 756c 6c20 5265 7175 6573  otes.Pull Reques
-000037d0: 7473 2c20 4275 6720 5265 706f 7274 732c  ts, Bug Reports,
-000037e0: 2061 6e64 2061 6c6c 2043 6f6e 7472 6962   and all Contrib
-000037f0: 7574 696f 6e73 2061 7265 2077 656c 636f  utions are welco
-00003800: 6d65 2120 506c 6561 7365 2075 7365 2074  me! Please use t
-00003810: 6865 2061 7070 726f 7072 6961 7465 2069  he appropriate i
-00003820: 7373 7565 206f 7220 7075 6c6c 2072 6571  ssue or pull req
-00003830: 7565 7374 2074 656d 706c 6174 6520 7768  uest template wh
-00003840: 656e 206d 616b 696e 6720 6120 636f 6e74  en making a cont
-00003850: 7269 6275 7469 6f6e 2e0a 0a57 6520 6d61  ribution...We ma
-00003860: 6b65 2075 7365 206f 6620 5b74 6865 2047  ke use of [the G
-00003870: 6974 4875 6220 4469 7363 7573 7369 6f6e  itHub Discussion
-00003880: 7320 7061 6765 5d28 6874 7470 733a 2f2f  s page](https://
-00003890: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
-000038a0: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
-000038b0: 2f64 6973 6375 7373 696f 6e73 2920 746f  /discussions) to
-000038c0: 2067 6f20 6f76 6572 2070 6f74 656e 7469   go over potenti
-000038d0: 616c 2066 6561 7475 7265 7320 746f 2061  al features to a
-000038e0: 6464 2e20 506c 6561 7365 2066 6565 6c20  dd. Please feel 
-000038f0: 6672 6565 2074 6f20 7374 6f70 2062 7920  free to stop by 
-00003900: 6966 2079 6f75 2061 7265 206c 6f6f 6b69  if you are looki
-00003910: 6e67 2066 6f72 2073 6f6d 6574 6869 6e67  ng for something
-00003920: 2074 6f20 6465 7665 6c6f 7020 6f72 2068   to develop or h
-00003930: 6176 6520 616e 2069 6465 6120 666f 7220  ave an idea for 
-00003940: 6120 7573 6566 756c 2066 6561 7475 7265  a useful feature
-00003950: 210a 0a57 6865 6e20 7375 626d 6974 7469  !..When submitti
-00003960: 6e67 2061 2050 522c 2070 6c65 6173 6520  ng a PR, please 
-00003970: 6d61 726b 2079 6f75 7220 5052 2077 6974  mark your PR wit
-00003980: 6820 7468 6520 2250 5220 5265 6164 7920  h the "PR Ready 
-00003990: 666f 7220 5265 7669 6577 2220 6c61 6265  for Review" labe
-000039a0: 6c20 7768 656e 2079 6f75 2061 7265 2066  l when you are f
-000039b0: 696e 6973 6865 6420 6d61 6b69 6e67 2063  inished making c
-000039c0: 6861 6e67 6573 2073 6f20 7468 6174 2074  hanges so that t
-000039d0: 6865 2047 6974 4875 6220 6163 7469 6f6e  he GitHub action
-000039e0: 7320 626f 7473 2063 616e 2077 6f72 6b20  s bots can work 
-000039f0: 7468 6569 7220 6d61 6769 6321 0a0a 2323  their magic!..##
-00003a00: 2320 4465 7665 6c6f 7065 7220 496e 7374  # Developer Inst
-00003a10: 616c 6c0a 0a54 6f20 636f 6e74 7269 6275  all..To contribu
-00003a20: 7465 2074 6f20 7468 6520 6061 7374 6172  te to the `astar
-00003a30: 7465 7360 2073 6f75 7263 6520 636f 6465  tes` source code
-00003a40: 2c20 7374 6172 7420 6279 2063 6c6f 6e69  , start by cloni
-00003a50: 6e67 2074 6865 2072 6570 6f73 6974 6f72  ng the repositor
-00003a60: 7920 2869 2e65 2e20 6067 6974 2063 6c6f  y (i.e. `git clo
-00003a70: 6e65 2067 6974 4067 6974 6875 622e 636f  ne git@github.co
-00003a80: 6d3a 4a61 636b 736f 6e42 7572 6e73 2f61  m:JacksonBurns/a
-00003a90: 7374 6172 7465 732e 6769 7460 2920 616e  startes.git`) an
-00003aa0: 6420 7468 656e 2069 6e73 6964 6520 7468  d then inside th
-00003ab0: 6520 7265 706f 7369 746f 7279 2072 756e  e repository run
-00003ac0: 2060 7069 7020 696e 7374 616c 6c20 2d65   `pip install -e
-00003ad0: 202e 5b6d 6f6c 6563 756c 6573 2c64 6576   .[molecules,dev
-00003ae0: 5d60 2e20 5468 6973 2077 696c 6c20 7365  ]`. This will se
-00003af0: 7420 796f 7520 7570 2077 6974 6820 616c  t you up with al
-00003b00: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
-00003b10: 6570 656e 6465 6e63 6965 7320 746f 2072  ependencies to r
-00003b20: 756e 2060 6173 7461 7274 6573 6020 616e  un `astartes` an
-00003b30: 6420 636f 6e66 6f72 6d20 746f 206f 7572  d conform to our
-00003b40: 2066 6f72 6d61 7474 696e 6720 7374 616e   formatting stan
-00003b50: 6461 7264 7320 2860 626c 6163 6b60 2061  dards (`black` a
-00003b60: 6e64 2060 6973 6f72 7460 292c 2077 6869  nd `isort`), whi
-00003b70: 6368 2079 6f75 2063 616e 2063 6f6e 6669  ch you can confi
-00003b80: 6775 7265 2074 6f20 7275 6e20 6175 746f  gure to run auto
-00003b90: 6d61 7469 6361 6c6c 7920 696e 2076 7363  matically in vsc
-00003ba0: 6f64 6520 5b6c 696b 6520 7468 6973 5d28  ode [like this](
-00003bb0: 6874 7470 733a 2f2f 6d61 7263 6f62 656c  https://marcobel
-00003bc0: 6f2e 6d65 6469 756d 2e63 6f6d 2f73 6574  o.medium.com/set
-00003bd0: 7469 6e67 2d75 702d 7079 7468 6f6e 2d62  ting-up-python-b
-00003be0: 6c61 636b 2d6f 6e2d 7669 7375 616c 2d73  lack-on-visual-s
-00003bf0: 7475 6469 6f2d 636f 6465 2d35 3331 3865  tudio-code-5318e
-00003c00: 6261 3463 6430 3023 3a7e 3a74 6578 743d  ba4cd00#:~:text=
-00003c10: 476f 2532 3074 6f25 3230 7365 7474 696e  Go%20to%20settin
-00003c20: 6773 2532 3069 6e25 3230 796f 7572 2c25  gs%20in%20your,%
-00003c30: 4532 2538 3025 3944 2532 3061 6e64 2532  E2%80%9D%20and%2
-00003c40: 3073 656c 6563 7425 3230 2545 3225 3830  0select%20%E2%80
-00003c50: 2539 4362 6c61 636b 2545 3225 3830 2539  %9Cblack%E2%80%9
-00003c60: 442e 292e 0a0a 3e20 2a2a 4e6f 7465 2a2a  D.)...> **Note**
-00003c70: 0a3e 2057 696e 646f 7773 2050 6f77 6572  .> Windows Power
-00003c80: 7368 656c 6c20 616e 6420 4d61 634f 5320  shell and MacOS 
-00003c90: 4361 7461 6c69 6e61 206f 7220 6e65 7765  Catalina or newe
-00003ca0: 7220 6d61 7920 636f 6d70 6c61 696e 2061  r may complain a
-00003cb0: 626f 7574 2073 7175 6172 6520 6272 6163  bout square brac
-00003cc0: 6b65 7473 2c20 736f 2079 6f75 2077 696c  kets, so you wil
-00003cd0: 6c20 6e65 6564 2074 6f20 646f 7562 6c65  l need to double
-00003ce0: 2071 756f 7465 2074 6865 2060 6d6f 6c65   quote the `mole
-00003cf0: 6375 6c65 7360 2063 6f6d 6d61 6e64 2028  cules` command (
-00003d00: 692e 652e 2060 7069 7020 696e 7374 616c  i.e. `pip instal
-00003d10: 6c20 2261 7374 6172 7465 735b 6d6f 6c65  l "astartes[mole
-00003d20: 6375 6c65 732c 6465 765d 2260 290a 0a23  cules,dev]"`)..#
-00003d30: 2323 2055 6e69 7420 5465 7374 696e 670a  ## Unit Testing.
-00003d40: 416c 6c20 6f66 2074 6865 2074 6573 7473  All of the tests
-00003d50: 2069 6e20 6061 7374 6172 7465 7360 2061   in `astartes` a
-00003d60: 7265 2077 7269 7474 656e 2075 7369 6e67  re written using
-00003d70: 2074 6865 2062 7569 6c74 2d69 6e20 7079   the built-in py
-00003d80: 7468 6f6e 2060 756e 6974 7465 7374 6020  thon `unittest` 
-00003d90: 6d6f 6475 6c65 2028 746f 2061 6c6c 6f77  module (to allow
-00003da0: 2072 756e 6e69 6e67 2077 6974 686f 7574   running without
-00003db0: 2060 7079 7465 7374 6029 2062 7574 2077   `pytest`) but w
-00003dc0: 6520 5f68 6967 686c 795f 2072 6563 6f6d  e _highly_ recom
-00003dd0: 6d65 6e64 2075 7369 6e67 2060 7079 7465  mend using `pyte
-00003de0: 7374 602e 2054 6f20 6578 6563 7574 6520  st`. To execute 
-00003df0: 7468 6520 7465 7374 7320 6672 6f6d 2074  the tests from t
-00003e00: 6865 2060 6173 7461 7274 6573 6020 7265  he `astartes` re
-00003e10: 706f 7369 746f 7279 2c20 7369 6d70 6c79  pository, simply
-00003e20: 2074 7970 6520 6070 7974 6573 7460 2061   type `pytest` a
-00003e30: 6674 6572 2072 756e 6e69 6e67 2074 6865  fter running the
-00003e40: 2064 6576 656c 6f70 6572 2069 6e73 7461   developer insta
-00003e50: 6c6c 2028 6f72 2061 6c74 6572 6e61 7465  ll (or alternate
-00003e60: 6c79 2c20 6070 7974 6573 7420 2d76 6020  ly, `pytest -v` 
-00003e70: 666f 7220 6120 6d6f 7265 2068 656c 7066  for a more helpf
-00003e80: 756c 206f 7574 7075 7429 2e0a 0a23 2323  ul output)...###
-00003e90: 2041 6464 696e 6720 4e65 7720 5361 6d70   Adding New Samp
-00003ea0: 6c65 7273 0a41 6464 696e 6720 6120 6e65  lers.Adding a ne
-00003eb0: 7720 7361 6d70 6c65 7220 7368 6f75 6c64  w sampler should
-00003ec0: 2065 7874 656e 6420 7468 6520 6061 6273   extend the `abs
-00003ed0: 7472 6163 745f 7361 6d70 6c65 722e 7079  tract_sampler.py
-00003ee0: 6020 6162 7374 7261 6374 2062 6173 6520  ` abstract base 
-00003ef0: 636c 6173 732e 0a0a 4974 2063 616e 2062  class...It can b
-00003f00: 6520 6173 2073 696d 706c 6520 6173 2061  e as simple as a
-00003f10: 2070 6173 7374 6872 6f75 6768 2074 6f20   passthrough to 
-00003f20: 6120 616e 6f74 6865 7220 6074 7261 696e  a another `train
-00003f30: 5f74 6573 745f 7370 6c69 7460 2c20 6f72  _test_split`, or
-00003f40: 2069 7420 6361 6e20 6265 2061 6e20 6f72   it can be an or
-00003f50: 6967 696e 616c 2069 6d70 6c65 6d65 6e74  iginal implement
-00003f60: 6174 696f 6e20 7468 6174 2072 6573 756c  ation that resul
-00003f70: 7473 2069 6e20 5820 616e 6420 7920 6265  ts in X and y be
-00003f80: 696e 6720 7370 6c69 7420 696e 746f 2074  ing split into t
-00003f90: 776f 206c 6973 7473 2e20 5461 6b65 2061  wo lists. Take a
-00003fa0: 206c 6f6f 6b20 6174 2060 6173 7461 7274   look at `astart
-00003fb0: 6573 2f73 616d 706c 6572 732f 7261 6e64  es/samplers/rand
-00003fc0: 6f6d 5f73 706c 6974 2e70 7960 2066 6f72  om_split.py` for
-00003fd0: 2061 2062 6173 6963 2065 7861 6d70 6c65   a basic example
-00003fe0: 210a 0a41 6674 6572 2074 6865 2073 616d  !..After the sam
-00003ff0: 706c 6572 2068 6173 2062 6565 6e20 696d  pler has been im
-00004000: 706c 656d 656e 7465 642c 2061 6464 2069  plemented, add i
-00004010: 7420 746f 2060 5f5f 696e 6974 5f5f 2e70  t to `__init__.p
-00004020: 7960 2069 6e20 696e 2060 6173 7461 7274  y` in in `astart
-00004030: 6573 2f73 616d 706c 6572 7360 2061 6e64  es/samplers` and
-00004040: 2069 7420 7769 6c6c 2061 7574 6f6d 6174   it will automat
-00004050: 6963 616c 6c79 2062 6520 756e 6974 2074  ically be unit t
-00004060: 6573 7465 642e 2041 6464 6974 696f 6e61  ested. Additiona
-00004070: 6c20 756e 6974 2074 6573 7473 2074 6f20  l unit tests to 
-00004080: 7665 7269 6679 2074 6861 7420 6879 7065  verify that hype
-00004090: 7270 6172 616d 6574 6572 7320 6361 6e20  rparameters can 
-000040a0: 6265 2070 726f 7065 726c 7920 7061 7373  be properly pass
-000040b0: 6564 2c20 6574 632e 2061 7265 2061 6c73  ed, etc. are als
-000040c0: 6f20 7265 636f 6d6d 656e 6465 642e 0a0a  o recommended...
-000040d0: 466f 7220 6869 7374 6f72 6963 616c 2072  For historical r
-000040e0: 6561 736f 6e73 2c20 616e 6420 6173 2061  easons, and as a
-000040f0: 2067 7569 6465 2066 6f72 2061 6e79 2064   guide for any d
-00004100: 6576 656c 6f70 6572 7320 7768 6f20 776f  evelopers who wo
-00004110: 756c 6420 6c69 6b65 2061 6464 206e 6577  uld like add new
-00004120: 2073 616d 706c 6572 732c 2062 656c 6f77   samplers, below
-00004130: 2069 7320 6120 7275 6e6e 696e 6720 6c69   is a running li
-00004140: 7374 206f 6620 7361 6d70 6c65 7273 2077  st of samplers w
-00004150: 6869 6368 2068 6176 6520 6265 656e 205f  hich have been _
-00004160: 636f 6e73 6964 6572 6564 5f20 666f 7220  considered_ for 
-00004170: 6164 6469 7469 6f6e 2074 6f20 6061 7361  addition to `asa
-00004180: 7274 6573 6020 6275 7420 756c 7469 6d61  rtes` but ultima
-00004190: 7465 6c79 206e 6f74 2061 6464 6564 2066  tely not added f
-000041a0: 6f72 2076 6172 696f 7573 2072 6561 736f  or various reaso
-000041b0: 6e73 2e0a 0a23 2323 2320 4e6f 7420 496d  ns...#### Not Im
-000041c0: 706c 656d 656e 7465 6420 5361 6d70 6c69  plemented Sampli
-000041d0: 6e67 2041 6c67 6f72 6974 686d 730a 0a7c  ng Algorithms..|
-000041e0: 2053 616d 706c 6572 204e 616d 6520 7c20   Sampler Name | 
-000041f0: 5265 6173 6f6e 696e 6720 7c20 5265 6c65  Reasoning | Rele
-00004200: 7661 6e74 204c 696e 6b28 7329 207c 0a7c  vant Link(s) |.|
-00004210: 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d 2d7c 0a7c  :---:|---|---|.|
-00004220: 2044 2d4f 7074 696d 616c 207c 2052 6571   D-Optimal | Req
-00004230: 7569 7265 7320 5f61 2d70 7269 6f72 695f  uires _a-priori_
-00004240: 206b 6e6f 776c 6564 6765 206f 6620 7468   knowledge of th
-00004250: 6520 7465 7374 2061 6e64 2074 7261 696e  e test and train
-00004260: 2073 697a 6520 7768 6963 6820 646f 6573   size which does
-00004270: 206e 6f74 2066 6974 2069 6e20 7468 6520   not fit in the 
-00004280: 6061 7374 6172 7465 7360 2066 7261 6d65  `astartes` frame
-00004290: 776f 726b 2028 7361 6d70 6c65 7273 2061  work (samplers a
-000042a0: 7265 2061 6c6c 2061 676e 6f73 7469 6320  re all agnostic 
-000042b0: 746f 2074 6865 2073 697a 6520 6f66 2074  to the size of t
-000042c0: 6865 2073 6574 7329 2061 6e64 2069 7420  he sets) and it 
-000042d0: 6973 2071 7565 7374 696f 6e61 626c 6520  is questionable 
-000042e0: 6966 2074 6865 2075 7365 206f 6620 7468  if the use of th
-000042f0: 6520 4669 7363 6865 7220 696e 666f 726d  e Fischer inform
-00004300: 6174 696f 6e20 6d61 7472 6978 2069 7320  ation matrix is 
-00004310: 6163 7475 616c 6c79 206d 6561 6e69 6e67  actually meaning
-00004320: 6675 6c20 696e 2074 6865 2063 6f6e 7465  ful in the conte
-00004330: 7874 206f 6620 7361 6d70 6c69 6e67 2065  xt of sampling e
-00004340: 7869 7374 696e 6720 6461 7461 2072 6174  xisting data rat
-00004350: 6865 7220 7468 616e 2074 756e 696e 6720  her than tuning 
-00004360: 666f 7220 6964 6561 6c20 6461 7461 2e20  for ideal data. 
-00004370: 7c20 5468 6520 5b57 696b 6970 6564 6961  | The [Wikipedia
-00004380: 2061 7274 6963 6c65 2066 6f72 206f 7074   article for opt
-00004390: 696d 616c 2064 6573 6967 6e5d 2868 7474  imal design](htt
-000043a0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000043b0: 612e 6f72 672f 7769 6b69 2f4f 7074 696d  a.org/wiki/Optim
-000043c0: 616c 5f64 6573 6967 6e23 3a7e 3a74 6578  al_design#:~:tex
-000043d0: 743d 4f66 2532 3063 6f75 7273 6525 3243  t=Of%20course%2C
-000043e0: 2532 3066 6978 696e 6725 3230 7468 6525  %20fixing%20the%
-000043f0: 3230 6e75 6d62 6572 2532 306f 6625 3230  20number%20of%20
-00004400: 6578 7065 7269 6d65 6e74 616c 2532 3072  experimental%20r
-00004410: 756e 7325 3230 6125 3230 7072 696f 7269  uns%20a%20priori
-00004420: 2532 3077 6f75 6c64 2532 3062 6525 3230  %20would%20be%20
-00004430: 696d 7072 6163 7469 6361 6c2e 2920 646f  impractical.) do
-00004440: 6573 2061 2067 6f6f 6420 6a6f 6220 6578  es a good job ex
-00004450: 706c 6169 6e69 6e67 2077 6879 2074 6869  plaining why thi
-00004460: 7320 6973 2064 6966 6669 6375 6c74 2c20  s is difficult, 
-00004470: 616e 6420 706f 696e 7473 2061 7420 736f  and points at so
-00004480: 6d65 2070 6f74 656e 7469 616c 2061 6c74  me potential alt
-00004490: 6572 6e61 7469 7665 732e 207c 0a7c 2044  ernatives. |.| D
-000044a0: 7570 6c65 7820 7c20 5265 7175 6972 6573  uplex | Requires
-000044b0: 206b 6e6f 7769 6e67 2074 6573 7420 616e   knowing test an
-000044c0: 6420 7472 6169 6e20 7369 7a65 2062 6566  d train size bef
-000044d0: 6f72 6520 6578 6563 7574 696f 6e2c 2061  ore execution, a
-000044e0: 6e64 2063 616e 206f 6e6c 7920 7061 7274  nd can only part
-000044f0: 6974 696f 6e20 6461 7461 2069 6e74 6f20  ition data into 
-00004500: 7477 6f20 7365 7473 2077 6869 6368 2077  two sets which w
-00004510: 6f75 6c64 206d 616b 6520 6974 2069 6e63  ould make it inc
-00004520: 6f6d 7061 7469 626c 6520 7769 7468 2060  ompatible with `
-00004530: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
-00004540: 706c 6974 602e 207c 2054 6869 7320 5b69  plit`. | This [i
-00004550: 6d70 6c65 6d65 6e74 6174 696f 6e20 696e  mplementation in
-00004560: 2052 5d28 6874 7470 733a 2f2f 7365 6172   R](https://sear
-00004570: 6368 2e72 2d70 726f 6a65 6374 2e6f 7267  ch.r-project.org
-00004580: 2f43 5241 4e2f 7265 666d 616e 732f 7072  /CRAN/refmans/pr
-00004590: 6f73 7065 6374 722f 6874 6d6c 2f64 7570  ospectr/html/dup
-000045a0: 6c65 782e 6874 6d6c 233a 7e3a 7465 7874  lex.html#:~:text
-000045b0: 3d54 6865 2532 3044 5550 4c45 5825 3230  =The%20DUPLEX%20
-000045c0: 616c 676f 7269 7468 6d25 3230 6973 2532  algorithm%20is%2
-000045d0: 3073 696d 696c 6172 2c74 6861 7425 3230  0similar,that%20
-000045e0: 6172 6525 3230 7468 6525 3230 6661 7274  are%20the%20fart
-000045f0: 6865 7374 2532 3061 7061 7274 2e29 2069  hest%20apart.) i
-00004600: 6e63 6c75 6465 7320 6865 6c70 6675 6c20  ncludes helpful 
-00004610: 7265 6665 7265 6e63 6573 2061 6e64 2061  references and a
-00004620: 2072 6566 6572 656e 6365 2069 6d70 6c65   reference imple
-00004630: 6d65 6e74 6174 696f 6e2e 207c 0a0a 2323  mentation. |..##
-00004640: 2320 4164 6469 6e67 204e 6577 2046 6561  # Adding New Fea
-00004650: 7475 7269 7a61 7469 6f6e 2053 6368 656d  turization Schem
-00004660: 6573 0a41 6c6c 206f 6620 7468 6520 7361  es.All of the sa
-00004670: 6d70 6c69 6e67 206d 6574 686f 6473 2069  mpling methods i
-00004680: 6d70 6c65 6d65 6e74 6564 2069 6e20 6061  mplemented in `a
-00004690: 7374 6172 7465 7360 2061 6363 6570 7420  startes` accept 
-000046a0: 6172 6269 7472 6172 7920 6172 7261 7973  arbitrary arrays
-000046b0: 206f 6620 6e75 6d62 6572 7320 616e 6420   of numbers and 
-000046c0: 7265 7475 726e 2074 6865 2073 616d 706c  return the sampl
-000046d0: 6564 2067 726f 7570 7320 2877 6974 6820  ed groups (with 
-000046e0: 7468 6520 6578 6365 7074 696f 6e20 6f66  the exception of
-000046f0: 2060 5363 6166 666f 6c64 2e70 7960 292e   `Scaffold.py`).
-00004700: 2049 6620 796f 7520 6861 7665 2061 6e20   If you have an 
-00004710: 6578 6973 7469 6e67 2066 6561 7475 7269  existing featuri
-00004720: 7a61 7469 6f6e 2073 6368 656d 6520 2869  zation scheme (i
-00004730: 2e65 2e20 7461 6b65 2061 6e20 6172 6269  .e. take an arbi
-00004740: 7472 6172 7920 696e 7075 7420 616e 6420  trary input and 
-00004750: 7475 726e 2069 7420 696e 746f 2061 6e20  turn it into an 
-00004760: 6172 7261 7920 6f66 206e 756d 6265 7273  array of numbers
-00004770: 292c 2077 6520 776f 756c 6420 6265 2074  ), we would be t
-00004780: 6872 696c 6c65 6420 746f 2069 6e63 6c75  hrilled to inclu
-00004790: 6465 2069 7420 696e 2060 6173 7461 7274  de it in `astart
-000047a0: 6573 602e 0a0a 4164 6469 6e67 2061 206e  es`...Adding a n
-000047b0: 6577 2069 6e74 6572 6661 6365 2073 686f  ew interface sho
-000047c0: 756c 6420 7461 6b65 206f 6e20 7468 6973  uld take on this
-000047d0: 2066 6f72 6d61 743a 0a0a 6060 6070 7974   format:..```pyt
-000047e0: 686f 6e0a 6672 6f6d 2061 7374 6172 7465  hon.from astarte
-000047f0: 7320 696d 706f 7274 2074 7261 696e 5f74  s import train_t
-00004800: 6573 745f 7370 6c69 740a 0a64 6566 2074  est_split..def t
-00004810: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
-00004820: 494e 5445 5246 4143 4528 0a20 2020 2049  INTERFACE(.    I
-00004830: 4e54 4552 4641 4345 5f69 6e70 7574 2c0a  NTERFACE_input,.
-00004840: 2020 2020 494e 5445 5246 4143 455f 4152      INTERFACE_AR
-00004850: 4753 2c0a 2020 2020 793a 206e 702e 6172  GS,.    y: np.ar
-00004860: 7261 7920 3d20 4e6f 6e65 2c0a 2020 2020  ray = None,.    
-00004870: 6c61 6265 6c73 3a20 6e70 2e61 7272 6179  labels: np.array
-00004880: 203d 204e 6f6e 652c 0a20 2020 2074 6573   = None,.    tes
-00004890: 745f 7369 7a65 3a20 666c 6f61 7420 3d20  t_size: float = 
-000048a0: 302e 3235 2c0a 2020 2020 7472 6169 6e5f  0.25,.    train_
-000048b0: 7369 7a65 3a20 666c 6f61 7420 3d20 302e  size: float = 0.
-000048c0: 3735 2c0a 2020 2020 7370 6c69 7474 6572  75,.    splitter
-000048d0: 3a20 7374 7220 3d20 2772 616e 646f 6d27  : str = 'random'
-000048e0: 2c0a 2020 2020 686f 7074 733a 2064 6963  ,.    hopts: dic
-000048f0: 7420 3d20 7b7d 2c0a 2020 2020 494e 5445  t = {},.    INTE
-00004900: 5246 4143 455f 686f 7074 733a 2064 6963  RFACE_hopts: dic
-00004910: 7420 3d20 7b7d 2c0a 293a 0a20 2020 2023  t = {},.):.    #
-00004920: 2074 7572 6e20 7468 6520 494e 5445 5246   turn the INTERF
-00004930: 4143 455f 696e 7075 7420 696e 746f 2061  ACE_input into a
-00004940: 6e20 696e 7075 7420 580a 2020 2020 2320  n input X.    # 
-00004950: 6261 7365 6420 6f6e 2049 4e54 4552 4641  based on INTERFA
-00004960: 4345 2041 5247 5320 7768 6572 6520 494e  CE ARGS where IN
-00004970: 5445 5246 4143 455f 686f 7074 730a 2020  TERFACE_hopts.  
-00004980: 2020 2320 7370 6563 6966 6965 7320 6164    # specifies ad
-00004990: 6469 7469 6f6e 616c 2062 6568 6176 696f  ditional behavio
-000049a0: 720a 2020 2020 5820 3d20 5b5d 0a20 2020  r.    X = [].   
-000049b0: 200a 2020 2020 2320 6361 6c6c 2074 7261   .    # call tra
-000049c0: 696e 2074 6573 7420 7370 6c69 7420 7769  in test split wi
-000049d0: 7468 2074 6869 7320 696e 7075 740a 2020  th this input.  
-000049e0: 2020 7265 7475 726e 2074 7261 696e 5f74    return train_t
-000049f0: 6573 745f 7370 6c69 7428 0a20 2020 2020  est_split(.     
-00004a00: 2020 2058 2c0a 2020 2020 2020 2020 793d     X,.        y=
-00004a10: 792c 0a20 2020 2020 2020 206c 6162 656c  y,.        label
-00004a20: 733d 6c61 6265 6c73 2c0a 2020 2020 2020  s=labels,.      
-00004a30: 2020 7465 7374 5f73 697a 653d 7465 7374    test_size=test
-00004a40: 5f73 697a 652c 0a20 2020 2020 2020 2074  _size,.        t
-00004a50: 7261 696e 5f73 697a 653d 7472 6169 6e5f  rain_size=train_
-00004a60: 7369 7a65 2c0a 2020 2020 2020 2020 7370  size,.        sp
-00004a70: 6c69 7474 6572 3d73 706c 6974 7465 722c  litter=splitter,
-00004a80: 0a20 2020 2020 2020 2068 6f70 7473 3d68  .        hopts=h
-00004a90: 6f70 7473 2c0a 2020 2020 290a 6060 600a  opts,.    ).```.
-00004aa0: 0a49 6620 706f 7373 6962 6c65 2c20 7765  .If possible, we
-00004ab0: 2077 6f75 6c64 206c 696b 6520 746f 2061   would like to a
-00004ac0: 6c73 6f20 6164 6420 616e 2065 7861 6d70  lso add an examp
-00004ad0: 6c65 204a 7570 7974 6572 204e 6f74 6562  le Jupyter Noteb
-00004ae0: 6f6f 6b20 7769 7468 2061 6e79 206e 6577  ook with any new
-00004af0: 2069 6e74 6572 6661 6365 2074 6f20 6465   interface to de
-00004b00: 6d6f 6e73 7472 6174 6520 746f 206e 6577  monstrate to new
-00004b10: 2075 7365 7273 2068 6f77 2069 7420 6675   users how it fu
-00004b20: 6e63 7469 6f6e 732e 2053 6565 206f 7572  nctions. See our
-00004b30: 206f 7468 6572 2065 7861 6d70 6c65 7320   other examples 
-00004b40: 696e 2074 6865 2060 6578 616d 706c 6573  in the `examples
-00004b50: 6020 6469 7265 6374 6f72 792e 0a0a 436f  ` directory...Co
-00004b60: 6e74 6163 7420 5b40 4a61 636b 736f 6e42  ntact [@JacksonB
-00004b70: 7572 6e73 5d28 6874 7470 733a 2f2f 6769  urns](https://gi
-00004b80: 7468 7562 2e63 6f6d 2f4a 6163 6b73 6f6e  thub.com/Jackson
-00004b90: 4275 726e 7329 2069 6620 796f 7520 6e65  Burns) if you ne
-00004ba0: 6564 2061 7373 6973 7461 6e63 6520 6164  ed assistance ad
-00004bb0: 6469 6e67 2061 6e20 6578 6973 7469 6e67  ding an existing
-00004bc0: 2077 6f72 6b66 6c6f 7720 746f 2060 6173   workflow to `as
-00004bd0: 7461 7274 6573 602e 2049 6620 7468 6973  tartes`. If this
-00004be0: 2066 6561 7475 7269 7a61 7469 6f6e 2073   featurization s
-00004bf0: 6368 656d 6520 7265 7175 6972 6573 2061  cheme requires a
-00004c00: 6464 6974 696f 6e61 6c20 6465 7065 6e64  dditional depend
-00004c10: 656e 6369 6573 2074 6f20 6675 6e63 7469  encies to functi
-00004c20: 6f6e 2c20 7765 206d 6179 2061 6464 2069  on, we may add i
-00004c30: 7420 6173 2061 6e20 6164 6469 7469 6f6e  t as an addition
-00004c40: 616c 205f 6578 7472 615f 2070 6163 6b61  al _extra_ packa
-00004c50: 6765 2069 6e20 7468 6520 7361 6d65 2077  ge in the same w
-00004c60: 6179 2074 6861 7420 606d 6f6c 6563 756c  ay that `molecul
-00004c70: 6573 6020 696e 2069 6e73 7461 6c6c 6564  es` in installed
-00004c80: 2e0a 0a23 2320 4a4f 5353 2042 7261 6e63  ...## JOSS Branc
-00004c90: 680a 0a60 6173 7461 7274 6573 6020 636f  h..`astartes` co
-00004ca0: 7272 6573 706f 6e64 696e 6720 4a4f 5353  rresponding JOSS
-00004cb0: 2070 6170 6572 2069 7320 7374 6f72 6564   paper is stored
-00004cc0: 2069 6e20 7468 6973 2072 6570 6f73 6974   in this reposit
-00004cd0: 6f72 7920 6f6e 2061 2073 6570 6172 6174  ory on a separat
-00004ce0: 6520 6272 616e 6368 2e20 596f 7520 6361  e branch. You ca
-00004cf0: 6e20 6669 6e64 2060 7061 7065 722e 6d64  n find `paper.md
-00004d00: 6020 6f6e 2074 6865 2061 7074 6c79 206e  ` on the aptly n
-00004d10: 616d 6564 2060 6a6f 7373 2d70 6170 6572  amed `joss-paper
-00004d20: 6020 6272 616e 6368 2e20 0a0a 5f4e 6f74  ` branch. .._Not
-00004d30: 6520 666f 7220 4d61 696e 7461 696e 6572  e for Maintainer
-00004d40: 735f 3a20 546f 2070 7573 6820 6368 616e  s_: To push chan
-00004d50: 6765 7320 6672 6f6d 2074 6865 2060 6d61  ges from the `ma
-00004d60: 696e 6020 6272 616e 6368 2069 6e74 6f20  in` branch into 
-00004d70: 7468 6520 606a 6f73 732d 7061 7065 7260  the `joss-paper`
-00004d80: 2062 7261 6e63 682c 2072 756e 2074 6865   branch, run the
-00004d90: 2060 5570 6461 7465 204a 4f53 5320 4272   `Update JOSS Br
-00004da0: 616e 6368 6020 776f 726b 666c 6f77 2e0a  anch` workflow..
-00004db0: 0a                                       .
+00000480: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000490: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3532  ://doi.org/10.52
+000004a0: 3831 2f7a 656e 6f64 6f2e 3831 3437 3230  81/zenodo.814720
+000004b0: 3522 3e3c 696d 6720 7372 633d 2268 7474  5"><img src="htt
+000004c0: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
+000004d0: 6261 6467 652f 444f 492f 3130 2e35 3238  badge/DOI/10.528
+000004e0: 312f 7a65 6e6f 646f 2e38 3134 3732 3035  1/zenodo.8147205
+000004f0: 2e73 7667 2220 616c 743d 2244 4f49 223e  .svg" alt="DOI">
+00000500: 3c2f 613e 0a3c 2f70 3e0a 0a23 2320 4f6e  </a>.</p>..## On
+00000510: 6c69 6e65 2044 6f63 756d 656e 7461 7469  line Documentati
+00000520: 6f6e 0a46 6f6c 6c6f 7720 5b74 6869 7320  on.Follow [this 
+00000530: 6c69 6e6b 5d28 6874 7470 733a 2f2f 4a61  link](https://Ja
+00000540: 636b 736f 6e42 7572 6e73 2e67 6974 6875  cksonBurns.githu
+00000550: 622e 696f 2f61 7374 6172 7465 732f 2920  b.io/astartes/) 
+00000560: 666f 7220 6120 6e69 6365 6c79 2d72 656e  for a nicely-ren
+00000570: 6465 7265 6420 7665 7273 696f 6e20 6f66  dered version of
+00000580: 2074 6869 7320 5245 4144 4d45 2061 6c6f   this README alo
+00000590: 6e67 2077 6974 6820 6164 6469 7469 6f6e  ng with addition
+000005a0: 616c 2074 7574 6f72 6961 6c73 2066 6f72  al tutorials for
+000005b0: 205b 6d6f 7669 6e67 2066 726f 6d20 7472   [moving from tr
+000005c0: 6169 6e5f 7465 7374 5f73 706c 6974 2069  ain_test_split i
+000005d0: 6e20 736b 6c65 6172 6e20 746f 2061 7374  n sklearn to ast
+000005e0: 6172 7465 735d 2868 7474 7073 3a2f 2f6a  artes](https://j
+000005f0: 6163 6b73 6f6e 6275 726e 732e 6769 7468  acksonburns.gith
+00000600: 7562 2e69 6f2f 6173 7461 7274 6573 2f73  ub.io/astartes/s
+00000610: 6b6c 6561 726e 5f74 6f5f 6173 7461 7274  klearn_to_astart
+00000620: 6573 2e68 746d 6c29 2e0a 4b65 6570 2072  es.html)..Keep r
+00000630: 6561 6469 6e67 2066 6f72 2061 2069 6e73  eading for a ins
+00000640: 7461 6c6c 6174 696f 6e20 6775 6964 6520  tallation guide 
+00000650: 616e 6420 6c69 6e6b 7320 746f 2074 7574  and links to tut
+00000660: 6f72 6961 6c73 210a 0a23 2320 496e 7374  orials!..## Inst
+00000670: 616c 6c69 6e67 2060 6173 7461 7274 6573  alling `astartes
+00000680: 600a 5765 2072 6563 6f6d 6d65 6e64 2069  `.We recommend i
+00000690: 6e73 7461 6c6c 696e 6720 6061 7374 6172  nstalling `astar
+000006a0: 7465 7360 2077 6974 6869 6e20 6120 7669  tes` within a vi
+000006b0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+000006c0: 742c 2075 7369 6e67 2065 6974 6865 7220  t, using either 
+000006d0: 6076 656e 7660 206f 7220 6063 6f6e 6461  `venv` or `conda
+000006e0: 6020 286f 7220 6f74 6865 7220 746f 6f6c  ` (or other tool
+000006f0: 7329 2074 6f20 7369 6d70 6c69 6679 2064  s) to simplify d
+00000700: 6570 656e 6465 6e63 7920 6d61 6e61 6765  ependency manage
+00000710: 6d65 6e74 2e20 5079 7468 6f6e 2076 6572  ment. Python ver
+00000720: 7369 6f6e 7320 332e 372c 2033 2e38 2c20  sions 3.7, 3.8, 
+00000730: 332e 392c 2033 2e31 302c 2061 6e64 2033  3.9, 3.10, and 3
+00000740: 2e31 3120 6172 6520 7375 7070 6f72 7465  .11 are supporte
+00000750: 6420 6f6e 2061 6c6c 2070 6c61 7466 6f72  d on all platfor
+00000760: 6d73 2e0a 0a60 6173 7461 7274 6573 6020  ms...`astartes` 
+00000770: 6973 2061 7661 696c 6162 6c65 206f 6e20  is available on 
+00000780: 6050 7950 4960 2061 6e64 2063 616e 2062  `PyPI` and can b
+00000790: 6520 696e 7374 616c 6c65 6420 7573 696e  e installed usin
+000007a0: 6720 6070 6970 603a 0a0a 202d 2054 6f20  g `pip`:.. - To 
+000007b0: 696e 636c 7564 6520 7468 6520 6665 6174  include the feat
+000007c0: 7572 697a 6174 696f 6e20 6f70 7469 6f6e  urization option
+000007d0: 7320 666f 7220 6368 656d 6963 616c 2064  s for chemical d
+000007e0: 6174 612c 2075 7365 2060 7069 7020 696e  ata, use `pip in
+000007f0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
+00000800: 6f6c 6563 756c 6573 5d60 2e0a 202d 2054  olecules]`.. - T
+00000810: 6f20 696e 7374 616c 6c20 6f6e 6c79 2074  o install only t
+00000820: 6865 2073 616d 706c 696e 6720 616c 676f  he sampling algo
+00000830: 7269 7468 6d73 2c20 7573 6520 6070 6970  rithms, use `pip
+00000840: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
+00000850: 7360 2028 7468 6973 2069 6e73 7461 6c6c  s` (this install
+00000860: 2077 696c 6c20 6861 7665 2066 6577 6572   will have fewer
+00000870: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
+00000880: 6420 6d61 7920 6265 206d 6f72 6520 7265  d may be more re
+00000890: 6164 696c 7920 636f 6d70 6174 6962 6c65  adily compatible
+000008a0: 2069 6e20 656e 7669 726f 6e6d 656e 7473   in environments
+000008b0: 2077 6974 6820 6578 6973 7469 6e67 2077   with existing w
+000008c0: 6f72 6b66 6c6f 7773 292e 0a0a 5468 6520  orkflows)...The 
+000008d0: 6261 7365 2060 6173 7461 7274 6573 6020  base `astartes` 
+000008e0: 7061 636b 6167 6520 6973 2061 6c73 6f20  package is also 
+000008f0: 6176 6169 6c61 626c 6520 6f6e 2060 636f  available on `co
+00000900: 6e64 6160 2077 6974 6820 7468 6973 2063  nda` with this c
+00000910: 6f6d 6d61 6e64 3a20 6063 6f6e 6461 2069  ommand: `conda i
+00000920: 6e73 7461 6c6c 202d 6320 6a61 636b 736f  nstall -c jackso
+00000930: 6e62 7572 6e73 2061 7374 6172 7465 7360  nburns astartes`
+00000940: 2e0a 4e6f 7465 2074 6861 7420 7468 6973  ..Note that this
+00000950: 2070 6163 6b61 6765 205f 646f 6573 206e   package _does n
+00000960: 6f74 5f20 696e 636c 7564 6520 6275 696c  ot_ include buil
+00000970: 742d 696e 2073 7570 706f 7274 2066 6f72  t-in support for
+00000980: 2066 6561 7475 7269 7a69 6e67 206d 6f6c   featurizing mol
+00000990: 6563 756c 6573 2c20 7768 6963 6820 6973  ecules, which is
+000009a0: 2063 7572 7265 6e74 6c79 206f 6e6c 7920   currently only 
+000009b0: 6176 6169 6c61 626c 6520 6672 6f6d 2074  available from t
+000009c0: 6865 2050 7950 4920 7061 636b 6167 6520  he PyPI package 
+000009d0: 6f72 2061 2073 6f75 7263 6520 696e 7374  or a source inst
+000009e0: 616c 6c2e 0a0a 3e20 2a2a 4e6f 7465 2a2a  all...> **Note**
+000009f0: 0a3e 2057 696e 646f 7773 2050 6f77 6572  .> Windows Power
+00000a00: 7368 656c 6c20 616e 6420 4d61 634f 5320  shell and MacOS 
+00000a10: 4361 7461 6c69 6e61 206f 7220 6e65 7765  Catalina or newe
+00000a20: 7220 6d61 7920 636f 6d70 6c61 696e 2061  r may complain a
+00000a30: 626f 7574 2073 7175 6172 6520 6272 6163  bout square brac
+00000a40: 6b65 7473 2c20 736f 2079 6f75 2077 696c  kets, so you wil
+00000a50: 6c20 6e65 6564 2074 6f20 646f 7562 6c65  l need to double
+00000a60: 2071 756f 7465 2074 6865 2060 6d6f 6c65   quote the `mole
+00000a70: 6375 6c65 7360 2063 6f6d 6d61 6e64 2028  cules` command (
+00000a80: 692e 652e 2060 7069 7020 696e 7374 616c  i.e. `pip instal
+00000a90: 6c20 2261 7374 6172 7465 735b 6d6f 6c65  l "astartes[mole
+00000aa0: 6375 6c65 735d 2260 290a 0a54 6f20 696e  cules]"`)..To in
+00000ab0: 7374 616c 6c20 6061 7374 6172 7465 7360  stall `astartes`
+00000ac0: 2066 726f 6d20 736f 7572 6365 2c20 7365   from source, se
+00000ad0: 6520 7468 6520 5b43 6f6e 7472 6962 7574  e the [Contribut
+00000ae0: 696e 6720 2620 4465 7665 6c6f 7065 7220  ing & Developer 
+00000af0: 4e6f 7465 735d 2823 636f 6e74 7269 6275  Notes](#contribu
+00000b00: 7469 6e67 2d2d 6465 7665 6c6f 7065 722d  ting--developer-
+00000b10: 6e6f 7465 7329 2073 6563 7469 6f6e 2e0a  notes) section..
+00000b20: 0a23 2320 5175 6963 6b20 5374 6172 740a  .## Quick Start.
+00000b30: 6061 7374 6172 7465 7360 2069 7320 6465  `astartes` is de
+00000b40: 7369 676e 6564 2061 7320 6120 6472 6f70  signed as a drop
+00000b50: 2d69 6e20 7265 706c 6163 656d 656e 7420  -in replacement 
+00000b60: 666f 7220 6073 6b6c 6561 726e 6027 7320  for `sklearn`'s 
+00000b70: 6074 7261 696e 5f74 6573 745f 7370 6c69  `train_test_spli
+00000b80: 7460 2066 756e 6374 696f 6e20 2873 6565  t` function (see
+00000b90: 2074 6865 205b 736b 6c65 6172 6e20 646f   the [sklearn do
+00000ba0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000bb0: 7073 3a2f 2f73 6369 6b69 742d 6c65 6172  ps://scikit-lear
+00000bc0: 6e2e 6f72 672f 7374 6162 6c65 2f6d 6f64  n.org/stable/mod
+00000bd0: 756c 6573 2f67 656e 6572 6174 6564 2f73  ules/generated/s
+00000be0: 6b6c 6561 726e 2e6d 6f64 656c 5f73 656c  klearn.model_sel
+00000bf0: 6563 7469 6f6e 2e74 7261 696e 5f74 6573  ection.train_tes
+00000c00: 745f 7370 6c69 742e 6874 6d6c 2929 2e20  t_split.html)). 
+00000c10: 546f 2073 7769 7463 6820 746f 2060 6173  To switch to `as
+00000c20: 7461 7274 6573 602c 2063 6861 6e67 6520  tartes`, change 
+00000c30: 6066 726f 6d20 736b 6c65 6172 6e2e 6d6f  `from sklearn.mo
+00000c40: 6465 6c5f 7365 6c65 6374 696f 6e20 696d  del_selection im
+00000c50: 706f 7274 2074 7261 696e 5f74 6573 745f  port train_test_
+00000c60: 7370 6c69 7460 2074 6f20 6066 726f 6d20  split` to `from 
+00000c70: 6173 7461 7274 6573 2069 6d70 6f72 7420  astartes import 
+00000c80: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
+00000c90: 602e 0a0a 4c69 6b65 2060 736b 6c65 6172  `...Like `sklear
+00000ca0: 6e60 2c20 6061 7374 6172 7465 7360 2061  n`, `astartes` a
+00000cb0: 6363 6570 7473 2061 6e79 2069 7465 7261  ccepts any itera
+00000cc0: 626c 6520 6f62 6a65 6374 2061 7320 6058  ble object as `X
+00000cd0: 602c 2060 7960 2c20 616e 6420 606c 6162  `, `y`, and `lab
+00000ce0: 656c 7360 2e0a 4561 6368 2077 696c 6c20  els`..Each will 
+00000cf0: 6265 2063 6f6e 7665 7274 6564 2074 6f20  be converted to 
+00000d00: 6120 606e 756d 7079 6020 6172 7261 7920  a `numpy` array 
+00000d10: 666f 7220 696e 7465 726e 616c 206f 7065  for internal ope
+00000d20: 7261 7469 6f6e 732c 2061 6e64 2072 6574  rations, and ret
+00000d30: 7572 6e65 6420 6173 2061 2060 6e75 6d70  urned as a `nump
+00000d40: 7960 2061 7272 6179 2077 6974 6820 6c69  y` array with li
+00000d50: 6d69 7465 6420 6578 6365 7074 696f 6e73  mited exceptions
+00000d60: 3a20 6966 2060 5860 2069 7320 6120 6070  : if `X` is a `p
+00000d70: 616e 6461 7360 2060 4461 7461 4672 616d  andas` `DataFram
+00000d80: 6560 2c20 6079 6020 6973 2061 2060 5365  e`, `y` is a `Se
+00000d90: 7269 6573 602c 206f 7220 606c 6162 656c  ries`, or `label
+00000da0: 7360 2069 7320 6120 6053 6572 6965 7360  s` is a `Series`
+00000db0: 2c20 6061 7374 6172 7465 7360 2077 696c  , `astartes` wil
+00000dc0: 6c20 6361 7374 2069 7420 6261 636b 2074  l cast it back t
+00000dd0: 6f20 6974 7320 6f72 6967 696e 616c 2074  o its original t
+00000de0: 7970 6520 696e 636c 7564 696e 6720 6974  ype including it
+00000df0: 7320 696e 6465 7820 616e 6420 636f 6c75  s index and colu
+00000e00: 6d6e 206e 616d 6573 2e0a 0a3e 202a 2a4e  mn names...> **N
+00000e10: 6f74 652a 2a0a 3e20 5468 6520 6465 7665  ote**.> The deve
+00000e20: 6c6f 7065 7273 2072 6563 6f6d 6d65 6e64  lopers recommend
+00000e30: 2070 6173 7369 6e67 2060 5860 2c20 6079   passing `X`, `y
+00000e40: 602c 2061 6e64 2060 6c61 6265 6c73 6020  `, and `labels` 
+00000e50: 6173 2060 6e75 6d70 7960 2061 7272 6179  as `numpy` array
+00000e60: 7320 616e 6420 6861 6e64 6c69 6e67 2074  s and handling t
+00000e70: 6865 2063 6f6e 7665 7273 696f 6e20 746f  he conversion to
+00000e80: 2061 6e64 2066 726f 6d20 6f74 6865 7220   and from other 
+00000e90: 7479 7065 7320 6578 706c 6963 6974 7920  types explicity 
+00000ea0: 6f6e 2079 6f75 7220 6f77 6e2e 2042 6568  on your own. Beh
+00000eb0: 696e 642d 7468 652d 7363 656e 6573 2074  ind-the-scenes t
+00000ec0: 7970 6520 6361 7374 696e 6720 6361 6e20  ype casting can 
+00000ed0: 6c65 6164 2074 6f20 756e 6578 7065 6374  lead to unexpect
+00000ee0: 6564 2062 6568 6176 696f 7221 0a0a 4279  ed behavior!..By
+00000ef0: 2064 6566 6175 6c74 2c20 6061 7374 6172   default, `astar
+00000f00: 7465 7360 2077 696c 6c20 7370 6c69 7420  tes` will split 
+00000f10: 6461 7461 2072 616e 646f 6d6c 792e 2041  data randomly. A
+00000f20: 6464 6974 696f 6e61 6c6c 792c 2061 2076  dditionally, a v
+00000f30: 6172 6965 7479 206f 6620 616c 676f 7269  ariety of algori
+00000f40: 7468 6d69 6320 7361 6d70 6c69 6e67 2061  thmic sampling a
+00000f50: 7070 726f 6163 6865 7320 6361 6e20 6265  pproaches can be
+00000f60: 2075 7365 6420 6279 2073 7065 6369 6679   used by specify
+00000f70: 696e 6720 7468 6520 6073 616d 706c 6572  ing the `sampler
+00000f80: 6020 6172 6775 6d65 6e74 2074 6f20 7468  ` argument to th
+00000f90: 6520 6675 6e63 7469 6f6e 2028 7365 6520  e function (see 
+00000fa0: 7468 6520 5b54 6162 6c65 206f 6620 496d  the [Table of Im
+00000fb0: 706c 656d 656e 7465 6420 5361 6d70 6c65  plemented Sample
+00000fc0: 7273 5d28 2369 6d70 6c65 6d65 6e74 6564  rs](#implemented
+00000fd0: 2d73 616d 706c 696e 672d 616c 676f 7269  -sampling-algori
+00000fe0: 7468 6d73 2920 666f 7220 6120 636f 6d70  thms) for a comp
+00000ff0: 6c65 7420 6c69 7374 206f 6620 6f70 7469  let list of opti
+00001000: 6f6e 7320 616e 6420 7468 6569 7220 636f  ons and their co
+00001010: 7272 6573 706f 6e64 696e 6720 7265 6665  rresponding refe
+00001020: 7265 6e63 6573 293a 0a0a 6060 6070 7974  rences):..```pyt
+00001030: 686f 6e0a 585f 7472 6169 6e2c 2058 5f74  hon.X_train, X_t
+00001040: 6573 742c 2079 5f74 7261 696e 2c20 795f  est, y_train, y_
+00001050: 7465 7374 203d 2074 7261 696e 5f74 6573  test = train_tes
+00001060: 745f 7370 6c69 7428 0a20 2058 2c20 2023  t_split(.  X,  #
+00001070: 2070 7265 6665 7261 626c 7920 6e75 6d70   preferably nump
+00001080: 7920 6172 7261 7973 2c20 6275 7420 6173  y arrays, but as
+00001090: 7461 7274 6573 2077 696c 6c20 6361 7374  tartes will cast
+000010a0: 2069 7420 666f 7220 796f 750a 2020 792c   it for you.  y,
+000010b0: 0a20 2073 616d 706c 6572 203d 2027 6b65  .  sampler = 'ke
+000010c0: 6e6e 6172 645f 7374 6f6e 6527 2c20 2023  nnard_stone',  #
+000010d0: 2061 6e79 206f 6620 7468 6520 7375 7070   any of the supp
+000010e0: 6f72 7465 6420 7361 6d70 6c65 7273 0a29  orted samplers.)
+000010f0: 0a60 6060 0a0a 5468 6174 2773 2061 6c6c  .```..That's all
+00001100: 2079 6f75 206e 6565 6420 746f 2067 6574   you need to get
+00001110: 2073 7461 7274 6564 2077 6974 6820 6061   started with `a
+00001120: 7374 6172 7465 7360 2120 5468 6520 6e65  startes`! The ne
+00001130: 7874 2073 6563 7469 6f6e 7320 696e 636c  xt sections incl
+00001140: 7564 6520 6d6f 7265 2065 7861 6d70 6c65  ude more example
+00001150: 7320 616e 6420 736f 6d65 2064 656d 6f20  s and some demo 
+00001160: 6e6f 7465 626f 6f6b 7320 796f 7520 6361  notebooks you ca
+00001170: 6e20 7472 7920 696e 2079 6f75 7220 6272  n try in your br
+00001180: 6f77 7365 722e 0a0a 2323 2320 4578 616d  owser...### Exam
+00001190: 706c 6520 4e6f 7465 626f 6f6b 730a 0a43  ple Notebooks..C
+000011a0: 6c69 636b 2074 6865 2062 6164 6765 7320  lick the badges 
+000011b0: 696e 2074 6865 2074 6162 6c65 2062 656c  in the table bel
+000011c0: 6f77 2074 6f20 6265 2074 616b 656e 2074  ow to be taken t
+000011d0: 6f20 6120 6c69 7665 2c20 696e 7465 7261  o a live, intera
+000011e0: 6374 6976 6520 6465 6d6f 206f 6620 6061  ctive demo of `a
+000011f0: 7374 6172 7465 7360 3a0a 0a7c 2044 656d  startes`:..| Dem
+00001200: 6f20 7c20 546f 7069 6320 7c20 4c69 6e6b  o | Topic | Link
+00001210: 207c 0a7c 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d   |.|:---:|---|--
+00001220: 2d7c 0a7c 2043 6f6d 7061 7269 6e67 2053  -|.| Comparing S
+00001230: 616d 706c 696e 6720 416c 676f 7269 7468  ampling Algorith
+00001240: 6d73 2077 6974 6820 4661 7374 2046 6f6f  ms with Fast Foo
+00001250: 6420 7c20 5669 7375 616c 2072 6570 7265  d | Visual repre
+00001260: 7365 6e74 6174 696f 6e73 206f 6620 686f  sentations of ho
+00001270: 7720 6469 6666 6572 656e 7420 7361 6d70  w different samp
+00001280: 6c65 7273 2061 6666 6563 7420 6461 7461  lers affect data
+00001290: 2070 6172 7469 7469 6f6e 696e 6720 7c20   partitioning | 
+000012a0: 5b21 5b43 6f6c 6162 5d28 6874 7470 733a  [![Colab](https:
+000012b0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+000012c0: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
+000012d0: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
+000012e0: 7667 295d 2868 7474 7073 3a2f 2f63 6f6c  vg)](https://col
+000012f0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00001300: 6c65 2e63 6f6d 2f67 6974 6875 622f 4a61  le.com/github/Ja
+00001310: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
+00001320: 7465 732f 626c 6f62 2f6d 6169 6e2f 6578  tes/blob/main/ex
+00001330: 616d 706c 6573 2f73 706c 6974 5f63 6f6d  amples/split_com
+00001340: 7061 7269 736f 6e73 2f73 706c 6974 5f63  parisons/split_c
+00001350: 6f6d 7061 7269 736f 6e73 2e69 7079 6e62  omparisons.ipynb
+00001360: 2920 7c0a 7c20 5573 696e 6720 6074 7261  ) |.| Using `tra
+00001370: 696e 5f76 616c 5f74 6573 745f 7370 6c69  in_val_test_spli
+00001380: 7460 2077 6974 6820 7468 6520 6073 6b6c  t` with the `skl
+00001390: 6561 726e 6020 6578 616d 706c 6520 6461  earn` example da
+000013a0: 7461 7365 7473 207c 2044 656d 6f6e 7374  tasets | Demonst
+000013b0: 7261 7469 6e67 2068 6f77 2077 6974 686f  rating how witho
+000013c0: 6c64 696e 6720 6120 7465 7374 2073 6574  lding a test set
+000013d0: 2077 6974 6820 6074 7261 696e 5f76 616c   with `train_val
+000013e0: 5f74 6573 745f 7370 6c69 7460 2063 616e  _test_split` can
+000013f0: 2069 6d70 6163 7420 7065 7266 6f72 6d61   impact performa
+00001400: 6e63 6520 7c20 5b21 5b43 6f6c 6162 5d28  nce | [![Colab](
+00001410: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00001420: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00001430: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
+00001440: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00001450: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+00001460: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
+00001470: 6875 622f 4a61 636b 736f 6e42 7572 6e73  hub/JacksonBurns
+00001480: 2f61 7374 6172 7465 732f 626c 6f62 2f6d  /astartes/blob/m
+00001490: 6169 6e2f 6578 616d 706c 6573 2f74 7261  ain/examples/tra
+000014a0: 696e 5f76 616c 5f74 6573 745f 7370 6c69  in_val_test_spli
+000014b0: 745f 736b 6c65 6172 6e5f 6578 616d 706c  t_sklearn_exampl
+000014c0: 652f 7472 6169 6e5f 7661 6c5f 7465 7374  e/train_val_test
+000014d0: 5f73 706c 6974 5f65 7861 6d70 6c65 2e69  _split_example.i
+000014e0: 7079 6e62 2920 7c0a 7c20 4368 656d 696e  pynb) |.| Chemin
+000014f0: 666f 726d 6174 6963 7320 7361 6d70 6c65  formatics sample
+00001500: 2073 6574 2070 6172 7469 7469 6f6e 696e   set partitionin
+00001510: 6720 7769 7468 2060 6173 7461 7274 6573  g with `astartes
+00001520: 6020 7c20 4578 7472 6170 6f6c 6174 696f  ` | Extrapolatio
+00001530: 6e20 7673 2e20 496e 7465 7270 6f6c 6174  n vs. Interpolat
+00001540: 696f 6e20 696d 7061 6374 206f 6e20 6368  ion impact on ch
+00001550: 656d 696e 666f 726d 6174 6963 7320 6d6f  eminformatics mo
+00001560: 6465 6c20 6163 6375 7261 6379 207c 205b  del accuracy | [
+00001570: 215b 436f 6c61 625d 2868 7474 7073 3a2f  ![Colab](https:/
+00001580: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00001590: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
+000015a0: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
+000015b0: 6729 5d28 6874 7470 733a 2f2f 636f 6c61  g)](https://cola
+000015c0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+000015d0: 652e 636f 6d2f 6769 7468 7562 2f4a 6163  e.com/github/Jac
+000015e0: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
+000015f0: 6573 2f62 6c6f 622f 6d61 696e 2f65 7861  es/blob/main/exa
+00001600: 6d70 6c65 732f 6261 7272 6965 725f 7072  mples/barrier_pr
+00001610: 6564 6963 7469 6f6e 5f77 6974 685f 5244  ediction_with_RD
+00001620: 4237 2f52 4442 375f 6261 7272 6965 725f  B7/RDB7_barrier_
+00001630: 7072 6564 6963 7469 6f6e 5f65 7861 6d70  prediction_examp
+00001640: 6c65 2e69 7079 6e62 2920 7c0a 7c20 436f  le.ipynb) |.| Co
+00001650: 6d70 6172 696e 6720 7061 7274 6974 696f  mparing partitio
+00001660: 6e69 6e67 2061 7070 726f 6163 6865 7320  ning approaches 
+00001670: 666f 7220 616c 6b61 6e65 7320 7c20 5669  for alkanes | Vi
+00001680: 7375 616c 697a 696e 6720 686f 7720 7361  sualizing how sa
+00001690: 6d70 6c65 7220 696d 7061 6374 206d 6f64  mpler impact mod
+000016a0: 656c 2070 6572 666f 726d 616e 6365 2077  el performance w
+000016b0: 6974 6820 7369 6d70 6c65 2063 6865 6d69  ith simple chemi
+000016c0: 6361 6c73 207c 205b 215b 436f 6c61 625d  cals | [![Colab]
+000016d0: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+000016e0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+000016f0: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
+00001700: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
+00001710: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001720: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00001730: 7468 7562 2f4a 6163 6b73 6f6e 4275 726e  thub/JacksonBurn
+00001740: 732f 6173 7461 7274 6573 2f62 6c6f 622f  s/astartes/blob/
+00001750: 6d61 696e 2f65 7861 6d70 6c65 732f 6d6c  main/examples/ml
+00001760: 7064 735f 3230 3233 5f61 7374 6172 7465  pds_2023_astarte
+00001770: 735f 6465 6d6f 6e73 7472 6174 696f 6e2f  s_demonstration/
+00001780: 6d6c 7064 735f 3230 3233 5f64 656d 6f2e  mlpds_2023_demo.
+00001790: 6970 796e 6229 207c 0a0a 546f 2065 7865  ipynb) |..To exe
+000017a0: 6375 7465 2074 6865 7365 206e 6f74 6562  cute these noteb
+000017b0: 6f6f 6b73 206c 6f63 616c 6c79 2c20 636c  ooks locally, cl
+000017c0: 6f6e 6520 7468 6973 2072 6570 6f73 6974  one this reposit
+000017d0: 6f72 7920 2869 2e65 2e20 6067 6974 2063  ory (i.e. `git c
+000017e0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000017f0: 6875 622e 636f 6d2f 4a61 636b 736f 6e42  hub.com/JacksonB
+00001800: 7572 6e73 2f61 7374 6172 7465 732e 6769  urns/astartes.gi
+00001810: 7460 292c 206e 6176 6967 6174 6520 746f  t`), navigate to
+00001820: 2074 6865 2060 6173 7461 7274 6573 6020   the `astartes` 
+00001830: 6469 7265 6374 6f72 792c 2072 756e 2060  directory, run `
+00001840: 7069 7020 696e 7374 616c 6c20 2e5b 6465  pip install .[de
+00001850: 6d6f 735d 602c 2074 6865 6e20 6f70 656e  mos]`, then open
+00001860: 2061 6e64 2072 756e 2074 6865 206e 6f74   and run the not
+00001870: 6562 6f6f 6b73 2069 6e20 796f 7572 2070  ebooks in your p
+00001880: 7265 6665 7272 6564 2065 6469 746f 722e  referred editor.
+00001890: 0a59 6f75 2064 6f20 5f6e 6f74 5f20 6e65  .You do _not_ ne
+000018a0: 6564 2074 6f20 6578 6563 7574 6520 7468  ed to execute th
+000018b0: 6520 6365 6c6c 7320 7072 6566 6978 6564  e cells prefixed
+000018c0: 2077 6974 6820 6025 2563 6170 7475 7265   with `%%capture
+000018d0: 6020 2d20 7468 6579 2061 7265 206f 6e6c  ` - they are onl
+000018e0: 7920 7072 6573 656e 7420 666f 7220 636f  y present for co
+000018f0: 6d70 6174 6962 696c 6974 7920 7769 7468  mpatibility with
+00001900: 2047 6f6f 676c 6520 436f 6c61 622e 0a0a   Google Colab...
+00001910: 2323 2320 5769 7468 686f 6c64 2054 6573  ### Withhold Tes
+00001920: 7469 6e67 2044 6174 6120 7769 7468 2060  ting Data with `
+00001930: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001940: 706c 6974 600a 466f 7220 7269 676f 726f  plit`.For rigoro
+00001950: 7573 204d 4c20 7265 7365 6172 6368 2c20  us ML research, 
+00001960: 6974 2069 7320 6372 6974 6963 616c 2074  it is critical t
+00001970: 6f20 7769 7468 686f 6c64 2073 6f6d 6520  o withhold some 
+00001980: 6461 7461 2064 7572 696e 6720 7472 6169  data during trai
+00001990: 6e69 6e67 2074 6f20 7573 6520 6120 6074  ning to use a `t
+000019a0: 6573 7460 2073 6574 2e0a 5468 6520 6d6f  est` set..The mo
+000019b0: 6465 6c20 7368 6f75 6c64 205f 6e65 7665  del should _neve
+000019c0: 725f 2073 6565 2074 6869 7320 6461 7461  r_ see this data
+000019d0: 2064 7572 696e 6720 7472 6169 6e69 6e67   during training
+000019e0: 2028 756e 6c69 6b65 2074 6865 2076 616c   (unlike the val
+000019f0: 6964 6174 696f 6e20 7365 7429 2073 6f20  idation set) so 
+00001a00: 7468 6174 2077 6520 6361 6e20 6765 7420  that we can get 
+00001a10: 616e 2061 6363 7572 6174 6520 6d65 6173  an accurate meas
+00001a20: 7572 656d 656e 7420 6f66 2069 7473 2070  urement of its p
+00001a30: 6572 666f 726d 616e 6365 2e0a 0a57 6974  erformance...Wit
+00001a40: 6820 6061 7374 6172 7465 7360 2070 6572  h `astartes` per
+00001a50: 666f 726d 696e 6720 7468 6973 2074 6872  forming this thr
+00001a60: 6565 2d77 6179 2064 6174 6120 7370 6c69  ee-way data spli
+00001a70: 7420 6973 2072 6561 6469 6c79 2061 7661  t is readily ava
+00001a80: 696c 6162 6c65 2077 6974 6820 6074 7261  ilable with `tra
+00001a90: 696e 5f76 616c 5f74 6573 745f 7370 6c69  in_val_test_spli
+00001aa0: 7460 3a0a 6060 6070 7974 686f 6e0a 6672  t`:.```python.fr
+00001ab0: 6f6d 2061 7374 6172 7465 7320 696d 706f  om astartes impo
+00001ac0: 7274 2074 7261 696e 5f76 616c 5f74 6573  rt train_val_tes
+00001ad0: 745f 7370 6c69 740a 0a58 5f74 7261 696e  t_split..X_train
+00001ae0: 2c20 585f 7661 6c2c 2058 5f74 6573 7420  , X_val, X_test 
+00001af0: 3d20 7472 6169 6e5f 7661 6c5f 7465 7374  = train_val_test
+00001b00: 5f73 706c 6974 2858 2c20 7361 6d70 6c65  _split(X, sample
+00001b10: 7220 3d20 2773 7068 6572 655f 6578 636c  r = 'sphere_excl
+00001b20: 7573 696f 6e27 290a 6060 600a 596f 7520  usion').```.You 
+00001b30: 6361 6e20 6e6f 7720 7472 6169 6e20 796f  can now train yo
+00001b40: 7572 206d 6f64 656c 2077 6974 6820 6058  ur model with `X
+00001b50: 5f74 7261 696e 602c 206f 7074 696d 697a  _train`, optimiz
+00001b60: 6520 796f 7572 206d 6f64 656c 2077 6974  e your model wit
+00001b70: 6820 6058 5f76 616c 602c 2061 6e64 206d  h `X_val`, and m
+00001b80: 6561 7375 7265 2069 7473 2070 6572 666f  easure its perfo
+00001b90: 726d 616e 6365 2077 6974 6820 6058 5f74  rmance with `X_t
+00001ba0: 6573 7460 2e0a 0a23 2323 2045 7661 6c75  est`...### Evalu
+00001bb0: 6174 6520 7468 6520 496d 7061 6374 206f  ate the Impact o
+00001bc0: 6620 5370 6c69 7474 696e 6720 416c 676f  f Splitting Algo
+00001bd0: 7269 7468 6d73 0a46 6f72 2064 6174 6120  rithms.For data 
+00001be0: 7769 7468 206d 616e 7920 6665 6174 7572  with many featur
+00001bf0: 6573 2069 7420 6361 6e20 6265 2064 6966  es it can be dif
+00001c00: 6669 6375 6c74 2074 6f20 7669 7375 616c  ficult to visual
+00001c10: 697a 6520 686f 7720 6469 6666 6572 656e  ize how differen
+00001c20: 7420 7361 6d70 6c69 6e67 2061 6c67 6f72  t sampling algor
+00001c30: 6974 686d 7320 6368 616e 6765 2074 6865  ithms change the
+00001c40: 2064 6973 7472 6962 7574 696f 6e20 6f66   distribution of
+00001c50: 2064 6174 6120 696e 746f 2074 7261 696e   data into train
+00001c60: 696e 672c 2076 616c 6964 6174 696f 6e2c  ing, validation,
+00001c70: 2061 6e64 2074 6573 7469 6e67 206c 696b   and testing lik
+00001c80: 6520 7765 2064 6f20 696e 2073 6f6d 6520  e we do in some 
+00001c90: 6f66 2074 6865 2064 656d 6f20 6e6f 7465  of the demo note
+00001ca0: 626f 6f6b 732e 0a54 6f20 6169 6420 696e  books..To aid in
+00001cb0: 2061 6e61 6c79 7a69 6e67 2074 6865 2069   analyzing the i
+00001cc0: 6d70 6163 7420 6f66 2074 6865 2061 6c67  mpact of the alg
+00001cd0: 6f72 6974 686d 732c 2060 6173 7461 7274  orithms, `astart
+00001ce0: 6573 6020 7072 6f76 6964 6573 2060 6765  es` provides `ge
+00001cf0: 6e65 7261 7465 5f72 6567 7265 7373 696f  nerate_regressio
+00001d00: 6e5f 7265 7375 6c74 735f 6469 6374 602e  n_results_dict`.
+00001d10: 0a54 6869 7320 6675 6e63 7469 6f6e 2061  .This function a
+00001d20: 6c6c 6f77 7320 7573 6572 7320 746f 2071  llows users to q
+00001d30: 7569 636b 6c79 2065 7661 6c75 6174 6520  uickly evaluate 
+00001d40: 7468 6520 696d 7061 6374 206f 6620 6469  the impact of di
+00001d50: 6666 6572 656e 7420 7370 6c69 7474 696e  fferent splittin
+00001d60: 6720 7465 6368 6e69 7175 6573 206f 6e20  g techniques on 
+00001d70: 616e 7920 6d6f 6465 6c20 7375 7070 6f72  any model suppor
+00001d80: 7465 6420 6279 2060 736b 6c65 6172 6e60  ted by `sklearn`
+00001d90: 2e20 416c 6c20 7265 7375 6c74 7320 6172  . All results ar
+00001da0: 6520 7374 6f72 6564 2069 6e20 6120 6469  e stored in a di
+00001db0: 6374 696f 6e61 7279 2066 6f72 6d61 7420  ctionary format 
+00001dc0: 616e 6420 6361 6e20 6265 2064 6973 706c  and can be displ
+00001dd0: 6179 6564 2069 6e20 6120 6e65 6174 6c79  ayed in a neatly
+00001de0: 2066 6f72 6d61 7474 6564 2074 6162 6c65   formatted table
+00001df0: 2075 7369 6e67 2074 6865 206f 7074 696f   using the optio
+00001e00: 6e61 6c20 6070 7269 6e74 5f72 6573 756c  nal `print_resul
+00001e10: 7473 6020 6172 6775 6d65 6e74 2e0a 0a60  ts` argument...`
+00001e20: 6060 7079 7468 6f6e 0a66 726f 6d20 736b  ``python.from sk
+00001e30: 6c65 6172 6e2e 7376 6d20 696d 706f 7274  learn.svm import
+00001e40: 204c 696e 6561 7253 5652 0a0a 6672 6f6d   LinearSVR..from
+00001e50: 2061 7374 6172 7465 732e 7574 696c 7320   astartes.utils 
+00001e60: 696d 706f 7274 2067 656e 6572 6174 655f  import generate_
+00001e70: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
+00001e80: 7473 5f64 6963 740a 0a73 6b6c 6561 726e  ts_dict..sklearn
+00001e90: 5f6d 6f64 656c 203d 204c 696e 6561 7253  _model = LinearS
+00001ea0: 5652 2829 0a72 6573 756c 7473 5f64 6963  VR().results_dic
+00001eb0: 7420 3d20 6765 6e65 7261 7465 5f72 6567  t = generate_reg
+00001ec0: 7265 7373 696f 6e5f 7265 7375 6c74 735f  ression_results_
+00001ed0: 6469 6374 280a 2020 2020 736b 6c65 6172  dict(.    sklear
+00001ee0: 6e5f 6d6f 6465 6c2c 0a20 2020 2058 2c0a  n_model,.    X,.
+00001ef0: 2020 2020 792c 0a20 2020 2070 7269 6e74      y,.    print
+00001f00: 5f72 6573 756c 7473 3d54 7275 652c 0a29  _results=True,.)
+00001f10: 0a0a 2020 2020 2020 2020 2054 7261 696e  ..         Train
+00001f20: 2020 2020 2020 2056 616c 2020 2020 2020         Val      
+00001f30: 5465 7374 0a2d 2d2d 2d20 202d 2d2d 2d2d  Test.----  -----
+00001f40: 2d2d 2d20 202d 2d2d 2d2d 2d2d 2d20 202d  ---  --------  -
+00001f50: 2d2d 2d2d 2d2d 2d0a 4d41 4520 2020 312e  -------.MAE   1.
+00001f60: 3431 3532 3220 2020 332e 3133 3433 3520  41522   3.13435 
+00001f70: 2020 322e 3137 3039 310a 524d 5345 2020    2.17091.RMSE  
+00001f80: 322e 3033 3036 3220 2020 332e 3733 3732  2.03062   3.7372
+00001f90: 3120 2020 322e 3430 3034 310a 5232 2020  1   2.40041.R2  
+00001fa0: 2020 302e 3930 3734 3520 2020 302e 3830    0.90745   0.80
+00001fb0: 3738 3720 2020 302e 3738 3431 320a 0a60  787   0.78412..`
+00001fc0: 6060 0a0a 2323 2320 4163 6365 7373 2053  ``..### Access S
+00001fd0: 616d 706c 696e 6720 416c 676f 7269 7468  ampling Algorith
+00001fe0: 6d73 2044 6972 6563 746c 790a 5468 6520  ms Directly.The 
+00001ff0: 7361 6d70 6c69 6e67 2061 6c67 6f72 6974  sampling algorit
+00002000: 686d 7320 696d 706c 656d 656e 7465 6420  hms implemented 
+00002010: 696e 2060 6173 7461 7274 6573 6020 6361  in `astartes` ca
+00002020: 6e20 616c 736f 2062 6520 6469 7265 6374  n also be direct
+00002030: 6c79 2061 6363 6573 7365 6420 616e 6420  ly accessed and 
+00002040: 7275 6e20 6966 2069 7420 6973 206d 6f72  run if it is mor
+00002050: 6520 7573 6566 756c 2066 6f72 2079 6f75  e useful for you
+00002060: 7220 6170 706c 6963 6174 696f 6e73 2e0a  r applications..
+00002070: 496e 2074 6865 2062 656c 6f77 2065 7861  In the below exa
+00002080: 6d70 6c65 2c20 7765 2069 6d70 6f72 7420  mple, we import 
+00002090: 7468 6520 4b65 6e6e 6172 6420 5374 6f6e  the Kennard Ston
+000020a0: 6520 7361 6d70 6c65 722c 2075 7365 2069  e sampler, use i
+000020b0: 7420 746f 2070 6172 7469 7469 6f6e 2061  t to partition a
+000020c0: 2073 696d 706c 6520 6172 7261 792c 2061   simple array, a
+000020d0: 6e64 2074 6865 6e20 7265 7472 6965 7665  nd then retrieve
+000020e0: 2061 2073 616d 706c 652e 0a60 6060 7079   a sample..```py
+000020f0: 7468 6f6e 0a66 726f 6d20 6173 7461 7274  thon.from astart
+00002100: 6573 2e73 616d 706c 6572 732e 696e 7465  es.samplers.inte
+00002110: 7270 6f6c 6174 696f 6e20 696d 706f 7274  rpolation import
+00002120: 204b 656e 6e61 7264 5374 6f6e 650a 0a6b   KennardStone..k
+00002130: 656e 6e61 7264 5f73 746f 6e65 203d 204b  ennard_stone = K
+00002140: 656e 6e61 7264 5374 6f6e 6528 5b5b 312c  ennardStone([[1,
+00002150: 2032 5d2c 205b 332c 2034 5d2c 205b 352c   2], [3, 4], [5,
+00002160: 2036 5d5d 290a 6669 7273 745f 325f 7361   6]]).first_2_sa
+00002170: 6d70 6c65 7320 3d20 6b65 6e6e 6172 645f  mples = kennard_
+00002180: 7374 6f6e 652e 6765 745f 7361 6d70 6c65  stone.get_sample
+00002190: 5f69 6478 7328 3229 0a60 6060 0a41 6c6c  _idxs(2).```.All
+000021a0: 2073 616d 706c 6572 7320 696e 2060 6173   samplers in `as
+000021b0: 7461 7274 6573 6020 696d 706c 656d 656e  tartes` implemen
+000021c0: 7420 6120 605f 7361 6d70 6c65 2829 6020  t a `_sample()` 
+000021d0: 6d65 7468 6f64 2074 6861 7420 6973 2063  method that is c
+000021e0: 616c 6c65 6420 6279 2074 6865 2063 6f6e  alled by the con
+000021f0: 7374 7275 6374 6f72 2028 692e 652e 2067  structor (i.e. g
+00002200: 7265 6564 696c 7929 2061 6e64 2065 6974  reedily) and eit
+00002210: 6865 7220 6120 6067 6574 5f73 616d 706c  her a `get_sampl
+00002220: 6572 5f69 6478 7360 206f 7220 6067 6574  er_idxs` or `get
+00002230: 5f63 6c75 7374 6572 5f69 6478 7360 2066  _cluster_idxs` f
+00002240: 6f72 2069 6e74 6572 706f 6c61 7469 7665  or interpolative
+00002250: 2061 6e64 2065 7874 7261 706f 6c61 7469   and extrapolati
+00002260: 7665 2073 616d 706c 6572 732c 2072 6573  ve samplers, res
+00002270: 7065 6374 6976 656c 792e 0a46 6f72 206d  pectively..For m
+00002280: 6f72 6520 6465 7461 696c 206f 6e20 7468  ore detail on th
+00002290: 6520 696d 706c 656d 656e 7461 6974 6f6e  e implementaiton
+000022a0: 2061 6e64 2064 6573 6967 6e20 6f66 2073   and design of s
+000022b0: 616d 706c 6572 7320 696e 2060 6173 7461  amplers in `asta
+000022c0: 7274 6573 602c 2073 6565 2074 6865 205b  rtes`, see the [
+000022d0: 4465 7665 6c6f 7065 7220 4e6f 7465 735d  Developer Notes]
+000022e0: 2823 636f 6e74 7269 6275 7469 6e67 2d2d  (#contributing--
+000022f0: 6465 7665 6c6f 7065 722d 6e6f 7465 7329  developer-notes)
+00002300: 2073 6563 7469 6f6e 2e0a 0a23 2320 5468   section...## Th
+00002310: 656f 7279 2061 6e64 2041 7070 6c69 6361  eory and Applica
+00002320: 7469 6f6e 206f 6620 6061 7374 6172 7465  tion of `astarte
+00002330: 7360 0a54 6869 7320 7365 6374 696f 6e20  s`.This section 
+00002340: 6f66 2074 6865 2052 4541 444d 4520 6465  of the README de
+00002350: 7461 696c 7320 736f 6d65 206f 6620 7468  tails some of th
+00002360: 6520 7468 656f 7279 2062 6568 696e 6420  e theory behind 
+00002370: 7768 7920 7468 6520 616c 676f 7269 7468  why the algorith
+00002380: 6d73 2069 6d70 6c65 6d65 6e74 6564 2069  ms implemented i
+00002390: 6e20 6061 7374 6172 7465 7360 2061 7265  n `astartes` are
+000023a0: 2069 6d70 6f72 7461 6e74 2061 6e64 2073   important and s
+000023b0: 6f6d 6520 6d6f 7469 7661 7469 6e67 2065  ome motivating e
+000023c0: 7861 6d70 6c65 732e 0a46 6f72 2061 2063  xamples..For a c
+000023d0: 6f6d 7072 6568 656e 7369 7665 2077 616c  omprehensive wal
+000023e0: 6b74 6872 6f75 6768 206f 6620 7468 6520  kthrough of the 
+000023f0: 7468 656f 7279 2061 6e64 2069 6d70 6c65  theory and imple
+00002400: 6d65 6e74 6174 696f 6e20 6f66 2060 6173  mentation of `as
+00002410: 7461 7274 6573 602c 2066 6f6c 6c6f 7720  tartes`, follow 
+00002420: 5b74 6869 7320 6c69 6e6b 5d28 6874 7470  [this link](http
+00002430: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
+00002440: 6163 6b73 6f6e 4275 726e 732f 6173 7461  acksonBurns/asta
+00002450: 7274 6573 2f72 6177 2f6a 6f73 732d 7061  rtes/raw/joss-pa
+00002460: 7065 722f 4275 726e 732d 5370 6965 6b65  per/Burns-Spieke
+00002470: 726d 616e 6e2d 4268 6174 7461 6368 6172  rmann-Bhattachar
+00002480: 6a65 655f 6173 7461 7274 6573 2e70 6466  jee_astartes.pdf
+00002490: 2920 746f 2072 6561 6420 7468 6520 636f  ) to read the co
+000024a0: 6d70 616e 696f 6e20 7061 7065 7220 2866  mpanion paper (f
+000024b0: 7265 656c 7920 6176 6169 6c61 626c 6520  reely available 
+000024c0: 616e 6420 686f 7374 6564 2068 6572 6520  and hosted here 
+000024d0: 6f6e 2047 6974 4875 6229 2e0a 0a3e 202a  on GitHub)...> *
+000024e0: 2a4e 6f74 652a 2a0a 3e20 5765 2072 6566  *Note**.> We ref
+000024f0: 6572 656e 6365 206f 7065 6e2d 6163 6365  erence open-acce
+00002500: 7373 2070 7562 6c69 6361 7469 6f6e 7320  ss publications 
+00002510: 7768 6572 6576 6572 2070 6f73 7369 626c  wherever possibl
+00002520: 652e 2046 6f72 2061 7274 6963 6c65 7320  e. For articles 
+00002530: 6c6f 636b 6564 2062 6568 696e 6420 6120  locked behind a 
+00002540: 7061 7977 616c 6c20 2864 656e 6f74 6564  paywall (denoted
+00002550: 2077 6974 6820 3a73 6d61 6c6c 5f62 6c75   with :small_blu
+00002560: 655f 6469 616d 6f6e 643a 292c 2077 6520  e_diamond:), we 
+00002570: 696e 7374 6561 6420 7375 6767 6573 7420  instead suggest 
+00002580: 7265 6164 696e 6720 5b74 6869 7320 5769  reading [this Wi
+00002590: 6b69 7065 6469 6120 7061 6765 5d28 6874  kipedia page](ht
+000025a0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000025b0: 6961 2e6f 7267 2f77 696b 692f 5363 692d  ia.org/wiki/Sci-
+000025c0: 4875 6229 2061 6e64 2061 6273 6f6c 7574  Hub) and absolut
+000025d0: 656c 7920 5f5f 6e6f 745f 5f20 6174 7465  ely __not__ atte
+000025e0: 6d70 7469 6e67 2074 6f20 6279 7061 7373  mpting to bypass
+000025f0: 2074 6865 2070 6179 7761 6c6c 2e0a 0a23   the paywall...#
+00002600: 2323 2052 6174 696f 6e61 6c20 5370 6c69  ## Rational Spli
+00002610: 7474 696e 6720 416c 676f 7269 7468 6d73  tting Algorithms
+00002620: 0a57 6869 6c65 206d 7563 6820 6d61 6368  .While much mach
+00002630: 696e 6520 6c65 6172 6e69 6e67 2069 7320  ine learning is 
+00002640: 646f 6e65 2077 6974 6820 6120 7261 6e64  done with a rand
+00002650: 6f6d 2063 686f 6963 6520 6265 7477 6565  om choice betwee
+00002660: 6e20 7472 6169 6e69 6e67 2f76 616c 6964  n training/valid
+00002670: 6174 696f 6e2f 7465 7374 2064 6174 612c  ation/test data,
+00002680: 2061 6e20 616c 7465 726e 6174 6976 6520   an alternative 
+00002690: 6973 2074 6865 2075 7365 206f 6620 736f  is the use of so
+000026a0: 2d63 616c 6c65 6420 2272 6174 696f 6e61  -called "rationa
+000026b0: 6c22 2073 706c 6974 7469 6e67 2061 6c67  l" splitting alg
+000026c0: 6f72 6974 686d 732e 0a54 6865 7365 2061  orithms..These a
+000026d0: 7070 726f 6163 6865 7320 7573 6520 736f  pproaches use so
+000026e0: 6d65 2073 696d 696c 6172 6974 792d 6261  me similarity-ba
+000026f0: 7365 6420 616c 676f 7269 7468 6d20 746f  sed algorithm to
+00002700: 2064 6976 6964 6520 6461 7461 2069 6e74   divide data int
+00002710: 6f20 7365 7473 2e0a 536f 6d65 206f 6620  o sets..Some of 
+00002720: 7468 6573 6520 616c 676f 7269 7468 6d73  these algorithms
+00002730: 2069 6e63 6c75 6465 204b 656e 6e61 7264   include Kennard
+00002740: 2d53 746f 6e65 2028 5b4b 656e 6e61 7264  -Stone ([Kennard
+00002750: 2026 2053 746f 6e65 5d28 6874 7470 733a   & Stone](https:
+00002760: 2f2f 7777 772e 7461 6e64 666f 6e6c 696e  //www.tandfonlin
+00002770: 652e 636f 6d2f 646f 692f 6162 732f 3130  e.com/doi/abs/10
+00002780: 2e31 3038 302f 3030 3430 3137 3036 2e31  .1080/00401706.1
+00002790: 3936 392e 3130 3439 3036 3636 2920 3a73  969.10490666) :s
+000027a0: 6d61 6c6c 5f62 6c75 655f 6469 616d 6f6e  mall_blue_diamon
+000027b0: 643a 292c 2053 7068 6572 6520 4578 636c  d:), Sphere Excl
+000027c0: 7573 696f 6e20 285b 5472 6f70 7368 6120  usion ([Tropsha 
+000027d0: 6574 2e20 616c 5d28 6874 7470 733a 2f2f  et. al](https://
+000027e0: 7075 6273 2e61 6373 2e6f 7267 2f64 6f69  pubs.acs.org/doi
+000027f0: 2f70 6466 2f31 302e 3130 3231 2f63 6933  /pdf/10.1021/ci3
+00002800: 3030 3333 3877 2920 3a73 6d61 6c6c 5f62  00338w) :small_b
+00002810: 6c75 655f 6469 616d 6f6e 643a 292c 6173  lue_diamond:),as
+00002820: 2077 656c 6c20 6173 2074 6865 204f 7074   well as the Opt
+00002830: 6953 696d 2061 7320 6469 7363 7573 7365  iSim as discusse
+00002840: 6420 696e 205b 4170 706c 6965 6420 4368  d in [Applied Ch
+00002850: 656d 6f69 6e66 6f72 6d61 7469 6373 3a20  emoinformatics: 
+00002860: 4163 6869 6576 656d 656e 7473 2061 6e64  Achievements and
+00002870: 2046 7574 7572 6520 4f70 706f 7274 756e   Future Opportun
+00002880: 6974 6965 735d 2868 7474 7073 3a2f 2f77  ities](https://w
+00002890: 7777 2e77 696c 6579 2e63 6f6d 2f65 6e2d  ww.wiley.com/en-
+000028a0: 7573 2f41 7070 6c69 6564 2b43 6865 6d6f  us/Applied+Chemo
+000028b0: 696e 666f 726d 6174 6963 7325 3341 2b41  informatics%3A+A
+000028c0: 6368 6965 7665 6d65 6e74 732b 616e 642b  chievements+and+
+000028d0: 4675 7475 7265 2b4f 7070 6f72 7475 6e69  Future+Opportuni
+000028e0: 7469 6573 2d70 2d39 3738 3335 3237 3830  ties-p-978352780
+000028f0: 3635 3436 2920 3a73 6d61 6c6c 5f62 6c75  6546) :small_blu
+00002900: 655f 6469 616d 6f6e 643a 2e0a 536f 6d65  e_diamond:..Some
+00002910: 2063 6c75 7374 6572 696e 672d 6261 7365   clustering-base
+00002920: 6420 7370 6c69 7474 696e 6720 7465 6368  d splitting tech
+00002930: 6e69 7175 6573 2068 6176 6520 616c 736f  niques have also
+00002940: 2062 6565 6e20 696e 636f 7270 6f72 6174   been incorporat
+00002950: 6564 2c20 7375 6368 2061 7320 5b44 4253  ed, such as [DBS
+00002960: 4341 4e5d 2868 7474 703a 2f2f 6369 7465  CAN](http://cite
+00002970: 7365 6572 782e 6973 742e 7073 752e 6564  seerx.ist.psu.ed
+00002980: 752f 7669 6577 646f 632f 646f 776e 6c6f  u/viewdoc/downlo
+00002990: 6164 3f64 6f69 3d31 302e 312e 312e 3130  ad?doi=10.1.1.10
+000029a0: 3136 2e38 3930 2672 6570 3d72 6570 3126  16.890&rep=rep1&
+000029b0: 7479 7065 3d70 6466 292e 0a0a 5468 6572  type=pdf)...Ther
+000029c0: 6520 6172 6520 7477 6f20 6272 6f61 6420  e are two broad 
+000029d0: 6361 7465 676f 7269 6573 206f 6620 7361  categories of sa
+000029e0: 6d70 6c69 6e67 2061 6c67 6f72 6974 686d  mpling algorithm
+000029f0: 7320 696d 706c 656d 656e 7465 6420 696e  s implemented in
+00002a00: 2060 6173 7461 7274 6573 603a 2065 7874   `astartes`: ext
+00002a10: 7261 706f 6c61 7469 7665 2061 6e64 2069  rapolative and i
+00002a20: 6e74 6572 706f 6c61 7469 7665 2e0a 5468  nterpolative..Th
+00002a30: 6520 666f 726d 6572 2077 696c 6c20 666f  e former will fo
+00002a40: 7263 6520 796f 7572 206d 6f64 656c 2074  rce your model t
+00002a50: 6f20 7072 6564 6963 7420 6f6e 206f 7574  o predict on out
+00002a60: 2d6f 662d 7361 6d70 6c65 2064 6174 612c  -of-sample data,
+00002a70: 2077 6869 6368 2063 7265 6174 6573 2061   which creates a
+00002a80: 206d 6f72 6520 6368 616c 6c65 6e67 696e   more challengin
+00002a90: 6720 7461 736b 2074 6861 6e20 696e 7465  g task than inte
+00002aa0: 7270 6f6c 6174 6976 6520 7361 6d70 6c69  rpolative sampli
+00002ab0: 6e67 2e0a 5365 6520 7468 6520 7461 626c  ng..See the tabl
+00002ac0: 6520 6265 6c6f 7720 666f 7220 616c 6c20  e below for all 
+00002ad0: 6f66 2074 6865 2073 616d 706c 696e 6720  of the sampling 
+00002ae0: 6170 7072 6f61 6368 6573 2063 7572 7265  approaches curre
+00002af0: 6e74 6c79 2069 6d70 6c65 6d65 6e74 6564  ntly implemented
+00002b00: 2069 6e20 6061 7374 6172 7465 7360 2c20   in `astartes`, 
+00002b10: 6173 2077 656c 6c20 6173 2074 6865 2068  as well as the h
+00002b20: 7970 6572 7061 7261 6d65 7465 7273 2074  yperparameters t
+00002b30: 6861 7420 6561 6368 2061 6c67 6f72 6974  hat each algorit
+00002b40: 686d 2061 6363 6570 7473 2028 7768 6963  hm accepts (whic
+00002b50: 6820 6172 6520 7061 7373 6564 2069 6e20  h are passed in 
+00002b60: 7769 7468 2060 686f 7074 7360 2920 616e  with `hopts`) an
+00002b70: 6420 6120 6865 6c70 6675 6c20 7265 6665  d a helpful refe
+00002b80: 7265 6e63 6520 666f 7220 756e 6465 7273  rence for unders
+00002b90: 7461 6e64 696e 6720 686f 7720 7468 6520  tanding how the 
+00002ba0: 6879 7065 7270 6172 616d 6574 6572 7320  hyperparameters 
+00002bb0: 776f 726b 2e0a 4e6f 7465 2074 6861 7420  work..Note that 
+00002bc0: 6072 616e 646f 6d5f 7374 6174 6560 2069  `random_state` i
+00002bd0: 7320 6465 6669 6e65 6420 6173 2061 206b  s defined as a k
+00002be0: 6579 776f 7264 2061 7267 756d 656e 7420  eyword argument 
+00002bf0: 696e 2060 7472 6169 6e5f 7465 7374 5f73  in `train_test_s
+00002c00: 706c 6974 6020 6974 7365 6c66 2c20 6576  plit` itself, ev
+00002c10: 656e 2074 686f 7567 6820 7468 6573 6520  en though these 
+00002c20: 616c 676f 7269 7468 6d73 2077 696c 6c20  algorithms will 
+00002c30: 7573 6520 7468 6520 6072 616e 646f 6d5f  use the `random_
+00002c40: 7374 6174 6560 2069 6e20 7468 6569 7220  state` in their 
+00002c50: 6f77 6e20 776f 726b 2e0a 446f 206e 6f74  own work..Do not
+00002c60: 2070 726f 7669 6465 2061 2060 7261 6e64   provide a `rand
+00002c70: 6f6d 5f73 7461 7465 6020 696e 2074 6865  om_state` in the
+00002c80: 2060 686f 7074 7360 2064 6963 7469 6f6e   `hopts` diction
+00002c90: 6172 7920 2d20 6974 2077 696c 6c20 6265  ary - it will be
+00002ca0: 206f 7665 7277 7269 7474 656e 2062 7920   overwritten by 
+00002cb0: 7468 6520 6072 616e 646f 6d5f 7374 6174  the `random_stat
+00002cc0: 6560 2079 6f75 2070 726f 7669 6465 2066  e` you provide f
+00002cd0: 6f72 2060 7472 6169 6e5f 7465 7374 5f73  or `train_test_s
+00002ce0: 706c 6974 6020 286f 7220 7468 6520 6465  plit` (or the de
+00002cf0: 6661 756c 7420 6966 206e 6f6e 6520 6973  fault if none is
+00002d00: 2070 726f 7669 6465 6429 2e0a 0a23 2323   provided)...###
+00002d10: 2320 496d 706c 656d 656e 7465 6420 5361  # Implemented Sa
+00002d20: 6d70 6c69 6e67 2041 6c67 6f72 6974 686d  mpling Algorithm
+00002d30: 730a 0a7c 2053 616d 706c 6572 204e 616d  s..| Sampler Nam
+00002d40: 6520 7c20 5573 6167 6520 5374 7269 6e67  e | Usage String
+00002d50: 207c 2054 7970 6520 7c20 4879 7065 7270   | Type | Hyperp
+00002d60: 6172 616d 6574 6572 7320 7c20 5265 6665  arameters | Refe
+00002d70: 7265 6e63 6520 7c20 4e6f 7465 7320 7c0a  rence | Notes |.
+00002d80: 7c3a 2d2d 2d3a 7c2d 2d2d 7c2d 2d2d 7c2d  |:---:|---|---|-
+00002d90: 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a 7c20 5261  --|---|---|.| Ra
+00002da0: 6e64 6f6d 207c 2027 7261 6e64 6f6d 2720  ndom | 'random' 
+00002db0: 7c20 496e 7465 7270 6f6c 6174 6976 6520  | Interpolative 
+00002dc0: 7c20 6073 6875 6666 6c65 6020 7c20 5b73  | `shuffle` | [s
+00002dd0: 6b6c 6561 726e 2074 7261 696e 5f74 6573  klearn train_tes
+00002de0: 745f 7370 6c69 745d 2868 7474 7073 3a2f  t_split](https:/
+00002df0: 2f73 6369 6b69 742d 6c65 6172 6e2e 6f72  /scikit-learn.or
+00002e00: 672f 7374 6162 6c65 2f6d 6f64 756c 6573  g/stable/modules
+00002e10: 2f67 656e 6572 6174 6564 2f73 6b6c 6561  /generated/sklea
+00002e20: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
+00002e30: 6f6e 2e74 7261 696e 5f74 6573 745f 7370  on.train_test_sp
+00002e40: 6c69 742e 6874 6d6c 2920 446f 6375 6d65  lit.html) Docume
+00002e50: 6e74 6174 696f 6e20 7c20 5468 6973 2073  ntation | This s
+00002e60: 616d 706c 6572 2069 7320 6120 6469 7265  ampler is a dire
+00002e70: 6374 2070 6173 7374 6872 6f75 6768 2074  ct passthrough t
+00002e80: 6f20 6073 6b6c 6561 726e 6027 7320 6074  o `sklearn`'s `t
+00002e90: 7261 696e 5f74 6573 745f 7370 6c69 7460  rain_test_split`
+00002ea0: 2e20 7c0a 7c20 4b65 6e6e 6172 642d 5374  . |.| Kennard-St
+00002eb0: 6f6e 6520 7c20 276b 656e 6e61 7264 5f73  one | 'kennard_s
+00002ec0: 746f 6e65 2720 7c20 496e 7465 7270 6f6c  tone' | Interpol
+00002ed0: 6174 6976 6520 7c20 606d 6574 7269 6360  ative | `metric`
+00002ee0: 207c 204f 7269 6769 6e61 6c20 5061 7065   | Original Pape
+00002ef0: 7220 6279 205b 4b65 6e6e 6172 6420 2620  r by [Kennard & 
+00002f00: 5374 6f6e 655d 2868 7474 7073 3a2f 2f77  Stone](https://w
+00002f10: 7777 2e74 616e 6466 6f6e 6c69 6e65 2e63  ww.tandfonline.c
+00002f20: 6f6d 2f64 6f69 2f61 6273 2f31 302e 3130  om/doi/abs/10.10
+00002f30: 3830 2f30 3034 3031 3730 362e 3139 3639  80/00401706.1969
+00002f40: 2e31 3034 3930 3636 3629 203a 736d 616c  .10490666) :smal
+00002f50: 6c5f 626c 7565 5f64 6961 6d6f 6e64 3a20  l_blue_diamond: 
+00002f60: 7c20 4575 636c 6964 6961 6e20 6469 7374  | Euclidian dist
+00002f70: 616e 6365 2069 7320 7573 6564 2062 7920  ance is used by 
+00002f80: 6465 6661 756c 742c 2061 7320 6465 7363  default, as desc
+00002f90: 7269 6265 6420 696e 2074 6865 206f 7269  ribed in the ori
+00002fa0: 6769 6e61 6c20 7061 7065 722e 207c 0a7c  ginal paper. |.|
+00002fb0: 2053 616d 706c 6520 7365 7420 5061 7274   Sample set Part
+00002fc0: 6974 696f 6e69 6e67 2062 6173 6564 206f  itioning based o
+00002fd0: 6e20 6a6f 696e 7420 582d 5920 6469 7374  n joint X-Y dist
+00002fe0: 616e 6365 7320 2853 5058 5929 207c 2027  ances (SPXY) | '
+00002ff0: 7370 7879 2720 7c20 496e 7465 7270 6f6c  spxy' | Interpol
+00003000: 6174 6976 6520 7c20 6064 6973 7461 6e63  ative | `distanc
+00003010: 655f 6d65 7472 6963 6020 7c20 5361 6c64  e_metric` | Sald
+00003020: 6861 6e61 2065 742e 2061 6c20 5b6f 7269  hana et. al [ori
+00003030: 6769 6e61 6c20 7061 7065 725d 2868 7474  ginal paper](htt
+00003040: 7073 3a2f 2f77 7777 2e73 6369 656e 6365  ps://www.science
+00003050: 6469 7265 6374 2e63 6f6d 2f73 6369 656e  direct.com/scien
+00003060: 6365 2f61 7274 6963 6c65 2f61 6273 2f70  ce/article/abs/p
+00003070: 6969 2f53 3030 3339 3931 3430 3035 3030  ii/S003991400500
+00003080: 3139 3258 2920 3a73 6d61 6c6c 5f62 6c75  192X) :small_blu
+00003090: 655f 6469 616d 6f6e 643a 207c 2045 7874  e_diamond: | Ext
+000030a0: 656e 7369 6f6e 206f 6620 4b65 6e6e 6172  ension of Kennar
+000030b0: 6420 5374 6f6e 6520 7468 6174 2061 6c73  d Stone that als
+000030c0: 6f20 696e 636c 7564 6573 2074 6865 2072  o includes the r
+000030d0: 6573 706f 6e73 6520 7768 656e 2073 616d  esponse when sam
+000030e0: 706c 696e 6720 6469 7374 616e 6365 732e  pling distances.
+000030f0: 207c 0a7c 2053 6361 6666 6f6c 6420 7c20   |.| Scaffold | 
+00003100: 2773 6361 6666 6f6c 6427 207c 2045 7874  'scaffold' | Ext
+00003110: 7261 706f 6c61 7469 7665 207c 2060 696e  rapolative | `in
+00003120: 636c 7564 655f 6368 6972 616c 6974 7960  clude_chirality`
+00003130: 207c 205b 4265 6d69 732d 4d75 7263 6b6f   | [Bemis-Murcko
+00003140: 2053 6361 6666 6f6c 645d 2868 7474 7073   Scaffold](https
+00003150: 3a2f 2f70 7562 732e 6163 732e 6f72 672f  ://pubs.acs.org/
+00003160: 646f 692f 6675 6c6c 2f31 302e 3130 3231  doi/full/10.1021
+00003170: 2f6a 6d39 3630 3239 3238 2920 3a73 6d61  /jm9602928) :sma
+00003180: 6c6c 5f62 6c75 655f 6469 616d 6f6e 643a  ll_blue_diamond:
+00003190: 2061 7320 696d 706c 656d 656e 7465 6420   as implemented 
+000031a0: 696e 2052 444b 6974 207c 2054 6869 7320  in RDKit | This 
+000031b0: 7361 6d70 6c65 7220 7265 7175 6972 6573  sampler requires
+000031c0: 2053 4d49 4c45 5320 7374 7269 6e67 7320   SMILES strings 
+000031d0: 6173 2069 6e70 7574 2028 7573 6520 7468  as input (use th
+000031e0: 6520 606d 6f6c 6563 756c 6573 6020 7375  e `molecules` su
+000031f0: 6270 6163 6b61 6765 2920 7c0a 7c20 5370  bpackage) |.| Sp
+00003200: 6865 7265 2045 7863 6c75 7369 6f6e 207c  here Exclusion |
+00003210: 2027 7370 6865 7265 5f65 7863 6c75 7369   'sphere_exclusi
+00003220: 6f6e 2720 7c20 4578 7472 6170 6f6c 6174  on' | Extrapolat
+00003230: 6976 6520 7c20 606d 6574 7269 6360 2c20  ive | `metric`, 
+00003240: 6064 6973 7461 6e63 655f 6375 746f 6666  `distance_cutoff
+00003250: 6020 7c20 5f63 7573 746f 6d20 696d 706c  ` | _custom impl
+00003260: 656d 656e 7461 7469 6f6e 5f20 7c20 5661  ementation_ | Va
+00003270: 7269 6174 696f 6e20 6f6e 2053 7068 6572  riation on Spher
+00003280: 6520 4578 636c 7573 696f 6e20 666f 7220  e Exclusion for 
+00003290: 6172 6269 7472 6172 792d 7661 6c75 6564  arbitrary-valued
+000032a0: 2076 6563 746f 7273 2e20 7c0a 7c20 5469   vectors. |.| Ti
+000032b0: 6d65 2042 6173 6564 207c 2027 7469 6d65  me Based | 'time
+000032c0: 5f62 6173 6564 2720 7c20 4578 7472 6170  _based' | Extrap
+000032d0: 6f6c 6174 6976 6520 7c20 5f6e 6f6e 655f  olative | _none_
+000032e0: 207c 2050 6170 6572 7320 7573 696e 6720   | Papers using 
+000032f0: 5469 6d65 2062 6173 6564 2073 706c 6974  Time based split
+00003300: 7469 6e67 3a20 5b43 6865 6e20 6574 2061  ting: [Chen et a
+00003310: 6c2e 5d28 6874 7470 733a 2f2f 7075 6273  l.](https://pubs
+00003320: 2e61 6373 2e6f 7267 2f64 6f69 2f66 756c  .acs.org/doi/ful
+00003330: 6c2f 3130 2e31 3032 312f 6369 3230 3036  l/10.1021/ci2006
+00003340: 3135 6829 203a 736d 616c 6c5f 626c 7565  15h) :small_blue
+00003350: 5f64 6961 6d6f 6e64 3a2c 205b 5368 6572  _diamond:, [Sher
+00003360: 6964 616e 2c20 522e 2050 5d28 6874 7470  idan, R. P](http
+00003370: 733a 2f2f 7075 6273 2e61 6373 2e6f 7267  s://pubs.acs.org
+00003380: 2f64 6f69 2f66 756c 6c2f 3130 2e31 3032  /doi/full/10.102
+00003390: 312f 6369 3430 3030 3834 6b29 203a 736d  1/ci400084k) :sm
+000033a0: 616c 6c5f 626c 7565 5f64 6961 6d6f 6e64  all_blue_diamond
+000033b0: 3a2c 205b 4665 696e 6265 7267 2065 7420  :, [Feinberg et 
+000033c0: 616c 2e5d 2868 7474 7073 3a2f 2f70 7562  al.](https://pub
+000033d0: 732e 6163 732e 6f72 672f 646f 692f 6675  s.acs.org/doi/fu
+000033e0: 6c6c 2f31 302e 3130 3231 2f61 6373 2e6a  ll/10.1021/acs.j
+000033f0: 6d65 6463 6865 6d2e 3962 3032 3138 3729  medchem.9b02187)
+00003400: 203a 736d 616c 6c5f 626c 7565 5f64 6961   :small_blue_dia
+00003410: 6d6f 6e64 3a2c 205b 5374 7275 626c 6520  mond:, [Struble 
+00003420: 6574 2061 6c2e 5d28 6874 7470 733a 2f2f  et al.](https://
+00003430: 7075 6273 2e72 7363 2e6f 7267 2f65 6e2f  pubs.rsc.org/en/
+00003440: 636f 6e74 656e 742f 6172 7469 636c 6568  content/articleh
+00003450: 746d 6c2f 3230 3230 2f72 652f 6430 7265  tml/2020/re/d0re
+00003460: 3030 3037 316a 2920 7c20 5468 6973 2073  00071j) | This s
+00003470: 616d 706c 6572 2072 6571 7569 7265 7320  ampler requires 
+00003480: 606c 6162 656c 7360 2074 6f20 6265 2061  `labels` to be a
+00003490: 6e20 6974 6572 6162 6c65 206f 6620 6569  n iterable of ei
+000034a0: 7468 6572 2064 6174 6520 6f72 2064 6174  ther date or dat
+000034b0: 6574 696d 6520 6f62 6a65 6374 732e 207c  etime objects. |
+000034c0: 0a7c 204f 7074 696d 697a 6162 6c65 204b  .| Optimizable K
+000034d0: 2d44 6973 7369 6d69 6c61 7269 7479 2053  -Dissimilarity S
+000034e0: 656c 6563 7469 6f6e 2028 4f70 7469 5369  election (OptiSi
+000034f0: 6d29 207c 2027 6f70 7469 7369 6d27 207c  m) | 'optisim' |
+00003500: 2045 7874 7261 706f 6c61 7469 7665 207c   Extrapolative |
+00003510: 2060 6e5f 636c 7573 7465 7273 602c 2060   `n_clusters`, `
+00003520: 6d61 785f 7375 6273 616d 706c 655f 7369  max_subsample_si
+00003530: 7a65 602c 2060 6469 7374 616e 6365 5f63  ze`, `distance_c
+00003540: 7574 6f66 6660 207c 205f 6375 7374 6f6d  utoff` | _custom
+00003550: 2069 6d70 6c65 6d65 6e74 6174 696f 6e5f   implementation_
+00003560: 207c 2056 6172 6961 7469 6f6e 206f 6e20   | Variation on 
+00003570: 5b4f 7074 6953 696d 5d28 6874 7470 733a  [OptiSim](https:
+00003580: 2f2f 7075 6273 2e61 6373 2e6f 7267 2f64  //pubs.acs.org/d
+00003590: 6f69 2f31 302e 3130 3231 2f63 6930 3235  oi/10.1021/ci025
+000035a0: 3636 3268 2920 666f 7220 6172 6269 7472  662h) for arbitr
+000035b0: 6172 792d 7661 6c75 6564 2076 6563 746f  ary-valued vecto
+000035c0: 7273 2e20 7c0a 7c20 4b2d 4d65 616e 7320  rs. |.| K-Means 
+000035d0: 7c20 276b 6d65 616e 7327 207c 2045 7874  | 'kmeans' | Ext
+000035e0: 7261 706f 6c61 7469 7665 207c 2060 6e5f  rapolative | `n_
+000035f0: 636c 7573 7465 7273 602c 2060 6e5f 696e  clusters`, `n_in
+00003600: 6974 6020 7c20 5b60 736b 6c65 6172 6e20  it` | [`sklearn 
+00003610: 4b4d 6561 6e73 605d 2868 7474 7073 3a2f  KMeans`](https:/
+00003620: 2f73 6369 6b69 742d 6c65 6172 6e2e 6f72  /scikit-learn.or
+00003630: 672f 7374 6162 6c65 2f6d 6f64 756c 6573  g/stable/modules
+00003640: 2f67 656e 6572 6174 6564 2f73 6b6c 6561  /generated/sklea
+00003650: 726e 2e63 6c75 7374 6572 2e4b 4d65 616e  rn.cluster.KMean
+00003660: 732e 6874 6d6c 2920 7c20 5061 7373 7468  s.html) | Passth
+00003670: 726f 7567 6820 746f 2060 736b 6c65 6172  rough to `sklear
+00003680: 6e60 2773 2060 4b4d 6561 6e73 602e 207c  n`'s `KMeans`. |
+00003690: 0a7c 2044 656e 7369 7479 2d42 6173 6564  .| Density-Based
+000036a0: 2053 7061 7469 616c 2043 6c75 7374 6572   Spatial Cluster
+000036b0: 696e 6720 6f66 2041 7070 6c69 6361 7469  ing of Applicati
+000036c0: 6f6e 7320 7769 7468 204e 6f69 7365 2028  ons with Noise (
+000036d0: 4442 5343 414e 2920 7c20 2764 6273 6361  DBSCAN) | 'dbsca
+000036e0: 6e27 207c 2045 7874 7261 706f 6c61 7469  n' | Extrapolati
+000036f0: 7665 207c 2060 6570 7360 2c20 606d 696e  ve | `eps`, `min
+00003700: 5f73 616d 706c 6573 602c 2060 616c 676f  _samples`, `algo
+00003710: 7269 7468 6d60 2c20 606d 6574 7269 6360  rithm`, `metric`
+00003720: 2c20 606c 6561 665f 7369 7a65 6020 7c20  , `leaf_size` | 
+00003730: 5b60 736b 6c65 6172 6e20 4442 5343 414e  [`sklearn DBSCAN
+00003740: 605d 2868 7474 7073 3a2f 2f73 6369 6b69  `](https://sciki
+00003750: 742d 6c65 6172 6e2e 6f72 672f 7374 6162  t-learn.org/stab
+00003760: 6c65 2f6d 6f64 756c 6573 2f67 656e 6572  le/modules/gener
+00003770: 6174 6564 2f73 6b6c 6561 726e 2e63 6c75  ated/sklearn.clu
+00003780: 7374 6572 2e44 4253 4341 4e2e 6874 6d6c  ster.DBSCAN.html
+00003790: 2920 446f 6375 6d65 6e74 6174 696f 6e7c  ) Documentation|
+000037a0: 2050 6173 7374 6872 6f75 6768 2074 6f20   Passthrough to 
+000037b0: 6073 6b6c 6561 726e 6027 7320 6044 4253  `sklearn`'s `DBS
+000037c0: 4341 4e60 2e20 7c0a 7c20 4d69 6e69 6d75  CAN`. |.| Minimu
+000037d0: 6d20 5465 7374 2053 6574 2044 6973 7369  m Test Set Dissi
+000037e0: 6d69 6c61 7269 7479 2028 4d54 5344 2920  milarity (MTSD) 
+000037f0: 7c20 7e20 7c20 7e20 7c20 5f75 7063 6f6d  | ~ | ~ | _upcom
+00003800: 696e 6720 696e 5f20 6061 7374 6172 7465  ing in_ `astarte
+00003810: 7360 205f 7631 2e78 5f20 7c20 7e20 7c20  s` _v1.x_ | ~ | 
+00003820: 7e20 7c0a 7c20 5265 7374 7269 6374 6564  ~ |.| Restricted
+00003830: 2042 6f6c 747a 6d61 6e6e 204d 6163 6869   Boltzmann Machi
+00003840: 6e65 2028 5242 4d29 207c 207e 207c 207e  ne (RBM) | ~ | ~
+00003850: 207c 205f 7570 636f 6d69 6e67 2069 6e5f   | _upcoming in_
+00003860: 2060 6173 7461 7274 6573 6020 5f76 312e   `astartes` _v1.
+00003870: 785f 207c 207e 207c 207e 207c 0a7c 204b  x_ | ~ | ~ |.| K
+00003880: 6f68 6f6e 656e 2053 656c 662d 4f72 6761  ohonen Self-Orga
+00003890: 6e69 7a69 6e67 204d 6170 2028 534f 4d29  nizing Map (SOM)
+000038a0: 207c 207e 207c 207e 207c 205f 7570 636f   | ~ | ~ | _upco
+000038b0: 6d69 6e67 2069 6e5f 2060 6173 7461 7274  ming in_ `astart
+000038c0: 6573 6020 5f76 312e 785f 207c 207e 207c  es` _v1.x_ | ~ |
+000038d0: 207e 207c 0a7c 2053 506c 6974 204d 6574   ~ |.| SPlit Met
+000038e0: 686f 6420 7c20 7e20 7c20 7e20 7c20 5f75  hod | ~ | ~ | _u
+000038f0: 7063 6f6d 696e 6720 696e 5f20 6061 7374  pcoming in_ `ast
+00003900: 6172 7465 7360 205f 7631 2e78 5f20 7c20  artes` _v1.x_ | 
+00003910: 7e20 7c20 7e20 7c0a 0a23 2323 2044 6f6d  ~ | ~ |..### Dom
+00003920: 6169 6e2d 5370 6563 6966 6963 2041 7070  ain-Specific App
+00003930: 6c69 6361 7469 6f6e 730a 4265 6c6f 7720  lications.Below 
+00003940: 6172 6520 736f 6d65 2066 6965 6c64 2073  are some field s
+00003950: 7065 6369 6669 6320 6170 706c 6963 6174  pecific applicat
+00003960: 696f 6e73 206f 6620 6061 7374 6172 7465  ions of `astarte
+00003970: 7360 2e20 496e 7465 7265 7374 6564 2069  s`. Interested i
+00003980: 6e20 6164 6469 6e67 2061 206e 6577 2073  n adding a new s
+00003990: 616d 706c 696e 6720 616c 676f 7269 7468  ampling algorith
+000039a0: 6d20 6f72 2066 6561 7475 7269 7a61 7469  m or featurizati
+000039b0: 6f6e 2061 7070 726f 6163 683f 2053 6565  on approach? See
+000039c0: 205b 6043 4f4e 5452 4942 5554 494e 472e   [`CONTRIBUTING.
+000039d0: 6d64 605d 282e 2f43 4f4e 5452 4942 5554  md`](./CONTRIBUT
+000039e0: 494e 472e 6d64 292e 0a0a 2323 2323 2043  ING.md)...#### C
+000039f0: 6865 6d69 6361 6c20 4461 7461 2061 6e64  hemical Data and
+00003a00: 2074 6865 2060 6173 7461 7274 6573 2e6d   the `astartes.m
+00003a10: 6f6c 6563 756c 6573 6020 5375 6270 6163  olecules` Subpac
+00003a20: 6b61 6765 0a4d 6163 6869 6e65 204c 6561  kage.Machine Lea
+00003a30: 726e 696e 6720 6973 2065 6e6f 726d 6f75  rning is enormou
+00003a40: 736c 7920 7573 6566 756c 2069 6e20 6368  sly useful in ch
+00003a50: 656d 6973 7472 792d 7265 6c61 7465 6420  emistry-related 
+00003a60: 6669 656c 6473 2064 7565 2074 6f20 7468  fields due to th
+00003a70: 6520 6869 6768 2d64 696d 656e 7369 6f6e  e high-dimension
+00003a80: 616c 2066 6561 7475 7265 2073 7061 6365  al feature space
+00003a90: 206f 6620 6368 656d 6963 616c 2064 6174   of chemical dat
+00003aa0: 612e 0a54 6f20 7072 6f70 6572 6c79 2061  a..To properly a
+00003ab0: 7070 6c79 204d 4c20 746f 2063 6865 6d69  pply ML to chemi
+00003ac0: 6361 6c20 6461 7461 2066 6f72 2069 6e66  cal data for inf
+00003ad0: 6572 656e 6365 205f 6f72 5f20 6469 7363  erence _or_ disc
+00003ae0: 6f76 6572 792c 2069 7420 6973 2069 6d70  overy, it is imp
+00003af0: 6f72 7461 6e74 2074 6f20 6b6e 6f77 2061  ortant to know a
+00003b00: 206d 6f64 656c 2773 2061 6363 7572 6163   model's accurac
+00003b10: 7920 756e 6465 7220 7468 6520 7477 6f20  y under the two 
+00003b20: 646f 6d61 696e 732e 0a54 6f20 7369 6d70  domains..To simp
+00003b30: 6c69 6679 2074 6865 2070 726f 6365 7373  lify the process
+00003b40: 206f 6620 7061 7274 6974 696f 6e69 6e67   of partitioning
+00003b50: 2063 6865 6d69 6361 6c20 6461 7461 2c20   chemical data, 
+00003b60: 6061 7374 6172 7465 7360 2069 6d70 6c65  `astartes` imple
+00003b70: 6d65 6e74 7320 6120 7072 652d 6275 696c  ments a pre-buil
+00003b80: 7420 6665 6174 7572 697a 6572 2066 6f72  t featurizer for
+00003b90: 2063 6f6d 6d6f 6e20 6368 656d 6973 7472   common chemistr
+00003ba0: 7920 6461 7461 2066 6f72 6d61 7473 2e0a  y data formats..
+00003bb0: 4166 7465 7220 696e 7374 616c 6c69 6e67  After installing
+00003bc0: 2077 6974 6820 6070 6970 2069 6e73 7461   with `pip insta
+00003bd0: 6c6c 2061 7374 6172 7465 735b 6d6f 6c65  ll astartes[mole
+00003be0: 6375 6c65 735d 6020 6f6e 6520 6361 6e20  cules]` one can 
+00003bf0: 696d 706f 7274 2074 6865 206e 6577 2074  import the new t
+00003c00: 7261 696e 2f74 6573 7420 7370 6c69 7474  rain/test splitt
+00003c10: 696e 6720 6675 6e63 7469 6f6e 206c 696b  ing function lik
+00003c20: 6520 7468 6973 3a20 6066 726f 6d20 6173  e this: `from as
+00003c30: 7461 7274 6573 2e6d 6f6c 6563 756c 6573  tartes.molecules
+00003c40: 2069 6d70 6f72 7420 7472 6169 6e5f 7465   import train_te
+00003c50: 7374 5f73 706c 6974 5f6d 6f6c 6563 756c  st_split_molecul
+00003c60: 6573 600a 0a54 6865 2075 7361 6765 206f  es`..The usage o
+00003c70: 6620 7468 6973 2066 756e 6374 696f 6e20  f this function 
+00003c80: 6973 2069 6465 6e74 6963 616c 2074 6f20  is identical to 
+00003c90: 6074 7261 696e 5f74 6573 745f 7370 6c69  `train_test_spli
+00003ca0: 7460 2062 7574 2077 6974 6820 7468 6520  t` but with the 
+00003cb0: 6164 6469 7469 6f6e 206f 6620 6e65 7720  addition of new 
+00003cc0: 6172 6775 6d65 6e74 7320 746f 2063 6f6e  arguments to con
+00003cd0: 7472 6f6c 2068 6f77 2074 6865 206d 6f6c  trol how the mol
+00003ce0: 6563 756c 6573 2061 7265 2066 6561 7475  ecules are featu
+00003cf0: 7269 7a65 643a 0a0a 6060 6070 7974 686f  rized:..```pytho
+00003d00: 6e0a 7472 6169 6e5f 7465 7374 5f73 706c  n.train_test_spl
+00003d10: 6974 5f6d 6f6c 6563 756c 6573 280a 2020  it_molecules(.  
+00003d20: 2020 6d6f 6c65 6375 6c65 733d 736d 696c    molecules=smil
+00003d30: 6573 2c0a 2020 2020 793d 792c 0a20 2020  es,.    y=y,.   
+00003d40: 2074 6573 745f 7369 7a65 3d30 2e32 2c0a   test_size=0.2,.
+00003d50: 2020 2020 7472 6169 6e5f 7369 7a65 3d30      train_size=0
+00003d60: 2e38 2c0a 2020 2020 6669 6e67 6572 7072  .8,.    fingerpr
+00003d70: 696e 743d 2264 6179 6c69 6768 745f 6669  int="daylight_fi
+00003d80: 6e67 6572 7072 696e 7422 2c0a 2020 2020  ngerprint",.    
+00003d90: 6670 7269 6e74 735f 686f 7074 733d 7b0a  fprints_hopts={.
+00003da0: 2020 2020 2020 2020 226d 696e 5061 7468          "minPath
+00003db0: 223a 2032 2c0a 2020 2020 2020 2020 226d  ": 2,.        "m
+00003dc0: 6178 5061 7468 223a 2035 2c0a 2020 2020  axPath": 5,.    
+00003dd0: 2020 2020 2266 7053 697a 6522 3a20 3230      "fpSize": 20
+00003de0: 302c 0a20 2020 2020 2020 2022 6269 7473  0,.        "bits
+00003df0: 5065 7248 6173 6822 3a20 342c 0a20 2020  PerHash": 4,.   
+00003e00: 2020 2020 2022 7573 6548 7322 3a20 312c       "useHs": 1,
+00003e10: 0a20 2020 2020 2020 2022 7467 7444 656e  .        "tgtDen
+00003e20: 7369 7479 223a 2030 2e34 2c0a 2020 2020  sity": 0.4,.    
+00003e30: 2020 2020 226d 696e 5369 7a65 223a 2036      "minSize": 6
+00003e40: 342c 0a20 2020 207d 2c0a 2020 2020 7361  4,.    },.    sa
+00003e50: 6d70 6c65 723d 2272 616e 646f 6d22 2c0a  mpler="random",.
+00003e60: 2020 2020 7261 6e64 6f6d 5f73 7461 7465      random_state
+00003e70: 3d34 322c 0a20 2020 2068 6f70 7473 3d7b  =42,.    hopts={
+00003e80: 0a20 2020 2020 2020 2022 7368 7566 666c  .        "shuffl
+00003e90: 6522 3a20 5472 7565 2c0a 2020 2020 7d2c  e": True,.    },
+00003ea0: 0a29 0a60 6060 0a0a 546f 2073 6565 2061  .).```..To see a
+00003eb0: 2063 6f6d 706c 6574 6520 6578 616d 706c   complete exampl
+00003ec0: 6520 6f66 2075 7369 6e67 2060 7472 6169  e of using `trai
+00003ed0: 6e5f 7465 7374 5f73 706c 6974 5f6d 6f6c  n_test_split_mol
+00003ee0: 6563 756c 6573 6020 7769 7468 2061 6374  ecules` with act
+00003ef0: 7561 6c20 6368 656d 6963 616c 2064 6174  ual chemical dat
+00003f00: 612c 2074 616b 6520 6120 6c6f 6f6b 2069  a, take a look i
+00003f10: 6e20 7468 6520 6065 7861 6d70 6c65 7360  n the `examples`
+00003f20: 2064 6972 6563 746f 7279 2061 6e64 2074   directory and t
+00003f30: 6865 2062 7269 6566 205b 636f 6d70 616e  he brief [compan
+00003f40: 696f 6e20 7061 7065 725d 2868 7474 7073  ion paper](https
+00003f50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
+00003f60: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
+00003f70: 7465 732f 7261 772f 6a6f 7373 2d70 6170  tes/raw/joss-pap
+00003f80: 6572 2f42 7572 6e73 2d53 7069 656b 6572  er/Burns-Spieker
+00003f90: 6d61 6e6e 2d42 6861 7474 6163 6861 726a  mann-Bhattacharj
+00003fa0: 6565 5f61 7374 6172 7465 732e 7064 6629  ee_astartes.pdf)
+00003fb0: 2e0a 0a43 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
+00003fc0: 206f 7074 696f 6e73 2066 6f72 2074 6865   options for the
+00003fd0: 2066 6561 7475 7269 7a61 7469 6f6e 2073   featurization s
+00003fe0: 6368 656d 6520 6361 6e20 6265 2066 6f75  cheme can be fou
+00003ff0: 6e64 2069 6e20 7468 6520 646f 6375 6d65  nd in the docume
+00004000: 6e74 6174 696f 6e20 666f 7220 5b41 494d  ntation for [AIM
+00004010: 5369 6d5d 2868 7474 7073 3a2f 2f76 6c61  Sim](https://vla
+00004020: 6368 6f73 6772 6f75 702e 6769 7468 7562  chosgroup.github
+00004030: 2e69 6f2f 4149 4d53 696d 2f52 4541 444d  .io/AIMSim/READM
+00004040: 452e 6874 6d6c 2363 7572 7265 6e74 6c79  E.html#currently
+00004050: 2d69 6d70 6c65 6d65 6e74 6564 2d66 696e  -implemented-fin
+00004060: 6765 7270 7269 6e74 7329 2074 686f 7567  gerprints) thoug
+00004070: 6820 6d6f 7374 206f 6620 7468 6520 6372  h most of the cr
+00004080: 6974 6963 616c 2063 6f6e 6669 6775 7261  itical configura
+00004090: 7469 6f6e 206f 7074 696f 6e73 2061 7265  tion options are
+000040a0: 2073 686f 776e 2061 626f 7665 2e0a 0a23   shown above...#
+000040b0: 2320 5265 7072 6f64 7563 6962 696c 6974  # Reproducibilit
+000040c0: 790a 6061 7374 6172 7465 7360 2061 696d  y.`astartes` aim
+000040d0: 7320 746f 2062 6520 636f 6d70 6c65 7465  s to be complete
+000040e0: 6c79 2072 6570 726f 6475 6369 626c 6520  ly reproducible 
+000040f0: 6163 726f 7373 2064 6966 6665 7265 6e74  across different
+00004100: 2070 6c61 7466 6f72 6d73 2c20 5079 7468   platforms, Pyth
+00004110: 6f6e 2076 6572 7369 6f6e 732c 2061 6e64  on versions, and
+00004120: 2064 6570 656e 6465 6e63 7920 636f 6e66   dependency conf
+00004130: 6967 7572 6174 696f 6e73 202d 2061 6e79  igurations - any
+00004140: 2076 6572 7369 6f6e 206f 6620 6061 7374   version of `ast
+00004150: 6172 7465 7360 2076 312e 7820 7368 6f75  artes` v1.x shou
+00004160: 6c64 2072 6573 756c 7420 696e 2074 6865  ld result in the
+00004170: 205f 6578 6163 745f 2073 616d 6520 7370   _exact_ same sp
+00004180: 6c69 7473 2c20 616c 7761 7973 2e0a 546f  lits, always..To
+00004190: 2074 6861 7420 656e 642c 2074 6865 2064   that end, the d
+000041a0: 6566 6175 6c74 2062 6568 6176 696f 7220  efault behavior 
+000041b0: 6f66 2060 6173 7461 7274 6573 6020 6973  of `astartes` is
+000041c0: 2074 6f20 7573 6520 6034 3260 2061 7320   to use `42` as 
+000041d0: 7468 6520 7261 6e64 6f6d 2073 6565 6420  the random seed 
+000041e0: 616e 6420 5f61 6c77 6179 735f 2073 6574  and _always_ set
+000041f0: 2069 742e 0a52 756e 6e69 6e67 2060 6173   it..Running `as
+00004200: 7461 7274 6573 6020 7769 7468 2074 6865  tartes` with the
+00004210: 2064 6566 6175 6c74 2073 6574 7469 6e67   default setting
+00004220: 7320 7769 6c6c 2061 6c77 6179 7320 7072  s will always pr
+00004230: 6f64 7563 6520 7468 6520 6578 6163 7420  oduce the exact 
+00004240: 7361 6d65 2072 6573 756c 7473 2e0a 5765  same results..We
+00004250: 2068 6176 6520 7665 7269 6669 6564 2074   have verified t
+00004260: 6869 7320 6265 6861 7669 6f72 206f 6e20  his behavior on 
+00004270: 4465 6269 616e 2055 6275 6e74 752c 2057  Debian Ubuntu, W
+00004280: 696e 646f 7773 2c20 616e 6420 496e 7465  indows, and Inte
+00004290: 6c20 4d61 6373 2066 726f 6d20 5079 7468  l Macs from Pyth
+000042a0: 6f6e 2076 6572 7369 6f6e 7320 332e 3720  on versions 3.7 
+000042b0: 7468 726f 7567 6820 332e 3131 2028 7769  through 3.11 (wi
+000042c0: 7468 2061 7070 726f 7072 6961 7465 2064  th appropriate d
+000042d0: 6570 656e 6465 6e63 6965 7320 666f 7220  ependencies for 
+000042e0: 6561 6368 2076 6572 7369 6f6e 292e 0a0a  each version)...
+000042f0: 2323 2320 4b6e 6f77 6e20 5265 7072 6f64  ### Known Reprod
+00004300: 7563 6962 696c 6974 7920 4c69 6d69 7461  ucibility Limita
+00004310: 7469 6f6e 730a 496e 6576 6974 6162 6c79  tions.Inevitably
+00004320: 2065 7874 6572 6e61 6c20 6465 7065 6e64   external depend
+00004330: 656e 6369 6573 206f 6620 6061 7374 6172  encies of `astar
+00004340: 7465 7360 2077 696c 6c20 696e 7472 6f64  tes` will introd
+00004350: 7563 6520 6261 636b 7761 7264 732d 696e  uce backwards-in
+00004360: 636f 6d70 6174 6962 6c65 2063 6861 6e67  compatible chang
+00004370: 6573 2e0a 5765 2063 6f6e 7469 6e75 616c  es..We continual
+00004380: 6c79 2072 756e 2072 6567 7265 7373 696f  ly run regressio
+00004390: 6e20 7465 7374 7320 746f 2063 6174 6368  n tests to catch
+000043a0: 2074 6865 7365 2c20 616e 6420 7769 6c6c   these, and will
+000043b0: 206c 6973 7420 616c 6c20 5f6b 6e6f 776e   list all _known
+000043c0: 5f20 6c69 6d69 7461 7469 6f6e 7320 6865  _ limitations he
+000043d0: 7265 3a0a 202d 2060 736b 6c65 6172 6e60  re:. - `sklearn`
+000043e0: 2076 312e 332e 3020 696e 7472 6f64 7563   v1.3.0 introduc
+000043f0: 6564 2062 6163 6b77 6172 6473 2d69 6e63  ed backwards-inc
+00004400: 6f6d 7061 7469 626c 6520 6368 616e 6765  ompatible change
+00004410: 7320 696e 2074 6865 2060 4b4d 6561 6e73  s in the `KMeans
+00004420: 6020 7361 6d70 6c65 7220 7468 6174 2063  ` sampler that c
+00004430: 6861 6e67 6564 2068 6f77 2074 6865 2072  hanged how the r
+00004440: 616e 646f 6d20 696e 6974 6961 6c69 7a61  andom initializa
+00004450: 7469 6f6e 2061 6666 6563 7473 2074 6865  tion affects the
+00004460: 2072 6573 756c 7473 2c20 6576 656e 2067   results, even g
+00004470: 6976 656e 2074 6865 2073 616d 6520 7261  iven the same ra
+00004480: 6e64 6f6d 2073 6565 642e 2044 6966 6665  ndom seed. Diffe
+00004490: 7265 6e74 2076 6572 7369 6f6e 206f 6620  rent version of 
+000044a0: 6073 6b6c 6561 726e 6020 7769 6c6c 2061  `sklearn` will a
+000044b0: 6666 6563 7420 7468 6520 7065 7266 6f72  ffect the perfor
+000044c0: 6d61 6e63 6520 6f66 2060 6173 7461 7274  mance of `astart
+000044d0: 6573 6020 616e 6420 7765 2072 6563 6f6d  es` and we recom
+000044e0: 6d65 6e64 2069 6e63 6c75 6469 6e67 2074  mend including t
+000044f0: 6865 2065 7861 6374 2076 6572 7369 6f6e  he exact version
+00004500: 206f 6620 6073 6369 6b69 742d 6c65 6172   of `scikit-lear
+00004510: 6e60 2061 6e64 2060 6173 7461 7274 6573  n` and `astartes
+00004520: 6020 7573 6564 2c20 7768 656e 2061 7070  ` used, when app
+00004530: 6c69 6361 626c 652e 0a0a 3e20 2a2a 4e6f  licable...> **No
+00004540: 7465 2a2a 0a3e 2057 6520 6172 6520 6c69  te**.> We are li
+00004550: 6d69 7465 6420 696e 206f 7572 2061 6269  mited in our abi
+00004560: 6c69 7479 2074 6f20 7465 7374 206f 6e20  lity to test on 
+00004570: 4d31 204d 6163 732c 2062 7574 2066 726f  M1 Macs, but fro
+00004580: 6d20 6f75 7220 6c69 6d69 7465 6420 6d61  m our limited ma
+00004590: 6e75 616c 2074 6573 7469 6e67 2077 6520  nual testing we 
+000045a0: 6163 6869 6576 6520 7065 7266 6563 7420  achieve perfect 
+000045b0: 7265 7072 6f64 7563 6269 6c69 7479 2069  reproducbility i
+000045c0: 6e20 616c 6c20 6361 7365 7320 5f65 7863  n all cases _exc
+000045d0: 6570 7420 6f63 6361 7369 6f6e 616c 6c79  ept occasionally
+000045e0: 5f20 7769 7468 2060 4b4d 6561 6e73 6020  _ with `KMeans` 
+000045f0: 6f6e 2041 7070 6c65 2073 696c 6963 6f6e  on Apple silicon
+00004600: 2e0a 6061 7374 6172 7465 7360 2069 7320  ..`astartes` is 
+00004610: 7374 696c 6c20 636f 6e73 6973 7465 6e74  still consistent
+00004620: 2062 6574 7765 656e 2072 756e 7320 6f6e   between runs on
+00004630: 2074 6865 2073 616d 6520 706c 6174 666f   the same platfo
+00004640: 726d 2069 6e20 616c 6c20 6361 7365 732c  rm in all cases,
+00004650: 2061 6e64 206f 7468 6572 2073 616d 706c   and other sampl
+00004660: 6572 7320 6172 6520 6e6f 7420 696d 7061  ers are not impa
+00004670: 6374 6564 2062 7920 7468 6973 2061 7070  cted by this app
+00004680: 6172 656e 7420 6275 672e 0a0a 2323 2048  arent bug...## H
+00004690: 6f77 2074 6f20 4369 7465 0a49 6620 796f  ow to Cite.If yo
+000046a0: 7520 7573 6520 6061 7374 6172 7465 7360  u use `astartes`
+000046b0: 2069 6e20 796f 7572 2077 6f72 6b20 706c   in your work pl
+000046c0: 6561 7365 2075 7365 2074 6865 2062 656c  ease use the bel
+000046d0: 6f77 2063 6974 6174 696f 6e20 6f72 2074  ow citation or t
+000046e0: 6865 2022 4369 7465 2074 6869 7320 7265  he "Cite this re
+000046f0: 706f 7369 746f 7279 2220 6275 7474 6f6e  pository" button
+00004700: 206f 6e20 4769 7448 7562 3a0a 3e20 2a2a   on GitHub:.> **
+00004710: 4269 6254 6558 2a2a 0a3e 2040 736f 6674  BibTeX**.> @soft
+00004720: 7761 7265 7b62 7572 6e73 5f6a 6163 6b73  ware{burns_jacks
+00004730: 6f6e 5f32 3032 335f 3831 3437 3230 352c  on_2023_8147205,
+00004740: 0a3e 2020 2061 7574 686f 7220 2020 2020  .>   author     
+00004750: 2020 3d20 7b42 7572 6e73 2c20 4a61 636b    = {Burns, Jack
+00004760: 736f 6e20 616e 640a 3e20 2020 2020 2020  son and.>       
+00004770: 2020 2020 2020 2020 2020 2020 5370 6965              Spie
+00004780: 6b65 726d 616e 6e2c 204b 6576 696e 2061  kermann, Kevin a
+00004790: 6e64 0a3e 2020 2020 2020 2020 2020 2020  nd.>            
+000047a0: 2020 2020 2020 2042 6861 7474 6163 6861         Bhattacha
+000047b0: 726a 6565 2c20 4869 6d61 6768 6e61 2061  rjee, Himaghna a
+000047c0: 6e64 0a3e 2020 2020 2020 2020 2020 2020  nd.>            
+000047d0: 2020 2020 2020 2056 6c61 6368 6f73 2c20         Vlachos, 
+000047e0: 4469 6f6e 6973 696f 7320 616e 640a 3e20  Dionisios and.> 
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 4772 6565 6e2c 2057 696c 6c69 616d    Green, William
+00004810: 7d2c 0a3e 2020 2074 6974 6c65 2020 2020  },.>   title    
+00004820: 2020 2020 3d20 7b7b 4d61 6368 696e 6520      = {{Machine 
+00004830: 4c65 6172 6e69 6e67 2056 616c 6964 6174  Learning Validat
+00004840: 696f 6e20 7669 6120 5261 7469 6f6e 616c  ion via Rational
+00004850: 2044 6174 6173 6574 200a 3e20 2020 2020   Dataset .>     
+00004860: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00004870: 616d 706c 696e 6720 7769 7468 2061 7374  ampling with ast
+00004880: 6172 7465 737d 7d2c 0a3e 2020 206d 6f6e  artes}},.>   mon
+00004890: 7468 2020 2020 2020 2020 3d20 6d61 792c  th        = may,
+000048a0: 0a3e 2020 2079 6561 7220 2020 2020 2020  .>   year       
+000048b0: 2020 3d20 3230 3233 2c0a 3e20 2020 7075    = 2023,.>   pu
+000048c0: 626c 6973 6865 7220 2020 203d 207b 5a65  blisher    = {Ze
+000048d0: 6e6f 646f 7d2c 0a3e 2020 2076 6572 7369  nodo},.>   versi
+000048e0: 6f6e 2020 2020 2020 3d20 7b31 2e31 2e31  on      = {1.1.1
+000048f0: 7d2c 0a3e 2020 2064 6f69 2020 2020 2020  },.>   doi      
+00004900: 2020 2020 3d20 7b31 302e 3532 3831 2f7a      = {10.5281/z
+00004910: 656e 6f64 6f2e 3831 3437 3230 357d 2c0a  enodo.8147205},.
+00004920: 3e20 2020 7572 6c20 2020 2020 2020 2020  >   url         
+00004930: 203d 207b 6874 7470 733a 2f2f 646f 692e   = {https://doi.
+00004940: 6f72 672f 3130 2e35 3238 312f 7a65 6e6f  org/10.5281/zeno
+00004950: 646f 2e38 3134 3732 3035 7d0a 3e20 7d0a  do.8147205}.> }.
+00004960: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00004970: 2026 2044 6576 656c 6f70 6572 204e 6f74   & Developer Not
+00004980: 6573 0a53 6565 205b 434f 4e54 5249 4255  es.See [CONTRIBU
+00004990: 5449 4e47 2e6d 645d 282e 2f43 4f4e 5452  TING.md](./CONTR
+000049a0: 4942 5554 494e 472e 6d64 2920 666f 7220  IBUTING.md) for 
+000049b0: 696e 7374 7275 6374 696f 6e73 206f 6e20  instructions on 
+000049c0: 696e 7374 616c 6c69 6e67 2060 6173 7461  installing `asta
+000049d0: 7274 6573 6020 666f 7220 6465 7665 6c6f  rtes` for develo
+000049e0: 706d 656e 742c 206d 616b 696e 6720 6120  pment, making a 
+000049f0: 636f 6e74 7269 6275 7469 6f6e 2c20 616e  contribution, an
+00004a00: 6420 6765 6e65 7261 6c20 6775 6964 616e  d general guidan
+00004a10: 6365 206f 6e20 7468 6520 6465 7369 676e  ce on the design
+00004a20: 206f 6620 6061 7374 6172 7465 7360 2e0a   of `astartes`..
+00004a30: 0a                                       .
```

### Comparing `astartes-1.1.1/astartes/main.py` & `astartes-1.1.2/astartes/main.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/molecules.py` & `astartes-1.1.2/astartes/molecules.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/__init__.py` & `astartes-1.1.2/astartes/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/abstract_sampler.py` & `astartes-1.1.2/astartes/samplers/abstract_sampler.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/dbscan.py` & `astartes-1.1.2/astartes/samplers/extrapolation/dbscan.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/kmeans.py` & `astartes-1.1.2/astartes/samplers/extrapolation/kmeans.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/optisim.py` & `astartes-1.1.2/astartes/samplers/extrapolation/optisim.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/scaffold.py` & `astartes-1.1.2/astartes/samplers/extrapolation/scaffold.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/sphere_exclusion.py` & `astartes-1.1.2/astartes/samplers/extrapolation/sphere_exclusion.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/extrapolation/time_based.py` & `astartes-1.1.2/astartes/samplers/extrapolation/time_based.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/interpolation/kennardstone.py` & `astartes-1.1.2/astartes/samplers/interpolation/kennardstone.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/interpolation/random_split.py` & `astartes-1.1.2/astartes/samplers/interpolation/random_split.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/samplers/interpolation/spxy.py` & `astartes-1.1.2/astartes/samplers/interpolation/spxy.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/utils/array_type_helpers.py` & `astartes-1.1.2/astartes/utils/array_type_helpers.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/utils/exceptions.py` & `astartes-1.1.2/astartes/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/utils/sampler_factory.py` & `astartes-1.1.2/astartes/utils/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/utils/user_utils.py` & `astartes-1.1.2/astartes/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes/utils/warnings.py` & `astartes-1.1.2/astartes/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/astartes.egg-info/PKG-INFO` & `astartes-1.1.2/astartes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6173 7461  : 2.1.Name: asta
 00000020: 7274 6573 0a56 6572 7369 6f6e 3a20 312e  rtes.Version: 1.
-00000030: 312e 310a 5375 6d6d 6172 793a 2054 7261  1.1.Summary: Tra
+00000030: 312e 320a 5375 6d6d 6172 793a 2054 7261  1.2.Summary: Tra
 00000040: 696e 3a54 6573 7420 416c 676f 7269 7468  in:Test Algorith
 00000050: 6d69 6320 5361 6d70 6c69 6e67 2066 6f72  mic Sampling for
 00000060: 204d 6f6c 6563 756c 6573 2061 6e64 2041   Molecules and A
 00000070: 7262 6974 7261 7279 2041 7272 6179 730a  rbitrary Arrays.
 00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 4a61  Author-email: Ja
 00000090: 636b 736f 6e20 4275 726e 7320 3c6a 7762  ckson Burns <jwb
 000000a0: 7572 6e73 406d 6974 2e65 6475 3e2c 2048  urns@mit.edu>, H
@@ -112,1179 +112,1123 @@
 000006f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000700: 4a61 636b 736f 6e42 7572 6e73 2f61 7374  JacksonBurns/ast
 00000710: 6172 7465 732f 6163 7469 6f6e 732f 776f  artes/actions/wo
 00000720: 726b 666c 6f77 732f 7265 7072 6f64 7563  rkflows/reproduc
 00000730: 655f 7061 7065 722e 796d 6c2f 6261 6467  e_paper.yml/badg
 00000740: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
 00000750: 6e26 6576 656e 743d 7363 6865 6475 6c65  n&event=schedule
-00000760: 223e 0a3c 2f70 3e0a 0a23 2320 496e 7374  ">.</p>..## Inst
-00000770: 616c 6c69 6e67 2060 6173 7461 7274 6573  alling `astartes
-00000780: 600a 5765 2072 6563 6f6d 6d65 6e64 2069  `.We recommend i
-00000790: 6e73 7461 6c6c 696e 6720 6061 7374 6172  nstalling `astar
-000007a0: 7465 7360 2077 6974 6869 6e20 6120 7669  tes` within a vi
-000007b0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-000007c0: 742c 2075 7369 6e67 2065 6974 6865 7220  t, using either 
-000007d0: 6076 656e 7660 206f 7220 6063 6f6e 6461  `venv` or `conda
-000007e0: 6020 286f 7220 6f74 6865 7220 746f 6f6c  ` (or other tool
-000007f0: 7329 2074 6f20 7369 6d70 6c69 6679 2064  s) to simplify d
-00000800: 6570 656e 6465 6e63 7920 6d61 6e61 6765  ependency manage
-00000810: 6d65 6e74 2e20 5079 7468 6f6e 2076 6572  ment. Python ver
-00000820: 7369 6f6e 7320 332e 372c 2033 2e38 2c20  sions 3.7, 3.8, 
-00000830: 332e 392c 2033 2e31 302c 2061 6e64 2033  3.9, 3.10, and 3
-00000840: 2e31 3120 6172 6520 7375 7070 6f72 7465  .11 are supporte
-00000850: 6420 6f6e 2061 6c6c 2070 6c61 7466 6f72  d on all platfor
-00000860: 6d73 2e0a 0a60 6173 7461 7274 6573 6020  ms...`astartes` 
-00000870: 6973 2061 7661 696c 6162 6c65 206f 6e20  is available on 
-00000880: 6050 7950 4960 2061 6e64 2063 616e 2062  `PyPI` and can b
-00000890: 6520 696e 7374 616c 6c65 6420 7573 696e  e installed usin
-000008a0: 6720 6070 6970 603a 0a0a 202d 2054 6f20  g `pip`:.. - To 
-000008b0: 696e 636c 7564 6520 7468 6520 6665 6174  include the feat
-000008c0: 7572 697a 6174 696f 6e20 6f70 7469 6f6e  urization option
-000008d0: 7320 666f 7220 6368 656d 6963 616c 2064  s for chemical d
-000008e0: 6174 612c 2075 7365 2060 7069 7020 696e  ata, use `pip in
-000008f0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
-00000900: 6f6c 6563 756c 6573 5d60 2e0a 202d 2054  olecules]`.. - T
-00000910: 6f20 696e 7374 616c 6c20 6f6e 6c79 2074  o install only t
-00000920: 6865 2073 616d 706c 696e 6720 616c 676f  he sampling algo
-00000930: 7269 7468 6d73 2c20 7573 6520 6070 6970  rithms, use `pip
-00000940: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
-00000950: 7360 2028 7468 6973 2069 6e73 7461 6c6c  s` (this install
-00000960: 2077 696c 6c20 6861 7665 2066 6577 6572   will have fewer
-00000970: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
-00000980: 6420 6d61 7920 6265 206d 6f72 6520 7265  d may be more re
-00000990: 6164 696c 7920 636f 6d70 6174 6962 6c65  adily compatible
-000009a0: 2069 6e20 656e 7669 726f 6e6d 656e 7473   in environments
-000009b0: 2077 6974 6820 6578 6973 7469 6e67 2077   with existing w
-000009c0: 6f72 6b66 6c6f 7773 292e 0a0a 5468 6520  orkflows)...The 
-000009d0: 6261 7365 2060 6173 7461 7274 6573 6020  base `astartes` 
-000009e0: 7061 636b 6167 6520 6973 2061 6c73 6f20  package is also 
-000009f0: 6176 6169 6c61 626c 6520 6f6e 2060 636f  available on `co
-00000a00: 6e64 6160 2077 6974 6820 7468 6973 2063  nda` with this c
-00000a10: 6f6d 6d61 6e64 3a20 6063 6f6e 6461 2069  ommand: `conda i
-00000a20: 6e73 7461 6c6c 202d 6320 6a61 636b 736f  nstall -c jackso
-00000a30: 6e62 7572 6e73 2061 7374 6172 7465 7360  nburns astartes`
-00000a40: 2e0a 4e6f 7465 2074 6861 7420 7468 6973  ..Note that this
-00000a50: 2070 6163 6b61 6765 205f 646f 6573 206e   package _does n
-00000a60: 6f74 5f20 696e 636c 7564 6520 6275 696c  ot_ include buil
-00000a70: 742d 696e 2073 7570 706f 7274 2066 6f72  t-in support for
-00000a80: 2066 6561 7475 7269 7a69 6e67 206d 6f6c   featurizing mol
-00000a90: 6563 756c 6573 2c20 7768 6963 6820 6973  ecules, which is
-00000aa0: 2063 7572 7265 6e74 6c79 206f 6e6c 7920   currently only 
-00000ab0: 6176 6169 6c61 626c 6520 6672 6f6d 2074  available from t
-00000ac0: 6865 2050 7950 4920 7061 636b 6167 6520  he PyPI package 
-00000ad0: 6f72 2061 2073 6f75 7263 6520 696e 7374  or a source inst
-00000ae0: 616c 6c2e 0a0a 3e20 2a2a 4e6f 7465 2a2a  all...> **Note**
-00000af0: 0a3e 2057 696e 646f 7773 2050 6f77 6572  .> Windows Power
-00000b00: 7368 656c 6c20 616e 6420 4d61 634f 5320  shell and MacOS 
-00000b10: 4361 7461 6c69 6e61 206f 7220 6e65 7765  Catalina or newe
-00000b20: 7220 6d61 7920 636f 6d70 6c61 696e 2061  r may complain a
-00000b30: 626f 7574 2073 7175 6172 6520 6272 6163  bout square brac
-00000b40: 6b65 7473 2c20 736f 2079 6f75 2077 696c  kets, so you wil
-00000b50: 6c20 6e65 6564 2074 6f20 646f 7562 6c65  l need to double
-00000b60: 2071 756f 7465 2074 6865 2060 6d6f 6c65   quote the `mole
-00000b70: 6375 6c65 7360 2063 6f6d 6d61 6e64 2028  cules` command (
-00000b80: 692e 652e 2060 7069 7020 696e 7374 616c  i.e. `pip instal
-00000b90: 6c20 2261 7374 6172 7465 735b 6d6f 6c65  l "astartes[mole
-00000ba0: 6375 6c65 735d 2260 290a 0a54 6f20 696e  cules]"`)..To in
-00000bb0: 7374 616c 6c20 6061 7374 6172 7465 7360  stall `astartes`
-00000bc0: 2066 726f 6d20 736f 7572 6365 2c20 7365   from source, se
-00000bd0: 6520 7468 6520 5b43 6f6e 7472 6962 7574  e the [Contribut
-00000be0: 696e 6720 2620 4465 7665 6c6f 7065 7220  ing & Developer 
-00000bf0: 4e6f 7465 735d 2823 636f 6e74 7269 6275  Notes](#contribu
-00000c00: 7469 6e67 2d2d 6465 7665 6c6f 7065 722d  ting--developer-
-00000c10: 6e6f 7465 7329 2073 6563 7469 6f6e 2e0a  notes) section..
-00000c20: 0a23 2320 5573 696e 6720 6061 7374 6172  .## Using `astar
-00000c30: 7465 7360 0a60 6173 7461 7274 6573 6020  tes`.`astartes` 
-00000c40: 6973 2064 6573 6967 6e65 6420 6173 2061  is designed as a
-00000c50: 2064 726f 702d 696e 2072 6570 6c61 6365   drop-in replace
-00000c60: 6d65 6e74 2066 6f72 2060 736b 6c65 6172  ment for `sklear
-00000c70: 6e60 2773 2060 7472 6169 6e5f 7465 7374  n`'s `train_test
-00000c80: 5f73 706c 6974 6020 6675 6e63 7469 6f6e  _split` function
-00000c90: 2e20 546f 2073 7769 7463 6820 746f 2060  . To switch to `
-00000ca0: 6173 7461 7274 6573 602c 2063 6861 6e67  astartes`, chang
-00000cb0: 6520 6066 726f 6d20 736b 6c65 6172 6e2e  e `from sklearn.
-00000cc0: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
-00000cd0: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
-00000ce0: 745f 7370 6c69 7460 2074 6f20 6066 726f  t_split` to `fro
-00000cf0: 6d20 6173 7461 7274 6573 2069 6d70 6f72  m astartes impor
-00000d00: 7420 7472 6169 6e5f 7465 7374 5f73 706c  t train_test_spl
-00000d10: 6974 602e 0a0a 4c69 6b65 2060 736b 6c65  it`...Like `skle
-00000d20: 6172 6e60 2c20 6061 7374 6172 7465 7360  arn`, `astartes`
-00000d30: 2061 6363 6570 7473 2061 6e79 2069 7465   accepts any ite
-00000d40: 7261 626c 6520 6f62 6a65 6374 2061 7320  rable object as 
-00000d50: 6058 602c 2060 7960 2c20 616e 6420 606c  `X`, `y`, and `l
-00000d60: 6162 656c 7360 2e0a 4561 6368 2077 696c  abels`..Each wil
-00000d70: 6c20 6265 2063 6f6e 7665 7274 6564 2074  l be converted t
-00000d80: 6f20 6120 606e 756d 7079 6020 6172 7261  o a `numpy` arra
-00000d90: 7920 666f 7220 696e 7465 726e 616c 206f  y for internal o
-00000da0: 7065 7261 7469 6f6e 732c 2061 6e64 2072  perations, and r
-00000db0: 6574 7572 6e65 6420 6173 2061 2060 6e75  eturned as a `nu
-00000dc0: 6d70 7960 2061 7272 6179 2077 6974 6820  mpy` array with 
-00000dd0: 6c69 6d69 7465 6420 6578 6365 7074 696f  limited exceptio
-00000de0: 6e73 3a20 6966 2060 5860 2069 7320 6120  ns: if `X` is a 
-00000df0: 6070 616e 6461 7360 2060 4461 7461 4672  `pandas` `DataFr
-00000e00: 616d 6560 2c20 6079 6020 6973 2061 2060  ame`, `y` is a `
-00000e10: 5365 7269 6573 602c 206f 7220 606c 6162  Series`, or `lab
-00000e20: 656c 7360 2069 7320 6120 6053 6572 6965  els` is a `Serie
-00000e30: 7360 2c20 6061 7374 6172 7465 7360 2077  s`, `astartes` w
-00000e40: 696c 6c20 6361 7374 2069 7420 6261 636b  ill cast it back
-00000e50: 2074 6f20 6974 7320 6f72 6967 696e 616c   to its original
-00000e60: 2074 7970 6520 696e 636c 7564 696e 6720   type including 
-00000e70: 6974 7320 696e 6465 7820 616e 6420 636f  its index and co
-00000e80: 6c75 6d6e 206e 616d 6573 2e0a 0a3e 202a  lumn names...> *
-00000e90: 2a4e 6f74 652a 2a0a 3e20 5468 6520 6465  *Note**.> The de
-00000ea0: 7665 6c6f 7065 7273 2072 6563 6f6d 6d65  velopers recomme
-00000eb0: 6e64 2070 6173 7369 6e67 2060 5860 2c20  nd passing `X`, 
-00000ec0: 6079 602c 2061 6e64 2060 6c61 6265 6c73  `y`, and `labels
-00000ed0: 6020 6173 2060 6e75 6d70 7960 2061 7272  ` as `numpy` arr
-00000ee0: 6179 7320 616e 6420 6861 6e64 6c69 6e67  ays and handling
-00000ef0: 2074 6865 2063 6f6e 7665 7273 696f 6e20   the conversion 
-00000f00: 746f 2061 6e64 2066 726f 6d20 6f74 6865  to and from othe
-00000f10: 7220 7479 7065 7320 6578 706c 6963 6974  r types explicit
-00000f20: 7920 6f6e 2079 6f75 7220 6f77 6e2e 2042  y on your own. B
-00000f30: 6568 696e 642d 7468 652d 7363 656e 6573  ehind-the-scenes
-00000f40: 2074 7970 6520 6361 7374 696e 6720 6361   type casting ca
-00000f50: 6e20 6c65 6164 2074 6f20 756e 6578 7065  n lead to unexpe
-00000f60: 6374 6564 2062 6568 6176 696f 7221 0a0a  cted behavior!..
-00000f70: 4279 2064 6566 6175 6c74 2c20 6061 7374  By default, `ast
-00000f80: 6172 7465 7360 2077 696c 6c20 7370 6c69  artes` will spli
-00000f90: 7420 6461 7461 2072 616e 646f 6d6c 792e  t data randomly.
-00000fa0: 2041 6464 6974 696f 6e61 6c6c 792c 2061   Additionally, a
-00000fb0: 2076 6172 6965 7479 206f 6620 616c 676f   variety of algo
-00000fc0: 7269 7468 6d69 6320 7361 6d70 6c69 6e67  rithmic sampling
-00000fd0: 2061 7070 726f 6163 6865 7320 6361 6e20   approaches can 
-00000fe0: 6265 2075 7365 6420 6279 2073 7065 6369  be used by speci
-00000ff0: 6679 696e 6720 7468 6520 6073 616d 706c  fying the `sampl
-00001000: 6572 6020 6172 6775 6d65 6e74 2074 6f20  er` argument to 
-00001010: 7468 6520 6675 6e63 7469 6f6e 3a0a 0a60  the function:..`
-00001020: 6060 7079 7468 6f6e 0a58 5f74 7261 696e  ``python.X_train
-00001030: 2c20 585f 7465 7374 2c20 795f 7472 6169  , X_test, y_trai
-00001040: 6e2c 2079 5f74 6573 7420 3d20 7472 6169  n, y_test = trai
-00001050: 6e5f 7465 7374 5f73 706c 6974 280a 2020  n_test_split(.  
-00001060: 582c 2020 2320 7072 6566 6572 6162 6c79  X,  # preferably
-00001070: 206e 756d 7079 2061 7272 6179 732c 2062   numpy arrays, b
-00001080: 7574 2061 7374 6172 7465 7320 7769 6c6c  ut astartes will
-00001090: 2063 6173 7420 6974 2066 6f72 2079 6f75   cast it for you
-000010a0: 0a20 2079 2c0a 2020 7361 6d70 6c65 7220  .  y,.  sampler 
-000010b0: 3d20 276b 656e 6e61 7264 5f73 746f 6e65  = 'kennard_stone
-000010c0: 272c 2020 2320 616e 7920 6f66 2074 6865  ',  # any of the
-000010d0: 2073 7570 706f 7274 6564 2073 616d 706c   supported sampl
-000010e0: 6572 730a 290a 6060 600a 0a23 2323 2050  ers.).```..### P
-000010f0: 6170 6572 0a46 6f72 2061 2063 6f6d 7072  aper.For a compr
-00001100: 6568 656e 7369 7665 2077 616c 6b74 6872  ehensive walkthr
-00001110: 6f75 6768 206f 6620 7468 6520 7468 656f  ough of the theo
-00001120: 7279 2061 6e64 2069 6d70 6c65 6d65 6e74  ry and implement
-00001130: 6174 696f 6e20 6f66 2060 6173 7461 7274  ation of `astart
-00001140: 6573 602c 2066 6f6c 6c6f 7720 5b74 6869  es`, follow [thi
-00001150: 7320 6c69 6e6b 5d28 6874 7470 733a 2f2f  s link](https://
-00001160: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
-00001170: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
-00001180: 2f72 6177 2f6a 6f73 732d 7061 7065 722f  /raw/joss-paper/
-00001190: 4275 726e 732d 5370 6965 6b65 726d 616e  Burns-Spiekerman
-000011a0: 6e2d 4268 6174 7461 6368 6172 6a65 655f  n-Bhattacharjee_
-000011b0: 6173 7461 7274 6573 2e70 6466 2920 746f  astartes.pdf) to
-000011c0: 2072 6561 6420 7468 6520 636f 6d70 616e   read the compan
-000011d0: 696f 6e20 7061 7065 722e 0a0a 2323 2320  ion paper...### 
-000011e0: 4578 616d 706c 6520 4e6f 7465 626f 6f6b  Example Notebook
-000011f0: 730a 0a43 6c69 636b 2074 6865 2062 6164  s..Click the bad
-00001200: 6765 7320 696e 2074 6865 2074 6162 6c65  ges in the table
-00001210: 2062 656c 6f77 2074 6f20 6265 2074 616b   below to be tak
-00001220: 656e 2074 6f20 6120 6c69 7665 2c20 696e  en to a live, in
-00001230: 7465 7261 6374 6976 6520 6465 6d6f 206f  teractive demo o
-00001240: 6620 6061 7374 6172 7465 7360 3a0a 0a7c  f `astartes`:..|
-00001250: 2044 656d 6f20 7c20 4c69 6e6b 207c 0a7c   Demo | Link |.|
-00001260: 3a2d 2d2d 3a7c 2d2d 2d7c 0a7c 2055 7369  :---:|---|.| Usi
-00001270: 6e67 2060 7472 6169 6e5f 7661 6c5f 7465  ng `train_val_te
-00001280: 7374 5f73 706c 6974 6020 7769 7468 2074  st_split` with t
-00001290: 6865 2060 736b 6c65 6172 6e60 2065 7861  he `sklearn` exa
-000012a0: 6d70 6c65 2064 6174 6173 6574 7320 7c20  mple datasets | 
-000012b0: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
-000012c0: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-000012d0: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
-000012e0: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
-000012f0: 722e 6f72 672f 7632 2f67 682f 4a61 636b  r.org/v2/gh/Jack
-00001300: 736f 6e42 7572 6e73 2f61 7374 6172 7465  sonBurns/astarte
-00001310: 732f 6d61 696e 3f6c 6162 7061 7468 3d65  s/main?labpath=e
-00001320: 7861 6d70 6c65 7325 3246 7472 6169 6e5f  xamples%2Ftrain_
-00001330: 7661 6c5f 7465 7374 5f73 706c 6974 5f73  val_test_split_s
-00001340: 6b6c 6561 726e 5f65 7861 6d70 6c65 2532  klearn_example%2
-00001350: 4674 7261 696e 5f76 616c 5f74 6573 745f  Ftrain_val_test_
-00001360: 7370 6c69 745f 6578 616d 706c 652e 6970  split_example.ip
-00001370: 796e 6229 207c 0a7c 2043 6f6d 7061 7269  ynb) |.| Compari
-00001380: 6e67 2053 616d 706c 696e 6720 416c 676f  ng Sampling Algo
-00001390: 7269 7468 6d73 2077 6974 6820 4661 7374  rithms with Fast
-000013a0: 2046 6f6f 6420 7c20 5b21 5b42 696e 6465   Food | [![Binde
-000013b0: 725d 2868 7474 7073 3a2f 2f6d 7962 696e  r](https://mybin
-000013c0: 6465 722e 6f72 672f 6261 6467 655f 6c6f  der.org/badge_lo
-000013d0: 676f 2e73 7667 295d 2868 7474 7073 3a2f  go.svg)](https:/
-000013e0: 2f6d 7962 696e 6465 722e 6f72 672f 7632  /mybinder.org/v2
-000013f0: 2f67 682f 4a61 636b 736f 6e42 7572 6e73  /gh/JacksonBurns
-00001400: 2f61 7374 6172 7465 732f 6d61 696e 3f6c  /astartes/main?l
-00001410: 6162 7061 7468 3d65 7861 6d70 6c65 7325  abpath=examples%
-00001420: 3246 7370 6c69 745f 636f 6d70 6172 6973  2Fsplit_comparis
-00001430: 6f6e 7325 3246 7370 6c69 745f 636f 6d70  ons%2Fsplit_comp
-00001440: 6172 6973 6f6e 732e 6970 796e 6229 207c  arisons.ipynb) |
-00001450: 0a7c 2043 6865 6d69 6e66 6f72 6d61 7469  .| Cheminformati
-00001460: 6373 2073 616d 706c 6520 7365 7420 7061  cs sample set pa
-00001470: 7274 6974 696f 6e69 6e67 2077 6974 6820  rtitioning with 
-00001480: 6061 7374 6172 7465 7360 207c 205b 215b  `astartes` | [![
-00001490: 4269 6e64 6572 5d28 6874 7470 733a 2f2f  Binder](https://
-000014a0: 6d79 6269 6e64 6572 2e6f 7267 2f62 6164  mybinder.org/bad
-000014b0: 6765 5f6c 6f67 6f2e 7376 6729 5d28 6874  ge_logo.svg)](ht
-000014c0: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
-000014d0: 7267 2f76 322f 6768 2f4a 6163 6b73 6f6e  rg/v2/gh/Jackson
-000014e0: 4275 726e 732f 6173 7461 7274 6573 2f6d  Burns/astartes/m
-000014f0: 6169 6e3f 6c61 6270 6174 683d 6578 616d  ain?labpath=exam
-00001500: 706c 6573 2532 4662 6172 7269 6572 5f70  ples%2Fbarrier_p
-00001510: 7265 6469 6374 696f 6e5f 7769 7468 5f52  rediction_with_R
-00001520: 4442 3725 3246 5244 4237 5f62 6172 7269  DB7%2FRDB7_barri
-00001530: 6572 5f70 7265 6469 6374 696f 6e5f 6578  er_prediction_ex
-00001540: 616d 706c 652e 6970 796e 6229 207c 0a7c  ample.ipynb) |.|
-00001550: 2043 6f6d 7061 7269 6e67 2070 6172 7469   Comparing parti
-00001560: 7469 6f6e 696e 6720 6170 7072 6f61 6368  tioning approach
-00001570: 6573 2066 6f72 2061 6c6b 616e 6573 207c  es for alkanes |
-00001580: 205b 215b 4269 6e64 6572 5d28 6874 7470   [![Binder](http
-00001590: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
-000015a0: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
-000015b0: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
-000015c0: 6572 2e6f 7267 2f76 322f 6768 2f4a 6163  er.org/v2/gh/Jac
-000015d0: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
-000015e0: 6573 2f6d 6169 6e3f 6c61 6270 6174 683d  es/main?labpath=
-000015f0: 6578 616d 706c 6573 2532 466d 6c70 6473  examples%2Fmlpds
-00001600: 5f32 3032 335f 6173 7461 7274 6573 5f64  _2023_astartes_d
-00001610: 656d 6f25 3246 6d6c 7064 735f 3230 3233  emo%2Fmlpds_2023
-00001620: 5f64 656d 6f2e 6970 796e 6229 207c 0a0a  _demo.ipynb) |..
-00001630: 546f 2065 7865 6375 7465 2074 6865 7365  To execute these
-00001640: 206e 6f74 6562 6f6f 6b73 206c 6f63 616c   notebooks local
-00001650: 6c79 2c20 636c 6f6e 6520 7468 6973 2072  ly, clone this r
-00001660: 6570 6f73 6974 6f72 7920 2869 2e65 2e20  epository (i.e. 
-00001670: 6067 6974 2063 6c6f 6e65 2068 7474 7073  `git clone https
-00001680: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00001690: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-000016a0: 7465 732e 6769 7460 292c 206e 6176 6967  tes.git`), navig
-000016b0: 6174 6520 746f 2074 6865 2060 6173 7461  ate to the `asta
-000016c0: 7274 6573 6020 6469 7265 6374 6f72 792c  rtes` directory,
-000016d0: 2072 756e 2060 7069 7020 696e 7374 616c   run `pip instal
-000016e0: 6c20 2e5b 6465 6d6f 735d 602c 2074 6865  l .[demos]`, the
-000016f0: 6e20 6f70 656e 2061 6e64 2072 756e 2074  n open and run t
-00001700: 6865 206e 6f74 6562 6f6f 6b73 2069 6e20  he notebooks in 
-00001710: 796f 7572 2070 7265 6665 7272 6564 2065  your preferred e
-00001720: 6469 746f 722e 0a0a 2323 2320 5261 7469  ditor...### Rati
-00001730: 6f6e 616c 2053 706c 6974 7469 6e67 2041  onal Splitting A
-00001740: 6c67 6f72 6974 686d 730a 5768 696c 6520  lgorithms.While 
-00001750: 6d75 6368 206d 6163 6869 6e65 206c 6561  much machine lea
-00001760: 726e 696e 6720 6973 2064 6f6e 6520 7769  rning is done wi
-00001770: 7468 2061 2072 616e 646f 6d20 6368 6f69  th a random choi
-00001780: 6365 2062 6574 7765 656e 2074 7261 696e  ce between train
-00001790: 696e 672f 7661 6c69 6461 7469 6f6e 2f74  ing/validation/t
-000017a0: 6573 7420 6461 7461 2c20 616e 2061 6c74  est data, an alt
-000017b0: 6572 6e61 7469 7665 2069 7320 7468 6520  ernative is the 
-000017c0: 7573 6520 6f66 2073 6f2d 6361 6c6c 6564  use of so-called
-000017d0: 2022 7261 7469 6f6e 616c 2220 7370 6c69   "rational" spli
-000017e0: 7474 696e 6720 616c 676f 7269 7468 6d73  tting algorithms
-000017f0: 2e20 5468 6573 6520 6170 7072 6f61 6368  . These approach
-00001800: 6573 2075 7365 2073 6f6d 6520 7369 6d69  es use some simi
-00001810: 6c61 7269 7479 2d62 6173 6564 2061 6c67  larity-based alg
-00001820: 6f72 6974 686d 2074 6f20 6469 7669 6465  orithm to divide
-00001830: 2064 6174 6120 696e 746f 2073 6574 732e   data into sets.
-00001840: 2053 6f6d 6520 6f66 2074 6865 7365 2061   Some of these a
-00001850: 6c67 6f72 6974 686d 7320 696e 636c 7564  lgorithms includ
-00001860: 6520 4b65 6e6e 6172 642d 5374 6f6e 652c  e Kennard-Stone,
-00001870: 206d 696e 696d 616c 2074 6573 7420 7365   minimal test se
-00001880: 7420 6469 7373 696d 696c 6172 6974 792c  t dissimilarity,
-00001890: 2061 6e64 2073 7068 6572 6520 6578 636c   and sphere excl
-000018a0: 7573 696f 6e20 616c 676f 7269 7468 6d73  usion algorithms
-000018b0: 205b 6173 2064 6973 6375 7373 6564 2062   [as discussed b
-000018c0: 7920 5472 6f70 7368 6120 6574 2e20 616c  y Tropsha et. al
-000018d0: 5d28 6874 7470 733a 2f2f 7075 6273 2e61  ](https://pubs.a
-000018e0: 6373 2e6f 7267 2f64 6f69 2f70 6466 2f31  cs.org/doi/pdf/1
-000018f0: 302e 3130 3231 2f63 6933 3030 3333 3877  0.1021/ci300338w
-00001900: 2920 6173 2077 656c 6c20 6173 2074 6865  ) as well as the
-00001910: 204f 7074 6953 696d 2061 7320 6469 7363   OptiSim as disc
-00001920: 7573 7365 6420 696e 205b 4170 706c 6965  ussed in [Applie
-00001930: 6420 4368 656d 6f69 6e66 6f72 6d61 7469  d Chemoinformati
-00001940: 6373 3a20 4163 6869 6576 656d 656e 7473  cs: Achievements
-00001950: 2061 6e64 2046 7574 7572 6520 4f70 706f   and Future Oppo
-00001960: 7274 756e 6974 6965 735d 2868 7474 7073  rtunities](https
-00001970: 3a2f 2f77 7777 2e77 696c 6579 2e63 6f6d  ://www.wiley.com
-00001980: 2f65 6e2d 7573 2f41 7070 6c69 6564 2b43  /en-us/Applied+C
-00001990: 6865 6d6f 696e 666f 726d 6174 6963 7325  hemoinformatics%
-000019a0: 3341 2b41 6368 6965 7665 6d65 6e74 732b  3A+Achievements+
-000019b0: 616e 642b 4675 7475 7265 2b4f 7070 6f72  and+Future+Oppor
-000019c0: 7475 6e69 7469 6573 2d70 2d39 3738 3335  tunities-p-97835
-000019d0: 3237 3830 3635 3436 292e 2053 6f6d 6520  27806546). Some 
-000019e0: 636c 7573 7465 7269 6e67 2d62 6173 6564  clustering-based
-000019f0: 2073 706c 6974 7469 6e67 2074 6563 686e   splitting techn
-00001a00: 6971 7565 7320 6861 7665 2061 6c73 6f20  iques have also 
-00001a10: 6265 656e 2069 6e63 6f72 706f 7261 7465  been incorporate
-00001a20: 642c 2073 7563 6820 6173 205b 4442 5343  d, such as [DBSC
-00001a30: 414e 5d28 6874 7470 3a2f 2f63 6974 6573  AN](http://cites
-00001a40: 6565 7278 2e69 7374 2e70 7375 2e65 6475  eerx.ist.psu.edu
-00001a50: 2f76 6965 7764 6f63 2f64 6f77 6e6c 6f61  /viewdoc/downloa
-00001a60: 643f 646f 693d 3130 2e31 2e31 2e31 3031  d?doi=10.1.1.101
-00001a70: 362e 3839 3026 7265 703d 7265 7031 2674  6.890&rep=rep1&t
-00001a80: 7970 653d 7064 6629 2e0a 0a54 6865 7265  ype=pdf)...There
-00001a90: 2061 7265 2074 776f 2062 726f 6164 2063   are two broad c
-00001aa0: 6174 6567 6f72 6965 7320 6f66 2073 616d  ategories of sam
-00001ab0: 706c 696e 6720 616c 676f 7269 7468 6d73  pling algorithms
-00001ac0: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-00001ad0: 6061 7374 6172 7465 7360 3a20 6578 7472  `astartes`: extr
-00001ae0: 6170 6f6c 6174 6976 6520 616e 6420 696e  apolative and in
-00001af0: 7465 7270 6f6c 6174 6976 652e 2054 6865  terpolative. The
-00001b00: 2066 6f72 6d65 7220 7769 6c6c 2066 6f72   former will for
-00001b10: 6365 2079 6f75 7220 6d6f 6465 6c20 746f  ce your model to
-00001b20: 2070 7265 6469 6374 206f 6e20 6f75 742d   predict on out-
-00001b30: 6f66 2d73 616d 706c 6520 6461 7461 2c20  of-sample data, 
-00001b40: 7768 6963 6820 6372 6561 7465 7320 6120  which creates a 
-00001b50: 6d6f 7265 2063 6861 6c6c 656e 6769 6e67  more challenging
-00001b60: 2074 6173 6b20 7468 616e 2069 6e74 6572   task than inter
-00001b70: 706f 6c61 7469 7665 2073 616d 706c 696e  polative samplin
-00001b80: 672e 2053 6565 2074 6865 2074 6162 6c65  g. See the table
-00001b90: 2062 656c 6f77 2066 6f72 2061 6c6c 206f   below for all o
-00001ba0: 6620 7468 6520 7361 6d70 6c69 6e67 2061  f the sampling a
-00001bb0: 7070 726f 6163 6865 7320 6375 7272 656e  pproaches curren
-00001bc0: 746c 7920 696d 706c 656d 656e 7465 6420  tly implemented 
-00001bd0: 696e 2060 6173 7461 7274 6573 602c 2061  in `astartes`, a
-00001be0: 7320 7765 6c6c 2061 7320 7468 6520 6879  s well as the hy
-00001bf0: 7065 7270 6172 616d 6574 6572 7320 7468  perparameters th
-00001c00: 6174 2065 6163 6820 616c 676f 7269 7468  at each algorith
-00001c10: 6d20 6163 6365 7074 7320 2877 6869 6368  m accepts (which
-00001c20: 2061 7265 2070 6173 7365 6420 696e 2077   are passed in w
-00001c30: 6974 6820 6068 6f70 7473 6029 2061 6e64  ith `hopts`) and
-00001c40: 2061 2068 656c 7066 756c 2072 6566 6572   a helpful refer
-00001c50: 656e 6365 2066 6f72 2075 6e64 6572 7374  ence for underst
-00001c60: 616e 6469 6e67 2068 6f77 2074 6865 2068  anding how the h
-00001c70: 7970 6572 7061 7261 6d65 7465 7273 2077  yperparameters w
-00001c80: 6f72 6b2e 204e 6f74 6520 7468 6174 2060  ork. Note that `
-00001c90: 7261 6e64 6f6d 5f73 7461 7465 6020 6973  random_state` is
-00001ca0: 2064 6566 696e 6564 2061 7320 6120 6b65   defined as a ke
-00001cb0: 7977 6f72 6420 6172 6775 6d65 6e74 2069  yword argument i
-00001cc0: 6e20 6074 7261 696e 5f74 6573 745f 7370  n `train_test_sp
-00001cd0: 6c69 7460 2069 7473 656c 662c 2065 7665  lit` itself, eve
-00001ce0: 6e20 7468 6f75 6768 2074 6865 7365 2061  n though these a
-00001cf0: 6c67 6f72 6974 686d 7320 7769 6c6c 2075  lgorithms will u
-00001d00: 7365 2074 6865 2060 7261 6e64 6f6d 5f73  se the `random_s
-00001d10: 7461 7465 6020 696e 2074 6865 6972 206f  tate` in their o
-00001d20: 776e 2077 6f72 6b2e 2044 6f20 6e6f 7420  wn work. Do not 
-00001d30: 7072 6f76 6964 6520 6120 6072 616e 646f  provide a `rando
-00001d40: 6d5f 7374 6174 6560 2069 6e20 7468 6520  m_state` in the 
-00001d50: 6068 6f70 7473 6020 6469 6374 696f 6e61  `hopts` dictiona
-00001d60: 7279 202d 2069 7420 7769 6c6c 2062 6520  ry - it will be 
-00001d70: 6f76 6572 7772 6974 7465 6e20 6279 2074  overwritten by t
-00001d80: 6865 2060 7261 6e64 6f6d 5f73 7461 7465  he `random_state
-00001d90: 6020 796f 7520 7072 6f76 6964 6520 666f  ` you provide fo
-00001da0: 7220 6074 7261 696e 5f74 6573 745f 7370  r `train_test_sp
-00001db0: 6c69 7460 2028 6f72 2074 6865 2064 6566  lit` (or the def
-00001dc0: 6175 6c74 2069 6620 6e6f 6e65 2069 7320  ault if none is 
-00001dd0: 7072 6f76 6964 6564 292e 0a0a 2323 2323  provided)...####
-00001de0: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
-00001df0: 706c 696e 6720 416c 676f 7269 7468 6d73  pling Algorithms
-00001e00: 0a0a 7c20 5361 6d70 6c65 7220 4e61 6d65  ..| Sampler Name
-00001e10: 207c 2055 7361 6765 2053 7472 696e 6720   | Usage String 
-00001e20: 7c20 5479 7065 207c 2048 7970 6572 7061  | Type | Hyperpa
-00001e30: 7261 6d65 7465 7273 207c 2052 6566 6572  rameters | Refer
-00001e40: 656e 6365 207c 204e 6f74 6573 207c 0a7c  ence | Notes |.|
-00001e50: 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d 2d7c 2d2d  :---:|---|---|--
-00001e60: 2d7c 2d2d 2d7c 2d2d 2d7c 0a7c 2052 616e  -|---|---|.| Ran
-00001e70: 646f 6d20 7c20 2772 616e 646f 6d27 207c  dom | 'random' |
-00001e80: 2049 6e74 6572 706f 6c61 7469 7665 207c   Interpolative |
-00001e90: 2060 7368 7566 666c 6560 207c 205b 6073   `shuffle` | [`s
-00001ea0: 6b6c 6561 726e 2074 7261 696e 5f74 6573  klearn train_tes
-00001eb0: 745f 7370 6c69 7460 5d28 6874 7470 733a  t_split`](https:
-00001ec0: 2f2f 7363 696b 6974 2d6c 6561 726e 2e6f  //scikit-learn.o
-00001ed0: 7267 2f73 7461 626c 652f 6d6f 6475 6c65  rg/stable/module
-00001ee0: 732f 6765 6e65 7261 7465 642f 736b 6c65  s/generated/skle
-00001ef0: 6172 6e2e 6d6f 6465 6c5f 7365 6c65 6374  arn.model_select
-00001f00: 696f 6e2e 7472 6169 6e5f 7465 7374 5f73  ion.train_test_s
-00001f10: 706c 6974 2e68 746d 6c29 207c 2054 6869  plit.html) | Thi
-00001f20: 7320 7361 6d70 6c65 7220 6973 2061 2064  s sampler is a d
-00001f30: 6972 6563 7420 7061 7373 7468 726f 7567  irect passthroug
-00001f40: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
-00001f50: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
-00001f60: 6974 602c 2074 686f 7567 6820 6974 2064  it`, though it d
-00001f70: 6f65 7320 6e6f 7420 6375 7272 656e 746c  oes not currentl
-00001f80: 7920 7265 7072 6f64 7563 6520 7370 6c69  y reproduce spli
-00001f90: 7473 2069 6465 6e74 6963 616c 6c79 2e20  ts identically. 
-00001fa0: 7c0a 7c20 4b65 6e6e 6172 642d 5374 6f6e  |.| Kennard-Ston
-00001fb0: 6520 7c20 276b 656e 6e61 7264 5f73 746f  e | 'kennard_sto
-00001fc0: 6e65 2720 7c20 496e 7465 7270 6f6c 6174  ne' | Interpolat
-00001fd0: 6976 6520 7c20 606d 6574 7269 6360 207c  ive | `metric` |
-00001fe0: 205b 4b65 6e6e 6172 6420 2620 5374 6f6e   [Kennard & Ston
-00001ff0: 655d 2868 7474 7073 3a2f 2f77 7777 2e74  e](https://www.t
-00002000: 616e 6466 6f6e 6c69 6e65 2e63 6f6d 2f64  andfonline.com/d
-00002010: 6f69 2f61 6273 2f31 302e 3130 3830 2f30  oi/abs/10.1080/0
-00002020: 3034 3031 3730 362e 3139 3639 2e31 3034  0401706.1969.104
-00002030: 3930 3636 3629 207c 2045 7563 6c69 6469  90666) | Euclidi
-00002040: 616e 2064 6973 7461 6e63 6520 6973 2075  an distance is u
-00002050: 7365 6420 6279 2064 6566 6175 6c74 2c20  sed by default, 
-00002060: 6173 2064 6573 6372 6962 6564 2069 6e20  as described in 
-00002070: 7468 6520 6f72 6967 696e 616c 2070 6170  the original pap
-00002080: 6572 2e20 7c0a 7c20 5361 6d70 6c65 2073  er. |.| Sample s
-00002090: 6574 2050 6172 7469 7469 6f6e 696e 6720  et Partitioning 
-000020a0: 6261 7365 6420 6f6e 206a 6f69 6e74 2058  based on joint X
-000020b0: 2d59 2064 6973 7461 6e63 6573 2028 5350  -Y distances (SP
-000020c0: 5859 2920 7c20 2773 7078 7927 207c 2049  XY) | 'spxy' | I
-000020d0: 6e74 6572 706f 6c61 7469 7665 207c 2060  nterpolative | `
-000020e0: 6469 7374 616e 6365 5f6d 6574 7269 6360  distance_metric`
-000020f0: 207c 2053 616c 6468 616e 6120 6574 2e20   | Saldhana et. 
-00002100: 616c 205b 6f72 6967 696e 616c 2070 6170  al [original pap
-00002110: 6572 5d28 6874 7470 733a 2f2f 7777 772e  er](https://www.
-00002120: 7363 6965 6e63 6564 6972 6563 742e 636f  sciencedirect.co
-00002130: 6d2f 7363 6965 6e63 652f 6172 7469 636c  m/science/articl
-00002140: 652f 6162 732f 7069 692f 5330 3033 3939  e/abs/pii/S00399
-00002150: 3134 3030 3530 3031 3932 5829 207c 2045  1400500192X) | E
-00002160: 7874 656e 7369 6f6e 206f 6620 4b65 6e6e  xtension of Kenn
-00002170: 6172 6420 5374 6f6e 6520 7468 6174 2061  ard Stone that a
-00002180: 6c73 6f20 696e 636c 7564 6573 2074 6865  lso includes the
-00002190: 2072 6573 706f 6e73 6520 7768 656e 2073   response when s
-000021a0: 616d 706c 696e 6720 6469 7374 616e 6365  ampling distance
-000021b0: 732e 207c 0a7c 2053 6361 6666 6f6c 6420  s. |.| Scaffold 
-000021c0: 7c20 2773 6361 6666 6f6c 6427 207c 2045  | 'scaffold' | E
-000021d0: 7874 7261 706f 6c61 7469 7665 207c 2060  xtrapolative | `
-000021e0: 696e 636c 7564 655f 6368 6972 616c 6974  include_chiralit
-000021f0: 7960 207c 205b 4265 6d69 732d 4d75 7263  y` | [Bemis-Murc
-00002200: 6b6f 2053 6361 6666 6f6c 645d 2868 7474  ko Scaffold](htt
-00002210: 7073 3a2f 2f70 7562 732e 6163 732e 6f72  ps://pubs.acs.or
-00002220: 672f 646f 692f 6675 6c6c 2f31 302e 3130  g/doi/full/10.10
-00002230: 3231 2f6a 6d39 3630 3239 3238 2920 6173  21/jm9602928) as
-00002240: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-00002250: 5244 4b69 7420 7c20 5468 6973 2073 616d  RDKit | This sam
-00002260: 706c 6572 2072 6571 7569 7265 7320 534d  pler requires SM
-00002270: 494c 4553 2073 7472 696e 6773 2061 7320  ILES strings as 
-00002280: 696e 7075 7420 2875 7365 2074 6865 2060  input (use the `
-00002290: 6d6f 6c65 6375 6c65 7360 2073 7562 7061  molecules` subpa
-000022a0: 636b 6167 6529 207c 0a7c 2053 7068 6572  ckage) |.| Spher
-000022b0: 6520 4578 636c 7573 696f 6e20 7c20 2773  e Exclusion | 's
-000022c0: 7068 6572 655f 6578 636c 7573 696f 6e27  phere_exclusion'
-000022d0: 207c 2045 7874 7261 706f 6c61 7469 7665   | Extrapolative
-000022e0: 207c 2060 6d65 7472 6963 602c 2060 6469   | `metric`, `di
-000022f0: 7374 616e 6365 5f63 7574 6f66 6660 207c  stance_cutoff` |
-00002300: 205f 6375 7374 6f6d 2069 6d70 6c65 6d65   _custom impleme
-00002310: 6e74 6174 696f 6e5f 207c 2056 6172 6961  ntation_ | Varia
-00002320: 7469 6f6e 206f 6e20 5370 6865 7265 2045  tion on Sphere E
-00002330: 7863 6c75 7369 6f6e 2066 6f72 2061 7262  xclusion for arb
-00002340: 6974 7261 7279 2d76 616c 7565 6420 7665  itrary-valued ve
-00002350: 6374 6f72 732e 207c 0a7c 2054 696d 6520  ctors. |.| Time 
-00002360: 4261 7365 6420 7c20 2774 696d 655f 6261  Based | 'time_ba
-00002370: 7365 6427 207c 2045 7874 7261 706f 6c61  sed' | Extrapola
-00002380: 7469 7665 207c 205f 6e6f 6e65 5f20 7c20  tive | _none_ | 
-00002390: 5b43 6865 6e20 6574 2061 6c2e 5d28 6874  [Chen et al.](ht
-000023a0: 7470 733a 2f2f 7075 6273 2e61 6373 2e6f  tps://pubs.acs.o
-000023b0: 7267 2f64 6f69 2f66 756c 6c2f 3130 2e31  rg/doi/full/10.1
-000023c0: 3032 312f 6369 3230 3036 3135 6829 2c20  021/ci200615h), 
-000023d0: 5b53 6865 7269 6461 6e2c 2052 2e20 505d  [Sheridan, R. P]
-000023e0: 2868 7474 7073 3a2f 2f70 7562 732e 6163  (https://pubs.ac
-000023f0: 732e 6f72 672f 646f 692f 6675 6c6c 2f31  s.org/doi/full/1
-00002400: 302e 3130 3231 2f63 6934 3030 3038 346b  0.1021/ci400084k
-00002410: 292c 205b 4665 696e 6265 7267 2065 7420  ), [Feinberg et 
-00002420: 616c 2e5d 2868 7474 7073 3a2f 2f70 7562  al.](https://pub
-00002430: 732e 6163 732e 6f72 672f 646f 692f 6675  s.acs.org/doi/fu
-00002440: 6c6c 2f31 302e 3130 3231 2f61 6373 2e6a  ll/10.1021/acs.j
-00002450: 6d65 6463 6865 6d2e 3962 3032 3138 3729  medchem.9b02187)
-00002460: 2c20 5b53 7472 7562 6c65 2065 7420 616c  , [Struble et al
-00002470: 2e5d 2868 7474 7073 3a2f 2f70 7562 732e  .](https://pubs.
-00002480: 7273 632e 6f72 672f 656e 2f63 6f6e 7465  rsc.org/en/conte
-00002490: 6e74 2f61 7274 6963 6c65 6874 6d6c 2f32  nt/articlehtml/2
-000024a0: 3032 302f 7265 2f64 3072 6530 3030 3731  020/re/d0re00071
-000024b0: 6a29 2020 7c20 5468 6973 2073 616d 706c  j)  | This sampl
-000024c0: 6572 2072 6571 7569 7265 7320 606c 6162  er requires `lab
-000024d0: 656c 7360 2074 6f20 6265 2061 6e20 6974  els` to be an it
-000024e0: 6572 6162 6c65 206f 6620 6569 7468 6572  erable of either
-000024f0: 2064 6174 6520 6f72 2064 6174 6574 696d   date or datetim
-00002500: 6520 6f62 6a65 6374 732e 207c 0a7c 204f  e objects. |.| O
-00002510: 7074 696d 697a 6162 6c65 204b 2d44 6973  ptimizable K-Dis
-00002520: 7369 6d69 6c61 7269 7479 2053 656c 6563  similarity Selec
-00002530: 7469 6f6e 2028 4f70 7469 5369 6d29 207c  tion (OptiSim) |
-00002540: 2027 6f70 7469 7369 6d27 207c 2045 7874   'optisim' | Ext
-00002550: 7261 706f 6c61 7469 7665 207c 2060 6e5f  rapolative | `n_
-00002560: 636c 7573 7465 7273 602c 2060 6d61 785f  clusters`, `max_
-00002570: 7375 6273 616d 706c 655f 7369 7a65 602c  subsample_size`,
-00002580: 2060 6469 7374 616e 6365 5f63 7574 6f66   `distance_cutof
-00002590: 6660 207c 205f 6375 7374 6f6d 2069 6d70  f` | _custom imp
-000025a0: 6c65 6d65 6e74 6174 696f 6e5f 207c 2056  lementation_ | V
-000025b0: 6172 6961 7469 6f6e 206f 6e20 5b4f 7074  ariation on [Opt
-000025c0: 6953 696d 5d28 6874 7470 733a 2f2f 7075  iSim](https://pu
-000025d0: 6273 2e61 6373 2e6f 7267 2f64 6f69 2f31  bs.acs.org/doi/1
-000025e0: 302e 3130 3231 2f63 6930 3235 3636 3268  0.1021/ci025662h
-000025f0: 2920 666f 7220 6172 6269 7472 6172 792d  ) for arbitrary-
-00002600: 7661 6c75 6564 2076 6563 746f 7273 2e20  valued vectors. 
-00002610: 7c0a 7c20 4b2d 4d65 616e 7320 7c20 276b  |.| K-Means | 'k
-00002620: 6d65 616e 7327 207c 2045 7874 7261 706f  means' | Extrapo
-00002630: 6c61 7469 7665 207c 2060 6e5f 636c 7573  lative | `n_clus
-00002640: 7465 7273 602c 2060 6e5f 696e 6974 6020  ters`, `n_init` 
-00002650: 7c20 5b60 736b 6c65 6172 6e20 4b4d 6561  | [`sklearn KMea
-00002660: 6e73 605d 2868 7474 7073 3a2f 2f73 6369  ns`](https://sci
-00002670: 6b69 742d 6c65 6172 6e2e 6f72 672f 7374  kit-learn.org/st
-00002680: 6162 6c65 2f6d 6f64 756c 6573 2f67 656e  able/modules/gen
-00002690: 6572 6174 6564 2f73 6b6c 6561 726e 2e63  erated/sklearn.c
-000026a0: 6c75 7374 6572 2e4b 4d65 616e 732e 6874  luster.KMeans.ht
-000026b0: 6d6c 2920 7c20 5061 7373 7468 726f 7567  ml) | Passthroug
-000026c0: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
-000026d0: 2060 4b4d 6561 6e73 602e 207c 0a7c 2044   `KMeans`. |.| D
-000026e0: 656e 7369 7479 2d42 6173 6564 2053 7061  ensity-Based Spa
-000026f0: 7469 616c 2043 6c75 7374 6572 696e 6720  tial Clustering 
-00002700: 6f66 2041 7070 6c69 6361 7469 6f6e 7320  of Applications 
-00002710: 7769 7468 204e 6f69 7365 2028 4442 5343  with Noise (DBSC
-00002720: 414e 2920 7c20 2764 6273 6361 6e27 207c  AN) | 'dbscan' |
-00002730: 2045 7874 7261 706f 6c61 7469 7665 207c   Extrapolative |
-00002740: 2060 6570 7360 2c20 606d 696e 5f73 616d   `eps`, `min_sam
-00002750: 706c 6573 602c 2060 616c 676f 7269 7468  ples`, `algorith
-00002760: 6d60 2c20 606d 6574 7269 6360 2c20 606c  m`, `metric`, `l
-00002770: 6561 665f 7369 7a65 6020 7c20 5b60 736b  eaf_size` | [`sk
-00002780: 6c65 6172 6e20 4442 5343 414e 605d 2868  learn DBSCAN`](h
-00002790: 7474 7073 3a2f 2f73 6369 6b69 742d 6c65  ttps://scikit-le
-000027a0: 6172 6e2e 6f72 672f 7374 6162 6c65 2f6d  arn.org/stable/m
-000027b0: 6f64 756c 6573 2f67 656e 6572 6174 6564  odules/generated
-000027c0: 2f73 6b6c 6561 726e 2e63 6c75 7374 6572  /sklearn.cluster
-000027d0: 2e44 4253 4341 4e2e 6874 6d6c 2920 7c20  .DBSCAN.html) | 
-000027e0: 5061 7373 7468 726f 7567 6820 746f 2060  Passthrough to `
-000027f0: 736b 6c65 6172 6e60 2773 2060 4442 5343  sklearn`'s `DBSC
-00002800: 414e 602e 207c 0a7c 204d 696e 696d 756d  AN`. |.| Minimum
-00002810: 2054 6573 7420 5365 7420 4469 7373 696d   Test Set Dissim
-00002820: 696c 6172 6974 7920 284d 5453 4429 207c  ilarity (MTSD) |
-00002830: 207e 207c 207e 207c 205f 7570 636f 6d69   ~ | ~ | _upcomi
-00002840: 6e67 2069 6e5f 2060 6173 7461 7274 6573  ng in_ `astartes
-00002850: 6020 5f76 312e 785f 207c 207e 207c 207e  ` _v1.x_ | ~ | ~
-00002860: 207c 0a7c 2052 6573 7472 6963 7465 6420   |.| Restricted 
-00002870: 426f 6c74 7a6d 616e 6e20 4d61 6368 696e  Boltzmann Machin
-00002880: 6520 2852 424d 2920 7c20 7e20 7c20 7e20  e (RBM) | ~ | ~ 
-00002890: 7c20 5f75 7063 6f6d 696e 6720 696e 5f20  | _upcoming in_ 
-000028a0: 6061 7374 6172 7465 7360 205f 7631 2e78  `astartes` _v1.x
-000028b0: 5f20 7c20 7e20 7c20 7e20 7c0a 7c20 4b6f  _ | ~ | ~ |.| Ko
-000028c0: 686f 6e65 6e20 5365 6c66 2d4f 7267 616e  honen Self-Organ
-000028d0: 697a 696e 6720 4d61 7020 2853 4f4d 2920  izing Map (SOM) 
-000028e0: 7c20 7e20 7c20 7e20 7c20 5f75 7063 6f6d  | ~ | ~ | _upcom
-000028f0: 696e 6720 696e 5f20 6061 7374 6172 7465  ing in_ `astarte
-00002900: 7360 205f 7631 2e78 5f20 7c20 7e20 7c20  s` _v1.x_ | ~ | 
-00002910: 7e20 7c0a 7c20 5350 6c69 7420 4d65 7468  ~ |.| SPlit Meth
-00002920: 6f64 207c 207e 207c 207e 207c 205f 7570  od | ~ | ~ | _up
-00002930: 636f 6d69 6e67 2069 6e5f 2060 6173 7461  coming in_ `asta
-00002940: 7274 6573 6020 5f76 312e 785f 207c 207e  rtes` _v1.x_ | ~
-00002950: 207c 207e 207c 0a0a 2323 2320 5573 696e   | ~ |..### Usin
-00002960: 6720 7468 6520 6061 7374 6172 7465 732e  g the `astartes.
-00002970: 6d6f 6c65 6375 6c65 7360 2053 7562 7061  molecules` Subpa
-00002980: 636b 6167 650a 4166 7465 7220 696e 7374  ckage.After inst
-00002990: 616c 6c69 6e67 2077 6974 6820 6070 6970  alling with `pip
-000029a0: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
-000029b0: 735b 6d6f 6c65 6375 6c65 735d 6020 6f6e  s[molecules]` on
-000029c0: 6520 6361 6e20 696d 706f 7274 2074 6865  e can import the
-000029d0: 206e 6577 2074 7261 696e 2f74 6573 7420   new train/test 
-000029e0: 7370 6c69 7474 696e 6720 6675 6e63 7469  splitting functi
-000029f0: 6f6e 206c 696b 6520 7468 6973 3a20 6066  on like this: `f
-00002a00: 726f 6d20 6173 7461 7274 6573 2e6d 6f6c  rom astartes.mol
-00002a10: 6563 756c 6573 2069 6d70 6f72 7420 7472  ecules import tr
-00002a20: 6169 6e5f 7465 7374 5f73 706c 6974 5f6d  ain_test_split_m
-00002a30: 6f6c 6563 756c 6573 600a 0a54 6865 2075  olecules`..The u
-00002a40: 7361 6765 206f 6620 7468 6973 2066 756e  sage of this fun
-00002a50: 6374 696f 6e20 6973 2069 6465 6e74 6963  ction is identic
-00002a60: 616c 2074 6f20 6074 7261 696e 5f74 6573  al to `train_tes
-00002a70: 745f 7370 6c69 7460 2062 7574 2077 6974  t_split` but wit
-00002a80: 6820 7468 6520 6164 6469 7469 6f6e 206f  h the addition o
-00002a90: 6620 6e65 7720 6172 6775 6d65 6e74 7320  f new arguments 
-00002aa0: 746f 2063 6f6e 7472 6f6c 2068 6f77 2074  to control how t
-00002ab0: 6865 206d 6f6c 6563 756c 6573 2061 7265  he molecules are
-00002ac0: 2066 6561 7475 7269 7a65 643a 0a0a 6060   featurized:..``
-00002ad0: 6070 7974 686f 6e0a 7472 6169 6e5f 7465  `python.train_te
-00002ae0: 7374 5f73 706c 6974 5f6d 6f6c 6563 756c  st_split_molecul
-00002af0: 6573 280a 2020 2020 6d6f 6c65 6375 6c65  es(.    molecule
-00002b00: 733d 736d 696c 6573 2c0a 2020 2020 793d  s=smiles,.    y=
-00002b10: 792c 0a20 2020 2074 6573 745f 7369 7a65  y,.    test_size
-00002b20: 3d30 2e32 2c0a 2020 2020 7472 6169 6e5f  =0.2,.    train_
-00002b30: 7369 7a65 3d30 2e38 2c0a 2020 2020 6669  size=0.8,.    fi
-00002b40: 6e67 6572 7072 696e 743d 2264 6179 6c69  ngerprint="dayli
-00002b50: 6768 745f 6669 6e67 6572 7072 696e 7422  ght_fingerprint"
-00002b60: 2c0a 2020 2020 6670 7269 6e74 735f 686f  ,.    fprints_ho
-00002b70: 7074 733d 7b0a 2020 2020 2020 2020 226d  pts={.        "m
-00002b80: 696e 5061 7468 223a 2032 2c0a 2020 2020  inPath": 2,.    
-00002b90: 2020 2020 226d 6178 5061 7468 223a 2035      "maxPath": 5
-00002ba0: 2c0a 2020 2020 2020 2020 2266 7053 697a  ,.        "fpSiz
-00002bb0: 6522 3a20 3230 302c 0a20 2020 2020 2020  e": 200,.       
-00002bc0: 2022 6269 7473 5065 7248 6173 6822 3a20   "bitsPerHash": 
-00002bd0: 342c 0a20 2020 2020 2020 2022 7573 6548  4,.        "useH
-00002be0: 7322 3a20 312c 0a20 2020 2020 2020 2022  s": 1,.        "
-00002bf0: 7467 7444 656e 7369 7479 223a 2030 2e34  tgtDensity": 0.4
-00002c00: 2c0a 2020 2020 2020 2020 226d 696e 5369  ,.        "minSi
-00002c10: 7a65 223a 2036 342c 0a20 2020 207d 2c0a  ze": 64,.    },.
-00002c20: 2020 2020 7361 6d70 6c65 723d 2272 616e      sampler="ran
-00002c30: 646f 6d22 2c0a 2020 2020 7261 6e64 6f6d  dom",.    random
-00002c40: 5f73 7461 7465 3d34 322c 0a20 2020 2068  _state=42,.    h
-00002c50: 6f70 7473 3d7b 0a20 2020 2020 2020 2022  opts={.        "
-00002c60: 7368 7566 666c 6522 3a20 5472 7565 2c0a  shuffle": True,.
-00002c70: 2020 2020 7d2c 0a29 0a60 6060 0a0a 546f      },.).```..To
-00002c80: 2073 6565 2061 2063 6f6d 706c 6574 6520   see a complete 
-00002c90: 6578 616d 706c 6520 6f66 2075 7369 6e67  example of using
-00002ca0: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
-00002cb0: 6974 5f6d 6f6c 6563 756c 6573 6020 7769  it_molecules` wi
-00002cc0: 7468 2061 6374 7561 6c20 6368 656d 6963  th actual chemic
-00002cd0: 616c 2064 6174 612c 2074 616b 6520 6120  al data, take a 
-00002ce0: 6c6f 6f6b 2069 6e20 7468 6520 6065 7861  look in the `exa
-00002cf0: 6d70 6c65 7360 2064 6972 6563 746f 7279  mples` directory
-00002d00: 2e0a 0a43 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
-00002d10: 206f 7074 696f 6e73 2066 6f72 2074 6865   options for the
-00002d20: 2066 6561 7475 7269 7a61 7469 6f6e 2073   featurization s
-00002d30: 6368 656d 6520 6361 6e20 6265 2066 6f75  cheme can be fou
-00002d40: 6e64 2069 6e20 7468 6520 646f 6375 6d65  nd in the docume
-00002d50: 6e74 6174 696f 6e20 666f 7220 5b60 4149  ntation for [`AI
-00002d60: 4d53 696d 605d 2868 7474 7073 3a2f 2f76  MSim`](https://v
-00002d70: 6c61 6368 6f73 6772 6f75 702e 6769 7468  lachosgroup.gith
-00002d80: 7562 2e69 6f2f 4149 4d53 696d 2f52 4541  ub.io/AIMSim/REA
-00002d90: 444d 452e 6874 6d6c 2363 7572 7265 6e74  DME.html#current
-00002da0: 6c79 2d69 6d70 6c65 6d65 6e74 6564 2d66  ly-implemented-f
-00002db0: 696e 6765 7270 7269 6e74 7329 2074 686f  ingerprints) tho
-00002dc0: 7567 6820 6d6f 7374 206f 6620 7468 6520  ugh most of the 
-00002dd0: 6372 6974 6963 616c 2063 6f6e 6669 6775  critical configu
-00002de0: 7261 7469 6f6e 206f 7074 696f 6e73 2061  ration options a
-00002df0: 7265 2073 686f 776e 2061 626f 7665 2e0a  re shown above..
-00002e00: 0a23 2323 2052 6570 726f 6475 6369 6269  .### Reproducibi
-00002e10: 6c69 7479 0a60 6173 7461 7274 6573 6020  lity.`astartes` 
-00002e20: 6169 6d73 2074 6f20 6265 2063 6f6d 706c  aims to be compl
-00002e30: 6574 656c 7920 7265 7072 6f64 7563 6962  etely reproducib
-00002e40: 6c65 2061 6372 6f73 7320 6469 6666 6572  le across differ
-00002e50: 656e 7420 706c 6174 666f 726d 732c 2050  ent platforms, P
-00002e60: 7974 686f 6e20 7665 7273 696f 6e73 2c20  ython versions, 
-00002e70: 616e 6420 6465 7065 6e64 656e 6379 2063  and dependency c
-00002e80: 6f6e 6669 6775 7261 7469 6f6e 7320 2d20  onfigurations - 
-00002e90: 616e 7920 7665 7273 696f 6e20 6f66 2060  any version of `
-00002ea0: 6173 7461 7274 6573 6020 7631 2e78 2073  astartes` v1.x s
-00002eb0: 686f 756c 6420 7265 7375 6c74 2069 6e20  hould result in 
-00002ec0: 7468 6520 5f65 7861 6374 5f20 7361 6d65  the _exact_ same
-00002ed0: 2073 706c 6974 732c 2061 6c77 6179 732e   splits, always.
-00002ee0: 0a54 6f20 7468 6174 2065 6e64 2c20 7468  .To that end, th
-00002ef0: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
-00002f00: 6f72 206f 6620 6061 7374 6172 7465 7360  or of `astartes`
-00002f10: 2069 7320 746f 2075 7365 2060 3432 6020   is to use `42` 
-00002f20: 6173 2074 6865 2072 616e 646f 6d20 7365  as the random se
-00002f30: 6564 2061 6e64 205f 616c 7761 7973 5f20  ed and _always_ 
-00002f40: 7365 7420 6974 2e0a 5275 6e6e 696e 6720  set it..Running 
-00002f50: 6061 7374 6172 7465 7360 2077 6974 6820  `astartes` with 
-00002f60: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
-00002f70: 696e 6773 2077 696c 6c20 616c 7761 7973  ings will always
-00002f80: 2070 726f 6475 6365 2074 6865 2065 7861   produce the exa
-00002f90: 6374 2073 616d 6520 7265 7375 6c74 732e  ct same results.
-00002fa0: 0a57 6520 6861 7665 2076 6572 6966 6965  .We have verifie
-00002fb0: 6420 7468 6973 2062 6568 6176 696f 7220  d this behavior 
-00002fc0: 6f6e 2044 6562 6961 6e20 5562 756e 7475  on Debian Ubuntu
-00002fd0: 2c20 5769 6e64 6f77 732c 2061 6e64 2049  , Windows, and I
-00002fe0: 6e74 656c 204d 6163 7320 6672 6f6d 2050  ntel Macs from P
-00002ff0: 7974 686f 6e20 7665 7273 696f 6e73 2033  ython versions 3
-00003000: 2e37 2074 6872 6f75 6768 2033 2e31 3120  .7 through 3.11 
-00003010: 2877 6974 6820 6170 7072 6f70 7269 6174  (with appropriat
-00003020: 6520 6465 7065 6e64 656e 6369 6573 2066  e dependencies f
-00003030: 6f72 2065 6163 6820 7665 7273 696f 6e29  or each version)
-00003040: 2e0a 0a23 2323 2320 4b6e 6f77 6e20 5265  ...#### Known Re
-00003050: 7072 6f64 7563 6962 696c 6974 7920 4c69  producibility Li
-00003060: 6d69 7461 7469 6f6e 730a 0a3e 202a 2a4e  mitations..> **N
-00003070: 6f74 652a 2a0a 3e20 5765 2061 7265 206c  ote**.> We are l
-00003080: 696d 6974 6564 2069 6e20 6f75 7220 6162  imited in our ab
-00003090: 696c 6974 7920 746f 2074 6573 7420 6f6e  ility to test on
-000030a0: 204d 3120 4d61 6373 2c20 6275 7420 6672   M1 Macs, but fr
-000030b0: 6f6d 206f 7572 206c 696d 6974 6564 206d  om our limited m
-000030c0: 616e 7561 6c20 7465 7374 696e 6720 7765  anual testing we
-000030d0: 2061 6368 6965 7665 2070 6572 6665 6374   achieve perfect
-000030e0: 2072 6570 726f 6475 6362 696c 6974 7920   reproducbility 
-000030f0: 696e 2061 6c6c 2063 6173 6573 205f 6578  in all cases _ex
-00003100: 6365 7074 206f 6363 6173 696f 6e61 6c6c  cept occasionall
-00003110: 795f 2077 6974 6820 604b 4d65 616e 7360  y_ with `KMeans`
-00003120: 206f 6e20 4170 706c 6520 7369 6c69 636f   on Apple silico
-00003130: 6e2e 0a49 7420 6861 7320 7072 6f64 7563  n..It has produc
-00003140: 6564 205f 736c 6967 6874 6c79 5f20 6469  ed _slightly_ di
-00003150: 6666 6572 656e 7420 7265 7375 6c74 7320  fferent results 
-00003160: 6265 7477 6565 6e20 706c 6174 666f 726d  between platform
-00003170: 7320 7265 6761 7264 6c65 7373 206f 6620  s regardless of 
-00003180: 6072 616e 646f 6d5f 7374 6174 6560 2c20  `random_state`, 
-00003190: 7769 7468 2075 7020 746f 2074 776f 2063  with up to two c
-000031a0: 6c75 7374 6572 7320 6265 696e 6720 6173  lusters being as
-000031b0: 7369 676e 6564 2064 6966 6665 7265 6e74  signed different
-000031c0: 6c79 2072 6573 756c 7469 6e67 2069 6e20  ly resulting in 
-000031d0: 6461 7461 2073 706c 6974 7320 7768 6963  data splits whic
-000031e0: 6820 6172 6520 3e39 3925 2069 6465 6e74  h are >99% ident
-000031f0: 6963 616c 2e0a 6061 7374 6172 7465 7360  ical..`astartes`
-00003200: 2069 7320 7374 696c 6c20 636f 6e73 6973   is still consis
-00003210: 7465 6e74 2062 6574 7765 656e 2072 756e  tent between run
-00003220: 7320 6f6e 2074 6865 2073 616d 6520 706c  s on the same pl
-00003230: 6174 666f 726d 2069 6e20 616c 6c20 6361  atform in all ca
-00003240: 7365 732c 2061 6e64 206f 7468 6572 2073  ses, and other s
-00003250: 616d 706c 6572 7320 6172 6520 6e6f 7420  amplers are not 
-00003260: 696d 7061 6374 6564 2062 7920 7468 6973  impacted by this
-00003270: 2061 7070 6172 656e 7420 6275 672e 0a0a   apparent bug...
-00003280: 202d 2060 736b 6c65 6172 6e60 2076 312e   - `sklearn` v1.
-00003290: 332e 3020 696e 7472 6f64 7563 6564 2062  3.0 introduced b
-000032a0: 6163 6b77 6172 6473 2d69 6e63 6f6d 7061  ackwards-incompa
-000032b0: 7469 626c 6520 6368 616e 6765 7320 696e  tible changes in
-000032c0: 2074 6865 2060 4b4d 6561 6e73 6020 7361   the `KMeans` sa
-000032d0: 6d70 6c65 7220 7468 6174 2063 6861 6e67  mpler that chang
-000032e0: 6564 2068 6f77 2074 6865 2072 616e 646f  ed how the rando
-000032f0: 6d20 696e 6974 6961 6c69 7a61 7469 6f6e  m initialization
-00003300: 2061 6666 6563 7473 2074 6865 2072 6573   affects the res
-00003310: 756c 7473 2c20 6576 656e 2067 6976 656e  ults, even given
-00003320: 2074 6865 2073 616d 6520 7261 6e64 6f6d   the same random
-00003330: 2073 6565 642e 2044 6966 6665 7265 6e74   seed. Different
-00003340: 2076 6572 7369 6f6e 206f 6620 6073 6b6c   version of `skl
-00003350: 6561 726e 6020 7769 6c6c 2061 6666 6563  earn` will affec
-00003360: 7420 7468 6520 7065 7266 6f72 6d61 6e63  t the performanc
-00003370: 6520 6f66 2060 6173 7461 7274 6573 6020  e of `astartes` 
-00003380: 616e 6420 7765 2072 6563 6f6d 6d65 6e64  and we recommend
-00003390: 2069 6e63 6c75 6469 6e67 2074 6865 2065   including the e
-000033a0: 7861 6374 2076 6572 7369 6f6e 206f 6620  xact version of 
-000033b0: 6073 6369 6b69 742d 6c65 6172 6e60 2061  `scikit-learn` a
-000033c0: 6e64 2060 6173 7461 7274 6573 6020 7573  nd `astartes` us
-000033d0: 6564 2c20 7768 656e 2061 7070 6c69 6361  ed, when applica
-000033e0: 626c 652e 0a0a 2323 2045 7661 6c75 6174  ble...## Evaluat
-000033f0: 6520 7468 6520 496d 7061 6374 206f 6620  e the Impact of 
-00003400: 5370 6c69 7474 696e 6720 416c 676f 7269  Splitting Algori
-00003410: 7468 6d73 0a54 6865 2060 6765 6e65 7261  thms.The `genera
-00003420: 7465 5f72 6567 7265 7373 696f 6e5f 7265  te_regression_re
-00003430: 7375 6c74 735f 6469 6374 6020 6675 6e63  sults_dict` func
-00003440: 7469 6f6e 2061 6c6c 6f77 7320 7573 6572  tion allows user
-00003450: 7320 746f 2071 7569 636b 6c79 2065 7661  s to quickly eva
-00003460: 6c75 6174 6520 7468 6520 696d 7061 6374  luate the impact
-00003470: 206f 6620 6469 6666 6572 656e 7420 7370   of different sp
-00003480: 6c69 7474 696e 6720 7465 6368 6e69 7175  litting techniqu
-00003490: 6573 206f 6e20 616e 7920 6d6f 6465 6c20  es on any model 
-000034a0: 7375 7070 6f72 7465 6420 6279 2060 736b  supported by `sk
-000034b0: 6c65 6172 6e60 2e20 416c 6c20 7265 7375  learn`. All resu
-000034c0: 6c74 7320 6172 6520 7374 6f72 6564 2069  lts are stored i
-000034d0: 6e20 6120 6469 6374 696f 6e61 7279 2066  n a dictionary f
-000034e0: 6f72 6d61 7420 616e 6420 6361 6e20 6265  ormat and can be
-000034f0: 2064 6973 706c 6179 6564 2069 6e20 6120   displayed in a 
-00003500: 6e65 6174 6c79 2066 6f72 6d61 7474 6564  neatly formatted
-00003510: 2074 6162 6c65 2075 7369 6e67 2074 6865   table using the
-00003520: 206f 7074 696f 6e61 6c20 6070 7269 6e74   optional `print
-00003530: 5f72 6573 756c 7473 6020 6172 6775 6d65  _results` argume
-00003540: 6e74 2e0a 0a60 6060 0a66 726f 6d20 736b  nt...```.from sk
-00003550: 6c65 6172 6e2e 7376 6d20 696d 706f 7274  learn.svm import
-00003560: 204c 696e 6561 7253 5652 0a0a 6672 6f6d   LinearSVR..from
-00003570: 2061 7374 6172 7465 732e 7574 696c 7320   astartes.utils 
-00003580: 696d 706f 7274 2067 656e 6572 6174 655f  import generate_
-00003590: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
-000035a0: 7473 5f64 6963 740a 0a73 6b6c 6561 726e  ts_dict..sklearn
-000035b0: 5f6d 6f64 656c 203d 204c 696e 6561 7253  _model = LinearS
-000035c0: 5652 2829 0a72 6573 756c 7473 5f64 6963  VR().results_dic
-000035d0: 7420 3d20 6765 6e65 7261 7465 5f72 6567  t = generate_reg
-000035e0: 7265 7373 696f 6e5f 7265 7375 6c74 735f  ression_results_
-000035f0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00003600: 2020 2020 2020 2020 2020 736b 6c65 6172            sklear
-00003610: 6e5f 6d6f 6465 6c2c 0a20 2020 2020 2020  n_model,.       
-00003620: 2020 2020 2020 2020 2020 2020 2058 2c0a               X,.
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 792c 0a20 2020 2020 2020 2020      y,.         
-00003650: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003660: 5f72 6573 756c 7473 3d54 7275 652c 0a20  _results=True,. 
-00003670: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00003680: 0a20 2020 2020 2020 2020 5472 6169 6e20  .         Train 
-00003690: 2020 2020 2020 5661 6c20 2020 2020 2054        Val      T
-000036a0: 6573 740a 2d2d 2d2d 2020 2d2d 2d2d 2d2d  est.----  ------
-000036b0: 2d2d 2020 2d2d 2d2d 2d2d 2d2d 2020 2d2d  --  --------  --
-000036c0: 2d2d 2d2d 2d2d 0a4d 4145 2020 2031 2e34  ------.MAE   1.4
-000036d0: 3135 3232 2020 2033 2e31 3334 3335 2020  1522   3.13435  
-000036e0: 2032 2e31 3730 3931 0a52 4d53 4520 2032   2.17091.RMSE  2
-000036f0: 2e30 3330 3632 2020 2033 2e37 3337 3231  .03062   3.73721
-00003700: 2020 2032 2e34 3030 3431 0a52 3220 2020     2.40041.R2   
-00003710: 2030 2e39 3037 3435 2020 2030 2e38 3037   0.90745   0.807
-00003720: 3837 2020 2030 2e37 3834 3132 0a0a 6060  87   0.78412..``
-00003730: 600a 0a23 2320 4f6e 6c69 6e65 2044 6f63  `..## Online Doc
-00003740: 756d 656e 7461 7469 6f6e 0a5b 5468 6520  umentation.[The 
-00003750: 6f6e 6c69 6e65 2064 6f63 756d 656e 7461  online documenta
-00003760: 7469 6f6e 5d28 6874 7470 733a 2f2f 4a61  tion](https://Ja
-00003770: 636b 736f 6e42 7572 6e73 2e67 6974 6875  cksonBurns.githu
-00003780: 622e 696f 2f61 7374 6172 7465 732f 2920  b.io/astartes/) 
-00003790: 636f 6e74 6169 6e73 2065 7665 7279 7468  contains everyth
-000037a0: 696e 6720 796f 7520 7365 6520 696e 2074  ing you see in t
-000037b0: 6869 7320 5245 4144 4d45 2077 6974 6820  his README with 
-000037c0: 616e 2061 6464 6974 696f 6e61 6c20 7475  an additional tu
-000037d0: 746f 7269 616c 2066 6f72 205b 6d6f 7669  torial for [movi
-000037e0: 6e67 2066 726f 6d20 6074 7261 696e 5f74  ng from `train_t
-000037f0: 6573 745f 7370 6c69 7460 2069 6e20 6073  est_split` in `s
-00003800: 6b6c 6561 726e 6020 746f 2060 6173 7461  klearn` to `asta
-00003810: 7274 6573 605d 2868 7474 7073 3a2f 2f6a  rtes`](https://j
-00003820: 6163 6b73 6f6e 6275 726e 732e 6769 7468  acksonburns.gith
-00003830: 7562 2e69 6f2f 6173 7461 7274 6573 2f73  ub.io/astartes/s
-00003840: 6b6c 6561 726e 5f74 6f5f 6173 7461 7274  klearn_to_astart
-00003850: 6573 2e68 746d 6c29 2e0a 0a23 2320 486f  es.html)...## Ho
-00003860: 7720 746f 2043 6974 650a 4966 2079 6f75  w to Cite.If you
-00003870: 2075 7365 2060 6173 7461 7274 6573 6020   use `astartes` 
-00003880: 696e 2079 6f75 7220 776f 726b 2070 6c65  in your work ple
-00003890: 6173 6520 7573 6520 7468 6520 6265 6c6f  ase use the belo
-000038a0: 7720 6369 7461 7469 6f6e 206f 7220 7468  w citation or th
-000038b0: 6520 2243 6974 6520 7468 6973 2072 6570  e "Cite this rep
-000038c0: 6f73 6974 6f72 7922 2062 7574 746f 6e20  ository" button 
-000038d0: 6f6e 2047 6974 4875 623a 0a3e 202a 2a42  on GitHub:.> **B
-000038e0: 6962 5465 582a 2a0a 3e20 4073 6f66 7477  ibTeX**.> @softw
-000038f0: 6172 657b 4275 726e 735f 6173 7461 7274  are{Burns_astart
-00003900: 6573 2c0a 3e20 2020 6175 7468 6f72 203d  es,.>   author =
-00003910: 207b 4275 726e 732c 204a 6163 6b73 6f6e   {Burns, Jackson
-00003920: 2061 6e64 2053 7069 656b 6572 6d61 6e6e   and Spiekermann
-00003930: 2c20 4b65 7669 6e20 616e 6420 4268 6174  , Kevin and Bhat
-00003940: 7461 6368 6172 6a65 652c 2048 696d 6167  tacharjee, Himag
-00003950: 686e 6120 616e 6420 566c 6163 686f 732c  hna and Vlachos,
-00003960: 2044 696f 6e69 7369 6f73 2061 6e64 2047   Dionisios and G
-00003970: 7265 656e 2c20 5769 6c6c 6961 6d7d 2c0a  reen, William},.
-00003980: 3e20 2020 6c69 6365 6e73 6520 3d20 7b4d  >   license = {M
-00003990: 4954 7d2c 0a3e 2020 2074 6974 6c65 203d  IT},.>   title =
-000039a0: 207b 7b61 7374 6172 7465 737d 7d2c 0a3e   {{astartes}},.>
-000039b0: 2020 2075 726c 203d 207b 6874 7470 733a     url = {https:
-000039c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4a 6163  //github.com/Jac
-000039d0: 6b73 6f6e 4275 726e 732f 6173 7461 7274  ksonBurns/astart
-000039e0: 6573 7d0a 3e20 7d0a 0a3e 202a 2a41 5041  es}.> }..> **APA
-000039f0: 2a2a 0a3e 2042 7572 6e73 2c20 4a2e 2c20  **.> Burns, J., 
-00003a00: 5370 6965 6b65 726d 616e 6e2c 204b 2e2c  Spiekermann, K.,
-00003a10: 2042 6861 7474 6163 6861 726a 6565 2c20   Bhattacharjee, 
-00003a20: 482e 2c20 566c 6163 686f 732c 2044 2e2c  H., Vlachos, D.,
-00003a30: 2026 2047 7265 656e 2c20 572e 2061 7374   & Green, W. ast
-00003a40: 6172 7465 7320 5b43 6f6d 7075 7465 7220  artes [Computer 
-00003a50: 736f 6674 7761 7265 5d2e 2068 7474 7073  software]. https
-00003a60: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00003a70: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-00003a80: 7465 730a 0a0a 2323 2043 6f6e 7472 6962  tes...## Contrib
-00003a90: 7574 696e 6720 2620 4465 7665 6c6f 7065  uting & Develope
-00003aa0: 7220 4e6f 7465 730a 5075 6c6c 2052 6571  r Notes.Pull Req
-00003ab0: 7565 7374 732c 2042 7567 2052 6570 6f72  uests, Bug Repor
-00003ac0: 7473 2c20 616e 6420 616c 6c20 436f 6e74  ts, and all Cont
-00003ad0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
-00003ae0: 6c63 6f6d 6521 2050 6c65 6173 6520 7573  lcome! Please us
-00003af0: 6520 7468 6520 6170 7072 6f70 7269 6174  e the appropriat
-00003b00: 6520 6973 7375 6520 6f72 2070 756c 6c20  e issue or pull 
-00003b10: 7265 7175 6573 7420 7465 6d70 6c61 7465  request template
-00003b20: 2077 6865 6e20 6d61 6b69 6e67 2061 2063   when making a c
-00003b30: 6f6e 7472 6962 7574 696f 6e2e 0a0a 5765  ontribution...We
-00003b40: 206d 616b 6520 7573 6520 6f66 205b 7468   make use of [th
-00003b50: 6520 4769 7448 7562 2044 6973 6375 7373  e GitHub Discuss
-00003b60: 696f 6e73 2070 6167 655d 2868 7474 7073  ions page](https
-00003b70: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
-00003b80: 636b 736f 6e42 7572 6e73 2f61 7374 6172  cksonBurns/astar
-00003b90: 7465 732f 6469 7363 7573 7369 6f6e 7329  tes/discussions)
-00003ba0: 2074 6f20 676f 206f 7665 7220 706f 7465   to go over pote
-00003bb0: 6e74 6961 6c20 6665 6174 7572 6573 2074  ntial features t
-00003bc0: 6f20 6164 642e 2050 6c65 6173 6520 6665  o add. Please fe
-00003bd0: 656c 2066 7265 6520 746f 2073 746f 7020  el free to stop 
-00003be0: 6279 2069 6620 796f 7520 6172 6520 6c6f  by if you are lo
-00003bf0: 6f6b 696e 6720 666f 7220 736f 6d65 7468  oking for someth
-00003c00: 696e 6720 746f 2064 6576 656c 6f70 206f  ing to develop o
-00003c10: 7220 6861 7665 2061 6e20 6964 6561 2066  r have an idea f
-00003c20: 6f72 2061 2075 7365 6675 6c20 6665 6174  or a useful feat
-00003c30: 7572 6521 0a0a 5768 656e 2073 7562 6d69  ure!..When submi
-00003c40: 7474 696e 6720 6120 5052 2c20 706c 6561  tting a PR, plea
-00003c50: 7365 206d 6172 6b20 796f 7572 2050 5220  se mark your PR 
-00003c60: 7769 7468 2074 6865 2022 5052 2052 6561  with the "PR Rea
-00003c70: 6479 2066 6f72 2052 6576 6965 7722 206c  dy for Review" l
-00003c80: 6162 656c 2077 6865 6e20 796f 7520 6172  abel when you ar
-00003c90: 6520 6669 6e69 7368 6564 206d 616b 696e  e finished makin
-00003ca0: 6720 6368 616e 6765 7320 736f 2074 6861  g changes so tha
-00003cb0: 7420 7468 6520 4769 7448 7562 2061 6374  t the GitHub act
-00003cc0: 696f 6e73 2062 6f74 7320 6361 6e20 776f  ions bots can wo
-00003cd0: 726b 2074 6865 6972 206d 6167 6963 210a  rk their magic!.
-00003ce0: 0a23 2323 2044 6576 656c 6f70 6572 2049  .### Developer I
-00003cf0: 6e73 7461 6c6c 0a0a 546f 2063 6f6e 7472  nstall..To contr
-00003d00: 6962 7574 6520 746f 2074 6865 2060 6173  ibute to the `as
-00003d10: 7461 7274 6573 6020 736f 7572 6365 2063  tartes` source c
-00003d20: 6f64 652c 2073 7461 7274 2062 7920 636c  ode, start by cl
-00003d30: 6f6e 696e 6720 7468 6520 7265 706f 7369  oning the reposi
-00003d40: 746f 7279 2028 692e 652e 2060 6769 7420  tory (i.e. `git 
-00003d50: 636c 6f6e 6520 6769 7440 6769 7468 7562  clone git@github
-00003d60: 2e63 6f6d 3a4a 6163 6b73 6f6e 4275 726e  .com:JacksonBurn
-00003d70: 732f 6173 7461 7274 6573 2e67 6974 6029  s/astartes.git`)
-00003d80: 2061 6e64 2074 6865 6e20 696e 7369 6465   and then inside
-00003d90: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00003da0: 7275 6e20 6070 6970 2069 6e73 7461 6c6c  run `pip install
-00003db0: 202d 6520 2e5b 6d6f 6c65 6375 6c65 732c   -e .[molecules,
-00003dc0: 6465 765d 602e 2054 6869 7320 7769 6c6c  dev]`. This will
-00003dd0: 2073 6574 2079 6f75 2075 7020 7769 7468   set you up with
-00003de0: 2061 6c6c 2074 6865 2072 6571 7569 7265   all the require
-00003df0: 6420 6465 7065 6e64 656e 6369 6573 2074  d dependencies t
-00003e00: 6f20 7275 6e20 6061 7374 6172 7465 7360  o run `astartes`
-00003e10: 2061 6e64 2063 6f6e 666f 726d 2074 6f20   and conform to 
-00003e20: 6f75 7220 666f 726d 6174 7469 6e67 2073  our formatting s
-00003e30: 7461 6e64 6172 6473 2028 6062 6c61 636b  tandards (`black
-00003e40: 6020 616e 6420 6069 736f 7274 6029 2c20  ` and `isort`), 
-00003e50: 7768 6963 6820 796f 7520 6361 6e20 636f  which you can co
-00003e60: 6e66 6967 7572 6520 746f 2072 756e 2061  nfigure to run a
-00003e70: 7574 6f6d 6174 6963 616c 6c79 2069 6e20  utomatically in 
-00003e80: 7673 636f 6465 205b 6c69 6b65 2074 6869  vscode [like thi
-00003e90: 735d 2868 7474 7073 3a2f 2f6d 6172 636f  s](https://marco
-00003ea0: 6265 6c6f 2e6d 6564 6975 6d2e 636f 6d2f  belo.medium.com/
-00003eb0: 7365 7474 696e 672d 7570 2d70 7974 686f  setting-up-pytho
-00003ec0: 6e2d 626c 6163 6b2d 6f6e 2d76 6973 7561  n-black-on-visua
-00003ed0: 6c2d 7374 7564 696f 2d63 6f64 652d 3533  l-studio-code-53
-00003ee0: 3138 6562 6134 6364 3030 233a 7e3a 7465  18eba4cd00#:~:te
-00003ef0: 7874 3d47 6f25 3230 746f 2532 3073 6574  xt=Go%20to%20set
-00003f00: 7469 6e67 7325 3230 696e 2532 3079 6f75  tings%20in%20you
-00003f10: 722c 2545 3225 3830 2539 4425 3230 616e  r,%E2%80%9D%20an
-00003f20: 6425 3230 7365 6c65 6374 2532 3025 4532  d%20select%20%E2
-00003f30: 2538 3025 3943 626c 6163 6b25 4532 2538  %80%9Cblack%E2%8
-00003f40: 3025 3944 2e29 2e0a 0a3e 202a 2a4e 6f74  0%9D.)...> **Not
-00003f50: 652a 2a0a 3e20 5769 6e64 6f77 7320 506f  e**.> Windows Po
-00003f60: 7765 7273 6865 6c6c 2061 6e64 204d 6163  wershell and Mac
-00003f70: 4f53 2043 6174 616c 696e 6120 6f72 206e  OS Catalina or n
-00003f80: 6577 6572 206d 6179 2063 6f6d 706c 6169  ewer may complai
-00003f90: 6e20 6162 6f75 7420 7371 7561 7265 2062  n about square b
-00003fa0: 7261 636b 6574 732c 2073 6f20 796f 7520  rackets, so you 
-00003fb0: 7769 6c6c 206e 6565 6420 746f 2064 6f75  will need to dou
-00003fc0: 626c 6520 7175 6f74 6520 7468 6520 606d  ble quote the `m
-00003fd0: 6f6c 6563 756c 6573 6020 636f 6d6d 616e  olecules` comman
-00003fe0: 6420 2869 2e65 2e20 6070 6970 2069 6e73  d (i.e. `pip ins
-00003ff0: 7461 6c6c 2022 6173 7461 7274 6573 5b6d  tall "astartes[m
-00004000: 6f6c 6563 756c 6573 2c64 6576 5d22 6029  olecules,dev]"`)
-00004010: 0a0a 2323 2320 556e 6974 2054 6573 7469  ..### Unit Testi
-00004020: 6e67 0a41 6c6c 206f 6620 7468 6520 7465  ng.All of the te
-00004030: 7374 7320 696e 2060 6173 7461 7274 6573  sts in `astartes
-00004040: 6020 6172 6520 7772 6974 7465 6e20 7573  ` are written us
-00004050: 696e 6720 7468 6520 6275 696c 742d 696e  ing the built-in
-00004060: 2070 7974 686f 6e20 6075 6e69 7474 6573   python `unittes
-00004070: 7460 206d 6f64 756c 6520 2874 6f20 616c  t` module (to al
-00004080: 6c6f 7720 7275 6e6e 696e 6720 7769 7468  low running with
-00004090: 6f75 7420 6070 7974 6573 7460 2920 6275  out `pytest`) bu
-000040a0: 7420 7765 205f 6869 6768 6c79 5f20 7265  t we _highly_ re
-000040b0: 636f 6d6d 656e 6420 7573 696e 6720 6070  commend using `p
-000040c0: 7974 6573 7460 2e20 546f 2065 7865 6375  ytest`. To execu
-000040d0: 7465 2074 6865 2074 6573 7473 2066 726f  te the tests fro
-000040e0: 6d20 7468 6520 6061 7374 6172 7465 7360  m the `astartes`
-000040f0: 2072 6570 6f73 6974 6f72 792c 2073 696d   repository, sim
-00004100: 706c 7920 7479 7065 2060 7079 7465 7374  ply type `pytest
-00004110: 6020 6166 7465 7220 7275 6e6e 696e 6720  ` after running 
-00004120: 7468 6520 6465 7665 6c6f 7065 7220 696e  the developer in
-00004130: 7374 616c 6c20 286f 7220 616c 7465 726e  stall (or altern
-00004140: 6174 656c 792c 2060 7079 7465 7374 202d  ately, `pytest -
-00004150: 7660 2066 6f72 2061 206d 6f72 6520 6865  v` for a more he
-00004160: 6c70 6675 6c20 6f75 7470 7574 292e 0a0a  lpful output)...
-00004170: 2323 2320 4164 6469 6e67 204e 6577 2053  ### Adding New S
-00004180: 616d 706c 6572 730a 4164 6469 6e67 2061  amplers.Adding a
-00004190: 206e 6577 2073 616d 706c 6572 2073 686f   new sampler sho
-000041a0: 756c 6420 6578 7465 6e64 2074 6865 2060  uld extend the `
-000041b0: 6162 7374 7261 6374 5f73 616d 706c 6572  abstract_sampler
-000041c0: 2e70 7960 2061 6273 7472 6163 7420 6261  .py` abstract ba
-000041d0: 7365 2063 6c61 7373 2e0a 0a49 7420 6361  se class...It ca
-000041e0: 6e20 6265 2061 7320 7369 6d70 6c65 2061  n be as simple a
-000041f0: 7320 6120 7061 7373 7468 726f 7567 6820  s a passthrough 
-00004200: 746f 2061 2061 6e6f 7468 6572 2060 7472  to a another `tr
-00004210: 6169 6e5f 7465 7374 5f73 706c 6974 602c  ain_test_split`,
-00004220: 206f 7220 6974 2063 616e 2062 6520 616e   or it can be an
-00004230: 206f 7269 6769 6e61 6c20 696d 706c 656d   original implem
-00004240: 656e 7461 7469 6f6e 2074 6861 7420 7265  entation that re
-00004250: 7375 6c74 7320 696e 2058 2061 6e64 2079  sults in X and y
-00004260: 2062 6569 6e67 2073 706c 6974 2069 6e74   being split int
-00004270: 6f20 7477 6f20 6c69 7374 732e 2054 616b  o two lists. Tak
-00004280: 6520 6120 6c6f 6f6b 2061 7420 6061 7374  e a look at `ast
-00004290: 6172 7465 732f 7361 6d70 6c65 7273 2f72  artes/samplers/r
-000042a0: 616e 646f 6d5f 7370 6c69 742e 7079 6020  andom_split.py` 
-000042b0: 666f 7220 6120 6261 7369 6320 6578 616d  for a basic exam
-000042c0: 706c 6521 0a0a 4166 7465 7220 7468 6520  ple!..After the 
-000042d0: 7361 6d70 6c65 7220 6861 7320 6265 656e  sampler has been
-000042e0: 2069 6d70 6c65 6d65 6e74 6564 2c20 6164   implemented, ad
-000042f0: 6420 6974 2074 6f20 605f 5f69 6e69 745f  d it to `__init_
-00004300: 5f2e 7079 6020 696e 2069 6e20 6061 7374  _.py` in in `ast
-00004310: 6172 7465 732f 7361 6d70 6c65 7273 6020  artes/samplers` 
-00004320: 616e 6420 6974 2077 696c 6c20 6175 746f  and it will auto
-00004330: 6d61 7469 6361 6c6c 7920 6265 2075 6e69  matically be uni
-00004340: 7420 7465 7374 6564 2e20 4164 6469 7469  t tested. Additi
-00004350: 6f6e 616c 2075 6e69 7420 7465 7374 7320  onal unit tests 
-00004360: 746f 2076 6572 6966 7920 7468 6174 2068  to verify that h
-00004370: 7970 6572 7061 7261 6d65 7465 7273 2063  yperparameters c
-00004380: 616e 2062 6520 7072 6f70 6572 6c79 2070  an be properly p
-00004390: 6173 7365 642c 2065 7463 2e20 6172 6520  assed, etc. are 
-000043a0: 616c 736f 2072 6563 6f6d 6d65 6e64 6564  also recommended
-000043b0: 2e0a 0a46 6f72 2068 6973 746f 7269 6361  ...For historica
-000043c0: 6c20 7265 6173 6f6e 732c 2061 6e64 2061  l reasons, and a
-000043d0: 7320 6120 6775 6964 6520 666f 7220 616e  s a guide for an
-000043e0: 7920 6465 7665 6c6f 7065 7273 2077 686f  y developers who
-000043f0: 2077 6f75 6c64 206c 696b 6520 6164 6420   would like add 
-00004400: 6e65 7720 7361 6d70 6c65 7273 2c20 6265  new samplers, be
-00004410: 6c6f 7720 6973 2061 2072 756e 6e69 6e67  low is a running
-00004420: 206c 6973 7420 6f66 2073 616d 706c 6572   list of sampler
-00004430: 7320 7768 6963 6820 6861 7665 2062 6565  s which have bee
-00004440: 6e20 5f63 6f6e 7369 6465 7265 645f 2066  n _considered_ f
-00004450: 6f72 2061 6464 6974 696f 6e20 746f 2060  or addition to `
-00004460: 6173 6172 7465 7360 2062 7574 2075 6c74  asartes` but ult
-00004470: 696d 6174 656c 7920 6e6f 7420 6164 6465  imately not adde
-00004480: 6420 666f 7220 7661 7269 6f75 7320 7265  d for various re
-00004490: 6173 6f6e 732e 0a0a 2323 2323 204e 6f74  asons...#### Not
-000044a0: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
-000044b0: 706c 696e 6720 416c 676f 7269 7468 6d73  pling Algorithms
-000044c0: 0a0a 7c20 5361 6d70 6c65 7220 4e61 6d65  ..| Sampler Name
-000044d0: 207c 2052 6561 736f 6e69 6e67 207c 2052   | Reasoning | R
-000044e0: 656c 6576 616e 7420 4c69 6e6b 2873 2920  elevant Link(s) 
-000044f0: 7c0a 7c3a 2d2d 2d3a 7c2d 2d2d 7c2d 2d2d  |.|:---:|---|---
-00004500: 7c0a 7c20 442d 4f70 7469 6d61 6c20 7c20  |.| D-Optimal | 
-00004510: 5265 7175 6972 6573 205f 612d 7072 696f  Requires _a-prio
-00004520: 7269 5f20 6b6e 6f77 6c65 6467 6520 6f66  ri_ knowledge of
-00004530: 2074 6865 2074 6573 7420 616e 6420 7472   the test and tr
-00004540: 6169 6e20 7369 7a65 2077 6869 6368 2064  ain size which d
-00004550: 6f65 7320 6e6f 7420 6669 7420 696e 2074  oes not fit in t
-00004560: 6865 2060 6173 7461 7274 6573 6020 6672  he `astartes` fr
-00004570: 616d 6577 6f72 6b20 2873 616d 706c 6572  amework (sampler
-00004580: 7320 6172 6520 616c 6c20 6167 6e6f 7374  s are all agnost
-00004590: 6963 2074 6f20 7468 6520 7369 7a65 206f  ic to the size o
-000045a0: 6620 7468 6520 7365 7473 2920 616e 6420  f the sets) and 
-000045b0: 6974 2069 7320 7175 6573 7469 6f6e 6162  it is questionab
-000045c0: 6c65 2069 6620 7468 6520 7573 6520 6f66  le if the use of
-000045d0: 2074 6865 2046 6973 6368 6572 2069 6e66   the Fischer inf
-000045e0: 6f72 6d61 7469 6f6e 206d 6174 7269 7820  ormation matrix 
-000045f0: 6973 2061 6374 7561 6c6c 7920 6d65 616e  is actually mean
-00004600: 696e 6766 756c 2069 6e20 7468 6520 636f  ingful in the co
-00004610: 6e74 6578 7420 6f66 2073 616d 706c 696e  ntext of samplin
-00004620: 6720 6578 6973 7469 6e67 2064 6174 6120  g existing data 
-00004630: 7261 7468 6572 2074 6861 6e20 7475 6e69  rather than tuni
-00004640: 6e67 2066 6f72 2069 6465 616c 2064 6174  ng for ideal dat
-00004650: 612e 207c 2054 6865 205b 5769 6b69 7065  a. | The [Wikipe
-00004660: 6469 6120 6172 7469 636c 6520 666f 7220  dia article for 
-00004670: 6f70 7469 6d61 6c20 6465 7369 676e 5d28  optimal design](
-00004680: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00004690: 6564 6961 2e6f 7267 2f77 696b 692f 4f70  edia.org/wiki/Op
-000046a0: 7469 6d61 6c5f 6465 7369 676e 233a 7e3a  timal_design#:~:
-000046b0: 7465 7874 3d4f 6625 3230 636f 7572 7365  text=Of%20course
-000046c0: 2532 4325 3230 6669 7869 6e67 2532 3074  %2C%20fixing%20t
-000046d0: 6865 2532 306e 756d 6265 7225 3230 6f66  he%20number%20of
-000046e0: 2532 3065 7870 6572 696d 656e 7461 6c25  %20experimental%
-000046f0: 3230 7275 6e73 2532 3061 2532 3070 7269  20runs%20a%20pri
-00004700: 6f72 6925 3230 776f 756c 6425 3230 6265  ori%20would%20be
-00004710: 2532 3069 6d70 7261 6374 6963 616c 2e29  %20impractical.)
-00004720: 2064 6f65 7320 6120 676f 6f64 206a 6f62   does a good job
-00004730: 2065 7870 6c61 696e 696e 6720 7768 7920   explaining why 
-00004740: 7468 6973 2069 7320 6469 6666 6963 756c  this is difficul
-00004750: 742c 2061 6e64 2070 6f69 6e74 7320 6174  t, and points at
-00004760: 2073 6f6d 6520 706f 7465 6e74 6961 6c20   some potential 
-00004770: 616c 7465 726e 6174 6976 6573 2e20 7c0a  alternatives. |.
-00004780: 7c20 4475 706c 6578 207c 2052 6571 7569  | Duplex | Requi
-00004790: 7265 7320 6b6e 6f77 696e 6720 7465 7374  res knowing test
-000047a0: 2061 6e64 2074 7261 696e 2073 697a 6520   and train size 
-000047b0: 6265 666f 7265 2065 7865 6375 7469 6f6e  before execution
-000047c0: 2c20 616e 6420 6361 6e20 6f6e 6c79 2070  , and can only p
-000047d0: 6172 7469 7469 6f6e 2064 6174 6120 696e  artition data in
-000047e0: 746f 2074 776f 2073 6574 7320 7768 6963  to two sets whic
-000047f0: 6820 776f 756c 6420 6d61 6b65 2069 7420  h would make it 
-00004800: 696e 636f 6d70 6174 6962 6c65 2077 6974  incompatible wit
-00004810: 6820 6074 7261 696e 5f76 616c 5f74 6573  h `train_val_tes
-00004820: 745f 7370 6c69 7460 2e20 7c20 5468 6973  t_split`. | This
-00004830: 205b 696d 706c 656d 656e 7461 7469 6f6e   [implementation
-00004840: 2069 6e20 525d 2868 7474 7073 3a2f 2f73   in R](https://s
-00004850: 6561 7263 682e 722d 7072 6f6a 6563 742e  earch.r-project.
-00004860: 6f72 672f 4352 414e 2f72 6566 6d61 6e73  org/CRAN/refmans
-00004870: 2f70 726f 7370 6563 7472 2f68 746d 6c2f  /prospectr/html/
-00004880: 6475 706c 6578 2e68 746d 6c23 3a7e 3a74  duplex.html#:~:t
-00004890: 6578 743d 5468 6525 3230 4455 504c 4558  ext=The%20DUPLEX
-000048a0: 2532 3061 6c67 6f72 6974 686d 2532 3069  %20algorithm%20i
-000048b0: 7325 3230 7369 6d69 6c61 722c 7468 6174  s%20similar,that
-000048c0: 2532 3061 7265 2532 3074 6865 2532 3066  %20are%20the%20f
-000048d0: 6172 7468 6573 7425 3230 6170 6172 742e  arthest%20apart.
-000048e0: 2920 696e 636c 7564 6573 2068 656c 7066  ) includes helpf
-000048f0: 756c 2072 6566 6572 656e 6365 7320 616e  ul references an
-00004900: 6420 6120 7265 6665 7265 6e63 6520 696d  d a reference im
-00004910: 706c 656d 656e 7461 7469 6f6e 2e20 7c0a  plementation. |.
-00004920: 0a23 2323 2041 6464 696e 6720 4e65 7720  .### Adding New 
-00004930: 4665 6174 7572 697a 6174 696f 6e20 5363  Featurization Sc
-00004940: 6865 6d65 730a 416c 6c20 6f66 2074 6865  hemes.All of the
-00004950: 2073 616d 706c 696e 6720 6d65 7468 6f64   sampling method
-00004960: 7320 696d 706c 656d 656e 7465 6420 696e  s implemented in
-00004970: 2060 6173 7461 7274 6573 6020 6163 6365   `astartes` acce
-00004980: 7074 2061 7262 6974 7261 7279 2061 7272  pt arbitrary arr
-00004990: 6179 7320 6f66 206e 756d 6265 7273 2061  ays of numbers a
-000049a0: 6e64 2072 6574 7572 6e20 7468 6520 7361  nd return the sa
-000049b0: 6d70 6c65 6420 6772 6f75 7073 2028 7769  mpled groups (wi
-000049c0: 7468 2074 6865 2065 7863 6570 7469 6f6e  th the exception
-000049d0: 206f 6620 6053 6361 6666 6f6c 642e 7079   of `Scaffold.py
-000049e0: 6029 2e20 4966 2079 6f75 2068 6176 6520  `). If you have 
-000049f0: 616e 2065 7869 7374 696e 6720 6665 6174  an existing feat
-00004a00: 7572 697a 6174 696f 6e20 7363 6865 6d65  urization scheme
-00004a10: 2028 692e 652e 2074 616b 6520 616e 2061   (i.e. take an a
-00004a20: 7262 6974 7261 7279 2069 6e70 7574 2061  rbitrary input a
-00004a30: 6e64 2074 7572 6e20 6974 2069 6e74 6f20  nd turn it into 
-00004a40: 616e 2061 7272 6179 206f 6620 6e75 6d62  an array of numb
-00004a50: 6572 7329 2c20 7765 2077 6f75 6c64 2062  ers), we would b
-00004a60: 6520 7468 7269 6c6c 6564 2074 6f20 696e  e thrilled to in
-00004a70: 636c 7564 6520 6974 2069 6e20 6061 7374  clude it in `ast
-00004a80: 6172 7465 7360 2e0a 0a41 6464 696e 6720  artes`...Adding 
-00004a90: 6120 6e65 7720 696e 7465 7266 6163 6520  a new interface 
-00004aa0: 7368 6f75 6c64 2074 616b 6520 6f6e 2074  should take on t
-00004ab0: 6869 7320 666f 726d 6174 3a0a 0a60 6060  his format:..```
-00004ac0: 7079 7468 6f6e 0a66 726f 6d20 6173 7461  python.from asta
-00004ad0: 7274 6573 2069 6d70 6f72 7420 7472 6169  rtes import trai
-00004ae0: 6e5f 7465 7374 5f73 706c 6974 0a0a 6465  n_test_split..de
-00004af0: 6620 7472 6169 6e5f 7465 7374 5f73 706c  f train_test_spl
-00004b00: 6974 5f49 4e54 4552 4641 4345 280a 2020  it_INTERFACE(.  
-00004b10: 2020 494e 5445 5246 4143 455f 696e 7075    INTERFACE_inpu
-00004b20: 742c 0a20 2020 2049 4e54 4552 4641 4345  t,.    INTERFACE
-00004b30: 5f41 5247 532c 0a20 2020 2079 3a20 6e70  _ARGS,.    y: np
-00004b40: 2e61 7272 6179 203d 204e 6f6e 652c 0a20  .array = None,. 
-00004b50: 2020 206c 6162 656c 733a 206e 702e 6172     labels: np.ar
-00004b60: 7261 7920 3d20 4e6f 6e65 2c0a 2020 2020  ray = None,.    
-00004b70: 7465 7374 5f73 697a 653a 2066 6c6f 6174  test_size: float
-00004b80: 203d 2030 2e32 352c 0a20 2020 2074 7261   = 0.25,.    tra
-00004b90: 696e 5f73 697a 653a 2066 6c6f 6174 203d  in_size: float =
-00004ba0: 2030 2e37 352c 0a20 2020 2073 706c 6974   0.75,.    split
-00004bb0: 7465 723a 2073 7472 203d 2027 7261 6e64  ter: str = 'rand
-00004bc0: 6f6d 272c 0a20 2020 2068 6f70 7473 3a20  om',.    hopts: 
-00004bd0: 6469 6374 203d 207b 7d2c 0a20 2020 2049  dict = {},.    I
-00004be0: 4e54 4552 4641 4345 5f68 6f70 7473 3a20  NTERFACE_hopts: 
-00004bf0: 6469 6374 203d 207b 7d2c 0a29 3a0a 2020  dict = {},.):.  
-00004c00: 2020 2320 7475 726e 2074 6865 2049 4e54    # turn the INT
-00004c10: 4552 4641 4345 5f69 6e70 7574 2069 6e74  ERFACE_input int
-00004c20: 6f20 616e 2069 6e70 7574 2058 0a20 2020  o an input X.   
-00004c30: 2023 2062 6173 6564 206f 6e20 494e 5445   # based on INTE
-00004c40: 5246 4143 4520 4152 4753 2077 6865 7265  RFACE ARGS where
-00004c50: 2049 4e54 4552 4641 4345 5f68 6f70 7473   INTERFACE_hopts
-00004c60: 0a20 2020 2023 2073 7065 6369 6669 6573  .    # specifies
-00004c70: 2061 6464 6974 696f 6e61 6c20 6265 6861   additional beha
-00004c80: 7669 6f72 0a20 2020 2058 203d 205b 5d0a  vior.    X = [].
-00004c90: 2020 2020 0a20 2020 2023 2063 616c 6c20      .    # call 
-00004ca0: 7472 6169 6e20 7465 7374 2073 706c 6974  train test split
-00004cb0: 2077 6974 6820 7468 6973 2069 6e70 7574   with this input
-00004cc0: 0a20 2020 2072 6574 7572 6e20 7472 6169  .    return trai
-00004cd0: 6e5f 7465 7374 5f73 706c 6974 280a 2020  n_test_split(.  
-00004ce0: 2020 2020 2020 582c 0a20 2020 2020 2020        X,.       
-00004cf0: 2079 3d79 2c0a 2020 2020 2020 2020 6c61   y=y,.        la
-00004d00: 6265 6c73 3d6c 6162 656c 732c 0a20 2020  bels=labels,.   
-00004d10: 2020 2020 2074 6573 745f 7369 7a65 3d74       test_size=t
-00004d20: 6573 745f 7369 7a65 2c0a 2020 2020 2020  est_size,.      
-00004d30: 2020 7472 6169 6e5f 7369 7a65 3d74 7261    train_size=tra
-00004d40: 696e 5f73 697a 652c 0a20 2020 2020 2020  in_size,.       
-00004d50: 2073 706c 6974 7465 723d 7370 6c69 7474   splitter=splitt
-00004d60: 6572 2c0a 2020 2020 2020 2020 686f 7074  er,.        hopt
-00004d70: 733d 686f 7074 732c 0a20 2020 2029 0a60  s=hopts,.    ).`
-00004d80: 6060 0a0a 4966 2070 6f73 7369 626c 652c  ``..If possible,
-00004d90: 2077 6520 776f 756c 6420 6c69 6b65 2074   we would like t
-00004da0: 6f20 616c 736f 2061 6464 2061 6e20 6578  o also add an ex
-00004db0: 616d 706c 6520 4a75 7079 7465 7220 4e6f  ample Jupyter No
-00004dc0: 7465 626f 6f6b 2077 6974 6820 616e 7920  tebook with any 
-00004dd0: 6e65 7720 696e 7465 7266 6163 6520 746f  new interface to
-00004de0: 2064 656d 6f6e 7374 7261 7465 2074 6f20   demonstrate to 
-00004df0: 6e65 7720 7573 6572 7320 686f 7720 6974  new users how it
-00004e00: 2066 756e 6374 696f 6e73 2e20 5365 6520   functions. See 
-00004e10: 6f75 7220 6f74 6865 7220 6578 616d 706c  our other exampl
-00004e20: 6573 2069 6e20 7468 6520 6065 7861 6d70  es in the `examp
-00004e30: 6c65 7360 2064 6972 6563 746f 7279 2e0a  les` directory..
-00004e40: 0a43 6f6e 7461 6374 205b 404a 6163 6b73  .Contact [@Jacks
-00004e50: 6f6e 4275 726e 735d 2868 7474 7073 3a2f  onBurns](https:/
-00004e60: 2f67 6974 6875 622e 636f 6d2f 4a61 636b  /github.com/Jack
-00004e70: 736f 6e42 7572 6e73 2920 6966 2079 6f75  sonBurns) if you
-00004e80: 206e 6565 6420 6173 7369 7374 616e 6365   need assistance
-00004e90: 2061 6464 696e 6720 616e 2065 7869 7374   adding an exist
-00004ea0: 696e 6720 776f 726b 666c 6f77 2074 6f20  ing workflow to 
-00004eb0: 6061 7374 6172 7465 7360 2e20 4966 2074  `astartes`. If t
-00004ec0: 6869 7320 6665 6174 7572 697a 6174 696f  his featurizatio
-00004ed0: 6e20 7363 6865 6d65 2072 6571 7569 7265  n scheme require
-00004ee0: 7320 6164 6469 7469 6f6e 616c 2064 6570  s additional dep
-00004ef0: 656e 6465 6e63 6965 7320 746f 2066 756e  endencies to fun
-00004f00: 6374 696f 6e2c 2077 6520 6d61 7920 6164  ction, we may ad
-00004f10: 6420 6974 2061 7320 616e 2061 6464 6974  d it as an addit
-00004f20: 696f 6e61 6c20 5f65 7874 7261 5f20 7061  ional _extra_ pa
-00004f30: 636b 6167 6520 696e 2074 6865 2073 616d  ckage in the sam
-00004f40: 6520 7761 7920 7468 6174 2060 6d6f 6c65  e way that `mole
-00004f50: 6375 6c65 7360 2069 6e20 696e 7374 616c  cules` in instal
-00004f60: 6c65 642e 0a0a 2323 204a 4f53 5320 4272  led...## JOSS Br
-00004f70: 616e 6368 0a0a 6061 7374 6172 7465 7360  anch..`astartes`
-00004f80: 2063 6f72 7265 7370 6f6e 6469 6e67 204a   corresponding J
-00004f90: 4f53 5320 7061 7065 7220 6973 2073 746f  OSS paper is sto
-00004fa0: 7265 6420 696e 2074 6869 7320 7265 706f  red in this repo
-00004fb0: 7369 746f 7279 206f 6e20 6120 7365 7061  sitory on a sepa
-00004fc0: 7261 7465 2062 7261 6e63 682e 2059 6f75  rate branch. You
-00004fd0: 2063 616e 2066 696e 6420 6070 6170 6572   can find `paper
-00004fe0: 2e6d 6460 206f 6e20 7468 6520 6170 746c  .md` on the aptl
-00004ff0: 7920 6e61 6d65 6420 606a 6f73 732d 7061  y named `joss-pa
-00005000: 7065 7260 2062 7261 6e63 682e 200a 0a5f  per` branch. .._
-00005010: 4e6f 7465 2066 6f72 204d 6169 6e74 6169  Note for Maintai
-00005020: 6e65 7273 5f3a 2054 6f20 7075 7368 2063  ners_: To push c
-00005030: 6861 6e67 6573 2066 726f 6d20 7468 6520  hanges from the 
-00005040: 606d 6169 6e60 2062 7261 6e63 6820 696e  `main` branch in
-00005050: 746f 2074 6865 2060 6a6f 7373 2d70 6170  to the `joss-pap
-00005060: 6572 6020 6272 616e 6368 2c20 7275 6e20  er` branch, run 
-00005070: 7468 6520 6055 7064 6174 6520 4a4f 5353  the `Update JOSS
-00005080: 2042 7261 6e63 6860 2077 6f72 6b66 6c6f   Branch` workflo
-00005090: 772e 0a0a                                w...
+00000760: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000770: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00000780: 2e35 3238 312f 7a65 6e6f 646f 2e38 3134  .5281/zenodo.814
+00000790: 3732 3035 223e 3c69 6d67 2073 7263 3d22  7205"><img src="
+000007a0: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+000007b0: 7267 2f62 6164 6765 2f44 4f49 2f31 302e  rg/badge/DOI/10.
+000007c0: 3532 3831 2f7a 656e 6f64 6f2e 3831 3437  5281/zenodo.8147
+000007d0: 3230 352e 7376 6722 2061 6c74 3d22 444f  205.svg" alt="DO
+000007e0: 4922 3e3c 2f61 3e0a 3c2f 703e 0a0a 2323  I"></a>.</p>..##
+000007f0: 204f 6e6c 696e 6520 446f 6375 6d65 6e74   Online Document
+00000800: 6174 696f 6e0a 466f 6c6c 6f77 205b 7468  ation.Follow [th
+00000810: 6973 206c 696e 6b5d 2868 7474 7073 3a2f  is link](https:/
+00000820: 2f4a 6163 6b73 6f6e 4275 726e 732e 6769  /JacksonBurns.gi
+00000830: 7468 7562 2e69 6f2f 6173 7461 7274 6573  thub.io/astartes
+00000840: 2f29 2066 6f72 2061 206e 6963 656c 792d  /) for a nicely-
+00000850: 7265 6e64 6572 6564 2076 6572 7369 6f6e  rendered version
+00000860: 206f 6620 7468 6973 2052 4541 444d 4520   of this README 
+00000870: 616c 6f6e 6720 7769 7468 2061 6464 6974  along with addit
+00000880: 696f 6e61 6c20 7475 746f 7269 616c 7320  ional tutorials 
+00000890: 666f 7220 5b6d 6f76 696e 6720 6672 6f6d  for [moving from
+000008a0: 2074 7261 696e 5f74 6573 745f 7370 6c69   train_test_spli
+000008b0: 7420 696e 2073 6b6c 6561 726e 2074 6f20  t in sklearn to 
+000008c0: 6173 7461 7274 6573 5d28 6874 7470 733a  astartes](https:
+000008d0: 2f2f 6a61 636b 736f 6e62 7572 6e73 2e67  //jacksonburns.g
+000008e0: 6974 6875 622e 696f 2f61 7374 6172 7465  ithub.io/astarte
+000008f0: 732f 736b 6c65 6172 6e5f 746f 5f61 7374  s/sklearn_to_ast
+00000900: 6172 7465 732e 6874 6d6c 292e 0a4b 6565  artes.html)..Kee
+00000910: 7020 7265 6164 696e 6720 666f 7220 6120  p reading for a 
+00000920: 696e 7374 616c 6c61 7469 6f6e 2067 7569  installation gui
+00000930: 6465 2061 6e64 206c 696e 6b73 2074 6f20  de and links to 
+00000940: 7475 746f 7269 616c 7321 0a0a 2323 2049  tutorials!..## I
+00000950: 6e73 7461 6c6c 696e 6720 6061 7374 6172  nstalling `astar
+00000960: 7465 7360 0a57 6520 7265 636f 6d6d 656e  tes`.We recommen
+00000970: 6420 696e 7374 616c 6c69 6e67 2060 6173  d installing `as
+00000980: 7461 7274 6573 6020 7769 7468 696e 2061  tartes` within a
+00000990: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+000009a0: 6d65 6e74 2c20 7573 696e 6720 6569 7468  ment, using eith
+000009b0: 6572 2060 7665 6e76 6020 6f72 2060 636f  er `venv` or `co
+000009c0: 6e64 6160 2028 6f72 206f 7468 6572 2074  nda` (or other t
+000009d0: 6f6f 6c73 2920 746f 2073 696d 706c 6966  ools) to simplif
+000009e0: 7920 6465 7065 6e64 656e 6379 206d 616e  y dependency man
+000009f0: 6167 656d 656e 742e 2050 7974 686f 6e20  agement. Python 
+00000a00: 7665 7273 696f 6e73 2033 2e37 2c20 332e  versions 3.7, 3.
+00000a10: 382c 2033 2e39 2c20 332e 3130 2c20 616e  8, 3.9, 3.10, an
+00000a20: 6420 332e 3131 2061 7265 2073 7570 706f  d 3.11 are suppo
+00000a30: 7274 6564 206f 6e20 616c 6c20 706c 6174  rted on all plat
+00000a40: 666f 726d 732e 0a0a 6061 7374 6172 7465  forms...`astarte
+00000a50: 7360 2069 7320 6176 6169 6c61 626c 6520  s` is available 
+00000a60: 6f6e 2060 5079 5049 6020 616e 6420 6361  on `PyPI` and ca
+00000a70: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
+00000a80: 7369 6e67 2060 7069 7060 3a0a 0a20 2d20  sing `pip`:.. - 
+00000a90: 546f 2069 6e63 6c75 6465 2074 6865 2066  To include the f
+00000aa0: 6561 7475 7269 7a61 7469 6f6e 206f 7074  eaturization opt
+00000ab0: 696f 6e73 2066 6f72 2063 6865 6d69 6361  ions for chemica
+00000ac0: 6c20 6461 7461 2c20 7573 6520 6070 6970  l data, use `pip
+00000ad0: 2069 6e73 7461 6c6c 2061 7374 6172 7465   install astarte
+00000ae0: 735b 6d6f 6c65 6375 6c65 735d 602e 0a20  s[molecules]`.. 
+00000af0: 2d20 546f 2069 6e73 7461 6c6c 206f 6e6c  - To install onl
+00000b00: 7920 7468 6520 7361 6d70 6c69 6e67 2061  y the sampling a
+00000b10: 6c67 6f72 6974 686d 732c 2075 7365 2060  lgorithms, use `
+00000b20: 7069 7020 696e 7374 616c 6c20 6173 7461  pip install asta
+00000b30: 7274 6573 6020 2874 6869 7320 696e 7374  rtes` (this inst
+00000b40: 616c 6c20 7769 6c6c 2068 6176 6520 6665  all will have fe
+00000b50: 7765 7220 6465 7065 6e64 656e 6369 6573  wer dependencies
+00000b60: 2061 6e64 206d 6179 2062 6520 6d6f 7265   and may be more
+00000b70: 2072 6561 6469 6c79 2063 6f6d 7061 7469   readily compati
+00000b80: 626c 6520 696e 2065 6e76 6972 6f6e 6d65  ble in environme
+00000b90: 6e74 7320 7769 7468 2065 7869 7374 696e  nts with existin
+00000ba0: 6720 776f 726b 666c 6f77 7329 2e0a 0a54  g workflows)...T
+00000bb0: 6865 2062 6173 6520 6061 7374 6172 7465  he base `astarte
+00000bc0: 7360 2070 6163 6b61 6765 2069 7320 616c  s` package is al
+00000bd0: 736f 2061 7661 696c 6162 6c65 206f 6e20  so available on 
+00000be0: 6063 6f6e 6461 6020 7769 7468 2074 6869  `conda` with thi
+00000bf0: 7320 636f 6d6d 616e 643a 2060 636f 6e64  s command: `cond
+00000c00: 6120 696e 7374 616c 6c20 2d63 206a 6163  a install -c jac
+00000c10: 6b73 6f6e 6275 726e 7320 6173 7461 7274  ksonburns astart
+00000c20: 6573 602e 0a4e 6f74 6520 7468 6174 2074  es`..Note that t
+00000c30: 6869 7320 7061 636b 6167 6520 5f64 6f65  his package _doe
+00000c40: 7320 6e6f 745f 2069 6e63 6c75 6465 2062  s not_ include b
+00000c50: 7569 6c74 2d69 6e20 7375 7070 6f72 7420  uilt-in support 
+00000c60: 666f 7220 6665 6174 7572 697a 696e 6720  for featurizing 
+00000c70: 6d6f 6c65 6375 6c65 732c 2077 6869 6368  molecules, which
+00000c80: 2069 7320 6375 7272 656e 746c 7920 6f6e   is currently on
+00000c90: 6c79 2061 7661 696c 6162 6c65 2066 726f  ly available fro
+00000ca0: 6d20 7468 6520 5079 5049 2070 6163 6b61  m the PyPI packa
+00000cb0: 6765 206f 7220 6120 736f 7572 6365 2069  ge or a source i
+00000cc0: 6e73 7461 6c6c 2e0a 0a3e 202a 2a4e 6f74  nstall...> **Not
+00000cd0: 652a 2a0a 3e20 5769 6e64 6f77 7320 506f  e**.> Windows Po
+00000ce0: 7765 7273 6865 6c6c 2061 6e64 204d 6163  wershell and Mac
+00000cf0: 4f53 2043 6174 616c 696e 6120 6f72 206e  OS Catalina or n
+00000d00: 6577 6572 206d 6179 2063 6f6d 706c 6169  ewer may complai
+00000d10: 6e20 6162 6f75 7420 7371 7561 7265 2062  n about square b
+00000d20: 7261 636b 6574 732c 2073 6f20 796f 7520  rackets, so you 
+00000d30: 7769 6c6c 206e 6565 6420 746f 2064 6f75  will need to dou
+00000d40: 626c 6520 7175 6f74 6520 7468 6520 606d  ble quote the `m
+00000d50: 6f6c 6563 756c 6573 6020 636f 6d6d 616e  olecules` comman
+00000d60: 6420 2869 2e65 2e20 6070 6970 2069 6e73  d (i.e. `pip ins
+00000d70: 7461 6c6c 2022 6173 7461 7274 6573 5b6d  tall "astartes[m
+00000d80: 6f6c 6563 756c 6573 5d22 6029 0a0a 546f  olecules]"`)..To
+00000d90: 2069 6e73 7461 6c6c 2060 6173 7461 7274   install `astart
+00000da0: 6573 6020 6672 6f6d 2073 6f75 7263 652c  es` from source,
+00000db0: 2073 6565 2074 6865 205b 436f 6e74 7269   see the [Contri
+00000dc0: 6275 7469 6e67 2026 2044 6576 656c 6f70  buting & Develop
+00000dd0: 6572 204e 6f74 6573 5d28 2363 6f6e 7472  er Notes](#contr
+00000de0: 6962 7574 696e 672d 2d64 6576 656c 6f70  ibuting--develop
+00000df0: 6572 2d6e 6f74 6573 2920 7365 6374 696f  er-notes) sectio
+00000e00: 6e2e 0a0a 2323 2051 7569 636b 2053 7461  n...## Quick Sta
+00000e10: 7274 0a60 6173 7461 7274 6573 6020 6973  rt.`astartes` is
+00000e20: 2064 6573 6967 6e65 6420 6173 2061 2064   designed as a d
+00000e30: 726f 702d 696e 2072 6570 6c61 6365 6d65  rop-in replaceme
+00000e40: 6e74 2066 6f72 2060 736b 6c65 6172 6e60  nt for `sklearn`
+00000e50: 2773 2060 7472 6169 6e5f 7465 7374 5f73  's `train_test_s
+00000e60: 706c 6974 6020 6675 6e63 7469 6f6e 2028  plit` function (
+00000e70: 7365 6520 7468 6520 5b73 6b6c 6561 726e  see the [sklearn
+00000e80: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00000e90: 6874 7470 733a 2f2f 7363 696b 6974 2d6c  https://scikit-l
+00000ea0: 6561 726e 2e6f 7267 2f73 7461 626c 652f  earn.org/stable/
+00000eb0: 6d6f 6475 6c65 732f 6765 6e65 7261 7465  modules/generate
+00000ec0: 642f 736b 6c65 6172 6e2e 6d6f 6465 6c5f  d/sklearn.model_
+00000ed0: 7365 6c65 6374 696f 6e2e 7472 6169 6e5f  selection.train_
+00000ee0: 7465 7374 5f73 706c 6974 2e68 746d 6c29  test_split.html)
+00000ef0: 292e 2054 6f20 7377 6974 6368 2074 6f20  ). To switch to 
+00000f00: 6061 7374 6172 7465 7360 2c20 6368 616e  `astartes`, chan
+00000f10: 6765 2060 6672 6f6d 2073 6b6c 6561 726e  ge `from sklearn
+00000f20: 2e6d 6f64 656c 5f73 656c 6563 7469 6f6e  .model_selection
+00000f30: 2069 6d70 6f72 7420 7472 6169 6e5f 7465   import train_te
+00000f40: 7374 5f73 706c 6974 6020 746f 2060 6672  st_split` to `fr
+00000f50: 6f6d 2061 7374 6172 7465 7320 696d 706f  om astartes impo
+00000f60: 7274 2074 7261 696e 5f74 6573 745f 7370  rt train_test_sp
+00000f70: 6c69 7460 2e0a 0a4c 696b 6520 6073 6b6c  lit`...Like `skl
+00000f80: 6561 726e 602c 2060 6173 7461 7274 6573  earn`, `astartes
+00000f90: 6020 6163 6365 7074 7320 616e 7920 6974  ` accepts any it
+00000fa0: 6572 6162 6c65 206f 626a 6563 7420 6173  erable object as
+00000fb0: 2060 5860 2c20 6079 602c 2061 6e64 2060   `X`, `y`, and `
+00000fc0: 6c61 6265 6c73 602e 0a45 6163 6820 7769  labels`..Each wi
+00000fd0: 6c6c 2062 6520 636f 6e76 6572 7465 6420  ll be converted 
+00000fe0: 746f 2061 2060 6e75 6d70 7960 2061 7272  to a `numpy` arr
+00000ff0: 6179 2066 6f72 2069 6e74 6572 6e61 6c20  ay for internal 
+00001000: 6f70 6572 6174 696f 6e73 2c20 616e 6420  operations, and 
+00001010: 7265 7475 726e 6564 2061 7320 6120 606e  returned as a `n
+00001020: 756d 7079 6020 6172 7261 7920 7769 7468  umpy` array with
+00001030: 206c 696d 6974 6564 2065 7863 6570 7469   limited excepti
+00001040: 6f6e 733a 2069 6620 6058 6020 6973 2061  ons: if `X` is a
+00001050: 2060 7061 6e64 6173 6020 6044 6174 6146   `pandas` `DataF
+00001060: 7261 6d65 602c 2060 7960 2069 7320 6120  rame`, `y` is a 
+00001070: 6053 6572 6965 7360 2c20 6f72 2060 6c61  `Series`, or `la
+00001080: 6265 6c73 6020 6973 2061 2060 5365 7269  bels` is a `Seri
+00001090: 6573 602c 2060 6173 7461 7274 6573 6020  es`, `astartes` 
+000010a0: 7769 6c6c 2063 6173 7420 6974 2062 6163  will cast it bac
+000010b0: 6b20 746f 2069 7473 206f 7269 6769 6e61  k to its origina
+000010c0: 6c20 7479 7065 2069 6e63 6c75 6469 6e67  l type including
+000010d0: 2069 7473 2069 6e64 6578 2061 6e64 2063   its index and c
+000010e0: 6f6c 756d 6e20 6e61 6d65 732e 0a0a 3e20  olumn names...> 
+000010f0: 2a2a 4e6f 7465 2a2a 0a3e 2054 6865 2064  **Note**.> The d
+00001100: 6576 656c 6f70 6572 7320 7265 636f 6d6d  evelopers recomm
+00001110: 656e 6420 7061 7373 696e 6720 6058 602c  end passing `X`,
+00001120: 2060 7960 2c20 616e 6420 606c 6162 656c   `y`, and `label
+00001130: 7360 2061 7320 606e 756d 7079 6020 6172  s` as `numpy` ar
+00001140: 7261 7973 2061 6e64 2068 616e 646c 696e  rays and handlin
+00001150: 6720 7468 6520 636f 6e76 6572 7369 6f6e  g the conversion
+00001160: 2074 6f20 616e 6420 6672 6f6d 206f 7468   to and from oth
+00001170: 6572 2074 7970 6573 2065 7870 6c69 6369  er types explici
+00001180: 7479 206f 6e20 796f 7572 206f 776e 2e20  ty on your own. 
+00001190: 4265 6869 6e64 2d74 6865 2d73 6365 6e65  Behind-the-scene
+000011a0: 7320 7479 7065 2063 6173 7469 6e67 2063  s type casting c
+000011b0: 616e 206c 6561 6420 746f 2075 6e65 7870  an lead to unexp
+000011c0: 6563 7465 6420 6265 6861 7669 6f72 210a  ected behavior!.
+000011d0: 0a42 7920 6465 6661 756c 742c 2060 6173  .By default, `as
+000011e0: 7461 7274 6573 6020 7769 6c6c 2073 706c  tartes` will spl
+000011f0: 6974 2064 6174 6120 7261 6e64 6f6d 6c79  it data randomly
+00001200: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
+00001210: 6120 7661 7269 6574 7920 6f66 2061 6c67  a variety of alg
+00001220: 6f72 6974 686d 6963 2073 616d 706c 696e  orithmic samplin
+00001230: 6720 6170 7072 6f61 6368 6573 2063 616e  g approaches can
+00001240: 2062 6520 7573 6564 2062 7920 7370 6563   be used by spec
+00001250: 6966 7969 6e67 2074 6865 2060 7361 6d70  ifying the `samp
+00001260: 6c65 7260 2061 7267 756d 656e 7420 746f  ler` argument to
+00001270: 2074 6865 2066 756e 6374 696f 6e20 2873   the function (s
+00001280: 6565 2074 6865 205b 5461 626c 6520 6f66  ee the [Table of
+00001290: 2049 6d70 6c65 6d65 6e74 6564 2053 616d   Implemented Sam
+000012a0: 706c 6572 735d 2823 696d 706c 656d 656e  plers](#implemen
+000012b0: 7465 642d 7361 6d70 6c69 6e67 2d61 6c67  ted-sampling-alg
+000012c0: 6f72 6974 686d 7329 2066 6f72 2061 2063  orithms) for a c
+000012d0: 6f6d 706c 6574 206c 6973 7420 6f66 206f  omplet list of o
+000012e0: 7074 696f 6e73 2061 6e64 2074 6865 6972  ptions and their
+000012f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2072   corresponding r
+00001300: 6566 6572 656e 6365 7329 3a0a 0a60 6060  eferences):..```
+00001310: 7079 7468 6f6e 0a58 5f74 7261 696e 2c20  python.X_train, 
+00001320: 585f 7465 7374 2c20 795f 7472 6169 6e2c  X_test, y_train,
+00001330: 2079 5f74 6573 7420 3d20 7472 6169 6e5f   y_test = train_
+00001340: 7465 7374 5f73 706c 6974 280a 2020 582c  test_split(.  X,
+00001350: 2020 2320 7072 6566 6572 6162 6c79 206e    # preferably n
+00001360: 756d 7079 2061 7272 6179 732c 2062 7574  umpy arrays, but
+00001370: 2061 7374 6172 7465 7320 7769 6c6c 2063   astartes will c
+00001380: 6173 7420 6974 2066 6f72 2079 6f75 0a20  ast it for you. 
+00001390: 2079 2c0a 2020 7361 6d70 6c65 7220 3d20   y,.  sampler = 
+000013a0: 276b 656e 6e61 7264 5f73 746f 6e65 272c  'kennard_stone',
+000013b0: 2020 2320 616e 7920 6f66 2074 6865 2073    # any of the s
+000013c0: 7570 706f 7274 6564 2073 616d 706c 6572  upported sampler
+000013d0: 730a 290a 6060 600a 0a54 6861 7427 7320  s.).```..That's 
+000013e0: 616c 6c20 796f 7520 6e65 6564 2074 6f20  all you need to 
+000013f0: 6765 7420 7374 6172 7465 6420 7769 7468  get started with
+00001400: 2060 6173 7461 7274 6573 6021 2054 6865   `astartes`! The
+00001410: 206e 6578 7420 7365 6374 696f 6e73 2069   next sections i
+00001420: 6e63 6c75 6465 206d 6f72 6520 6578 616d  nclude more exam
+00001430: 706c 6573 2061 6e64 2073 6f6d 6520 6465  ples and some de
+00001440: 6d6f 206e 6f74 6562 6f6f 6b73 2079 6f75  mo notebooks you
+00001450: 2063 616e 2074 7279 2069 6e20 796f 7572   can try in your
+00001460: 2062 726f 7773 6572 2e0a 0a23 2323 2045   browser...### E
+00001470: 7861 6d70 6c65 204e 6f74 6562 6f6f 6b73  xample Notebooks
+00001480: 0a0a 436c 6963 6b20 7468 6520 6261 6467  ..Click the badg
+00001490: 6573 2069 6e20 7468 6520 7461 626c 6520  es in the table 
+000014a0: 6265 6c6f 7720 746f 2062 6520 7461 6b65  below to be take
+000014b0: 6e20 746f 2061 206c 6976 652c 2069 6e74  n to a live, int
+000014c0: 6572 6163 7469 7665 2064 656d 6f20 6f66  eractive demo of
+000014d0: 2060 6173 7461 7274 6573 603a 0a0a 7c20   `astartes`:..| 
+000014e0: 4465 6d6f 207c 2054 6f70 6963 207c 204c  Demo | Topic | L
+000014f0: 696e 6b20 7c0a 7c3a 2d2d 2d3a 7c2d 2d2d  ink |.|:---:|---
+00001500: 7c2d 2d2d 7c0a 7c20 436f 6d70 6172 696e  |---|.| Comparin
+00001510: 6720 5361 6d70 6c69 6e67 2041 6c67 6f72  g Sampling Algor
+00001520: 6974 686d 7320 7769 7468 2046 6173 7420  ithms with Fast 
+00001530: 466f 6f64 207c 2056 6973 7561 6c20 7265  Food | Visual re
+00001540: 7072 6573 656e 7461 7469 6f6e 7320 6f66  presentations of
+00001550: 2068 6f77 2064 6966 6665 7265 6e74 2073   how different s
+00001560: 616d 706c 6572 7320 6166 6665 6374 2064  amplers affect d
+00001570: 6174 6120 7061 7274 6974 696f 6e69 6e67  ata partitioning
+00001580: 207c 205b 215b 436f 6c61 625d 2868 7474   | [![Colab](htt
+00001590: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000015a0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000015b0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000015c0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000015d0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+000015e0: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+000015f0: 2f4a 6163 6b73 6f6e 4275 726e 732f 6173  /JacksonBurns/as
+00001600: 7461 7274 6573 2f62 6c6f 622f 6d61 696e  tartes/blob/main
+00001610: 2f65 7861 6d70 6c65 732f 7370 6c69 745f  /examples/split_
+00001620: 636f 6d70 6172 6973 6f6e 732f 7370 6c69  comparisons/spli
+00001630: 745f 636f 6d70 6172 6973 6f6e 732e 6970  t_comparisons.ip
+00001640: 796e 6229 207c 0a7c 2055 7369 6e67 2060  ynb) |.| Using `
+00001650: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001660: 706c 6974 6020 7769 7468 2074 6865 2060  plit` with the `
+00001670: 736b 6c65 6172 6e60 2065 7861 6d70 6c65  sklearn` example
+00001680: 2064 6174 6173 6574 7320 7c20 4465 6d6f   datasets | Demo
+00001690: 6e73 7472 6174 696e 6720 686f 7720 7769  nstrating how wi
+000016a0: 7468 6f6c 6469 6e67 2061 2074 6573 7420  tholding a test 
+000016b0: 7365 7420 7769 7468 2060 7472 6169 6e5f  set with `train_
+000016c0: 7661 6c5f 7465 7374 5f73 706c 6974 6020  val_test_split` 
+000016d0: 6361 6e20 696d 7061 6374 2070 6572 666f  can impact perfo
+000016e0: 726d 616e 6365 207c 205b 215b 436f 6c61  rmance | [![Cola
+000016f0: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
+00001700: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001710: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+00001720: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
+00001730: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+00001740: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+00001750: 6769 7468 7562 2f4a 6163 6b73 6f6e 4275  github/JacksonBu
+00001760: 726e 732f 6173 7461 7274 6573 2f62 6c6f  rns/astartes/blo
+00001770: 622f 6d61 696e 2f65 7861 6d70 6c65 732f  b/main/examples/
+00001780: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001790: 706c 6974 5f73 6b6c 6561 726e 5f65 7861  plit_sklearn_exa
+000017a0: 6d70 6c65 2f74 7261 696e 5f76 616c 5f74  mple/train_val_t
+000017b0: 6573 745f 7370 6c69 745f 6578 616d 706c  est_split_exampl
+000017c0: 652e 6970 796e 6229 207c 0a7c 2043 6865  e.ipynb) |.| Che
+000017d0: 6d69 6e66 6f72 6d61 7469 6373 2073 616d  minformatics sam
+000017e0: 706c 6520 7365 7420 7061 7274 6974 696f  ple set partitio
+000017f0: 6e69 6e67 2077 6974 6820 6061 7374 6172  ning with `astar
+00001800: 7465 7360 207c 2045 7874 7261 706f 6c61  tes` | Extrapola
+00001810: 7469 6f6e 2076 732e 2049 6e74 6572 706f  tion vs. Interpo
+00001820: 6c61 7469 6f6e 2069 6d70 6163 7420 6f6e  lation impact on
+00001830: 2063 6865 6d69 6e66 6f72 6d61 7469 6373   cheminformatics
+00001840: 206d 6f64 656c 2061 6363 7572 6163 7920   model accuracy 
+00001850: 7c20 5b21 5b43 6f6c 6162 5d28 6874 7470  | [![Colab](http
+00001860: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001870: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
+00001880: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
+00001890: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+000018a0: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+000018b0: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+000018c0: 4a61 636b 736f 6e42 7572 6e73 2f61 7374  JacksonBurns/ast
+000018d0: 6172 7465 732f 626c 6f62 2f6d 6169 6e2f  artes/blob/main/
+000018e0: 6578 616d 706c 6573 2f62 6172 7269 6572  examples/barrier
+000018f0: 5f70 7265 6469 6374 696f 6e5f 7769 7468  _prediction_with
+00001900: 5f52 4442 372f 5244 4237 5f62 6172 7269  _RDB7/RDB7_barri
+00001910: 6572 5f70 7265 6469 6374 696f 6e5f 6578  er_prediction_ex
+00001920: 616d 706c 652e 6970 796e 6229 207c 0a7c  ample.ipynb) |.|
+00001930: 2043 6f6d 7061 7269 6e67 2070 6172 7469   Comparing parti
+00001940: 7469 6f6e 696e 6720 6170 7072 6f61 6368  tioning approach
+00001950: 6573 2066 6f72 2061 6c6b 616e 6573 207c  es for alkanes |
+00001960: 2056 6973 7561 6c69 7a69 6e67 2068 6f77   Visualizing how
+00001970: 2073 616d 706c 6572 2069 6d70 6163 7420   sampler impact 
+00001980: 6d6f 6465 6c20 7065 7266 6f72 6d61 6e63  model performanc
+00001990: 6520 7769 7468 2073 696d 706c 6520 6368  e with simple ch
+000019a0: 656d 6963 616c 7320 7c20 5b21 5b43 6f6c  emicals | [![Col
+000019b0: 6162 5d28 6874 7470 733a 2f2f 636f 6c61  ab](https://cola
+000019c0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+000019d0: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
+000019e0: 6162 2d62 6164 6765 2e73 7667 295d 2868  ab-badge.svg)](h
+000019f0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00001a00: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00001a10: 2f67 6974 6875 622f 4a61 636b 736f 6e42  /github/JacksonB
+00001a20: 7572 6e73 2f61 7374 6172 7465 732f 626c  urns/astartes/bl
+00001a30: 6f62 2f6d 6169 6e2f 6578 616d 706c 6573  ob/main/examples
+00001a40: 2f6d 6c70 6473 5f32 3032 335f 6173 7461  /mlpds_2023_asta
+00001a50: 7274 6573 5f64 656d 6f6e 7374 7261 7469  rtes_demonstrati
+00001a60: 6f6e 2f6d 6c70 6473 5f32 3032 335f 6465  on/mlpds_2023_de
+00001a70: 6d6f 2e69 7079 6e62 2920 7c0a 0a54 6f20  mo.ipynb) |..To 
+00001a80: 6578 6563 7574 6520 7468 6573 6520 6e6f  execute these no
+00001a90: 7465 626f 6f6b 7320 6c6f 6361 6c6c 792c  tebooks locally,
+00001aa0: 2063 6c6f 6e65 2074 6869 7320 7265 706f   clone this repo
+00001ab0: 7369 746f 7279 2028 692e 652e 2060 6769  sitory (i.e. `gi
+00001ac0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00001ad0: 6769 7468 7562 2e63 6f6d 2f4a 6163 6b73  github.com/Jacks
+00001ae0: 6f6e 4275 726e 732f 6173 7461 7274 6573  onBurns/astartes
+00001af0: 2e67 6974 6029 2c20 6e61 7669 6761 7465  .git`), navigate
+00001b00: 2074 6f20 7468 6520 6061 7374 6172 7465   to the `astarte
+00001b10: 7360 2064 6972 6563 746f 7279 2c20 7275  s` directory, ru
+00001b20: 6e20 6070 6970 2069 6e73 7461 6c6c 202e  n `pip install .
+00001b30: 5b64 656d 6f73 5d60 2c20 7468 656e 206f  [demos]`, then o
+00001b40: 7065 6e20 616e 6420 7275 6e20 7468 6520  pen and run the 
+00001b50: 6e6f 7465 626f 6f6b 7320 696e 2079 6f75  notebooks in you
+00001b60: 7220 7072 6566 6572 7265 6420 6564 6974  r preferred edit
+00001b70: 6f72 2e0a 596f 7520 646f 205f 6e6f 745f  or..You do _not_
+00001b80: 206e 6565 6420 746f 2065 7865 6375 7465   need to execute
+00001b90: 2074 6865 2063 656c 6c73 2070 7265 6669   the cells prefi
+00001ba0: 7865 6420 7769 7468 2060 2525 6361 7074  xed with `%%capt
+00001bb0: 7572 6560 202d 2074 6865 7920 6172 6520  ure` - they are 
+00001bc0: 6f6e 6c79 2070 7265 7365 6e74 2066 6f72  only present for
+00001bd0: 2063 6f6d 7061 7469 6269 6c69 7479 2077   compatibility w
+00001be0: 6974 6820 476f 6f67 6c65 2043 6f6c 6162  ith Google Colab
+00001bf0: 2e0a 0a23 2323 2057 6974 6868 6f6c 6420  ...### Withhold 
+00001c00: 5465 7374 696e 6720 4461 7461 2077 6974  Testing Data wit
+00001c10: 6820 6074 7261 696e 5f76 616c 5f74 6573  h `train_val_tes
+00001c20: 745f 7370 6c69 7460 0a46 6f72 2072 6967  t_split`.For rig
+00001c30: 6f72 6f75 7320 4d4c 2072 6573 6561 7263  orous ML researc
+00001c40: 682c 2069 7420 6973 2063 7269 7469 6361  h, it is critica
+00001c50: 6c20 746f 2077 6974 6868 6f6c 6420 736f  l to withhold so
+00001c60: 6d65 2064 6174 6120 6475 7269 6e67 2074  me data during t
+00001c70: 7261 696e 696e 6720 746f 2075 7365 2061  raining to use a
+00001c80: 2060 7465 7374 6020 7365 742e 0a54 6865   `test` set..The
+00001c90: 206d 6f64 656c 2073 686f 756c 6420 5f6e   model should _n
+00001ca0: 6576 6572 5f20 7365 6520 7468 6973 2064  ever_ see this d
+00001cb0: 6174 6120 6475 7269 6e67 2074 7261 696e  ata during train
+00001cc0: 696e 6720 2875 6e6c 696b 6520 7468 6520  ing (unlike the 
+00001cd0: 7661 6c69 6461 7469 6f6e 2073 6574 2920  validation set) 
+00001ce0: 736f 2074 6861 7420 7765 2063 616e 2067  so that we can g
+00001cf0: 6574 2061 6e20 6163 6375 7261 7465 206d  et an accurate m
+00001d00: 6561 7375 7265 6d65 6e74 206f 6620 6974  easurement of it
+00001d10: 7320 7065 7266 6f72 6d61 6e63 652e 0a0a  s performance...
+00001d20: 5769 7468 2060 6173 7461 7274 6573 6020  With `astartes` 
+00001d30: 7065 7266 6f72 6d69 6e67 2074 6869 7320  performing this 
+00001d40: 7468 7265 652d 7761 7920 6461 7461 2073  three-way data s
+00001d50: 706c 6974 2069 7320 7265 6164 696c 7920  plit is readily 
+00001d60: 6176 6169 6c61 626c 6520 7769 7468 2060  available with `
+00001d70: 7472 6169 6e5f 7661 6c5f 7465 7374 5f73  train_val_test_s
+00001d80: 706c 6974 603a 0a60 6060 7079 7468 6f6e  plit`:.```python
+00001d90: 0a66 726f 6d20 6173 7461 7274 6573 2069  .from astartes i
+00001da0: 6d70 6f72 7420 7472 6169 6e5f 7661 6c5f  mport train_val_
+00001db0: 7465 7374 5f73 706c 6974 0a0a 585f 7472  test_split..X_tr
+00001dc0: 6169 6e2c 2058 5f76 616c 2c20 585f 7465  ain, X_val, X_te
+00001dd0: 7374 203d 2074 7261 696e 5f76 616c 5f74  st = train_val_t
+00001de0: 6573 745f 7370 6c69 7428 582c 2073 616d  est_split(X, sam
+00001df0: 706c 6572 203d 2027 7370 6865 7265 5f65  pler = 'sphere_e
+00001e00: 7863 6c75 7369 6f6e 2729 0a60 6060 0a59  xclusion').```.Y
+00001e10: 6f75 2063 616e 206e 6f77 2074 7261 696e  ou can now train
+00001e20: 2079 6f75 7220 6d6f 6465 6c20 7769 7468   your model with
+00001e30: 2060 585f 7472 6169 6e60 2c20 6f70 7469   `X_train`, opti
+00001e40: 6d69 7a65 2079 6f75 7220 6d6f 6465 6c20  mize your model 
+00001e50: 7769 7468 2060 585f 7661 6c60 2c20 616e  with `X_val`, an
+00001e60: 6420 6d65 6173 7572 6520 6974 7320 7065  d measure its pe
+00001e70: 7266 6f72 6d61 6e63 6520 7769 7468 2060  rformance with `
+00001e80: 585f 7465 7374 602e 0a0a 2323 2320 4576  X_test`...### Ev
+00001e90: 616c 7561 7465 2074 6865 2049 6d70 6163  aluate the Impac
+00001ea0: 7420 6f66 2053 706c 6974 7469 6e67 2041  t of Splitting A
+00001eb0: 6c67 6f72 6974 686d 730a 466f 7220 6461  lgorithms.For da
+00001ec0: 7461 2077 6974 6820 6d61 6e79 2066 6561  ta with many fea
+00001ed0: 7475 7265 7320 6974 2063 616e 2062 6520  tures it can be 
+00001ee0: 6469 6666 6963 756c 7420 746f 2076 6973  difficult to vis
+00001ef0: 7561 6c69 7a65 2068 6f77 2064 6966 6665  ualize how diffe
+00001f00: 7265 6e74 2073 616d 706c 696e 6720 616c  rent sampling al
+00001f10: 676f 7269 7468 6d73 2063 6861 6e67 6520  gorithms change 
+00001f20: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+00001f30: 206f 6620 6461 7461 2069 6e74 6f20 7472   of data into tr
+00001f40: 6169 6e69 6e67 2c20 7661 6c69 6461 7469  aining, validati
+00001f50: 6f6e 2c20 616e 6420 7465 7374 696e 6720  on, and testing 
+00001f60: 6c69 6b65 2077 6520 646f 2069 6e20 736f  like we do in so
+00001f70: 6d65 206f 6620 7468 6520 6465 6d6f 206e  me of the demo n
+00001f80: 6f74 6562 6f6f 6b73 2e0a 546f 2061 6964  otebooks..To aid
+00001f90: 2069 6e20 616e 616c 797a 696e 6720 7468   in analyzing th
+00001fa0: 6520 696d 7061 6374 206f 6620 7468 6520  e impact of the 
+00001fb0: 616c 676f 7269 7468 6d73 2c20 6061 7374  algorithms, `ast
+00001fc0: 6172 7465 7360 2070 726f 7669 6465 7320  artes` provides 
+00001fd0: 6067 656e 6572 6174 655f 7265 6772 6573  `generate_regres
+00001fe0: 7369 6f6e 5f72 6573 756c 7473 5f64 6963  sion_results_dic
+00001ff0: 7460 2e0a 5468 6973 2066 756e 6374 696f  t`..This functio
+00002000: 6e20 616c 6c6f 7773 2075 7365 7273 2074  n allows users t
+00002010: 6f20 7175 6963 6b6c 7920 6576 616c 7561  o quickly evalua
+00002020: 7465 2074 6865 2069 6d70 6163 7420 6f66  te the impact of
+00002030: 2064 6966 6665 7265 6e74 2073 706c 6974   different split
+00002040: 7469 6e67 2074 6563 686e 6971 7565 7320  ting techniques 
+00002050: 6f6e 2061 6e79 206d 6f64 656c 2073 7570  on any model sup
+00002060: 706f 7274 6564 2062 7920 6073 6b6c 6561  ported by `sklea
+00002070: 726e 602e 2041 6c6c 2072 6573 756c 7473  rn`. All results
+00002080: 2061 7265 2073 746f 7265 6420 696e 2061   are stored in a
+00002090: 2064 6963 7469 6f6e 6172 7920 666f 726d   dictionary form
+000020a0: 6174 2061 6e64 2063 616e 2062 6520 6469  at and can be di
+000020b0: 7370 6c61 7965 6420 696e 2061 206e 6561  splayed in a nea
+000020c0: 746c 7920 666f 726d 6174 7465 6420 7461  tly formatted ta
+000020d0: 626c 6520 7573 696e 6720 7468 6520 6f70  ble using the op
+000020e0: 7469 6f6e 616c 2060 7072 696e 745f 7265  tional `print_re
+000020f0: 7375 6c74 7360 2061 7267 756d 656e 742e  sults` argument.
+00002100: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00002110: 2073 6b6c 6561 726e 2e73 766d 2069 6d70   sklearn.svm imp
+00002120: 6f72 7420 4c69 6e65 6172 5356 520a 0a66  ort LinearSVR..f
+00002130: 726f 6d20 6173 7461 7274 6573 2e75 7469  rom astartes.uti
+00002140: 6c73 2069 6d70 6f72 7420 6765 6e65 7261  ls import genera
+00002150: 7465 5f72 6567 7265 7373 696f 6e5f 7265  te_regression_re
+00002160: 7375 6c74 735f 6469 6374 0a0a 736b 6c65  sults_dict..skle
+00002170: 6172 6e5f 6d6f 6465 6c20 3d20 4c69 6e65  arn_model = Line
+00002180: 6172 5356 5228 290a 7265 7375 6c74 735f  arSVR().results_
+00002190: 6469 6374 203d 2067 656e 6572 6174 655f  dict = generate_
+000021a0: 7265 6772 6573 7369 6f6e 5f72 6573 756c  regression_resul
+000021b0: 7473 5f64 6963 7428 0a20 2020 2073 6b6c  ts_dict(.    skl
+000021c0: 6561 726e 5f6d 6f64 656c 2c0a 2020 2020  earn_model,.    
+000021d0: 582c 0a20 2020 2079 2c0a 2020 2020 7072  X,.    y,.    pr
+000021e0: 696e 745f 7265 7375 6c74 733d 5472 7565  int_results=True
+000021f0: 2c0a 290a 0a20 2020 2020 2020 2020 5472  ,.)..         Tr
+00002200: 6169 6e20 2020 2020 2020 5661 6c20 2020  ain       Val   
+00002210: 2020 2054 6573 740a 2d2d 2d2d 2020 2d2d     Test.----  --
+00002220: 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2d2d 2d2d  ------  --------
+00002230: 2020 2d2d 2d2d 2d2d 2d2d 0a4d 4145 2020    --------.MAE  
+00002240: 2031 2e34 3135 3232 2020 2033 2e31 3334   1.41522   3.134
+00002250: 3335 2020 2032 2e31 3730 3931 0a52 4d53  35   2.17091.RMS
+00002260: 4520 2032 2e30 3330 3632 2020 2033 2e37  E  2.03062   3.7
+00002270: 3337 3231 2020 2032 2e34 3030 3431 0a52  3721   2.40041.R
+00002280: 3220 2020 2030 2e39 3037 3435 2020 2030  2    0.90745   0
+00002290: 2e38 3037 3837 2020 2030 2e37 3834 3132  .80787   0.78412
+000022a0: 0a0a 6060 600a 0a23 2323 2041 6363 6573  ..```..### Acces
+000022b0: 7320 5361 6d70 6c69 6e67 2041 6c67 6f72  s Sampling Algor
+000022c0: 6974 686d 7320 4469 7265 6374 6c79 0a54  ithms Directly.T
+000022d0: 6865 2073 616d 706c 696e 6720 616c 676f  he sampling algo
+000022e0: 7269 7468 6d73 2069 6d70 6c65 6d65 6e74  rithms implement
+000022f0: 6564 2069 6e20 6061 7374 6172 7465 7360  ed in `astartes`
+00002300: 2063 616e 2061 6c73 6f20 6265 2064 6972   can also be dir
+00002310: 6563 746c 7920 6163 6365 7373 6564 2061  ectly accessed a
+00002320: 6e64 2072 756e 2069 6620 6974 2069 7320  nd run if it is 
+00002330: 6d6f 7265 2075 7365 6675 6c20 666f 7220  more useful for 
+00002340: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
+00002350: 732e 0a49 6e20 7468 6520 6265 6c6f 7720  s..In the below 
+00002360: 6578 616d 706c 652c 2077 6520 696d 706f  example, we impo
+00002370: 7274 2074 6865 204b 656e 6e61 7264 2053  rt the Kennard S
+00002380: 746f 6e65 2073 616d 706c 6572 2c20 7573  tone sampler, us
+00002390: 6520 6974 2074 6f20 7061 7274 6974 696f  e it to partitio
+000023a0: 6e20 6120 7369 6d70 6c65 2061 7272 6179  n a simple array
+000023b0: 2c20 616e 6420 7468 656e 2072 6574 7269  , and then retri
+000023c0: 6576 6520 6120 7361 6d70 6c65 2e0a 6060  eve a sample..``
+000023d0: 6070 7974 686f 6e0a 6672 6f6d 2061 7374  `python.from ast
+000023e0: 6172 7465 732e 7361 6d70 6c65 7273 2e69  artes.samplers.i
+000023f0: 6e74 6572 706f 6c61 7469 6f6e 2069 6d70  nterpolation imp
+00002400: 6f72 7420 4b65 6e6e 6172 6453 746f 6e65  ort KennardStone
+00002410: 0a0a 6b65 6e6e 6172 645f 7374 6f6e 6520  ..kennard_stone 
+00002420: 3d20 4b65 6e6e 6172 6453 746f 6e65 285b  = KennardStone([
+00002430: 5b31 2c20 325d 2c20 5b33 2c20 345d 2c20  [1, 2], [3, 4], 
+00002440: 5b35 2c20 365d 5d29 0a66 6972 7374 5f32  [5, 6]]).first_2
+00002450: 5f73 616d 706c 6573 203d 206b 656e 6e61  _samples = kenna
+00002460: 7264 5f73 746f 6e65 2e67 6574 5f73 616d  rd_stone.get_sam
+00002470: 706c 655f 6964 7873 2832 290a 6060 600a  ple_idxs(2).```.
+00002480: 416c 6c20 7361 6d70 6c65 7273 2069 6e20  All samplers in 
+00002490: 6061 7374 6172 7465 7360 2069 6d70 6c65  `astartes` imple
+000024a0: 6d65 6e74 2061 2060 5f73 616d 706c 6528  ment a `_sample(
+000024b0: 2960 206d 6574 686f 6420 7468 6174 2069  )` method that i
+000024c0: 7320 6361 6c6c 6564 2062 7920 7468 6520  s called by the 
+000024d0: 636f 6e73 7472 7563 746f 7220 2869 2e65  constructor (i.e
+000024e0: 2e20 6772 6565 6469 6c79 2920 616e 6420  . greedily) and 
+000024f0: 6569 7468 6572 2061 2060 6765 745f 7361  either a `get_sa
+00002500: 6d70 6c65 725f 6964 7873 6020 6f72 2060  mpler_idxs` or `
+00002510: 6765 745f 636c 7573 7465 725f 6964 7873  get_cluster_idxs
+00002520: 6020 666f 7220 696e 7465 7270 6f6c 6174  ` for interpolat
+00002530: 6976 6520 616e 6420 6578 7472 6170 6f6c  ive and extrapol
+00002540: 6174 6976 6520 7361 6d70 6c65 7273 2c20  ative samplers, 
+00002550: 7265 7370 6563 7469 7665 6c79 2e0a 466f  respectively..Fo
+00002560: 7220 6d6f 7265 2064 6574 6169 6c20 6f6e  r more detail on
+00002570: 2074 6865 2069 6d70 6c65 6d65 6e74 6169   the implementai
+00002580: 746f 6e20 616e 6420 6465 7369 676e 206f  ton and design o
+00002590: 6620 7361 6d70 6c65 7273 2069 6e20 6061  f samplers in `a
+000025a0: 7374 6172 7465 7360 2c20 7365 6520 7468  startes`, see th
+000025b0: 6520 5b44 6576 656c 6f70 6572 204e 6f74  e [Developer Not
+000025c0: 6573 5d28 2363 6f6e 7472 6962 7574 696e  es](#contributin
+000025d0: 672d 2d64 6576 656c 6f70 6572 2d6e 6f74  g--developer-not
+000025e0: 6573 2920 7365 6374 696f 6e2e 0a0a 2323  es) section...##
+000025f0: 2054 6865 6f72 7920 616e 6420 4170 706c   Theory and Appl
+00002600: 6963 6174 696f 6e20 6f66 2060 6173 7461  ication of `asta
+00002610: 7274 6573 600a 5468 6973 2073 6563 7469  rtes`.This secti
+00002620: 6f6e 206f 6620 7468 6520 5245 4144 4d45  on of the README
+00002630: 2064 6574 6169 6c73 2073 6f6d 6520 6f66   details some of
+00002640: 2074 6865 2074 6865 6f72 7920 6265 6869   the theory behi
+00002650: 6e64 2077 6879 2074 6865 2061 6c67 6f72  nd why the algor
+00002660: 6974 686d 7320 696d 706c 656d 656e 7465  ithms implemente
+00002670: 6420 696e 2060 6173 7461 7274 6573 6020  d in `astartes` 
+00002680: 6172 6520 696d 706f 7274 616e 7420 616e  are important an
+00002690: 6420 736f 6d65 206d 6f74 6976 6174 696e  d some motivatin
+000026a0: 6720 6578 616d 706c 6573 2e0a 466f 7220  g examples..For 
+000026b0: 6120 636f 6d70 7265 6865 6e73 6976 6520  a comprehensive 
+000026c0: 7761 6c6b 7468 726f 7567 6820 6f66 2074  walkthrough of t
+000026d0: 6865 2074 6865 6f72 7920 616e 6420 696d  he theory and im
+000026e0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+000026f0: 6061 7374 6172 7465 7360 2c20 666f 6c6c  `astartes`, foll
+00002700: 6f77 205b 7468 6973 206c 696e 6b5d 2868  ow [this link](h
+00002710: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002720: 6d2f 4a61 636b 736f 6e42 7572 6e73 2f61  m/JacksonBurns/a
+00002730: 7374 6172 7465 732f 7261 772f 6a6f 7373  startes/raw/joss
+00002740: 2d70 6170 6572 2f42 7572 6e73 2d53 7069  -paper/Burns-Spi
+00002750: 656b 6572 6d61 6e6e 2d42 6861 7474 6163  ekermann-Bhattac
+00002760: 6861 726a 6565 5f61 7374 6172 7465 732e  harjee_astartes.
+00002770: 7064 6629 2074 6f20 7265 6164 2074 6865  pdf) to read the
+00002780: 2063 6f6d 7061 6e69 6f6e 2070 6170 6572   companion paper
+00002790: 2028 6672 6565 6c79 2061 7661 696c 6162   (freely availab
+000027a0: 6c65 2061 6e64 2068 6f73 7465 6420 6865  le and hosted he
+000027b0: 7265 206f 6e20 4769 7448 7562 292e 0a0a  re on GitHub)...
+000027c0: 3e20 2a2a 4e6f 7465 2a2a 0a3e 2057 6520  > **Note**.> We 
+000027d0: 7265 6665 7265 6e63 6520 6f70 656e 2d61  reference open-a
+000027e0: 6363 6573 7320 7075 626c 6963 6174 696f  ccess publicatio
+000027f0: 6e73 2077 6865 7265 7665 7220 706f 7373  ns wherever poss
+00002800: 6962 6c65 2e20 466f 7220 6172 7469 636c  ible. For articl
+00002810: 6573 206c 6f63 6b65 6420 6265 6869 6e64  es locked behind
+00002820: 2061 2070 6179 7761 6c6c 2028 6465 6e6f   a paywall (deno
+00002830: 7465 6420 7769 7468 203a 736d 616c 6c5f  ted with :small_
+00002840: 626c 7565 5f64 6961 6d6f 6e64 3a29 2c20  blue_diamond:), 
+00002850: 7765 2069 6e73 7465 6164 2073 7567 6765  we instead sugge
+00002860: 7374 2072 6561 6469 6e67 205b 7468 6973  st reading [this
+00002870: 2057 696b 6970 6564 6961 2070 6167 655d   Wikipedia page]
+00002880: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+00002890: 7065 6469 612e 6f72 672f 7769 6b69 2f53  pedia.org/wiki/S
+000028a0: 6369 2d48 7562 2920 616e 6420 6162 736f  ci-Hub) and abso
+000028b0: 6c75 7465 6c79 205f 5f6e 6f74 5f5f 2061  lutely __not__ a
+000028c0: 7474 656d 7074 696e 6720 746f 2062 7970  ttempting to byp
+000028d0: 6173 7320 7468 6520 7061 7977 616c 6c2e  ass the paywall.
+000028e0: 0a0a 2323 2320 5261 7469 6f6e 616c 2053  ..### Rational S
+000028f0: 706c 6974 7469 6e67 2041 6c67 6f72 6974  plitting Algorit
+00002900: 686d 730a 5768 696c 6520 6d75 6368 206d  hms.While much m
+00002910: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+00002920: 6973 2064 6f6e 6520 7769 7468 2061 2072  is done with a r
+00002930: 616e 646f 6d20 6368 6f69 6365 2062 6574  andom choice bet
+00002940: 7765 656e 2074 7261 696e 696e 672f 7661  ween training/va
+00002950: 6c69 6461 7469 6f6e 2f74 6573 7420 6461  lidation/test da
+00002960: 7461 2c20 616e 2061 6c74 6572 6e61 7469  ta, an alternati
+00002970: 7665 2069 7320 7468 6520 7573 6520 6f66  ve is the use of
+00002980: 2073 6f2d 6361 6c6c 6564 2022 7261 7469   so-called "rati
+00002990: 6f6e 616c 2220 7370 6c69 7474 696e 6720  onal" splitting 
+000029a0: 616c 676f 7269 7468 6d73 2e0a 5468 6573  algorithms..Thes
+000029b0: 6520 6170 7072 6f61 6368 6573 2075 7365  e approaches use
+000029c0: 2073 6f6d 6520 7369 6d69 6c61 7269 7479   some similarity
+000029d0: 2d62 6173 6564 2061 6c67 6f72 6974 686d  -based algorithm
+000029e0: 2074 6f20 6469 7669 6465 2064 6174 6120   to divide data 
+000029f0: 696e 746f 2073 6574 732e 0a53 6f6d 6520  into sets..Some 
+00002a00: 6f66 2074 6865 7365 2061 6c67 6f72 6974  of these algorit
+00002a10: 686d 7320 696e 636c 7564 6520 4b65 6e6e  hms include Kenn
+00002a20: 6172 642d 5374 6f6e 6520 285b 4b65 6e6e  ard-Stone ([Kenn
+00002a30: 6172 6420 2620 5374 6f6e 655d 2868 7474  ard & Stone](htt
+00002a40: 7073 3a2f 2f77 7777 2e74 616e 6466 6f6e  ps://www.tandfon
+00002a50: 6c69 6e65 2e63 6f6d 2f64 6f69 2f61 6273  line.com/doi/abs
+00002a60: 2f31 302e 3130 3830 2f30 3034 3031 3730  /10.1080/0040170
+00002a70: 362e 3139 3639 2e31 3034 3930 3636 3629  6.1969.10490666)
+00002a80: 203a 736d 616c 6c5f 626c 7565 5f64 6961   :small_blue_dia
+00002a90: 6d6f 6e64 3a29 2c20 5370 6865 7265 2045  mond:), Sphere E
+00002aa0: 7863 6c75 7369 6f6e 2028 5b54 726f 7073  xclusion ([Trops
+00002ab0: 6861 2065 742e 2061 6c5d 2868 7474 7073  ha et. al](https
+00002ac0: 3a2f 2f70 7562 732e 6163 732e 6f72 672f  ://pubs.acs.org/
+00002ad0: 646f 692f 7064 662f 3130 2e31 3032 312f  doi/pdf/10.1021/
+00002ae0: 6369 3330 3033 3338 7729 203a 736d 616c  ci300338w) :smal
+00002af0: 6c5f 626c 7565 5f64 6961 6d6f 6e64 3a29  l_blue_diamond:)
+00002b00: 2c61 7320 7765 6c6c 2061 7320 7468 6520  ,as well as the 
+00002b10: 4f70 7469 5369 6d20 6173 2064 6973 6375  OptiSim as discu
+00002b20: 7373 6564 2069 6e20 5b41 7070 6c69 6564  ssed in [Applied
+00002b30: 2043 6865 6d6f 696e 666f 726d 6174 6963   Chemoinformatic
+00002b40: 733a 2041 6368 6965 7665 6d65 6e74 7320  s: Achievements 
+00002b50: 616e 6420 4675 7475 7265 204f 7070 6f72  and Future Oppor
+00002b60: 7475 6e69 7469 6573 5d28 6874 7470 733a  tunities](https:
+00002b70: 2f2f 7777 772e 7769 6c65 792e 636f 6d2f  //www.wiley.com/
+00002b80: 656e 2d75 732f 4170 706c 6965 642b 4368  en-us/Applied+Ch
+00002b90: 656d 6f69 6e66 6f72 6d61 7469 6373 2533  emoinformatics%3
+00002ba0: 412b 4163 6869 6576 656d 656e 7473 2b61  A+Achievements+a
+00002bb0: 6e64 2b46 7574 7572 652b 4f70 706f 7274  nd+Future+Opport
+00002bc0: 756e 6974 6965 732d 702d 3937 3833 3532  unities-p-978352
+00002bd0: 3738 3036 3534 3629 203a 736d 616c 6c5f  7806546) :small_
+00002be0: 626c 7565 5f64 6961 6d6f 6e64 3a2e 0a53  blue_diamond:..S
+00002bf0: 6f6d 6520 636c 7573 7465 7269 6e67 2d62  ome clustering-b
+00002c00: 6173 6564 2073 706c 6974 7469 6e67 2074  ased splitting t
+00002c10: 6563 686e 6971 7565 7320 6861 7665 2061  echniques have a
+00002c20: 6c73 6f20 6265 656e 2069 6e63 6f72 706f  lso been incorpo
+00002c30: 7261 7465 642c 2073 7563 6820 6173 205b  rated, such as [
+00002c40: 4442 5343 414e 5d28 6874 7470 3a2f 2f63  DBSCAN](http://c
+00002c50: 6974 6573 6565 7278 2e69 7374 2e70 7375  iteseerx.ist.psu
+00002c60: 2e65 6475 2f76 6965 7764 6f63 2f64 6f77  .edu/viewdoc/dow
+00002c70: 6e6c 6f61 643f 646f 693d 3130 2e31 2e31  nload?doi=10.1.1
+00002c80: 2e31 3031 362e 3839 3026 7265 703d 7265  .1016.890&rep=re
+00002c90: 7031 2674 7970 653d 7064 6629 2e0a 0a54  p1&type=pdf)...T
+00002ca0: 6865 7265 2061 7265 2074 776f 2062 726f  here are two bro
+00002cb0: 6164 2063 6174 6567 6f72 6965 7320 6f66  ad categories of
+00002cc0: 2073 616d 706c 696e 6720 616c 676f 7269   sampling algori
+00002cd0: 7468 6d73 2069 6d70 6c65 6d65 6e74 6564  thms implemented
+00002ce0: 2069 6e20 6061 7374 6172 7465 7360 3a20   in `astartes`: 
+00002cf0: 6578 7472 6170 6f6c 6174 6976 6520 616e  extrapolative an
+00002d00: 6420 696e 7465 7270 6f6c 6174 6976 652e  d interpolative.
+00002d10: 0a54 6865 2066 6f72 6d65 7220 7769 6c6c  .The former will
+00002d20: 2066 6f72 6365 2079 6f75 7220 6d6f 6465   force your mode
+00002d30: 6c20 746f 2070 7265 6469 6374 206f 6e20  l to predict on 
+00002d40: 6f75 742d 6f66 2d73 616d 706c 6520 6461  out-of-sample da
+00002d50: 7461 2c20 7768 6963 6820 6372 6561 7465  ta, which create
+00002d60: 7320 6120 6d6f 7265 2063 6861 6c6c 656e  s a more challen
+00002d70: 6769 6e67 2074 6173 6b20 7468 616e 2069  ging task than i
+00002d80: 6e74 6572 706f 6c61 7469 7665 2073 616d  nterpolative sam
+00002d90: 706c 696e 672e 0a53 6565 2074 6865 2074  pling..See the t
+00002da0: 6162 6c65 2062 656c 6f77 2066 6f72 2061  able below for a
+00002db0: 6c6c 206f 6620 7468 6520 7361 6d70 6c69  ll of the sampli
+00002dc0: 6e67 2061 7070 726f 6163 6865 7320 6375  ng approaches cu
+00002dd0: 7272 656e 746c 7920 696d 706c 656d 656e  rrently implemen
+00002de0: 7465 6420 696e 2060 6173 7461 7274 6573  ted in `astartes
+00002df0: 602c 2061 7320 7765 6c6c 2061 7320 7468  `, as well as th
+00002e00: 6520 6879 7065 7270 6172 616d 6574 6572  e hyperparameter
+00002e10: 7320 7468 6174 2065 6163 6820 616c 676f  s that each algo
+00002e20: 7269 7468 6d20 6163 6365 7074 7320 2877  rithm accepts (w
+00002e30: 6869 6368 2061 7265 2070 6173 7365 6420  hich are passed 
+00002e40: 696e 2077 6974 6820 6068 6f70 7473 6029  in with `hopts`)
+00002e50: 2061 6e64 2061 2068 656c 7066 756c 2072   and a helpful r
+00002e60: 6566 6572 656e 6365 2066 6f72 2075 6e64  eference for und
+00002e70: 6572 7374 616e 6469 6e67 2068 6f77 2074  erstanding how t
+00002e80: 6865 2068 7970 6572 7061 7261 6d65 7465  he hyperparamete
+00002e90: 7273 2077 6f72 6b2e 0a4e 6f74 6520 7468  rs work..Note th
+00002ea0: 6174 2060 7261 6e64 6f6d 5f73 7461 7465  at `random_state
+00002eb0: 6020 6973 2064 6566 696e 6564 2061 7320  ` is defined as 
+00002ec0: 6120 6b65 7977 6f72 6420 6172 6775 6d65  a keyword argume
+00002ed0: 6e74 2069 6e20 6074 7261 696e 5f74 6573  nt in `train_tes
+00002ee0: 745f 7370 6c69 7460 2069 7473 656c 662c  t_split` itself,
+00002ef0: 2065 7665 6e20 7468 6f75 6768 2074 6865   even though the
+00002f00: 7365 2061 6c67 6f72 6974 686d 7320 7769  se algorithms wi
+00002f10: 6c6c 2075 7365 2074 6865 2060 7261 6e64  ll use the `rand
+00002f20: 6f6d 5f73 7461 7465 6020 696e 2074 6865  om_state` in the
+00002f30: 6972 206f 776e 2077 6f72 6b2e 0a44 6f20  ir own work..Do 
+00002f40: 6e6f 7420 7072 6f76 6964 6520 6120 6072  not provide a `r
+00002f50: 616e 646f 6d5f 7374 6174 6560 2069 6e20  andom_state` in 
+00002f60: 7468 6520 6068 6f70 7473 6020 6469 6374  the `hopts` dict
+00002f70: 696f 6e61 7279 202d 2069 7420 7769 6c6c  ionary - it will
+00002f80: 2062 6520 6f76 6572 7772 6974 7465 6e20   be overwritten 
+00002f90: 6279 2074 6865 2060 7261 6e64 6f6d 5f73  by the `random_s
+00002fa0: 7461 7465 6020 796f 7520 7072 6f76 6964  tate` you provid
+00002fb0: 6520 666f 7220 6074 7261 696e 5f74 6573  e for `train_tes
+00002fc0: 745f 7370 6c69 7460 2028 6f72 2074 6865  t_split` (or the
+00002fd0: 2064 6566 6175 6c74 2069 6620 6e6f 6e65   default if none
+00002fe0: 2069 7320 7072 6f76 6964 6564 292e 0a0a   is provided)...
+00002ff0: 2323 2323 2049 6d70 6c65 6d65 6e74 6564  #### Implemented
+00003000: 2053 616d 706c 696e 6720 416c 676f 7269   Sampling Algori
+00003010: 7468 6d73 0a0a 7c20 5361 6d70 6c65 7220  thms..| Sampler 
+00003020: 4e61 6d65 207c 2055 7361 6765 2053 7472  Name | Usage Str
+00003030: 696e 6720 7c20 5479 7065 207c 2048 7970  ing | Type | Hyp
+00003040: 6572 7061 7261 6d65 7465 7273 207c 2052  erparameters | R
+00003050: 6566 6572 656e 6365 207c 204e 6f74 6573  eference | Notes
+00003060: 207c 0a7c 3a2d 2d2d 3a7c 2d2d 2d7c 2d2d   |.|:---:|---|--
+00003070: 2d7c 2d2d 2d7c 2d2d 2d7c 2d2d 2d7c 0a7c  -|---|---|---|.|
+00003080: 2052 616e 646f 6d20 7c20 2772 616e 646f   Random | 'rando
+00003090: 6d27 207c 2049 6e74 6572 706f 6c61 7469  m' | Interpolati
+000030a0: 7665 207c 2060 7368 7566 666c 6560 207c  ve | `shuffle` |
+000030b0: 205b 736b 6c65 6172 6e20 7472 6169 6e5f   [sklearn train_
+000030c0: 7465 7374 5f73 706c 6974 5d28 6874 7470  test_split](http
+000030d0: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
+000030e0: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
+000030f0: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
+00003100: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
+00003110: 6374 696f 6e2e 7472 6169 6e5f 7465 7374  ction.train_test
+00003120: 5f73 706c 6974 2e68 746d 6c29 2044 6f63  _split.html) Doc
+00003130: 756d 656e 7461 7469 6f6e 207c 2054 6869  umentation | Thi
+00003140: 7320 7361 6d70 6c65 7220 6973 2061 2064  s sampler is a d
+00003150: 6972 6563 7420 7061 7373 7468 726f 7567  irect passthroug
+00003160: 6820 746f 2060 736b 6c65 6172 6e60 2773  h to `sklearn`'s
+00003170: 2060 7472 6169 6e5f 7465 7374 5f73 706c   `train_test_spl
+00003180: 6974 602e 207c 0a7c 204b 656e 6e61 7264  it`. |.| Kennard
+00003190: 2d53 746f 6e65 207c 2027 6b65 6e6e 6172  -Stone | 'kennar
+000031a0: 645f 7374 6f6e 6527 207c 2049 6e74 6572  d_stone' | Inter
+000031b0: 706f 6c61 7469 7665 207c 2060 6d65 7472  polative | `metr
+000031c0: 6963 6020 7c20 4f72 6967 696e 616c 2050  ic` | Original P
+000031d0: 6170 6572 2062 7920 5b4b 656e 6e61 7264  aper by [Kennard
+000031e0: 2026 2053 746f 6e65 5d28 6874 7470 733a   & Stone](https:
+000031f0: 2f2f 7777 772e 7461 6e64 666f 6e6c 696e  //www.tandfonlin
+00003200: 652e 636f 6d2f 646f 692f 6162 732f 3130  e.com/doi/abs/10
+00003210: 2e31 3038 302f 3030 3430 3137 3036 2e31  .1080/00401706.1
+00003220: 3936 392e 3130 3439 3036 3636 2920 3a73  969.10490666) :s
+00003230: 6d61 6c6c 5f62 6c75 655f 6469 616d 6f6e  mall_blue_diamon
+00003240: 643a 207c 2045 7563 6c69 6469 616e 2064  d: | Euclidian d
+00003250: 6973 7461 6e63 6520 6973 2075 7365 6420  istance is used 
+00003260: 6279 2064 6566 6175 6c74 2c20 6173 2064  by default, as d
+00003270: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+00003280: 6f72 6967 696e 616c 2070 6170 6572 2e20  original paper. 
+00003290: 7c0a 7c20 5361 6d70 6c65 2073 6574 2050  |.| Sample set P
+000032a0: 6172 7469 7469 6f6e 696e 6720 6261 7365  artitioning base
+000032b0: 6420 6f6e 206a 6f69 6e74 2058 2d59 2064  d on joint X-Y d
+000032c0: 6973 7461 6e63 6573 2028 5350 5859 2920  istances (SPXY) 
+000032d0: 7c20 2773 7078 7927 207c 2049 6e74 6572  | 'spxy' | Inter
+000032e0: 706f 6c61 7469 7665 207c 2060 6469 7374  polative | `dist
+000032f0: 616e 6365 5f6d 6574 7269 6360 207c 2053  ance_metric` | S
+00003300: 616c 6468 616e 6120 6574 2e20 616c 205b  aldhana et. al [
+00003310: 6f72 6967 696e 616c 2070 6170 6572 5d28  original paper](
+00003320: 6874 7470 733a 2f2f 7777 772e 7363 6965  https://www.scie
+00003330: 6e63 6564 6972 6563 742e 636f 6d2f 7363  ncedirect.com/sc
+00003340: 6965 6e63 652f 6172 7469 636c 652f 6162  ience/article/ab
+00003350: 732f 7069 692f 5330 3033 3939 3134 3030  s/pii/S003991400
+00003360: 3530 3031 3932 5829 203a 736d 616c 6c5f  500192X) :small_
+00003370: 626c 7565 5f64 6961 6d6f 6e64 3a20 7c20  blue_diamond: | 
+00003380: 4578 7465 6e73 696f 6e20 6f66 204b 656e  Extension of Ken
+00003390: 6e61 7264 2053 746f 6e65 2074 6861 7420  nard Stone that 
+000033a0: 616c 736f 2069 6e63 6c75 6465 7320 7468  also includes th
+000033b0: 6520 7265 7370 6f6e 7365 2077 6865 6e20  e response when 
+000033c0: 7361 6d70 6c69 6e67 2064 6973 7461 6e63  sampling distanc
+000033d0: 6573 2e20 7c0a 7c20 5363 6166 666f 6c64  es. |.| Scaffold
+000033e0: 207c 2027 7363 6166 666f 6c64 2720 7c20   | 'scaffold' | 
+000033f0: 4578 7472 6170 6f6c 6174 6976 6520 7c20  Extrapolative | 
+00003400: 6069 6e63 6c75 6465 5f63 6869 7261 6c69  `include_chirali
+00003410: 7479 6020 7c20 5b42 656d 6973 2d4d 7572  ty` | [Bemis-Mur
+00003420: 636b 6f20 5363 6166 666f 6c64 5d28 6874  cko Scaffold](ht
+00003430: 7470 733a 2f2f 7075 6273 2e61 6373 2e6f  tps://pubs.acs.o
+00003440: 7267 2f64 6f69 2f66 756c 6c2f 3130 2e31  rg/doi/full/10.1
+00003450: 3032 312f 6a6d 3936 3032 3932 3829 203a  021/jm9602928) :
+00003460: 736d 616c 6c5f 626c 7565 5f64 6961 6d6f  small_blue_diamo
+00003470: 6e64 3a20 6173 2069 6d70 6c65 6d65 6e74  nd: as implement
+00003480: 6564 2069 6e20 5244 4b69 7420 7c20 5468  ed in RDKit | Th
+00003490: 6973 2073 616d 706c 6572 2072 6571 7569  is sampler requi
+000034a0: 7265 7320 534d 494c 4553 2073 7472 696e  res SMILES strin
+000034b0: 6773 2061 7320 696e 7075 7420 2875 7365  gs as input (use
+000034c0: 2074 6865 2060 6d6f 6c65 6375 6c65 7360   the `molecules`
+000034d0: 2073 7562 7061 636b 6167 6529 207c 0a7c   subpackage) |.|
+000034e0: 2053 7068 6572 6520 4578 636c 7573 696f   Sphere Exclusio
+000034f0: 6e20 7c20 2773 7068 6572 655f 6578 636c  n | 'sphere_excl
+00003500: 7573 696f 6e27 207c 2045 7874 7261 706f  usion' | Extrapo
+00003510: 6c61 7469 7665 207c 2060 6d65 7472 6963  lative | `metric
+00003520: 602c 2060 6469 7374 616e 6365 5f63 7574  `, `distance_cut
+00003530: 6f66 6660 207c 205f 6375 7374 6f6d 2069  off` | _custom i
+00003540: 6d70 6c65 6d65 6e74 6174 696f 6e5f 207c  mplementation_ |
+00003550: 2056 6172 6961 7469 6f6e 206f 6e20 5370   Variation on Sp
+00003560: 6865 7265 2045 7863 6c75 7369 6f6e 2066  here Exclusion f
+00003570: 6f72 2061 7262 6974 7261 7279 2d76 616c  or arbitrary-val
+00003580: 7565 6420 7665 6374 6f72 732e 207c 0a7c  ued vectors. |.|
+00003590: 2054 696d 6520 4261 7365 6420 7c20 2774   Time Based | 't
+000035a0: 696d 655f 6261 7365 6427 207c 2045 7874  ime_based' | Ext
+000035b0: 7261 706f 6c61 7469 7665 207c 205f 6e6f  rapolative | _no
+000035c0: 6e65 5f20 7c20 5061 7065 7273 2075 7369  ne_ | Papers usi
+000035d0: 6e67 2054 696d 6520 6261 7365 6420 7370  ng Time based sp
+000035e0: 6c69 7474 696e 673a 205b 4368 656e 2065  litting: [Chen e
+000035f0: 7420 616c 2e5d 2868 7474 7073 3a2f 2f70  t al.](https://p
+00003600: 7562 732e 6163 732e 6f72 672f 646f 692f  ubs.acs.org/doi/
+00003610: 6675 6c6c 2f31 302e 3130 3231 2f63 6932  full/10.1021/ci2
+00003620: 3030 3631 3568 2920 3a73 6d61 6c6c 5f62  00615h) :small_b
+00003630: 6c75 655f 6469 616d 6f6e 643a 2c20 5b53  lue_diamond:, [S
+00003640: 6865 7269 6461 6e2c 2052 2e20 505d 2868  heridan, R. P](h
+00003650: 7474 7073 3a2f 2f70 7562 732e 6163 732e  ttps://pubs.acs.
+00003660: 6f72 672f 646f 692f 6675 6c6c 2f31 302e  org/doi/full/10.
+00003670: 3130 3231 2f63 6934 3030 3038 346b 2920  1021/ci400084k) 
+00003680: 3a73 6d61 6c6c 5f62 6c75 655f 6469 616d  :small_blue_diam
+00003690: 6f6e 643a 2c20 5b46 6569 6e62 6572 6720  ond:, [Feinberg 
+000036a0: 6574 2061 6c2e 5d28 6874 7470 733a 2f2f  et al.](https://
+000036b0: 7075 6273 2e61 6373 2e6f 7267 2f64 6f69  pubs.acs.org/doi
+000036c0: 2f66 756c 6c2f 3130 2e31 3032 312f 6163  /full/10.1021/ac
+000036d0: 732e 6a6d 6564 6368 656d 2e39 6230 3231  s.jmedchem.9b021
+000036e0: 3837 2920 3a73 6d61 6c6c 5f62 6c75 655f  87) :small_blue_
+000036f0: 6469 616d 6f6e 643a 2c20 5b53 7472 7562  diamond:, [Strub
+00003700: 6c65 2065 7420 616c 2e5d 2868 7474 7073  le et al.](https
+00003710: 3a2f 2f70 7562 732e 7273 632e 6f72 672f  ://pubs.rsc.org/
+00003720: 656e 2f63 6f6e 7465 6e74 2f61 7274 6963  en/content/artic
+00003730: 6c65 6874 6d6c 2f32 3032 302f 7265 2f64  lehtml/2020/re/d
+00003740: 3072 6530 3030 3731 6a29 207c 2054 6869  0re00071j) | Thi
+00003750: 7320 7361 6d70 6c65 7220 7265 7175 6972  s sampler requir
+00003760: 6573 2060 6c61 6265 6c73 6020 746f 2062  es `labels` to b
+00003770: 6520 616e 2069 7465 7261 626c 6520 6f66  e an iterable of
+00003780: 2065 6974 6865 7220 6461 7465 206f 7220   either date or 
+00003790: 6461 7465 7469 6d65 206f 626a 6563 7473  datetime objects
+000037a0: 2e20 7c0a 7c20 4f70 7469 6d69 7a61 626c  . |.| Optimizabl
+000037b0: 6520 4b2d 4469 7373 696d 696c 6172 6974  e K-Dissimilarit
+000037c0: 7920 5365 6c65 6374 696f 6e20 284f 7074  y Selection (Opt
+000037d0: 6953 696d 2920 7c20 276f 7074 6973 696d  iSim) | 'optisim
+000037e0: 2720 7c20 4578 7472 6170 6f6c 6174 6976  ' | Extrapolativ
+000037f0: 6520 7c20 606e 5f63 6c75 7374 6572 7360  e | `n_clusters`
+00003800: 2c20 606d 6178 5f73 7562 7361 6d70 6c65  , `max_subsample
+00003810: 5f73 697a 6560 2c20 6064 6973 7461 6e63  _size`, `distanc
+00003820: 655f 6375 746f 6666 6020 7c20 5f63 7573  e_cutoff` | _cus
+00003830: 746f 6d20 696d 706c 656d 656e 7461 7469  tom implementati
+00003840: 6f6e 5f20 7c20 5661 7269 6174 696f 6e20  on_ | Variation 
+00003850: 6f6e 205b 4f70 7469 5369 6d5d 2868 7474  on [OptiSim](htt
+00003860: 7073 3a2f 2f70 7562 732e 6163 732e 6f72  ps://pubs.acs.or
+00003870: 672f 646f 692f 3130 2e31 3032 312f 6369  g/doi/10.1021/ci
+00003880: 3032 3536 3632 6829 2066 6f72 2061 7262  025662h) for arb
+00003890: 6974 7261 7279 2d76 616c 7565 6420 7665  itrary-valued ve
+000038a0: 6374 6f72 732e 207c 0a7c 204b 2d4d 6561  ctors. |.| K-Mea
+000038b0: 6e73 207c 2027 6b6d 6561 6e73 2720 7c20  ns | 'kmeans' | 
+000038c0: 4578 7472 6170 6f6c 6174 6976 6520 7c20  Extrapolative | 
+000038d0: 606e 5f63 6c75 7374 6572 7360 2c20 606e  `n_clusters`, `n
+000038e0: 5f69 6e69 7460 207c 205b 6073 6b6c 6561  _init` | [`sklea
+000038f0: 726e 204b 4d65 616e 7360 5d28 6874 7470  rn KMeans`](http
+00003900: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
+00003910: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
+00003920: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
+00003930: 6c65 6172 6e2e 636c 7573 7465 722e 4b4d  learn.cluster.KM
+00003940: 6561 6e73 2e68 746d 6c29 207c 2050 6173  eans.html) | Pas
+00003950: 7374 6872 6f75 6768 2074 6f20 6073 6b6c  sthrough to `skl
+00003960: 6561 726e 6027 7320 604b 4d65 616e 7360  earn`'s `KMeans`
+00003970: 2e20 7c0a 7c20 4465 6e73 6974 792d 4261  . |.| Density-Ba
+00003980: 7365 6420 5370 6174 6961 6c20 436c 7573  sed Spatial Clus
+00003990: 7465 7269 6e67 206f 6620 4170 706c 6963  tering of Applic
+000039a0: 6174 696f 6e73 2077 6974 6820 4e6f 6973  ations with Nois
+000039b0: 6520 2844 4253 4341 4e29 207c 2027 6462  e (DBSCAN) | 'db
+000039c0: 7363 616e 2720 7c20 4578 7472 6170 6f6c  scan' | Extrapol
+000039d0: 6174 6976 6520 7c20 6065 7073 602c 2060  ative | `eps`, `
+000039e0: 6d69 6e5f 7361 6d70 6c65 7360 2c20 6061  min_samples`, `a
+000039f0: 6c67 6f72 6974 686d 602c 2060 6d65 7472  lgorithm`, `metr
+00003a00: 6963 602c 2060 6c65 6166 5f73 697a 6560  ic`, `leaf_size`
+00003a10: 207c 205b 6073 6b6c 6561 726e 2044 4253   | [`sklearn DBS
+00003a20: 4341 4e60 5d28 6874 7470 733a 2f2f 7363  CAN`](https://sc
+00003a30: 696b 6974 2d6c 6561 726e 2e6f 7267 2f73  ikit-learn.org/s
+00003a40: 7461 626c 652f 6d6f 6475 6c65 732f 6765  table/modules/ge
+00003a50: 6e65 7261 7465 642f 736b 6c65 6172 6e2e  nerated/sklearn.
+00003a60: 636c 7573 7465 722e 4442 5343 414e 2e68  cluster.DBSCAN.h
+00003a70: 746d 6c29 2044 6f63 756d 656e 7461 7469  tml) Documentati
+00003a80: 6f6e 7c20 5061 7373 7468 726f 7567 6820  on| Passthrough 
+00003a90: 746f 2060 736b 6c65 6172 6e60 2773 2060  to `sklearn`'s `
+00003aa0: 4442 5343 414e 602e 207c 0a7c 204d 696e  DBSCAN`. |.| Min
+00003ab0: 696d 756d 2054 6573 7420 5365 7420 4469  imum Test Set Di
+00003ac0: 7373 696d 696c 6172 6974 7920 284d 5453  ssimilarity (MTS
+00003ad0: 4429 207c 207e 207c 207e 207c 205f 7570  D) | ~ | ~ | _up
+00003ae0: 636f 6d69 6e67 2069 6e5f 2060 6173 7461  coming in_ `asta
+00003af0: 7274 6573 6020 5f76 312e 785f 207c 207e  rtes` _v1.x_ | ~
+00003b00: 207c 207e 207c 0a7c 2052 6573 7472 6963   | ~ |.| Restric
+00003b10: 7465 6420 426f 6c74 7a6d 616e 6e20 4d61  ted Boltzmann Ma
+00003b20: 6368 696e 6520 2852 424d 2920 7c20 7e20  chine (RBM) | ~ 
+00003b30: 7c20 7e20 7c20 5f75 7063 6f6d 696e 6720  | ~ | _upcoming 
+00003b40: 696e 5f20 6061 7374 6172 7465 7360 205f  in_ `astartes` _
+00003b50: 7631 2e78 5f20 7c20 7e20 7c20 7e20 7c0a  v1.x_ | ~ | ~ |.
+00003b60: 7c20 4b6f 686f 6e65 6e20 5365 6c66 2d4f  | Kohonen Self-O
+00003b70: 7267 616e 697a 696e 6720 4d61 7020 2853  rganizing Map (S
+00003b80: 4f4d 2920 7c20 7e20 7c20 7e20 7c20 5f75  OM) | ~ | ~ | _u
+00003b90: 7063 6f6d 696e 6720 696e 5f20 6061 7374  pcoming in_ `ast
+00003ba0: 6172 7465 7360 205f 7631 2e78 5f20 7c20  artes` _v1.x_ | 
+00003bb0: 7e20 7c20 7e20 7c0a 7c20 5350 6c69 7420  ~ | ~ |.| SPlit 
+00003bc0: 4d65 7468 6f64 207c 207e 207c 207e 207c  Method | ~ | ~ |
+00003bd0: 205f 7570 636f 6d69 6e67 2069 6e5f 2060   _upcoming in_ `
+00003be0: 6173 7461 7274 6573 6020 5f76 312e 785f  astartes` _v1.x_
+00003bf0: 207c 207e 207c 207e 207c 0a0a 2323 2320   | ~ | ~ |..### 
+00003c00: 446f 6d61 696e 2d53 7065 6369 6669 6320  Domain-Specific 
+00003c10: 4170 706c 6963 6174 696f 6e73 0a42 656c  Applications.Bel
+00003c20: 6f77 2061 7265 2073 6f6d 6520 6669 656c  ow are some fiel
+00003c30: 6420 7370 6563 6966 6963 2061 7070 6c69  d specific appli
+00003c40: 6361 7469 6f6e 7320 6f66 2060 6173 7461  cations of `asta
+00003c50: 7274 6573 602e 2049 6e74 6572 6573 7465  rtes`. Intereste
+00003c60: 6420 696e 2061 6464 696e 6720 6120 6e65  d in adding a ne
+00003c70: 7720 7361 6d70 6c69 6e67 2061 6c67 6f72  w sampling algor
+00003c80: 6974 686d 206f 7220 6665 6174 7572 697a  ithm or featuriz
+00003c90: 6174 696f 6e20 6170 7072 6f61 6368 3f20  ation approach? 
+00003ca0: 5365 6520 5b60 434f 4e54 5249 4255 5449  See [`CONTRIBUTI
+00003cb0: 4e47 2e6d 6460 5d28 2e2f 434f 4e54 5249  NG.md`](./CONTRI
+00003cc0: 4255 5449 4e47 2e6d 6429 2e0a 0a23 2323  BUTING.md)...###
+00003cd0: 2320 4368 656d 6963 616c 2044 6174 6120  # Chemical Data 
+00003ce0: 616e 6420 7468 6520 6061 7374 6172 7465  and the `astarte
+00003cf0: 732e 6d6f 6c65 6375 6c65 7360 2053 7562  s.molecules` Sub
+00003d00: 7061 636b 6167 650a 4d61 6368 696e 6520  package.Machine 
+00003d10: 4c65 6172 6e69 6e67 2069 7320 656e 6f72  Learning is enor
+00003d20: 6d6f 7573 6c79 2075 7365 6675 6c20 696e  mously useful in
+00003d30: 2063 6865 6d69 7374 7279 2d72 656c 6174   chemistry-relat
+00003d40: 6564 2066 6965 6c64 7320 6475 6520 746f  ed fields due to
+00003d50: 2074 6865 2068 6967 682d 6469 6d65 6e73   the high-dimens
+00003d60: 696f 6e61 6c20 6665 6174 7572 6520 7370  ional feature sp
+00003d70: 6163 6520 6f66 2063 6865 6d69 6361 6c20  ace of chemical 
+00003d80: 6461 7461 2e0a 546f 2070 726f 7065 726c  data..To properl
+00003d90: 7920 6170 706c 7920 4d4c 2074 6f20 6368  y apply ML to ch
+00003da0: 656d 6963 616c 2064 6174 6120 666f 7220  emical data for 
+00003db0: 696e 6665 7265 6e63 6520 5f6f 725f 2064  inference _or_ d
+00003dc0: 6973 636f 7665 7279 2c20 6974 2069 7320  iscovery, it is 
+00003dd0: 696d 706f 7274 616e 7420 746f 206b 6e6f  important to kno
+00003de0: 7720 6120 6d6f 6465 6c27 7320 6163 6375  w a model's accu
+00003df0: 7261 6379 2075 6e64 6572 2074 6865 2074  racy under the t
+00003e00: 776f 2064 6f6d 6169 6e73 2e0a 546f 2073  wo domains..To s
+00003e10: 696d 706c 6966 7920 7468 6520 7072 6f63  implify the proc
+00003e20: 6573 7320 6f66 2070 6172 7469 7469 6f6e  ess of partition
+00003e30: 696e 6720 6368 656d 6963 616c 2064 6174  ing chemical dat
+00003e40: 612c 2060 6173 7461 7274 6573 6020 696d  a, `astartes` im
+00003e50: 706c 656d 656e 7473 2061 2070 7265 2d62  plements a pre-b
+00003e60: 7569 6c74 2066 6561 7475 7269 7a65 7220  uilt featurizer 
+00003e70: 666f 7220 636f 6d6d 6f6e 2063 6865 6d69  for common chemi
+00003e80: 7374 7279 2064 6174 6120 666f 726d 6174  stry data format
+00003e90: 732e 0a41 6674 6572 2069 6e73 7461 6c6c  s..After install
+00003ea0: 696e 6720 7769 7468 2060 7069 7020 696e  ing with `pip in
+00003eb0: 7374 616c 6c20 6173 7461 7274 6573 5b6d  stall astartes[m
+00003ec0: 6f6c 6563 756c 6573 5d60 206f 6e65 2063  olecules]` one c
+00003ed0: 616e 2069 6d70 6f72 7420 7468 6520 6e65  an import the ne
+00003ee0: 7720 7472 6169 6e2f 7465 7374 2073 706c  w train/test spl
+00003ef0: 6974 7469 6e67 2066 756e 6374 696f 6e20  itting function 
+00003f00: 6c69 6b65 2074 6869 733a 2060 6672 6f6d  like this: `from
+00003f10: 2061 7374 6172 7465 732e 6d6f 6c65 6375   astartes.molecu
+00003f20: 6c65 7320 696d 706f 7274 2074 7261 696e  les import train
+00003f30: 5f74 6573 745f 7370 6c69 745f 6d6f 6c65  _test_split_mole
+00003f40: 6375 6c65 7360 0a0a 5468 6520 7573 6167  cules`..The usag
+00003f50: 6520 6f66 2074 6869 7320 6675 6e63 7469  e of this functi
+00003f60: 6f6e 2069 7320 6964 656e 7469 6361 6c20  on is identical 
+00003f70: 746f 2060 7472 6169 6e5f 7465 7374 5f73  to `train_test_s
+00003f80: 706c 6974 6020 6275 7420 7769 7468 2074  plit` but with t
+00003f90: 6865 2061 6464 6974 696f 6e20 6f66 206e  he addition of n
+00003fa0: 6577 2061 7267 756d 656e 7473 2074 6f20  ew arguments to 
+00003fb0: 636f 6e74 726f 6c20 686f 7720 7468 6520  control how the 
+00003fc0: 6d6f 6c65 6375 6c65 7320 6172 6520 6665  molecules are fe
+00003fd0: 6174 7572 697a 6564 3a0a 0a60 6060 7079  aturized:..```py
+00003fe0: 7468 6f6e 0a74 7261 696e 5f74 6573 745f  thon.train_test_
+00003ff0: 7370 6c69 745f 6d6f 6c65 6375 6c65 7328  split_molecules(
+00004000: 0a20 2020 206d 6f6c 6563 756c 6573 3d73  .    molecules=s
+00004010: 6d69 6c65 732c 0a20 2020 2079 3d79 2c0a  miles,.    y=y,.
+00004020: 2020 2020 7465 7374 5f73 697a 653d 302e      test_size=0.
+00004030: 322c 0a20 2020 2074 7261 696e 5f73 697a  2,.    train_siz
+00004040: 653d 302e 382c 0a20 2020 2066 696e 6765  e=0.8,.    finge
+00004050: 7270 7269 6e74 3d22 6461 796c 6967 6874  rprint="daylight
+00004060: 5f66 696e 6765 7270 7269 6e74 222c 0a20  _fingerprint",. 
+00004070: 2020 2066 7072 696e 7473 5f68 6f70 7473     fprints_hopts
+00004080: 3d7b 0a20 2020 2020 2020 2022 6d69 6e50  ={.        "minP
+00004090: 6174 6822 3a20 322c 0a20 2020 2020 2020  ath": 2,.       
+000040a0: 2022 6d61 7850 6174 6822 3a20 352c 0a20   "maxPath": 5,. 
+000040b0: 2020 2020 2020 2022 6670 5369 7a65 223a         "fpSize":
+000040c0: 2032 3030 2c0a 2020 2020 2020 2020 2262   200,.        "b
+000040d0: 6974 7350 6572 4861 7368 223a 2034 2c0a  itsPerHash": 4,.
+000040e0: 2020 2020 2020 2020 2275 7365 4873 223a          "useHs":
+000040f0: 2031 2c0a 2020 2020 2020 2020 2274 6774   1,.        "tgt
+00004100: 4465 6e73 6974 7922 3a20 302e 342c 0a20  Density": 0.4,. 
+00004110: 2020 2020 2020 2022 6d69 6e53 697a 6522         "minSize"
+00004120: 3a20 3634 2c0a 2020 2020 7d2c 0a20 2020  : 64,.    },.   
+00004130: 2073 616d 706c 6572 3d22 7261 6e64 6f6d   sampler="random
+00004140: 222c 0a20 2020 2072 616e 646f 6d5f 7374  ",.    random_st
+00004150: 6174 653d 3432 2c0a 2020 2020 686f 7074  ate=42,.    hopt
+00004160: 733d 7b0a 2020 2020 2020 2020 2273 6875  s={.        "shu
+00004170: 6666 6c65 223a 2054 7275 652c 0a20 2020  ffle": True,.   
+00004180: 207d 2c0a 290a 6060 600a 0a54 6f20 7365   },.).```..To se
+00004190: 6520 6120 636f 6d70 6c65 7465 2065 7861  e a complete exa
+000041a0: 6d70 6c65 206f 6620 7573 696e 6720 6074  mple of using `t
+000041b0: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
+000041c0: 6d6f 6c65 6375 6c65 7360 2077 6974 6820  molecules` with 
+000041d0: 6163 7475 616c 2063 6865 6d69 6361 6c20  actual chemical 
+000041e0: 6461 7461 2c20 7461 6b65 2061 206c 6f6f  data, take a loo
+000041f0: 6b20 696e 2074 6865 2060 6578 616d 706c  k in the `exampl
+00004200: 6573 6020 6469 7265 6374 6f72 7920 616e  es` directory an
+00004210: 6420 7468 6520 6272 6965 6620 5b63 6f6d  d the brief [com
+00004220: 7061 6e69 6f6e 2070 6170 6572 5d28 6874  panion paper](ht
+00004230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004240: 2f4a 6163 6b73 6f6e 4275 726e 732f 6173  /JacksonBurns/as
+00004250: 7461 7274 6573 2f72 6177 2f6a 6f73 732d  tartes/raw/joss-
+00004260: 7061 7065 722f 4275 726e 732d 5370 6965  paper/Burns-Spie
+00004270: 6b65 726d 616e 6e2d 4268 6174 7461 6368  kermann-Bhattach
+00004280: 6172 6a65 655f 6173 7461 7274 6573 2e70  arjee_astartes.p
+00004290: 6466 292e 0a0a 436f 6e66 6967 7572 6174  df)...Configurat
+000042a0: 696f 6e20 6f70 7469 6f6e 7320 666f 7220  ion options for 
+000042b0: 7468 6520 6665 6174 7572 697a 6174 696f  the featurizatio
+000042c0: 6e20 7363 6865 6d65 2063 616e 2062 6520  n scheme can be 
+000042d0: 666f 756e 6420 696e 2074 6865 2064 6f63  found in the doc
+000042e0: 756d 656e 7461 7469 6f6e 2066 6f72 205b  umentation for [
+000042f0: 4149 4d53 696d 5d28 6874 7470 733a 2f2f  AIMSim](https://
+00004300: 766c 6163 686f 7367 726f 7570 2e67 6974  vlachosgroup.git
+00004310: 6875 622e 696f 2f41 494d 5369 6d2f 5245  hub.io/AIMSim/RE
+00004320: 4144 4d45 2e68 746d 6c23 6375 7272 656e  ADME.html#curren
+00004330: 746c 792d 696d 706c 656d 656e 7465 642d  tly-implemented-
+00004340: 6669 6e67 6572 7072 696e 7473 2920 7468  fingerprints) th
+00004350: 6f75 6768 206d 6f73 7420 6f66 2074 6865  ough most of the
+00004360: 2063 7269 7469 6361 6c20 636f 6e66 6967   critical config
+00004370: 7572 6174 696f 6e20 6f70 7469 6f6e 7320  uration options 
+00004380: 6172 6520 7368 6f77 6e20 6162 6f76 652e  are shown above.
+00004390: 0a0a 2323 2052 6570 726f 6475 6369 6269  ..## Reproducibi
+000043a0: 6c69 7479 0a60 6173 7461 7274 6573 6020  lity.`astartes` 
+000043b0: 6169 6d73 2074 6f20 6265 2063 6f6d 706c  aims to be compl
+000043c0: 6574 656c 7920 7265 7072 6f64 7563 6962  etely reproducib
+000043d0: 6c65 2061 6372 6f73 7320 6469 6666 6572  le across differ
+000043e0: 656e 7420 706c 6174 666f 726d 732c 2050  ent platforms, P
+000043f0: 7974 686f 6e20 7665 7273 696f 6e73 2c20  ython versions, 
+00004400: 616e 6420 6465 7065 6e64 656e 6379 2063  and dependency c
+00004410: 6f6e 6669 6775 7261 7469 6f6e 7320 2d20  onfigurations - 
+00004420: 616e 7920 7665 7273 696f 6e20 6f66 2060  any version of `
+00004430: 6173 7461 7274 6573 6020 7631 2e78 2073  astartes` v1.x s
+00004440: 686f 756c 6420 7265 7375 6c74 2069 6e20  hould result in 
+00004450: 7468 6520 5f65 7861 6374 5f20 7361 6d65  the _exact_ same
+00004460: 2073 706c 6974 732c 2061 6c77 6179 732e   splits, always.
+00004470: 0a54 6f20 7468 6174 2065 6e64 2c20 7468  .To that end, th
+00004480: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
+00004490: 6f72 206f 6620 6061 7374 6172 7465 7360  or of `astartes`
+000044a0: 2069 7320 746f 2075 7365 2060 3432 6020   is to use `42` 
+000044b0: 6173 2074 6865 2072 616e 646f 6d20 7365  as the random se
+000044c0: 6564 2061 6e64 205f 616c 7761 7973 5f20  ed and _always_ 
+000044d0: 7365 7420 6974 2e0a 5275 6e6e 696e 6720  set it..Running 
+000044e0: 6061 7374 6172 7465 7360 2077 6974 6820  `astartes` with 
+000044f0: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
+00004500: 696e 6773 2077 696c 6c20 616c 7761 7973  ings will always
+00004510: 2070 726f 6475 6365 2074 6865 2065 7861   produce the exa
+00004520: 6374 2073 616d 6520 7265 7375 6c74 732e  ct same results.
+00004530: 0a57 6520 6861 7665 2076 6572 6966 6965  .We have verifie
+00004540: 6420 7468 6973 2062 6568 6176 696f 7220  d this behavior 
+00004550: 6f6e 2044 6562 6961 6e20 5562 756e 7475  on Debian Ubuntu
+00004560: 2c20 5769 6e64 6f77 732c 2061 6e64 2049  , Windows, and I
+00004570: 6e74 656c 204d 6163 7320 6672 6f6d 2050  ntel Macs from P
+00004580: 7974 686f 6e20 7665 7273 696f 6e73 2033  ython versions 3
+00004590: 2e37 2074 6872 6f75 6768 2033 2e31 3120  .7 through 3.11 
+000045a0: 2877 6974 6820 6170 7072 6f70 7269 6174  (with appropriat
+000045b0: 6520 6465 7065 6e64 656e 6369 6573 2066  e dependencies f
+000045c0: 6f72 2065 6163 6820 7665 7273 696f 6e29  or each version)
+000045d0: 2e0a 0a23 2323 204b 6e6f 776e 2052 6570  ...### Known Rep
+000045e0: 726f 6475 6369 6269 6c69 7479 204c 696d  roducibility Lim
+000045f0: 6974 6174 696f 6e73 0a49 6e65 7669 7461  itations.Inevita
+00004600: 626c 7920 6578 7465 726e 616c 2064 6570  bly external dep
+00004610: 656e 6465 6e63 6965 7320 6f66 2060 6173  endencies of `as
+00004620: 7461 7274 6573 6020 7769 6c6c 2069 6e74  tartes` will int
+00004630: 726f 6475 6365 2062 6163 6b77 6172 6473  roduce backwards
+00004640: 2d69 6e63 6f6d 7061 7469 626c 6520 6368  -incompatible ch
+00004650: 616e 6765 732e 0a57 6520 636f 6e74 696e  anges..We contin
+00004660: 7561 6c6c 7920 7275 6e20 7265 6772 6573  ually run regres
+00004670: 7369 6f6e 2074 6573 7473 2074 6f20 6361  sion tests to ca
+00004680: 7463 6820 7468 6573 652c 2061 6e64 2077  tch these, and w
+00004690: 696c 6c20 6c69 7374 2061 6c6c 205f 6b6e  ill list all _kn
+000046a0: 6f77 6e5f 206c 696d 6974 6174 696f 6e73  own_ limitations
+000046b0: 2068 6572 653a 0a20 2d20 6073 6b6c 6561   here:. - `sklea
+000046c0: 726e 6020 7631 2e33 2e30 2069 6e74 726f  rn` v1.3.0 intro
+000046d0: 6475 6365 6420 6261 636b 7761 7264 732d  duced backwards-
+000046e0: 696e 636f 6d70 6174 6962 6c65 2063 6861  incompatible cha
+000046f0: 6e67 6573 2069 6e20 7468 6520 604b 4d65  nges in the `KMe
+00004700: 616e 7360 2073 616d 706c 6572 2074 6861  ans` sampler tha
+00004710: 7420 6368 616e 6765 6420 686f 7720 7468  t changed how th
+00004720: 6520 7261 6e64 6f6d 2069 6e69 7469 616c  e random initial
+00004730: 697a 6174 696f 6e20 6166 6665 6374 7320  ization affects 
+00004740: 7468 6520 7265 7375 6c74 732c 2065 7665  the results, eve
+00004750: 6e20 6769 7665 6e20 7468 6520 7361 6d65  n given the same
+00004760: 2072 616e 646f 6d20 7365 6564 2e20 4469   random seed. Di
+00004770: 6666 6572 656e 7420 7665 7273 696f 6e20  fferent version 
+00004780: 6f66 2060 736b 6c65 6172 6e60 2077 696c  of `sklearn` wil
+00004790: 6c20 6166 6665 6374 2074 6865 2070 6572  l affect the per
+000047a0: 666f 726d 616e 6365 206f 6620 6061 7374  formance of `ast
+000047b0: 6172 7465 7360 2061 6e64 2077 6520 7265  artes` and we re
+000047c0: 636f 6d6d 656e 6420 696e 636c 7564 696e  commend includin
+000047d0: 6720 7468 6520 6578 6163 7420 7665 7273  g the exact vers
+000047e0: 696f 6e20 6f66 2060 7363 696b 6974 2d6c  ion of `scikit-l
+000047f0: 6561 726e 6020 616e 6420 6061 7374 6172  earn` and `astar
+00004800: 7465 7360 2075 7365 642c 2077 6865 6e20  tes` used, when 
+00004810: 6170 706c 6963 6162 6c65 2e0a 0a3e 202a  applicable...> *
+00004820: 2a4e 6f74 652a 2a0a 3e20 5765 2061 7265  *Note**.> We are
+00004830: 206c 696d 6974 6564 2069 6e20 6f75 7220   limited in our 
+00004840: 6162 696c 6974 7920 746f 2074 6573 7420  ability to test 
+00004850: 6f6e 204d 3120 4d61 6373 2c20 6275 7420  on M1 Macs, but 
+00004860: 6672 6f6d 206f 7572 206c 696d 6974 6564  from our limited
+00004870: 206d 616e 7561 6c20 7465 7374 696e 6720   manual testing 
+00004880: 7765 2061 6368 6965 7665 2070 6572 6665  we achieve perfe
+00004890: 6374 2072 6570 726f 6475 6362 696c 6974  ct reproducbilit
+000048a0: 7920 696e 2061 6c6c 2063 6173 6573 205f  y in all cases _
+000048b0: 6578 6365 7074 206f 6363 6173 696f 6e61  except occasiona
+000048c0: 6c6c 795f 2077 6974 6820 604b 4d65 616e  lly_ with `KMean
+000048d0: 7360 206f 6e20 4170 706c 6520 7369 6c69  s` on Apple sili
+000048e0: 636f 6e2e 0a60 6173 7461 7274 6573 6020  con..`astartes` 
+000048f0: 6973 2073 7469 6c6c 2063 6f6e 7369 7374  is still consist
+00004900: 656e 7420 6265 7477 6565 6e20 7275 6e73  ent between runs
+00004910: 206f 6e20 7468 6520 7361 6d65 2070 6c61   on the same pla
+00004920: 7466 6f72 6d20 696e 2061 6c6c 2063 6173  tform in all cas
+00004930: 6573 2c20 616e 6420 6f74 6865 7220 7361  es, and other sa
+00004940: 6d70 6c65 7273 2061 7265 206e 6f74 2069  mplers are not i
+00004950: 6d70 6163 7465 6420 6279 2074 6869 7320  mpacted by this 
+00004960: 6170 7061 7265 6e74 2062 7567 2e0a 0a23  apparent bug...#
+00004970: 2320 486f 7720 746f 2043 6974 650a 4966  # How to Cite.If
+00004980: 2079 6f75 2075 7365 2060 6173 7461 7274   you use `astart
+00004990: 6573 6020 696e 2079 6f75 7220 776f 726b  es` in your work
+000049a0: 2070 6c65 6173 6520 7573 6520 7468 6520   please use the 
+000049b0: 6265 6c6f 7720 6369 7461 7469 6f6e 206f  below citation o
+000049c0: 7220 7468 6520 2243 6974 6520 7468 6973  r the "Cite this
+000049d0: 2072 6570 6f73 6974 6f72 7922 2062 7574   repository" but
+000049e0: 746f 6e20 6f6e 2047 6974 4875 623a 0a3e  ton on GitHub:.>
+000049f0: 202a 2a42 6962 5465 582a 2a0a 3e20 4073   **BibTeX**.> @s
+00004a00: 6f66 7477 6172 657b 6275 726e 735f 6a61  oftware{burns_ja
+00004a10: 636b 736f 6e5f 3230 3233 5f38 3134 3732  ckson_2023_81472
+00004a20: 3035 2c0a 3e20 2020 6175 7468 6f72 2020  05,.>   author  
+00004a30: 2020 2020 203d 207b 4275 726e 732c 204a       = {Burns, J
+00004a40: 6163 6b73 6f6e 2061 6e64 0a3e 2020 2020  ackson and.>    
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00004a60: 7069 656b 6572 6d61 6e6e 2c20 4b65 7669  piekermann, Kevi
+00004a70: 6e20 616e 640a 3e20 2020 2020 2020 2020  n and.>         
+00004a80: 2020 2020 2020 2020 2020 4268 6174 7461            Bhatta
+00004a90: 6368 6172 6a65 652c 2048 696d 6167 686e  charjee, Himaghn
+00004aa0: 6120 616e 640a 3e20 2020 2020 2020 2020  a and.>         
+00004ab0: 2020 2020 2020 2020 2020 566c 6163 686f            Vlacho
+00004ac0: 732c 2044 696f 6e69 7369 6f73 2061 6e64  s, Dionisios and
+00004ad0: 0a3e 2020 2020 2020 2020 2020 2020 2020  .>              
+00004ae0: 2020 2020 2047 7265 656e 2c20 5769 6c6c       Green, Will
+00004af0: 6961 6d7d 2c0a 3e20 2020 7469 746c 6520  iam},.>   title 
+00004b00: 2020 2020 2020 203d 207b 7b4d 6163 6869         = {{Machi
+00004b10: 6e65 204c 6561 726e 696e 6720 5661 6c69  ne Learning Vali
+00004b20: 6461 7469 6f6e 2076 6961 2052 6174 696f  dation via Ratio
+00004b30: 6e61 6c20 4461 7461 7365 7420 0a3e 2020  nal Dataset .>  
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 5361 6d70 6c69 6e67 2077 6974 6820    Sampling with 
+00004b60: 6173 7461 7274 6573 7d7d 2c0a 3e20 2020  astartes}},.>   
+00004b70: 6d6f 6e74 6820 2020 2020 2020 203d 206d  month        = m
+00004b80: 6179 2c0a 3e20 2020 7965 6172 2020 2020  ay,.>   year    
+00004b90: 2020 2020 203d 2032 3032 332c 0a3e 2020       = 2023,.>  
+00004ba0: 2070 7562 6c69 7368 6572 2020 2020 3d20   publisher    = 
+00004bb0: 7b5a 656e 6f64 6f7d 2c0a 3e20 2020 7665  {Zenodo},.>   ve
+00004bc0: 7273 696f 6e20 2020 2020 203d 207b 312e  rsion      = {1.
+00004bd0: 312e 317d 2c0a 3e20 2020 646f 6920 2020  1.1},.>   doi   
+00004be0: 2020 2020 2020 203d 207b 3130 2e35 3238         = {10.528
+00004bf0: 312f 7a65 6e6f 646f 2e38 3134 3732 3035  1/zenodo.8147205
+00004c00: 7d2c 0a3e 2020 2075 726c 2020 2020 2020  },.>   url      
+00004c10: 2020 2020 3d20 7b68 7474 7073 3a2f 2f64      = {https://d
+00004c20: 6f69 2e6f 7267 2f31 302e 3532 3831 2f7a  oi.org/10.5281/z
+00004c30: 656e 6f64 6f2e 3831 3437 3230 357d 0a3e  enodo.8147205}.>
+00004c40: 207d 0a0a 2323 2043 6f6e 7472 6962 7574   }..## Contribut
+00004c50: 696e 6720 2620 4465 7665 6c6f 7065 7220  ing & Developer 
+00004c60: 4e6f 7465 730a 5365 6520 5b43 4f4e 5452  Notes.See [CONTR
+00004c70: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
+00004c80: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00004c90: 6f72 2069 6e73 7472 7563 7469 6f6e 7320  or instructions 
+00004ca0: 6f6e 2069 6e73 7461 6c6c 696e 6720 6061  on installing `a
+00004cb0: 7374 6172 7465 7360 2066 6f72 2064 6576  startes` for dev
+00004cc0: 656c 6f70 6d65 6e74 2c20 6d61 6b69 6e67  elopment, making
+00004cd0: 2061 2063 6f6e 7472 6962 7574 696f 6e2c   a contribution,
+00004ce0: 2061 6e64 2067 656e 6572 616c 2067 7569   and general gui
+00004cf0: 6461 6e63 6520 6f6e 2074 6865 2064 6573  dance on the des
+00004d00: 6967 6e20 6f66 2060 6173 7461 7274 6573  ign of `astartes
+00004d10: 602e 0a0a                                `...
```

### Comparing `astartes-1.1.1/astartes.egg-info/SOURCES.txt` & `astartes-1.1.2/astartes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astartes-1.1.1/pyproject.toml` & `astartes-1.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astartes"
-version = "1.1.1"
+# update this in astartes/__init__.py, too
+version = "1.1.2"
 authors = [
     { name = "Jackson Burns", email = "jwburns@mit.edu" },
     { name = "Himaghna Bhattacharjee", email = "himaghna@udel.edu" },
     { name = "Kevin Spiekermann", email = "kspieker@mit.edu" },
 ]
 license = { text = "MIT" }
 description = "Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays"
```

