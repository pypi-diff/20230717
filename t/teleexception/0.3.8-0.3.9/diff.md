# Comparing `tmp/teleexception-0.3.8-py3-none-any.whl.zip` & `tmp/teleexception-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12562 bytes, number of entries: 10
+Zip file size: 12713 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      248 b- defN 23-Jan-29 10:59 teleexception/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-06 12:58 teleexception/status/__init__.py
--rw-rw-r--  2.0 unx    46514 b- defN 23-Feb-06 01:28 teleexception/status/http_status.py
+-rw-rw-r--  2.0 unx    47342 b- defN 23-Feb-15 07:32 teleexception/status/http_status.py
 -rw-rw-r--  2.0 unx     4361 b- defN 23-Feb-13 10:51 teleexception/status/http_status_digital_life.py
 -rw-rw-r--  2.0 unx      373 b- defN 22-Dec-06 12:58 teleexception/status/status_exception.py
 -rw-rw-r--  2.0 unx      419 b- defN 23-Jan-29 11:11 teleexception/status/status_exception_digital_life.py
--rw-rw-r--  2.0 unx     4678 b- defN 23-Feb-13 10:52 teleexception-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-13 10:52 teleexception-0.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Feb-13 10:52 teleexception-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      892 b- defN 23-Feb-13 10:52 teleexception-0.3.8.dist-info/RECORD
-10 files, 57591 bytes uncompressed, 11010 bytes compressed:  80.9%
+-rw-rw-r--  2.0 unx     4678 b- defN 23-Feb-15 07:33 teleexception-0.3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Feb-15 07:33 teleexception-0.3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Feb-15 07:33 teleexception-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      892 b- defN 23-Feb-15 07:33 teleexception-0.3.9.dist-info/RECORD
+10 files, 58419 bytes uncompressed, 11161 bytes compressed:  80.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: teleexception/status/status_exception.py
 Comment: 
 
 Filename: teleexception/status/status_exception_digital_life.py
 Comment: 
 
-Filename: teleexception-0.3.8.dist-info/METADATA
+Filename: teleexception-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: teleexception-0.3.8.dist-info/WHEEL
+Filename: teleexception-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: teleexception-0.3.8.dist-info/top_level.txt
+Filename: teleexception-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: teleexception-0.3.8.dist-info/RECORD
+Filename: teleexception-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teleexception/status/http_status.py

```diff
@@ -81,14 +81,16 @@
     VERSION_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Version）未传")
 
     MAKEUP_TYPE_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（MakeupType）未传") # 人脸美妆
     SUBTASK_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（SubTask）未传") # 内容审核
     SUBEVENT_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（SubEvent）未传") # 内容审核
     TASKID_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（TaskId）未传") # 内容审核
     SIGNAL_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Signal）未传") # 实时语音识别
+    ROI_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Roi）未传") # 电子围栏
+    
     DBNAME_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（DbName）未传") # 数据库
     ENTITY_ID_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（EntityId）未传") # 数据库
     LABELS_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Labels）未传") # 数据库
     OFFSET_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Offset）未传") # 数据库
     EXTRA_DATA_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（ExtraData）未传") # 数据库
     LIMIT_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（Limit）未传") # 数据库
     FACE_ID_MUST_PRAM_ERR = (400006, "必传的参数未传", "必须的参数（FaceId）未传") # 数据库
@@ -132,15 +134,16 @@
     SMOKE_LEVEL_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Level 字段应该是 int 类型")  # 吸烟检测
     MAKEUP_TYPE_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "MakeupType 字段应该是 int 类型")  # 人脸美妆
     MAX_FACE_NUM_TYPE_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "MaxFaceNum 字段应该是 int 类型")  # 人脸检测
     MIN_FACE_SIZE_TYPE_ERR = (400008, "请求体的参数字段类型错误", "MinFaceSize 字段应该是 int 类型")  # 人脸检测
     FREQUENCY_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Frequency 字段应该是 int 类型")  # 视频内容审核
     OFFSET_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Offset 字段应该是 int 类型") # 数据库
     LIMIT_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Limit 字段应该是 int 类型") # 数据库
-
+    ROI_ITEM_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Roi 字段中的两点坐标应该是 int 类型")  # 电子围栏
+    
     PITCH_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Pitch 字段应该是 float 类型")  # 语音合成
     SPEED_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Speed 字段应该是 float 类型")  # 语音合成
     VOLUME_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Volume 字段应该是 float 类型")  # 语音合成
     SCORE_THRESH_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "ScoreThresh 字段应该是 float 类型")  # 通用分数阈值
     PERSON_THRESH_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "PersonThresh 字段应该是 float 类型")  # 行人检测
     FACE_THRESH_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "FaceThresh 字段应该是 float 类型")  # 人脸检测
     FIRE_THRESH_FLOAT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "FireThresh 字段应该是 float 类型")  # 烟雾明火检测
@@ -198,16 +201,17 @@
     EXTRA_DATA_STRING_TYPE_ERR = (400008, "请求体的参数字段类型错误", "ExtraData 字段应该是 string 类型") # 数据库
     FACE_ID_STRING_TYPE_ERR = (400008, "请求体的参数字段类型错误", "FaceId 字段应该是 string 类型") # 数据库
     FACE_ID_INT_TYPE_ERR = (400008, "请求体的参数字段类型错误", "FaceId 字段应该是 int 类型") # 数据库
 
     INPUTS_LIST_TYPE_ERR = (400008, "请求体的参数字段类型错误", "inputs 字段应该是 list 类型") # 内容审核
     IMG_CENSOR_SUBTASK_LIST_TYPE_ERR = (400008, "请求体的参数字段类型错误", "SubTask 字段应该是 list 类型")  # 内容审核
     SUBEVENT_LIST_TYPE_ERR = (400008, "请求体的参数字段类型错误", "SubEvent 字段应该是 list 类型")  # 内容审核
-    
+    ROI_LIST_TYPE_ERR = (400008, "请求体的参数字段类型错误", "Roi 字段应该是 list 类型")  # 电子围栏
 
+    
     # 400009 请求体的参数字段值为空
     IMAGE_DATA_AND_ACTION_EMPTY_ERR = (400009, "请求体的参数字段值为空", "Action、ImageData 字段值为空字符")
     IMAGE_DATA_EMPTY_ERR = (400009, "请求体的参数字段值为空", "ImageData 字段值为空字符")
     IMAGE_DATA_LIST_EMPTY_ERR = (400009, "请求体的参数字段值为空", "ImageData 列表为空")
     IMAGE_AB_DATA_EMPTY_ERR = (400009, "请求体的参数字段值为空", "ImageDataA、ImageDataB 字段值为空字符")
     TEXT_DATA_EMPTY_ERR = (400009, "请求体的参数字段值为空", "TextData 字段值为空字符")
     AUDIO_DATA_EMPTY_ERR = (400009, "请求体的参数字段值为空", "AudioData 字段值为空字符")
@@ -234,14 +238,15 @@
     ENTITY_ID_EMPTY_ERR = (400009, "请求体的参数字段值为空", "EntityId 字段值为空字符") # 数据库
     LABELS_EMPTY_ERR = (400009, "请求体的参数字段值为空", "Labels 字段值为空字符") # 数据库
     EXTRA_DATA_EMPTY_ERR = (400009, "请求体的参数字段值为空", "ExtraData 字段值为空字符") # 数据库
     FACE_ID_EMPTY_ERR = (400009, "请求体的参数字段值为空", "FaceId 字段值为空字符") # 数据库
     
     IMG_CENSOR_SUBTASK_EMPTY_ERR = (400009, "请求体的参数字段值为空", "SubTask 列表为空") # 内容审核
     SUBEVENT_EMPTY_ERR = (400009, "请求体的参数字段值为空", "SubEvent 列表为空") # 内容审核
+    ROI_EMPTY_ERR = (400009, "请求体的参数字段值为空", "Roi 列表为空") # 电子围栏
 
 
     # 400010 请求体的参数字段值设置错误
     ACTION_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "Action 值设置错误")  # ACTION
     IMAGE_DATA_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "ImageData 字段不符合规范，请参考接口文档说明")
     TEXT_DATA_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "TextData 字段不符合规范，请参考接口文档说明")
     AUDIO_DATA_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "AudioData 字段不符合规范，请参考接口文档说明")
@@ -267,14 +272,15 @@
     IMG_CENSOR_SUBTASK_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "SubTask 字段不符合规范，请参考接口文档说明")  # 内容审核
     SUBEVENT_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "SubEvent 字段不符合规范，请参考接口文档说明")  # 视频内容审核
     FREQUENCY_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "Frequency 字段不符合规范，请参考接口文档说明")  # 视频内容审核
     LANGUAGE_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "Language 字段不符合规范，请参考接口文档说明")  # 语音识别
     IS_MONOLINGUAL_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "IsMonolingual 字段不符合规范，请参考接口文档说明")  # 语种分类
     MAX_FACE_NUM_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "MaxFaceNum 字段不符合规范，请参考接口文档说明")  # 人脸检测
     MIN_FACE_SIZE_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "MinFaceSize 字段不符合规范，请参考接口文档说明")  # 人脸检测
+    ROI_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "Roi 字段不符合规范，请参考接口文档说明")  # 电子围栏
 
     SCORE_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "ScoreThresh 字段不符合规范，请参考接口文档说明")  # 通用分数阈值
     PERSON_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "PersonThresh 字段不符合规范，请参考接口文档说明")  # 行人检测
     FACE_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "FaceThresh 字段不符合规范，请参考接口文档说明")  # 人脸检测
     FIRE_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "FireThresh 字段不符合规范，请参考接口文档说明")  # 烟雾明火检测
     SMOKE_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "SmokeThresh 字段不符合规范，请参考接口文档说明")  # 烟雾明火检测
     CAR_THRESH_VALUE_ERR = (400010, "请求体的参数字段值设置错误", "CarThresh 字段不符合规范，请参考接口文档说明")  # 车辆检测
@@ -388,15 +394,18 @@
 
     AUDIO_DATA_OVER_LIMIT_DOC_ERR = (400018, "超过个数限制", "AudioData 超过个数限制，请参考接口文档说明")
     AUDIO_URL_OVER_LIMIT_DOC_ERR = (400018, "超过个数限制", "AudioURL 超过个数限制，请参考接口文档说明")
 
     VIDEO_DATA_OVER_LIMIT_DOC_ERR = (400018, "超过个数限制", "VideoData 超过个数限制，请参考接口文档说明")
     VIDEO_URL_OVER_LIMIT_DOC_ERR = (400018, "超过个数限制", "VideoURL 超过个数限制，请参考接口文档说明")
 
-
+    
+    # 4000019 请求体的参数字段长度错误
+    ROI_LENGTH_ERR = (400019, "请求体的参数字段长度错误", "Roi 字段长度必须大于 3 或者小于 10") # 电子围栏
+    
 
     ### 图片 41xxxxx ###
 
     # 410001 图片解码错误
     IMAGE_DECODE_ERR = (410001, "图片解码错误", "字节码解码为图片错误")
 
     # 410002 图片尺寸不符合要求
```

## Comparing `teleexception-0.3.8.dist-info/METADATA` & `teleexception-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teleexception
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python Package for tele exception
 Home-page: UNKNOWN
 Author: imason
 Author-email: 635761952@qq.com
 License: UNKNOWN
 Keywords: python exception
 Platform: UNKNOWN
```

## Comparing `teleexception-0.3.8.dist-info/RECORD` & `teleexception-0.3.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 teleexception/__init__.py,sha256=ZCJikkZXg9y6NWKrRPJFOipnuhuLP4ue45YM3zcvldI,248
 teleexception/status/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-teleexception/status/http_status.py,sha256=suZl9NSstWc-CclEtSq0yBJ1Po1Gaj-l8MIZEQ24Cxk,46514
+teleexception/status/http_status.py,sha256=VAXViSeyZ5QIx8hoN_ZpIXJfl0uoWgbM8x5X9ATbiHo,47342
 teleexception/status/http_status_digital_life.py,sha256=mscC8D5igKw5LXCBlSYYj_E-ZF625xQzqTTXghRzPco,4361
 teleexception/status/status_exception.py,sha256=c8Hn-TIuPn5wMydVaSeaESalv14XjtLOD38m2-gSpR0,373
 teleexception/status/status_exception_digital_life.py,sha256=ClbhY_3a9EY5jWjxEsV9JBhR90wBgsLMoj591KGwH2A,419
-teleexception-0.3.8.dist-info/METADATA,sha256=bBMx_qDQReCt-0ytRY1ultcnMHuFO2Nb7UcToFYOxfw,4678
-teleexception-0.3.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-teleexception-0.3.8.dist-info/top_level.txt,sha256=8UE4OrNUAjQojJfld8TkzSD2RaYtO4XlXHzQIGBrTXU,14
-teleexception-0.3.8.dist-info/RECORD,,
+teleexception-0.3.9.dist-info/METADATA,sha256=zH3EpUhkMk3cLzxm_MZqqCi6IFZp8K9gXG2Ft3-mJco,4678
+teleexception-0.3.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+teleexception-0.3.9.dist-info/top_level.txt,sha256=8UE4OrNUAjQojJfld8TkzSD2RaYtO4XlXHzQIGBrTXU,14
+teleexception-0.3.9.dist-info/RECORD,,
```

