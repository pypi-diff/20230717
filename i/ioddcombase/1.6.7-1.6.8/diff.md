# Comparing `tmp/ioddcombase-1.6.7-cp39-cp39-win_amd64.whl.zip` & `tmp/ioddcombase-1.6.8-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1565347 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      732 b- defN 23-May-08 20:34 siogeen/LICENSE.txt
--rw-rw-rw-  2.0 fat   617984 b- defN 23-May-08 20:34 siogeen/base/IoddUtility.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  3224064 b- defN 23-May-08 20:36 siogeen/base/_IoddDrv.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      416 b- defN 23-May-08 20:34 siogeen/base/__init__.py
--rw-rw-rw-  2.0 fat      732 b- defN 23-May-08 20:36 IoddComBase-1.6.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5116 b- defN 23-May-08 20:36 IoddComBase-1.6.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-08 20:36 IoddComBase-1.6.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-08 20:36 IoddComBase-1.6.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      766 b- defN 23-May-08 20:36 IoddComBase-1.6.7.dist-info/RECORD
-9 files, 3849918 bytes uncompressed, 1564023 bytes compressed:  59.4%
+Zip file size: 1573303 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:29 siogeen/LICENSE.txt
+-rw-rw-rw-  2.0 fat   618496 b- defN 23-May-16 04:29 siogeen/base/IoddUtility.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  3246080 b- defN 23-May-16 04:31 siogeen/base/_IoddDrv.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      416 b- defN 23-May-16 04:29 siogeen/base/__init__.py
+-rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:31 ioddcombase-1.6.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5008 b- defN 23-May-16 04:31 ioddcombase-1.6.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-16 04:31 ioddcombase-1.6.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-16 04:31 ioddcombase-1.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      766 b- defN 23-May-16 04:31 ioddcombase-1.6.8.dist-info/RECORD
+9 files, 3872338 bytes uncompressed, 1571979 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: siogeen/base/_IoddDrv.cp39-win_amd64.pyd
 Comment: 
 
 Filename: siogeen/base/__init__.py
 Comment: 
 
-Filename: IoddComBase-1.6.7.dist-info/LICENSE.txt
+Filename: ioddcombase-1.6.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComBase-1.6.7.dist-info/METADATA
+Filename: ioddcombase-1.6.8.dist-info/METADATA
 Comment: 
 
-Filename: IoddComBase-1.6.7.dist-info/WHEEL
+Filename: ioddcombase-1.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComBase-1.6.7.dist-info/top_level.txt
+Filename: ioddcombase-1.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComBase-1.6.7.dist-info/RECORD
+Filename: ioddcombase-1.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/base/__init__.py

```diff
@@ -8,8 +8,8 @@
 Created on 04.03.2017
 '''
 
 __author__ = "Reimund Renner"
 __email__ = "reimund@siogeen.com"
 __contact__ = "contact@siogeen.com"
 __license__ = "proprietary and confidential"
-__version__ = "1.6.7"
+__version__ = "1.6.8"
```

## Comparing `IoddComBase-1.6.7.dist-info/LICENSE.txt` & `ioddcombase-1.6.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComBase-1.6.7.dist-info/METADATA` & `ioddcombase-1.6.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: IoddComBase
-Version: 1.6.7
+Name: ioddcombase
+Version: 1.6.8
 Summary: IoddCom base
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -59,55 +59,54 @@
 
 ========================= ===================== ===================
 **OS**                    Python 2.7, 3.4-3.5   Python 3.6 - 3.11
 ========================= ===================== ===================
 **Windows**                 [1]_                   x
 **Linux x86/x64**           [1]_                   x
 **Linux Arm (Raspberry)**   [1]_                  3.7-3.11
-**macOS**                   [1]_                  3.8-3.11 [2]_
+**macOS**                   [1]_                  3.8-3.11
 ========================= ===================== ===================
 
 .. [1] IoddCom for Python 2.7, 3.4 - 3.5 on request_.
-.. [2] IoddCom for macOS: Intel chip only, yet
 
 Support for other platforms on request_.
 
 Supported operating systems and IO-Link masters
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Table of supported IO-Link masters for specific operating systems (OS):
 
 +---------------------------------+---------------------------------------------------+
 | Master                          | supported OS                                      |
 |                                 +---------+----------+--------------+---------------+
-|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [3]_ |
+|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [2]_ |
 +=================================+=========+==========+==============+===============+
-| TMG-USB based masters [4]_      |   x     |    x     |    x         |    x          |
+| TMG-USB based masters [3]_      |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| TMG ethernet based masters [5]_ |   x     |    x     |    x         |    x          |
+| TMG ethernet based masters [4]_ |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| ifm ethernet based masters [6]_ |   x     |    x     |    x         |    x          |
+| ifm ethernet based masters [5]_ |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| ifm USB based masters [7]_      |   x     |    x     |    x         |    x          |
+| ifm USB based masters [6]_      |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
 
 For Windows, Linux and Raspberry Pi both, 32-bit and 64-bit versions are available.
 
-.. [3] For macOS 10.15+ Python 3.8-3.11 with Intel chip (others on request)
+.. [2] For macOS 13+
 
-.. [4] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
+.. [3] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
 
-.. [5] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
+.. [4] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
 
-.. [6] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
+.. [5] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
        master type.
        The following functions are missing yet: PD streaming, master data storage read/write,
        master commands, PD valid status
 
-.. [7] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
-       like for [6]_
+.. [6] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
+       like for [5]_
 
 Not supported masters:
 
 * RevolutionPi RevPi masters
 * Pepperl & Fuchs comtrol masters
 * Baumer USB-C and senscontrol masters
 * Germbedded masters
```

## Comparing `IoddComBase-1.6.7.dist-info/RECORD` & `ioddcombase-1.6.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 siogeen/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-siogeen/base/IoddUtility.cp39-win_amd64.pyd,sha256=JMzWiD2_I50hnzXrWpqTbqOcbRBUV3bVWTQQmZZ3NFk,617984
-siogeen/base/_IoddDrv.cp39-win_amd64.pyd,sha256=_0cNhYNKGRu1j5FXlN_aoFFCoabOGQH9N63DZKbbr-k,3224064
-siogeen/base/__init__.py,sha256=3RWsLirPaIRGyeSo6UgmaN-dhBzyChoqlP56S54XJTE,416
-IoddComBase-1.6.7.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-IoddComBase-1.6.7.dist-info/METADATA,sha256=2eD7QZI6XobC-h_GvweFoKbQDoUfyoxefeHNZKAVuqk,5116
-IoddComBase-1.6.7.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-IoddComBase-1.6.7.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
-IoddComBase-1.6.7.dist-info/RECORD,,
+siogeen/base/IoddUtility.cp39-win_amd64.pyd,sha256=rv-9D_XupfoLx4h4KYU_Kkb9lPHseM5UtMf_fPM12tU,618496
+siogeen/base/_IoddDrv.cp39-win_amd64.pyd,sha256=nTo2GaW_BnSliF5fFgU4CIRtrEAj9JTxASwUzJcoVWo,3246080
+siogeen/base/__init__.py,sha256=EleD32l5dnOBGo5NB6no_iG2RIMXGt4fCuAMg7UfjSA,416
+ioddcombase-1.6.8.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
+ioddcombase-1.6.8.dist-info/METADATA,sha256=xfq1fTUjUCN0hb56TN9QT7zMCVgHAZiVCoVZpL5WnT0,5008
+ioddcombase-1.6.8.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+ioddcombase-1.6.8.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
+ioddcombase-1.6.8.dist-info/RECORD,,
```

