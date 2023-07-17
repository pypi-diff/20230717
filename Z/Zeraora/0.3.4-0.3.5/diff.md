# Comparing `tmp/Zeraora-0.3.4.tar.gz` & `tmp/Zeraora-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.3.4.tar", last modified: Fri Jul  7 15:23:38 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.3.5.tar", last modified: Mon Jul 17 05:57:42 2023, max compression
```

## Comparing `Zeraora-0.3.4.tar` & `Zeraora-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 15:23:38.000000 Zeraora-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-07 15:23:24.000000 Zeraora-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:23:38.000000 Zeraora-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 15:23:24.000000 Zeraora-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/click/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/click/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/dj/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/drf/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/gvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/throwables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-17 05:57:42.000000 Zeraora-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-17 05:57:31.000000 Zeraora-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-17 05:57:42.000000 Zeraora-0.3.5/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-17 05:57:42.000000 Zeraora-0.3.5/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:57:42.000000 Zeraora-0.3.5/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 05:57:42.000000 Zeraora-0.3.5/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 05:57:42.000000 Zeraora-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 05:57:31.000000 Zeraora-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/zeraora/click/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/click/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/zeraora/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/constants/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/constants/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/constants/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/zeraora/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/dj/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/dj/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/dj/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:57:42.000000 Zeraora-0.3.5/zeraora/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/drf/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/gvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/throwables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-17 05:57:31.000000 Zeraora-0.3.5/zeraora/utils.py
```

### Comparing `Zeraora-0.3.4/PKG-INFO` & `Zeraora-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.4
+Version: 0.3.5
 Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -65,18 +65,18 @@
         |       | 状态      | 维护结束时间 | 首版时间   | 安全版本 | 分支  | 依赖 |
         | ----- | --------- | ------------ | ---------- | -------- | ----- | ---- |
         | 0.3.x | 🆕feature  | ~ 0.5.x      | 2023.06.09 | -        | main  | 3.7+ |
         | 0.2.x | ✅security | ~ 0.4.x      | 2023.04.12 | 0.2.14   | 0.2.x | 3.7+ |
         | 0.1.x | ❌EOL      | 2023.06.09   | 2023.03.27 | -        | 0.1.x | 3.7+ |
         
         - 状态
-          - feature 指功能还在开发或测试，回退子版本可能会出现兼容性问题。
+          - feature 指还在新增功能或测试，当前版本可能会有问题，或回退子版本可能会出现兼容性问题。
           - security 指功能已经稳定，回退不会出现兼容性问题；会为问题修复发布新的子版本，但不会迁移新版功能。
           - EOL 指已经停止维护，不会处理与之相关的任何问题，也不会发布新的子版本。
-          - 没有 prerelease 状态，因为这个状态通常不会发布包，进而难以测试。
+          - 没有 prerelease 状态，因为人少管理不了那么多。
         
         - 维护结束时间
           - 一般是到下下一个版本的安全版本发布为止。
         
         - 安全版本
           - 指的是 security 状态开始的那一个版本，这个版本往后的那些版本可以安全回退。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.4 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.5 Summary:
 ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
@@ -34,21 +34,20 @@
 pypi.mirrors.ustc.edu.cn/simple/ ``` å ä¸ºæ²¡æéæ±ï¼æä»¥è¿æ²¡æåå»º
 conda çæ¬ã ## çæ¬ | | ç¶æ | ç»´æ¤ç»ææ¶é´ | é¦çæ¶é´ |
 å®å¨çæ¬ | åæ¯ | ä¾èµ | | ----- | --------- | ------------ | ---------
 - | -------- | ----- | ---- | | 0.3.x | ðfeature | ~ 0.5.x | 2023.06.09 | -
 | main | 3.7+ | | 0.2.x | âsecurity | ~ 0.4.x | 2023.04.12 | 0.2.14 | 0.2.x |
 3.7+ | | 0.1.x | âEOL | 2023.06.09 | 2023.03.27 | - | 0.1.x | 3.7+ | - ç¶æ
 - feature
-æåè½è¿å¨å¼åææµè¯ï¼åéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
+æè¿å¨æ°å¢åè½ææµè¯ï¼å½åçæ¬å¯è½ä¼æé®é¢ï¼æåéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
 - security
 æåè½å·²ç»ç¨³å®ï¼åéä¸ä¼åºç°å¼å®¹æ§é®é¢ï¼ä¼ä¸ºé®é¢ä¿®å¤åå¸æ°çå­çæ¬ï¼ä½ä¸ä¼è¿ç§»æ°çåè½ã
 - EOL
 æå·²ç»åæ­¢ç»´æ¤ï¼ä¸ä¼å¤çä¸ä¹ç¸å³çä»»ä½é®é¢ï¼ä¹ä¸ä¼åå¸æ°çå­çæ¬ã
-- æ²¡æ prerelease
-ç¶æï¼å ä¸ºè¿ä¸ªç¶æéå¸¸ä¸ä¼åå¸åï¼è¿èé¾ä»¥æµè¯ã -
+- æ²¡æ prerelease ç¶æï¼å ä¸ºäººå°ç®¡çä¸äºé£ä¹å¤ã -
 ç»´æ¤ç»ææ¶é´ -
 ä¸è¬æ¯å°ä¸ä¸ä¸ä¸ªçæ¬çå®å¨çæ¬åå¸ä¸ºæ­¢ã - å®å¨çæ¬ -
 æçæ¯ security
 ç¶æå¼å§çé£ä¸ä¸ªçæ¬ï¼è¿ä¸ªçæ¬å¾åçé£äºçæ¬å¯ä»¥å®å¨åéã
 - ä¾èµ - å¯¹äº Python çæ¬çä¾èµï¼ä¾å¦ 3.7+ æçæ¯éè¦ 3.7
 ææ´æ°ç Pythonã ## ææ¡£ è¯¦è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
 README.md)ã ## å¼å
```

### Comparing `Zeraora-0.3.4/README.md` & `Zeraora-0.3.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -55,18 +55,18 @@
 |       | 状态      | 维护结束时间 | 首版时间   | 安全版本 | 分支  | 依赖 |
 | ----- | --------- | ------------ | ---------- | -------- | ----- | ---- |
 | 0.3.x | 🆕feature  | ~ 0.5.x      | 2023.06.09 | -        | main  | 3.7+ |
 | 0.2.x | ✅security | ~ 0.4.x      | 2023.04.12 | 0.2.14   | 0.2.x | 3.7+ |
 | 0.1.x | ❌EOL      | 2023.06.09   | 2023.03.27 | -        | 0.1.x | 3.7+ |
 
 - 状态
-  - feature 指功能还在开发或测试，回退子版本可能会出现兼容性问题。
+  - feature 指还在新增功能或测试，当前版本可能会有问题，或回退子版本可能会出现兼容性问题。
   - security 指功能已经稳定，回退不会出现兼容性问题；会为问题修复发布新的子版本，但不会迁移新版功能。
   - EOL 指已经停止维护，不会处理与之相关的任何问题，也不会发布新的子版本。
-  - 没有 prerelease 状态，因为这个状态通常不会发布包，进而难以测试。
+  - 没有 prerelease 状态，因为人少管理不了那么多。
 
 - 维护结束时间
   - 一般是到下下一个版本的安全版本发布为止。
 
 - 安全版本
   - 指的是 security 状态开始的那一个版本，这个版本往后的那些版本可以安全回退。
```

#### html2text {}

```diff
@@ -27,21 +27,20 @@
 pypi.mirrors.ustc.edu.cn/simple/ ``` å ä¸ºæ²¡æéæ±ï¼æä»¥è¿æ²¡æåå»º
 conda çæ¬ã ## çæ¬ | | ç¶æ | ç»´æ¤ç»ææ¶é´ | é¦çæ¶é´ |
 å®å¨çæ¬ | åæ¯ | ä¾èµ | | ----- | --------- | ------------ | ---------
 - | -------- | ----- | ---- | | 0.3.x | ðfeature | ~ 0.5.x | 2023.06.09 | -
 | main | 3.7+ | | 0.2.x | âsecurity | ~ 0.4.x | 2023.04.12 | 0.2.14 | 0.2.x |
 3.7+ | | 0.1.x | âEOL | 2023.06.09 | 2023.03.27 | - | 0.1.x | 3.7+ | - ç¶æ
 - feature
-æåè½è¿å¨å¼åææµè¯ï¼åéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
+æè¿å¨æ°å¢åè½ææµè¯ï¼å½åçæ¬å¯è½ä¼æé®é¢ï¼æåéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
 - security
 æåè½å·²ç»ç¨³å®ï¼åéä¸ä¼åºç°å¼å®¹æ§é®é¢ï¼ä¼ä¸ºé®é¢ä¿®å¤åå¸æ°çå­çæ¬ï¼ä½ä¸ä¼è¿ç§»æ°çåè½ã
 - EOL
 æå·²ç»åæ­¢ç»´æ¤ï¼ä¸ä¼å¤çä¸ä¹ç¸å³çä»»ä½é®é¢ï¼ä¹ä¸ä¼åå¸æ°çå­çæ¬ã
-- æ²¡æ prerelease
-ç¶æï¼å ä¸ºè¿ä¸ªç¶æéå¸¸ä¸ä¼åå¸åï¼è¿èé¾ä»¥æµè¯ã -
+- æ²¡æ prerelease ç¶æï¼å ä¸ºäººå°ç®¡çä¸äºé£ä¹å¤ã -
 ç»´æ¤ç»ææ¶é´ -
 ä¸è¬æ¯å°ä¸ä¸ä¸ä¸ªçæ¬çå®å¨çæ¬åå¸ä¸ºæ­¢ã - å®å¨çæ¬ -
 æçæ¯ security
 ç¶æå¼å§çé£ä¸ä¸ªçæ¬ï¼è¿ä¸ªçæ¬å¾åçé£äºçæ¬å¯ä»¥å®å¨åéã
 - ä¾èµ - å¯¹äº Python çæ¬çä¾èµï¼ä¾å¦ 3.7+ æçæ¯éè¦ 3.7
 ææ´æ°ç Pythonã ## ææ¡£ è¯¦è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
 README.md)ã ## å¼å
```

### Comparing `Zeraora-0.3.4/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.3.5/Zeraora.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.4
+Version: 0.3.5
 Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -65,18 +65,18 @@
         |       | 状态      | 维护结束时间 | 首版时间   | 安全版本 | 分支  | 依赖 |
         | ----- | --------- | ------------ | ---------- | -------- | ----- | ---- |
         | 0.3.x | 🆕feature  | ~ 0.5.x      | 2023.06.09 | -        | main  | 3.7+ |
         | 0.2.x | ✅security | ~ 0.4.x      | 2023.04.12 | 0.2.14   | 0.2.x | 3.7+ |
         | 0.1.x | ❌EOL      | 2023.06.09   | 2023.03.27 | -        | 0.1.x | 3.7+ |
         
         - 状态
-          - feature 指功能还在开发或测试，回退子版本可能会出现兼容性问题。
+          - feature 指还在新增功能或测试，当前版本可能会有问题，或回退子版本可能会出现兼容性问题。
           - security 指功能已经稳定，回退不会出现兼容性问题；会为问题修复发布新的子版本，但不会迁移新版功能。
           - EOL 指已经停止维护，不会处理与之相关的任何问题，也不会发布新的子版本。
-          - 没有 prerelease 状态，因为这个状态通常不会发布包，进而难以测试。
+          - 没有 prerelease 状态，因为人少管理不了那么多。
         
         - 维护结束时间
           - 一般是到下下一个版本的安全版本发布为止。
         
         - 安全版本
           - 指的是 security 状态开始的那一个版本，这个版本往后的那些版本可以安全回退。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.4 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.5 Summary:
 ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
@@ -34,21 +34,20 @@
 pypi.mirrors.ustc.edu.cn/simple/ ``` å ä¸ºæ²¡æéæ±ï¼æä»¥è¿æ²¡æåå»º
 conda çæ¬ã ## çæ¬ | | ç¶æ | ç»´æ¤ç»ææ¶é´ | é¦çæ¶é´ |
 å®å¨çæ¬ | åæ¯ | ä¾èµ | | ----- | --------- | ------------ | ---------
 - | -------- | ----- | ---- | | 0.3.x | ðfeature | ~ 0.5.x | 2023.06.09 | -
 | main | 3.7+ | | 0.2.x | âsecurity | ~ 0.4.x | 2023.04.12 | 0.2.14 | 0.2.x |
 3.7+ | | 0.1.x | âEOL | 2023.06.09 | 2023.03.27 | - | 0.1.x | 3.7+ | - ç¶æ
 - feature
-æåè½è¿å¨å¼åææµè¯ï¼åéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
+æè¿å¨æ°å¢åè½ææµè¯ï¼å½åçæ¬å¯è½ä¼æé®é¢ï¼æåéå­çæ¬å¯è½ä¼åºç°å¼å®¹æ§é®é¢ã
 - security
 æåè½å·²ç»ç¨³å®ï¼åéä¸ä¼åºç°å¼å®¹æ§é®é¢ï¼ä¼ä¸ºé®é¢ä¿®å¤åå¸æ°çå­çæ¬ï¼ä½ä¸ä¼è¿ç§»æ°çåè½ã
 - EOL
 æå·²ç»åæ­¢ç»´æ¤ï¼ä¸ä¼å¤çä¸ä¹ç¸å³çä»»ä½é®é¢ï¼ä¹ä¸ä¼åå¸æ°çå­çæ¬ã
-- æ²¡æ prerelease
-ç¶æï¼å ä¸ºè¿ä¸ªç¶æéå¸¸ä¸ä¼åå¸åï¼è¿èé¾ä»¥æµè¯ã -
+- æ²¡æ prerelease ç¶æï¼å ä¸ºäººå°ç®¡çä¸äºé£ä¹å¤ã -
 ç»´æ¤ç»ææ¶é´ -
 ä¸è¬æ¯å°ä¸ä¸ä¸ä¸ªçæ¬çå®å¨çæ¬åå¸ä¸ºæ­¢ã - å®å¨çæ¬ -
 æçæ¯ security
 ç¶æå¼å§çé£ä¸ä¸ªçæ¬ï¼è¿ä¸ªçæ¬å¾åçé£äºçæ¬å¯ä»¥å®å¨åéã
 - ä¾èµ - å¯¹äº Python çæ¬çä¾èµï¼ä¾å¦ 3.7+ æçæ¯éè¦ 3.7
 ææ´æ°ç Pythonã ## ææ¡£ è¯¦è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
 README.md)ã ## å¼å
```

### Comparing `Zeraora-0.3.4/Zeraora.egg-info/SOURCES.txt` & `Zeraora-0.3.5/Zeraora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/setup.py` & `Zeraora-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/click/decorators.py` & `Zeraora-0.3.5/zeraora/click/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/constants/charsets.py` & `Zeraora-0.3.5/zeraora/constants/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/constants/configs.py` & `Zeraora-0.3.5/zeraora/constants/configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,35 +6,33 @@
 STANDARD_LOG_FMT = (
     '[%(asctime)s] [%(levelname)s] '
     '[%(module)s.%(funcName)s:%(lineno)d] '
     '%(message)s'
 )
 
 
-class FixedDict(dict):
-
-    def __new__(cls, **kwargs: Any):
-        return super().__new__(
-            cls, ((k.rstrip('_'), v) for k, v in kwargs.items())
-        )
+def fix(**kwargs: Any):
+    return dict(
+        (k.rstrip('_'), v) for k, v in kwargs.items()
+    )
 
 
 LOG_CONF_BEAR = dict(
     version=1,
     formatters={
         'bear': dict(
             format='[%(asctime)s] [%(levelname)s] %(message)s',
         ),
         'bear_plus': dict(
             format=STANDARD_LOG_FMT,
         ),
     },
     filters={},
     handlers={
-        'Console': FixedDict(
+        'Console': fix(
             level='DEBUG',
             class_='logging.StreamHandler',
             filters=[],
             formatter='bear',
         ),
     },
     loggers={
```

### Comparing `Zeraora-0.3.4/zeraora/constants/enumerations.py` & `Zeraora-0.3.5/zeraora/constants/enumerations.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/converters.py` & `Zeraora-0.3.5/zeraora/converters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/dj/fields.py` & `Zeraora-0.3.5/zeraora/dj/fields.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/dj/lookups.py` & `Zeraora-0.3.5/zeraora/dj/lookups.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/dj/models.py` & `Zeraora-0.3.5/zeraora/dj/models.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/drf/filters.py` & `Zeraora-0.3.5/zeraora/drf/filters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/drf/viewsets.py` & `Zeraora-0.3.5/zeraora/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/generators.py` & `Zeraora-0.3.5/zeraora/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,25 @@
     assert n >= 0
     return getrandbits(n * 8).to_bytes(n, 'little')
 
 
 def randb62(n: int) -> str:
     """
     生成 n 个 base62 随机字符。
+
+    返回结果不受 random 库的 seed() 影响。
     """
     return ''.join(BASE62[i % 62] for i in os.urandom(n))
 
 
 def randb64(n: int) -> str:
     """
     生成 n 个 base64 随机字符。
+
+    返回结果不受 random 库的 seed() 影响。
     """
     return ''.join(BASE64[i >> 2] for i in os.urandom(n))
 
 
 class SnowflakeWorker(object):
     STAMP = (1 << 41) - 1
     WORKER = (1 << 10) - 1
```

### Comparing `Zeraora-0.3.4/zeraora/typeclasses.py` & `Zeraora-0.3.5/zeraora/typeclasses.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.4/zeraora/utils.py` & `Zeraora-0.3.5/zeraora/utils.py`

 * *Files identical despite different names*

