# Comparing `tmp/maui_rc-0.1.5.tar.gz` & `tmp/maui_rc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_rc-0.1.5.tar", max compression
+gzip compressed data, was "maui_rc-0.1.6.tar", max compression
```

## Comparing `maui_rc-0.1.5.tar` & `maui_rc-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.5/LICENSE
--rw-r--r--   0        0        0      759 2023-07-17 11:55:29.750458 maui_rc-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.5/maui_rc/__init__.py
--rw-r--r--   0        0        0     1537 2023-07-17 12:17:35.029616 maui_rc-0.1.5/maui_rc/datatypes.py
--rw-r--r--   0        0        0     2510 2023-07-17 12:15:56.144720 maui_rc-0.1.5/maui_rc/scope.py
--rw-r--r--   0        0        0     8686 2023-07-17 13:28:51.841986 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
--rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
--rw-r--r--   0        0        0    28616 2023-07-17 13:29:46.983870 maui_rc-0.1.5/maui_rc/subsystems/__pycache__/waveform.cpython-311.pyc
--rw-r--r--   0        0        0     5016 2023-07-17 12:15:27.478571 maui_rc-0.1.5/maui_rc/subsystems/acquisition.py
--rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.5/maui_rc/subsystems/panelsetup.py
--rw-r--r--   0        0        0    22653 2023-07-17 13:29:39.757355 maui_rc-0.1.5/maui_rc/subsystems/waveform.py
--rw-r--r--   0        0        0      555 2023-07-17 17:28:55.432869 maui_rc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 maui_rc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.6/LICENSE
+-rw-r--r--   0        0        0      759 2023-07-17 11:55:29.750458 maui_rc-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.6/maui_rc/__init__.py
+-rw-r--r--   0        0        0     1537 2023-07-17 12:17:35.029616 maui_rc-0.1.6/maui_rc/datatypes.py
+-rw-r--r--   0        0        0     2510 2023-07-17 12:15:56.144720 maui_rc-0.1.6/maui_rc/scope.py
+-rw-r--r--   0        0        0     8686 2023-07-17 13:28:51.841986 maui_rc-0.1.6/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
+-rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.6/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
+-rw-r--r--   0        0        0    29014 2023-07-17 18:39:11.132614 maui_rc-0.1.6/maui_rc/subsystems/__pycache__/waveform.cpython-311.pyc
+-rw-r--r--   0        0        0     5016 2023-07-17 12:15:27.478571 maui_rc-0.1.6/maui_rc/subsystems/acquisition.py
+-rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.6/maui_rc/subsystems/panelsetup.py
+-rw-r--r--   0        0        0    24003 2023-07-17 18:38:20.750287 maui_rc-0.1.6/maui_rc/subsystems/waveform.py
+-rw-r--r--   0        0        0      555 2023-07-17 18:39:31.478870 maui_rc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 maui_rc-0.1.6/PKG-INFO
```

### Comparing `maui_rc-0.1.5/LICENSE` & `maui_rc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/README.md` & `maui_rc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/datatypes.py` & `maui_rc-0.1.6/maui_rc/datatypes.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/scope.py` & `maui_rc-0.1.6/maui_rc/scope.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc` & `maui_rc-0.1.6/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc` & `maui_rc-0.1.6/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/__pycache__/waveform.cpython-311.pyc` & `maui_rc-0.1.6/maui_rc/subsystems/__pycache__/waveform.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x4342b564 (Mon Jul 17 13:29:39 2023 UTC)
-files sz: 22653
+moddate:  0x9c8ab564 (Mon Jul 17 18:38:20 2023 UTC)
+files sz: 24003
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064016c055a05640064016c065a07020047006404840064
-      05a6020000ab0200000000000000005a0802004700640684006407a60200
-      00ab0200000000000000005a0964015300
+      045a040100640064016c055a05640064016c065a07640064016c085a0802
+      004700640484006405a6020000ab0200000000000000005a090200470064
+      0684006407a6020000ab0200000000000000005a0a64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pyvisa)
                  8 STORE_NAME               0 (pyvisa)
    
@@ -38,42 +38,47 @@
                 40 STORE_NAME               5 (struct)
    
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               1 (None)
                 46 IMPORT_NAME              6 (numpy)
                 48 STORE_NAME               7 (np)
    
-     7          50 PUSH_NULL
-                52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               4 (<code object WaveformData, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 7>)
-                56 MAKE_FUNCTION            0
-                58 LOAD_CONST               5 ('WaveformData')
-                60 PRECALL                  2
-                64 CALL                     2
-                74 STORE_NAME               8 (WaveformData)
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               1 (None)
+                54 IMPORT_NAME              8 (pickle)
+                56 STORE_NAME               8 (pickle)
    
-   570          76 PUSH_NULL
-                78 LOAD_BUILD_CLASS
-                80 LOAD_CONST               6 (<code object Waveform, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 570>)
-                82 MAKE_FUNCTION            0
-                84 LOAD_CONST               7 ('Waveform')
-                86 PRECALL                  2
-                90 CALL                     2
-               100 STORE_NAME               9 (Waveform)
-               102 LOAD_CONST               1 (None)
-               104 RETURN_VALUE
+     8          58 PUSH_NULL
+                60 LOAD_BUILD_CLASS
+                62 LOAD_CONST               4 (<code object WaveformData, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 8>)
+                64 MAKE_FUNCTION            0
+                66 LOAD_CONST               5 ('WaveformData')
+                68 PRECALL                  2
+                72 CALL                     2
+                82 STORE_NAME               9 (WaveformData)
+   
+   597          84 PUSH_NULL
+                86 LOAD_BUILD_CLASS
+                88 LOAD_CONST               6 (<code object Waveform, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 597>)
+                90 MAKE_FUNCTION            0
+                92 LOAD_CONST               7 ('Waveform')
+                94 PRECALL                  2
+                98 CALL                     2
+               108 STORE_NAME              10 (Waveform)
+               110 LOAD_CONST               1 (None)
+               112 RETURN_VALUE
    consts
       0
       None
       ('Enum',)
       ('Channel',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 10
+         stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02550064015a03020047006402840064036504a6
             030000ab0300000000000000005a05020047006404840064056504a60300
             00ab0300000000000000005a06020047006406840064076504a6030000ab
             0300000000000000005a07020047006408840064096504a6030000ab0300
             000000000000005a0802004700640a8400640b6504a6030000ab03000000
@@ -98,578 +103,570 @@
             006505650d64383c00000009006506650d64393c0000000900650e650d64
             3a3c00000009006507650d643b3c00000009006508650d643c3c00000009
             00650f650d643d3c00000009006509650d643e3c00000009006510650d64
             3f3c0000000900650f650d64403c0000000900650f650d64413c00000009
             00650a650d64423c0000000900644365116602644484045a126443651166
             02644584045a13644365116602644684045a14644365116602644784045a
             15644865116602644984045a16644a65116602644b84045a17644c651166
-            02644d84045a18644e6511644f65116604645084045a1964516511645265
-            11645365116454651164556511660a645684045a1a64575300
-           7           0 RESUME                   0
+            02644d84045a18644e6511644f65116604645084045a1964436511660264
+            5184045a1a64525300
+           8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('WaveformData')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-           8          12 LOAD_CONST               1 ('Class which parses and contains the complete waveform data.')
+           9          12 LOAD_CONST               1 ('Class which parses and contains the complete waveform data.')
                       14 STORE_NAME               3 (__doc__)
          
-          10          16 PUSH_NULL
+          11          16 PUSH_NULL
                       18 LOAD_BUILD_CLASS
-                      20 LOAD_CONST               2 (<code object RecordType, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 10>)
+                      20 LOAD_CONST               2 (<code object RecordType, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 11>)
                       22 MAKE_FUNCTION            0
                       24 LOAD_CONST               3 ('RecordType')
                       26 LOAD_NAME                4 (Enum)
                       28 PRECALL                  3
                       32 CALL                     3
                       42 STORE_NAME               5 (RecordType)
          
-          27          44 PUSH_NULL
+          28          44 PUSH_NULL
                       46 LOAD_BUILD_CLASS
-                      48 LOAD_CONST               4 (<code object ProcessingDone, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 27>)
+                      48 LOAD_CONST               4 (<code object ProcessingDone, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 28>)
                       50 MAKE_FUNCTION            0
                       52 LOAD_CONST               5 ('ProcessingDone')
                       54 LOAD_NAME                4 (Enum)
                       56 PRECALL                  3
                       60 CALL                     3
                       70 STORE_NAME               6 (ProcessingDone)
          
-          42          72 PUSH_NULL
+          43          72 PUSH_NULL
                       74 LOAD_BUILD_CLASS
-                      76 LOAD_CONST               6 (<code object TimeBase, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 42>)
+                      76 LOAD_CONST               6 (<code object TimeBase, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 43>)
                       78 MAKE_FUNCTION            0
                       80 LOAD_CONST               7 ('TimeBase')
                       82 LOAD_NAME                4 (Enum)
                       84 PRECALL                  3
                       88 CALL                     3
                       98 STORE_NAME               7 (TimeBase)
          
-         119         100 PUSH_NULL
+         120         100 PUSH_NULL
                      102 LOAD_BUILD_CLASS
-                     104 LOAD_CONST               8 (<code object Coupling, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 119>)
+                     104 LOAD_CONST               8 (<code object Coupling, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 120>)
                      106 MAKE_FUNCTION            0
                      108 LOAD_CONST               9 ('Coupling')
                      110 LOAD_NAME                4 (Enum)
                      112 PRECALL                  3
                      116 CALL                     3
                      126 STORE_NAME               8 (Coupling)
          
-         129         128 PUSH_NULL
+         130         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST              10 (<code object VertGain, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 129>)
+                     132 LOAD_CONST              10 (<code object VertGain, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 130>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST              11 ('VertGain')
                      138 LOAD_NAME                4 (Enum)
                      140 PRECALL                  3
                      144 CALL                     3
                      154 STORE_NAME               9 (VertGain)
          
-         174         156 PUSH_NULL
+         175         156 PUSH_NULL
                      158 LOAD_BUILD_CLASS
-                     160 LOAD_CONST              12 (<code object Source, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 174>)
+                     160 LOAD_CONST              12 (<code object Source, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 175>)
                      162 MAKE_FUNCTION            0
                      164 LOAD_CONST              13 ('Source')
                      166 LOAD_NAME                4 (Enum)
                      168 PRECALL                  3
                      172 CALL                     3
                      182 STORE_NAME              10 (Source)
          
-         184         184 PUSH_NULL
+         185         184 PUSH_NULL
                      186 LOAD_BUILD_CLASS
-                     188 LOAD_CONST              14 (<code object Timestamp, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 184>)
+                     188 LOAD_CONST              14 (<code object Timestamp, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 185>)
                      190 MAKE_FUNCTION            0
                      192 LOAD_CONST              15 ('Timestamp')
                      194 PRECALL                  2
                      198 CALL                     2
                      208 STORE_NAME              11 (Timestamp)
          
-         198         210 LOAD_NAME               12 (str)
+         199         210 LOAD_NAME               12 (str)
                      212 LOAD_NAME               13 (__annotations__)
                      214 LOAD_CONST              16 ('byteorder')
                      216 STORE_SUBSCR
          
-         199         220 NOP
+         200         220 NOP
          
-         200         222 LOAD_NAME               14 (int)
+         201         222 LOAD_NAME               14 (int)
                      224 LOAD_NAME               13 (__annotations__)
                      226 LOAD_CONST              17 ('wf_datapoint_size')
                      228 STORE_SUBSCR
          
-         201         232 NOP
+         202         232 NOP
          
-         203         234 LOAD_NAME               14 (int)
+         204         234 LOAD_NAME               14 (int)
                      236 LOAD_NAME               13 (__annotations__)
                      238 LOAD_CONST              18 ('wave_desc_size')
                      240 STORE_SUBSCR
          
-         204         244 NOP
+         205         244 NOP
          
-         205         246 LOAD_NAME               14 (int)
+         206         246 LOAD_NAME               14 (int)
                      248 LOAD_NAME               13 (__annotations__)
                      250 LOAD_CONST              19 ('user_text_size')
                      252 STORE_SUBSCR
          
-         206         256 NOP
+         207         256 NOP
          
-         207         258 LOAD_NAME               14 (int)
+         208         258 LOAD_NAME               14 (int)
                      260 LOAD_NAME               13 (__annotations__)
                      262 LOAD_CONST              20 ('reserved_desc_size')
                      264 STORE_SUBSCR
          
-         208         268 NOP
+         209         268 NOP
          
-         209         270 LOAD_NAME               14 (int)
+         210         270 LOAD_NAME               14 (int)
                      272 LOAD_NAME               13 (__annotations__)
                      274 LOAD_CONST              21 ('trigtime_array_size')
                      276 STORE_SUBSCR
          
-         210         280 NOP
+         211         280 NOP
          
-         211         282 LOAD_NAME               14 (int)
+         212         282 LOAD_NAME               14 (int)
                      284 LOAD_NAME               13 (__annotations__)
                      286 LOAD_CONST              22 ('ris_time_array_size')
                      288 STORE_SUBSCR
          
-         212         292 NOP
+         213         292 NOP
          
-         213         294 LOAD_NAME               14 (int)
+         214         294 LOAD_NAME               14 (int)
                      296 LOAD_NAME               13 (__annotations__)
                      298 LOAD_CONST              23 ('res1_array_size')
                      300 STORE_SUBSCR
          
-         214         304 NOP
+         215         304 NOP
          
-         215         306 LOAD_NAME               14 (int)
+         216         306 LOAD_NAME               14 (int)
                      308 LOAD_NAME               13 (__annotations__)
                      310 LOAD_CONST              24 ('res2_array_size')
                      312 STORE_SUBSCR
          
-         216         316 NOP
+         217         316 NOP
          
-         217         318 LOAD_NAME               14 (int)
+         218         318 LOAD_NAME               14 (int)
                      320 LOAD_NAME               13 (__annotations__)
                      322 LOAD_CONST              25 ('res3_array_size')
                      324 STORE_SUBSCR
          
-         218         328 NOP
+         219         328 NOP
          
-         222         330 LOAD_NAME               12 (str)
+         223         330 LOAD_NAME               12 (str)
                      332 LOAD_NAME               13 (__annotations__)
                      334 LOAD_CONST              26 ('instrument_name')
                      336 STORE_SUBSCR
          
-         223         340 NOP
+         224         340 NOP
          
-         224         342 LOAD_NAME               14 (int)
+         225         342 LOAD_NAME               14 (int)
                      344 LOAD_NAME               13 (__annotations__)
                      346 LOAD_CONST              27 ('instrument_number')
                      348 STORE_SUBSCR
          
-         225         352 NOP
+         226         352 NOP
          
-         226         354 LOAD_NAME               12 (str)
+         227         354 LOAD_NAME               12 (str)
                      356 LOAD_NAME               13 (__annotations__)
                      358 LOAD_CONST              28 ('trace_label')
                      360 STORE_SUBSCR
          
-         227         364 NOP
+         228         364 NOP
          
-         228         366 LOAD_NAME               14 (int)
+         229         366 LOAD_NAME               14 (int)
                      368 LOAD_NAME               13 (__annotations__)
                      370 LOAD_CONST              29 ('reserved_1')
                      372 STORE_SUBSCR
          
-         229         376 NOP
+         230         376 NOP
          
-         230         378 LOAD_NAME               14 (int)
+         231         378 LOAD_NAME               14 (int)
                      380 LOAD_NAME               13 (__annotations__)
                      382 LOAD_CONST              30 ('reserved_2')
                      384 STORE_SUBSCR
          
-         231         388 NOP
+         232         388 NOP
          
-         235         390 LOAD_NAME               14 (int)
+         236         390 LOAD_NAME               14 (int)
                      392 LOAD_NAME               13 (__annotations__)
                      394 LOAD_CONST              31 ('wave_array_count')
                      396 STORE_SUBSCR
          
-         236         400 NOP
+         237         400 NOP
          
-         237         402 LOAD_NAME               14 (int)
+         238         402 LOAD_NAME               14 (int)
                      404 LOAD_NAME               13 (__annotations__)
                      406 LOAD_CONST              32 ('points_per_screen')
                      408 STORE_SUBSCR
          
-         238         412 NOP
+         239         412 NOP
          
-         239         414 LOAD_NAME               14 (int)
+         240         414 LOAD_NAME               14 (int)
                      416 LOAD_NAME               13 (__annotations__)
                      418 LOAD_CONST              33 ('first_valid_point')
                      420 STORE_SUBSCR
          
-         240         424 NOP
+         241         424 NOP
          
-         241         426 LOAD_NAME               14 (int)
+         242         426 LOAD_NAME               14 (int)
                      428 LOAD_NAME               13 (__annotations__)
                      430 LOAD_CONST              34 ('last_valid_point')
                      432 STORE_SUBSCR
          
-         242         436 NOP
+         243         436 NOP
          
-         243         438 LOAD_NAME               14 (int)
+         244         438 LOAD_NAME               14 (int)
                      440 LOAD_NAME               13 (__annotations__)
                      442 LOAD_CONST              35 ('first_point')
                      444 STORE_SUBSCR
          
-         244         448 NOP
+         245         448 NOP
          
-         245         450 LOAD_NAME               14 (int)
+         246         450 LOAD_NAME               14 (int)
                      452 LOAD_NAME               13 (__annotations__)
                      454 LOAD_CONST              36 ('sparsing_factor')
                      456 STORE_SUBSCR
          
-         246         460 NOP
+         247         460 NOP
          
-         247         462 LOAD_NAME               14 (int)
+         248         462 LOAD_NAME               14 (int)
                      464 LOAD_NAME               13 (__annotations__)
                      466 LOAD_CONST              37 ('segment_index')
                      468 STORE_SUBSCR
          
-         248         472 NOP
+         249         472 NOP
          
-         250         474 LOAD_NAME               14 (int)
+         251         474 LOAD_NAME               14 (int)
                      476 LOAD_NAME               13 (__annotations__)
                      478 LOAD_CONST              38 ('subarray_count')
                      480 STORE_SUBSCR
          
-         251         484 NOP
+         252         484 NOP
          
-         252         486 LOAD_NAME               14 (int)
+         253         486 LOAD_NAME               14 (int)
                      488 LOAD_NAME               13 (__annotations__)
                      490 LOAD_CONST              39 ('nominal_subarray_count')
                      492 STORE_SUBSCR
          
-         253         496 NOP
+         254         496 NOP
          
-         255         498 LOAD_NAME               14 (int)
+         256         498 LOAD_NAME               14 (int)
                      500 LOAD_NAME               13 (__annotations__)
                      502 LOAD_CONST              40 ('sweeps_per_acquisition')
                      504 STORE_SUBSCR
          
-         256         508 NOP
+         257         508 NOP
          
-         257         510 LOAD_NAME               14 (int)
+         258         510 LOAD_NAME               14 (int)
                      512 LOAD_NAME               13 (__annotations__)
                      514 LOAD_CONST              41 ('points_per_pair')
                      516 STORE_SUBSCR
          
-         258         520 NOP
+         259         520 NOP
          
-         259         522 LOAD_NAME               14 (int)
+         260         522 LOAD_NAME               14 (int)
                      524 LOAD_NAME               13 (__annotations__)
                      526 LOAD_CONST              42 ('pair_offset')
                      528 STORE_SUBSCR
          
-         260         532 NOP
+         261         532 NOP
          
-         262         534 LOAD_NAME               15 (float)
+         263         534 LOAD_NAME               15 (float)
                      536 LOAD_NAME               13 (__annotations__)
                      538 LOAD_CONST              43 ('vertical_gain')
                      540 STORE_SUBSCR
          
-         263         544 NOP
+         264         544 NOP
          
-         264         546 LOAD_NAME               15 (float)
+         265         546 LOAD_NAME               15 (float)
                      548 LOAD_NAME               13 (__annotations__)
                      550 LOAD_CONST              44 ('vertical_offset')
                      552 STORE_SUBSCR
          
-         265         556 NOP
+         266         556 NOP
          
-         266         558 LOAD_NAME               15 (float)
+         267         558 LOAD_NAME               15 (float)
                      560 LOAD_NAME               13 (__annotations__)
                      562 LOAD_CONST              45 ('max_value')
                      564 STORE_SUBSCR
          
-         267         568 NOP
+         268         568 NOP
          
-         268         570 LOAD_NAME               15 (float)
+         269         570 LOAD_NAME               15 (float)
                      572 LOAD_NAME               13 (__annotations__)
                      574 LOAD_CONST              46 ('min_value')
                      576 STORE_SUBSCR
          
-         269         580 NOP
+         270         580 NOP
          
-         271         582 LOAD_NAME               14 (int)
+         272         582 LOAD_NAME               14 (int)
                      584 LOAD_NAME               13 (__annotations__)
                      586 LOAD_CONST              47 ('nomimal_bits')
                      588 STORE_SUBSCR
          
-         272         592 NOP
+         273         592 NOP
          
-         274         594 LOAD_NAME               15 (float)
+         275         594 LOAD_NAME               15 (float)
                      596 LOAD_NAME               13 (__annotations__)
                      598 LOAD_CONST              48 ('horizontal_interval')
                      600 STORE_SUBSCR
          
-         275         604 NOP
+         276         604 NOP
          
-         276         606 LOAD_NAME               15 (float)
+         277         606 LOAD_NAME               15 (float)
                      608 LOAD_NAME               13 (__annotations__)
                      610 LOAD_CONST              49 ('horizontal_offset')
                      612 STORE_SUBSCR
          
-         277         616 NOP
+         278         616 NOP
          
-         279         618 LOAD_NAME               15 (float)
+         280         618 LOAD_NAME               15 (float)
                      620 LOAD_NAME               13 (__annotations__)
                      622 LOAD_CONST              50 ('pixel_offset')
                      624 STORE_SUBSCR
          
-         280         628 NOP
+         281         628 NOP
          
-         282         630 LOAD_NAME               12 (str)
+         283         630 LOAD_NAME               12 (str)
                      632 LOAD_NAME               13 (__annotations__)
                      634 LOAD_CONST              51 ('vertical_unit')
                      636 STORE_SUBSCR
          
-         283         640 NOP
+         284         640 NOP
          
-         284         642 LOAD_NAME               12 (str)
+         285         642 LOAD_NAME               12 (str)
                      644 LOAD_NAME               13 (__annotations__)
                      646 LOAD_CONST              52 ('horizontal_unit')
                      648 STORE_SUBSCR
          
-         285         652 NOP
+         286         652 NOP
          
-         286         654 LOAD_NAME               15 (float)
+         287         654 LOAD_NAME               15 (float)
                      656 LOAD_NAME               13 (__annotations__)
                      658 LOAD_CONST              53 ('horizontal_uncertainty')
                      660 STORE_SUBSCR
          
-         287         664 NOP
+         288         664 NOP
          
-         288         666 LOAD_NAME               11 (Timestamp)
+         289         666 LOAD_NAME               11 (Timestamp)
                      668 LOAD_NAME               13 (__annotations__)
                      670 LOAD_CONST              54 ('trigger_time')
                      672 STORE_SUBSCR
          
-         289         676 NOP
+         290         676 NOP
          
-         290         678 LOAD_NAME               15 (float)
+         291         678 LOAD_NAME               15 (float)
                      680 LOAD_NAME               13 (__annotations__)
                      682 LOAD_CONST              55 ('acquisition_duration')
                      684 STORE_SUBSCR
          
-         291         688 NOP
+         292         688 NOP
          
-         293         690 LOAD_NAME                5 (RecordType)
+         294         690 LOAD_NAME                5 (RecordType)
                      692 LOAD_NAME               13 (__annotations__)
                      694 LOAD_CONST              56 ('record_type')
                      696 STORE_SUBSCR
          
-         294         700 NOP
+         295         700 NOP
          
-         295         702 LOAD_NAME                6 (ProcessingDone)
+         296         702 LOAD_NAME                6 (ProcessingDone)
                      704 LOAD_NAME               13 (__annotations__)
                      706 LOAD_CONST              57 ('processing_done')
                      708 STORE_SUBSCR
          
-         296         712 NOP
+         297         712 NOP
          
-         298         714 LOAD_NAME               14 (int)
+         299         714 LOAD_NAME               14 (int)
                      716 LOAD_NAME               13 (__annotations__)
                      718 LOAD_CONST              58 ('ris_sweeps')
                      720 STORE_SUBSCR
          
-         299         724 NOP
+         300         724 NOP
          
-         303         726 LOAD_NAME                7 (TimeBase)
+         304         726 LOAD_NAME                7 (TimeBase)
                      728 LOAD_NAME               13 (__annotations__)
                      730 LOAD_CONST              59 ('timebase')
                      732 STORE_SUBSCR
          
-         304         736 NOP
+         305         736 NOP
          
-         305         738 LOAD_NAME                8 (Coupling)
+         306         738 LOAD_NAME                8 (Coupling)
                      740 LOAD_NAME               13 (__annotations__)
                      742 LOAD_CONST              60 ('vertical_coupling')
                      744 STORE_SUBSCR
          
-         306         748 NOP
+         307         748 NOP
          
-         307         750 LOAD_NAME               15 (float)
+         308         750 LOAD_NAME               15 (float)
                      752 LOAD_NAME               13 (__annotations__)
                      754 LOAD_CONST              61 ('probe_attenuation')
                      756 STORE_SUBSCR
          
-         308         760 NOP
+         309         760 NOP
          
-         309         762 LOAD_NAME                9 (VertGain)
+         310         762 LOAD_NAME                9 (VertGain)
                      764 LOAD_NAME               13 (__annotations__)
                      766 LOAD_CONST              62 ('fixed_vertical_gain')
                      768 STORE_SUBSCR
          
-         310         772 NOP
+         311         772 NOP
          
-         311         774 LOAD_NAME               16 (bool)
+         312         774 LOAD_NAME               16 (bool)
                      776 LOAD_NAME               13 (__annotations__)
                      778 LOAD_CONST              63 ('bandwidth_limit')
                      780 STORE_SUBSCR
          
-         312         784 NOP
+         313         784 NOP
          
-         313         786 LOAD_NAME               15 (float)
+         314         786 LOAD_NAME               15 (float)
                      788 LOAD_NAME               13 (__annotations__)
                      790 LOAD_CONST              64 ('vertical_vernier')
                      792 STORE_SUBSCR
          
-         314         796 NOP
+         315         796 NOP
          
-         315         798 LOAD_NAME               15 (float)
+         316         798 LOAD_NAME               15 (float)
                      800 LOAD_NAME               13 (__annotations__)
                      802 LOAD_CONST              65 ('acquisition_vertical_offset')
                      804 STORE_SUBSCR
          
-         316         808 NOP
+         317         808 NOP
          
-         317         810 LOAD_NAME               10 (Source)
+         318         810 LOAD_NAME               10 (Source)
                      812 LOAD_NAME               13 (__annotations__)
                      814 LOAD_CONST              66 ('wave_source')
                      816 STORE_SUBSCR
          
-         318         820 NOP
+         319         820 NOP
          
-         320         822 LOAD_CONST              67 ('data')
+         321         822 LOAD_CONST              67 ('data')
                      824 LOAD_NAME               17 (bytes)
                      826 BUILD_TUPLE              2
-                     828 LOAD_CONST              68 (<code object __parse_to_string, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 320>)
+                     828 LOAD_CONST              68 (<code object __parse_to_string, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 321>)
                      830 MAKE_FUNCTION            4 (annotations)
                      832 STORE_NAME              18 (_WaveformData__parse_to_string)
          
-         324         834 LOAD_CONST              67 ('data')
+         325         834 LOAD_CONST              67 ('data')
                      836 LOAD_NAME               17 (bytes)
                      838 BUILD_TUPLE              2
-                     840 LOAD_CONST              69 (<code object __parse_timestamp, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 324>)
+                     840 LOAD_CONST              69 (<code object __parse_timestamp, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 325>)
                      842 MAKE_FUNCTION            4 (annotations)
                      844 STORE_NAME              19 (_WaveformData__parse_timestamp)
          
-         338         846 LOAD_CONST              67 ('data')
+         339         846 LOAD_CONST              67 ('data')
                      848 LOAD_NAME               17 (bytes)
                      850 BUILD_TUPLE              2
-                     852 LOAD_CONST              70 (<code object __parse_to_int, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 338>)
+                     852 LOAD_CONST              70 (<code object __parse_to_int, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 339>)
                      854 MAKE_FUNCTION            4 (annotations)
                      856 STORE_NAME              20 (_WaveformData__parse_to_int)
          
-         353         858 LOAD_CONST              67 ('data')
+         354         858 LOAD_CONST              67 ('data')
                      860 LOAD_NAME               17 (bytes)
                      862 BUILD_TUPLE              2
-                     864 LOAD_CONST              71 (<code object __parse_to_float, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 353>)
+                     864 LOAD_CONST              71 (<code object __parse_to_float, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 354>)
                      866 MAKE_FUNCTION            4 (annotations)
                      868 STORE_NAME              21 (_WaveformData__parse_to_float)
          
-         366         870 LOAD_CONST              72 ('desc_block')
+         367         870 LOAD_CONST              72 ('desc_block')
                      872 LOAD_NAME               17 (bytes)
                      874 BUILD_TUPLE              2
-                     876 LOAD_CONST              73 (<code object __parse_wavedesc, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 366>)
+                     876 LOAD_CONST              73 (<code object __parse_wavedesc, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 367>)
                      878 MAKE_FUNCTION            4 (annotations)
                      880 STORE_NAME              22 (_WaveformData__parse_wavedesc)
          
-         454         882 LOAD_CONST              74 ('text_block')
+         455         882 LOAD_CONST              74 ('text_block')
                      884 LOAD_NAME               17 (bytes)
                      886 BUILD_TUPLE              2
-                     888 LOAD_CONST              75 (<code object __parse_usertext, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 454>)
+                     888 LOAD_CONST              75 (<code object __parse_usertext, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 455>)
                      890 MAKE_FUNCTION            4 (annotations)
                      892 STORE_NAME              23 (_WaveformData__parse_usertext)
          
-         457         894 LOAD_CONST              76 ('time_block')
+         458         894 LOAD_CONST              76 ('time_block')
                      896 LOAD_NAME               17 (bytes)
                      898 BUILD_TUPLE              2
-                     900 LOAD_CONST              77 (<code object __parse_horizontal_values, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 457>)
+                     900 LOAD_CONST              77 (<code object __parse_horizontal_values, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 458>)
                      902 MAKE_FUNCTION            4 (annotations)
                      904 STORE_NAME              24 (_WaveformData__parse_horizontal_values)
          
-         500         906 LOAD_CONST              78 ('data_block_1')
+         501         906 LOAD_CONST              78 ('data_block_1')
                      908 LOAD_NAME               17 (bytes)
                      910 LOAD_CONST              79 ('data_block_2')
                      912 LOAD_NAME               17 (bytes)
                      914 BUILD_TUPLE              4
-                     916 LOAD_CONST              80 (<code object __parse_vertical_values, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 500>)
+                     916 LOAD_CONST              80 (<code object __parse_vertical_values, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 501>)
                      918 MAKE_FUNCTION            4 (annotations)
                      920 STORE_NAME              25 (_WaveformData__parse_vertical_values)
          
-         536         922 LOAD_CONST              81 ('desc')
+         571         922 LOAD_CONST              67 ('data')
                      924 LOAD_NAME               17 (bytes)
-                     926 LOAD_CONST              82 ('text')
-                     928 LOAD_NAME               17 (bytes)
-                     930 LOAD_CONST              83 ('time')
-                     932 LOAD_NAME               17 (bytes)
-                     934 LOAD_CONST              84 ('dat1')
-                     936 LOAD_NAME               17 (bytes)
-                     938 LOAD_CONST              85 ('dat2')
-                     940 LOAD_NAME               17 (bytes)
-                     942 BUILD_TUPLE             10
-                     944 LOAD_CONST              86 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 536>)
-                     946 MAKE_FUNCTION            4 (annotations)
-                     948 STORE_NAME              26 (__init__)
-                     950 LOAD_CONST              87 (None)
-                     952 RETURN_VALUE
+                     926 BUILD_TUPLE              2
+                     928 LOAD_CONST              81 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 571>)
+                     930 MAKE_FUNCTION            4 (annotations)
+                     932 STORE_NAME              26 (__init__)
+                     934 LOAD_CONST              82 (None)
+                     936 RETURN_VALUE
          consts
             'WaveformData'
             'Class which parses and contains the complete waveform data.'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code
                   0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
                   0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c84005a
                   0e640d5300
-                10           0 RESUME                   0
+                11           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.RecordType')
                              8 STORE_NAME               2 (__qualname__)
                
-                11          10 LOAD_CONST               1 ('The type of data of the waveform.')
+                12          10 LOAD_CONST               1 ('The type of data of the waveform.')
                             12 STORE_NAME               3 (__doc__)
                
-                13          14 LOAD_CONST               2 (0)
+                14          14 LOAD_CONST               2 (0)
                             16 STORE_NAME               4 (SingleSweep)
                
-                14          18 LOAD_CONST               3 (1)
+                15          18 LOAD_CONST               3 (1)
                             20 STORE_NAME               5 (Interleaved)
                
-                15          22 LOAD_CONST               4 (2)
+                16          22 LOAD_CONST               4 (2)
                             24 STORE_NAME               6 (Histogram)
                
-                16          26 LOAD_CONST               5 (3)
+                17          26 LOAD_CONST               5 (3)
                             28 STORE_NAME               7 (Graph)
                
-                17          30 LOAD_CONST               6 (4)
+                18          30 LOAD_CONST               6 (4)
                             32 STORE_NAME               8 (FilterCoefficient)
                
-                18          34 LOAD_CONST               7 (5)
+                19          34 LOAD_CONST               7 (5)
                             36 STORE_NAME               9 (Complex)
                
-                19          38 LOAD_CONST               8 (6)
+                20          38 LOAD_CONST               8 (6)
                             40 STORE_NAME              10 (Extrema)
                
-                20          42 LOAD_CONST               9 (7)
+                21          42 LOAD_CONST               9 (7)
                             44 STORE_NAME              11 (SequenceObsolete)
                
-                21          46 LOAD_CONST              10 (8)
+                22          46 LOAD_CONST              10 (8)
                             48 STORE_NAME              12 (CenteredRIS)
                
-                22          50 LOAD_CONST              11 (9)
+                23          50 LOAD_CONST              11 (9)
                             52 STORE_NAME              13 (PeakDetect)
                
-                24          54 LOAD_CONST              12 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 24>)
+                25          54 LOAD_CONST              12 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 25>)
                             56 MAKE_FUNCTION            0
                             58 STORE_NAME              14 (__str__)
                             60 LOAD_CONST              13 (None)
                             62 RETURN_VALUE
                consts
                   'WaveformData.RecordType'
                   'The type of data of the waveform.'
@@ -685,81 +682,81 @@
                   9
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 1
                      flags     : 3
                      code 0x97007c006a0000000000000000005300
-                      24           0 RESUME                   0
+                      25           0 RESUME                   0
                      
-                      25           2 LOAD_FAST                0 (self)
+                      26           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 RETURN_VALUE
                      consts
                         None
                      names      ('name',)
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__str__'
-                     firstlineno 24
+                     firstlineno 25
                      lnotab 0x0201
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'SingleSweep', 'Interleaved', 'Histogram', 'Graph', 'FilterCoefficient', 'Complex', 'Extrema', 'SequenceObsolete', 'CenteredRIS', 'PeakDetect', '__str__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'RecordType'
-               firstlineno 10
+               firstlineno 11
                lnotab 0x0a0104020401040104010401040104010401040104010402
             'RecordType'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code
                   0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
                   0764065a0864075a0964085a0a64095a0b640a84005a0c640b5300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.ProcessingDone')
                              8 STORE_NAME               2 (__qualname__)
                
-                28          10 LOAD_CONST               1 ('The processing done on the waveform.')
+                29          10 LOAD_CONST               1 ('The processing done on the waveform.')
                             12 STORE_NAME               3 (__doc__)
                
-                30          14 LOAD_CONST               2 (0)
+                31          14 LOAD_CONST               2 (0)
                             16 STORE_NAME               4 (NoProcessing)
                
-                31          18 LOAD_CONST               3 (1)
+                32          18 LOAD_CONST               3 (1)
                             20 STORE_NAME               5 (FirFilter)
                
-                32          22 LOAD_CONST               4 (2)
+                33          22 LOAD_CONST               4 (2)
                             24 STORE_NAME               6 (Interpolated)
                
-                33          26 LOAD_CONST               5 (3)
+                34          26 LOAD_CONST               5 (3)
                             28 STORE_NAME               7 (Sparsed)
                
-                34          30 LOAD_CONST               6 (4)
+                35          30 LOAD_CONST               6 (4)
                             32 STORE_NAME               8 (AutoScaled)
                
-                35          34 LOAD_CONST               7 (5)
+                36          34 LOAD_CONST               7 (5)
                             36 STORE_NAME               9 (NoResult)
                
-                36          38 LOAD_CONST               8 (6)
+                37          38 LOAD_CONST               8 (6)
                             40 STORE_NAME              10 (Rolling)
                
-                37          42 LOAD_CONST               9 (7)
+                38          42 LOAD_CONST               9 (7)
                             44 STORE_NAME              11 (Cumulative)
                
-                39          46 LOAD_CONST              10 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 39>)
+                40          46 LOAD_CONST              10 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 40>)
                             48 MAKE_FUNCTION            0
                             50 STORE_NAME              12 (__str__)
                             52 LOAD_CONST              11 (None)
                             54 RETURN_VALUE
                consts
                   'WaveformData.ProcessingDone'
                   'The processing done on the waveform.'
@@ -773,37 +770,37 @@
                   7
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 1
                      flags     : 3
                      code 0x97007c006a0000000000000000005300
-                      39           0 RESUME                   0
+                      40           0 RESUME                   0
                      
-                      40           2 LOAD_FAST                0 (self)
+                      41           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 RETURN_VALUE
                      consts
                         None
                      names      ('name',)
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__str__'
-                     firstlineno 39
+                     firstlineno 40
                      lnotab 0x0201
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'NoProcessing', 'FirFilter', 'Interpolated', 'Sparsed', 'AutoScaled', 'NoResult', 'Rolling', 'Cumulative', '__str__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'ProcessingDone'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x0a01040204010401040104010401040104010402
             'ProcessingDone'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 2
                flags     : 0
@@ -812,174 +809,174 @@
                   0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
                   0d5a0f640e5a10640f5a1164105a1264115a1364125a1464135a1564145a
                   1664155a1764165a1864175a1964185a1a64195a1b641a5a1c641b5a1d64
                   1c5a1e641d5a1f641e5a20641f5a2164205a2264215a2364225a2464235a
                   2564245a2664255a2764265a2864275a2964285a2a64295a2b642a5a2c64
                   2b5a2d642c5a2e642d5a2f642e5a30642f5a3164305a3264315a3364325a
                   34643365356602643484045a3664355300
-                42           0 RESUME                   0
+                43           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.TimeBase')
                              8 STORE_NAME               2 (__qualname__)
                
-                43          10 LOAD_CONST               1 ('Available timebases on the WS3054z.')
+                44          10 LOAD_CONST               1 ('Available timebases on the WS3054z.')
                             12 STORE_NAME               3 (__doc__)
                
-                45          14 LOAD_CONST               2 (0)
+                46          14 LOAD_CONST               2 (0)
                             16 STORE_NAME               4 (PS_1)
                
-                46          18 LOAD_CONST               3 (1)
+                47          18 LOAD_CONST               3 (1)
                             20 STORE_NAME               5 (PS_2)
                
-                47          22 LOAD_CONST               4 (2)
+                48          22 LOAD_CONST               4 (2)
                             24 STORE_NAME               6 (PS_5)
                
-                48          26 LOAD_CONST               5 (3)
+                49          26 LOAD_CONST               5 (3)
                             28 STORE_NAME               7 (PS_10)
                
-                49          30 LOAD_CONST               6 (4)
+                50          30 LOAD_CONST               6 (4)
                             32 STORE_NAME               8 (PS_20)
                
-                50          34 LOAD_CONST               7 (5)
+                51          34 LOAD_CONST               7 (5)
                             36 STORE_NAME               9 (PS_50)
                
-                51          38 LOAD_CONST               8 (6)
+                52          38 LOAD_CONST               8 (6)
                             40 STORE_NAME              10 (PS_100)
                
-                52          42 LOAD_CONST               9 (7)
+                53          42 LOAD_CONST               9 (7)
                             44 STORE_NAME              11 (PS_200)
                
-                53          46 LOAD_CONST              10 (8)
+                54          46 LOAD_CONST              10 (8)
                             48 STORE_NAME              12 (PS_500)
                
-                54          50 LOAD_CONST              11 (9)
+                55          50 LOAD_CONST              11 (9)
                             52 STORE_NAME              13 (NS_1)
                
-                55          54 LOAD_CONST              12 (10)
+                56          54 LOAD_CONST              12 (10)
                             56 STORE_NAME              14 (NS_2)
                
-                56          58 LOAD_CONST              13 (11)
+                57          58 LOAD_CONST              13 (11)
                             60 STORE_NAME              15 (NS_5)
                
-                57          62 LOAD_CONST              14 (12)
+                58          62 LOAD_CONST              14 (12)
                             64 STORE_NAME              16 (NS_10)
                
-                58          66 LOAD_CONST              15 (13)
+                59          66 LOAD_CONST              15 (13)
                             68 STORE_NAME              17 (NS_20)
                
-                59          70 LOAD_CONST              16 (14)
+                60          70 LOAD_CONST              16 (14)
                             72 STORE_NAME              18 (NS_50)
                
-                60          74 LOAD_CONST              17 (15)
+                61          74 LOAD_CONST              17 (15)
                             76 STORE_NAME              19 (NS_100)
                
-                61          78 LOAD_CONST              18 (16)
+                62          78 LOAD_CONST              18 (16)
                             80 STORE_NAME              20 (NS_200)
                
-                62          82 LOAD_CONST              19 (17)
+                63          82 LOAD_CONST              19 (17)
                             84 STORE_NAME              21 (NS_500)
                
-                63          86 LOAD_CONST              20 (18)
+                64          86 LOAD_CONST              20 (18)
                             88 STORE_NAME              22 (US_1)
                
-                64          90 LOAD_CONST              21 (19)
+                65          90 LOAD_CONST              21 (19)
                             92 STORE_NAME              23 (US_2)
                
-                65          94 LOAD_CONST              22 (20)
+                66          94 LOAD_CONST              22 (20)
                             96 STORE_NAME              24 (US_5)
                
-                66          98 LOAD_CONST              23 (21)
+                67          98 LOAD_CONST              23 (21)
                            100 STORE_NAME              25 (US_10)
                
-                67         102 LOAD_CONST              24 (22)
+                68         102 LOAD_CONST              24 (22)
                            104 STORE_NAME              26 (US_20)
                
-                68         106 LOAD_CONST              25 (23)
+                69         106 LOAD_CONST              25 (23)
                            108 STORE_NAME              27 (US_50)
                
-                69         110 LOAD_CONST              26 (24)
+                70         110 LOAD_CONST              26 (24)
                            112 STORE_NAME              28 (US_100)
                
-                70         114 LOAD_CONST              27 (25)
+                71         114 LOAD_CONST              27 (25)
                            116 STORE_NAME              29 (US_200)
                
-                71         118 LOAD_CONST              28 (26)
+                72         118 LOAD_CONST              28 (26)
                            120 STORE_NAME              30 (US_500)
                
-                72         122 LOAD_CONST              29 (27)
+                73         122 LOAD_CONST              29 (27)
                            124 STORE_NAME              31 (MS_1)
                
-                73         126 LOAD_CONST              30 (28)
+                74         126 LOAD_CONST              30 (28)
                            128 STORE_NAME              32 (MS_2)
                
-                74         130 LOAD_CONST              31 (29)
+                75         130 LOAD_CONST              31 (29)
                            132 STORE_NAME              33 (MS_5)
                
-                75         134 LOAD_CONST              32 (30)
+                76         134 LOAD_CONST              32 (30)
                            136 STORE_NAME              34 (MS_10)
                
-                76         138 LOAD_CONST              33 (31)
+                77         138 LOAD_CONST              33 (31)
                            140 STORE_NAME              35 (MS_20)
                
-                77         142 LOAD_CONST              34 (32)
+                78         142 LOAD_CONST              34 (32)
                            144 STORE_NAME              36 (MS_50)
                
-                78         146 LOAD_CONST              35 (33)
+                79         146 LOAD_CONST              35 (33)
                            148 STORE_NAME              37 (MS_100)
                
-                79         150 LOAD_CONST              36 (34)
+                80         150 LOAD_CONST              36 (34)
                            152 STORE_NAME              38 (MS_200)
                
-                80         154 LOAD_CONST              37 (35)
+                81         154 LOAD_CONST              37 (35)
                            156 STORE_NAME              39 (MS_500)
                
-                81         158 LOAD_CONST              38 (36)
+                82         158 LOAD_CONST              38 (36)
                            160 STORE_NAME              40 (S_1)
                
-                82         162 LOAD_CONST              39 (37)
+                83         162 LOAD_CONST              39 (37)
                            164 STORE_NAME              41 (S_2)
                
-                83         166 LOAD_CONST              40 (38)
+                84         166 LOAD_CONST              40 (38)
                            168 STORE_NAME              42 (S_5)
                
-                84         170 LOAD_CONST              41 (39)
+                85         170 LOAD_CONST              41 (39)
                            172 STORE_NAME              43 (S_10)
                
-                85         174 LOAD_CONST              42 (40)
+                86         174 LOAD_CONST              42 (40)
                            176 STORE_NAME              44 (S_20)
                
-                86         178 LOAD_CONST              43 (41)
+                87         178 LOAD_CONST              43 (41)
                            180 STORE_NAME              45 (S_50)
                
-                87         182 LOAD_CONST              44 (42)
+                88         182 LOAD_CONST              44 (42)
                            184 STORE_NAME              46 (S_100)
                
-                88         186 LOAD_CONST              45 (43)
+                89         186 LOAD_CONST              45 (43)
                            188 STORE_NAME              47 (S_200)
                
-                89         190 LOAD_CONST              46 (44)
+                90         190 LOAD_CONST              46 (44)
                            192 STORE_NAME              48 (S_500)
                
-                90         194 LOAD_CONST              47 (45)
+                91         194 LOAD_CONST              47 (45)
                            196 STORE_NAME              49 (KS_1)
                
-                91         198 LOAD_CONST              48 (46)
+                92         198 LOAD_CONST              48 (46)
                            200 STORE_NAME              50 (KS_2)
                
-                92         202 LOAD_CONST              49 (47)
+                93         202 LOAD_CONST              49 (47)
                            204 STORE_NAME              51 (KS_5)
                
-                93         206 LOAD_CONST              50 (100)
+                94         206 LOAD_CONST              50 (100)
                            208 STORE_NAME              52 (EXTERNAL)
                
-                95         210 LOAD_CONST              51 ('return')
+                96         210 LOAD_CONST              51 ('return')
                            212 LOAD_NAME               53 (float)
                            214 BUILD_TUPLE              2
-                           216 LOAD_CONST              52 (<code object value, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 95>)
+                           216 LOAD_CONST              52 (<code object value, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 96>)
                            218 MAKE_FUNCTION            4 (annotations)
                            220 STORE_NAME              54 (value)
                            222 LOAD_CONST              53 (None)
                            224 RETURN_VALUE
                consts
                   'WaveformData.TimeBase'
                   'Available timebases on the WS3054z.'
@@ -1045,103 +1042,103 @@
                         03a6010000ab0100000000000000007d017c016404190000000000000000
                         007d027407000000000000000000007c01640519000000000000000000a6
                         010000ab0100000000000000007d037c02780164066b0200000000720401
                         0064077d026e2f780164086b02000000007204010064097d026e25780164
                         0a6b020000000072040100640b7d026e1b7801640c6b0200000000720401
                         00640d7d026e117801640e6b020000000072040100640f7d026e0764106b
                         0200000000720264117d027c027c037a0500005300
-                      95           0 RESUME                   0
+                      96           0 RESUME                   0
                      
-                      99           2 LOAD_FAST                0 (self)
+                     100           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 LOAD_CONST               1 ('EXTERNAL')
                                   16 COMPARE_OP               2 (==)
                                   22 POP_JUMP_FORWARD_IF_FALSE    15 (to 54)
                      
-                     100          24 LOAD_GLOBAL              3 (NULL + Exception)
+                     101          24 LOAD_GLOBAL              3 (NULL + Exception)
                                   36 LOAD_CONST               2 ('unimplemented error: external timebase is not implemented')
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 RAISE_VARARGS            1
                      
-                     103     >>   54 LOAD_FAST                0 (self)
+                     104     >>   54 LOAD_FAST                0 (self)
                                   56 LOAD_ATTR                0 (name)
                                   66 LOAD_METHOD              2 (split)
                                   88 LOAD_CONST               3 ('_')
                                   90 PRECALL                  1
                                   94 CALL                     1
                                  104 STORE_FAST               1 (name)
                      
-                     105         106 LOAD_FAST                1 (name)
+                     106         106 LOAD_FAST                1 (name)
                                  108 LOAD_CONST               4 (0)
                                  110 BINARY_SUBSCR
                                  120 STORE_FAST               2 (scale)
                      
-                     107         122 LOAD_GLOBAL              7 (NULL + float)
+                     108         122 LOAD_GLOBAL              7 (NULL + float)
                                  134 LOAD_FAST                1 (name)
                                  136 LOAD_CONST               5 (1)
                                  138 BINARY_SUBSCR
                                  148 PRECALL                  1
                                  152 CALL                     1
                                  162 STORE_FAST               3 (factor)
                      
-                     109         164 LOAD_FAST                2 (scale)
+                     110         164 LOAD_FAST                2 (scale)
                      
-                     110         166 COPY                     1
+                     111         166 COPY                     1
                                  168 LOAD_CONST               6 ('PS')
                                  170 COMPARE_OP               2 (==)
                                  176 POP_JUMP_FORWARD_IF_FALSE     4 (to 186)
                                  178 POP_TOP
                                  180 LOAD_CONST               7 (1e-12)
                                  182 STORE_FAST               2 (scale)
                                  184 JUMP_FORWARD            47 (to 280)
                      
-                     111     >>  186 COPY                     1
+                     112     >>  186 COPY                     1
                                  188 LOAD_CONST               8 ('NS')
                                  190 COMPARE_OP               2 (==)
                                  196 POP_JUMP_FORWARD_IF_FALSE     4 (to 206)
                                  198 POP_TOP
                                  200 LOAD_CONST               9 (1e-09)
                                  202 STORE_FAST               2 (scale)
                                  204 JUMP_FORWARD            37 (to 280)
                      
-                     112     >>  206 COPY                     1
+                     113     >>  206 COPY                     1
                                  208 LOAD_CONST              10 ('US')
                                  210 COMPARE_OP               2 (==)
                                  216 POP_JUMP_FORWARD_IF_FALSE     4 (to 226)
                                  218 POP_TOP
                                  220 LOAD_CONST              11 (1e-06)
                                  222 STORE_FAST               2 (scale)
                                  224 JUMP_FORWARD            27 (to 280)
                      
-                     113     >>  226 COPY                     1
+                     114     >>  226 COPY                     1
                                  228 LOAD_CONST              12 ('MS')
                                  230 COMPARE_OP               2 (==)
                                  236 POP_JUMP_FORWARD_IF_FALSE     4 (to 246)
                                  238 POP_TOP
                                  240 LOAD_CONST              13 (0.001)
                                  242 STORE_FAST               2 (scale)
                                  244 JUMP_FORWARD            17 (to 280)
                      
-                     114     >>  246 COPY                     1
+                     115     >>  246 COPY                     1
                                  248 LOAD_CONST              14 ('S')
                                  250 COMPARE_OP               2 (==)
                                  256 POP_JUMP_FORWARD_IF_FALSE     4 (to 266)
                                  258 POP_TOP
                                  260 LOAD_CONST              15 (1.0)
                                  262 STORE_FAST               2 (scale)
                                  264 JUMP_FORWARD             7 (to 280)
                      
-                     115     >>  266 LOAD_CONST              16 ('KS')
+                     116     >>  266 LOAD_CONST              16 ('KS')
                                  268 COMPARE_OP               2 (==)
                                  274 POP_JUMP_FORWARD_IF_FALSE     2 (to 280)
                                  276 LOAD_CONST              17 (1000.0)
                                  278 STORE_FAST               2 (scale)
                      
-                     117     >>  280 LOAD_FAST                2 (scale)
+                     118     >>  280 LOAD_FAST                2 (scale)
                                  282 LOAD_FAST                3 (factor)
                                  284 BINARY_OP                5 (*)
                                  288 RETURN_VALUE
                      consts
                         'Return the timebase in seconds.'
                         'EXTERNAL'
                         'unimplemented error: external timebase is not implemented'
@@ -1162,60 +1159,60 @@
                         1000.0
                      names      ('name', 'Exception', 'split', 'float')
                      varnames   ('self', 'name', 'scale', 'factor')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       'value'
-                     firstlineno 95
+                     firstlineno 96
                      lnotab 0x020416011e03340210022a020201140114011401140114010e02
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'PS_1', 'PS_2', 'PS_5', 'PS_10', 'PS_20', 'PS_50', 'PS_100', 'PS_200', 'PS_500', 'NS_1', 'NS_2', 'NS_5', 'NS_10', 'NS_20', 'NS_50', 'NS_100', 'NS_200', 'NS_500', 'US_1', 'US_2', 'US_5', 'US_10', 'US_20', 'US_50', 'US_100', 'US_200', 'US_500', 'MS_1', 'MS_2', 'MS_5', 'MS_10', 'MS_20', 'MS_50', 'MS_100', 'MS_200', 'MS_500', 'S_1', 'S_2', 'S_5', 'S_10', 'S_20', 'S_50', 'S_100', 'S_200', 'S_500', 'KS_1', 'KS_2', 'KS_5', 'EXTERNAL', 'float', 'value')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'TimeBase'
-               firstlineno 42
+               firstlineno 43
                lnotab
                   0x0a01040204010401040104010401040104010401040104010401040104
                   010401040104010401040104010401040104010401040104010401040104
                   010401040104010401040104010401040104010401040104010401040104
                   01040104010401040104010402
             'TimeBase'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code
                   0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
                   07640684005a0864075300
-               119           0 RESUME                   0
+               120           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.Coupling')
                              8 STORE_NAME               2 (__qualname__)
                
-               120          10 LOAD_CONST               1 ('The coupling of a channel.')
+               121          10 LOAD_CONST               1 ('The coupling of a channel.')
                             12 STORE_NAME               3 (__doc__)
                
-               121          14 LOAD_CONST               2 (0)
+               122          14 LOAD_CONST               2 (0)
                             16 STORE_NAME               4 (DC_50_Ohms)
                
-               122          18 LOAD_CONST               3 (3)
+               123          18 LOAD_CONST               3 (3)
                             20 STORE_NAME               5 (Ground)
                
-               123          22 LOAD_CONST               4 (2)
+               124          22 LOAD_CONST               4 (2)
                             24 STORE_NAME               6 (DC_1M_Ohm)
                
-               124          26 LOAD_CONST               5 (4)
+               125          26 LOAD_CONST               5 (4)
                             28 STORE_NAME               7 (AC_1MOhm)
                
-               126          30 LOAD_CONST               6 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 126>)
+               127          30 LOAD_CONST               6 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 127>)
                             32 MAKE_FUNCTION            0
                             34 STORE_NAME               8 (__str__)
                             36 LOAD_CONST               7 (None)
                             38 RETURN_VALUE
                consts
                   'WaveformData.Coupling'
                   'The coupling of a channel.'
@@ -1225,144 +1222,144 @@
                   4
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 1
                      flags     : 3
                      code 0x97007c006a0000000000000000005300
-                     126           0 RESUME                   0
+                     127           0 RESUME                   0
                      
-                     127           2 LOAD_FAST                0 (self)
+                     128           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 RETURN_VALUE
                      consts
                         None
                      names      ('name',)
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__str__'
-                     firstlineno 126
+                     firstlineno 127
                      lnotab 0x0201
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'DC_50_Ohms', 'Ground', 'DC_1M_Ohm', 'AC_1MOhm', '__str__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'Coupling'
-               firstlineno 119
+               firstlineno 120
                lnotab 0x0a0104010401040104010402
             'Coupling'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 2
                flags     : 0
                code
                   0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
                   0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
                   0d5a0f640e5a10640f5a1164105a1264115a1364125a1464135a1564145a
                   1664155a1764165a1864175a1964185a1a64195a1b641a5a1c641b5a1d64
                   1c5a1e641d651f6602641e84045a20641f5300
-               129           0 RESUME                   0
+               130           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.VertGain')
                              8 STORE_NAME               2 (__qualname__)
                
-               130          10 LOAD_CONST               1 (0)
+               131          10 LOAD_CONST               1 (0)
                             12 STORE_NAME               3 (UV_1)
                
-               131          14 LOAD_CONST               2 (1)
+               132          14 LOAD_CONST               2 (1)
                             16 STORE_NAME               4 (UV_2)
                
-               132          18 LOAD_CONST               3 (2)
+               133          18 LOAD_CONST               3 (2)
                             20 STORE_NAME               5 (UV_5)
                
-               133          22 LOAD_CONST               4 (3)
+               134          22 LOAD_CONST               4 (3)
                             24 STORE_NAME               6 (UV_10)
                
-               134          26 LOAD_CONST               5 (4)
+               135          26 LOAD_CONST               5 (4)
                             28 STORE_NAME               7 (UV_20)
                
-               135          30 LOAD_CONST               6 (5)
+               136          30 LOAD_CONST               6 (5)
                             32 STORE_NAME               8 (UV_50)
                
-               136          34 LOAD_CONST               7 (6)
+               137          34 LOAD_CONST               7 (6)
                             36 STORE_NAME               9 (UV_100)
                
-               137          38 LOAD_CONST               8 (7)
+               138          38 LOAD_CONST               8 (7)
                             40 STORE_NAME              10 (UV_200)
                
-               138          42 LOAD_CONST               9 (8)
+               139          42 LOAD_CONST               9 (8)
                             44 STORE_NAME              11 (UV_500)
                
-               139          46 LOAD_CONST              10 (9)
+               140          46 LOAD_CONST              10 (9)
                             48 STORE_NAME              12 (MV_1)
                
-               140          50 LOAD_CONST              11 (10)
+               141          50 LOAD_CONST              11 (10)
                             52 STORE_NAME              13 (MV_2)
                
-               141          54 LOAD_CONST              12 (11)
+               142          54 LOAD_CONST              12 (11)
                             56 STORE_NAME              14 (MV_5)
                
-               142          58 LOAD_CONST              13 (12)
+               143          58 LOAD_CONST              13 (12)
                             60 STORE_NAME              15 (MV_10)
                
-               143          62 LOAD_CONST              14 (13)
+               144          62 LOAD_CONST              14 (13)
                             64 STORE_NAME              16 (MV_20)
                
-               144          66 LOAD_CONST              15 (14)
+               145          66 LOAD_CONST              15 (14)
                             68 STORE_NAME              17 (MV_50)
                
-               145          70 LOAD_CONST              16 (15)
+               146          70 LOAD_CONST              16 (15)
                             72 STORE_NAME              18 (MV_100)
                
-               146          74 LOAD_CONST              17 (16)
+               147          74 LOAD_CONST              17 (16)
                             76 STORE_NAME              19 (MV_200)
                
-               147          78 LOAD_CONST              18 (17)
+               148          78 LOAD_CONST              18 (17)
                             80 STORE_NAME              20 (MV_500)
                
-               148          82 LOAD_CONST              19 (18)
+               149          82 LOAD_CONST              19 (18)
                             84 STORE_NAME              21 (V_1)
                
-               149          86 LOAD_CONST              20 (19)
+               150          86 LOAD_CONST              20 (19)
                             88 STORE_NAME              22 (V_2)
                
-               150          90 LOAD_CONST              21 (20)
+               151          90 LOAD_CONST              21 (20)
                             92 STORE_NAME              23 (V_5)
                
-               151          94 LOAD_CONST              22 (21)
+               152          94 LOAD_CONST              22 (21)
                             96 STORE_NAME              24 (V_10)
                
-               152          98 LOAD_CONST              23 (22)
+               153          98 LOAD_CONST              23 (22)
                            100 STORE_NAME              25 (V_20)
                
-               153         102 LOAD_CONST              24 (23)
+               154         102 LOAD_CONST              24 (23)
                            104 STORE_NAME              26 (V_50)
                
-               154         106 LOAD_CONST              25 (24)
+               155         106 LOAD_CONST              25 (24)
                            108 STORE_NAME              27 (V_100)
                
-               155         110 LOAD_CONST              26 (25)
+               156         110 LOAD_CONST              26 (25)
                            112 STORE_NAME              28 (V_200)
                
-               156         114 LOAD_CONST              27 (26)
+               157         114 LOAD_CONST              27 (26)
                            116 STORE_NAME              29 (V_500)
                
-               157         118 LOAD_CONST              28 (27)
+               158         118 LOAD_CONST              28 (27)
                            120 STORE_NAME              30 (KV_1)
                
-               159         122 LOAD_CONST              29 ('return')
+               160         122 LOAD_CONST              29 ('return')
                            124 LOAD_NAME               31 (float)
                            126 BUILD_TUPLE              2
-                           128 LOAD_CONST              30 (<code object value, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 159>)
+                           128 LOAD_CONST              30 (<code object value, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 160>)
                            130 MAKE_FUNCTION            4 (annotations)
                            132 STORE_NAME              32 (value)
                            134 LOAD_CONST              31 (None)
                            136 RETURN_VALUE
                consts
                   'WaveformData.VertGain'
                   0
@@ -1403,73 +1400,73 @@
                         0x97007c006a000000000000000000a00100000000000000000000000000
                         000000000000006401a6010000ab0100000000000000007d017c01640219
                         0000000000000000007d027405000000000000000000007c016403190000
                         00000000000000a6010000ab0100000000000000007d037c02780164046b
                         02000000007204010064057d026e1b780164066b02000000007204010064
                         077d026e11780164086b02000000007204010064097d026e07640a6b0200
                         0000007202640b7d027c027c037a0500005300
-                     159           0 RESUME                   0
+                     160           0 RESUME                   0
                      
-                     162           2 LOAD_FAST                0 (self)
+                     163           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 LOAD_METHOD              1 (split)
                                   36 LOAD_CONST               1 ('_')
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 STORE_FAST               1 (name)
                      
-                     163          54 LOAD_FAST                1 (name)
+                     164          54 LOAD_FAST                1 (name)
                                   56 LOAD_CONST               2 (0)
                                   58 BINARY_SUBSCR
                                   68 STORE_FAST               2 (scale)
                      
-                     164          70 LOAD_GLOBAL              5 (NULL + float)
+                     165          70 LOAD_GLOBAL              5 (NULL + float)
                                   82 LOAD_FAST                1 (name)
                                   84 LOAD_CONST               3 (1)
                                   86 BINARY_SUBSCR
                                   96 PRECALL                  1
                                  100 CALL                     1
                                  110 STORE_FAST               3 (factor)
                      
-                     166         112 LOAD_FAST                2 (scale)
+                     167         112 LOAD_FAST                2 (scale)
                      
-                     167         114 COPY                     1
+                     168         114 COPY                     1
                                  116 LOAD_CONST               4 ('UV')
                                  118 COMPARE_OP               2 (==)
                                  124 POP_JUMP_FORWARD_IF_FALSE     4 (to 134)
                                  126 POP_TOP
                                  128 LOAD_CONST               5 (1e-06)
                                  130 STORE_FAST               2 (scale)
                                  132 JUMP_FORWARD            27 (to 188)
                      
-                     168     >>  134 COPY                     1
+                     169     >>  134 COPY                     1
                                  136 LOAD_CONST               6 ('MV')
                                  138 COMPARE_OP               2 (==)
                                  144 POP_JUMP_FORWARD_IF_FALSE     4 (to 154)
                                  146 POP_TOP
                                  148 LOAD_CONST               7 (0.001)
                                  150 STORE_FAST               2 (scale)
                                  152 JUMP_FORWARD            17 (to 188)
                      
-                     169     >>  154 COPY                     1
+                     170     >>  154 COPY                     1
                                  156 LOAD_CONST               8 ('V')
                                  158 COMPARE_OP               2 (==)
                                  164 POP_JUMP_FORWARD_IF_FALSE     4 (to 174)
                                  166 POP_TOP
                                  168 LOAD_CONST               9 (1.0)
                                  170 STORE_FAST               2 (scale)
                                  172 JUMP_FORWARD             7 (to 188)
                      
-                     170     >>  174 LOAD_CONST              10 ('KV')
+                     171     >>  174 LOAD_CONST              10 ('KV')
                                  176 COMPARE_OP               2 (==)
                                  182 POP_JUMP_FORWARD_IF_FALSE     2 (to 188)
                                  184 LOAD_CONST              11 (1000.0)
                                  186 STORE_FAST               2 (scale)
                      
-                     172     >>  188 LOAD_FAST                2 (scale)
+                     173     >>  188 LOAD_FAST                2 (scale)
                                  190 LOAD_FAST                3 (factor)
                                  192 BINARY_OP                5 (*)
                                  196 RETURN_VALUE
                      consts
                         'Return the vertical gain in volts.'
                         '_'
                         0
@@ -1484,58 +1481,58 @@
                         1000.0
                      names      ('name', 'split', 'float')
                      varnames   ('self', 'name', 'scale', 'factor')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       'value'
-                     firstlineno 159
+                     firstlineno 160
                      lnotab 0x0203340110012a0202011401140114010e02
                   None
                names      ('__name__', '__module__', '__qualname__', 'UV_1', 'UV_2', 'UV_5', 'UV_10', 'UV_20', 'UV_50', 'UV_100', 'UV_200', 'UV_500', 'MV_1', 'MV_2', 'MV_5', 'MV_10', 'MV_20', 'MV_50', 'MV_100', 'MV_200', 'MV_500', 'V_1', 'V_2', 'V_5', 'V_10', 'V_20', 'V_50', 'V_100', 'V_200', 'V_500', 'KV_1', 'float', 'value')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'VertGain'
-               firstlineno 129
+               firstlineno 130
                lnotab
                   0x0a01040104010401040104010401040104010401040104010401040104
                   0104010401040104010401040104010401040104010401040104010402
             'VertGain'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code
                   0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
                   07640684005a0864075300
-               174           0 RESUME                   0
+               175           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.Source')
                              8 STORE_NAME               2 (__qualname__)
                
-               175          10 LOAD_CONST               1 (0)
+               176          10 LOAD_CONST               1 (0)
                             12 STORE_NAME               3 (CHANNEL_1)
                
-               176          14 LOAD_CONST               2 (1)
+               177          14 LOAD_CONST               2 (1)
                             16 STORE_NAME               4 (CHANNEL_2)
                
-               177          18 LOAD_CONST               3 (2)
+               178          18 LOAD_CONST               3 (2)
                             20 STORE_NAME               5 (CHANNEL_3)
                
-               178          22 LOAD_CONST               4 (3)
+               179          22 LOAD_CONST               4 (3)
                             24 STORE_NAME               6 (CHANNEL_4)
                
-               179          26 LOAD_CONST               5 (9)
+               180          26 LOAD_CONST               5 (9)
                             28 STORE_NAME               7 (UNKNOWN)
                
-               181          30 LOAD_CONST               6 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 181>)
+               182          30 LOAD_CONST               6 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 182>)
                             32 MAKE_FUNCTION            0
                             34 STORE_NAME               8 (__str__)
                             36 LOAD_CONST               7 (None)
                             38 RETURN_VALUE
                consts
                   'WaveformData.Source'
                   0
@@ -1545,71 +1542,71 @@
                   9
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 1
                      flags     : 3
                      code 0x97007c006a0000000000000000005300
-                     181           0 RESUME                   0
+                     182           0 RESUME                   0
                      
-                     182           2 LOAD_FAST                0 (self)
+                     183           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (name)
                                   14 RETURN_VALUE
                      consts
                         None
                      names      ('name',)
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__str__'
-                     firstlineno 181
+                     firstlineno 182
                      lnotab 0x0201
                   None
                names      ('__name__', '__module__', '__qualname__', 'CHANNEL_1', 'CHANNEL_2', 'CHANNEL_3', 'CHANNEL_4', 'UNKNOWN', '__str__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'Source'
-               firstlineno 174
+               firstlineno 175
                lnotab 0x0a0104010401040104010402
             'Source'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 12
                flags     : 0
                code
                   0x970065005a0164005a0264016503640265036403650364046503640565
                   0364066504660c640784045a05640884005a0664095300
-               184           0 RESUME                   0
+               185           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('WaveformData.Timestamp')
                              8 STORE_NAME               2 (__qualname__)
                
-               185          10 LOAD_CONST               1 ('year')
+               186          10 LOAD_CONST               1 ('year')
                             12 LOAD_NAME                3 (int)
                             14 LOAD_CONST               2 ('month')
                             16 LOAD_NAME                3 (int)
                             18 LOAD_CONST               3 ('day')
                             20 LOAD_NAME                3 (int)
                             22 LOAD_CONST               4 ('hour')
                             24 LOAD_NAME                3 (int)
                             26 LOAD_CONST               5 ('minute')
                             28 LOAD_NAME                3 (int)
                             30 LOAD_CONST               6 ('second')
                             32 LOAD_NAME                4 (float)
                             34 BUILD_TUPLE             12
-                            36 LOAD_CONST               7 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 185>)
+                            36 LOAD_CONST               7 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 186>)
                             38 MAKE_FUNCTION            4 (annotations)
                             40 STORE_NAME               5 (__init__)
                
-               193          42 LOAD_CONST               8 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 193>)
+               194          42 LOAD_CONST               8 (<code object __str__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 194>)
                             44 MAKE_FUNCTION            0
                             46 STORE_NAME               6 (__str__)
                             48 LOAD_CONST               9 (None)
                             50 RETURN_VALUE
                consts
                   'WaveformData.Timestamp'
                   'year'
@@ -1624,64 +1621,64 @@
                      stacksize : 2
                      flags     : 3
                      code
                         0x97007c017c005f0000000000000000007c027c005f0100000000000000
                         007c037c005f0200000000000000007c047c005f0300000000000000007c
                         057c005f0400000000000000007c067c005f050000000000000000640053
                         00
-                     185           0 RESUME                   0
+                     186           0 RESUME                   0
                      
-                     186           2 LOAD_FAST                1 (year)
+                     187           2 LOAD_FAST                1 (year)
                                    4 LOAD_FAST                0 (self)
                                    6 STORE_ATTR               0 (year)
                      
-                     187          16 LOAD_FAST                2 (month)
+                     188          16 LOAD_FAST                2 (month)
                                   18 LOAD_FAST                0 (self)
                                   20 STORE_ATTR               1 (month)
                      
-                     188          30 LOAD_FAST                3 (day)
+                     189          30 LOAD_FAST                3 (day)
                                   32 LOAD_FAST                0 (self)
                                   34 STORE_ATTR               2 (day)
                      
-                     189          44 LOAD_FAST                4 (hour)
+                     190          44 LOAD_FAST                4 (hour)
                                   46 LOAD_FAST                0 (self)
                                   48 STORE_ATTR               3 (hour)
                      
-                     190          58 LOAD_FAST                5 (minute)
+                     191          58 LOAD_FAST                5 (minute)
                                   60 LOAD_FAST                0 (self)
                                   62 STORE_ATTR               4 (minute)
                      
-                     191          72 LOAD_FAST                6 (second)
+                     192          72 LOAD_FAST                6 (second)
                                   74 LOAD_FAST                0 (self)
                                   76 STORE_ATTR               5 (second)
                                   86 LOAD_CONST               0 (None)
                                   88 RETURN_VALUE
                      consts
                         None
                      names      ('year', 'month', 'day', 'hour', 'minute', 'second')
                      varnames   ('self', 'year', 'month', 'day', 'hour', 'minute', 'second')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__init__'
-                     firstlineno 185
+                     firstlineno 186
                      lnotab 0x02010e010e010e010e010e01
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 11
                      flags     : 3
                      code
                         0x97007c006a0000000000000000009b0064017c006a0100000000000000
                         009b0064017c006a0200000000000000009b0064027c006a030000000000
                         0000009b0064037c006a0400000000000000009b0064037c006a05000000
                         00000000009b009d0b5300
-                     193           0 RESUME                   0
+                     194           0 RESUME                   0
                      
-                     194           2 LOAD_FAST                0 (self)
+                     195           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (year)
                                   14 FORMAT_VALUE             0
                                   16 LOAD_CONST               1 ('-')
                                   18 LOAD_FAST                0 (self)
                                   20 LOAD_ATTR                1 (month)
                                   30 FORMAT_VALUE             0
                                   32 LOAD_CONST               1 ('-')
@@ -1709,24 +1706,24 @@
                         ':'
                      names      ('year', 'month', 'day', 'hour', 'minute', 'second')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                      name       '__str__'
-                     firstlineno 193
+                     firstlineno 194
                      lnotab 0x0201
                   None
                names      ('__name__', '__module__', '__qualname__', 'int', 'float', '__init__', '__str__')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'Timestamp'
-               firstlineno 184
+               firstlineno 185
                lnotab 0x0a012008
             'Timestamp'
             'byteorder'
             'wf_datapoint_size'
             'wave_desc_size'
             'user_text_size'
             'reserved_desc_size'
@@ -1783,17 +1780,17 @@
                stacksize : 3
                flags     : 3
                code
                   0x97007c01a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000a001000000000000000000000000000000
                   00000000006402a6010000ab010000000000000000a00100000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-               320           0 RESUME                   0
+               321           0 RESUME                   0
                
-               322           2 LOAD_FAST                1 (data)
+               323           2 LOAD_FAST                1 (data)
                              4 LOAD_METHOD              0 (decode)
                             26 LOAD_CONST               1 ('utf-8')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 LOAD_METHOD              1 (strip)
                             64 LOAD_CONST               2 ('\x00')
                             66 PRECALL                  1
@@ -1808,15 +1805,15 @@
                   '\x00'
                names      ('decode', 'strip')
                varnames   ('self', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_to_string'
-               firstlineno 320
+               firstlineno 321
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 8
                flags     : 3
                code
@@ -1832,97 +1829,97 @@
                   0164066407850219000000000000000000a6010000ab0100000000000000
                   007d057c00a00300000000000000000000000000000000000000007c0164
                   076408850219000000000000000000a6010000ab0100000000000000007d
                   067c00a00300000000000000000000000000000000000000007c01640864
                   09850219000000000000000000a6010000ab0100000000000000007d077c
                   00a00400000000000000000000000000000000000000007c077c067c057c
                   047c037c02a6060000ab0600000000000000005300
-               324           0 RESUME                   0
+               325           0 RESUME                   0
                
-               326           2 LOAD_GLOBAL              1 (NULL + len)
+               327           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                1 (data)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (16)
                             32 COMPARE_OP               3 (!=)
                             38 POP_JUMP_FORWARD_IF_FALSE    15 (to 70)
                
-               327          40 LOAD_GLOBAL              3 (NULL + Exception)
+               328          40 LOAD_GLOBAL              3 (NULL + Exception)
                             52 LOAD_CONST               2 ('parsing error: timestamp must be 16 bytes long')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 RAISE_VARARGS            1
                
-               329     >>   70 LOAD_FAST                0 (self)
+               330     >>   70 LOAD_FAST                0 (self)
                             72 LOAD_METHOD              2 (_WaveformData__parse_to_float)
                             94 LOAD_FAST                1 (data)
                             96 LOAD_CONST               3 (0)
                             98 LOAD_CONST               4 (8)
                            100 BUILD_SLICE              2
                            102 BINARY_SUBSCR
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               2 (second)
                
-               330         128 LOAD_FAST                0 (self)
+               331         128 LOAD_FAST                0 (self)
                            130 LOAD_METHOD              3 (_WaveformData__parse_to_int)
                            152 LOAD_FAST                1 (data)
                            154 LOAD_CONST               4 (8)
                            156 LOAD_CONST               5 (9)
                            158 BUILD_SLICE              2
                            160 BINARY_SUBSCR
                            170 PRECALL                  1
                            174 CALL                     1
                            184 STORE_FAST               3 (minute)
                
-               331         186 LOAD_FAST                0 (self)
+               332         186 LOAD_FAST                0 (self)
                            188 LOAD_METHOD              3 (_WaveformData__parse_to_int)
                            210 LOAD_FAST                1 (data)
                            212 LOAD_CONST               5 (9)
                            214 LOAD_CONST               6 (10)
                            216 BUILD_SLICE              2
                            218 BINARY_SUBSCR
                            228 PRECALL                  1
                            232 CALL                     1
                            242 STORE_FAST               4 (hour)
                
-               332         244 LOAD_FAST                0 (self)
+               333         244 LOAD_FAST                0 (self)
                            246 LOAD_METHOD              3 (_WaveformData__parse_to_int)
                            268 LOAD_FAST                1 (data)
                            270 LOAD_CONST               6 (10)
                            272 LOAD_CONST               7 (11)
                            274 BUILD_SLICE              2
                            276 BINARY_SUBSCR
                            286 PRECALL                  1
                            290 CALL                     1
                            300 STORE_FAST               5 (day)
                
-               333         302 LOAD_FAST                0 (self)
+               334         302 LOAD_FAST                0 (self)
                            304 LOAD_METHOD              3 (_WaveformData__parse_to_int)
                            326 LOAD_FAST                1 (data)
                            328 LOAD_CONST               7 (11)
                            330 LOAD_CONST               8 (12)
                            332 BUILD_SLICE              2
                            334 BINARY_SUBSCR
                            344 PRECALL                  1
                            348 CALL                     1
                            358 STORE_FAST               6 (month)
                
-               334         360 LOAD_FAST                0 (self)
+               335         360 LOAD_FAST                0 (self)
                            362 LOAD_METHOD              3 (_WaveformData__parse_to_int)
                            384 LOAD_FAST                1 (data)
                            386 LOAD_CONST               8 (12)
                            388 LOAD_CONST               9 (14)
                            390 BUILD_SLICE              2
                            392 BINARY_SUBSCR
                            402 PRECALL                  1
                            406 CALL                     1
                            416 STORE_FAST               7 (year)
                
-               336         418 LOAD_FAST                0 (self)
+               337         418 LOAD_FAST                0 (self)
                            420 LOAD_METHOD              4 (Timestamp)
                            442 LOAD_FAST                7 (year)
                            444 LOAD_FAST                6 (month)
                            446 LOAD_FAST                5 (day)
                            448 LOAD_FAST                4 (hour)
                            450 LOAD_FAST                3 (minute)
                            452 LOAD_FAST                2 (second)
@@ -1942,15 +1939,15 @@
                   14
                names      ('len', 'Exception', '_WaveformData__parse_to_float', '_WaveformData__parse_to_int', 'Timestamp')
                varnames   ('self', 'data', 'second', 'minute', 'hour', 'day', 'month', 'year')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_timestamp'
-               firstlineno 324
+               firstlineno 325
                lnotab 0x020226011e023a013a013a013a013a013a02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -1968,25 +1965,25 @@
                   00720264036e0164049b00640a9d027c01a6020000ab0200000000000000
                   0064061900000000000000000053007401000000000000000000007c01a6
                   010000ab010000000000000000640b6b0200000000722b74030000000000
                   00000000006a0200000000000000007c006a03000000000000000064026b
                   0200000000720264036e0164049b00640c9d027c01a6020000ab02000000
                   000000000064061900000000000000000053007409000000000000000000
                   00640da6010000ab0100000000000000008201
-               338           0 RESUME                   0
+               339           0 RESUME                   0
                
-               340           2 LOAD_GLOBAL              1 (NULL + len)
+               341           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                1 (data)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (1)
                             32 COMPARE_OP               2 (==)
                             38 POP_JUMP_FORWARD_IF_FALSE    43 (to 126)
                
-               341          40 LOAD_GLOBAL              3 (NULL + struct)
+               342          40 LOAD_GLOBAL              3 (NULL + struct)
                             52 LOAD_ATTR                2 (unpack)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (byteorder)
                             74 LOAD_CONST               2 ('big')
                             76 COMPARE_OP               2 (==)
                             82 POP_JUMP_FORWARD_IF_FALSE     2 (to 88)
                             84 LOAD_CONST               3 ('>')
@@ -1998,23 +1995,23 @@
                             96 LOAD_FAST                1 (data)
                             98 PRECALL                  2
                            102 CALL                     2
                            112 LOAD_CONST               6 (0)
                            114 BINARY_SUBSCR
                            124 RETURN_VALUE
                
-               342     >>  126 LOAD_GLOBAL              1 (NULL + len)
+               343     >>  126 LOAD_GLOBAL              1 (NULL + len)
                            138 LOAD_FAST                1 (data)
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               7 (2)
                            156 COMPARE_OP               2 (==)
                            162 POP_JUMP_FORWARD_IF_FALSE    43 (to 250)
                
-               343         164 LOAD_GLOBAL              3 (NULL + struct)
+               344         164 LOAD_GLOBAL              3 (NULL + struct)
                            176 LOAD_ATTR                2 (unpack)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                3 (byteorder)
                            198 LOAD_CONST               2 ('big')
                            200 COMPARE_OP               2 (==)
                            206 POP_JUMP_FORWARD_IF_FALSE     2 (to 212)
                            208 LOAD_CONST               3 ('>')
@@ -2026,23 +2023,23 @@
                            220 LOAD_FAST                1 (data)
                            222 PRECALL                  2
                            226 CALL                     2
                            236 LOAD_CONST               6 (0)
                            238 BINARY_SUBSCR
                            248 RETURN_VALUE
                
-               344     >>  250 LOAD_GLOBAL              1 (NULL + len)
+               345     >>  250 LOAD_GLOBAL              1 (NULL + len)
                            262 LOAD_FAST                1 (data)
                            264 PRECALL                  1
                            268 CALL                     1
                            278 LOAD_CONST               9 (4)
                            280 COMPARE_OP               2 (==)
                            286 POP_JUMP_FORWARD_IF_FALSE    43 (to 374)
                
-               345         288 LOAD_GLOBAL              3 (NULL + struct)
+               346         288 LOAD_GLOBAL              3 (NULL + struct)
                            300 LOAD_ATTR                2 (unpack)
                            310 LOAD_FAST                0 (self)
                            312 LOAD_ATTR                3 (byteorder)
                            322 LOAD_CONST               2 ('big')
                            324 COMPARE_OP               2 (==)
                            330 POP_JUMP_FORWARD_IF_FALSE     2 (to 336)
                            332 LOAD_CONST               3 ('>')
@@ -2054,23 +2051,23 @@
                            344 LOAD_FAST                1 (data)
                            346 PRECALL                  2
                            350 CALL                     2
                            360 LOAD_CONST               6 (0)
                            362 BINARY_SUBSCR
                            372 RETURN_VALUE
                
-               346     >>  374 LOAD_GLOBAL              1 (NULL + len)
+               347     >>  374 LOAD_GLOBAL              1 (NULL + len)
                            386 LOAD_FAST                1 (data)
                            388 PRECALL                  1
                            392 CALL                     1
                            402 LOAD_CONST              11 (8)
                            404 COMPARE_OP               2 (==)
                            410 POP_JUMP_FORWARD_IF_FALSE    43 (to 498)
                
-               347         412 LOAD_GLOBAL              3 (NULL + struct)
+               348         412 LOAD_GLOBAL              3 (NULL + struct)
                            424 LOAD_ATTR                2 (unpack)
                            434 LOAD_FAST                0 (self)
                            436 LOAD_ATTR                3 (byteorder)
                            446 LOAD_CONST               2 ('big')
                            448 COMPARE_OP               2 (==)
                            454 POP_JUMP_FORWARD_IF_FALSE     2 (to 460)
                            456 LOAD_CONST               3 ('>')
@@ -2082,15 +2079,15 @@
                            468 LOAD_FAST                1 (data)
                            470 PRECALL                  2
                            474 CALL                     2
                            484 LOAD_CONST               6 (0)
                            486 BINARY_SUBSCR
                            496 RETURN_VALUE
                
-               349     >>  498 LOAD_GLOBAL              9 (NULL + Exception)
+               350     >>  498 LOAD_GLOBAL              9 (NULL + Exception)
                            510 LOAD_CONST              13 ('parsing error: data is not 8, 16 or 32 bits, cannot parse to int')
                            512 PRECALL                  1
                            516 CALL                     1
                            526 RAISE_VARARGS            1
                consts
                   'Parse a chunk of bytes into an integer.'
                   1
@@ -2108,15 +2105,15 @@
                   'parsing error: data is not 8, 16 or 32 bits, cannot parse to int'
                names      ('len', 'struct', 'unpack', 'byteorder', 'Exception', 'int', 'from_bytes')
                varnames   ('self', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_to_int'
-               firstlineno 338
+               firstlineno 339
                lnotab 0x020226015601260156012601560126015602
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -2126,25 +2123,25 @@
                   049b0064059d027c01a6020000ab02000000000000000064061900000000
                   000000000053007401000000000000000000007c01a6010000ab01000000
                   000000000064076b0200000000722b7403000000000000000000006a0200
                   000000000000007c006a03000000000000000064026b0200000000720264
                   036e0164049b0064089d027c01a6020000ab020000000000000000640619
                   00000000000000000053007409000000000000000000006409a6010000ab
                   0100000000000000008201
-               353           0 RESUME                   0
+               354           0 RESUME                   0
                
-               356           2 LOAD_GLOBAL              1 (NULL + len)
+               357           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                1 (data)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (4)
                             32 COMPARE_OP               2 (==)
                             38 POP_JUMP_FORWARD_IF_FALSE    43 (to 126)
                
-               358          40 LOAD_GLOBAL              3 (NULL + struct)
+               359          40 LOAD_GLOBAL              3 (NULL + struct)
                             52 LOAD_ATTR                2 (unpack)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (byteorder)
                             74 LOAD_CONST               2 ('big')
                             76 COMPARE_OP               2 (==)
                             82 POP_JUMP_FORWARD_IF_FALSE     2 (to 88)
                             84 LOAD_CONST               3 ('>')
@@ -2156,23 +2153,23 @@
                             96 LOAD_FAST                1 (data)
                             98 PRECALL                  2
                            102 CALL                     2
                            112 LOAD_CONST               6 (0)
                            114 BINARY_SUBSCR
                            124 RETURN_VALUE
                
-               359     >>  126 LOAD_GLOBAL              1 (NULL + len)
+               360     >>  126 LOAD_GLOBAL              1 (NULL + len)
                            138 LOAD_FAST                1 (data)
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               7 (8)
                            156 COMPARE_OP               2 (==)
                            162 POP_JUMP_FORWARD_IF_FALSE    43 (to 250)
                
-               361         164 LOAD_GLOBAL              3 (NULL + struct)
+               362         164 LOAD_GLOBAL              3 (NULL + struct)
                            176 LOAD_ATTR                2 (unpack)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                3 (byteorder)
                            198 LOAD_CONST               2 ('big')
                            200 COMPARE_OP               2 (==)
                            206 POP_JUMP_FORWARD_IF_FALSE     2 (to 212)
                            208 LOAD_CONST               3 ('>')
@@ -2184,15 +2181,15 @@
                            220 LOAD_FAST                1 (data)
                            222 PRECALL                  2
                            226 CALL                     2
                            236 LOAD_CONST               6 (0)
                            238 BINARY_SUBSCR
                            248 RETURN_VALUE
                
-               364     >>  250 LOAD_GLOBAL              9 (NULL + Exception)
+               365     >>  250 LOAD_GLOBAL              9 (NULL + Exception)
                            262 LOAD_CONST               9 ('parsing error: data is not 32 or 64 bits, cannot parse to float')
                            264 PRECALL                  1
                            268 CALL                     1
                            278 RAISE_VARARGS            1
                consts
                   'Parse a chunk of bytes into a float.'
                   4
@@ -2206,15 +2203,15 @@
                   'parsing error: data is not 32 or 64 bits, cannot parse to float'
                names      ('len', 'struct', 'unpack', 'byteorder', 'Exception')
                varnames   ('self', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_to_float'
-               firstlineno 353
+               firstlineno 354
                lnotab 0x02032602560126025603
             'desc_block'
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 7
                flags     : 3
@@ -2358,619 +2355,619 @@
                   0000007c005f4300000000000000007c00a0250000000000000000000000
                   0000000000000000007c0264416442850219000000000000000000a60100
                   00ab0100000000000000007c005f4400000000000000007c00a045000000
                   00000000000000000000000000000000007c00a009000000000000000000
                   00000000000000000000007c0264426443850219000000000000000000a6
                   010000ab010000000000000000a6010000ab0100000000000000007c005f
                   46000000000000000064015300
-               366           0 RESUME                   0
+               367           0 RESUME                   0
                
-               369           2 LOAD_FAST                1 (desc_block)
+               370           2 LOAD_FAST                1 (desc_block)
                              4 STORE_FAST               2 (desc)
                
-               371           6 LOAD_FAST                0 (self)
+               372           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (_WaveformData__parse_to_string)
                             30 LOAD_FAST                2 (desc)
                             32 LOAD_CONST               1 (None)
                             34 LOAD_CONST               2 (15)
                             36 BUILD_SLICE              2
                             38 BINARY_SUBSCR
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               1 (descriptor_name)
                
-               372          74 LOAD_FAST                0 (self)
+               373          74 LOAD_FAST                0 (self)
                             76 LOAD_METHOD              0 (_WaveformData__parse_to_string)
                             98 LOAD_FAST                2 (desc)
                            100 LOAD_CONST               3 (16)
                            102 LOAD_CONST               4 (31)
                            104 BUILD_SLICE              2
                            106 BINARY_SUBSCR
                            116 PRECALL                  1
                            120 CALL                     1
                            130 LOAD_FAST                0 (self)
                            132 STORE_ATTR               2 (template_name)
                
-               375         142 LOAD_FAST                0 (self)
+               376         142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (template_name)
                            154 LOAD_CONST               5 ('LECROY_2_3')
                            156 COMPARE_OP               3 (!=)
                            162 POP_JUMP_FORWARD_IF_FALSE    76 (to 316)
                
-               376         164 LOAD_GLOBAL              7 (NULL + print)
+               377         164 LOAD_GLOBAL              7 (NULL + print)
                            176 LOAD_GLOBAL              9 (NULL + len)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                2 (template_name)
                            200 PRECALL                  1
                            204 CALL                     1
                            214 PRECALL                  1
                            218 CALL                     1
                            228 POP_TOP
                
-               377         230 LOAD_GLOBAL              7 (NULL + print)
+               378         230 LOAD_GLOBAL              7 (NULL + print)
                            242 LOAD_GLOBAL              9 (NULL + len)
                            254 LOAD_CONST               5 ('LECROY_2_3')
                            256 PRECALL                  1
                            260 CALL                     1
                            270 PRECALL                  1
                            274 CALL                     1
                            284 POP_TOP
                
-               378         286 LOAD_GLOBAL             11 (NULL + Exception)
+               379         286 LOAD_GLOBAL             11 (NULL + Exception)
                            298 LOAD_CONST               6 ('Waveform data does not use Lecroy 2.3 template.')
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               381     >>  316 LOAD_GLOBAL             12 (int)
+               382     >>  316 LOAD_GLOBAL             12 (int)
                            328 LOAD_METHOD              7 (from_bytes)
                            350 LOAD_FAST                2 (desc)
                            352 LOAD_CONST               7 (34)
                            354 LOAD_CONST               8 (36)
                            356 BUILD_SLICE              2
                            358 BINARY_SUBSCR
                            368 LOAD_CONST               9 ('big')
                            370 PRECALL                  2
                            374 CALL                     2
                            384 STORE_FAST               3 (comm_order)
                
-               382         386 LOAD_FAST                3 (comm_order)
+               383         386 LOAD_FAST                3 (comm_order)
                            388 LOAD_CONST              10 (1)
                            390 COMPARE_OP               3 (!=)
                            396 POP_JUMP_FORWARD_IF_TRUE     6 (to 410)
                            398 LOAD_FAST                3 (comm_order)
                            400 LOAD_CONST              11 (0)
                            402 COMPARE_OP               3 (!=)
                            408 POP_JUMP_FORWARD_IF_FALSE    35 (to 480)
                
-               383     >>  410 LOAD_GLOBAL             12 (int)
+               384     >>  410 LOAD_GLOBAL             12 (int)
                            422 LOAD_METHOD              7 (from_bytes)
                            444 LOAD_FAST                2 (desc)
                            446 LOAD_CONST               7 (34)
                            448 LOAD_CONST               8 (36)
                            450 BUILD_SLICE              2
                            452 BINARY_SUBSCR
                            462 LOAD_CONST              12 ('little')
                            464 PRECALL                  2
                            468 CALL                     2
                            478 STORE_FAST               3 (comm_order)
                
-               384     >>  480 LOAD_FAST                3 (comm_order)
+               385     >>  480 LOAD_FAST                3 (comm_order)
                            482 LOAD_CONST              11 (0)
                            484 COMPARE_OP               2 (==)
                            490 POP_JUMP_FORWARD_IF_FALSE     8 (to 508)
                
-               385         492 LOAD_CONST               9 ('big')
+               386         492 LOAD_CONST               9 ('big')
                            494 LOAD_FAST                0 (self)
                            496 STORE_ATTR               8 (byteorder)
                            506 JUMP_FORWARD             7 (to 522)
                
-               387     >>  508 LOAD_CONST              12 ('little')
+               388     >>  508 LOAD_CONST              12 ('little')
                            510 LOAD_FAST                0 (self)
                            512 STORE_ATTR               8 (byteorder)
                
-               390     >>  522 LOAD_FAST                0 (self)
+               391     >>  522 LOAD_FAST                0 (self)
                            524 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            546 LOAD_FAST                2 (desc)
                            548 LOAD_CONST              13 (32)
                            550 LOAD_CONST               7 (34)
                            552 BUILD_SLICE              2
                            554 BINARY_SUBSCR
                            564 PRECALL                  1
                            568 CALL                     1
                            578 STORE_FAST               4 (comm_type)
                
-               391         580 LOAD_FAST                4 (comm_type)
+               392         580 LOAD_FAST                4 (comm_type)
                            582 LOAD_CONST              11 (0)
                            584 COMPARE_OP               2 (==)
                            590 POP_JUMP_FORWARD_IF_FALSE     8 (to 608)
                
-               392         592 LOAD_CONST              10 (1)
+               393         592 LOAD_CONST              10 (1)
                            594 LOAD_FAST                0 (self)
                            596 STORE_ATTR              10 (wf_datapoint_size)
                            606 JUMP_FORWARD             7 (to 622)
                
-               394     >>  608 LOAD_CONST              14 (2)
+               395     >>  608 LOAD_CONST              14 (2)
                            610 LOAD_FAST                0 (self)
                            612 STORE_ATTR              10 (wf_datapoint_size)
                
-               397     >>  622 LOAD_FAST                0 (self)
+               398     >>  622 LOAD_FAST                0 (self)
                            624 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            646 LOAD_FAST                2 (desc)
                            648 LOAD_CONST               8 (36)
                            650 LOAD_CONST              15 (40)
                            652 BUILD_SLICE              2
                            654 BINARY_SUBSCR
                            664 PRECALL                  1
                            668 CALL                     1
                            678 LOAD_FAST                0 (self)
                            680 STORE_ATTR              11 (wave_desc_size)
                
-               398         690 LOAD_FAST                0 (self)
+               399         690 LOAD_FAST                0 (self)
                            692 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            714 LOAD_FAST                2 (desc)
                            716 LOAD_CONST              15 (40)
                            718 LOAD_CONST              16 (44)
                            720 BUILD_SLICE              2
                            722 BINARY_SUBSCR
                            732 PRECALL                  1
                            736 CALL                     1
                            746 LOAD_FAST                0 (self)
                            748 STORE_ATTR              12 (user_text_size)
                
-               399         758 LOAD_FAST                0 (self)
+               400         758 LOAD_FAST                0 (self)
                            760 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            782 LOAD_FAST                2 (desc)
                            784 LOAD_CONST              16 (44)
                            786 LOAD_CONST              17 (48)
                            788 BUILD_SLICE              2
                            790 BINARY_SUBSCR
                            800 PRECALL                  1
                            804 CALL                     1
                            814 LOAD_FAST                0 (self)
                            816 STORE_ATTR              13 (reserved_desc_size)
                
-               400         826 LOAD_FAST                0 (self)
+               401         826 LOAD_FAST                0 (self)
                            828 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            850 LOAD_FAST                2 (desc)
                            852 LOAD_CONST              17 (48)
                            854 LOAD_CONST              18 (52)
                            856 BUILD_SLICE              2
                            858 BINARY_SUBSCR
                            868 PRECALL                  1
                            872 CALL                     1
                            882 LOAD_FAST                0 (self)
                            884 STORE_ATTR              14 (trigtime_array_size)
                
-               401         894 LOAD_FAST                0 (self)
+               402         894 LOAD_FAST                0 (self)
                            896 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            918 LOAD_FAST                2 (desc)
                            920 LOAD_CONST              18 (52)
                            922 LOAD_CONST              19 (56)
                            924 BUILD_SLICE              2
                            926 BINARY_SUBSCR
                            936 PRECALL                  1
                            940 CALL                     1
                            950 LOAD_FAST                0 (self)
                            952 STORE_ATTR              15 (ris_time_array_size)
                
-               402         962 LOAD_FAST                0 (self)
+               403         962 LOAD_FAST                0 (self)
                            964 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                            986 LOAD_FAST                2 (desc)
                            988 LOAD_CONST              19 (56)
                            990 LOAD_CONST              20 (60)
                            992 BUILD_SLICE              2
                            994 BINARY_SUBSCR
                           1004 PRECALL                  1
                           1008 CALL                     1
                           1018 LOAD_FAST                0 (self)
                           1020 STORE_ATTR              16 (res1_array_size)
                
-               403        1030 LOAD_FAST                0 (self)
+               404        1030 LOAD_FAST                0 (self)
                           1032 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1054 LOAD_FAST                2 (desc)
                           1056 LOAD_CONST              20 (60)
                           1058 LOAD_CONST              21 (64)
                           1060 BUILD_SLICE              2
                           1062 BINARY_SUBSCR
                           1072 PRECALL                  1
                           1076 CALL                     1
                           1086 LOAD_FAST                0 (self)
                           1088 STORE_ATTR              17 (dat1_array_size)
                
-               404        1098 LOAD_FAST                0 (self)
+               405        1098 LOAD_FAST                0 (self)
                           1100 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1122 LOAD_FAST                2 (desc)
                           1124 LOAD_CONST              21 (64)
                           1126 LOAD_CONST              22 (68)
                           1128 BUILD_SLICE              2
                           1130 BINARY_SUBSCR
                           1140 PRECALL                  1
                           1144 CALL                     1
                           1154 LOAD_FAST                0 (self)
                           1156 STORE_ATTR              18 (dat2_array_size)
                
-               405        1166 LOAD_FAST                0 (self)
+               406        1166 LOAD_FAST                0 (self)
                           1168 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1190 LOAD_FAST                2 (desc)
                           1192 LOAD_CONST              22 (68)
                           1194 LOAD_CONST              23 (72)
                           1196 BUILD_SLICE              2
                           1198 BINARY_SUBSCR
                           1208 PRECALL                  1
                           1212 CALL                     1
                           1222 LOAD_FAST                0 (self)
                           1224 STORE_ATTR              19 (res2_array_size)
                
-               406        1234 LOAD_FAST                0 (self)
+               407        1234 LOAD_FAST                0 (self)
                           1236 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1258 LOAD_FAST                2 (desc)
                           1260 LOAD_CONST              24 (74)
                           1262 LOAD_CONST              25 (76)
                           1264 BUILD_SLICE              2
                           1266 BINARY_SUBSCR
                           1276 PRECALL                  1
                           1280 CALL                     1
                           1290 LOAD_FAST                0 (self)
                           1292 STORE_ATTR              20 (res3_array_size)
                
-               409        1302 LOAD_FAST                0 (self)
+               410        1302 LOAD_FAST                0 (self)
                           1304 LOAD_METHOD              0 (_WaveformData__parse_to_string)
                           1326 LOAD_FAST                2 (desc)
                           1328 LOAD_CONST              25 (76)
                           1330 LOAD_CONST              26 (92)
                           1332 BUILD_SLICE              2
                           1334 BINARY_SUBSCR
                           1344 PRECALL                  1
                           1348 CALL                     1
                           1358 LOAD_FAST                0 (self)
                           1360 STORE_ATTR              21 (instrument_name)
                
-               410        1370 LOAD_FAST                0 (self)
+               411        1370 LOAD_FAST                0 (self)
                           1372 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1394 LOAD_FAST                2 (desc)
                           1396 LOAD_CONST              26 (92)
                           1398 LOAD_CONST              27 (96)
                           1400 BUILD_SLICE              2
                           1402 BINARY_SUBSCR
                           1412 PRECALL                  1
                           1416 CALL                     1
                           1426 LOAD_FAST                0 (self)
                           1428 STORE_ATTR              22 (instrument_number)
                
-               411        1438 LOAD_FAST                0 (self)
+               412        1438 LOAD_FAST                0 (self)
                           1440 LOAD_METHOD              0 (_WaveformData__parse_to_string)
                           1462 LOAD_FAST                2 (desc)
                           1464 LOAD_CONST              27 (96)
                           1466 LOAD_CONST              28 (112)
                           1468 BUILD_SLICE              2
                           1470 BINARY_SUBSCR
                           1480 PRECALL                  1
                           1484 CALL                     1
                           1494 LOAD_FAST                0 (self)
                           1496 STORE_ATTR              23 (trace_label)
                
-               412        1506 LOAD_FAST                0 (self)
+               413        1506 LOAD_FAST                0 (self)
                           1508 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1530 LOAD_FAST                2 (desc)
                           1532 LOAD_CONST              28 (112)
                           1534 LOAD_CONST              29 (114)
                           1536 BUILD_SLICE              2
                           1538 BINARY_SUBSCR
                           1548 PRECALL                  1
                           1552 CALL                     1
                           1562 LOAD_FAST                0 (self)
                           1564 STORE_ATTR              24 (reserved_1)
                
-               413        1574 LOAD_FAST                0 (self)
+               414        1574 LOAD_FAST                0 (self)
                           1576 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1598 LOAD_FAST                2 (desc)
                           1600 LOAD_CONST              29 (114)
                           1602 LOAD_CONST              30 (116)
                           1604 BUILD_SLICE              2
                           1606 BINARY_SUBSCR
                           1616 PRECALL                  1
                           1620 CALL                     1
                           1630 LOAD_FAST                0 (self)
                           1632 STORE_ATTR              25 (reserved_2)
                
-               416        1642 LOAD_FAST                0 (self)
+               417        1642 LOAD_FAST                0 (self)
                           1644 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1666 LOAD_FAST                2 (desc)
                           1668 LOAD_CONST              30 (116)
                           1670 LOAD_CONST              31 (120)
                           1672 BUILD_SLICE              2
                           1674 BINARY_SUBSCR
                           1684 PRECALL                  1
                           1688 CALL                     1
                           1698 LOAD_FAST                0 (self)
                           1700 STORE_ATTR              26 (wave_array_count)
                
-               417        1710 LOAD_FAST                0 (self)
+               418        1710 LOAD_FAST                0 (self)
                           1712 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1734 LOAD_FAST                2 (desc)
                           1736 LOAD_CONST              31 (120)
                           1738 LOAD_CONST              32 (124)
                           1740 BUILD_SLICE              2
                           1742 BINARY_SUBSCR
                           1752 PRECALL                  1
                           1756 CALL                     1
                           1766 LOAD_FAST                0 (self)
                           1768 STORE_ATTR              27 (points_per_screen)
                
-               418        1778 LOAD_FAST                0 (self)
+               419        1778 LOAD_FAST                0 (self)
                           1780 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1802 LOAD_FAST                2 (desc)
                           1804 LOAD_CONST              32 (124)
                           1806 LOAD_CONST              33 (128)
                           1808 BUILD_SLICE              2
                           1810 BINARY_SUBSCR
                           1820 PRECALL                  1
                           1824 CALL                     1
                           1834 LOAD_FAST                0 (self)
                           1836 STORE_ATTR              28 (first_valid_point)
                
-               419        1846 LOAD_FAST                0 (self)
+               420        1846 LOAD_FAST                0 (self)
                           1848 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1870 LOAD_FAST                2 (desc)
                           1872 LOAD_CONST              33 (128)
                           1874 LOAD_CONST              34 (132)
                           1876 BUILD_SLICE              2
                           1878 BINARY_SUBSCR
                           1888 PRECALL                  1
                           1892 CALL                     1
                           1902 LOAD_FAST                0 (self)
                           1904 STORE_ATTR              29 (last_valid_point)
                
-               420        1914 LOAD_FAST                0 (self)
+               421        1914 LOAD_FAST                0 (self)
                           1916 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           1938 LOAD_FAST                2 (desc)
                           1940 LOAD_CONST              34 (132)
                           1942 LOAD_CONST              35 (136)
                           1944 BUILD_SLICE              2
                           1946 BINARY_SUBSCR
                           1956 PRECALL                  1
                           1960 CALL                     1
                           1970 LOAD_FAST                0 (self)
                           1972 STORE_ATTR              30 (first_point)
                
-               421        1982 LOAD_FAST                0 (self)
+               422        1982 LOAD_FAST                0 (self)
                           1984 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2006 LOAD_FAST                2 (desc)
                           2008 LOAD_CONST              35 (136)
                           2010 LOAD_CONST              36 (140)
                           2012 BUILD_SLICE              2
                           2014 BINARY_SUBSCR
                           2024 PRECALL                  1
                           2028 CALL                     1
                           2038 LOAD_FAST                0 (self)
                           2040 STORE_ATTR              31 (sparsing_factor)
                
-               422        2050 LOAD_FAST                0 (self)
+               423        2050 LOAD_FAST                0 (self)
                           2052 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2074 LOAD_FAST                2 (desc)
                           2076 LOAD_CONST              36 (140)
                           2078 LOAD_CONST              37 (144)
                           2080 BUILD_SLICE              2
                           2082 BINARY_SUBSCR
                           2092 PRECALL                  1
                           2096 CALL                     1
                           2106 LOAD_FAST                0 (self)
                           2108 STORE_ATTR              32 (segment_index)
                
-               423        2118 LOAD_FAST                0 (self)
+               424        2118 LOAD_FAST                0 (self)
                           2120 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2142 LOAD_FAST                2 (desc)
                           2144 LOAD_CONST              37 (144)
                           2146 LOAD_CONST              38 (148)
                           2148 BUILD_SLICE              2
                           2150 BINARY_SUBSCR
                           2160 PRECALL                  1
                           2164 CALL                     1
                           2174 LOAD_FAST                0 (self)
                           2176 STORE_ATTR              33 (subarray_count)
                
-               424        2186 LOAD_FAST                0 (self)
+               425        2186 LOAD_FAST                0 (self)
                           2188 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2210 LOAD_FAST                2 (desc)
                           2212 LOAD_CONST              38 (148)
                           2214 LOAD_CONST              39 (152)
                           2216 BUILD_SLICE              2
                           2218 BINARY_SUBSCR
                           2228 PRECALL                  1
                           2232 CALL                     1
                           2242 LOAD_FAST                0 (self)
                           2244 STORE_ATTR              34 (sweeps_per_acquisition)
                
-               425        2254 LOAD_FAST                0 (self)
+               426        2254 LOAD_FAST                0 (self)
                           2256 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2278 LOAD_FAST                2 (desc)
                           2280 LOAD_CONST              39 (152)
                           2282 LOAD_CONST              40 (154)
                           2284 BUILD_SLICE              2
                           2286 BINARY_SUBSCR
                           2296 PRECALL                  1
                           2300 CALL                     1
                           2310 LOAD_FAST                0 (self)
                           2312 STORE_ATTR              35 (points_per_pair)
                
-               426        2322 LOAD_FAST                0 (self)
+               427        2322 LOAD_FAST                0 (self)
                           2324 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2346 LOAD_FAST                2 (desc)
                           2348 LOAD_CONST              40 (154)
                           2350 LOAD_CONST              41 (156)
                           2352 BUILD_SLICE              2
                           2354 BINARY_SUBSCR
                           2364 PRECALL                  1
                           2368 CALL                     1
                           2378 LOAD_FAST                0 (self)
                           2380 STORE_ATTR              36 (pair_offset)
                
-               428        2390 LOAD_FAST                0 (self)
+               429        2390 LOAD_FAST                0 (self)
                           2392 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2414 LOAD_FAST                2 (desc)
                           2416 LOAD_CONST              41 (156)
                           2418 LOAD_CONST              42 (160)
                           2420 BUILD_SLICE              2
                           2422 BINARY_SUBSCR
                           2432 PRECALL                  1
                           2436 CALL                     1
                           2446 LOAD_FAST                0 (self)
                           2448 STORE_ATTR              38 (vertical_gain)
                
-               429        2458 LOAD_FAST                0 (self)
+               430        2458 LOAD_FAST                0 (self)
                           2460 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2482 LOAD_FAST                2 (desc)
                           2484 LOAD_CONST              42 (160)
                           2486 LOAD_CONST              43 (164)
                           2488 BUILD_SLICE              2
                           2490 BINARY_SUBSCR
                           2500 PRECALL                  1
                           2504 CALL                     1
                           2514 LOAD_FAST                0 (self)
                           2516 STORE_ATTR              39 (vertical_offset)
                
-               430        2526 LOAD_FAST                0 (self)
+               431        2526 LOAD_FAST                0 (self)
                           2528 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2550 LOAD_FAST                2 (desc)
                           2552 LOAD_CONST              43 (164)
                           2554 LOAD_CONST              44 (168)
                           2556 BUILD_SLICE              2
                           2558 BINARY_SUBSCR
                           2568 PRECALL                  1
                           2572 CALL                     1
                           2582 LOAD_FAST                0 (self)
                           2584 STORE_ATTR              40 (max_value)
                
-               431        2594 LOAD_FAST                0 (self)
+               432        2594 LOAD_FAST                0 (self)
                           2596 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2618 LOAD_FAST                2 (desc)
                           2620 LOAD_CONST              44 (168)
                           2622 LOAD_CONST              45 (172)
                           2624 BUILD_SLICE              2
                           2626 BINARY_SUBSCR
                           2636 PRECALL                  1
                           2640 CALL                     1
                           2650 LOAD_FAST                0 (self)
                           2652 STORE_ATTR              41 (min_value)
                
-               432        2662 LOAD_FAST                0 (self)
+               433        2662 LOAD_FAST                0 (self)
                           2664 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2686 LOAD_FAST                2 (desc)
                           2688 LOAD_CONST              45 (172)
                           2690 LOAD_CONST              46 (174)
                           2692 BUILD_SLICE              2
                           2694 BINARY_SUBSCR
                           2704 PRECALL                  1
                           2708 CALL                     1
                           2718 LOAD_FAST                0 (self)
                           2720 STORE_ATTR              42 (nomimal_bits)
                
-               433        2730 LOAD_FAST                0 (self)
+               434        2730 LOAD_FAST                0 (self)
                           2732 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           2754 LOAD_FAST                2 (desc)
                           2756 LOAD_CONST              46 (174)
                           2758 LOAD_CONST              47 (176)
                           2760 BUILD_SLICE              2
                           2762 BINARY_SUBSCR
                           2772 PRECALL                  1
                           2776 CALL                     1
                           2786 LOAD_FAST                0 (self)
                           2788 STORE_ATTR              43 (nominal_subarray_count)
                
-               434        2798 LOAD_FAST                0 (self)
+               435        2798 LOAD_FAST                0 (self)
                           2800 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2822 LOAD_FAST                2 (desc)
                           2824 LOAD_CONST              47 (176)
                           2826 LOAD_CONST              48 (180)
                           2828 BUILD_SLICE              2
                           2830 BINARY_SUBSCR
                           2840 PRECALL                  1
                           2844 CALL                     1
                           2854 LOAD_FAST                0 (self)
                           2856 STORE_ATTR              44 (horizontal_interval)
                
-               435        2866 LOAD_FAST                0 (self)
+               436        2866 LOAD_FAST                0 (self)
                           2868 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2890 LOAD_FAST                2 (desc)
                           2892 LOAD_CONST              48 (180)
                           2894 LOAD_CONST              49 (188)
                           2896 BUILD_SLICE              2
                           2898 BINARY_SUBSCR
                           2908 PRECALL                  1
                           2912 CALL                     1
                           2922 LOAD_FAST                0 (self)
                           2924 STORE_ATTR              45 (horizontal_offset)
                
-               436        2934 LOAD_FAST                0 (self)
+               437        2934 LOAD_FAST                0 (self)
                           2936 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           2958 LOAD_FAST                2 (desc)
                           2960 LOAD_CONST              49 (188)
                           2962 LOAD_CONST              50 (196)
                           2964 BUILD_SLICE              2
                           2966 BINARY_SUBSCR
                           2976 PRECALL                  1
                           2980 CALL                     1
                           2990 LOAD_FAST                0 (self)
                           2992 STORE_ATTR              46 (pixel_offset)
                
-               437        3002 LOAD_FAST                2 (desc)
+               438        3002 LOAD_FAST                2 (desc)
                           3004 LOAD_CONST              50 (196)
                           3006 LOAD_CONST              51 (244)
                           3008 BUILD_SLICE              2
                           3010 BINARY_SUBSCR
                           3020 LOAD_FAST                0 (self)
                           3022 STORE_ATTR              47 (vertical_unit)
                
-               438        3032 LOAD_FAST                2 (desc)
+               439        3032 LOAD_FAST                2 (desc)
                           3034 LOAD_CONST              51 (244)
                           3036 LOAD_CONST              52 (292)
                           3038 BUILD_SLICE              2
                           3040 BINARY_SUBSCR
                           3050 LOAD_FAST                0 (self)
                           3052 STORE_ATTR              48 (horizontal_unit)
                
-               439        3062 LOAD_FAST                0 (self)
+               440        3062 LOAD_FAST                0 (self)
                           3064 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           3086 LOAD_FAST                2 (desc)
                           3088 LOAD_CONST              52 (292)
                           3090 LOAD_CONST              53 (296)
                           3092 BUILD_SLICE              2
                           3094 BINARY_SUBSCR
                           3104 PRECALL                  1
                           3108 CALL                     1
                           3118 LOAD_FAST                0 (self)
                           3120 STORE_ATTR              49 (horizontal_uncertainty)
                
-               440        3130 LOAD_FAST                0 (self)
+               441        3130 LOAD_FAST                0 (self)
                           3132 LOAD_METHOD             50 (_WaveformData__parse_timestamp)
                           3154 LOAD_FAST                2 (desc)
                           3156 LOAD_CONST              53 (296)
                           3158 LOAD_CONST              54 (312)
                           3160 BUILD_SLICE              2
                           3162 BINARY_SUBSCR
                           3172 PRECALL                  1
                           3176 CALL                     1
                           3186 LOAD_FAST                0 (self)
                           3188 STORE_ATTR              51 (trigger_time)
                
-               441        3198 LOAD_FAST                0 (self)
+               442        3198 LOAD_FAST                0 (self)
                           3200 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           3222 LOAD_FAST                2 (desc)
                           3224 LOAD_CONST              54 (312)
                           3226 LOAD_CONST              55 (316)
                           3228 BUILD_SLICE              2
                           3230 BINARY_SUBSCR
                           3240 PRECALL                  1
                           3244 CALL                     1
                           3254 LOAD_FAST                0 (self)
                           3256 STORE_ATTR              52 (acquisition_duration)
                
-               442        3266 LOAD_FAST                0 (self)
+               443        3266 LOAD_FAST                0 (self)
                           3268 LOAD_METHOD             53 (RecordType)
                           3290 LOAD_FAST                0 (self)
                           3292 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3314 LOAD_FAST                2 (desc)
                           3316 LOAD_CONST              55 (316)
                           3318 LOAD_CONST              56 (318)
                           3320 BUILD_SLICE              2
@@ -2978,15 +2975,15 @@
                           3332 PRECALL                  1
                           3336 CALL                     1
                           3346 PRECALL                  1
                           3350 CALL                     1
                           3360 LOAD_FAST                0 (self)
                           3362 STORE_ATTR              54 (record_type)
                
-               443        3372 LOAD_FAST                0 (self)
+               444        3372 LOAD_FAST                0 (self)
                           3374 LOAD_METHOD             55 (ProcessingDone)
                           3396 LOAD_FAST                0 (self)
                           3398 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3420 LOAD_FAST                2 (desc)
                           3422 LOAD_CONST              56 (318)
                           3424 LOAD_CONST              57 (320)
                           3426 BUILD_SLICE              2
@@ -2994,27 +2991,27 @@
                           3438 PRECALL                  1
                           3442 CALL                     1
                           3452 PRECALL                  1
                           3456 CALL                     1
                           3466 LOAD_FAST                0 (self)
                           3468 STORE_ATTR              56 (processing_done)
                
-               444        3478 LOAD_FAST                0 (self)
+               445        3478 LOAD_FAST                0 (self)
                           3480 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3502 LOAD_FAST                2 (desc)
                           3504 LOAD_CONST              58 (322)
                           3506 LOAD_CONST              59 (324)
                           3508 BUILD_SLICE              2
                           3510 BINARY_SUBSCR
                           3520 PRECALL                  1
                           3524 CALL                     1
                           3534 LOAD_FAST                0 (self)
                           3536 STORE_ATTR              57 (ris_sweeps)
                
-               445        3546 LOAD_FAST                0 (self)
+               446        3546 LOAD_FAST                0 (self)
                           3548 LOAD_METHOD             58 (TimeBase)
                           3570 LOAD_FAST                0 (self)
                           3572 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3594 LOAD_FAST                2 (desc)
                           3596 LOAD_CONST              59 (324)
                           3598 LOAD_CONST              60 (326)
                           3600 BUILD_SLICE              2
@@ -3022,15 +3019,15 @@
                           3612 PRECALL                  1
                           3616 CALL                     1
                           3626 PRECALL                  1
                           3630 CALL                     1
                           3640 LOAD_FAST                0 (self)
                           3642 STORE_ATTR              59 (timebase)
                
-               446        3652 LOAD_FAST                0 (self)
+               447        3652 LOAD_FAST                0 (self)
                           3654 LOAD_METHOD             60 (Coupling)
                           3676 LOAD_FAST                0 (self)
                           3678 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3700 LOAD_FAST                2 (desc)
                           3702 LOAD_CONST              60 (326)
                           3704 LOAD_CONST              61 (328)
                           3706 BUILD_SLICE              2
@@ -3038,27 +3035,27 @@
                           3718 PRECALL                  1
                           3722 CALL                     1
                           3732 PRECALL                  1
                           3736 CALL                     1
                           3746 LOAD_FAST                0 (self)
                           3748 STORE_ATTR              61 (vertical_coupling)
                
-               447        3758 LOAD_FAST                0 (self)
+               448        3758 LOAD_FAST                0 (self)
                           3760 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           3782 LOAD_FAST                2 (desc)
                           3784 LOAD_CONST              61 (328)
                           3786 LOAD_CONST              62 (332)
                           3788 BUILD_SLICE              2
                           3790 BINARY_SUBSCR
                           3800 PRECALL                  1
                           3804 CALL                     1
                           3814 LOAD_FAST                0 (self)
                           3816 STORE_ATTR              62 (probe_attenuation)
                
-               448        3826 LOAD_FAST                0 (self)
+               449        3826 LOAD_FAST                0 (self)
                           3828 LOAD_METHOD             63 (VertGain)
                           3850 LOAD_FAST                0 (self)
                           3852 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3874 LOAD_FAST                2 (desc)
                           3876 LOAD_CONST              62 (332)
                           3878 LOAD_CONST              63 (334)
                           3880 BUILD_SLICE              2
@@ -3066,54 +3063,54 @@
                           3892 PRECALL                  1
                           3896 CALL                     1
                           3906 PRECALL                  1
                           3910 CALL                     1
                           3920 LOAD_FAST                0 (self)
                           3922 STORE_ATTR              64 (fixed_vertical_gain)
                
-               449        3932 LOAD_GLOBAL            131 (NULL + bool)
+               450        3932 LOAD_GLOBAL            131 (NULL + bool)
                           3944 LOAD_FAST                0 (self)
                           3946 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           3968 LOAD_FAST                2 (desc)
                           3970 LOAD_CONST              63 (334)
                           3972 LOAD_CONST              64 (336)
                           3974 BUILD_SLICE              2
                           3976 BINARY_SUBSCR
                           3986 PRECALL                  1
                           3990 CALL                     1
                           4000 PRECALL                  1
                           4004 CALL                     1
                           4014 LOAD_FAST                0 (self)
                           4016 STORE_ATTR              66 (bandwidth_limit)
                
-               450        4026 LOAD_FAST                0 (self)
+               451        4026 LOAD_FAST                0 (self)
                           4028 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           4050 LOAD_FAST                2 (desc)
                           4052 LOAD_CONST              64 (336)
                           4054 LOAD_CONST              65 (340)
                           4056 BUILD_SLICE              2
                           4058 BINARY_SUBSCR
                           4068 PRECALL                  1
                           4072 CALL                     1
                           4082 LOAD_FAST                0 (self)
                           4084 STORE_ATTR              67 (vertical_vernier)
                
-               451        4094 LOAD_FAST                0 (self)
+               452        4094 LOAD_FAST                0 (self)
                           4096 LOAD_METHOD             37 (_WaveformData__parse_to_float)
                           4118 LOAD_FAST                2 (desc)
                           4120 LOAD_CONST              65 (340)
                           4122 LOAD_CONST              66 (344)
                           4124 BUILD_SLICE              2
                           4126 BINARY_SUBSCR
                           4136 PRECALL                  1
                           4140 CALL                     1
                           4150 LOAD_FAST                0 (self)
                           4152 STORE_ATTR              68 (acquisition_vertical_offset)
                
-               452        4162 LOAD_FAST                0 (self)
+               453        4162 LOAD_FAST                0 (self)
                           4164 LOAD_METHOD             69 (Source)
                           4186 LOAD_FAST                0 (self)
                           4188 LOAD_METHOD              9 (_WaveformData__parse_to_int)
                           4210 LOAD_FAST                2 (desc)
                           4212 LOAD_CONST              66 (344)
                           4214 LOAD_CONST              67 (346)
                           4216 BUILD_SLICE              2
@@ -3197,15 +3194,15 @@
                   346
                names      ('_WaveformData__parse_to_string', 'descriptor_name', 'template_name', 'print', 'len', 'Exception', 'int', 'from_bytes', 'byteorder', '_WaveformData__parse_to_int', 'wf_datapoint_size', 'wave_desc_size', 'user_text_size', 'reserved_desc_size', 'trigtime_array_size', 'ris_time_array_size', 'res1_array_size', 'dat1_array_size', 'dat2_array_size', 'res2_array_size', 'res3_array_size', 'instrument_name', 'instrument_number', 'trace_label', 'reserved_1', 'reserved_2', 'wave_array_count', 'points_per_screen', 'first_valid_point', 'last_valid_point', 'first_point', 'sparsing_factor', 'segment_index', 'subarray_count', 'sweeps_per_acquisition', 'points_per_pair', 'pair_offset', '_WaveformData__parse_to_float', 'vertical_gain', 'vertical_offset', 'max_value', 'min_value', 'nomimal_bits', 'nominal_subarray_count', 'horizontal_interval', 'horizontal_offset', 'pixel_offset', 'vertical_unit', 'horizontal_unit', 'horizontal_uncertainty', '_WaveformData__parse_timestamp', 'trigger_time', 'acquisition_duration', 'RecordType', 'record_type', 'ProcessingDone', 'processing_done', 'ris_sweeps', 'TimeBase', 'timebase', 'Coupling', 'vertical_coupling', 'probe_attenuation', 'VertGain', 'fixed_vertical_gain', 'bool', 'bandwidth_limit', 'vertical_vernier', 'acquisition_vertical_offset', 'Source', 'wave_source')
                varnames   ('self', 'desc_block', 'desc', 'comm_order', 'comm_type')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_wavedesc'
-               firstlineno 366
+               firstlineno 367
                lnotab
                   0x02030402440144031601420138011e034601180146010c0110020e033a
                   010c0110020e034401440144014401440144014401440144014403440144
                   014401440144034401440144014401440144014401440144014401440244
                   01440144014401440144014401440144011e011e014401440144016a016a
                   0144016a016a0144016a015e0144014401
             'text_block'
@@ -3213,17 +3210,17 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007c005f01000000000000000064005300
-               454           0 RESUME                   0
+               455           0 RESUME                   0
                
-               455           2 LOAD_FAST                0 (self)
+               456           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_WaveformData__parse_to_string)
                             26 LOAD_FAST                1 (text_block)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 LOAD_FAST                0 (self)
                             44 STORE_ATTR               1 (usertext)
                             54 LOAD_CONST               0 (None)
@@ -3232,15 +3229,15 @@
                   None
                names      ('_WaveformData__parse_to_string', 'usertext')
                varnames   ('self', 'text_block')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_usertext'
-               firstlineno 454
+               firstlineno 455
                lnotab 0x0201
             'time_block'
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 9
                flags     : 3
@@ -3283,97 +3280,97 @@
                   006a0300000000000000007c006a040000000000000000a6020000ab0200
                   0000000000000044005d377d037c037c006a0f00000000000000007a0600
                   007d087c037c087a0a00007d0b7c02a00500000000000000000000000000
                   000000000000007c006a0600000000000000007c0b7a0500007c0a7c0819
                   0000000000000000007a000000a6010000ab01000000000000000001008c
                   387411000000000000000000006a0900000000000000007c02a6010000ab
                   0100000000000000007c005f0a00000000000000006405530064055300
-               457           0 RESUME                   0
+               458           0 RESUME                   0
                
-               461           2 LOAD_GLOBAL              1 (NULL + len)
+               462           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                1 (time_block)
                             16 LOAD_METHOD              1 (strip)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 LOAD_CONST               1 (0)
                             68 COMPARE_OP               2 (==)
                             74 POP_JUMP_FORWARD_IF_FALSE    95 (to 266)
                
-               464          76 BUILD_LIST               0
+               465          76 BUILD_LIST               0
                             78 STORE_FAST               2 (data)
                
-               465          80 LOAD_GLOBAL              5 (NULL + range)
+               466          80 LOAD_GLOBAL              5 (NULL + range)
                             92 LOAD_FAST                0 (self)
                             94 LOAD_ATTR                3 (first_valid_point)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                4 (last_valid_point)
                            116 PRECALL                  2
                            120 CALL                     2
                            130 GET_ITER
                        >>  132 FOR_ITER                39 (to 212)
                            134 STORE_FAST               3 (i)
                
-               466         136 LOAD_FAST                2 (data)
+               467         136 LOAD_FAST                2 (data)
                            138 LOAD_METHOD              5 (append)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                6 (horizontal_interval)
                            172 LOAD_FAST                3 (i)
                            174 BINARY_OP                5 (*)
                            178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                7 (horizontal_offset)
                            190 BINARY_OP                0 (+)
                            194 PRECALL                  1
                            198 CALL                     1
                            208 POP_TOP
                            210 JUMP_BACKWARD           40 (to 132)
                
-               467     >>  212 LOAD_GLOBAL             17 (NULL + np)
+               468     >>  212 LOAD_GLOBAL             17 (NULL + np)
                            224 LOAD_ATTR                9 (array)
                            234 LOAD_FAST                2 (data)
                            236 PRECALL                  1
                            240 CALL                     1
                            250 LOAD_FAST                0 (self)
                            252 STORE_ATTR              10 (data_x)
                            262 LOAD_CONST               5 (None)
                            264 RETURN_VALUE
                
-               468     >>  266 LOAD_FAST                0 (self)
+               469     >>  266 LOAD_FAST                0 (self)
                            268 LOAD_ATTR               11 (nominal_subarray_count)
                            278 LOAD_CONST               2 (1)
                            280 COMPARE_OP               3 (!=)
                            286 EXTENDED_ARG             1
                            288 POP_JUMP_FORWARD_IF_FALSE   276 (to 842)
                
-               471         290 BUILD_LIST               0
+               472         290 BUILD_LIST               0
                            292 STORE_FAST               2 (data)
                
-               473         294 BUILD_LIST               0
+               474         294 BUILD_LIST               0
                            296 STORE_FAST               4 (first_trig_times)
                
-               474         298 BUILD_LIST               0
+               475         298 BUILD_LIST               0
                            300 STORE_FAST               5 (trigger_offsets)
                
-               475         302 LOAD_GLOBAL              5 (NULL + range)
+               476         302 LOAD_GLOBAL              5 (NULL + range)
                            314 LOAD_CONST               1 (0)
                            316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR               11 (nominal_subarray_count)
                            328 PRECALL                  2
                            332 CALL                     2
                            342 GET_ITER
                        >>  344 FOR_ITER               112 (to 570)
                            346 STORE_FAST               3 (i)
                
-               476         348 LOAD_FAST                3 (i)
+               477         348 LOAD_FAST                3 (i)
                            350 LOAD_CONST               3 (16)
                            352 BINARY_OP                5 (*)
                            356 STORE_FAST               6 (start_pos)
                
-               477         358 LOAD_FAST                4 (first_trig_times)
+               478         358 LOAD_FAST                4 (first_trig_times)
                            360 LOAD_METHOD              5 (append)
                            382 LOAD_FAST                0 (self)
                            384 LOAD_METHOD             12 (_WaveformData__parse_to_float)
                            406 LOAD_FAST                1 (time_block)
                            408 LOAD_FAST                6 (start_pos)
                            410 LOAD_FAST                6 (start_pos)
                            412 LOAD_CONST               4 (8)
@@ -3382,15 +3379,15 @@
                            420 BINARY_SUBSCR
                            430 PRECALL                  1
                            434 CALL                     1
                            444 PRECALL                  1
                            448 CALL                     1
                            458 POP_TOP
                
-               478         460 LOAD_FAST                5 (trigger_offsets)
+               479         460 LOAD_FAST                5 (trigger_offsets)
                            462 LOAD_METHOD              5 (append)
                            484 LOAD_FAST                0 (self)
                            486 LOAD_METHOD             12 (_WaveformData__parse_to_float)
                            508 LOAD_FAST                1 (time_block)
                            510 LOAD_FAST                6 (start_pos)
                            512 LOAD_CONST               4 (8)
                            514 BINARY_OP                0 (+)
@@ -3402,41 +3399,41 @@
                            538 PRECALL                  1
                            542 CALL                     1
                            552 PRECALL                  1
                            556 CALL                     1
                            566 POP_TOP
                            568 JUMP_BACKWARD          113 (to 344)
                
-               480     >>  570 LOAD_GLOBAL             27 (NULL + int)
+               481     >>  570 LOAD_GLOBAL             27 (NULL + int)
                            582 LOAD_FAST                0 (self)
                            584 LOAD_ATTR               14 (wave_array_count)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR               11 (nominal_subarray_count)
                            606 BINARY_OP               11 (/)
                            610 PRECALL                  1
                            614 CALL                     1
                            624 STORE_FAST               7 (points_per_segment)
                
-               481         626 LOAD_GLOBAL              5 (NULL + range)
+               482         626 LOAD_GLOBAL              5 (NULL + range)
                            638 LOAD_FAST                0 (self)
                            640 LOAD_ATTR                3 (first_valid_point)
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR                4 (last_valid_point)
                            662 PRECALL                  2
                            666 CALL                     2
                            676 GET_ITER
                        >>  678 FOR_ITER                54 (to 788)
                            680 STORE_FAST               3 (i)
                
-               482         682 LOAD_FAST                3 (i)
+               483         682 LOAD_FAST                3 (i)
                            684 LOAD_FAST                7 (points_per_segment)
                            686 BINARY_OP                2 (//)
                            690 STORE_FAST               8 (m)
                
-               483         692 LOAD_FAST                2 (data)
+               484         692 LOAD_FAST                2 (data)
                            694 LOAD_METHOD              5 (append)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                6 (horizontal_interval)
                            728 LOAD_FAST                3 (i)
                            730 BINARY_OP                5 (*)
                            734 LOAD_FAST                5 (trigger_offsets)
                            736 LOAD_FAST                8 (m)
@@ -3447,135 +3444,135 @@
                            756 BINARY_SUBSCR
                            766 BINARY_OP                0 (+)
                            770 PRECALL                  1
                            774 CALL                     1
                            784 POP_TOP
                            786 JUMP_BACKWARD           55 (to 678)
                
-               485     >>  788 LOAD_GLOBAL             17 (NULL + np)
+               486     >>  788 LOAD_GLOBAL             17 (NULL + np)
                            800 LOAD_ATTR                9 (array)
                            810 LOAD_FAST                2 (data)
                            812 PRECALL                  1
                            816 CALL                     1
                            826 LOAD_FAST                0 (self)
                            828 STORE_ATTR              10 (data_x)
                            838 LOAD_CONST               5 (None)
                            840 RETURN_VALUE
                
-               486     >>  842 LOAD_FAST                0 (self)
+               487     >>  842 LOAD_FAST                0 (self)
                            844 LOAD_ATTR               15 (ris_sweeps)
                            854 LOAD_CONST               2 (1)
                            856 COMPARE_OP               3 (!=)
                            862 POP_JUMP_FORWARD_IF_FALSE   195 (to 1254)
                
-               488         864 BUILD_LIST               0
+               489         864 BUILD_LIST               0
                            866 STORE_FAST               9 (offsets)
                
-               489         868 LOAD_GLOBAL              5 (NULL + range)
+               490         868 LOAD_GLOBAL              5 (NULL + range)
                            880 LOAD_CONST               1 (0)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               15 (ris_sweeps)
                            894 PRECALL                  2
                            898 CALL                     2
                            908 GET_ITER
                        >>  910 FOR_ITER                60 (to 1032)
                            912 STORE_FAST               3 (i)
                
-               490         914 LOAD_FAST                3 (i)
+               491         914 LOAD_FAST                3 (i)
                            916 LOAD_CONST               4 (8)
                            918 BINARY_OP                5 (*)
                            922 STORE_FAST               6 (start_pos)
                
-               491         924 LOAD_FAST                0 (self)
+               492         924 LOAD_FAST                0 (self)
                            926 LOAD_METHOD             12 (_WaveformData__parse_to_float)
                            948 LOAD_FAST                1 (time_block)
                            950 LOAD_FAST                6 (start_pos)
                            952 LOAD_FAST                6 (start_pos)
                            954 LOAD_CONST               4 (8)
                            956 BINARY_OP                0 (+)
                            960 BUILD_SLICE              2
                            962 BINARY_SUBSCR
                            972 PRECALL                  1
                            976 CALL                     1
                            986 STORE_FAST              10 (ris_offset)
                
-               492         988 LOAD_FAST                9 (offsets)
+               493         988 LOAD_FAST                9 (offsets)
                            990 LOAD_METHOD              5 (append)
                           1012 LOAD_FAST               10 (ris_offset)
                           1014 PRECALL                  1
                           1018 CALL                     1
                           1028 POP_TOP
                           1030 JUMP_BACKWARD           61 (to 910)
                
-               493     >> 1032 BUILD_LIST               0
+               494     >> 1032 BUILD_LIST               0
                           1034 STORE_FAST               2 (data)
                
-               494        1036 LOAD_GLOBAL              5 (NULL + range)
+               495        1036 LOAD_GLOBAL              5 (NULL + range)
                           1048 LOAD_FAST                0 (self)
                           1050 LOAD_ATTR                3 (first_valid_point)
                           1060 LOAD_FAST                0 (self)
                           1062 LOAD_ATTR                4 (last_valid_point)
                           1072 PRECALL                  2
                           1076 CALL                     2
                           1086 GET_ITER
                        >> 1088 FOR_ITER                55 (to 1200)
                           1090 STORE_FAST               3 (i)
                
-               495        1092 LOAD_FAST                3 (i)
+               496        1092 LOAD_FAST                3 (i)
                           1094 LOAD_FAST                0 (self)
                           1096 LOAD_ATTR               15 (ris_sweeps)
                           1106 BINARY_OP                6 (%)
                           1110 STORE_FAST               8 (m)
                
-               496        1112 LOAD_FAST                3 (i)
+               497        1112 LOAD_FAST                3 (i)
                           1114 LOAD_FAST                8 (m)
                           1116 BINARY_OP               10 (-)
                           1120 STORE_FAST              11 (j)
                
-               497        1122 LOAD_FAST                2 (data)
+               498        1122 LOAD_FAST                2 (data)
                           1124 LOAD_METHOD              5 (append)
                           1146 LOAD_FAST                0 (self)
                           1148 LOAD_ATTR                6 (horizontal_interval)
                           1158 LOAD_FAST               11 (j)
                           1160 BINARY_OP                5 (*)
                           1164 LOAD_FAST               10 (ris_offset)
                           1166 LOAD_FAST                8 (m)
                           1168 BINARY_SUBSCR
                           1178 BINARY_OP                0 (+)
                           1182 PRECALL                  1
                           1186 CALL                     1
                           1196 POP_TOP
                           1198 JUMP_BACKWARD           56 (to 1088)
                
-               498     >> 1200 LOAD_GLOBAL             17 (NULL + np)
+               499     >> 1200 LOAD_GLOBAL             17 (NULL + np)
                           1212 LOAD_ATTR                9 (array)
                           1222 LOAD_FAST                2 (data)
                           1224 PRECALL                  1
                           1228 CALL                     1
                           1238 LOAD_FAST                0 (self)
                           1240 STORE_ATTR              10 (data_x)
                           1250 LOAD_CONST               5 (None)
                           1252 RETURN_VALUE
                
-               486     >> 1254 LOAD_CONST               5 (None)
+               487     >> 1254 LOAD_CONST               5 (None)
                           1256 RETURN_VALUE
                consts
                   'Parse the horizontal values of a waveform (i.e. the time (x) axis).'
                   0
                   1
                   16
                   8
                   None
                names      ('len', 'strip', 'range', 'first_valid_point', 'last_valid_point', 'append', 'horizontal_interval', 'horizontal_offset', 'np', 'array', 'data_x', 'nominal_subarray_count', '_WaveformData__parse_to_float', 'int', 'wave_array_count', 'ris_sweeps')
                varnames   ('self', 'time_block', 'data', 'i', 'first_trig_times', 'trigger_offsets', 'start_pos', 'points_per_segment', 'm', 'offsets', 'ris_offset', 'j')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_horizontal_values'
-               firstlineno 457
+               firstlineno 458
                lnotab
                   0x02044a03040138014c01360118030402040104012e010a0166016e0238
                   0138010a0160023601160204012e010a0140012c010401380114010a014e
                   0136f4
             'data_block_1'
             'data_block_2'
             code
@@ -3616,658 +3613,722 @@
                   000000000001008c477c006a060000000000000000740f00000000000000
                   0000006a0800000000000000007c07a6010000ab0100000000000000007a
                   0500007c006a0900000000000000007a0a00007d07741500000000000000
                   0000007c07a6010000ab01000000000000000064016b0300000000721d74
                   0f000000000000000000006a0800000000000000007c037c076702a60100
                   00ab0100000000000000007c005f0d0000000000000000640253007c037c
                   005f0d000000000000000064025300
-               500           0 RESUME                   0
+               501           0 RESUME                   0
                
-               504           2 BUILD_LIST               0
+               505           2 BUILD_LIST               0
                              4 STORE_FAST               3 (data_1)
                
-               505           6 LOAD_GLOBAL              1 (NULL + range)
+               506           6 LOAD_GLOBAL              1 (NULL + range)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (first_valid_point)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (last_valid_point)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 GET_ITER
                        >>   58 FOR_ITER                70 (to 200)
                             60 STORE_FAST               4 (i)
                
-               506          62 LOAD_FAST                4 (i)
+               507          62 LOAD_FAST                4 (i)
                             64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                3 (wf_datapoint_size)
                             76 BINARY_OP                5 (*)
                             80 STORE_FAST               5 (start_pos)
                
-               507          82 LOAD_FAST                1 (data_block_1)
+               508          82 LOAD_FAST                1 (data_block_1)
                             84 LOAD_FAST                5 (start_pos)
                             86 LOAD_FAST                5 (start_pos)
                             88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                3 (wf_datapoint_size)
                            100 BINARY_OP                0 (+)
                            104 BUILD_SLICE              2
                            106 BINARY_SUBSCR
                            116 STORE_FAST               6 (data)
                
-               508         118 LOAD_FAST                3 (data_1)
+               509         118 LOAD_FAST                3 (data_1)
                            120 LOAD_METHOD              4 (append)
                            142 LOAD_FAST                0 (self)
                            144 LOAD_METHOD              5 (_WaveformData__parse_to_int)
                            166 LOAD_FAST                6 (data)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 PRECALL                  1
                            186 CALL                     1
                            196 POP_TOP
                            198 JUMP_BACKWARD           71 (to 58)
                
-               509     >>  200 LOAD_FAST                0 (self)
+               510     >>  200 LOAD_FAST                0 (self)
                            202 LOAD_ATTR                6 (vertical_gain)
                            212 LOAD_GLOBAL             15 (NULL + np)
                            224 LOAD_ATTR                8 (array)
                            234 LOAD_FAST                3 (data_1)
                            236 PRECALL                  1
                            240 CALL                     1
                            250 BINARY_OP                5 (*)
                            254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                9 (vertical_offset)
                            266 BINARY_OP               10 (-)
                            270 STORE_FAST               3 (data_1)
                
-               512         272 BUILD_LIST               0
+               513         272 BUILD_LIST               0
                            274 STORE_FAST               7 (data_2)
                
-               513         276 LOAD_GLOBAL             21 (NULL + len)
+               514         276 LOAD_GLOBAL             21 (NULL + len)
                            288 LOAD_FAST                2 (data_block_2)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 LOAD_CONST               1 (0)
                            306 COMPARE_OP               3 (!=)
                            312 EXTENDED_ARG             1
                            314 POP_JUMP_FORWARD_IF_FALSE   317 (to 950)
                
-               515         316 LOAD_GLOBAL             21 (NULL + len)
+               516         316 LOAD_GLOBAL             21 (NULL + len)
                            328 LOAD_FAST                2 (data_block_2)
                            330 PRECALL                  1
                            334 CALL                     1
                            344 LOAD_GLOBAL             21 (NULL + len)
                            356 LOAD_FAST                1 (data_block_1)
                            358 PRECALL                  1
                            362 CALL                     1
                            372 COMPARE_OP               3 (!=)
                            378 POP_JUMP_FORWARD_IF_FALSE   152 (to 684)
                
-               517         380 LOAD_GLOBAL              1 (NULL + range)
+               518         380 LOAD_GLOBAL              1 (NULL + range)
                            392 LOAD_FAST                0 (self)
                            394 LOAD_ATTR                1 (first_valid_point)
                            404 LOAD_FAST                0 (self)
                            406 LOAD_ATTR                2 (last_valid_point)
                            416 PRECALL                  2
                            420 CALL                     2
                            430 GET_ITER
                        >>  432 FOR_ITER                88 (to 610)
                            434 STORE_FAST               4 (i)
                
-               518         436 LOAD_FAST                4 (i)
+               519         436 LOAD_FAST                4 (i)
                            438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR               11 (points_per_pair)
                            450 BINARY_OP                6 (%)
                            454 STORE_FAST               8 (m)
                
-               519         456 LOAD_FAST                8 (m)
+               520         456 LOAD_FAST                8 (m)
                            458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR               12 (pair_offset)
                            470 BINARY_OP                0 (+)
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                3 (wf_datapoint_size)
                            486 BINARY_OP                5 (*)
                            490 STORE_FAST               5 (start_pos)
                
-               520         492 LOAD_FAST                2 (data_block_2)
+               521         492 LOAD_FAST                2 (data_block_2)
                            494 LOAD_FAST                5 (start_pos)
                            496 LOAD_FAST                5 (start_pos)
                            498 LOAD_FAST                0 (self)
                            500 LOAD_ATTR                3 (wf_datapoint_size)
                            510 BINARY_OP                0 (+)
                            514 BUILD_SLICE              2
                            516 BINARY_SUBSCR
                            526 STORE_FAST               6 (data)
                
-               521         528 LOAD_FAST                7 (data_2)
+               522         528 LOAD_FAST                7 (data_2)
                            530 LOAD_METHOD              4 (append)
                            552 LOAD_FAST                0 (self)
                            554 LOAD_METHOD              5 (_WaveformData__parse_to_int)
                            576 LOAD_FAST                6 (data)
                            578 PRECALL                  1
                            582 CALL                     1
                            592 PRECALL                  1
                            596 CALL                     1
                            606 POP_TOP
                            608 JUMP_BACKWARD           89 (to 432)
                
-               522     >>  610 LOAD_FAST                0 (self)
+               523     >>  610 LOAD_FAST                0 (self)
                            612 LOAD_ATTR                6 (vertical_gain)
                            622 LOAD_GLOBAL             15 (NULL + np)
                            634 LOAD_ATTR                8 (array)
                            644 LOAD_FAST                7 (data_2)
                            646 PRECALL                  1
                            650 CALL                     1
                            660 BINARY_OP                5 (*)
                            664 LOAD_FAST                0 (self)
                            666 LOAD_ATTR                9 (vertical_offset)
                            676 BINARY_OP               10 (-)
                            680 STORE_FAST               7 (data_2)
                            682 JUMP_FORWARD           133 (to 950)
                
-               525     >>  684 LOAD_GLOBAL              1 (NULL + range)
+               526     >>  684 LOAD_GLOBAL              1 (NULL + range)
                            696 LOAD_FAST                0 (self)
                            698 LOAD_ATTR                1 (first_valid_point)
                            708 LOAD_FAST                0 (self)
                            710 LOAD_ATTR                2 (last_valid_point)
                            720 PRECALL                  2
                            724 CALL                     2
                            734 GET_ITER
                        >>  736 FOR_ITER                70 (to 878)
                            738 STORE_FAST               4 (i)
                
-               526         740 LOAD_FAST                4 (i)
+               527         740 LOAD_FAST                4 (i)
                            742 LOAD_FAST                0 (self)
                            744 LOAD_ATTR                3 (wf_datapoint_size)
                            754 BINARY_OP                5 (*)
                            758 STORE_FAST               9 (start_post)
                
-               527         760 LOAD_FAST                2 (data_block_2)
+               528         760 LOAD_FAST                2 (data_block_2)
                            762 LOAD_FAST                5 (start_pos)
                            764 LOAD_FAST                5 (start_pos)
                            766 LOAD_FAST                0 (self)
                            768 LOAD_ATTR                3 (wf_datapoint_size)
                            778 BINARY_OP                0 (+)
                            782 BUILD_SLICE              2
                            784 BINARY_SUBSCR
                            794 STORE_FAST               6 (data)
                
-               528         796 LOAD_FAST                7 (data_2)
+               529         796 LOAD_FAST                7 (data_2)
                            798 LOAD_METHOD              4 (append)
                            820 LOAD_FAST                0 (self)
                            822 LOAD_METHOD              5 (_WaveformData__parse_to_int)
                            844 LOAD_FAST                6 (data)
                            846 PRECALL                  1
                            850 CALL                     1
                            860 PRECALL                  1
                            864 CALL                     1
                            874 POP_TOP
                            876 JUMP_BACKWARD           71 (to 736)
                
-               529     >>  878 LOAD_FAST                0 (self)
+               530     >>  878 LOAD_FAST                0 (self)
                            880 LOAD_ATTR                6 (vertical_gain)
                            890 LOAD_GLOBAL             15 (NULL + np)
                            902 LOAD_ATTR                8 (array)
                            912 LOAD_FAST                7 (data_2)
                            914 PRECALL                  1
                            918 CALL                     1
                            928 BINARY_OP                5 (*)
                            932 LOAD_FAST                0 (self)
                            934 LOAD_ATTR                9 (vertical_offset)
                            944 BINARY_OP               10 (-)
                            948 STORE_FAST               7 (data_2)
                
-               531     >>  950 LOAD_GLOBAL             21 (NULL + len)
+               532     >>  950 LOAD_GLOBAL             21 (NULL + len)
                            962 LOAD_FAST                7 (data_2)
                            964 PRECALL                  1
                            968 CALL                     1
                            978 LOAD_CONST               1 (0)
                            980 COMPARE_OP               3 (!=)
                            986 POP_JUMP_FORWARD_IF_FALSE    29 (to 1046)
                
-               532         988 LOAD_GLOBAL             15 (NULL + np)
+               533         988 LOAD_GLOBAL             15 (NULL + np)
                           1000 LOAD_ATTR                8 (array)
                           1010 LOAD_FAST                3 (data_1)
                           1012 LOAD_FAST                7 (data_2)
                           1014 BUILD_LIST               2
                           1016 PRECALL                  1
                           1020 CALL                     1
                           1030 LOAD_FAST                0 (self)
                           1032 STORE_ATTR              13 (data_y)
                           1042 LOAD_CONST               2 (None)
                           1044 RETURN_VALUE
                
-               534     >> 1046 LOAD_FAST                3 (data_1)
+               535     >> 1046 LOAD_FAST                3 (data_1)
                           1048 LOAD_FAST                0 (self)
                           1050 STORE_ATTR              13 (data_y)
                           1060 LOAD_CONST               2 (None)
                           1062 RETURN_VALUE
                consts
                   'Parse the vertical values of a waveform (i.e. the amplitude (y) axis)'
                   0
                   None
                names      ('range', 'first_valid_point', 'last_valid_point', 'wf_datapoint_size', 'append', '_WaveformData__parse_to_int', 'vertical_gain', 'np', 'array', 'vertical_offset', 'len', 'points_per_pair', 'pair_offset', 'data_y')
                varnames   ('self', 'data_block_1', 'data_block_2', 'data_1', 'i', 'start_pos', 'data', 'data_2', 'm', 'start_post')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__parse_vertical_values'
-               firstlineno 500
+               firstlineno 501
                lnotab
                   0x0204040138011401240152014803040128024002380114012401240152
                   014a033801140124015201480226013a02
-            'desc'
-            'text'
-            'time'
-            'dat1'
-            'dat2'
             code
-               argcount  : 6
-               nlocals   : 9
-               stacksize : 6
+               argcount  : 2
+               nlocals   : 8
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c017c027c037c047c0564019c057d067c0644005d337d077c067c
-                  0719000000000000000000a0000000000000000000000000000000000000
-                  0000006402a6010000ab0100000000000000007d087c067c071900000000
-                  00000000007c0864037a00000064008502190000000000000000007c067c
-                  073c0000008c347c066404190000000000000000007d017c00a001000000
-                  00000000000000000000000000000000007c066404190000000000000000
-                  00a6010000ab01000000000000000001007c00a002000000000000000000
-                  00000000000000000000007c06640519000000000000000000a6010000ab
-                  01000000000000000001007c00a003000000000000000000000000000000
-                  00000000007c06640619000000000000000000a6010000ab010000000000
-                  00000001007c00a00400000000000000000000000000000000000000007c
-                  06640719000000000000000000a005000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007c06640819000000000000
-                  000000a0050000000000000000000000000000000000000000a6000000ab
-                  000000000000000000a6020000ab020000000000000000010064005300
-               536           0 RESUME                   0
-               
-               543           2 LOAD_FAST                1 (desc)
-               
-               544           4 LOAD_FAST                2 (text)
-               
-               545           6 LOAD_FAST                3 (time)
-               
-               546           8 LOAD_FAST                4 (dat1)
-               
-               547          10 LOAD_FAST                5 (dat2)
-               
-               542          12 LOAD_CONST               1 (('desc', 'text', 'time', 'dat1', 'dat2'))
-                            14 BUILD_CONST_KEY_MAP      5
-                            16 STORE_FAST               6 (blocks)
-               
-               551          18 LOAD_FAST                6 (blocks)
-                            20 GET_ITER
-                       >>   22 FOR_ITER                51 (to 126)
-                            24 STORE_FAST               7 (key)
-               
-               552          26 LOAD_FAST                6 (blocks)
-                            28 LOAD_FAST                7 (key)
-                            30 BINARY_SUBSCR
-                            40 LOAD_METHOD              0 (index)
-                            62 LOAD_CONST               2 (b'#9')
-                            64 PRECALL                  1
-                            68 CALL                     1
-                            78 STORE_FAST               8 (start_pos)
-               
-               553          80 LOAD_FAST                6 (blocks)
-                            82 LOAD_FAST                7 (key)
-                            84 BINARY_SUBSCR
-                            94 LOAD_FAST                8 (start_pos)
-                            96 LOAD_CONST               3 (11)
-                            98 BINARY_OP                0 (+)
-                           102 LOAD_CONST               0 (None)
-                           104 BUILD_SLICE              2
-                           106 BINARY_SUBSCR
-                           116 LOAD_FAST                6 (blocks)
-                           118 LOAD_FAST                7 (key)
-                           120 STORE_SUBSCR
-                           124 JUMP_BACKWARD           52 (to 22)
-               
-               556     >>  126 LOAD_FAST                6 (blocks)
-                           128 LOAD_CONST               4 ('desc')
-                           130 BINARY_SUBSCR
-                           140 STORE_FAST               1 (desc)
-               
-               559         142 LOAD_FAST                0 (self)
-                           144 LOAD_METHOD              1 (_WaveformData__parse_wavedesc)
-                           166 LOAD_FAST                6 (blocks)
-                           168 LOAD_CONST               4 ('desc')
-                           170 BINARY_SUBSCR
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 POP_TOP
-               
-               562         196 LOAD_FAST                0 (self)
-                           198 LOAD_METHOD              2 (_WaveformData__parse_usertext)
-                           220 LOAD_FAST                6 (blocks)
-                           222 LOAD_CONST               5 ('text')
-                           224 BINARY_SUBSCR
-                           234 PRECALL                  1
-                           238 CALL                     1
-                           248 POP_TOP
-               
-               565         250 LOAD_FAST                0 (self)
-                           252 LOAD_METHOD              3 (_WaveformData__parse_horizontal_values)
-                           274 LOAD_FAST                6 (blocks)
-                           276 LOAD_CONST               6 ('time')
-                           278 BINARY_SUBSCR
-                           288 PRECALL                  1
-                           292 CALL                     1
-                           302 POP_TOP
-               
-               568         304 LOAD_FAST                0 (self)
-                           306 LOAD_METHOD              4 (_WaveformData__parse_vertical_values)
-                           328 LOAD_FAST                6 (blocks)
-                           330 LOAD_CONST               7 ('dat1')
-                           332 BINARY_SUBSCR
-                           342 LOAD_METHOD              5 (strip)
-                           364 PRECALL                  0
-                           368 CALL                     0
-                           378 LOAD_FAST                6 (blocks)
-                           380 LOAD_CONST               8 ('dat2')
-                           382 BINARY_SUBSCR
-                           392 LOAD_METHOD              5 (strip)
-                           414 PRECALL                  0
-                           418 CALL                     0
-                           428 PRECALL                  2
-                           432 CALL                     2
-                           442 POP_TOP
-                           444 LOAD_CONST               0 (None)
-                           446 RETURN_VALUE
+                  0x97007c01a00000000000000000000000000000000000000000006401a6
+                  010000ab0100000000000000007d027c017c0264027a0000006400850219
+                  0000000000000000007d017c00a001000000000000000000000000000000
+                  00000000007c01a6010000ab01000000000000000001007c006a02000000
+                  000000000064036b030000000072087c006a0200000000000000007d036e
+                  157c006a03000000000000000064036b030000000072087c006a03000000
+                  00000000007d036e0264037d037c017c006a0400000000000000007c006a
+                  0400000000000000007c006a0500000000000000007a0000008502190000
+                  000000000000007d047c017c006a0400000000000000007c006a05000000
+                  00000000007a0000007c006a0400000000000000007c006a050000000000
+                  0000007a0000007c037a0000008502190000000000000000007d057c017c
+                  006a0400000000000000007c006a0500000000000000007a0000007c037a
+                  0000007c006a0400000000000000007c006a0500000000000000007a0000
+                  007c037a0000007c006a0600000000000000007a00000085021900000000
+                  00000000007d067c017c006a0400000000000000007c006a050000000000
+                  0000007a0000007c037a0000007c006a0600000000000000007a0000007c
+                  006a0400000000000000007c006a0500000000000000007a0000007c037a
+                  0000007c006a0600000000000000007a0000007c006a0700000000000000
+                  007a0000008502190000000000000000007d077c00a00800000000000000
+                  000000000000000000000000007c04a6010000ab01000000000000000001
+                  007c00a00900000000000000000000000000000000000000007c05a60100
+                  00ab01000000000000000001007c00a00a00000000000000000000000000
+                  000000000000007c067c07a6020000ab0200000000000000000100640053
+                  00
+               571           0 RESUME                   0
+               
+               573           2 LOAD_FAST                1 (data)
+                             4 LOAD_METHOD              0 (index)
+                            26 LOAD_CONST               1 (b'#9')
+                            28 PRECALL                  1
+                            32 CALL                     1
+                            42 STORE_FAST               2 (start_pos)
+               
+               574          44 LOAD_FAST                1 (data)
+                            46 LOAD_FAST                2 (start_pos)
+                            48 LOAD_CONST               2 (11)
+                            50 BINARY_OP                0 (+)
+                            54 LOAD_CONST               0 (None)
+                            56 BUILD_SLICE              2
+                            58 BINARY_SUBSCR
+                            68 STORE_FAST               1 (data)
+               
+               577          70 LOAD_FAST                0 (self)
+                            72 LOAD_METHOD              1 (_WaveformData__parse_wavedesc)
+                            94 LOAD_FAST                1 (data)
+                            96 PRECALL                  1
+                           100 CALL                     1
+                           110 POP_TOP
+               
+               579         112 LOAD_FAST                0 (self)
+                           114 LOAD_ATTR                2 (trigtime_array_size)
+                           124 LOAD_CONST               3 (0)
+                           126 COMPARE_OP               3 (!=)
+                           132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
+               
+               580         134 LOAD_FAST                0 (self)
+                           136 LOAD_ATTR                2 (trigtime_array_size)
+                           146 STORE_FAST               3 (time_array_size)
+                           148 JUMP_FORWARD            21 (to 192)
+               
+               581     >>  150 LOAD_FAST                0 (self)
+                           152 LOAD_ATTR                3 (ris_time_array_size)
+                           162 LOAD_CONST               3 (0)
+                           164 COMPARE_OP               3 (!=)
+                           170 POP_JUMP_FORWARD_IF_FALSE     8 (to 188)
+               
+               582         172 LOAD_FAST                0 (self)
+                           174 LOAD_ATTR                3 (ris_time_array_size)
+                           184 STORE_FAST               3 (time_array_size)
+                           186 JUMP_FORWARD             2 (to 192)
+               
+               584     >>  188 LOAD_CONST               3 (0)
+                           190 STORE_FAST               3 (time_array_size)
+               
+               587     >>  192 LOAD_FAST                1 (data)
+                           194 LOAD_FAST                0 (self)
+                           196 LOAD_ATTR                4 (wave_desc_size)
+                           206 LOAD_FAST                0 (self)
+                           208 LOAD_ATTR                4 (wave_desc_size)
+                           218 LOAD_FAST                0 (self)
+                           220 LOAD_ATTR                5 (user_text_size)
+                           230 BINARY_OP                0 (+)
+                           234 BUILD_SLICE              2
+                           236 BINARY_SUBSCR
+                           246 STORE_FAST               4 (text)
+               
+               588         248 LOAD_FAST                1 (data)
+                           250 LOAD_FAST                0 (self)
+                           252 LOAD_ATTR                4 (wave_desc_size)
+                           262 LOAD_FAST                0 (self)
+                           264 LOAD_ATTR                5 (user_text_size)
+                           274 BINARY_OP                0 (+)
+                           278 LOAD_FAST                0 (self)
+                           280 LOAD_ATTR                4 (wave_desc_size)
+                           290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                5 (user_text_size)
+                           302 BINARY_OP                0 (+)
+                           306 LOAD_FAST                3 (time_array_size)
+                           308 BINARY_OP                0 (+)
+                           312 BUILD_SLICE              2
+                           314 BINARY_SUBSCR
+                           324 STORE_FAST               5 (time)
+               
+               589         326 LOAD_FAST                1 (data)
+                           328 LOAD_FAST                0 (self)
+                           330 LOAD_ATTR                4 (wave_desc_size)
+                           340 LOAD_FAST                0 (self)
+                           342 LOAD_ATTR                5 (user_text_size)
+                           352 BINARY_OP                0 (+)
+                           356 LOAD_FAST                3 (time_array_size)
+                           358 BINARY_OP                0 (+)
+                           362 LOAD_FAST                0 (self)
+                           364 LOAD_ATTR                4 (wave_desc_size)
+                           374 LOAD_FAST                0 (self)
+                           376 LOAD_ATTR                5 (user_text_size)
+                           386 BINARY_OP                0 (+)
+                           390 LOAD_FAST                3 (time_array_size)
+                           392 BINARY_OP                0 (+)
+                           396 LOAD_FAST                0 (self)
+                           398 LOAD_ATTR                6 (dat1_array_size)
+                           408 BINARY_OP                0 (+)
+                           412 BUILD_SLICE              2
+                           414 BINARY_SUBSCR
+                           424 STORE_FAST               6 (dat1)
+               
+               590         426 LOAD_FAST                1 (data)
+                           428 LOAD_FAST                0 (self)
+                           430 LOAD_ATTR                4 (wave_desc_size)
+                           440 LOAD_FAST                0 (self)
+                           442 LOAD_ATTR                5 (user_text_size)
+                           452 BINARY_OP                0 (+)
+                           456 LOAD_FAST                3 (time_array_size)
+                           458 BINARY_OP                0 (+)
+                           462 LOAD_FAST                0 (self)
+                           464 LOAD_ATTR                6 (dat1_array_size)
+                           474 BINARY_OP                0 (+)
+                           478 LOAD_FAST                0 (self)
+                           480 LOAD_ATTR                4 (wave_desc_size)
+                           490 LOAD_FAST                0 (self)
+                           492 LOAD_ATTR                5 (user_text_size)
+                           502 BINARY_OP                0 (+)
+                           506 LOAD_FAST                3 (time_array_size)
+                           508 BINARY_OP                0 (+)
+                           512 LOAD_FAST                0 (self)
+                           514 LOAD_ATTR                6 (dat1_array_size)
+                           524 BINARY_OP                0 (+)
+                           528 LOAD_FAST                0 (self)
+                           530 LOAD_ATTR                7 (dat2_array_size)
+                           540 BINARY_OP                0 (+)
+                           544 BUILD_SLICE              2
+                           546 BINARY_SUBSCR
+                           556 STORE_FAST               7 (dat2)
+               
+               592         558 LOAD_FAST                0 (self)
+                           560 LOAD_METHOD              8 (_WaveformData__parse_usertext)
+                           582 LOAD_FAST                4 (text)
+                           584 PRECALL                  1
+                           588 CALL                     1
+                           598 POP_TOP
+               
+               593         600 LOAD_FAST                0 (self)
+                           602 LOAD_METHOD              9 (_WaveformData__parse_horizontal_values)
+                           624 LOAD_FAST                5 (time)
+                           626 PRECALL                  1
+                           630 CALL                     1
+                           640 POP_TOP
+               
+               594         642 LOAD_FAST                0 (self)
+                           644 LOAD_METHOD             10 (_WaveformData__parse_vertical_values)
+                           666 LOAD_FAST                6 (dat1)
+                           668 LOAD_FAST                7 (dat2)
+                           670 PRECALL                  2
+                           674 CALL                     2
+                           684 POP_TOP
+                           686 LOAD_CONST               0 (None)
+                           688 RETURN_VALUE
                consts
                   None
-                  ('desc', 'text', 'time', 'dat1', 'dat2')
                   b'#9'
                   11
-                  'desc'
-                  'text'
-                  'time'
-                  'dat1'
-                  'dat2'
-               names      ('index', '_WaveformData__parse_wavedesc', '_WaveformData__parse_usertext', '_WaveformData__parse_horizontal_values', '_WaveformData__parse_vertical_values', 'strip')
-               varnames   ('self', 'desc', 'text', 'time', 'dat1', 'dat2', 'blocks', 'key', 'start_pos')
+                  0
+               names      ('index', '_WaveformData__parse_wavedesc', 'trigtime_array_size', 'ris_time_array_size', 'wave_desc_size', 'user_text_size', 'dat1_array_size', 'dat2_array_size', '_WaveformData__parse_usertext', '_WaveformData__parse_horizontal_values', '_WaveformData__parse_vertical_values')
+               varnames   ('self', 'data', 'start_pos', 'time_array_size', 'text', 'time', 'dat1', 'dat2')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__init__'
-               firstlineno 536
-               lnotab 0x0207020102010201020102fb0609080136012e031003360336033603
+               firstlineno 571
+               lnotab
+                  0x02022a011a032a021601100116011002040338014e01640184022a012a
+                  01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Enum', 'RecordType', 'ProcessingDone', 'TimeBase', 'Coupling', 'VertGain', 'Source', 'Timestamp', 'str', '__annotations__', 'int', 'float', 'bool', 'bytes', '_WaveformData__parse_to_string', '_WaveformData__parse_timestamp', '_WaveformData__parse_to_int', '_WaveformData__parse_to_float', '_WaveformData__parse_wavedesc', '_WaveformData__parse_usertext', '_WaveformData__parse_horizontal_values', '_WaveformData__parse_vertical_values', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
          name       'WaveformData'
-         firstlineno 7
+         firstlineno 8
          lnotab
             0x0c0104021c111c0f1c4d1c0a1c2d1c0a1a0e0a0102010a0102020a0102
             010a0102010a0102010a0102010a0102010a0102010a0102010a0102040a
             0102010a0102010a0102010a0102010a0102040a0102010a0102010a0102
             010a0102010a0102010a0102010a0102020a0102010a0102020a0102010a
             0102010a0102020a0102010a0102010a0102010a0102020a0102020a0102
             010a0102020a0102020a0102010a0102010a0102010a0102010a0102020a
             0102010a0102020a0102040a0102010a0102010a0102010a0102010a0102
-            010a0102010a0102010a0102020c040c0e0c0f0c0d0c580c030c2b1024
+            010a0102010a0102010a0102020c040c0e0c0f0c0d0c580c030c2b1046
       'WaveformData'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 2
+         stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046a05000000000000000066
-            02640384045a06640465076602640584045a08640665096602640784045a
-            0a64085300
-         570           0 RESUME                   0
+            02640384045a0664046507640565086604640684045a0964056508640765
+            0a6604640884045a0b640465076407650a6604640984045a0c640a5300
+         597           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Waveform')
                        8 STORE_NAME               2 (__qualname__)
          
-         571          10 LOAD_CONST               1 ('Class used to transfer waveform data and parse it.')
+         598          10 LOAD_CONST               1 ('Class used to transfer waveform data and parse it.')
                       12 STORE_NAME               3 (__doc__)
          
-         573          14 LOAD_CONST               2 ('scope')
+         600          14 LOAD_CONST               2 ('scope')
                       16 LOAD_NAME                4 (pyvisa)
                       18 LOAD_ATTR                5 (Resource)
                       28 BUILD_TUPLE              2
-                      30 LOAD_CONST               3 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 573>)
+                      30 LOAD_CONST               3 (<code object __init__, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 600>)
                       32 MAKE_FUNCTION            4 (annotations)
                       34 STORE_NAME               6 (__init__)
          
-         577          36 LOAD_CONST               4 ('channel')
+         603          36 LOAD_CONST               4 ('source')
                       38 LOAD_NAME                7 (Channel)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object transfer_from_device, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 577>)
-                      44 MAKE_FUNCTION            4 (annotations)
-                      46 STORE_NAME               8 (transfer_from_device)
-         
-         596          48 LOAD_CONST               6 ('return')
-                      50 LOAD_NAME                9 (WaveformData)
-                      52 BUILD_TUPLE              2
-                      54 LOAD_CONST               7 (<code object get_data, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 596>)
-                      56 MAKE_FUNCTION            4 (annotations)
-                      58 STORE_NAME              10 (get_data)
-                      60 LOAD_CONST               8 (None)
-                      62 RETURN_VALUE
+                      40 LOAD_CONST               5 ('filepath')
+                      42 LOAD_NAME                8 (str)
+                      44 BUILD_TUPLE              4
+                      46 LOAD_CONST               6 (<code object dump_data_to_file, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 603>)
+                      48 MAKE_FUNCTION            4 (annotations)
+                      50 STORE_NAME               9 (dump_data_to_file)
+         
+         615          52 LOAD_CONST               5 ('filepath')
+                      54 LOAD_NAME                8 (str)
+                      56 LOAD_CONST               7 ('return')
+                      58 LOAD_NAME               10 (WaveformData)
+                      60 BUILD_TUPLE              4
+                      62 LOAD_CONST               8 (<code object parse_data_from_binary, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 615>)
+                      64 MAKE_FUNCTION            4 (annotations)
+                      66 STORE_NAME              11 (parse_data_from_binary)
+         
+         627          68 LOAD_CONST               4 ('source')
+                      70 LOAD_NAME                7 (Channel)
+                      72 LOAD_CONST               7 ('return')
+                      74 LOAD_NAME               10 (WaveformData)
+                      76 BUILD_TUPLE              4
+                      78 LOAD_CONST               9 (<code object get_data, file "/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py", line 627>)
+                      80 MAKE_FUNCTION            4 (annotations)
+                      82 STORE_NAME              12 (get_data)
+                      84 LOAD_CONST              10 (None)
+                      86 RETURN_VALUE
          consts
             'Waveform'
             'Class used to transfer waveform data and parse it.'
             'scope'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
-               code
-                  0x97007c017c005f00000000000000000064007c005f0100000000000000
-                  0064005300
-               573           0 RESUME                   0
+               code 0x97007c017c005f00000000000000000064005300
+               600           0 RESUME                   0
                
-               574           2 LOAD_FAST                1 (scope)
+               601           2 LOAD_FAST                1 (scope)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (_Waveform__scope)
-               
-               575          16 LOAD_CONST               0 (None)
-                            18 LOAD_FAST                0 (self)
-                            20 STORE_ATTR               1 (_Waveform__waveform_data)
-                            30 LOAD_CONST               0 (None)
-                            32 RETURN_VALUE
+                            16 LOAD_CONST               0 (None)
+                            18 RETURN_VALUE
                consts
                   None
-               names      ('_Waveform__scope', '_Waveform__waveform_data')
+               names      ('_Waveform__scope',)
                varnames   ('self', 'scope')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       '__init__'
-               firstlineno 573
-               lnotab 0x02010e01
-            'channel'
+               firstlineno 600
+               lnotab 0x0201
+            'source'
+            'filepath'
             code
-               argcount  : 2
-               nlocals   : 7
-               stacksize : 7
+               argcount  : 3
+               nlocals   : 5
+               stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c019b0064019d02a6010000ab01000000000000000001
                   007c006a000000000000000000a002000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d027c006a000000000000
-                  000000a00100000000000000000000000000000000000000007c019b0064
-                  029d02a6010000ab01000000000000000001007c006a0000000000000000
-                  00a0020000000000000000000000000000000000000000a6000000ab0000
-                  000000000000007d037c006a000000000000000000a00100000000000000
-                  000000000000000000000000007c019b0064039d02a6010000ab01000000
-                  000000000001007c006a000000000000000000a002000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000007d047c006a
-                  000000000000000000a00100000000000000000000000000000000000000
-                  007c019b0064049d02a6010000ab01000000000000000001007c006a0000
-                  00000000000000a0020000000000000000000000000000000000000000a6
-                  000000ab0000000000000000007d057c006a000000000000000000a00100
-                  000000000000000000000000000000000000007c019b0064059d02a60100
-                  00ab01000000000000000001007c006a000000000000000000a002000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  007d067407000000000000000000007c027c037c047c057c06a6050000ab
-                  0500000000000000007c005f04000000000000000064065300
-               577           0 RESUME                   0
+                  0000000000a6000000ab0000000000000000007d03740700000000000000
+                  0000007c026402a6020000ab0200000000000000007d0474090000000000
+                  00000000006a0500000000000000007c037c04a6020000ab020000000000
+                  00000001007c04a0060000000000000000000000000000000000000000a6
+                  000000ab000000000000000000010064035300
+               603           0 RESUME                   0
                
-               582           2 LOAD_FAST                0 (self)
+               607           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_Waveform__scope)
                             14 LOAD_METHOD              1 (write)
-                            36 LOAD_FAST                1 (channel)
+                            36 LOAD_FAST                1 (source)
                             38 FORMAT_VALUE             0
-                            40 LOAD_CONST               1 (':WF? DESC')
+                            40 LOAD_CONST               1 (':WF? ALL')
                             42 BUILD_STRING             2
                             44 PRECALL                  1
                             48 CALL                     1
                             58 POP_TOP
                
-               583          60 LOAD_FAST                0 (self)
+               608          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                0 (_Waveform__scope)
                             72 LOAD_METHOD              2 (read_raw)
                             94 PRECALL                  0
                             98 CALL                     0
-                           108 STORE_FAST               2 (desc)
+                           108 STORE_FAST               3 (data)
                
-               584         110 LOAD_FAST                0 (self)
-                           112 LOAD_ATTR                0 (_Waveform__scope)
-                           122 LOAD_METHOD              1 (write)
-                           144 LOAD_FAST                1 (channel)
-                           146 FORMAT_VALUE             0
-                           148 LOAD_CONST               2 (':WF? TEXT')
-                           150 BUILD_STRING             2
-                           152 PRECALL                  1
-                           156 CALL                     1
-                           166 POP_TOP
-               
-               585         168 LOAD_FAST                0 (self)
-                           170 LOAD_ATTR                0 (_Waveform__scope)
-                           180 LOAD_METHOD              2 (read_raw)
-                           202 PRECALL                  0
-                           206 CALL                     0
-                           216 STORE_FAST               3 (text)
-               
-               586         218 LOAD_FAST                0 (self)
-                           220 LOAD_ATTR                0 (_Waveform__scope)
-                           230 LOAD_METHOD              1 (write)
-                           252 LOAD_FAST                1 (channel)
-                           254 FORMAT_VALUE             0
-                           256 LOAD_CONST               3 (':WF? TIME')
-                           258 BUILD_STRING             2
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 POP_TOP
-               
-               587         276 LOAD_FAST                0 (self)
-                           278 LOAD_ATTR                0 (_Waveform__scope)
-                           288 LOAD_METHOD              2 (read_raw)
-                           310 PRECALL                  0
-                           314 CALL                     0
-                           324 STORE_FAST               4 (time)
-               
-               588         326 LOAD_FAST                0 (self)
-                           328 LOAD_ATTR                0 (_Waveform__scope)
-                           338 LOAD_METHOD              1 (write)
-                           360 LOAD_FAST                1 (channel)
-                           362 FORMAT_VALUE             0
-                           364 LOAD_CONST               4 (':WF? DAT1')
-                           366 BUILD_STRING             2
-                           368 PRECALL                  1
-                           372 CALL                     1
-                           382 POP_TOP
-               
-               589         384 LOAD_FAST                0 (self)
-                           386 LOAD_ATTR                0 (_Waveform__scope)
-                           396 LOAD_METHOD              2 (read_raw)
-                           418 PRECALL                  0
-                           422 CALL                     0
-                           432 STORE_FAST               5 (dat1)
-               
-               590         434 LOAD_FAST                0 (self)
-                           436 LOAD_ATTR                0 (_Waveform__scope)
-                           446 LOAD_METHOD              1 (write)
-                           468 LOAD_FAST                1 (channel)
-                           470 FORMAT_VALUE             0
-                           472 LOAD_CONST               5 (':WF? DAT2')
-                           474 BUILD_STRING             2
-                           476 PRECALL                  1
-                           480 CALL                     1
-                           490 POP_TOP
-               
-               591         492 LOAD_FAST                0 (self)
-                           494 LOAD_ATTR                0 (_Waveform__scope)
-                           504 LOAD_METHOD              2 (read_raw)
-                           526 PRECALL                  0
-                           530 CALL                     0
-                           540 STORE_FAST               6 (dat2)
-               
-               594         542 LOAD_GLOBAL              7 (NULL + WaveformData)
-                           554 LOAD_FAST                2 (desc)
-                           556 LOAD_FAST                3 (text)
-                           558 LOAD_FAST                4 (time)
-                           560 LOAD_FAST                5 (dat1)
-                           562 LOAD_FAST                6 (dat2)
-                           564 PRECALL                  5
-                           568 CALL                     5
-                           578 LOAD_FAST                0 (self)
-                           580 STORE_ATTR               4 (_Waveform__waveform_data)
-                           590 LOAD_CONST               6 (None)
-                           592 RETURN_VALUE
+               610         110 LOAD_GLOBAL              7 (NULL + open)
+                           122 LOAD_FAST                2 (filepath)
+                           124 LOAD_CONST               2 ('wb')
+                           126 PRECALL                  2
+                           130 CALL                     2
+                           140 STORE_FAST               4 (file)
+               
+               612         142 LOAD_GLOBAL              9 (NULL + pickle)
+                           154 LOAD_ATTR                5 (dump)
+                           164 LOAD_FAST                3 (data)
+                           166 LOAD_FAST                4 (file)
+                           168 PRECALL                  2
+                           172 CALL                     2
+                           182 POP_TOP
+               
+               613         184 LOAD_FAST                4 (file)
+                           186 LOAD_METHOD              6 (close)
+                           208 PRECALL                  0
+                           212 CALL                     0
+                           222 POP_TOP
+                           224 LOAD_CONST               3 (None)
+                           226 RETURN_VALUE
                consts
-                  'Load the waveform data into the Waveform class. This function must be called prior to other methods.'
-                  ':WF? DESC'
-                  ':WF? TEXT'
-                  ':WF? TIME'
-                  ':WF? DAT1'
-                  ':WF? DAT2'
+                  'Dump the binary data from the device to a file.'
+                  ':WF? ALL'
+                  'wb'
                   None
-               names      ('_Waveform__scope', 'write', 'read_raw', 'WaveformData', '_Waveform__waveform_data')
-               varnames   ('self', 'channel', 'desc', 'text', 'time', 'dat1', 'dat2')
+               names      ('_Waveform__scope', 'write', 'read_raw', 'open', 'pickle', 'dump', 'close')
+               varnames   ('self', 'source', 'filepath', 'data', 'file')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
-               name       'transfer_from_device'
-               firstlineno 577
-               lnotab 0x02053a0132013a0132013a0132013a0132013a013203
+               name       'dump_data_to_file'
+               firstlineno 603
+               lnotab 0x02043a01320220022a01
             'return'
             code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c016401a6020000ab020000000000
+                  0000007d027403000000000000000000006a0200000000000000007c02a6
+                  010000ab0100000000000000007d037c02a0030000000000000000000000
+                  000000000000000000a6000000ab00000000000000000001007409000000
+                  000000000000007c03a6010000ab0100000000000000005300
+               615           0 RESUME                   0
+               
+               619           2 LOAD_GLOBAL              1 (NULL + open)
+                            14 LOAD_FAST                1 (filepath)
+                            16 LOAD_CONST               1 ('rb')
+                            18 PRECALL                  2
+                            22 CALL                     2
+                            32 STORE_FAST               2 (file)
+               
+               620          34 LOAD_GLOBAL              3 (NULL + pickle)
+                            46 LOAD_ATTR                2 (load)
+                            56 LOAD_FAST                2 (file)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 STORE_FAST               3 (data)
+               
+               621          74 LOAD_FAST                2 (file)
+                            76 LOAD_METHOD              3 (close)
+                            98 PRECALL                  0
+                           102 CALL                     0
+                           112 POP_TOP
+               
+               624         114 LOAD_GLOBAL              9 (NULL + WaveformData)
+                           126 LOAD_FAST                3 (data)
+                           128 PRECALL                  1
+                           132 CALL                     1
+                           142 RETURN_VALUE
+               consts
+                  'Read the binary from a file to a WaveformData object.'
+                  'rb'
+               names      ('open', 'pickle', 'load', 'close', 'WaveformData')
+               varnames   ('self', 'filepath', 'file', 'data')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
+               name       'parse_data_from_binary'
+               firstlineno 615
+               lnotab 0x0204200128012803
+            code
+               argcount  : 2
+               nlocals   : 3
+               stacksize : 4
                flags     : 3
-               code 0x97007c006a0000000000000000005300
-               596           0 RESUME                   0
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c019b0064019d02a6010000ab01000000000000000001
+                  007c006a000000000000000000a002000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000007d02740700000000000000
+                  0000007c02a6010000ab0100000000000000005300
+               627           0 RESUME                   0
                
-               598           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (_Waveform__waveform_data)
-                            14 RETURN_VALUE
+               631           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_Waveform__scope)
+                            14 LOAD_METHOD              1 (write)
+                            36 LOAD_FAST                1 (source)
+                            38 FORMAT_VALUE             0
+                            40 LOAD_CONST               1 (':WF? ALL')
+                            42 BUILD_STRING             2
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 POP_TOP
+               
+               632          60 LOAD_FAST                0 (self)
+                            62 LOAD_ATTR                0 (_Waveform__scope)
+                            72 LOAD_METHOD              2 (read_raw)
+                            94 PRECALL                  0
+                            98 CALL                     0
+                           108 STORE_FAST               2 (data)
+               
+               635         110 LOAD_GLOBAL              7 (NULL + WaveformData)
+                           122 LOAD_FAST                2 (data)
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 RETURN_VALUE
                consts
-                  'Get direct access to the WaveformData object.'
-               names      ('_Waveform__waveform_data',)
-               varnames   ('self',)
+                  'Read and parse data from the device.'
+                  ':WF? ALL'
+               names      ('_Waveform__scope', 'write', 'read_raw', 'WaveformData')
+               varnames   ('self', 'source', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
                name       'get_data'
-               firstlineno 596
-               lnotab 0x0202
+               firstlineno 627
+               lnotab 0x02043a013203
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'pyvisa', 'Resource', '__init__', 'Channel', 'transfer_from_device', 'WaveformData', 'get_data')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'pyvisa', 'Resource', '__init__', 'Channel', 'str', 'dump_data_to_file', 'WaveformData', 'parse_data_from_binary', 'get_data')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
          name       'Waveform'
-         firstlineno 570
-         lnotab 0x0a01040216040c13
+         firstlineno 597
+         lnotab 0x0a0104021603100c100c
       'Waveform'
-   names      ('pyvisa', 'enum', 'Enum', 'maui_rc.datatypes', 'Channel', 'struct', 'numpy', 'np', 'WaveformData', 'Waveform')
+   names      ('pyvisa', 'enum', 'Enum', 'maui_rc.datatypes', 'Channel', 'struct', 'numpy', 'np', 'pickle', 'WaveformData', 'Waveform')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/koko/SNOLAB/projects/maui_rc/maui_rc/subsystems/waveform.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c010c01080108021a7f007f007f007f0037
+   lnotab 0x00ff020108010c010c010801080108021a7f007f007f007f0051
```

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/acquisition.py` & `maui_rc-0.1.6/maui_rc/subsystems/acquisition.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/panelsetup.py` & `maui_rc-0.1.6/maui_rc/subsystems/panelsetup.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.5/maui_rc/subsystems/waveform.py` & `maui_rc-0.1.6/maui_rc/subsystems/waveform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pyvisa
 from enum import Enum
 from maui_rc.datatypes import Channel
 import struct
 import numpy as np
+import pickle
 
 class WaveformData:
     """Class which parses and contains the complete waveform data."""
 
     class RecordType(Enum):
         """The type of data of the waveform."""
 
@@ -529,70 +530,106 @@
                 data_2 = self.vertical_gain * np.array(data_2) - self.vertical_offset
 
         if len(data_2) != 0:
             self.data_y = np.array([data_1, data_2])
         else:
             self.data_y = data_1
     
-    def __init__(self, desc: bytes, text: bytes, time: bytes, dat1: bytes, dat2: bytes):
-        # It begins with parsing the description
-        # ----------
+    # def OLD__init__(self, desc: bytes, text: bytes, time: bytes, dat1: bytes, dat2: bytes):
+    #     # It begins with parsing the description
+    #     # ----------
 
         
-        # for the sake of shortening code, I'll put the blocks in a dict
-        blocks = {
-            "desc": desc,
-            "text": text,
-            "time": time,
-            "dat1": dat1,
-            "dat2": dat2,
-        }
-
-        # first, remove the query message bit and block size for each set of bytes
-        for key in blocks:
-            start_pos = blocks[key].index(b"#9")
-            blocks[key] = blocks[key][start_pos+11:]
+    #     # for the sake of shortening code, I'll put the blocks in a dict
+    #     blocks = {
+    #         "desc": desc,
+    #         "text": text,
+    #         "time": time,
+    #         "dat1": dat1,
+    #         "dat2": dat2,
+    #     }
+
+    #     # first, remove the query message bit and block size for each set of bytes
+    #     for key in blocks:
+    #         start_pos = blocks[key].index(b"#9")
+    #         blocks[key] = blocks[key][start_pos+11:]
 
-        # again for shortening the code
-        desc = blocks["desc"]
+    #     # again for shortening the code
+    #     desc = blocks["desc"]
 
-        # Parse the WAVEDESC block
-        self.__parse_wavedesc(blocks["desc"])
+    #     # Parse the WAVEDESC block
+    #     self.__parse_wavedesc(blocks["desc"])
         
-        # Parsing USERTEXT block
-        self.__parse_usertext(blocks["text"])
+    #     # Parsing USERTEXT block
+    #     self.__parse_usertext(blocks["text"])
 
-        # Parse the horizontal values
-        self.__parse_horizontal_values(blocks["time"])
+    #     # Parse the horizontal values
+    #     self.__parse_horizontal_values(blocks["time"])
+
+    #     # Parse the vertical values
+    #     self.__parse_vertical_values(blocks["dat1"].strip(), blocks["dat2"].strip())
+
+    def __init__(self, data: bytes):
+        # first, we remove the prefix 
+        start_pos = data.index(b"#9")
+        data = data[start_pos+11:]
+
+        # then we parse the description
+        self.__parse_wavedesc(data)
+
+        if self.trigtime_array_size != 0:
+            time_array_size = self.trigtime_array_size
+        elif self.ris_time_array_size != 0:
+            time_array_size = self.ris_time_array_size
+        else:
+            time_array_size = 0
+
+        # from the number of bytes know in each section, we can now split the big block of bytes into sections
+        text = data[self.wave_desc_size:(self.wave_desc_size+self.user_text_size)]
+        time = data[(self.wave_desc_size+self.user_text_size):(self.wave_desc_size+self.user_text_size+time_array_size)]
+        dat1 = data[(self.wave_desc_size+self.user_text_size+time_array_size):(self.wave_desc_size+self.user_text_size+time_array_size+self.dat1_array_size)]
+        dat2 = data[(self.wave_desc_size+self.user_text_size+time_array_size+self.dat1_array_size):(self.wave_desc_size+self.user_text_size+time_array_size+self.dat1_array_size+self.dat2_array_size)]
+
+        self.__parse_usertext(text)
+        self.__parse_horizontal_values(time)
+        self.__parse_vertical_values(dat1, dat2)
 
-        # Parse the vertical values
-        self.__parse_vertical_values(blocks["dat1"].strip(), blocks["dat2"].strip())
 
 class Waveform:
     """Class used to transfer waveform data and parse it."""
 
     def __init__(self, scope: pyvisa.Resource):
         self.__scope = scope
-        self.__waveform_data = None
 
-    def transfer_from_device(self, channel: Channel):
-        """Load the waveform data into the Waveform class. This function must be called prior to other methods."""
+    def dump_data_to_file(self, source: Channel, filepath: str):
+        """Dump the binary data from the device to a file."""
+
+        # extract the data from the device
+        self.__scope.write(f"{source}:WF? ALL")
+        data = self.__scope.read_raw()
+        # open up a file to write the data to
+        file = open(filepath, 'wb')
+        # dump the data to it
+        pickle.dump(data, file)
+        file.close()
+
+    def parse_data_from_binary(self, filepath: str) -> WaveformData:
+        """Read the binary from a file to a WaveformData object."""
+
+        # get the data from the file
+        file = open(filepath, 'rb')
+        data = pickle.load(file)
+        file.close()
+
+        # parse the data
+        return WaveformData(data)
+
+
+    def get_data(self, source: Channel) -> WaveformData:
+        """Read and parse data from the device."""
+
+        # extract the data from the device
+        self.__scope.write(f"{source}:WF? ALL")
+        data = self.__scope.read_raw()
 
-        # First, load all data blocks individually 
-        # (TODO remake the function such that all blocks can be parsed from the `ALL` data block.)
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
-        # Parse the waveform
-        self.__waveform_data = WaveformData(desc, text, time, dat1, dat2)
-
-    def get_data(self) -> WaveformData:
-        """Get direct access to the WaveformData object."""
-        return self.__waveform_data
+        # parse the data
+        return WaveformData(data)
```

### Comparing `maui_rc-0.1.5/pyproject.toml` & `maui_rc-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maui-rc"
-version = "0.1.5"
+version = "0.1.6"
 description = "Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes."
 authors = ["Kristofer Karam <karamrkristofer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maui_rc"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `maui_rc-0.1.5/PKG-INFO` & `maui_rc-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maui-rc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes.
 Author: Kristofer Karam
 Author-email: karamrkristofer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.7.0,<24.0.0)
```

