# Comparing `tmp/nonebot_plugin_smallapi-1.0.5.tar.gz` & `tmp/nonebot_plugin_smallapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-1.0.5.tar", last modified: Tue May 23 22:20:36 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.0.6.tar", last modified: Mon Jul 17 05:41:19 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-1.0.5.tar` & `nonebot_plugin_smallapi-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.701962 nonebot_plugin_smallapi-1.0.5/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 22:20:36.699962 nonebot_plugin_smallapi-1.0.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     5066 2023-05-23 22:16:25.000000 nonebot_plugin_smallapi-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.695962 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_menu.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_pic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2023-05-23 22:13:37.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_site.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_text.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 22:20:36.698962 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 22:20:36.000000 nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      921 2023-05-23 22:18:40.000000 nonebot_plugin_smallapi-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 22:20:36.701962 nonebot_plugin_smallapi-1.0.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-23 22:14:40.000000 nonebot_plugin_smallapi-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-07-17 05:39:35.000000 nonebot_plugin_smallapi-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.931472 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-07-02 01:12:30.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_menu.py
+-rwxr-xr-x   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_pic.py
+-rwxr-xr-x   0 root         (0) root         (0)     6026 2023-05-23 22:13:37.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_site.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_text.py
+-rwxr-xr-x   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander.py
+-rwxr-xr-x   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      922 2023-07-17 05:40:20.000000 nonebot_plugin_smallapi-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1075 2023-07-17 05:41:14.000000 nonebot_plugin_smallapi-1.0.6/setup.py
```

### Comparing `nonebot_plugin_smallapi-1.0.5/LICENSE` & `nonebot_plugin_smallapi-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/README.md` & `nonebot_plugin_smallapi-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/chaichaisi/nonebot_plugin_smallapi.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_smallapi">
     <img src="https://img.shields.io/pypi/v/nonebot_plugin_smallapi.svg" alt="pypi">
 </a>
 <a href="https://www.python.org">
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 </a>
 
 </div>
 
 
 ## 📖 前言及介绍
 
@@ -150,12 +150,16 @@
 
 - 更换稳定API, 修复部分Bug
 
 ### 1.0.5
 
 - 修复ip查询中的致命语法错误
 
+### 1.0.6
+
+- 维护更新，蟒蛇(Python)版本要求最低改为3.10
+
 </details>
 
 ## 致谢
 - [借鉴的代码](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py)
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

#### html2text {}

```diff
@@ -39,11 +39,12 @@
 (ç«ç¹ç³»ç») ### APIå¾çç³»ç» å½ä»¤ç»æï¼```(/)APIå¾çç³»ç»```
 ä¾å¦ï¼```APIå¾çç³»ç»``` ### APIæå­ç³»ç» å½ä»¤ç»æï¼```(/
 )APIæå­ç³»ç»``` ä¾å¦ï¼```APIæå­ç³»ç»``` ### APIç«ç¹ç³»ç»
 å½ä»¤ç»æï¼```(/)APIç«ç¹ç³»ç»``` ä¾å¦ï¼```APIç«ç¹ç³»ç»``` ## â
 æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 -
 æä»¶åæ¬¡åå¸ ### 1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ###
 1.0.3 - æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
-ä¿®å¤é¨åBug ### 1.0.5 - ä¿®å¤ipæ¥è¯¢ä¸­çè´å½è¯­æ³éè¯¯  ## è´è°¢ -
+ä¿®å¤é¨åBug ### 1.0.5 - ä¿®å¤ipæ¥è¯¢ä¸­çè´å½è¯­æ³éè¯¯ ### 1.0.6 -
+ç»´æ¤æ´æ°ï¼èè(Python)çæ¬è¦æ±æä½æ¹ä¸º3.10  ## è´è°¢ -
 [åé´çä»£ç ](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/
 plugins/shigure_bot/plugins/site_tool/__main__.py) - [nonebot-plugin-template]
 (https://github.com/A-kirami/nonebot-plugin-template)
```

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_text.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/nonebot_plugin_smallapi.egg-info/SOURCES.txt` & `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.5/pyproject.toml` & `nonebot_plugin_smallapi-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_smallapi"
-version = "1.0.5"
+version = "1.0.6"
 description = "高效，快速的小小WEBAPI调用插件！"
 authors = ["Chaichaisi <chaichaisi@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_smallapi"}]
 homepage = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
 repository = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
@@ -13,14 +13,14 @@
 # 添加清华镜像
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true  # 设置清华镜像为默认回调, 以避免 poetry 在某些缺省操作里又回调到 pypi 仓库.
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 nonebot2 = "^2.0.0rc4"
 nonebot-adapter-onebot = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_smallapi-1.0.5/setup.py` & `nonebot_plugin_smallapi-1.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools #导入setuptools打包工具
 
 setuptools.setup(
     install_requires=['jsonpath','nonebot2[aiohttp]','nonebot-adapter-onebot','nonebot2[httpx]'],
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.5",    #包版本号，便于维护版本
+    version="1.0.6",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',    #对python的最低版本要求
+    python_requires='>=3.10',    #对python的最低版本要求
 )
```

