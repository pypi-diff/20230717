# Comparing `tmp/esupar-1.6.2-py3-none-any.whl.zip` & `tmp/esupar-1.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59152 bytes, number of entries: 12
+Zip file size: 59177 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       25 b- defN 21-Sep-17 12:30 esupar/__init__.py
 -rw-r--r--  2.0 unx     2922 b- defN 23-Feb-06 04:16 esupar/ainu.py
 -rw-r--r--  2.0 unx    10460 b- defN 23-Feb-18 01:09 esupar/esupar.py
 -rw-r--r--  2.0 unx    35949 b- defN 22-Nov-30 11:18 esupar/hangul.py
--rw-r--r--  2.0 unx    48779 b- defN 21-Aug-17 14:50 esupar/simplify.py
--rw-r--r--  2.0 unx    19270 b- defN 22-Dec-30 03:01 esupar/tradify.py
+-rw-r--r--  2.0 unx    48810 b- defN 23-Jul-17 03:11 esupar/simplify.py
+-rw-r--r--  2.0 unx    19301 b- defN 23-Jul-17 03:10 esupar/tradify.py
 -rw-r--r--  2.0 unx    11139 b- defN 22-Dec-30 07:29 esupar/train.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Feb-18 01:14 esupar-1.6.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6858 b- defN 23-Feb-18 01:14 esupar-1.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-18 01:14 esupar-1.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-18 01:14 esupar-1.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      900 b- defN 23-Feb-18 01:14 esupar-1.6.2.dist-info/RECORD
-12 files, 137472 bytes uncompressed, 57674 bytes compressed:  58.0%
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6858 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      900 b- defN 23-Jul-17 03:14 esupar-1.6.3.dist-info/RECORD
+12 files, 137534 bytes uncompressed, 57699 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: esupar/tradify.py
 Comment: 
 
 Filename: esupar/train.py
 Comment: 
 
-Filename: esupar-1.6.2.dist-info/LICENSE.txt
+Filename: esupar-1.6.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: esupar-1.6.2.dist-info/METADATA
+Filename: esupar-1.6.3.dist-info/METADATA
 Comment: 
 
-Filename: esupar-1.6.2.dist-info/WHEEL
+Filename: esupar-1.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: esupar-1.6.2.dist-info/top_level.txt
+Filename: esupar-1.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: esupar-1.6.2.dist-info/RECORD
+Filename: esupar-1.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## esupar/simplify.py

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/python3 -i
 # coding=utf-8
 simplify={
   "𧦧":"𫍟",
   "𨬟":"𰾵",
   "𡑍":"𫭼",
   "𥳁":"𥲤",
+  "𠕋":"册",
   "𡐨":"壄",
   "𣙜":"榷",
   "㑳":"㑇",
   "㑹":"会",
   "㘚":"㘎",
   "㠣":"𫵷",
   "㥮":"㤘",
@@ -117,14 +118,15 @@
   "兎":"兔",
   "児":"儿",
   "兒":"儿",
   "兗":"兖",
   "內":"内",
   "兩":"两",
   "円":"园",
+  "冊":"册",
   "冑":"胄",
   "凍":"冻",
   "処":"处",
   "凱":"凯",
   "別":"别",
   "刦":"劫",
   "刪":"删",
```

## esupar/tradify.py

```diff
@@ -1,16 +1,12 @@
 #! /usr/bin/python3 -i
 # coding=utf-8
 tradify={
-  "锯":"鋸",
-  "块":"塊",
-  "闹":"鬧",
-  "纽":"紐",
-  "订":"訂",
   "𫍟":"𧦧",
+  "𠕋":"冊",
   "𫮃":"墠",
   "𪪼":"彃",
   "𢭏":"擣",
   "𥐟":"礒",
   "𬘝":"紾",
   "𫄨":"絺",
   "𮉪":"緅",
@@ -138,14 +134,15 @@
   "关":"關",
   "兴":"興",
   "兹":"茲",
   "养":"養",
   "兽":"獸",
   "内":"內",
   "円":"園",
+  "册":"冊",
   "写":"寫",
   "军":"軍",
   "农":"農",
   "冯":"馮",
   "决":"決",
   "况":"況",
   "冻":"凍",
@@ -243,14 +240,15 @@
   "国":"國",
   "图":"圖",
   "圆":"圓",
   "圣":"聖",
   "圹":"壙",
   "场":"場",
   "坏":"壞",
+  "块":"塊",
   "坚":"堅",
   "坠":"墜",
   "垫":"墊",
   "埀":"垂",
   "堕":"墮",
   "塩":"鹽",
   "填":"塡",
@@ -708,14 +706,15 @@
   "纲":"綱",
   "纳":"納",
   "纵":"縱",
   "纶":"綸",
   "纷":"紛",
   "纸":"紙",
   "纺":"紡",
+  "纽":"紐",
   "线":"綫",
   "绀":"紺",
   "练":"練",
   "组":"組",
   "绅":"紳",
   "细":"細",
   "织":"織",
@@ -867,14 +866,15 @@
   "読":"讀",
   "諸":"諸",
   "謁":"謁",
   "謹":"謹",
   "譲":"讓",
   "讐":"讎",
   "计":"計",
+  "订":"訂",
   "认":"認",
   "讥":"譏",
   "讦":"訐",
   "讨":"討",
   "让":"讓",
   "讪":"訕",
   "训":"訓",
@@ -1088,14 +1088,15 @@
   "锁":"鎖",
   "锐":"銳",
   "错":"錯",
   "锜":"錡",
   "锡":"錫",
   "锦":"錦",
   "锭":"錠",
+  "锯":"鋸",
   "锸":"鍤",
   "镂":"鏤",
   "镃":"鎡",
   "镇":"鎭",
   "镒":"鎰",
   "镜":"鏡",
   "镦":"鐓",
@@ -1106,14 +1107,15 @@
   "闘":"鬭",
   "门":"門",
   "闭":"閉",
   "问":"問",
   "闲":"閑",
   "间":"間",
   "闵":"閔",
+  "闹":"鬧",
   "闺":"閨",
   "闻":"聞",
   "阁":"閣",
   "阅":"閱",
   "阈":"閾",
   "阉":"閹",
   "阐":"闡",
```

## Comparing `esupar-1.6.2.dist-info/LICENSE.txt` & `esupar-1.6.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `esupar-1.6.2.dist-info/METADATA` & `esupar-1.6.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esupar
-Version: 1.6.2
+Version: 1.6.3
 Summary: Tokenizer POS-tagger and Dependency-parser with BERT/RoBERTa/DeBERTa models for Japanese and other languages
 Home-page: https://github.com/KoichiYasuoka/esupar
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: Source, https://github.com/KoichiYasuoka/esupar
 Project-URL: Tracker, https://github.com/KoichiYasuoka/esupar/issues
```

## Comparing `esupar-1.6.2.dist-info/RECORD` & `esupar-1.6.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 esupar/__init__.py,sha256=WFHrDfbc3mwVJWPVIsRhF8RWkFX_WHFkHlyfESJg_TE,25
 esupar/ainu.py,sha256=qxfj8LtRlG9Z0TyQkyn0W9EoW-a_e3h10HwTRNqGBp8,2922
 esupar/esupar.py,sha256=2oV_tH0kGFOUEncYQuFA8QbDCgzL4AgNVaNKe05QqKs,10460
 esupar/hangul.py,sha256=kZV0_pkhTGqi1FWrLUm_oBg-6pcLEhtGVJlp5-bKC80,35949
-esupar/simplify.py,sha256=Z0WBiuYpRByr-mbHcdQLlkC7HJ8aNHK0K872FghIDOM,48779
-esupar/tradify.py,sha256=H_-qVa0Bk_Sg9Txihh_dZXYbvKKKsrpG-V8bEwoIbTg,19270
+esupar/simplify.py,sha256=jUC67P77P-kPsJYBBf_d0XF-Vp2HGrssHOyQSXTk6EY,48810
+esupar/tradify.py,sha256=TeLFzAq7PAy1rfDApub3BorlK872NER_WRd9jiAddHI,19301
 esupar/train.py,sha256=_MIDJ9uiEGKLWlJMoVIH_kTstylp9DY8-pKsD6HfK7w,11139
-esupar-1.6.2.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
-esupar-1.6.2.dist-info/METADATA,sha256=Hw3TN-JlkQhsMN6qaYYIPV30C2i7DOOffD7V9c9Se4Y,6858
-esupar-1.6.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-esupar-1.6.2.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
-esupar-1.6.2.dist-info/RECORD,,
+esupar-1.6.3.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
+esupar-1.6.3.dist-info/METADATA,sha256=kwVsV9ckXVC27AZhX-sBFnqkcgJAannK_JTZ6EBwi_k,6858
+esupar-1.6.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+esupar-1.6.3.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
+esupar-1.6.3.dist-info/RECORD,,
```

