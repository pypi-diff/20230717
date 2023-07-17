# Comparing `tmp/nonebot_plugin_smallapi-1.0.6.tar.gz` & `tmp/nonebot_plugin_smallapi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-1.0.6.tar", last modified: Mon Jul 17 05:41:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.0.7.tar", last modified: Mon Jul 17 06:07:08 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-1.0.6.tar` & `nonebot_plugin_smallapi-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5139 2023-07-17 05:39:35.000000 nonebot_plugin_smallapi-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.931472 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/
--rwxr-xr-x   0 root         (0) root         (0)      503 2023-07-02 01:12:30.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_menu.py
--rwxr-xr-x   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_pic.py
--rwxr-xr-x   0 root         (0) root         (0)     6026 2023-05-23 22:13:37.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_site.py
--rwxr-xr-x   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_text.py
--rwxr-xr-x   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander.py
--rwxr-xr-x   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-17 05:41:19.000000 nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      922 2023-07-17 05:40:20.000000 nonebot_plugin_smallapi-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 05:41:19.932472 nonebot_plugin_smallapi-1.0.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1075 2023-07-17 05:41:14.000000 nonebot_plugin_smallapi-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5165 2023-07-17 06:06:35.000000 nonebot_plugin_smallapi-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.501358 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-07-02 01:12:30.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_menu.py
+-rwxr-xr-x   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_pic.py
+-rwxr-xr-x   0 root         (0) root         (0)     6032 2023-07-17 06:05:45.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_site.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_text.py
+-rwxr-xr-x   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander.py
+-rwxr-xr-x   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      922 2023-07-17 06:07:03.000000 nonebot_plugin_smallapi-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1075 2023-07-17 06:06:10.000000 nonebot_plugin_smallapi-1.0.7/setup.py
```

### Comparing `nonebot_plugin_smallapi-1.0.6/LICENSE` & `nonebot_plugin_smallapi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/README.md` & `nonebot_plugin_smallapi-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,12 +154,15 @@
 
 - 修复ip查询中的致命语法错误
 
 ### 1.0.6
 
 - 维护更新，蟒蛇(Python)版本要求最低改为3.10
 
+### 1.0.7
+
+- 优化更新
 </details>
 
 ## 致谢
 - [借鉴的代码](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py)
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

#### html2text {}

```diff
@@ -40,11 +40,11 @@
 ä¾å¦ï¼```APIå¾çç³»ç»``` ### APIæå­ç³»ç» å½ä»¤ç»æï¼```(/
 )APIæå­ç³»ç»``` ä¾å¦ï¼```APIæå­ç³»ç»``` ### APIç«ç¹ç³»ç»
 å½ä»¤ç»æï¼```(/)APIç«ç¹ç³»ç»``` ä¾å¦ï¼```APIç«ç¹ç³»ç»``` ## â
 æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 -
 æä»¶åæ¬¡åå¸ ### 1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ###
 1.0.3 - æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
 ä¿®å¤é¨åBug ### 1.0.5 - ä¿®å¤ipæ¥è¯¢ä¸­çè´å½è¯­æ³éè¯¯ ### 1.0.6 -
-ç»´æ¤æ´æ°ï¼èè(Python)çæ¬è¦æ±æä½æ¹ä¸º3.10  ## è´è°¢ -
-[åé´çä»£ç ](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/
-plugins/shigure_bot/plugins/site_tool/__main__.py) - [nonebot-plugin-template]
-(https://github.com/A-kirami/nonebot-plugin-template)
+ç»´æ¤æ´æ°ï¼èè(Python)çæ¬è¦æ±æä½æ¹ä¸º3.10 ### 1.0.7 -
+ä¼åæ´æ°  ## è´è°¢ - [åé´çä»£ç ](https://github.com/lgc-NB2Dev/
+ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py) -
+[nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 @on_command("ip查询", aliases={"IP查询", "IPSOSO"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
-        format_return(
+        format_return_site(
             await get_api_resp("IP", {"ip": arg}),
             lambda ret_web: (
                 f'查询目标：{ret_web["ip"]}\n'
                 f'IP地址：{ret_web["location"].get("ip")}\n'
                 #f'IP类型：{ret_web["location"].get("isp")}\n'
                 f'IP地区：{ret_web["location"].get("country")}\n'
                 f'IP段起始: {ret_web["location"].get("range").get("start")}\n'
@@ -151,8 +151,8 @@
                 f'DNS服务器：{ret_web["nameServer"]}\n'
                 #f'域名状态：{", ".join([x["domainState"] for x in ret_web["domainState"]])}\n'
                 f'域名状态：{ret_web["domainState"]}\n'
                 f'数据更新时间：{ret_web["updateTime"]}'
             ),
         ),
         at_sender=True,
-    )
+    )
```

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_text.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/nonebot_plugin_smallapi.egg-info/SOURCES.txt` & `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.6/pyproject.toml` & `nonebot_plugin_smallapi-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_smallapi"
-version = "1.0.6"
+version = "1.0.7"
 description = "高效，快速的小小WEBAPI调用插件！"
 authors = ["Chaichaisi <chaichaisi@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_smallapi"}]
 homepage = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
 repository = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
```

### Comparing `nonebot_plugin_smallapi-1.0.6/setup.py` & `nonebot_plugin_smallapi-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools #导入setuptools打包工具
 
 setuptools.setup(
     install_requires=['jsonpath','nonebot2[aiohttp]','nonebot-adapter-onebot','nonebot2[httpx]'],
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.6",    #包版本号，便于维护版本
+    version="1.0.7",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

