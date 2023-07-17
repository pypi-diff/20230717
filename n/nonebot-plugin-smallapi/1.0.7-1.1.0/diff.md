# Comparing `tmp/nonebot_plugin_smallapi-1.0.7.tar.gz` & `tmp/nonebot_plugin_smallapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smallapi-1.0.7.tar", last modified: Mon Jul 17 06:07:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_smallapi-1.1.0.tar", last modified: Mon Jul 17 06:23:24 2023, max compression
```

## Comparing `nonebot_plugin_smallapi-1.0.7.tar` & `nonebot_plugin_smallapi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/
--rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5165 2023-07-17 06:06:35.000000 nonebot_plugin_smallapi-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.501358 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/
--rwxr-xr-x   0 root         (0) root         (0)      503 2023-07-02 01:12:30.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_menu.py
--rwxr-xr-x   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_pic.py
--rwxr-xr-x   0 root         (0) root         (0)     6032 2023-07-17 06:05:45.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_site.py
--rwxr-xr-x   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_text.py
--rwxr-xr-x   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander.py
--rwxr-xr-x   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander_site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-17 06:07:08.000000 nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      922 2023-07-17 06:07:03.000000 nonebot_plugin_smallapi-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 06:07:08.502358 nonebot_plugin_smallapi-1.0.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1075 2023-07-17 06:06:10.000000 nonebot_plugin_smallapi-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:23:24.919060 nonebot_plugin_smallapi-1.1.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1072 2023-05-15 01:08:18.000000 nonebot_plugin_smallapi-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:23:24.918060 nonebot_plugin_smallapi-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-07-17 06:15:34.000000 nonebot_plugin_smallapi-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:23:24.917060 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-07-02 01:12:30.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1980 2023-05-23 15:12:35.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_menu.py
+-rwxr-xr-x   0 root         (0) root         (0)     2153 2023-05-23 15:00:36.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_pic.py
+-rwxr-xr-x   0 root         (0) root         (0)     6112 2023-07-17 06:17:10.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_site.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-05-23 15:05:23.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_text.py
+-rwxr-xr-x   0 root         (0) root         (0)     2204 2023-05-23 15:01:55.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/hander.py
+-rwxr-xr-x   0 root         (0) root         (0)     1940 2023-05-23 15:02:43.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/hander_site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 06:23:24.918060 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 06:23:24.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-17 06:23:24.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 06:23:24.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-17 06:23:24.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-17 06:23:24.000000 nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      922 2023-07-17 06:14:50.000000 nonebot_plugin_smallapi-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 06:23:24.919060 nonebot_plugin_smallapi-1.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1075 2023-07-17 06:14:28.000000 nonebot_plugin_smallapi-1.1.0/setup.py
```

### Comparing `nonebot_plugin_smallapi-1.0.7/LICENSE` & `nonebot_plugin_smallapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/README.md` & `nonebot_plugin_smallapi-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,12 +157,16 @@
 ### 1.0.6
 
 - 维护更新，蟒蛇(Python)版本要求最低改为3.10
 
 ### 1.0.7
 
 - 优化更新
+
+### 1.1.0
+
+- 站点代码重写更新
 </details>
 
 ## 致谢
 - [借鉴的代码](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py)
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
```

#### html2text {}

```diff
@@ -41,10 +41,11 @@
 )APIæå­ç³»ç»``` ä¾å¦ï¼```APIæå­ç³»ç»``` ### APIç«ç¹ç³»ç»
 å½ä»¤ç»æï¼```(/)APIç«ç¹ç³»ç»``` ä¾å¦ï¼```APIç«ç¹ç³»ç»``` ## â
 æå± è¿æ²¡æå¢ï½ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 1.0.0 -
 æä»¶åæ¬¡åå¸ ### 1.0.1 - ä¿®å¤ä¾èµé®é¢ ### 1.0.2 - æ¢å¼äºåº¦ ###
 1.0.3 - æ¢å¼ä¸åº¦ï¼ç»äºä¿®å¥½äºä¾èµ ### 1.0.4 - æ´æ¢ç¨³å®API,
 ä¿®å¤é¨åBug ### 1.0.5 - ä¿®å¤ipæ¥è¯¢ä¸­çè´å½è¯­æ³éè¯¯ ### 1.0.6 -
 ç»´æ¤æ´æ°ï¼èè(Python)çæ¬è¦æ±æä½æ¹ä¸º3.10 ### 1.0.7 -
-ä¼åæ´æ°  ## è´è°¢ - [åé´çä»£ç ](https://github.com/lgc-NB2Dev/
-ShigureBot/blob/main/src/plugins/shigure_bot/plugins/site_tool/__main__.py) -
-[nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
+ä¼åæ´æ° ### 1.1.0 - ç«ç¹ä»£ç éåæ´æ°  ## è´è°¢ -
+[åé´çä»£ç ](https://github.com/lgc-NB2Dev/ShigureBot/blob/main/src/
+plugins/shigure_bot/plugins/site_tool/__main__.py) - [nonebot-plugin-template]
+(https://github.com/A-kirami/nonebot-plugin-template)
```

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_menu.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_menu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_pic.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_site.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
         format_return_site(
-            await get_api_resp("IP", {"ip": arg}),
+            await get_api_resp_site("IP", {"ip": arg}),
             lambda ret_web: (
                 f'查询目标：{ret_web["ip"]}\n'
                 f'IP地址：{ret_web["location"].get("ip")}\n'
                 #f'IP类型：{ret_web["location"].get("isp")}\n'
                 f'IP地区：{ret_web["location"].get("country")}\n'
                 f'IP段起始: {ret_web["location"].get("range").get("start")}\n'
                 f'IP段结束: {ret_web["location"].get("range").get("end")}\n'
@@ -24,16 +24,16 @@
 @on_command("网站测速", aliases={"web测速", "WEB测速"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return(
-            await get_api_resp("speed", {"url": "http://" + arg}),
+        format_return_site(
+            await get_api_resp_site("speed", {"url": "http://" + arg}),
             lambda ret_web: (
                 f'访问速度：{ret_web}'
                 ),
         ),
         at_sender=True,
     )
 """
@@ -42,16 +42,16 @@
 @on_command("ping", aliases={"Ping", "PING"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入IP/域名")
 
     await matcher.finish(
-        format_return(
-            await get_api_resp("Ping", {"ip": arg}),
+        format_return_site(
+            await get_api_resp_site("Ping", {"ip": arg}),
             lambda ret_web: (
                 f'查询目标：{ret_web["host"]}\n'
                 f'IP地址：{ret_web["ip"]}\n'
                 f'延迟：{ret_web["ping_avg"]}\n'
                 f'主机位置：{ret_web["location"]}\n'
                 f'请求节点: {ret_web["node"]}\n'
                 #f'主机类型: {ret_web["type"]}\n'
@@ -65,16 +65,16 @@
 @on_command("ICP查询", aliases={"icp查询", "Icp查询", "备案查询"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return(
-            await get_api_resp("ICP", {"domain": arg}),
+        format_return_site(
+            await get_api_resp_site("ICP", {"domain": arg}),
             lambda ret_web: (
                 f'查询域名：{ret_web["domain"]}\n'
                 f'网站名称：{ret_web["serviceName"]}\n'
                 f'主页地址：{ret_web["homeUrl"]}\n'
                 f'主办单位名称：{ret_web["unitName"]}\n'
                 f'主办单位性质：{ret_web["class"]}\n'
                 f'备案号：{ret_web["icp"]}\n'
@@ -88,40 +88,40 @@
 @on_command("拦截检测").handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入网址")
 
     params = {"url": arg}
-    qq = await get_api_resp("TencentUrl", params)
+    qq = await get_api_resp_site("TencentUrl", params)
     if qq["code"] != 200:
-        await matcher.finish(format_return(qq))
+        await matcher.finish(format_return_site(qq))
 
-    wx = await get_api_resp("WxUrl", params)
+    wx = await get_api_resp_site("WxUrl", params)
     if wx["code"] != 200:
-        await matcher.finish(format_return(wx))
+        await matcher.finish(format_return_site(wx))
 
     qq["data"]["type"] = wx["data"]["type"]
     await matcher.finish(
-        format_return(
+        format_return_site(
             wx,
             lambda ret_web: f'查询网址：{ret_web["url"]}\nQQ/微信拦截状态：{ret_web["type"]}/{ret_web["type"]}',
         ),
         at_sender=True,
     )
 
 @on_command("收录查询").handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return(
-            await get_api_resp("CheckSEO", {"domain": arg}),
+        format_return_site(
+            await get_api_resp_site("CheckSEO", {"domain": arg}),
             lambda ret_web: (
                 f'查询域名：{ret_web["domain"]}\n'
                 f'网站标题：{title if (title := ret_web["title"]) else "未知"}\n'
                 f'百度收录量：{ret_web["baidu"]}\n'
                 f'好搜收录量：{ret_web["haoso"]}\n'
                 f'神马收录量：{ret_web["sm"]}\n'
                 f'搜狗收录量：{ret_web["sogou"]}\n'
@@ -135,16 +135,16 @@
 @on_command("whois查询", aliases={"Whois查询", "WhoIs查询", "WHOIS查询"}).handle()
 @error_handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     if not (arg := args.extract_plain_text()):
         await matcher.finish("请输入域名")
 
     await matcher.finish(
-        format_return(
-            await get_api_resp("Whois", {"domain": arg}),
+        format_return_site(
+            await get_api_resp_site("Whois", {"domain": arg}),
             lambda ret_web: (
                 f'查询域名：{ret_web["domain"]}\n'
                 f'注册商：{ret_web["registrar"]}\n'
                 f'注册人：{ret_web["registrant"]}\n'
                 f'注册邮箱：{ret_web["email"]}\n'
                 f'注册时间：{format_json_time(ret_web["registrationTime"])}\n'
                 f'到期时间：{format_json_time(ret_web["expirationTime"])}\n'
```

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/api_text.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/api_text.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/hander.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi/hander_site.py` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi/hander_site.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/nonebot_plugin_smallapi.egg-info/SOURCES.txt` & `nonebot_plugin_smallapi-1.1.0/nonebot_plugin_smallapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smallapi-1.0.7/pyproject.toml` & `nonebot_plugin_smallapi-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_smallapi"
-version = "1.0.7"
+version = "1.1.0"
 description = "高效，快速的小小WEBAPI调用插件！"
 authors = ["Chaichaisi <chaichaisi@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_smallapi"}]
 homepage = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
 repository = "https://github.com/chaichaisi/nonebot_plugin_smallapi"
```

### Comparing `nonebot_plugin_smallapi-1.0.7/setup.py` & `nonebot_plugin_smallapi-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools #导入setuptools打包工具
 
 setuptools.setup(
     install_requires=['jsonpath','nonebot2[aiohttp]','nonebot-adapter-onebot','nonebot2[httpx]'],
     name="nonebot_plugin_smallapi", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.7",    #包版本号，便于维护版本
+    version="1.1.0",    #包版本号，便于维护版本
     author="Chaichaisi",    #作者，可以写自己的姓名
     author_email="chaichaisi@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small nonebot_plugin_smallapi plugin",#包的简述
     long_description="come in to read more",    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/chaichaisi/nonebot_plugin_smallapi",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

