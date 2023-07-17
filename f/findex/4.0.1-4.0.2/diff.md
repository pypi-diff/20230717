# Comparing `tmp/findex-4.0.1-cp37-abi3-win_amd64.whl.zip` & `tmp/findex-4.0.2-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 1855146 bytes, number of entries: 7
--rw-r--r--  4.6 unx      462 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     6630 b- defN 23-Jun-05 10:00 cloudproof_findex/__init__.pyi
--rw-r--r--  4.6 unx       27 b- defN 23-Jun-05 10:00 cloudproof_findex/py.typed
--rw-r--r--  4.6 unx      462 b- defN 23-Jun-05 10:00 cloudproof_findex/__init__.py
--rwxr-xr-x  4.6 unx  3670528 b- defN 23-Jun-05 10:00 cloudproof_findex/cloudproof_findex.pyd
--rw-r--r--  4.6 unx      554 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/RECORD
-7 files, 3678757 bytes uncompressed, 1854168 bytes compressed:  49.6%
+Zip file size: 1932078 bytes, number of entries: 8
+-rw-r--r--  4.6 unx      533 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx    32275 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     6630 b- defN 23-Jul-17 11:22 cloudproof_findex/__init__.pyi
+-rw-r--r--  4.6 unx       27 b- defN 23-Jul-17 11:22 cloudproof_findex/py.typed
+-rw-r--r--  4.6 unx      462 b- defN 23-Jul-17 11:22 cloudproof_findex/__init__.py
+-rwxr-xr-x  4.6 unx  3817984 b- defN 23-Jul-17 11:22 cloudproof_findex/cloudproof_findex.pyd
+-rw-r--r--  4.6 unx      659 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/RECORD
+8 files, 3858664 bytes uncompressed, 1930930 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: findex-4.0.1.dist-info/METADATA
+Filename: findex-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: findex-4.0.1.dist-info/WHEEL
+Filename: findex-4.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: findex-4.0.2.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: cloudproof_findex/__init__.pyi
 Comment: 
 
 Filename: cloudproof_findex/py.typed
 Comment: 
 
 Filename: cloudproof_findex/__init__.py
 Comment: 
 
 Filename: cloudproof_findex/cloudproof_findex.pyd
 Comment: 
 
-Filename: findex-4.0.1.dist-info/RECORD
+Filename: findex-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `findex-4.0.1.dist-info/RECORD` & `findex-4.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-findex-4.0.1.dist-info/METADATA,sha256=MjRJHqowcQxUQaGUDv8dOfvZEypkg48QqtWJdsqRJqs,462
-findex-4.0.1.dist-info/WHEEL,sha256=lO8DhDEyNhXrOG0fb7degSdk7XyHtCDkr6WQEBfaH0A,94
+findex-4.0.2.dist-info/METADATA,sha256=DrszezIS4geRaBKqWYjOmAMjGsYYmkoioxIyntez6t8,533
+findex-4.0.2.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+findex-4.0.2.dist-info/license_files/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
 cloudproof_findex/__init__.pyi,sha256=s4cLBzc0_qzzX67jtRAOxuwD67t2Iwei8dsGVxDMlMw,6630
 cloudproof_findex/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
 cloudproof_findex/__init__.py,sha256=woy5cZfk_uN-PjUlPNLnr-Hy3U2u3_6YJACHQWExrMc,462
-cloudproof_findex/cloudproof_findex.pyd,sha256=RQzPF8XUCjJfUY5U38l1sn0lKGW4mEtqPlArAFM_uZo,3670528
-findex-4.0.1.dist-info/RECORD,,
+cloudproof_findex/cloudproof_findex.pyd,sha256=hrnFBpdpNhzJfd0_G1ohj4txHpxWswv57iqJ75VFtqU,3817984
+findex-4.0.2.dist-info/RECORD,,
```

