# Comparing `tmp/wpcsys-2.1.4.tar.gz` & `tmp/wpcsys-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.1.4.tar", last modified: Thu Jun  8 05:37:00 2023, max compression
+gzip compressed data, was "wpcsys-2.1.5.tar", last modified: Mon Jul 17 04:03:42 2023, max compression
```

## Comparing `wpcsys-2.1.4.tar` & `wpcsys-2.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.902944 wpcsys-2.1.4/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.4/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0    10325 2023-06-08 05:37:00.893920 wpcsys-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     9264 2023-06-08 05:31:19.000000 wpcsys-2.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-08 05:37:00.902944 wpcsys-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.839378 wpcsys-2.1.4/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.4/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.4/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  7016448 2023-06-08 05:33:58.000000 wpcsys-2.1.4/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  7566336 2023-06-08 05:36:18.000000 wpcsys-2.1.4/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  7575552 2023-06-08 05:34:38.000000 wpcsys-2.1.4/wpcsys/pywpc.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.892032 wpcsys-2.1.4/wpcsys.egg-info/
--rw-rw-rw-   0        0        0    10325 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.133986 wpcsys-2.1.5/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10221 2023-07-17 04:03:42.125985 wpcsys-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9160 2023-07-14 09:03:31.000000 wpcsys-2.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 04:03:42.133986 wpcsys-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.069066 wpcsys-2.1.5/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.5/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.5/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  7552000 2023-07-17 03:59:27.000000 wpcsys-2.1.5/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8136704 2023-07-17 04:03:09.000000 wpcsys-2.1.5/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8145920 2023-07-17 04:02:02.000000 wpcsys-2.1.5/wpcsys/pywpc.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.122985 wpcsys-2.1.5/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0    10221 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.1.4/LICENSE` & `wpcsys-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.4/PKG-INFO` & `wpcsys-2.1.5/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: wpcsys
-Version: 2.1.4
-Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
-Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
-Author: chunglee_people, Chieh-An Lin
-Author-email: wu@wpc.com.tw
-License: MIT
-Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: System :: Hardware :: Hardware Drivers
-Classifier: Topic :: Documentation :: Sphinx
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Overview
 --------
 
 **WPC Python driver**, also known as `pywpc`, contains APIs for interacting with basically WPC DAQ cards or any other WPC USB, WiFi and Ethernet based devices.
 It supports Python version from 3.8 to 3.10 under Windows 10 operating systems.
 
 Our APIs support synchronous and asynchronous modes for computer processes or threads.
@@ -34,15 +10,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +64,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -159,51 +135,75 @@
 - Wifi-DAQ-E3-A
 
 - Wifi-DAQ-F4-A
 
 I/O port function table
 -----------------------
 
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-L        |     |     |    |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-O        |     | 0   |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+- EMotion & Motor driver series
+
++----------------+-------+------+
+| Product/module |Motion |Drive |
++----------------+-------+------+
+|  EMotion       |0      |      |
++----------------+-------+------+
+| Edrive-ST      |       |0     |
++----------------+-------+------+
+
+- STEM series
+
++----------------+------+------+------+------+
+| Product/module |AI    |AO    |DI    |DO    |
++----------------+------+------+------+------+
+|  EMotion       |1,2,4 |1,2,4 |0~7   |0~7   |
++----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
+- Ethan & Wifi series
+
++----------------+-----+-----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |
++----------------+-----+-----+----+----+
+| Emotion        |     |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-A        |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-D        |     |     |1   |0   |
++----------------+-----+-----+----+----+
+| Ethan-L        |     |     |    |0   |
++----------------+-----+-----+----+----+
+| Ethan-O        |     | 0   |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+
+- USB series
+
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
 
 - Port 2 is available for DI
```

### Comparing `wpcsys-2.1.4/README.rst` & `wpcsys-2.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: wpcsys
+Version: 2.1.5
+Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
+Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
+Author: chunglee_people, Chieh-An Lin
+Author-email: wu@wpc.com.tw
+License: MIT
+Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware :: Hardware Drivers
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Overview
 --------
 
 **WPC Python driver**, also known as `pywpc`, contains APIs for interacting with basically WPC DAQ cards or any other WPC USB, WiFi and Ethernet based devices.
 It supports Python version from 3.8 to 3.10 under Windows 10 operating systems.
 
 Our APIs support synchronous and asynchronous modes for computer processes or threads.
@@ -10,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -64,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -135,51 +159,75 @@
 - Wifi-DAQ-E3-A
 
 - Wifi-DAQ-F4-A
 
 I/O port function table
 -----------------------
 
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-L        |     |     |    |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-O        |     | 0   |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+- EMotion & Motor driver series
+
++----------------+-------+------+
+| Product/module |Motion |Drive |
++----------------+-------+------+
+|  EMotion       |0      |      |
++----------------+-------+------+
+| Edrive-ST      |       |0     |
++----------------+-------+------+
+
+- STEM series
+
++----------------+------+------+------+------+
+| Product/module |AI    |AO    |DI    |DO    |
++----------------+------+------+------+------+
+|  EMotion       |1,2,4 |1,2,4 |0~7   |0~7   |
++----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
+- Ethan & Wifi series
+
++----------------+-----+-----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |
++----------------+-----+-----+----+----+
+| Emotion        |     |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-A        |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-D        |     |     |1   |0   |
++----------------+-----+-----+----+----+
+| Ethan-L        |     |     |    |0   |
++----------------+-----+-----+----+----+
+| Ethan-O        |     | 0   |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+
+- USB series
+
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
 
 - Port 2 is available for DI
```

### Comparing `wpcsys-2.1.4/setup.py` & `wpcsys-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.4/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.5/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.4/wpcsys.egg-info/PKG-INFO` & `wpcsys-2.1.5/wpcsys.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.4
+Version: 2.1.5
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -159,51 +159,75 @@
 - Wifi-DAQ-E3-A
 
 - Wifi-DAQ-F4-A
 
 I/O port function table
 -----------------------
 
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-L        |     |     |    |0   |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Ethan-O        |     | 0   |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
-+----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+- EMotion & Motor driver series
+
++----------------+-------+------+
+| Product/module |Motion |Drive |
++----------------+-------+------+
+|  EMotion       |0      |      |
++----------------+-------+------+
+| Edrive-ST      |       |0     |
++----------------+-------+------+
+
+- STEM series
+
++----------------+------+------+------+------+
+| Product/module |AI    |AO    |DI    |DO    |
++----------------+------+------+------+------+
+|  EMotion       |1,2,4 |1,2,4 |0~7   |0~7   |
++----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
+- Ethan & Wifi series
+
++----------------+-----+-----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |
++----------------+-----+-----+----+----+
+| Emotion        |     |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-A        |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Ethan-D        |     |     |1   |0   |
++----------------+-----+-----+----+----+
+| Ethan-L        |     |     |    |0   |
++----------------+-----+-----+----+----+
+| Ethan-O        |     | 0   |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |
++----------------+-----+-----+----+----+
+
+- USB series
+
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
+
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
 
 - Port 2 is available for DI
```

