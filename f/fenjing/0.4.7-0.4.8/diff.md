# Comparing `tmp/fenjing-0.4.7.tar.gz` & `tmp/fenjing-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.7.tar", last modified: Mon Jul 17 15:35:37 2023, max compression
+gzip compressed data, was "fenjing-0.4.8.tar", last modified: Mon Jul 17 16:56:37 2023, max compression
```

## Comparing `fenjing-0.4.7.tar` & `fenjing-0.4.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.251654 fenjing-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 15:35:23.000000 fenjing-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 15:35:23.000000 fenjing-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-17 15:35:37.247654 fenjing-0.4.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7664 2023-07-17 15:35:23.000000 fenjing-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:35:23.000000 fenjing-0.4.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    33353 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 15:35:23.000000 fenjing-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:35:37.251654 fenjing-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 15:35:23.000000 fenjing-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 16:56:26.000000 fenjing-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 16:56:26.000000 fenjing-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-17 16:56:37.666393 fenjing-0.4.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9016 2023-07-17 16:56:26.000000 fenjing-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 16:56:26.000000 fenjing-0.4.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33353 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-17 16:56:26.000000 fenjing-0.4.8/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:56:37.000000 fenjing-0.4.8/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 16:56:26.000000 fenjing-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:56:37.666393 fenjing-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 16:56:26.000000 fenjing-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:56:37.666393 fenjing-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-17 16:56:26.000000 fenjing-0.4.8/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.7/LICENSE` & `fenjing-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/PKG-INFO` & `fenjing-0.4.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.7
+Version: 0.4.8
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
+- 使用Shell指令对要发送的payload进行编码
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -126,14 +127,16 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+各个功能的介绍：
+
 - webui: 网页UI
   - 顾名思义，网页UI
   - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
@@ -143,27 +146,49 @@
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - crack-path: 对某个特定的路径进行攻击
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
+
+一些特殊的选项：
+
+- `--detect-mode`：检测模式，可为accurate或fast
+  - 默认为accurate
+  - 在开始尝试触发WAF, 获取WAF页面对应hash时：
+    - accurate模式会一个接一个地发送尽可能多的payload
+    - fast模式会将多个payload组合在一起发送，
+  - 在生成payload时：
+    - accurate模式会先从最简单的方法试起
+    - fast模式会先尝试使用复杂但通常更能绕过WAF的方法
+- `--tamper-cmd`：编码payload
+  - 某些情况下，目标会先将用户输入进行base64解码后再渲染
+  - tamper-cmd可以在payload发出前先调用shell指令对payload进行编码，从而处理上述情况
+  - 例如：
+    - `--tamper-cmd 'rev'`：将payload反转后再发出
+    - `--tamper-cmd 'base64'`：将payload进行base64编码后发出
+    - `--tamper-cmd 'base64 | rev'`：将payload进行base64编码并反转后再发出
+  - 更多例子可以参考[examples.md](examples.md)
+
+
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
 Options:
@@ -173,14 +198,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
@@ -189,28 +215,30 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
@@ -238,8 +266,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
+[![](https://mermaid.ink/img/pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE?type=png)](https://mermaid.live/edit#pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE)
```

### Comparing `fenjing-0.4.7/README.md` & `fenjing-0.4.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
+- 使用Shell指令对要发送的payload进行编码
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -113,14 +114,16 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+各个功能的介绍：
+
 - webui: 网页UI
   - 顾名思义，网页UI
   - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
@@ -130,27 +133,49 @@
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - crack-path: 对某个特定的路径进行攻击
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
+
+一些特殊的选项：
+
+- `--detect-mode`：检测模式，可为accurate或fast
+  - 默认为accurate
+  - 在开始尝试触发WAF, 获取WAF页面对应hash时：
+    - accurate模式会一个接一个地发送尽可能多的payload
+    - fast模式会将多个payload组合在一起发送，
+  - 在生成payload时：
+    - accurate模式会先从最简单的方法试起
+    - fast模式会先尝试使用复杂但通常更能绕过WAF的方法
+- `--tamper-cmd`：编码payload
+  - 某些情况下，目标会先将用户输入进行base64解码后再渲染
+  - tamper-cmd可以在payload发出前先调用shell指令对payload进行编码，从而处理上述情况
+  - 例如：
+    - `--tamper-cmd 'rev'`：将payload反转后再发出
+    - `--tamper-cmd 'base64'`：将payload进行base64编码后发出
+    - `--tamper-cmd 'base64 | rev'`：将payload进行base64编码并反转后再发出
+  - 更多例子可以参考[examples.md](examples.md)
+
+
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
 Options:
@@ -160,14 +185,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
@@ -176,28 +202,30 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
@@ -225,8 +253,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
+[![](https://mermaid.ink/img/pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE?type=png)](https://mermaid.live/edit#pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE)
```

### Comparing `fenjing-0.4.7/fenjing/cli.py` & `fenjing-0.4.8/fenjing/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import partial
 
 import click
 
 
 from .form import get_form
 from .cracker import Cracker
-from .submitter import Submitter, PathSubmitter, FormSubmitter
+from .submitter import Submitter, PathSubmitter, FormSubmitter, shell_tamperer
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
 from .const import (
     OS_POPEN_READ,
     DEFAULT_USER_AGENT,
     CONFIG,
@@ -128,24 +128,28 @@
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
 @click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
+@click.option(
+    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
+)
 def get_config(
     url: str,
     action: str,
     method: str,
     inputs: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    tamper_cmd: str,
 ):
     """
     攻击指定的表单，并获得目标服务器的flask config
     """
     print(TITLE)
     assert all(
         param is not None for param in [url, inputs]
@@ -158,17 +162,22 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
+    tamperer = None
+    if tamper_cmd:
+        tamperer = shell_tamperer(tamper_cmd)
     found, submitter, full_payload_gen = False, None, None
     for input_field in form["inputs"]:
         submitter = FormSubmitter(url, form, input_field, requester)
+        if tamperer:
+            submitter.add_tamperer(tamperer)
         cracker = Cracker(submitter, detect_mode=detect_mode)
         if not cracker.has_respond():
             logger.info(
                 "Test input field %s failed, continue...", input_field
             )
             continue
         full_payload_gen = cracker.crack()
@@ -213,25 +222,29 @@
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
 @click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
+@click.option(
+    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
+)
 def crack(
     url: str,
     action: str,
     method: str,
     inputs: str,
     exec_cmd: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    tamper_cmd: str,
 ):
     """
     攻击指定的表单
     """
     print(TITLE)
     assert all(
         param is not None for param in [url, inputs]
@@ -244,17 +257,22 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
+    tamperer = None
+    if tamper_cmd:
+        tamperer = shell_tamperer(tamper_cmd)
     found, submitter, full_payload_gen = False, None, None
     for input_field in form["inputs"]:
         submitter = FormSubmitter(url, form, input_field, requester)
+        if tamperer:
+            submitter.add_tamperer(tamperer)
         cracker = Cracker(submitter, detect_mode=detect_mode)
         if not cracker.has_respond():
             logger.info(
                 "Test input field %s failed, continue...", input_field
             )
             continue
         full_payload_gen = cracker.crack()
@@ -290,36 +308,43 @@
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
 @click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
+@click.option(
+    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
+)
 def crack_path(
     url: str,
     exec_cmd: str,
     interval: float,
     detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
+    tamper_cmd: str,
 ):
     """
     攻击指定的路径
     """
     assert url is not None, "Please provide URL!"
     print(TITLE)
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
     submitter = PathSubmitter(url=url, requester=requester)
+    if tamper_cmd:
+        tamperer = shell_tamperer(tamper_cmd)
+        submitter.add_tamperer(tamperer)
     cracker = Cracker(submitter=submitter, detect_mode=detect_mode)
     full_payload_gen = cracker.crack()
     if full_payload_gen is None:
         logger.warning("Test form failed...")
         return
     cmd_exec_func = partial(
         cmd_exec_submitter,
@@ -341,15 +366,27 @@
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="检测模式，可为accurate或fast"
 )
 @click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-def scan(url, exec_cmd, interval, detect_mode, user_agent, header, cookies):
+@click.option(
+    "--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作"
+)
+def scan(
+    url,
+    exec_cmd,
+    interval,
+    detect_mode,
+    user_agent,
+    header,
+    cookies,
+    tamper_cmd: str,
+):
     """
     扫描指定的网站
     """
     print(TITLE)
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
@@ -358,17 +395,22 @@
         ),
     )
     url_forms = (
         (page_url, form)
         for (page_url, forms) in yield_form(requester, url)
         for form in forms
     )
+    tamperer = None
+    if tamper_cmd:
+        tamperer = shell_tamperer(tamper_cmd)
     for page_url, form in url_forms:
         for input_field in form["inputs"]:
             submitter = FormSubmitter(page_url, form, input_field, requester)
+            if tamperer:
+                submitter.add_tamperer(tamperer)
             cracker = Cracker(submitter, detect_mode=detect_mode)
             if not cracker.has_respond():
                 continue
             full_payload_gen = cracker.crack()
             if full_payload_gen is None:
                 continue
             cmd_exec_func = partial(
```

### Comparing `fenjing-0.4.7/fenjing/colorize.py` & `fenjing-0.4.8/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/config_payload.py` & `fenjing-0.4.8/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/const.py` & `fenjing-0.4.8/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/context_vars.py` & `fenjing-0.4.8/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/cracker.py` & `fenjing-0.4.8/fenjing/cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/form.py` & `fenjing-0.4.8/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/full_payload_gen.py` & `fenjing-0.4.8/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/payload_gen.py` & `fenjing-0.4.8/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/requester.py` & `fenjing-0.4.8/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/scan_url.py` & `fenjing-0.4.8/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/shell_payload.py` & `fenjing-0.4.8/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/submitter.py` & `fenjing-0.4.8/fenjing/submitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 from typing import List, Callable, Union, NamedTuple, Dict
 from urllib.parse import quote
 import logging
+import subprocess
 
 from .form import Form, fill_form
 from .requester import Requester
 from .colorize import colored
 from .const import CALLBACK_SUBMIT
+
 logger = logging.getLogger("submitter")
 
 
 Tamperer = Callable[[str], str]
 
 
+def shell_tamperer(shell_cmd: str) -> Tamperer:
+    def tamperer(payload: str):
+        proc = subprocess.Popen(
+            shell_cmd,
+            shell=True,
+            stdout=subprocess.PIPE,
+            stdin=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        proc.stdin.write(payload.encode())
+        proc.stdin.close()
+        ret = proc.wait()
+        if ret != 0:
+            raise ValueError(
+                f"Shell command return non-zero code {ret} for input {payload}"
+            )
+        return proc.stdout.read().decode()
+
+    return tamperer
+
+
 class HTTPResponse(NamedTuple):
     """解析后的HTTP响应
 
     Args:
         status_code: 返回值
         text: HTTP的正文
     """
@@ -76,23 +99,24 @@
         self.url = url
         self.form = form
         self.req = requester
         self.target_field = target_field
 
     def submit_raw(self, raw_payload: str) -> Union[HTTPResponse, None]:
         inputs = {self.target_field: raw_payload}
-        resp = self.req.request(
-            **fill_form(self.url, self.form, inputs)
+        resp = self.req.request(**fill_form(self.url, self.form, inputs))
+        self.callback(
+            CALLBACK_SUBMIT,
+            {
+                "type": "form",
+                "form": self.form,
+                "inputs": inputs,
+                "response": resp,
+            },
         )
-        self.callback(CALLBACK_SUBMIT, {
-            "type": "form",
-            "form": self.form,
-            "inputs": inputs,
-            "response": resp,
-        })
         if resp is None:
             return None
         return HTTPResponse(resp.status_code, resp.text)
 
 
 class PathSubmitter(BaseSubmitter):
     """将payload进行url编码后拼接在某个url的后面并提交，看见..和/时拒绝提交"""
@@ -120,19 +144,22 @@
                 "Don't submit %s because it can't be in the path.",
                 colored("yellow", repr(raw_payload)),
             )
             return None
         resp = self.req.request(
             method="GET", url=self.url + quote(raw_payload)
         )
-        self.callback(CALLBACK_SUBMIT, {
-            "type": "path",
-            "url": self.url,
-            "payload": raw_payload,
-            "response": resp,
-        })
+        self.callback(
+            CALLBACK_SUBMIT,
+            {
+                "type": "path",
+                "url": self.url,
+                "payload": raw_payload,
+                "response": resp,
+            },
+        )
         if resp is None:
             return None
         return HTTPResponse(resp.status_code, resp.text)
 
 
 Submitter = BaseSubmitter
```

### Comparing `fenjing-0.4.7/fenjing/templates/index.html` & `fenjing-0.4.8/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/waf_func_gen.py` & `fenjing-0.4.8/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing/webui.py` & `fenjing-0.4.8/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.8/fenjing.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.7
+Version: 0.4.8
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 支持攻击对应的HTML表单或HTML路径
+- 使用Shell指令对要发送的payload进行编码
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -126,14 +127,16 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+各个功能的介绍：
+
 - webui: 网页UI
   - 顾名思义，网页UI
   - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
@@ -143,27 +146,49 @@
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - crack-path: 对某个特定的路径进行攻击
   - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
   - 参数大致上和crack相同，但是只需要提供对应的路径
   - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
+
+一些特殊的选项：
+
+- `--detect-mode`：检测模式，可为accurate或fast
+  - 默认为accurate
+  - 在开始尝试触发WAF, 获取WAF页面对应hash时：
+    - accurate模式会一个接一个地发送尽可能多的payload
+    - fast模式会将多个payload组合在一起发送，
+  - 在生成payload时：
+    - accurate模式会先从最简单的方法试起
+    - fast模式会先尝试使用复杂但通常更能绕过WAF的方法
+- `--tamper-cmd`：编码payload
+  - 某些情况下，目标会先将用户输入进行base64解码后再渲染
+  - tamper-cmd可以在payload发出前先调用shell指令对payload进行编码，从而处理上述情况
+  - 例如：
+    - `--tamper-cmd 'rev'`：将payload反转后再发出
+    - `--tamper-cmd 'base64'`：将payload进行base64编码后发出
+    - `--tamper-cmd 'base64 | rev'`：将payload进行base64编码并反转后再发出
+  - 更多例子可以参考[examples.md](examples.md)
+
+
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
   攻击指定的表单
 
 Options:
@@ -173,14 +198,15 @@
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
@@ -189,28 +215,30 @@
   -m, --method TEXT   form的提交方式，默认为POST
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help              Show this message and exit.
 
 Usage: python -m fenjing crack-path [OPTIONS]
 
   攻击指定的路径
 
 Options:
   -u, --url TEXT       需要攻击的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
   --header TEXT        请求时使用的Headers
   --cookies TEXT       请求时使用的Cookie
+  --tamper-cmd TEXT    在发送payload之前进行编码的命令，默认不进行额外操作
   --help               Show this message and exit.
 
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
@@ -238,8 +266,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
+[![](https://mermaid.ink/img/pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE?type=png)](https://mermaid.live/edit#pako:eNptU8tuwyAQ_BWE1JziH8ihh6rXntpT68ja4CVGxYvLo0ka5d-L7SQGxxwQDLuzj1nOXJga-YZLbQ6iAevZx0tJLC4XdnsLXcOCV9qxEeyXMNpY9YcTYvEnoPNoJ0ga26Yu5Px0HU9I9TySQ1soikQSBKYhtfqS4DYSivjYKgLdY9vJ4oC70NvsehupLEpzHMFtRsOK4nnE70mwWRbCgvhG6xK_EUmigaxkIFHtkSY0MrTKZ21wAqgKVj9wDXksOKTPy1FSdIllaGtJs6I6OGkDdVLU0xOrY5-EV4buol_F8nj01S-kPXANal1daTJjqfaPuAyTdZ7_IpjTsFUebihzzjiA6X21kPl9xm7SZ1LewFylcR9mZMEl0eexxpL4mrdxQkHV8VOde5-S-wZbLPkmHgmDt6BLXtIlmkLw5v1Egm-8DbjmoavB46uCKFrL4yhrF9EO6NOY6Y618sa-jR93-L-Xf1aoMIE)
```

### Comparing `fenjing-0.4.7/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.8/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/setup.py` & `fenjing-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/tests/test_cracker.py` & `fenjing-0.4.8/tests/test_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/tests/test_full_payload_gen.py` & `fenjing-0.4.8/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.7/tests/test_payload_gen.py` & `fenjing-0.4.8/tests/test_payload_gen.py`

 * *Files identical despite different names*

