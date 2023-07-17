# Comparing `tmp/aliyundriveAutoCheckin-0.1.7.tar.gz` & `tmp/aliyundriveAutoCheckin-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliyundriveAutoCheckin-0.1.7.tar", last modified: Mon Jul 17 12:38:31 2023, max compression
+gzip compressed data, was "aliyundriveAutoCheckin-1.7.tar", last modified: Mon Jul 17 02:26:57 2023, max compression
```

## Comparing `aliyundriveAutoCheckin-0.1.7.tar` & `aliyundriveAutoCheckin-1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:38:31.454969 aliyundriveAutoCheckin-0.1.7/
--rw-rw-rw-   0        0        0     2668 2023-07-17 12:38:31.452961 aliyundriveAutoCheckin-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-07-17 12:36:19.000000 aliyundriveAutoCheckin-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:38:31.419628 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin/
--rw-rw-rw-   0        0        0       35 2023-07-17 12:10:27.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin/__init__.py
--rw-rw-rw-   0        0        0     6340 2023-07-17 10:44:26.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin/aliyundriveAutoCheckin.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:38:31.452119 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/
--rw-rw-rw-   0        0        0     2668 2023-07-17 12:38:31.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-07-17 12:38:31.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:38:31.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-17 12:38:31.000000 aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:38:31.454969 aliyundriveAutoCheckin-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-07-17 12:38:25.000000 aliyundriveAutoCheckin-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:26:57.325819 aliyundriveAutoCheckin-1.7/
+-rw-rw-rw-   0        0        0     3371 2023-07-17 02:26:57.324802 aliyundriveAutoCheckin-1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 02:26:57.297457 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin/
+-rw-rw-rw-   0        0        0       54 2023-07-17 02:19:05.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin/__init__.py
+-rw-rw-rw-   0        0        0     4992 2023-07-14 07:40:38.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin/aliyundriveAutoCheckin.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:26:57.322852 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/
+-rw-rw-rw-   0        0        0     3371 2023-07-17 02:26:57.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-17 02:26:57.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 02:26:57.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 02:26:57.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-17 02:26:57.000000 aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 02:26:57.325819 aliyundriveAutoCheckin-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-07-17 02:26:49.000000 aliyundriveAutoCheckin-1.7/setup.py
```

### Comparing `aliyundriveAutoCheckin-0.1.7/PKG-INFO` & `aliyundriveAutoCheckin-1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 Metadata-Version: 2.1
 Name: aliyundriveAutoCheckin
-Version: 0.1.7
-Summary: 阿里云盘自动签到
-Home-page: https://github.com/zzh0107/aliyundriveAutoCheckin
+Version: 1.7
 Author: xiaohan17
 Author-email: 2799153122@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# 阿里云盘自动签到(aliyundriveAutoCheckin)
+若图片看不了,按照名字进入图片文件夹里手动打开看!
+
+
+
+文件名必须是 "阿里云盘签到.txt" 不能修改
+
+
+
+# (基础版)
+
+每一行包含两个字段，用逗号分隔：
+refresh_token：如 4ded1234da004cd4a287daed77a7a1e7，这是你的阿里云盘的 refresh token。
+是否领取奖励：如 是 或 否，表示是否在签到后领取奖励。
+
+refresh_token,是/否(领取奖励)
+例如:
+4ded4874da4cd4a287da77a7a1e7,是
+5fedcba9ba9876543210dcba,否
+
+![1](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529183.png)
+
+
+
+
+
+# (邮件版)
+
+每一行包含两个字段，用逗号分隔：
 
 1. `refresh_token`: 阿里云盘的refresh_token，用于获取access_token。
 2. `is_get_reward`: 是否领取签到奖励。如果值为 "是"，则在签到后会尝试领取奖励。
 3. `is_send_email`: 是否发送签到结果的邮件。如果值为 "是"，则会尝试发送邮件。
 4. `is_custom_email`: 是否使用自定义的SMTP服务器发送邮件。如果值为 "是"，则会使用接下来的字段作为SMTP服务器的配置。
 5. `to_addr`: 邮件的接收者地址。
 
 如果 `is_custom_email` 为 "是"，则还需要提供以下字段：
 
 1. `smtp_server`: SMTP服务器的地址。
 2. `smtp_port`: SMTP服务器的端口。
 3. `smtp_user`: SMTP服务器的用户名。
 4. `smtp_password`: SMTP服务器的密码。
 
+一个示例的文件内容可能如下：
+
+4ded123da004cd4a287daed77a7a1e7,是,是,是,123456@gmail.com,smtp.qq.com,465,654321@qq.com,uoeqqqzjwomkddjj
+
+
+
+**无论是基础版还是邮箱版,都可以签到多个阿里云盘,每行填一个即可!**
+
+
+
 # refresh_token获取方法:
 
 ![2](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529209.png)
 
 ![3](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529614.png)
 
 ![4](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529639.png)
@@ -56,7 +87,8 @@
 
 这样，每次你的电脑启动时，这个exe文件就会自动运行。
 
 
 
 
 
+ps:阿里云盘.exe 和 阿里云盘签到.txt 原文件必须放在一个文件夹里!
```

### Comparing `aliyundriveAutoCheckin-0.1.7/aliyundriveAutoCheckin.egg-info/PKG-INFO` & `aliyundriveAutoCheckin-1.7/aliyundriveAutoCheckin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 Metadata-Version: 2.1
 Name: aliyundriveAutoCheckin
-Version: 0.1.7
-Summary: 阿里云盘自动签到
-Home-page: https://github.com/zzh0107/aliyundriveAutoCheckin
+Version: 1.7
 Author: xiaohan17
 Author-email: 2799153122@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# 阿里云盘自动签到(aliyundriveAutoCheckin)
+若图片看不了,按照名字进入图片文件夹里手动打开看!
+
+
+
+文件名必须是 "阿里云盘签到.txt" 不能修改
+
+
+
+# (基础版)
+
+每一行包含两个字段，用逗号分隔：
+refresh_token：如 4ded1234da004cd4a287daed77a7a1e7，这是你的阿里云盘的 refresh token。
+是否领取奖励：如 是 或 否，表示是否在签到后领取奖励。
+
+refresh_token,是/否(领取奖励)
+例如:
+4ded4874da4cd4a287da77a7a1e7,是
+5fedcba9ba9876543210dcba,否
+
+![1](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529183.png)
+
+
+
+
+
+# (邮件版)
+
+每一行包含两个字段，用逗号分隔：
 
 1. `refresh_token`: 阿里云盘的refresh_token，用于获取access_token。
 2. `is_get_reward`: 是否领取签到奖励。如果值为 "是"，则在签到后会尝试领取奖励。
 3. `is_send_email`: 是否发送签到结果的邮件。如果值为 "是"，则会尝试发送邮件。
 4. `is_custom_email`: 是否使用自定义的SMTP服务器发送邮件。如果值为 "是"，则会使用接下来的字段作为SMTP服务器的配置。
 5. `to_addr`: 邮件的接收者地址。
 
 如果 `is_custom_email` 为 "是"，则还需要提供以下字段：
 
 1. `smtp_server`: SMTP服务器的地址。
 2. `smtp_port`: SMTP服务器的端口。
 3. `smtp_user`: SMTP服务器的用户名。
 4. `smtp_password`: SMTP服务器的密码。
 
+一个示例的文件内容可能如下：
+
+4ded123da004cd4a287daed77a7a1e7,是,是,是,123456@gmail.com,smtp.qq.com,465,654321@qq.com,uoeqqqzjwomkddjj
+
+
+
+**无论是基础版还是邮箱版,都可以签到多个阿里云盘,每行填一个即可!**
+
+
+
 # refresh_token获取方法:
 
 ![2](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529209.png)
 
 ![3](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529614.png)
 
 ![4](https://xiaohan17.oss-cn-hangzhou.aliyuncs.com/xiaohan17/wenzhang/202307141529639.png)
@@ -56,7 +87,8 @@
 
 这样，每次你的电脑启动时，这个exe文件就会自动运行。
 
 
 
 
 
+ps:阿里云盘.exe 和 阿里云盘签到.txt 原文件必须放在一个文件夹里!
```

