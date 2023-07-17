# Comparing `tmp/xj_payment-1.0.8.tar.gz` & `tmp/xj_payment-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_payment-1.0.8.tar", last modified: Thu Oct 13 08:54:53 2022, max compression
+gzip compressed data, was "dist\xj_payment-1.0.9.tar", last modified: Thu Oct 13 09:01:56 2022, max compression
```

## Comparing `xj_payment-1.0.8.tar` & `xj_payment-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:53.000000 xj_payment-1.0.8/
--rw-rw-rw-   0        0        0     1438 2022-10-13 08:54:53.000000 xj_payment-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      946 2022-08-26 02:08:41.000000 xj_payment-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-10-13 08:54:53.000000 xj_payment-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2000 2022-10-13 08:53:17.000000 xj_payment-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment/
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/__init__.py
--rw-rw-rw-   0        0        0      615 2022-09-06 09:29:32.000000 xj_payment-1.0.8/xj_payment/admin.py
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:53.000000 xj_payment-1.0.8/xj_payment/apis/
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/apis/__init__.py
--rw-rw-rw-   0        0        0    10845 2022-08-26 02:42:21.000000 xj_payment-1.0.8/xj_payment/apis/alipay.py
--rw-rw-rw-   0        0        0     2928 2022-09-07 07:56:56.000000 xj_payment-1.0.8/xj_payment/apis/data.py
--rw-rw-rw-   0        0        0     2330 2022-08-29 09:35:13.000000 xj_payment-1.0.8/xj_payment/apis/payment_alipay.py
--rw-rw-rw-   0        0        0      251 2022-09-05 07:02:37.000000 xj_payment-1.0.8/xj_payment/apis/payment_unionpay.py
--rw-rw-rw-   0        0        0     1354 2022-10-12 06:29:39.000000 xj_payment-1.0.8/xj_payment/apis/payment_wechat.py
--rw-rw-rw-   0        0        0     1211 2022-08-26 02:42:29.000000 xj_payment-1.0.8/xj_payment/apis/transaction_inquiry.py
--rw-rw-rw-   0        0        0     2571 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/apis/wechat.py
--rw-rw-rw-   0        0        0     3531 2022-09-20 02:07:10.000000 xj_payment-1.0.8/xj_payment/apis/wechat_payment.py
--rw-rw-rw-   0        0        0      208 2022-09-06 08:56:42.000000 xj_payment-1.0.8/xj_payment/apps.py
--rw-rw-rw-   0        0        0     1675 2022-08-29 03:39:13.000000 xj_payment-1.0.8/xj_payment/common.py
--rw-rw-rw-   0        0        0     3951 2022-09-06 09:51:38.000000 xj_payment-1.0.8/xj_payment/models.py
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:53.000000 xj_payment-1.0.8/xj_payment/services/
--rw-rw-rw-   0        0        0     4944 2022-09-07 08:47:14.000000 xj_payment-1.0.8/xj_payment/services/DataConsolidation.py
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/services/__init__.py
--rw-rw-rw-   0        0        0     5412 2022-10-12 03:09:23.000000 xj_payment-1.0.8/xj_payment/services/payment_alipay_service.py
--rw-rw-rw-   0        0        0      441 2022-09-01 08:12:02.000000 xj_payment-1.0.8/xj_payment/services/payment_service.py
--rw-rw-rw-   0        0        0     4568 2022-09-05 07:00:52.000000 xj_payment-1.0.8/xj_payment/services/payment_unionpay_service.py
--rw-rw-rw-   0        0        0     6616 2022-10-12 06:28:28.000000 xj_payment-1.0.8/xj_payment/services/payment_wechat_service.py
--rw-rw-rw-   0        0        0      725 2022-09-05 01:43:15.000000 xj_payment-1.0.8/xj_payment/services/pyment_finance_service.py
--rw-rw-rw-   0        0        0     2211 2022-09-26 03:16:12.000000 xj_payment-1.0.8/xj_payment/urls.py
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:53.000000 xj_payment-1.0.8/xj_payment/utils/
--rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/utils/__init__.py
--rw-rw-rw-   0        0        0     3037 2022-10-12 05:22:18.000000 xj_payment-1.0.8/xj_payment/utils/alipay_utils.py
--rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_payment-1.0.8/xj_payment/utils/common.py
--rw-rw-rw-   0        0        0     1350 2022-08-22 01:46:29.000000 xj_payment-1.0.8/xj_payment/utils/custom_response.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_payment-1.0.8/xj_payment/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-08-29 07:52:36.000000 xj_payment-1.0.8/xj_payment/utils/j_dict.py
--rw-rw-rw-   0        0        0     7311 2022-10-12 03:02:19.000000 xj_payment-1.0.8/xj_payment/utils/model_handle.py
--rw-rw-rw-   0        0        0     7599 2022-09-05 06:52:36.000000 xj_payment-1.0.8/xj_payment/utils/unionpay_utils.py
--rw-rw-rw-   0        0        0     2942 2022-10-12 05:31:42.000000 xj_payment-1.0.8/xj_payment/utils/utils.py
--rw-rw-rw-   0        0        0     1059 2022-09-23 02:48:43.000000 xj_payment-1.0.8/xj_payment/utils/wechat_utils.py
-drwxrwxrwx   0        0        0        0 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/
--rw-rw-rw-   0        0        0     1438 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-13 08:54:52.000000 xj_payment-1.0.8/xj_payment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/
+-rw-rw-rw-   0        0        0     1438 2022-10-13 09:01:56.000000 xj_payment-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2022-08-26 02:08:41.000000 xj_payment-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-13 09:01:56.000000 xj_payment-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2003 2022-10-13 09:01:53.000000 xj_payment-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/__init__.py
+-rw-rw-rw-   0        0        0      615 2022-09-06 09:29:32.000000 xj_payment-1.0.9/xj_payment/admin.py
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/apis/__init__.py
+-rw-rw-rw-   0        0        0    10845 2022-08-26 02:42:21.000000 xj_payment-1.0.9/xj_payment/apis/alipay.py
+-rw-rw-rw-   0        0        0     2928 2022-09-07 07:56:56.000000 xj_payment-1.0.9/xj_payment/apis/data.py
+-rw-rw-rw-   0        0        0     2330 2022-08-29 09:35:13.000000 xj_payment-1.0.9/xj_payment/apis/payment_alipay.py
+-rw-rw-rw-   0        0        0      251 2022-09-05 07:02:37.000000 xj_payment-1.0.9/xj_payment/apis/payment_unionpay.py
+-rw-rw-rw-   0        0        0     1354 2022-10-12 06:29:39.000000 xj_payment-1.0.9/xj_payment/apis/payment_wechat.py
+-rw-rw-rw-   0        0        0     1211 2022-08-26 02:42:29.000000 xj_payment-1.0.9/xj_payment/apis/transaction_inquiry.py
+-rw-rw-rw-   0        0        0     2571 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/apis/wechat.py
+-rw-rw-rw-   0        0        0     3531 2022-09-20 02:07:10.000000 xj_payment-1.0.9/xj_payment/apis/wechat_payment.py
+-rw-rw-rw-   0        0        0      208 2022-09-06 08:56:42.000000 xj_payment-1.0.9/xj_payment/apps.py
+-rw-rw-rw-   0        0        0     1675 2022-08-29 03:39:13.000000 xj_payment-1.0.9/xj_payment/common.py
+-rw-rw-rw-   0        0        0     3951 2022-09-06 09:51:38.000000 xj_payment-1.0.9/xj_payment/models.py
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment/services/
+-rw-rw-rw-   0        0        0     4944 2022-09-07 08:47:14.000000 xj_payment-1.0.9/xj_payment/services/DataConsolidation.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/services/__init__.py
+-rw-rw-rw-   0        0        0     5412 2022-10-12 03:09:23.000000 xj_payment-1.0.9/xj_payment/services/payment_alipay_service.py
+-rw-rw-rw-   0        0        0      441 2022-09-01 08:12:02.000000 xj_payment-1.0.9/xj_payment/services/payment_service.py
+-rw-rw-rw-   0        0        0     4568 2022-09-05 07:00:52.000000 xj_payment-1.0.9/xj_payment/services/payment_unionpay_service.py
+-rw-rw-rw-   0        0        0     6616 2022-10-12 06:28:28.000000 xj_payment-1.0.9/xj_payment/services/payment_wechat_service.py
+-rw-rw-rw-   0        0        0      725 2022-09-05 01:43:15.000000 xj_payment-1.0.9/xj_payment/services/pyment_finance_service.py
+-rw-rw-rw-   0        0        0     2211 2022-09-26 03:16:12.000000 xj_payment-1.0.9/xj_payment/urls.py
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/utils/__init__.py
+-rw-rw-rw-   0        0        0     3037 2022-10-12 05:22:18.000000 xj_payment-1.0.9/xj_payment/utils/alipay_utils.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_payment-1.0.9/xj_payment/utils/common.py
+-rw-rw-rw-   0        0        0     1350 2022-08-22 01:46:29.000000 xj_payment-1.0.9/xj_payment/utils/custom_response.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_payment-1.0.9/xj_payment/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-08-29 07:52:36.000000 xj_payment-1.0.9/xj_payment/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7311 2022-10-12 03:02:19.000000 xj_payment-1.0.9/xj_payment/utils/model_handle.py
+-rw-rw-rw-   0        0        0     7599 2022-09-05 06:52:36.000000 xj_payment-1.0.9/xj_payment/utils/unionpay_utils.py
+-rw-rw-rw-   0        0        0     2942 2022-10-12 05:31:42.000000 xj_payment-1.0.9/xj_payment/utils/utils.py
+-rw-rw-rw-   0        0        0     1059 2022-09-23 02:48:43.000000 xj_payment-1.0.9/xj_payment/utils/wechat_utils.py
+drwxrwxrwx   0        0        0        0 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment.egg-info/
+-rw-rw-rw-   0        0        0     1438 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2022-10-13 09:01:56.000000 xj_payment-1.0.9/xj_payment.egg-info/top_level.txt
```

### Comparing `xj_payment-1.0.8/PKG-INFO` & `xj_payment-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_payment
-Version: 1.0.8
+Version: 1.0.9
 Summary: 支付模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_payment
         
         #### 介绍
         支付模块
```

### Comparing `xj_payment-1.0.8/README.md` & `xj_payment-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/setup.py` & `xj_payment-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_payment',  # 模块名称
-    version='1.0.8',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='支付模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_payment'],  # 系指定安装模块
     license="apache 3.0",
 
     install_requires=[
-        "python-alipay-sdk>=3.1.0",
-        "wechatpy>=1.8.18",
-        "pyOpenSSL>=22.0.0"
+        #"python-alipay-sdk>=3.1.0",
+        #"wechatpy>=1.8.18",
+        #"pyOpenSSL>=22.0.0"
     ]
 )
 """
 name : 打包后包的文件名
 version : 版本号
 author : 作者
 author_email : 作者的邮箱
```

### Comparing `xj_payment-1.0.8/xj_payment/admin.py` & `xj_payment-1.0.9/xj_payment/admin.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/alipay.py` & `xj_payment-1.0.9/xj_payment/apis/alipay.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/data.py` & `xj_payment-1.0.9/xj_payment/apis/data.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/payment_alipay.py` & `xj_payment-1.0.9/xj_payment/apis/payment_alipay.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/payment_wechat.py` & `xj_payment-1.0.9/xj_payment/apis/payment_wechat.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/transaction_inquiry.py` & `xj_payment-1.0.9/xj_payment/apis/transaction_inquiry.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/wechat.py` & `xj_payment-1.0.9/xj_payment/apis/wechat.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/apis/wechat_payment.py` & `xj_payment-1.0.9/xj_payment/apis/wechat_payment.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/common.py` & `xj_payment-1.0.9/xj_payment/common.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/models.py` & `xj_payment-1.0.9/xj_payment/models.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/services/DataConsolidation.py` & `xj_payment-1.0.9/xj_payment/services/DataConsolidation.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/services/payment_alipay_service.py` & `xj_payment-1.0.9/xj_payment/services/payment_alipay_service.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/services/payment_unionpay_service.py` & `xj_payment-1.0.9/xj_payment/services/payment_unionpay_service.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/services/payment_wechat_service.py` & `xj_payment-1.0.9/xj_payment/services/payment_wechat_service.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/services/pyment_finance_service.py` & `xj_payment-1.0.9/xj_payment/services/pyment_finance_service.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/urls.py` & `xj_payment-1.0.9/xj_payment/urls.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/alipay_utils.py` & `xj_payment-1.0.9/xj_payment/utils/alipay_utils.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/common.py` & `xj_payment-1.0.9/xj_payment/utils/common.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/custom_response.py` & `xj_payment-1.0.9/xj_payment/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/j_config.py` & `xj_payment-1.0.9/xj_payment/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/model_handle.py` & `xj_payment-1.0.9/xj_payment/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/unionpay_utils.py` & `xj_payment-1.0.9/xj_payment/utils/unionpay_utils.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/utils.py` & `xj_payment-1.0.9/xj_payment/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment/utils/wechat_utils.py` & `xj_payment-1.0.9/xj_payment/utils/wechat_utils.py`

 * *Files identical despite different names*

### Comparing `xj_payment-1.0.8/xj_payment.egg-info/PKG-INFO` & `xj_payment-1.0.9/xj_payment.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-payment
-Version: 1.0.8
+Version: 1.0.9
 Summary: 支付模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_payment
         
         #### 介绍
         支付模块
```

### Comparing `xj_payment-1.0.8/xj_payment.egg-info/SOURCES.txt` & `xj_payment-1.0.9/xj_payment.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 xj_payment/apps.py
 xj_payment/common.py
 xj_payment/models.py
 xj_payment/urls.py
 xj_payment.egg-info/PKG-INFO
 xj_payment.egg-info/SOURCES.txt
 xj_payment.egg-info/dependency_links.txt
-xj_payment.egg-info/requires.txt
 xj_payment.egg-info/top_level.txt
 xj_payment/apis/__init__.py
 xj_payment/apis/alipay.py
 xj_payment/apis/data.py
 xj_payment/apis/payment_alipay.py
 xj_payment/apis/payment_unionpay.py
 xj_payment/apis/payment_wechat.py
```

