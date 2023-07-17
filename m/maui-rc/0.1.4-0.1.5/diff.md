# Comparing `tmp/maui_rc-0.1.4.tar.gz` & `tmp/maui_rc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_rc-0.1.4.tar", max compression
+gzip compressed data, was "maui_rc-0.1.5.tar", max compression
```

## Comparing `maui_rc-0.1.4.tar` & `maui_rc-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.4/LICENSE
--rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.4/maui_rc/__init__.py
--rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.4/maui_rc/datatypes.py
--rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.4/maui_rc/scope.py
--rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.4/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
--rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.4/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
--rw-r--r--   0        0        0     5748 2023-07-14 18:50:36.992217 maui_rc-0.1.4/maui_rc/subsystems/acquisition.py
--rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.4/maui_rc/subsystems/panelsetup.py
--rw-r--r--   0        0        0    20905 2023-07-14 19:18:00.821261 maui_rc-0.1.4/maui_rc/subsystems/wavedata.py
--rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.4/maui_rc/subsystems/waveform.py
--rw-r--r--   0        0        0      555 2023-07-14 19:18:41.893429 maui_rc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.5/LICENSE
+-rw-r--r--   0        0        0      759 2023-07-17 11:55:29.750458 maui_rc-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.5/maui_rc/__init__.py
+-rw-r--r--   0        0        0     1537 2023-07-17 12:17:35.029616 maui_rc-0.1.5/maui_rc/datatypes.py
+-rw-r--r--   0        0        0     2510 2023-07-17 12:15:56.144720 maui_rc-0.1.5/maui_rc/scope.py
+-rw-r--r--   0        0        0     8686 2023-07-17 13:28:51.841986 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
+-rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
+-rw-r--r--   0        0        0    28616 2023-07-17 13:29:46.983870 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/waveform.cpython-311.pyc
+-rw-r--r--   0        0        0     5016 2023-07-17 12:15:27.478571 maui_rc-0.1.5/maui_rc/subsystems/acquisition.py
+-rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.5/maui_rc/subsystems/panelsetup.py
+-rw-r--r--   0        0        0    22653 2023-07-17 13:29:39.757355 maui_rc-0.1.5/maui_rc/subsystems/waveform.py
+-rw-r--r--   0        0        0      555 2023-07-17 17:28:55.432869 maui_rc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 maui_rc-0.1.5/PKG-INFO
```

### Comparing `maui_rc-0.1.4/LICENSE` & `maui_rc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.4/maui_rc/datatypes.py` & `maui_rc-0.1.5/maui_rc/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     - `CHAN_4` -> channel 4
     """
 
     CHAN_1 = "C1"
     CHAN_2 = "C2"
     CHAN_3 = "C3"
     CHAN_4 = "C4"
+    CHAN_5 = "C5"
+    CHAN_6 = "C6"
+    CHAN_7 = "C7"
+    CHAN_8 = "C8"
 
     def __str__(self):
         return self.value
 
 
 class CouplingMode(Enum):
     """Enum of possible trigger coupling modes.
```

### Comparing `maui_rc-0.1.4/maui_rc/scope.py` & `maui_rc-0.1.5/maui_rc/scope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pyvisa
 
 from maui_rc.subsystems.panelsetup import PanelSetup
 from maui_rc.subsystems.acquisition import Acquitision
+from maui_rc.subsystems.waveform import Waveform
 
 
 class VirtualScope:
     """
     Class representing the oscilloscope. Initialize using the VISA address of the device (e.g. 'VICP::<IP shown on device>::INSTR')
     """
 
@@ -20,16 +21,18 @@
         # set the log on the device to display full dialog and to
         # reset this decision on poweroff
         self.__scope.write("COMM_HELP FD,YES")
 
         # setup the subsystems
         self.panelsetup = PanelSetup(self.__scope)
         self.acquisition = Acquitision(self.__scope)
+        self.waveform = Waveform(self.__scope)
 
     def list_instruments():
+        """List the resources (devices) available to MAUI RC."""
         rm = pyvisa.ResourceManager("@py")
         print(rm.list_resources())
 
     def set_timeout(self, duration: int):
         """Set the timeout on queries to the device.
 
         Arguments:
@@ -54,15 +57,18 @@
         # parse the log out of the query
         # first remove the first and last characters (those are quotations)
         log = resp.removeprefix('"').removesuffix('\n"\n').split("\n")
         for line in log:
             print(line)
 
     def command(self, cmd: str):
+        """Send a command to the instrument."""
         self.__scope.write(cmd)
 
     def query(self, cmd: str) -> str:
+        """Query the intrument and return the decoded response."""
         return self.__scope.query(cmd)
     
     def query_raw(self, cmd: str) -> bytes:
+        """Query the intrument and return the raw response of bytes."""
         self.__scope.write(cmd)
         return self.__scope.read_raw()
```

### Comparing `maui_rc-0.1.4/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc` & `maui_rc-0.1.5/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,40 +1,45 @@
 magic:    0xa70d0d0a
-moddate:  0x09f0ae64 (Wed Jul 12 18:25:13 2023 UTC)
-files sz: 4967
+moddate:  0xdf30b564 (Mon Jul 17 12:15:27 2023 UTC)
+files sz: 5016
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c005a00640064026c01540002004700640384006404a6
-      020000ab0200000000000000005a0264015300
+      0x9700640064016c005a00640064026c015400640064016c025a03020047
+      00640384006404a6020000ab0200000000000000005a0464015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pyvisa)
                  8 STORE_NAME               0 (pyvisa)
    
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               2 (('*',))
                 14 IMPORT_NAME              1 (maui_rc.datatypes)
                 16 IMPORT_STAR
    
-     5          18 PUSH_NULL
-                20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object Acquitision, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 5>)
-                24 MAKE_FUNCTION            0
-                26 LOAD_CONST               4 ('Acquitision')
-                28 PRECALL                  2
-                32 CALL                     2
-                42 STORE_NAME               2 (Acquitision)
-                44 LOAD_CONST               1 (None)
-                46 RETURN_VALUE
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               1 (None)
+                22 IMPORT_NAME              2 (numpy)
+                24 STORE_NAME               3 (np)
+   
+     6          26 PUSH_NULL
+                28 LOAD_BUILD_CLASS
+                30 LOAD_CONST               3 (<code object Acquitision, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 6>)
+                32 MAKE_FUNCTION            0
+                34 LOAD_CONST               4 ('Acquitision')
+                36 PRECALL                  2
+                40 CALL                     2
+                50 STORE_NAME               4 (Acquitision)
+                52 LOAD_CONST               1 (None)
+                54 RETURN_VALUE
    consts
       0
       None
       ('*',)
       code
          argcount  : 0
          nlocals   : 0
@@ -45,177 +50,177 @@
             02640384045a06640484005a0764056508640665086604640784045a0964
             0884005a0a640984005a0b640a84005a0c640b650d6602640c84045a0e64
             0d650d6602640e84045a0f640b650d6602640f84045a10640d650d660264
             1084045a11641165086602641284045a12640d65086602641384045a1364
             1e6415650d641665146604641784055a15641665146602641884045a1664
             1984005a17641a84005a18641b84005a19641c84005a1a640d651b660264
             1d84045a1c64145300
-           5           0 RESUME                   0
+           6           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Acquitision')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 ('Class that groups functions relating to acquisition.')
+           7          10 LOAD_CONST               1 ('Class that groups functions relating to acquisition.')
                       12 STORE_NAME               3 (__doc__)
          
-           8          14 LOAD_CONST               2 ('scope')
+           9          14 LOAD_CONST               2 ('scope')
                       16 LOAD_NAME                4 (pyvisa)
                       18 LOAD_ATTR                5 (Resource)
                       28 BUILD_TUPLE              2
-                      30 LOAD_CONST               3 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 8>)
+                      30 LOAD_CONST               3 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 9>)
                       32 MAKE_FUNCTION            4 (annotations)
                       34 STORE_NAME               6 (__init__)
          
-          11          36 LOAD_CONST               4 (<code object arm_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 11>)
+          12          36 LOAD_CONST               4 (<code object arm_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 12>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               7 (arm_acquisition)
          
-          15          42 LOAD_CONST               5 ('number_segments')
+          16          42 LOAD_CONST               5 ('number_segments')
                       44 LOAD_NAME                8 (int)
                       46 LOAD_CONST               6 ('max_size')
                       48 LOAD_NAME                8 (int)
                       50 BUILD_TUPLE              4
-                      52 LOAD_CONST               7 (<code object enable_sequence, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 15>)
+                      52 LOAD_CONST               7 (<code object enable_sequence, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 16>)
                       54 MAKE_FUNCTION            4 (annotations)
                       56 STORE_NAME               9 (enable_sequence)
          
-          27          58 LOAD_CONST               8 (<code object disable_sequence, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 27>)
+          28          58 LOAD_CONST               8 (<code object disable_sequence, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 28>)
                       60 MAKE_FUNCTION            0
                       62 STORE_NAME              10 (disable_sequence)
          
-          33          64 LOAD_CONST               9 (<code object stop_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 33>)
+          34          64 LOAD_CONST               9 (<code object stop_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 34>)
                       66 MAKE_FUNCTION            0
                       68 STORE_NAME              11 (stop_acquisition)
          
-          39          70 LOAD_CONST              10 (<code object wait_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 39>)
+          40          70 LOAD_CONST              10 (<code object wait_acquisition, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 40>)
                       72 MAKE_FUNCTION            0
                       74 STORE_NAME              12 (wait_acquisition)
          
-          45          76 LOAD_CONST              11 ('value')
+          46          76 LOAD_CONST              11 ('value')
                       78 LOAD_NAME               13 (float)
                       80 BUILD_TUPLE              2
-                      82 LOAD_CONST              12 (<code object set_time_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 45>)
+                      82 LOAD_CONST              12 (<code object set_time_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 46>)
                       84 MAKE_FUNCTION            4 (annotations)
                       86 STORE_NAME              14 (set_time_div)
          
-          56          88 LOAD_CONST              13 ('return')
+          57          88 LOAD_CONST              13 ('return')
                       90 LOAD_NAME               13 (float)
                       92 BUILD_TUPLE              2
-                      94 LOAD_CONST              14 (<code object get_time_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 56>)
+                      94 LOAD_CONST              14 (<code object get_time_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 57>)
                       96 MAKE_FUNCTION            4 (annotations)
                       98 STORE_NAME              15 (get_time_div)
          
-          63         100 LOAD_CONST              11 ('value')
+          64         100 LOAD_CONST              11 ('value')
                      102 LOAD_NAME               13 (float)
                      104 BUILD_TUPLE              2
-                     106 LOAD_CONST              15 (<code object set_volt_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 63>)
+                     106 LOAD_CONST              15 (<code object set_volt_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 64>)
                      108 MAKE_FUNCTION            4 (annotations)
                      110 STORE_NAME              16 (set_volt_div)
          
-          73         112 LOAD_CONST              13 ('return')
+          74         112 LOAD_CONST              13 ('return')
                      114 LOAD_NAME               13 (float)
                      116 BUILD_TUPLE              2
-                     118 LOAD_CONST              16 (<code object get_volt_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 73>)
+                     118 LOAD_CONST              16 (<code object get_volt_div, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 74>)
                      120 MAKE_FUNCTION            4 (annotations)
                      122 STORE_NAME              17 (get_volt_div)
          
-          80         124 LOAD_CONST              17 ('delay')
+          81         124 LOAD_CONST              17 ('delay')
                      126 LOAD_NAME                8 (int)
                      128 BUILD_TUPLE              2
-                     130 LOAD_CONST              18 (<code object set_trigger_delay, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 80>)
+                     130 LOAD_CONST              18 (<code object set_trigger_delay, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 81>)
                      132 MAKE_FUNCTION            4 (annotations)
                      134 STORE_NAME              18 (set_trigger_delay)
          
-          97         136 LOAD_CONST              13 ('return')
+          98         136 LOAD_CONST              13 ('return')
                      138 LOAD_NAME                8 (int)
                      140 BUILD_TUPLE              2
-                     142 LOAD_CONST              19 (<code object get_trigger_delay, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 97>)
+                     142 LOAD_CONST              19 (<code object get_trigger_delay, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 98>)
                      144 MAKE_FUNCTION            4 (annotations)
                      146 STORE_NAME              19 (get_trigger_delay)
          
-         106         148 LOAD_CONST              30 ((None,))
+         107         148 LOAD_CONST              30 ((None,))
                      150 LOAD_CONST              21 ('level')
                      152 LOAD_NAME               13 (float)
                      154 LOAD_CONST              22 ('trigger_source')
                      156 LOAD_NAME               20 (Channel)
                      158 BUILD_TUPLE              4
-                     160 LOAD_CONST              23 (<code object set_trigger_level, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 106>)
+                     160 LOAD_CONST              23 (<code object set_trigger_level, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 107>)
                      162 MAKE_FUNCTION            5 (defaults, annotations)
                      164 STORE_NAME              21 (set_trigger_level)
          
-         124         166 LOAD_CONST              22 ('trigger_source')
+         125         166 LOAD_CONST              22 ('trigger_source')
                      168 LOAD_NAME               20 (Channel)
                      170 BUILD_TUPLE              2
-                     172 LOAD_CONST              24 (<code object get_trigger_level, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 124>)
+                     172 LOAD_CONST              24 (<code object get_trigger_level, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 125>)
                      174 MAKE_FUNCTION            4 (annotations)
                      176 STORE_NAME              22 (get_trigger_level)
          
-         137         178 LOAD_CONST              25 (<code object trigger_normal, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 137>)
+         138         178 LOAD_CONST              25 (<code object trigger_normal, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 138>)
                      180 MAKE_FUNCTION            0
                      182 STORE_NAME              23 (trigger_normal)
          
-         141         184 LOAD_CONST              26 (<code object trigger_auto, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 141>)
+         142         184 LOAD_CONST              26 (<code object trigger_auto, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 142>)
                      186 MAKE_FUNCTION            0
                      188 STORE_NAME              24 (trigger_auto)
          
-         145         190 LOAD_CONST              27 (<code object trigger_single, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 145>)
+         146         190 LOAD_CONST              27 (<code object trigger_single, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 146>)
                      192 MAKE_FUNCTION            0
                      194 STORE_NAME              25 (trigger_single)
          
-         149         196 LOAD_CONST              28 (<code object trigger_stop, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 149>)
+         150         196 LOAD_CONST              28 (<code object trigger_stop, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 150>)
                      198 MAKE_FUNCTION            0
                      200 STORE_NAME              26 (trigger_stop)
          
-         153         202 LOAD_CONST              13 ('return')
+         154         202 LOAD_CONST              13 ('return')
                      204 LOAD_NAME               27 (TriggerMode)
                      206 BUILD_TUPLE              2
-                     208 LOAD_CONST              29 (<code object get_trigger_mode, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 153>)
+                     208 LOAD_CONST              29 (<code object get_trigger_mode, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py", line 154>)
                      210 MAKE_FUNCTION            4 (annotations)
                      212 STORE_NAME              28 (get_trigger_mode)
                      214 LOAD_CONST              20 (None)
                      216 RETURN_VALUE
          consts
             'Acquitision'
             'Class that groups functions relating to acquisition.'
             'scope'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c017c005f00000000000000000064005300
-                 8           0 RESUME                   0
+                 9           0 RESUME                   0
                
-                 9           2 LOAD_FAST                1 (scope)
+                10           2 LOAD_FAST                1 (scope)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (_Acquitision__scope)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('_Acquitision__scope',)
                varnames   ('self', 'scope')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       '__init__'
-               firstlineno 8
+               firstlineno 9
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-                11           0 RESUME                   0
+                12           0 RESUME                   0
                
-                13           2 LOAD_FAST                0 (self)
+                14           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('ARM_ACQUISITION')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -226,15 +231,15 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'arm_acquisition'
-               firstlineno 11
+               firstlineno 12
                lnotab 0x0202
             'number_segments'
             'max_size'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -242,31 +247,31 @@
                code
                   0x97006401a0000000000000000000000000000000000000000000740300
                   0000000000000000007c01a6010000ab0100000000000000007403000000
                   000000000000007c01a6010000ab010000000000000000a6020000ab0200
                   000000000000007d037c006a020000000000000000a00300000000000000
                   000000000000000000000000007c03a6010000ab01000000000000000001
                   0064025300
-                15           0 RESUME                   0
+                16           0 RESUME                   0
                
-                24           2 LOAD_CONST               1 ('SEQUENCE ON,{},{:e}')
+                25           2 LOAD_CONST               1 ('SEQUENCE ON,{},{:e}')
                              4 LOAD_METHOD              0 (format)
                             26 LOAD_GLOBAL              3 (NULL + int)
                             38 LOAD_FAST                1 (number_segments)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 LOAD_GLOBAL              3 (NULL + int)
                             66 LOAD_FAST                1 (number_segments)
                             68 PRECALL                  1
                             72 CALL                     1
                             82 PRECALL                  2
                             86 CALL                     2
                             96 STORE_FAST               3 (cmd)
                
-                25          98 LOAD_FAST                0 (self)
+                26          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                2 (_Acquitision__scope)
                            110 LOAD_METHOD              3 (write)
                            132 LOAD_FAST                3 (cmd)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 POP_TOP
                            150 LOAD_CONST               2 (None)
@@ -277,27 +282,27 @@
                   None
                names      ('format', 'int', '_Acquitision__scope', 'write')
                varnames   ('self', 'number_segments', 'max_size', 'cmd')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'enable_sequence'
-               firstlineno 15
+               firstlineno 16
                lnotab 0x02096001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                
-                31           2 LOAD_FAST                0 (self)
+                32           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('SEQUENCE OFF')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -308,27 +313,27 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'disable_sequence'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x0204
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-                33           0 RESUME                   0
+                34           0 RESUME                   0
                
-                37           2 LOAD_FAST                0 (self)
+                38           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('STOP')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -339,27 +344,27 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'stop_acquisition'
-               firstlineno 33
+               firstlineno 34
                lnotab 0x0204
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-                39           0 RESUME                   0
+                40           0 RESUME                   0
                
-                43           2 LOAD_FAST                0 (self)
+                44           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('WAIT')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -370,41 +375,41 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'wait_acquisition'
-               firstlineno 39
+               firstlineno 40
                lnotab 0x0204
             'value'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97006401a0000000000000000000000000000000000000000000740300
                   0000000000000000007c01a6010000ab010000000000000000a6010000ab
                   0100000000000000007d027c006a020000000000000000a0030000000000
                   0000000000000000000000000000007c02a6010000ab0100000000000000
                   00010064025300
-                45           0 RESUME                   0
+                46           0 RESUME                   0
                
-                53           2 LOAD_CONST               1 ('TIME_DIV {:e}')
+                54           2 LOAD_CONST               1 ('TIME_DIV {:e}')
                              4 LOAD_METHOD              0 (format)
                             26 LOAD_GLOBAL              3 (NULL + float)
                             38 LOAD_FAST                1 (value)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (cmd)
                
-                54          70 LOAD_FAST                0 (self)
+                55          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (_Acquitision__scope)
                             82 LOAD_METHOD              3 (write)
                            104 LOAD_FAST                2 (cmd)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_TOP
                            122 LOAD_CONST               2 (None)
@@ -415,81 +420,81 @@
                   None
                names      ('format', 'float', '_Acquitision__scope', 'write')
                varnames   ('self', 'value', 'cmd')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'set_time_div'
-               firstlineno 45
+               firstlineno 46
                lnotab 0x02084401
             'return'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab0000000000000000007d
                   017407000000000000000000007c01a6010000ab01000000000000000053
                   00
-                56           0 RESUME                   0
+                57           0 RESUME                   0
                
-                60           2 LOAD_FAST                0 (self)
+                61           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (query)
                             36 LOAD_CONST               1 ('TIME_DIV?')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (strip)
                             74 PRECALL                  0
                             78 CALL                     0
                             88 STORE_FAST               1 (time_div)
                
-                61          90 LOAD_GLOBAL              7 (NULL + float)
+                62          90 LOAD_GLOBAL              7 (NULL + float)
                            102 LOAD_FAST                1 (time_div)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 RETURN_VALUE
                consts
                   'Get the current timebase setting.'
                   'TIME_DIV?'
                names      ('_Acquitision__scope', 'query', 'strip', 'float')
                varnames   ('self', 'time_div')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'get_time_div'
-               firstlineno 56
+               firstlineno 57
                lnotab 0x02045801
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97006401a0000000000000000000000000000000000000000000740300
                   0000000000000000007c01a6010000ab010000000000000000a6010000ab
                   0100000000000000007d027c006a020000000000000000a0030000000000
                   0000000000000000000000000000007c02a6010000ab0100000000000000
                   00010064025300
-                63           0 RESUME                   0
+                64           0 RESUME                   0
                
-                70           2 LOAD_CONST               1 ('VOLT_DIV {:e}')
+                71           2 LOAD_CONST               1 ('VOLT_DIV {:e}')
                              4 LOAD_METHOD              0 (format)
                             26 LOAD_GLOBAL              3 (NULL + float)
                             38 LOAD_FAST                1 (value)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (cmd)
                
-                71          70 LOAD_FAST                0 (self)
+                72          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (_Acquitision__scope)
                             82 LOAD_METHOD              3 (write)
                            104 LOAD_FAST                2 (cmd)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_TOP
                            122 LOAD_CONST               2 (None)
@@ -500,92 +505,98 @@
                   None
                names      ('format', 'float', '_Acquitision__scope', 'write')
                varnames   ('self', 'value', 'cmd')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'set_volt_div'
-               firstlineno 63
+               firstlineno 64
                lnotab 0x02074401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007d
-                  017407000000000000000000007c01a6010000ab01000000000000000053
-                  00
-                73           0 RESUME                   0
+                  0000000000000000000000000000006402a6010000ab0100000000000000
+                  00a0030000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d017409000000000000000000007c01a6010000ab0100
+                  000000000000005300
+                74           0 RESUME                   0
                
-                77           2 LOAD_FAST                0 (self)
+                78           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (query)
                             36 LOAD_CONST               1 ('VOLT_DIV?')
                             38 PRECALL                  1
                             42 CALL                     1
-                            52 LOAD_METHOD              2 (strip)
-                            74 PRECALL                  0
-                            78 CALL                     0
-                            88 STORE_FAST               1 (volt_div)
-               
-                78          90 LOAD_GLOBAL              7 (NULL + float)
-                           102 LOAD_FAST                1 (volt_div)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 RETURN_VALUE
+                            52 LOAD_METHOD              2 (decode)
+                            74 LOAD_CONST               2 ('utf-8')
+                            76 PRECALL                  1
+                            80 CALL                     1
+                            90 LOAD_METHOD              3 (strip)
+                           112 PRECALL                  0
+                           116 CALL                     0
+                           126 STORE_FAST               1 (volt_div)
+               
+                79         128 LOAD_GLOBAL              9 (NULL + float)
+                           140 LOAD_FAST                1 (volt_div)
+                           142 PRECALL                  1
+                           146 CALL                     1
+                           156 RETURN_VALUE
                consts
                   'Gets the vertical sensitivity'
                   'VOLT_DIV?'
-               names      ('_Acquitision__scope', 'query', 'strip', 'float')
+                  'utf-8'
+               names      ('_Acquitision__scope', 'query', 'decode', 'strip', 'float')
                varnames   ('self', 'volt_div')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'get_volt_div'
-               firstlineno 73
-               lnotab 0x02045801
+               firstlineno 74
+               lnotab 0x02047e01
             'delay'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c0164016b040000000073067c0164026b0000000000720f740100
                   0000000000000000006403a6010000ab010000000000000000820164047c
                   019b009d027d027c006a010000000000000000a002000000000000000000
                   00000000000000000000007c02a6010000ab010000000000000000010064
                   055300
-                80           0 RESUME                   0
+                81           0 RESUME                   0
                
-                90           2 LOAD_FAST                1 (delay)
+                91           2 LOAD_FAST                1 (delay)
                              4 LOAD_CONST               1 (10)
                              6 COMPARE_OP               4 (>)
                             12 POP_JUMP_FORWARD_IF_TRUE     6 (to 26)
                             14 LOAD_FAST                1 (delay)
                             16 LOAD_CONST               2 (-10000)
                             18 COMPARE_OP               0 (<)
                             24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
                
-                91     >>   26 LOAD_GLOBAL              1 (NULL + Exception)
+                92     >>   26 LOAD_GLOBAL              1 (NULL + Exception)
                             38 LOAD_CONST               3 ('trigger delay must be between -10000 and 10 inclusively')
                             40 PRECALL                  1
                             44 CALL                     1
                             54 RAISE_VARARGS            1
                
-                94     >>   56 LOAD_CONST               4 ('TRIG_DELAY ')
+                95     >>   56 LOAD_CONST               4 ('TRIG_DELAY ')
                             58 LOAD_FAST                1 (delay)
                             60 FORMAT_VALUE             0
                             62 BUILD_STRING             2
                             64 STORE_FAST               2 (cmd)
                
-                95          66 LOAD_FAST                0 (self)
+                96          66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                1 (_Acquitision__scope)
                             78 LOAD_METHOD              2 (write)
                            100 LOAD_FAST                2 (cmd)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 POP_TOP
                            118 LOAD_CONST               5 (None)
@@ -599,61 +610,65 @@
                   None
                names      ('Exception', '_Acquitision__scope', 'write')
                varnames   ('self', 'delay', 'cmd')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'set_trigger_delay'
-               firstlineno 80
+               firstlineno 81
                lnotab 0x020a18011e030a01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   0000000000000000000000000000006402a6010000ab0100000000000000
-                  007d017407000000000000000000007c01a6010000ab0100000000000000
-                  007d027c025300
-                97           0 RESUME                   0
+                  00a0030000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d017409000000000000000000007c01a6010000ab0100
+                  000000000000007d027c025300
+                98           0 RESUME                   0
                
-               101           2 LOAD_FAST                0 (self)
+               102           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (query)
                             36 LOAD_CONST               1 ('TRIG_DELAY?')
                             38 PRECALL                  1
                             42 CALL                     1
-                            52 LOAD_METHOD              2 (removesuffix)
-                            74 LOAD_CONST               2 ('\n')
+                            52 LOAD_METHOD              2 (decode)
+                            74 LOAD_CONST               2 ('utf-8')
                             76 PRECALL                  1
                             80 CALL                     1
-                            90 STORE_FAST               1 (resp)
-               
-               102          92 LOAD_GLOBAL              7 (NULL + int)
-                           104 LOAD_FAST                1 (resp)
-                           106 PRECALL                  1
-                           110 CALL                     1
-                           120 STORE_FAST               2 (delay)
+                            90 LOAD_METHOD              3 (strip)
+                           112 PRECALL                  0
+                           116 CALL                     0
+                           126 STORE_FAST               1 (resp)
+               
+               103         128 LOAD_GLOBAL              9 (NULL + int)
+                           140 LOAD_FAST                1 (resp)
+                           142 PRECALL                  1
+                           146 CALL                     1
+                           156 STORE_FAST               2 (delay)
                
-               104         122 LOAD_FAST                2 (delay)
-                           124 RETURN_VALUE
+               105         158 LOAD_FAST                2 (delay)
+                           160 RETURN_VALUE
                consts
                   'Gets the time at which the trigger is to occur'
                   'TRIG_DELAY?'
-                  '\n'
-               names      ('_Acquitision__scope', 'query', 'removesuffix', 'int')
+                  'utf-8'
+               names      ('_Acquitision__scope', 'query', 'decode', 'strip', 'int')
                varnames   ('self', 'resp', 'delay')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'get_trigger_delay'
-               firstlineno 97
-               lnotab 0x02045a011e02
+               firstlineno 98
+               lnotab 0x02047e011e02
             None
             'level'
             'trigger_source'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -661,46 +676,46 @@
                code
                   0x97007c02811464027401000000000000000000007c01a6010000ab0100
                   000000000000009b0064039d037d036e227403000000000000000000007c
                   02a6010000ab0100000000000000009b0064047401000000000000000000
                   007c01a6010000ab0100000000000000009b0064039d047d037c006a0200
                   00000000000000a00300000000000000000000000000000000000000007c
                   03a6010000ab010000000000000000010064015300
-               106           0 RESUME                   0
+               107           0 RESUME                   0
                
-               116           2 LOAD_FAST                2 (trigger_source)
+               117           2 LOAD_FAST                2 (trigger_source)
                              4 POP_JUMP_FORWARD_IF_NONE    20 (to 46)
                
-               117           6 LOAD_CONST               2 ('TRIG_LEVEL ')
+               118           6 LOAD_CONST               2 ('TRIG_LEVEL ')
                              8 LOAD_GLOBAL              1 (NULL + float)
                             20 LOAD_FAST                1 (level)
                             22 PRECALL                  1
                             26 CALL                     1
                             36 FORMAT_VALUE             0
                             38 LOAD_CONST               3 ('V')
                             40 BUILD_STRING             3
                             42 STORE_FAST               3 (cmd)
                             44 JUMP_FORWARD            34 (to 114)
                
-               119     >>   46 LOAD_GLOBAL              3 (NULL + Channel)
+               120     >>   46 LOAD_GLOBAL              3 (NULL + Channel)
                             58 LOAD_FAST                2 (trigger_source)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 (':TRIG_LEVEL ')
                             78 LOAD_GLOBAL              1 (NULL + float)
                             90 LOAD_FAST                1 (level)
                             92 PRECALL                  1
                             96 CALL                     1
                            106 FORMAT_VALUE             0
                            108 LOAD_CONST               3 ('V')
                            110 BUILD_STRING             4
                            112 STORE_FAST               3 (cmd)
                
-               122     >>  114 LOAD_FAST                0 (self)
+               123     >>  114 LOAD_FAST                0 (self)
                            116 LOAD_ATTR                2 (_Acquitision__scope)
                            126 LOAD_METHOD              3 (write)
                            148 LOAD_FAST                3 (cmd)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 POP_TOP
                            166 LOAD_CONST               1 (None)
@@ -713,75 +728,79 @@
                   ':TRIG_LEVEL '
                names      ('float', 'Channel', '_Acquitision__scope', 'write')
                varnames   ('self', 'level', 'trigger_source', 'cmd')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'set_trigger_level'
-               firstlineno 106
+               firstlineno 107
                lnotab 0x020a040128024403
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c01a6010000ab0100000000000000
                   009b0064019d027d027c006a010000000000000000a00200000000000000
                   000000000000000000000000007c02a6010000ab010000000000000000a0
                   0300000000000000000000000000000000000000006402a6010000ab0100
-                  000000000000007d037c035300
-               124           0 RESUME                   0
+                  00000000000000a0040000000000000000000000000000000000000000a6
+                  000000ab0000000000000000007d037c035300
+               125           0 RESUME                   0
                
-               132           2 LOAD_GLOBAL              1 (NULL + Channel)
+               133           2 LOAD_GLOBAL              1 (NULL + Channel)
                             14 LOAD_FAST                1 (trigger_source)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 ('TRIG_LEVEL?')
                             34 BUILD_STRING             2
                             36 STORE_FAST               2 (cmd)
                
-               134          38 LOAD_FAST                0 (self)
+               135          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                1 (_Acquitision__scope)
                             50 LOAD_METHOD              2 (query)
                             72 LOAD_FAST                2 (cmd)
                             74 PRECALL                  1
                             78 CALL                     1
-                            88 LOAD_METHOD              3 (removesuffix)
-                           110 LOAD_CONST               2 ('\n')
+                            88 LOAD_METHOD              3 (decode)
+                           110 LOAD_CONST               2 ('utf-8')
                            112 PRECALL                  1
                            116 CALL                     1
-                           126 STORE_FAST               3 (level)
+                           126 LOAD_METHOD              4 (strip)
+                           148 PRECALL                  0
+                           152 CALL                     0
+                           162 STORE_FAST               3 (level)
                
-               135         128 LOAD_FAST                3 (level)
-                           130 RETURN_VALUE
+               136         164 LOAD_FAST                3 (level)
+                           166 RETURN_VALUE
                consts
                   'Gets the trigger level of the specified trigger source.\n\n        Arguments:\n        - `trigger_source` -> specified trigger source\n        '
                   'TRIG_LEVEL?'
-                  '\n'
-               names      ('Channel', '_Acquitision__scope', 'query', 'removesuffix')
+                  'utf-8'
+               names      ('Channel', '_Acquitision__scope', 'query', 'decode', 'strip')
                varnames   ('self', 'trigger_source', 'cmd', 'level')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'get_trigger_level'
-               firstlineno 124
-               lnotab 0x020824025a01
+               firstlineno 125
+               lnotab 0x020824027e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-               137           0 RESUME                   0
+               138           0 RESUME                   0
                
-               139           2 LOAD_FAST                0 (self)
+               140           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('TRIG_MODE NORMAL')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -792,27 +811,27 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'trigger_normal'
-               firstlineno 137
+               firstlineno 138
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-               141           0 RESUME                   0
+               142           0 RESUME                   0
                
-               143           2 LOAD_FAST                0 (self)
+               144           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('TRIG_MODE AUTO')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -823,27 +842,27 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'trigger_auto'
-               firstlineno 141
+               firstlineno 142
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-               145           0 RESUME                   0
+               146           0 RESUME                   0
                
-               147           2 LOAD_FAST                0 (self)
+               148           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('TRIG_MODE SINGLE')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -854,27 +873,27 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'trigger_single'
-               firstlineno 145
+               firstlineno 146
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000010064025300
-               149           0 RESUME                   0
+               150           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (self)
+               152           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (write)
                             36 LOAD_CONST               1 ('TRIG_MODE STOP')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               2 (None)
@@ -885,74 +904,78 @@
                   None
                names      ('_Acquitision__scope', 'write')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'trigger_stop'
-               firstlineno 149
+               firstlineno 150
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   0000000000000000000000000000006402a6010000ab0100000000000000
-                  007d017407000000000000000000007c01a6010000ab0100000000000000
-                  007d027c025300
-               153           0 RESUME                   0
+                  00a0030000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d017409000000000000000000007c01a6010000ab0100
+                  000000000000007d027c025300
+               154           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               158           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Acquitision__scope)
                             14 LOAD_METHOD              1 (query)
                             36 LOAD_CONST               1 ('TRIG_MODE?')
                             38 PRECALL                  1
                             42 CALL                     1
-                            52 LOAD_METHOD              2 (removesuffix)
-                            74 LOAD_CONST               2 ('\n')
+                            52 LOAD_METHOD              2 (decode)
+                            74 LOAD_CONST               2 ('utf-8')
                             76 PRECALL                  1
                             80 CALL                     1
-                            90 STORE_FAST               1 (resp)
-               
-               158          92 LOAD_GLOBAL              7 (NULL + TriggerMode)
-                           104 LOAD_FAST                1 (resp)
-                           106 PRECALL                  1
-                           110 CALL                     1
-                           120 STORE_FAST               2 (mode)
+                            90 LOAD_METHOD              3 (strip)
+                           112 PRECALL                  0
+                           116 CALL                     0
+                           126 STORE_FAST               1 (resp)
+               
+               159         128 LOAD_GLOBAL              9 (NULL + TriggerMode)
+                           140 LOAD_FAST                1 (resp)
+                           142 PRECALL                  1
+                           146 CALL                     1
+                           156 STORE_FAST               2 (mode)
                
-               159         122 LOAD_FAST                2 (mode)
-                           124 RETURN_VALUE
+               160         158 LOAD_FAST                2 (mode)
+                           160 RETURN_VALUE
                consts
                   'Get the current specified trigger mode.'
                   'TRIG_MODE?'
-                  '\n'
-               names      ('_Acquitision__scope', 'query', 'removesuffix', 'TriggerMode')
+                  'utf-8'
+               names      ('_Acquitision__scope', 'query', 'decode', 'strip', 'TriggerMode')
                varnames   ('self', 'resp', 'mode')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
                name       'get_trigger_mode'
-               firstlineno 153
-               lnotab 0x02045a011e01
+               firstlineno 154
+               lnotab 0x02047e011e01
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'pyvisa', 'Resource', '__init__', 'arm_acquisition', 'int', 'enable_sequence', 'disable_sequence', 'stop_acquisition', 'wait_acquisition', 'float', 'set_time_div', 'get_time_div', 'set_volt_div', 'get_volt_div', 'set_trigger_delay', 'get_trigger_delay', 'Channel', 'set_trigger_level', 'get_trigger_level', 'trigger_normal', 'trigger_auto', 'trigger_single', 'trigger_stop', 'TriggerMode', 'get_trigger_mode')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
          name       'Acquitision'
-         firstlineno 5
+         firstlineno 6
          lnotab
             0x0a01040216030604100c0606060606060c0b0c070c0a0c070c110c0912
             120c0d0604060406040604
       'Acquitision'
-   names      ('pyvisa', 'maui_rc.datatypes', 'Acquitision')
+   names      ('pyvisa', 'maui_rc.datatypes', 'numpy', 'np', 'Acquitision')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/acquisition.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010803
+   lnotab 0x00ff0201080108010803
```

### Comparing `maui_rc-0.1.4/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc` & `maui_rc-0.1.5/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.4/maui_rc/subsystems/acquisition.py` & `maui_rc-0.1.5/maui_rc/subsystems/acquisition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pyvisa
 from maui_rc.datatypes import *
-from maui_rc.subsystems.wavedata import WaveformData
 import numpy as np
 
 
 class Acquitision:
     """Class that groups functions relating to acquisition."""
 
     def __init__(self, scope: pyvisa.Resource):
@@ -72,15 +71,15 @@
         cmd = "VOLT_DIV {:e}".format(float(value))
         self.__scope.write(cmd)
 
     def get_volt_div(self) -> float:
         """Gets the vertical sensitivity"""
 
         # query the device
-        volt_div = self.__scope.query("VOLT_DIV?").strip()
+        volt_div = self.__scope.query("VOLT_DIV?").decode('utf-8').strip()
         return float(volt_div)
 
     def set_trigger_delay(self, delay: int):
         """Sets the time at which the trigger is to occur.
 
         Arguments:
         - `delay`
@@ -96,15 +95,15 @@
         cmd = f"TRIG_DELAY {delay}"
         self.__scope.write(cmd)
 
     def get_trigger_delay(self) -> int:
         """Gets the time at which the trigger is to occur"""
 
         # query and parse the response
-        resp: str = self.__scope.query("TRIG_DELAY?").removesuffix("\n")
+        resp: str = self.__scope.query("TRIG_DELAY?").decode('utf-8').strip()
         delay = int(resp)
 
         return delay
 
     def set_trigger_level(self, level: float, trigger_source: Channel = None):
         """
         Adjusts the trigger level of the specified trigger source. If no trigger source is specified, the level is adjusted for all sources.
@@ -129,15 +128,15 @@
         Arguments:
         - `trigger_source` -> specified trigger source
         """
 
         # setup the query
         cmd = f"{Channel(trigger_source)}TRIG_LEVEL?"
         # run and parse the query
-        level = self.__scope.query(cmd).removesuffix("\n")
+        level = self.__scope.query(cmd).decode('utf-8').strip()
         return level
 
     def trigger_normal(self):
         """Set the trigger mode to normal."""
         self.__scope.write("TRIG_MODE NORMAL")
 
     def trigger_auto(self):
@@ -152,28 +151,10 @@
         """Set the trigger mode to stop. Stops acquisitions."""
         self.__scope.write("TRIG_MODE STOP")
 
     def get_trigger_mode(self) -> TriggerMode:
         """Get the current specified trigger mode."""
 
         # query and parse the response
-        resp: str = self.__scope.query("TRIG_MODE?").removesuffix("\n")
+        resp: str = self.__scope.query("TRIG_MODE?").decode('utf-8').strip()
         mode = TriggerMode(resp)
-        return mode
-
-    def get_waveform(self, channel: Channel) -> WaveformData:
-        """Extract the waveform from the scope and parse it."""
-
-        # Transfer the data blocks over
-        self.__scope.write(f"{channel}:WF? DESC")
-        desc = self.__scope.read_raw()
-        self.__scope.write(f"{channel}:WF? TEXT")
-        text = self.__scope.read_raw()
-        self.__scope.write(f"{channel}:WF? TIME")
-        time = self.__scope.read_raw()
-        self.__scope.write(f"{channel}:WF? DAT1")
-        dat1 = self.__scope.read_raw()
-        self.__scope.write(f"{channel}:WF? DAT2")
-        dat2 = self.__scope.read_raw()
-
-        # Parse it into waveform data
-        return WaveformData(desc, text, time, dat1, dat2)
+        return mode
```

### Comparing `maui_rc-0.1.4/maui_rc/subsystems/panelsetup.py` & `maui_rc-0.1.5/maui_rc/subsystems/panelsetup.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.4/maui_rc/subsystems/wavedata.py` & `maui_rc-0.1.5/maui_rc/subsystems/waveform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import pyvisa
 from enum import Enum
+from maui_rc.datatypes import Channel
 import struct
 import numpy as np
 
 class WaveformData:
+    """Class which parses and contains the complete waveform data."""
 
     class RecordType(Enum):
+        """The type of data of the waveform."""
+
         SingleSweep = 0
         Interleaved = 1
         Histogram = 2
         Graph = 3
         FilterCoefficient = 4
         Complex = 5
         Extrema = 6
@@ -16,28 +21,31 @@
         CenteredRIS = 8
         PeakDetect = 9
 
         def __str__(self):
             return self.name
         
     class ProcessingDone(Enum):
+        """The processing done on the waveform."""
+
         NoProcessing = 0
         FirFilter = 1
         Interpolated = 2
         Sparsed = 3
         AutoScaled = 4
         NoResult = 5
         Rolling = 6
         Cumulative = 7
     
         def __str__(self):
             return self.name
         
     class TimeBase(Enum):
-        """Enum identifying a specific timebase."""
+        """Available timebases on the WS3054z."""
+
         PS_1 = 0
         PS_2 = 1
         PS_5 = 2
         PS_10 = 3
         PS_20 = 4
         PS_50 = 5
         PS_100 = 6
@@ -105,14 +113,15 @@
                 case "MS": scale = 1.e-3
                 case "S": scale = 1.
                 case "KS": scale = 1.e3
             
             return scale * factor
 
     class Coupling(Enum):
+        """The coupling of a channel."""
         DC_50_Ohms = 0
         Ground = 1 | 3
         DC_1M_Ohm = 2
         AC_1MOhm = 4
 
         def __str__(self):
             return self.name 
@@ -322,16 +331,14 @@
         hour = self.__parse_to_int(data[9:10])
         day = self.__parse_to_int(data[10:11])
         month = self.__parse_to_int(data[11:12])
         year = self.__parse_to_int(data[12:14])
 
         return self.Timestamp(year, month, day, hour, minute, second)
 
-
-
     def __parse_to_int(self, data: bytes):
         """Parse a chunk of bytes into an integer."""
         if len(data) == 1:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}b", data)[0]
         if len(data) == 2:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}h", data)[0]
         elif len(data) == 4:
@@ -353,14 +360,16 @@
             # 64 bit
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}d", data)[0]
         else:
             # can't parse to float
             raise Exception("parsing error: data is not 32 or 64 bits, cannot parse to float")
 
     def __parse_wavedesc(self, desc_block: bytes):
+        """Take a waveform description block and parse it. This step is required before parsing the remaining blocks."""
+
         desc = desc_block
         # Get the descriptor name and template name
         self.descriptor_name = self.__parse_to_string(desc[:15])
         self.template_name = self.__parse_to_string(desc[16:31])
 
         # validate that the waveform uses the correct template
         if self.template_name != "LECROY_2_3":
@@ -442,14 +451,16 @@
         self.acquisition_vertical_offset = self.__parse_to_float(desc[340:344])
         self.wave_source = self.Source(self.__parse_to_int(desc[344:346]))
 
     def __parse_usertext(self, text_block: bytes):
         self.usertext = self.__parse_to_string(text_block)
 
     def __parse_horizontal_values(self, time_block: bytes):
+        """Parse the horizontal values of a waveform (i.e. the time (x) axis)."""
+
         # First, we need to check if we are in SingleSweep, Sequence or RIS
         if len(time_block.strip()) == 0:
             # The time block is ONLY used by Sequence OR RIS, so 
             # if it is empty, we MUST be in single sweep
             data = []
             for i in range(self.first_valid_point, self.last_valid_point):
                 data.append((self.horizontal_interval * i + self.horizontal_offset))
@@ -483,14 +494,16 @@
             for i in range(self.first_valid_point, self.last_valid_point):
                 m = i % self.ris_sweeps
                 j = i - m
                 data.append(self.horizontal_interval * j + ris_offset[m])
             self.data_x = np.array(data)
 
     def __parse_vertical_values(self, data_block_1: bytes, data_block_2: bytes):
+        """Parse the vertical values of a waveform (i.e. the amplitude (y) axis)"""
+
         # Parse the first block
         data_1 = []
         for i in range(self.first_valid_point, self.last_valid_point):
             start_pos = i * self.wf_datapoint_size
             data = data_block_1[start_pos:start_pos+self.wf_datapoint_size]
             data_1.append(self.__parse_to_int(data))
         data_1 = self.vertical_gain * np.array(data_1) - self.vertical_offset
@@ -515,16 +528,14 @@
                     data_2.append(self.__parse_to_int(data))
                 data_2 = self.vertical_gain * np.array(data_2) - self.vertical_offset
 
         if len(data_2) != 0:
             self.data_y = np.array([data_1, data_2])
         else:
             self.data_y = data_1
-
-
     
     def __init__(self, desc: bytes, text: bytes, time: bytes, dat1: bytes, dat2: bytes):
         # It begins with parsing the description
         # ----------
 
         
         # for the sake of shortening code, I'll put the blocks in a dict
@@ -551,7 +562,37 @@
         self.__parse_usertext(blocks["text"])
 
         # Parse the horizontal values
         self.__parse_horizontal_values(blocks["time"])
 
         # Parse the vertical values
         self.__parse_vertical_values(blocks["dat1"].strip(), blocks["dat2"].strip())
+
+class Waveform:
+    """Class used to transfer waveform data and parse it."""
+
+    def __init__(self, scope: pyvisa.Resource):
+        self.__scope = scope
+        self.__waveform_data = None
+
+    def transfer_from_device(self, channel: Channel):
+        """Load the waveform data into the Waveform class. This function must be called prior to other methods."""
+
+        # First, load all data blocks individually 
+        # (TODO remake the function such that all blocks can be parsed from the `ALL` data block.)
+        self.__scope.write(f"{channel}:WF? DESC")
+        desc = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? TEXT")
+        text = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? TIME")
+        time = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? DAT1")
+        dat1 = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? DAT2")
+        dat2 = self.__scope.read_raw()
+
+        # Parse the waveform
+        self.__waveform_data = WaveformData(desc, text, time, dat1, dat2)
+
+    def get_data(self) -> WaveformData:
+        """Get direct access to the WaveformData object."""
+        return self.__waveform_data
```

### Comparing `maui_rc-0.1.4/pyproject.toml` & `maui_rc-0.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maui-rc"
-version = "0.1.4"
+version = "0.1.5"
 description = "Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes."
 authors = ["Kristofer Karam <karamrkristofer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maui_rc"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -13,13 +13,13 @@
 pyvicp = "^1.1.0"
 black = "^23.7.0"
 pytest = "^7.4.0"
 numpy = "^1.25.1"
 zeroconf = "^0.71.0"
 psutil = "^5.9.5"
 pyusb = "^1.2.1"
-ieee754 = "^0.2"
+tqdm = "^4.65.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

