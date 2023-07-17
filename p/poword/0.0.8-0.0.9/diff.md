# Comparing `tmp/poword-0.0.8.tar.gz` & `tmp/poword-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poword-0.0.8.tar", last modified: Sun Apr  2 04:58:39 2023, max compression
+gzip compressed data, was "poword-0.0.9.tar", last modified: Sun Apr  2 14:29:37 2023, max compression
```

## Comparing `poword-0.0.8.tar` & `poword-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.536169 poword-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poword-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    10534 2023-04-02 04:58:39.537530 poword-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10006 2023-03-20 14:08:18.000000 poword-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.488851 poword-0.0.8/poword/
--rw-rw-rw-   0        0        0       31 2022-09-17 09:42:03.000000 poword-0.0.8/poword/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.523975 poword-0.0.8/poword/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.8/poword/api/__init__.py
--rw-rw-rw-   0        0        0      950 2023-04-02 04:18:47.000000 poword-0.0.8/poword/api/word.py
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.527499 poword-0.0.8/poword/core/
--rw-rw-rw-   0        0        0     3929 2023-04-02 04:40:54.000000 poword-0.0.8/poword/core/WordType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.8/poword/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.529133 poword-0.0.8/poword/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.8/poword/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.518964 poword-0.0.8/poword.egg-info/
--rw-rw-rw-   0        0        0    10534 2023-04-02 04:58:39.000000 poword-0.0.8/poword.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-02 04:58:39.000000 poword-0.0.8/poword.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 04:58:39.000000 poword-0.0.8/poword.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-01 19:03:46.000000 poword-0.0.8/poword.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-04-02 04:58:39.000000 poword-0.0.8/poword.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-02 04:58:39.000000 poword-0.0.8/poword.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-04-02 04:58:39.539551 poword-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poword-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 04:58:39.535167 poword-0.0.8/tests/
--rw-rw-rw-   0        0        0      182 2022-09-17 09:42:03.000000 poword-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      189 2023-04-01 18:57:08.000000 poword-0.0.8/tests/test_word.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:37.029149 poword-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poword-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    10533 2023-04-02 14:29:37.029149 poword-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10005 2023-04-02 05:09:26.000000 poword-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:36.961827 poword-0.0.9/poword/
+-rw-rw-rw-   0        0        0       31 2022-09-17 09:42:03.000000 poword-0.0.9/poword/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:37.003044 poword-0.0.9/poword/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.9/poword/api/__init__.py
+-rw-rw-rw-   0        0        0      950 2023-04-02 04:18:47.000000 poword-0.0.9/poword/api/word.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:37.008055 poword-0.0.9/poword/core/
+-rw-rw-rw-   0        0        0     3931 2023-04-02 14:29:18.000000 poword-0.0.9/poword/core/WordType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.9/poword/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:37.009055 poword-0.0.9/poword/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poword-0.0.9/poword/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:36.999488 poword-0.0.9/poword.egg-info/
+-rw-rw-rw-   0        0        0    10533 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-02 14:29:36.000000 poword-0.0.9/poword.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-04-02 14:29:37.031656 poword-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poword-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-02 14:29:37.026149 poword-0.0.9/tests/
+-rw-rw-rw-   0        0        0      182 2022-09-17 09:42:03.000000 poword-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      189 2023-04-01 18:57:08.000000 poword-0.0.9/tests/test_word.py
```

### Comparing `poword-0.0.8/LICENSE` & `poword-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poword-0.0.8/PKG-INFO` & `poword-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poword
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poword
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poword/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poword/blob/master/README.md
@@ -73,15 +73,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple python-office -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ python-office -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝文档
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poword Version: 0.0.8 Summary: pip install poword
+Metadata-Version: 2.1 Name: poword Version: 0.0.9 Summary: pip install poword
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poword/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poword/blob/master/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poword Platform: any Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -24,40 +24,40 @@
 FgKB-9XEG_KunLfjJbvdYw) ![](https://python-office-1300615378.cos.ap-
 chongqing.myqcloud.com/python-office-qr.jpg) ### ðºç¹ç¹ -
 ä¸é®æ­å»ºææ Python + èªå¨ååå¬çç¼ç¨ç¯å¢ã -
 ä½¿ç¨ä¸è¡ä»£ç è§£å³å¤§é¨åèªå¨ååå¬çé®é¢ï¼ä¸éè¦å°ç½å­¦ä¹ 
 Python ç¥è¯ - è´´åèåºåå¬éæ± -
 æç®ç¼ç¨ï¼å­¦ä¹ ææ¬æä½ï¼å·¥ä½æçæåæ¾è ------------------
 ------------------------------------------------------------- ## ð¦å®è£ ###
-ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
-pypi.tuna.tsinghua.edu.cn/simple python-office -U ``` -------------------------
------------------------------------------------------- ## ðææ¡£
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
-) å¨é¨åè½çè¯´æ - æå­æç¨ð[ä¼ éé¨](https://www.python-
-office.com/guide/allFunc.html) - è§é¢æç¨ð[ä¼ éé¨](https://
-www.python-office.com/video/video.html) ## ð ï¸åå«ç»ä»¶
-ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å | ä»ç» |GitHubå°å|
-star| | ----------------------|------------------------------------------------
----------------------------------- |-----|-----| | PyOfficeRobot |
-èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot |[github star]|
-| search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/search4file |
-[github star]| | poexcel | excelå¤ç |https://github.com/CoderWanFeng/poexcel
-|[github star]| | poword | wordå¤ç |https://github.com/CoderWanFeng/poword |
-[github star]| | poppt | pptå¤ç |https://github.com/CoderWanFeng/poppt |
-[github star]| | popdf | pdfå¤ç |https://github.com/CoderWanFeng/popdf |
-[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½ |https://github.com/
-CoderWanFeng/pofile |[github star]| | wftools | ä¾¿æ·å°å·¥å· |https://
-github.com/CoderWanFeng/wftools |[github star]| | poimage | å¾çå¤ç
-|https://github.com/CoderWanFeng/poimage |[github star]| | povideo |
-è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github star]| | pydatav
-| æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |[github star]| |
-potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime |[github star]| |
-webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | | emailï¼åç§°å¾å®ï¼ |
-é®ä»¶åè½ | | | | potencent | è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« |
-https://github.com/CoderWanFeng/potencent |[github star] |
+ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/
+simple/ python-office -U ``` --------------------------------------------------
+----------------------------- ## ðææ¡£ [ðå®ç½ï¼https://www.python-
+office.com/](https://www.python-office.com/) å¨é¨åè½çè¯´æ -
+æå­æç¨ð[ä¼ éé¨](https://www.python-office.com/guide/allFunc.html) -
+è§é¢æç¨ð[ä¼ éé¨](https://www.python-office.com/video/video.html) ##
+ð ï¸åå«ç»ä»¶ ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å |
+ä»ç» |GitHubå°å| star| | ----------------------|--------------------------
+-------------------------------------------------------- |-----|-----| |
+PyOfficeRobot | èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot
+|[github star]| | search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/
+search4file |[github star]| | poexcel | excelå¤ç |https://github.com/
+CoderWanFeng/poexcel |[github star]| | poword | wordå¤ç |https://github.com/
+CoderWanFeng/poword |[github star]| | poppt | pptå¤ç |https://github.com/
+CoderWanFeng/poppt |[github star]| | popdf | pdfå¤ç |https://github.com/
+CoderWanFeng/popdf |[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½
+|https://github.com/CoderWanFeng/pofile |[github star]| | wftools |
+ä¾¿æ·å°å·¥å· |https://github.com/CoderWanFeng/wftools |[github star]| |
+poimage | å¾çå¤ç |https://github.com/CoderWanFeng/poimage |[github star]|
+| povideo | è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github
+star]| | pydatav | æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |
+[github star]| | potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime
+|[github star]| | webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | |
+emailï¼åç§°å¾å®ï¼ | é®ä»¶åè½ | | | | potencent |
+è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« | https://github.com/CoderWanFeng/
+potencent |[github star] |
 å¯ä»¥æ ¹æ®éæ±å¯¹æ¯ä¸ªæ¨¡ååç¬å¼å¥ï¼ä¹å¯ä»¥éè¿`import
 office`æ¹å¼å¼å¥æææ¨¡åã --------------------------------------------
 ----------------------------------- ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
 python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼æ¾å¨ä¸ä¸ªåç¬çæä»¶å¤¹ä¸ï¼ - å¨[contributors](https://
 github.com/CoderWanFeng/python-office/tree/master/
```

### Comparing `poword-0.0.8/README.md` & `poword-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple python-office -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ python-office -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝文档
```

#### html2text {}

```diff
@@ -17,40 +17,40 @@
 FgKB-9XEG_KunLfjJbvdYw) ![](https://python-office-1300615378.cos.ap-
 chongqing.myqcloud.com/python-office-qr.jpg) ### ðºç¹ç¹ -
 ä¸é®æ­å»ºææ Python + èªå¨ååå¬çç¼ç¨ç¯å¢ã -
 ä½¿ç¨ä¸è¡ä»£ç è§£å³å¤§é¨åèªå¨ååå¬çé®é¢ï¼ä¸éè¦å°ç½å­¦ä¹ 
 Python ç¥è¯ - è´´åèåºåå¬éæ± -
 æç®ç¼ç¨ï¼å­¦ä¹ ææ¬æä½ï¼å·¥ä½æçæåæ¾è ------------------
 ------------------------------------------------------------- ## ð¦å®è£ ###
-ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
-pypi.tuna.tsinghua.edu.cn/simple python-office -U ``` -------------------------
------------------------------------------------------- ## ðææ¡£
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
-) å¨é¨åè½çè¯´æ - æå­æç¨ð[ä¼ éé¨](https://www.python-
-office.com/guide/allFunc.html) - è§é¢æç¨ð[ä¼ éé¨](https://
-www.python-office.com/video/video.html) ## ð ï¸åå«ç»ä»¶
-ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å | ä»ç» |GitHubå°å|
-star| | ----------------------|------------------------------------------------
----------------------------------- |-----|-----| | PyOfficeRobot |
-èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot |[github star]|
-| search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/search4file |
-[github star]| | poexcel | excelå¤ç |https://github.com/CoderWanFeng/poexcel
-|[github star]| | poword | wordå¤ç |https://github.com/CoderWanFeng/poword |
-[github star]| | poppt | pptå¤ç |https://github.com/CoderWanFeng/poppt |
-[github star]| | popdf | pdfå¤ç |https://github.com/CoderWanFeng/popdf |
-[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½ |https://github.com/
-CoderWanFeng/pofile |[github star]| | wftools | ä¾¿æ·å°å·¥å· |https://
-github.com/CoderWanFeng/wftools |[github star]| | poimage | å¾çå¤ç
-|https://github.com/CoderWanFeng/poimage |[github star]| | povideo |
-è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github star]| | pydatav
-| æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |[github star]| |
-potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime |[github star]| |
-webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | | emailï¼åç§°å¾å®ï¼ |
-é®ä»¶åè½ | | | | potencent | è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« |
-https://github.com/CoderWanFeng/potencent |[github star] |
+ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/
+simple/ python-office -U ``` --------------------------------------------------
+----------------------------- ## ðææ¡£ [ðå®ç½ï¼https://www.python-
+office.com/](https://www.python-office.com/) å¨é¨åè½çè¯´æ -
+æå­æç¨ð[ä¼ éé¨](https://www.python-office.com/guide/allFunc.html) -
+è§é¢æç¨ð[ä¼ éé¨](https://www.python-office.com/video/video.html) ##
+ð ï¸åå«ç»ä»¶ ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å |
+ä»ç» |GitHubå°å| star| | ----------------------|--------------------------
+-------------------------------------------------------- |-----|-----| |
+PyOfficeRobot | èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot
+|[github star]| | search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/
+search4file |[github star]| | poexcel | excelå¤ç |https://github.com/
+CoderWanFeng/poexcel |[github star]| | poword | wordå¤ç |https://github.com/
+CoderWanFeng/poword |[github star]| | poppt | pptå¤ç |https://github.com/
+CoderWanFeng/poppt |[github star]| | popdf | pdfå¤ç |https://github.com/
+CoderWanFeng/popdf |[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½
+|https://github.com/CoderWanFeng/pofile |[github star]| | wftools |
+ä¾¿æ·å°å·¥å· |https://github.com/CoderWanFeng/wftools |[github star]| |
+poimage | å¾çå¤ç |https://github.com/CoderWanFeng/poimage |[github star]|
+| povideo | è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github
+star]| | pydatav | æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |
+[github star]| | potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime
+|[github star]| | webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | |
+emailï¼åç§°å¾å®ï¼ | é®ä»¶åè½ | | | | potencent |
+è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« | https://github.com/CoderWanFeng/
+potencent |[github star] |
 å¯ä»¥æ ¹æ®éæ±å¯¹æ¯ä¸ªæ¨¡ååç¬å¼å¥ï¼ä¹å¯ä»¥éè¿`import
 office`æ¹å¼å¼å¥æææ¨¡åã --------------------------------------------
 ----------------------------------- ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
 python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼æ¾å¨ä¸ä¸ªåç¬çæä»¶å¤¹ä¸ï¼ - å¨[contributors](https://
 github.com/CoderWanFeng/python-office/tree/master/
```

### Comparing `poword-0.0.8/poword/api/word.py` & `poword-0.0.9/poword/api/word.py`

 * *Files identical despite different names*

### Comparing `poword-0.0.8/poword/core/WordType.py` & `poword-0.0.9/poword/core/WordType.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from win32com.client import constants, gencache
 from pathlib import Path
 
 
 class MainWord():
 
     def docx2pdf(self, path, output_path, docxSuffix=".docx", pdfSuffix='.pdf'):
-        waiting_covert_docx_files = get_files(path, name=docxSuffix)
+        waiting_covert_docx_files = get_files(path, suffix=docxSuffix)
         if waiting_covert_docx_files:
             print(f'一共有{len(waiting_covert_docx_files)}个docx文件')
             for i, docx_file in simple_progress(enumerate(waiting_covert_docx_files)):
                 abs_output_path = Path(output_path).absolute()
                 if not abs_output_path.exists():
                     abs_output_path.mkdir()
                 abs_single_docx_path = Path(docx_file).absolute()
```

### Comparing `poword-0.0.8/poword.egg-info/PKG-INFO` & `poword-0.0.9/poword.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poword
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poword
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poword/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poword/blob/master/README.md
@@ -73,15 +73,15 @@
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple python-office -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ python-office -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝文档
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poword Version: 0.0.8 Summary: pip install poword
+Metadata-Version: 2.1 Name: poword Version: 0.0.9 Summary: pip install poword
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poword/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poword/blob/master/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poword Platform: any Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -24,40 +24,40 @@
 FgKB-9XEG_KunLfjJbvdYw) ![](https://python-office-1300615378.cos.ap-
 chongqing.myqcloud.com/python-office-qr.jpg) ### ðºç¹ç¹ -
 ä¸é®æ­å»ºææ Python + èªå¨ååå¬çç¼ç¨ç¯å¢ã -
 ä½¿ç¨ä¸è¡ä»£ç è§£å³å¤§é¨åèªå¨ååå¬çé®é¢ï¼ä¸éè¦å°ç½å­¦ä¹ 
 Python ç¥è¯ - è´´åèåºåå¬éæ± -
 æç®ç¼ç¨ï¼å­¦ä¹ ææ¬æä½ï¼å·¥ä½æçæåæ¾è ------------------
 ------------------------------------------------------------- ## ð¦å®è£ ###
-ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
-pypi.tuna.tsinghua.edu.cn/simple python-office -U ``` -------------------------
------------------------------------------------------- ## ðææ¡£
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
-) å¨é¨åè½çè¯´æ - æå­æç¨ð[ä¼ éé¨](https://www.python-
-office.com/guide/allFunc.html) - è§é¢æç¨ð[ä¼ éé¨](https://
-www.python-office.com/video/video.html) ## ð ï¸åå«ç»ä»¶
-ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å | ä»ç» |GitHubå°å|
-star| | ----------------------|------------------------------------------------
----------------------------------- |-----|-----| | PyOfficeRobot |
-èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot |[github star]|
-| search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/search4file |
-[github star]| | poexcel | excelå¤ç |https://github.com/CoderWanFeng/poexcel
-|[github star]| | poword | wordå¤ç |https://github.com/CoderWanFeng/poword |
-[github star]| | poppt | pptå¤ç |https://github.com/CoderWanFeng/poppt |
-[github star]| | popdf | pdfå¤ç |https://github.com/CoderWanFeng/popdf |
-[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½ |https://github.com/
-CoderWanFeng/pofile |[github star]| | wftools | ä¾¿æ·å°å·¥å· |https://
-github.com/CoderWanFeng/wftools |[github star]| | poimage | å¾çå¤ç
-|https://github.com/CoderWanFeng/poimage |[github star]| | povideo |
-è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github star]| | pydatav
-| æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |[github star]| |
-potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime |[github star]| |
-webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | | emailï¼åç§°å¾å®ï¼ |
-é®ä»¶åè½ | | | | potencent | è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« |
-https://github.com/CoderWanFeng/potencent |[github star] |
+ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/
+simple/ python-office -U ``` --------------------------------------------------
+----------------------------- ## ðææ¡£ [ðå®ç½ï¼https://www.python-
+office.com/](https://www.python-office.com/) å¨é¨åè½çè¯´æ -
+æå­æç¨ð[ä¼ éé¨](https://www.python-office.com/guide/allFunc.html) -
+è§é¢æç¨ð[ä¼ éé¨](https://www.python-office.com/video/video.html) ##
+ð ï¸åå«ç»ä»¶ ä»¥ä¸ææåè½ï¼é½å¨éæ­¥æ­å»ºä¸­ã | æ¨¡å |
+ä»ç» |GitHubå°å| star| | ----------------------|--------------------------
+-------------------------------------------------------- |-----|-----| |
+PyOfficeRobot | èå¤©æºå¨äºº | https://github.com/CoderWanFeng/PyOfficeRobot
+|[github star]| | search4file | ææ¡£æç´¢ | https://github.com/CoderWanFeng/
+search4file |[github star]| | poexcel | excelå¤ç |https://github.com/
+CoderWanFeng/poexcel |[github star]| | poword | wordå¤ç |https://github.com/
+CoderWanFeng/poword |[github star]| | poppt | pptå¤ç |https://github.com/
+CoderWanFeng/poppt |[github star]| | popdf | pdfå¤ç |https://github.com/
+CoderWanFeng/popdf |[github star]| | pofile | æä»¶åæä»¶å¤¹çæä½
+|https://github.com/CoderWanFeng/pofile |[github star]| | wftools |
+ä¾¿æ·å°å·¥å· |https://github.com/CoderWanFeng/wftools |[github star]| |
+poimage | å¾çå¤ç |https://github.com/CoderWanFeng/poimage |[github star]|
+| povideo | è§é¢å¤ç |https://github.com/CoderWanFeng/povideo |[github
+star]| | pydatav | æ°æ®å¯è§å |https://github.com/CoderWanFeng/pydatav |
+[github star]| | potime | æ¶é´å·¥å· |https://github.com/CoderWanFeng/potime
+|[github star]| | webï¼åç§°å¾å®ï¼ | ç½ç«å¿«æ·æ­å»º | | | |
+emailï¼åç§°å¾å®ï¼ | é®ä»¶åè½ | | | | potencent |
+è¯å«åè½ï¼æå­è¯å«ãè¯­é³è¯å« | https://github.com/CoderWanFeng/
+potencent |[github star] |
 å¯ä»¥æ ¹æ®éæ±å¯¹æ¯ä¸ªæ¨¡ååç¬å¼å¥ï¼ä¹å¯ä»¥éè¿`import
 office`æ¹å¼å¼å¥æææ¨¡åã --------------------------------------------
 ----------------------------------- ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
 python-
 officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
 requestï¼æ¾å¨ä¸ä¸ªåç¬çæä»¶å¤¹ä¸ï¼ - å¨[contributors](https://
 github.com/CoderWanFeng/python-office/tree/master/
```

### Comparing `poword-0.0.8/setup.cfg` & `poword-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f77 6f72 640d 0a76 6572 7369   = poword..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6465 7363  on = 0.0.8..desc
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6465 7363  on = 0.0.9..desc
 00000030: 7269 7074 696f 6e20 3d20 7069 7020 696e  ription = pip in
 00000040: 7374 616c 6c20 706f 776f 7264 0d0a 6c6f  stall poword..lo
 00000050: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
 00000060: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
 00000070: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000080: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000090: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
```

