# Comparing `tmp/esupar-1.6.3-py3-none-any.whl.zip` & `tmp/esupar-1.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59177 bytes, number of entries: 12
+Zip file size: 59169 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       25 b- defN 21-Sep-17 12:30 esupar/__init__.py
 -rw-r--r--  2.0 unx     2922 b- defN 23-Feb-06 04:16 esupar/ainu.py
 -rw-r--r--  2.0 unx    10460 b- defN 23-Feb-18 01:09 esupar/esupar.py
 -rw-r--r--  2.0 unx    35949 b- defN 22-Nov-30 11:18 esupar/hangul.py
 -rw-r--r--  2.0 unx    48810 b- defN 23-Jul-17 03:11 esupar/simplify.py
--rw-r--r--  2.0 unx    19301 b- defN 23-Jul-17 03:10 esupar/tradify.py
+-rw-r--r--  2.0 unx    19286 b- defN 23-Jul-17 08:29 esupar/tradify.py
 -rw-r--r--  2.0 unx    11139 b- defN 22-Dec-30 07:29 esupar/train.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6858 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      900 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/RECORD
-12 files, 137534 bytes uncompressed, 57699 bytes compressed:  58.0%
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-17 08:31 esupar-1.6.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6858 b- defN 23-Jul-17 08:31 esupar-1.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 08:31 esupar-1.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-17 08:31 esupar-1.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      900 b- defN 23-Jul-17 08:31 esupar-1.6.4.dist-info/RECORD
+12 files, 137519 bytes uncompressed, 57691 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: esupar/tradify.py
 Comment: 
 
 Filename: esupar/train.py
 Comment: 
 
-Filename: esupar-1.6.3.dist-info/LICENSE.txt
+Filename: esupar-1.6.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: esupar-1.6.3.dist-info/METADATA
+Filename: esupar-1.6.4.dist-info/METADATA
 Comment: 
 
-Filename: esupar-1.6.3.dist-info/WHEEL
+Filename: esupar-1.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: esupar-1.6.3.dist-info/top_level.txt
+Filename: esupar-1.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: esupar-1.6.3.dist-info/RECORD
+Filename: esupar-1.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## esupar/tradify.py

```diff
@@ -77,15 +77,14 @@
   "习":"習",
   "乡":"郷",
   "书":"書",
   "买":"買",
   "乱":"亂",
   "亀":"龜",
   "争":"爭",
-  "云":"雲",
   "亚":"亞",
   "亜":"亞",
   "产":"產",
   "亩":"畝",
   "亲":"親",
   "亵":"褻",
   "亿":"億",
```

## Comparing `esupar-1.6.3.dist-info/LICENSE.txt` & `esupar-1.6.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `esupar-1.6.3.dist-info/METADATA` & `esupar-1.6.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esupar
-Version: 1.6.3
+Version: 1.6.4
 Summary: Tokenizer POS-tagger and Dependency-parser with BERT/RoBERTa/DeBERTa models for Japanese and other languages
 Home-page: https://github.com/KoichiYasuoka/esupar
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: Source, https://github.com/KoichiYasuoka/esupar
 Project-URL: Tracker, https://github.com/KoichiYasuoka/esupar/issues
```

## Comparing `esupar-1.6.3.dist-info/RECORD` & `esupar-1.6.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 esupar/__init__.py,sha256=WFHrDfbc3mwVJWPVIsRhF8RWkFX_WHFkHlyfESJg_TE,25
 esupar/ainu.py,sha256=qxfj8LtRlG9Z0TyQkyn0W9EoW-a_e3h10HwTRNqGBp8,2922
 esupar/esupar.py,sha256=2oV_tH0kGFOUEncYQuFA8QbDCgzL4AgNVaNKe05QqKs,10460
 esupar/hangul.py,sha256=kZV0_pkhTGqi1FWrLUm_oBg-6pcLEhtGVJlp5-bKC80,35949
 esupar/simplify.py,sha256=jUC67P77P-kPsJYBBf_d0XF-Vp2HGrssHOyQSXTk6EY,48810
-esupar/tradify.py,sha256=TeLFzAq7PAy1rfDApub3BorlK872NER_WRd9jiAddHI,19301
+esupar/tradify.py,sha256=oX4vRPXG7jbGhycT2G6yqaM_OzEA2ha4_Dp-OXeROFA,19286
 esupar/train.py,sha256=_MIDJ9uiEGKLWlJMoVIH_kTstylp9DY8-pKsD6HfK7w,11139
-esupar-1.6.3.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
-esupar-1.6.3.dist-info/METADATA,sha256=kwVsV9ckXVC27AZhX-sBFnqkcgJAannK_JTZ6EBwi_k,6858
-esupar-1.6.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-esupar-1.6.3.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
-esupar-1.6.3.dist-info/RECORD,,
+esupar-1.6.4.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
+esupar-1.6.4.dist-info/METADATA,sha256=DPay7PeSuNjm4T9okAq-6TGD0Ey_bzdfcgb49umZHJA,6858
+esupar-1.6.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+esupar-1.6.4.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
+esupar-1.6.4.dist-info/RECORD,,
```

