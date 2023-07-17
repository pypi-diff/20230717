# Comparing `tmp/aws_ssm_run_command-0.1.2.tar.gz` & `tmp/aws_ssm_run_command-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_run_command-0.1.2.tar", last modified: Wed Jun 21 14:18:55 2023, max compression
+gzip compressed data, was "aws_ssm_run_command-0.2.1.tar", last modified: Mon Jul 17 16:38:43 2023, max compression
```

## Comparing `aws_ssm_run_command-0.1.2.tar` & `aws_ssm_run_command-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.155211 aws_ssm_run_command-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-21 14:18:55.155083 aws_ssm_run_command-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2979 2023-06-19 03:39:39.000000 aws_ssm_run_command-0.1.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.150489 aws_ssm_run_command-0.1.2/aws_ssm_run_command/
--rw-r--r--   0 sanhehu    (501) staff       (20)      331 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-21 14:13:12.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-19 03:32:02.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.152260 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-19 02:18:57.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-06-19 02:33:36.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5165 2023-06-21 14:15:03.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/better_boto/aws_ssm_send_command.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.152510 aws_ssm_run_command-0.1.2/aws_ssm_run_command/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.153563 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:13:56.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       92 2023-06-19 03:34:31.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7974 2023-06-19 03:30:56.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/run_command_on_one_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      147 2023-06-19 03:34:15.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/patterns/run_command_on_one_ec2_api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154059 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154475 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-18 23:14:42.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.151125 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1101 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-21 14:18:55.000000 aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1317 2023-06-21 14:16:13.000000 aws_ssm_run_command-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      445 2023-06-19 03:40:42.000000 aws_ssm_run_command-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       36 2023-06-19 03:31:19.000000 aws_ssm_run_command-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-21 14:18:55.155251 aws_ssm_run_command-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 14:18:55.154817 aws_ssm_run_command-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      618 2023-06-19 03:35:27.000000 aws_ssm_run_command-0.1.2/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.117611 aws_ssm_run_command-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4162 2023-07-17 16:38:43.117441 aws_ssm_run_command-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3046 2023-07-17 16:36:43.000000 aws_ssm_run_command-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.113829 aws_ssm_run_command-0.2.1/aws_ssm_run_command/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      331 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-17 16:03:29.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      125 2023-07-17 16:10:28.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.114959 aws_ssm_run_command-0.2.1/aws_ssm_run_command/better_boto/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-19 02:18:57.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/better_boto/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      354 2023-07-17 16:10:16.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/better_boto/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6432 2023-07-17 16:25:01.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/better_boto/aws_ssm_send_command.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.115222 aws_ssm_run_command-0.2.1/aws_ssm_run_command/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      619 2023-07-17 16:06:34.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.116061 aws_ssm_run_command-0.2.1/aws_ssm_run_command/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:13:56.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       92 2023-06-19 03:34:31.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/patterns/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8100 2023-07-17 16:30:03.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/patterns/run_command_on_one_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-07-17 16:30:12.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/patterns/run_command_on_one_ec2_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.116406 aws_ssm_run_command-0.2.1/aws_ssm_run_command/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.116824 aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-18 23:14:42.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.114418 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4162 2023-07-17 16:38:43.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1128 2023-07-17 16:38:43.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-17 16:38:43.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-07-17 16:38:43.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-07-17 16:38:43.000000 aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1628 2023-07-17 16:38:16.000000 aws_ssm_run_command-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      445 2023-06-19 03:40:42.000000 aws_ssm_run_command-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       36 2023-06-19 03:31:19.000000 aws_ssm_run_command-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-17 16:38:43.117660 aws_ssm_run_command-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-18 23:12:23.000000 aws_ssm_run_command-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 16:38:43.117057 aws_ssm_run_command-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      683 2023-07-17 16:22:31.000000 aws_ssm_run_command-0.2.1/tests/test_api.py
```

### Comparing `aws_ssm_run_command-0.1.2/AUTHORS.rst` & `aws_ssm_run_command-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/LICENSE.txt` & `aws_ssm_run_command-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/PKG-INFO` & `aws_ssm_run_command-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_ssm_run_command
-Version: 0.1.2
+Version: 0.2.1
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_ssm_run_command-project
-Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -82,14 +82,15 @@
 
 Welcome to ``aws_ssm_run_command`` Documentation
 ==============================================================================
 Utility tool to use AWS SSM run command feature more efficiently.
 
 Example:
 
+- `run_command synchronously <./examples/run_command/example.py>`_
 - `run_command_on_one_ec2-run_python_script <./examples/run_command_on_one_ec2-run_python_script>`_
 - `run_command_on_one_ec2-run_python_script_large_payload <./examples/run_command_on_one_ec2-run_python_script_large_payload>`_
 
 
 .. _install:
 
 Install
```

### Comparing `aws_ssm_run_command-0.1.2/README.rst` & `aws_ssm_run_command-0.2.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 Welcome to ``aws_ssm_run_command`` Documentation
 ==============================================================================
 Utility tool to use AWS SSM run command feature more efficiently.
 
 Example:
 
+- `run_command synchronously <./examples/run_command/example.py>`_
 - `run_command_on_one_ec2-run_python_script <./examples/run_command_on_one_ec2-run_python_script>`_
 - `run_command_on_one_ec2-run_python_script_large_payload <./examples/run_command_on_one_ec2-run_python_script_large_payload>`_
 
 
 .. _install:
 
 Install
```

### Comparing `aws_ssm_run_command-0.1.2/aws_ssm_run_command/paths.py` & `aws_ssm_run_command-0.2.1/aws_ssm_run_command/paths.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/pytest_cov_helper.py` & `aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/aws_ssm_run_command/vendor/waiter.py` & `aws_ssm_run_command-0.2.1/aws_ssm_run_command/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/PKG-INFO` & `aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-ssm-run-command
-Version: 0.1.2
+Version: 0.2.1
 Summary: Package short description.
 Home-page: https://github.com/MacHu-GWU/aws_ssm_run_command-project
-Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/aws_ssm_run_command/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -82,14 +82,15 @@
 
 Welcome to ``aws_ssm_run_command`` Documentation
 ==============================================================================
 Utility tool to use AWS SSM run command feature more efficiently.
 
 Example:
 
+- `run_command synchronously <./examples/run_command/example.py>`_
 - `run_command_on_one_ec2-run_python_script <./examples/run_command_on_one_ec2-run_python_script>`_
 - `run_command_on_one_ec2-run_python_script_large_payload <./examples/run_command_on_one_ec2-run_python_script_large_payload>`_
 
 
 .. _install:
 
 Install
```

### Comparing `aws_ssm_run_command-0.1.2/aws_ssm_run_command.egg-info/SOURCES.txt` & `aws_ssm_run_command-0.2.1/aws_ssm_run_command.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 aws_ssm_run_command/__init__.py
 aws_ssm_run_command/_version.py
 aws_ssm_run_command/api.py
+aws_ssm_run_command/exc.py
 aws_ssm_run_command/paths.py
 aws_ssm_run_command.egg-info/PKG-INFO
 aws_ssm_run_command.egg-info/SOURCES.txt
 aws_ssm_run_command.egg-info/dependency_links.txt
 aws_ssm_run_command.egg-info/requires.txt
 aws_ssm_run_command.egg-info/top_level.txt
 aws_ssm_run_command/better_boto/__init__.py
```

### Comparing `aws_ssm_run_command-0.1.2/release-history.rst` & `aws_ssm_run_command-0.2.1/release-history.rst`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.1 (2023-07-17)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``aws_ssm_run_command.api.better_boto.send_command_async`` and ``aws_ssm_run_command.api.better_boto.send_command_sync`` API.
+
+**Minor Improvements**
+
+- improve example code
+
+
 0.1.2 (2023-06-21)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - add ``raises`` argument to ``aws_ssm_run_command.api.better_boto.wait_until_command_succeeded`` function. Allow user to specify whether to raise an exception if the command fails. Default to ``True``.
```

### Comparing `aws_ssm_run_command-0.1.2/requirements-doc.txt` & `aws_ssm_run_command-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/setup.py` & `aws_ssm_run_command-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_run_command-0.1.2/tests/test_api.py` & `aws_ssm_run_command-0.2.1/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 from aws_ssm_run_command import api
 
 
 def test():
     _ = api
 
-    _ = api.better_boto.CommandInvocationFailedError
     _ = api.better_boto.send_command
+    _ = api.better_boto.send_command_sync
+    _ = api.better_boto.send_command_async
     _ = api.better_boto.CommandInvocationStatusEnum
     _ = api.better_boto.CommandInvocation
     _ = api.better_boto.wait_until_command_succeeded
 
     _ = api.patterns.run_command_on_one_ec2.run_python_script
     _ = api.patterns.run_command_on_one_ec2.run_python_script_large_payload
 
+    _ = api.exc.RunCommandError
+
 
 if __name__ == "__main__":
     from aws_ssm_run_command.tests import run_cov_test
 
     run_cov_test(__file__, "aws_ssm_run_command.api", preview=False)
```

