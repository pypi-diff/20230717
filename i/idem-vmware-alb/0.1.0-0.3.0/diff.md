# Comparing `tmp/idem_vmware_alb-0.1.0.tar.gz` & `tmp/idem_vmware_alb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_vmware_alb-0.1.0.tar", last modified: Wed May 24 15:47:11 2023, max compression
+gzip compressed data, was "idem_vmware_alb-0.3.0.tar", last modified: Mon Jul 17 17:38:52 2023, max compression
```

## Comparing `idem_vmware_alb-0.1.0.tar` & `idem_vmware_alb-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3291 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2238 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.799389 idem_vmware_alb-0.1.0/idem_vmware_alb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.799389 idem_vmware_alb-0.1.0/idem_vmware_alb/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/idem_vmware_alb/acct/vmware_alb/
--rw-r--r--   0 root         (0) root         (0)     1228 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/acct/vmware_alb/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.799389 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/
--rw-r--r--   0 root         (0) root         (0)   118336 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/healthmonitor.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/init.py
--rw-r--r--   0 root         (0) root         (0)   149839 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/pool.py
--rw-r--r--   0 root         (0) root         (0)   457251 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/virtualservice.py
--rw-r--r--   0 root         (0) root         (0)    76837 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/vsvip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.799389 idem_vmware_alb-0.1.0/idem_vmware_alb/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/
--rw-r--r--   0 root         (0) root         (0)    64081 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/healthmonitor.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/init.py
--rw-r--r--   0 root         (0) root         (0)    82896 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/pool.py
--rw-r--r--   0 root         (0) root         (0)   237679 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/virtualservice.py
--rw-r--r--   0 root         (0) root         (0)    42518 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/vsvip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.799389 idem_vmware_alb-0.1.0/idem_vmware_alb/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/idem_vmware_alb/tool/vmware_alb/
--rw-r--r--   0 root         (0) root         (0)     3149 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/tool/vmware_alb/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/tool/vmware_alb/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3291 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      901 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-24 15:47:11.000000 idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 15:47:11.803389 idem_vmware_alb-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3007 2023-05-24 15:46:56.000000 idem_vmware_alb-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)      694 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/customize/nsx_alb.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/
+-rw-r--r--   0 root         (0) root         (0)    28941 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationpersistenceprofile.py
+-rw-r--r--   0 root         (0) root         (0)   653506 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationprofile.py
+-rw-r--r--   0 root         (0) root         (0)   256843 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/cloud.py
+-rw-r--r--   0 root         (0) root         (0)   115841 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/healthmonitor.py
+-rw-r--r--   0 root         (0) root         (0)    50174 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/networkprofile.py
+-rw-r--r--   0 root         (0) root         (0)   147756 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py
+-rw-r--r--   0 root         (0) root         (0)   335167 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/serviceenginegroup.py
+-rw-r--r--   0 root         (0) root         (0)    32044 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/sslprofile.py
+-rw-r--r--   0 root         (0) root         (0)   455650 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/virtualservice.py
+-rw-r--r--   0 root         (0) root         (0)    74157 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/vsvip.py
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/
+-rw-r--r--   0 root         (0) root         (0)    20940 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationpersistenceprofile.py
+-rw-r--r--   0 root         (0) root         (0)   332037 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationprofile.py
+-rw-r--r--   0 root         (0) root         (0)   134347 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/cloud.py
+-rw-r--r--   0 root         (0) root         (0)    63671 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/healthmonitor.py
+-rw-r--r--   0 root         (0) root         (0)    30893 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/networkprofile.py
+-rw-r--r--   0 root         (0) root         (0)    84673 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/pool.py
+-rw-r--r--   0 root         (0) root         (0)   185809 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/serviceenginegroup.py
+-rw-r--r--   0 root         (0) root         (0)    21142 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/sslprofile.py
+-rw-r--r--   0 root         (0) root         (0)   236548 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/virtualservice.py
+-rw-r--r--   0 root         (0) root         (0)    42893 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/vsvip.py
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/session.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 17:38:51.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/setup.py
```

### Comparing `idem_vmware_alb-0.1.0/LICENSE` & `idem_vmware_alb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.1.0/PKG-INFO` & `idem_vmware_alb-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem_vmware_alb
-Version: 0.1.0
+Version: 0.3.0
 Summary: VMware ALB Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-vmware-alb
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-vmware-alb
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-vmware-alb/-/issues
@@ -23,49 +23,49 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Idem_vmware_alb
 ===============
 
-vmware_alb Cloud Provider for Idem
+NSX Advanced Load Balancer provider for Idem
 
 DEVELOPMENT
 ===========
 
 Clone the `idem_vmware_alb` repository and install with pip.
 
 .. code:: bash
 
     git clone git@gitlab.com:my-user/idem_vmware_alb.git
     pip install -e idem_vmware_alb
 
 ACCT
 ====
 
-After installation vmware_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
+After installation nsx_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
 In order to use them we need to set up our credentials.
 
 Create a new file called `credentials.yaml` and populate it with profiles.
 The `default` profile will be used automatically by `idem` unless you specify one with `--acct-profile=profile_name` on the cli.
 
 `acct backends <https://gitlab.com/saltstack/pop/acct-backends>`_ provide alternate methods for storing profiles.
 
-The vmware_alb provider uses the vmware_alb acct plugin for authentication.
-A profile needs to specify the authentication parameters for vmware_alb.
+The nsx_alb provider uses the nsx_alb.alb acct plugin for authentication.
+A profile needs to specify the authentication parameters for nsx_alb.alb.
 
 credentials.yaml
 
 ..  code:: sls
 
-    vmware_alb:
+    nsx_alb.alb:
       default:
         username: my_user
         password: my_good_password
-        endpoint_url: https://console.vmware_alb.com/api
+        endpoint_url: https://console.nsx_alb.com/api
 
 Now encrypt the credentials file and add the encryption key and encrypted file path to the ENVIRONMENT.
 
 The `acct` command should be available as it is a requisite of `idem` and `idem_vmware_alb`.
 Encrypt the the credential file.
 
 .. code:: bash
@@ -88,25 +88,25 @@
 =====
 A profile can be specified for use with a specific state.
 If no profile is specified, the profile called "default", if one exists, will be used:
 
 .. code:: sls
 
     ensure_user_exists:
-      vmware_alb.user.present:
+      nsx_alb.user.present:
         - acct_profile: my-staging-env
         - name: a_user_name
         - kwarg1: val1
 
 It can also be specified from the command line when executing states.
 
 .. code:: bash
 
     idem state --acct-profile my-staging-env my_state.sls
 
 It can also be specified from the command line when calling an exec module directly.
 
 .. code:: bash
 
-    idem exec --acct-profile my-staging-env vmware_alb.user.list
+    idem exec --acct-profile my-staging-env nsx_alb.user.list
```

### Comparing `idem_vmware_alb-0.1.0/README.rst` & `idem_vmware_alb-0.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Idem_vmware_alb
 ===============
 
-vmware_alb Cloud Provider for Idem
+NSX Advanced Load Balancer provider for Idem
 
 DEVELOPMENT
 ===========
 
 Clone the `idem_vmware_alb` repository and install with pip.
 
 .. code:: bash
 
     git clone git@gitlab.com:my-user/idem_vmware_alb.git
     pip install -e idem_vmware_alb
 
 ACCT
 ====
 
-After installation vmware_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
+After installation nsx_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
 In order to use them we need to set up our credentials.
 
 Create a new file called `credentials.yaml` and populate it with profiles.
 The `default` profile will be used automatically by `idem` unless you specify one with `--acct-profile=profile_name` on the cli.
 
 `acct backends <https://gitlab.com/saltstack/pop/acct-backends>`_ provide alternate methods for storing profiles.
 
-The vmware_alb provider uses the vmware_alb acct plugin for authentication.
-A profile needs to specify the authentication parameters for vmware_alb.
+The nsx_alb provider uses the nsx_alb.alb acct plugin for authentication.
+A profile needs to specify the authentication parameters for nsx_alb.alb.
 
 credentials.yaml
 
 ..  code:: sls
 
-    vmware_alb:
+    nsx_alb.alb:
       default:
         username: my_user
         password: my_good_password
-        endpoint_url: https://console.vmware_alb.com/api
+        endpoint_url: https://console.nsx_alb.com/api
 
 Now encrypt the credentials file and add the encryption key and encrypted file path to the ENVIRONMENT.
 
 The `acct` command should be available as it is a requisite of `idem` and `idem_vmware_alb`.
 Encrypt the the credential file.
 
 .. code:: bash
@@ -62,23 +62,23 @@
 =====
 A profile can be specified for use with a specific state.
 If no profile is specified, the profile called "default", if one exists, will be used:
 
 .. code:: sls
 
     ensure_user_exists:
-      vmware_alb.user.present:
+      nsx_alb.user.present:
         - acct_profile: my-staging-env
         - name: a_user_name
         - kwarg1: val1
 
 It can also be specified from the command line when executing states.
 
 .. code:: bash
 
     idem state --acct-profile my-staging-env my_state.sls
 
 It can also be specified from the command line when calling an exec module directly.
 
 .. code:: bash
 
-    idem exec --acct-profile my-staging-env vmware_alb.user.list
+    idem exec --acct-profile my-staging-env nsx_alb.user.list
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/acct/vmware_alb/basic_auth.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 async def gather(hub, profiles) -> Dict[str, Any]:
     """
     Generate token with basic auth
 
     Example:
     .. code-block:: yaml
 
-        vmware_alb:
-            default:
-                username: "admin"
-                password: "password"
-                controller: "10.65.11.14"
-                api_version: "22.1.2"
-                endpoint_url: 'https://10.65.11.14/'
-                tenant: "admin"
+        nsx_alb.alb:
+          profile_name:
+            username: "admin"
+            password: "password"
+            controller: "10.65.11.14"
+            api_version: "22.1.2"
+            endpoint_url: 'https://10.65.11.14/'
+            tenant: "admin"
+
     """
 
     sub_profiles = {}
     for (
         profile,
         ctx,
-    ) in profiles.get("vmware_alb", {}).items():
+    ) in profiles.get("nsx_alb", {}).items():
         endpoint_url = ctx.get("endpoint_url")
 
         if not re.search(BASE_URL, endpoint_url):
             endpoint_url = "".join((endpoint_url.rstrip("/"), BASE_URL))
 
         creds = f"{ctx.get('username')}:{ctx.get('password')}"
         sub_profiles[profile] = dict(
             endpoint_url=endpoint_url,
             headers={
-                "X-Avi-Tenant": ctx.get("tenant", None),
                 "X-Avi-Version": ctx.get("api_version", None),
                 "Authorization": f"Basic {base64.b64encode(creds.encode('utf-8')).decode('ascii')}",
             },
         )
     return sub_profiles
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/conf.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,14 @@
     # "my_option1": {"subcommands": ["A list of subcommands that exclusively extend this option"]},
     # This option will be available under all subcommands and the root command
     # "my_option2": {"subcommands": ["_global_"]},
 }
 
 # These are the namespaces that your project extends
 # The hub will extend these keys with the modules listed in the values
-DYNE = {"states": ["states"], "acct": ["acct"], "exec": ["exec"], "tool": ["tool"]}
+DYNE = {
+    "cloudspec": ["cloudspec"],
+    "exec": ["exec"],
+    "states": ["states"],
+    "tool": ["tool"],
+    "acct": ["acct"],
+}
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/healthmonitor.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/healthmonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,64 +6,61 @@
 from collections import OrderedDict
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-# __contracts__ = ['auto_state', 'soft_fail']
+__contracts__ = ["soft_fail"]
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: vmware_alb.healthmonitor.get
+                - path: nsx_alb.alb.healthmonitor.get
                 - kwargs:
-                  x_avi_version: value
-                  uuid: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.healthmonitor.get x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.healthmonitor.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
-    get = await hub.tool.vmware_alb.session.request(
+    get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
-        path="/healthmonitor/{uuid}".format(**{"uuid": resource_id}),
-        query_params={},
+        path="/healthmonitor/{uuid}".format(**{"uuid": resource_id})
+        if resource_id
+        else "/healthmonitor",
+        query_params={"name": name},
         data={},
+        headers={"X-Avi-Tenant": "*"},
     )
 
     if not get["result"]:
         # Send empty result for not found
         if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             result["result"] = False
@@ -74,16 +71,24 @@
         return result
 
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(f"Get '{name}' result is empty")
         return result
 
-    # Convert raw response into present format
-    raw_resource = get["ret"]
+    if "results" in get["ret"].keys():
+        if get["ret"]["count"] != 0:
+            # Convert raw response into present format
+            raw_resource = get["ret"]["results"][0]
+            resource_id = get["ret"]["results"][0]["uuid"]
+        else:
+            return result
+    else:
+        # Convert raw response into present format
+        raw_resource = get["ret"]
 
     resource_in_present_format = {"name": name, "resource_id": resource_id}
     resource_parameters = OrderedDict(
         {
             "allow_duplicate_monitors": "allow_duplicate_monitors",
             "authentication": "authentication",
             "configpb_attributes": "configpb_attributes",
@@ -114,96 +119,72 @@
             "smtp_monitor": "smtp_monitor",
             "smtps_monitor": "smtps_monitor",
             "successful_checks": "successful_checks",
             "tcp_monitor": "tcp_monitor",
             "tenant_ref": "tenant_ref",
             "type": "type",
             "udp_monitor": "udp_monitor",
-            "url": "url",
         }
     )
 
     for parameter_raw, parameter_present in resource_parameters.items():
         if parameter_raw in raw_resource and raw_resource.get(parameter_raw):
             resource_in_present_format[parameter_present] = raw_resource.get(
                 parameter_raw
             )
 
     result["ret"] = resource_in_present_format
 
     return result
 
 
-async def list_(
-    hub,
-    ctx,
-    refers_to: str = None,
-    referred_by: str = None,
-    fields: str = None,
-    include_name: bool = None,
-    skip_default: bool = None,
-    join_subresources: str = None,
-) -> Dict[str, Any]:
+async def list_(hub, ctx) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: vmware_alb.healthmonitor.list
+                - path: nsx_alb.alb.healthmonitor.list
                 - kwargs:
-                  x_avi_version: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.healthmonitor.list x_avi_version=value
+            idem exec nsx_alb.alb.healthmonitor.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.healthmonitor
+            $ idem describe nsx_alb.alb.healthmonitor
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    list = await hub.tool.vmware_alb.session.request(
+    list = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
         path="/healthmonitor",
-        query_params={
-            "refers_to": refers_to,
-            "referred_by": referred_by,
-            "fields": fields,
-            "include_name": include_name,
-            "skip_default": skip_default,
-            "join_subresources": join_subresources,
-        },
+        query_params={},
         data={},
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
@@ -545,15 +526,14 @@
         "udp_monitor",
         [
             ("maintenance_response", str, field(default=None)),
             ("udp_request", str, field(default=None)),
             ("udp_response", str, field(default=None)),
         ],
     ) = None,
-    url: str = None,
     name: str = None,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
@@ -712,48 +692,46 @@
         successful_checks(int, optional): Number of continuous successful health checks before server is marked up. Allowed values are 1-50. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tcp_monitor(Dict[str, Any], optional): tcp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * tcp_half_open (bool, optional): Configure TCP health monitor to use half-open TCP connections to monitor the health of backend servers thereby avoiding consumption of a full fledged server side connection and the overhead and logs associated with it.  This method is light-weight as it makes use of listener in server's kernel layer to measure the health and a child socket or user thread is not created on the server side. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * tcp_request (str, optional): Request data to send after completing the TCP handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * tcp_response (str, optional): Match for the desired keyword in the first 2Kb of the server's TCP response. If this field is left blank, no server response is required. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
+        type(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
         udp_monitor(Dict[str, Any], optional): udp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * udp_request (str, optional): Send UDP request. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * udp_response (str, optional): Match for keyword in the UDP response. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-        url(str, optional): url. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.healthmonitor.present:
-                - x_avi_version: value
-                - type_: value
+              nsx_alb.alb.healthmonitor.present:
+                - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.healthmonitor.create x_avi_version=value, type_=value
+            idem exec nsx_alb.alb.healthmonitor.create type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "allow_duplicate_monitors": "allow_duplicate_monitors",
         "authentication": "authentication",
         "configpb_attributes": "configpb_attributes",
         "description": "description",
@@ -783,51 +761,49 @@
         "smtp_monitor": "smtp_monitor",
         "smtps_monitor": "smtps_monitor",
         "successful_checks": "successful_checks",
         "tcp_monitor": "tcp_monitor",
         "tenant_ref": "tenant_ref",
         "type": "type",
         "udp_monitor": "udp_monitor",
-        "url": "url",
-        "uuid": "uuid",
     }
 
     payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
             payload[resource_to_raw_input_mapping[key]] = value
 
-    create = await hub.tool.vmware_alb.session.request(
+    create = await hub.tool.nsx_alb.session.request(
         ctx,
         method="post",
         path="/healthmonitor",
         query_params={},
         data=payload,
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created vmware_alb.healthmonitor '{name}'",
+        f"Created nsx_alb.alb.healthmonitor '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
 
 async def update(
     hub,
     ctx,
-    resource_id: str,
     type: str,
+    resource_id: str,
     allow_duplicate_monitors: bool = None,
     authentication: make_dataclass(
         "authentication", [("password", str), ("username", str)]
     ) = None,
     configpb_attributes: make_dataclass(
         "configpb_attributes", [("version", int, field(default=None))]
     ) = None,
@@ -1149,15 +1125,14 @@
         "udp_monitor",
         [
             ("maintenance_response", str, field(default=None)),
             ("udp_request", str, field(default=None)),
             ("udp_response", str, field(default=None)),
         ],
     ) = None,
-    url: str = None,
     name: str = None,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
@@ -1316,48 +1291,46 @@
         successful_checks(int, optional): Number of continuous successful health checks before server is marked up. Allowed values are 1-50. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tcp_monitor(Dict[str, Any], optional): tcp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * tcp_half_open (bool, optional): Configure TCP health monitor to use half-open TCP connections to monitor the health of backend servers thereby avoiding consumption of a full fledged server side connection and the overhead and logs associated with it.  This method is light-weight as it makes use of listener in server's kernel layer to measure the health and a child socket or user thread is not created on the server side. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * tcp_request (str, optional): Request data to send after completing the TCP handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * tcp_response (str, optional): Match for the desired keyword in the first 2Kb of the server's TCP response. If this field is left blank, no server response is required. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
+        type(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
         udp_monitor(Dict[str, Any], optional): udp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * udp_request (str, optional): Send UDP request. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * udp_response (str, optional): Match for keyword in the UDP response. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-        url(str, optional): url. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.healthmonitor.present:
-                - x_avi_version: value
-                - type_: value
+              nsx_alb.alb.healthmonitor.present:
+                - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.healthmonitor.update x_avi_version=value, type_=value
+            idem exec nsx_alb.alb.healthmonitor.update type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "allow_duplicate_monitors": "allow_duplicate_monitors",
         "authentication": "authentication",
         "configpb_attributes": "configpb_attributes",
         "description": "description",
@@ -1399,15 +1372,15 @@
             key in resource_to_raw_input_mapping.keys()
             and value is not None
             and key != "_last_modified"
         ):
             payload[resource_to_raw_input_mapping[key]] = value
 
     if payload:
-        update = await hub.tool.vmware_alb.session.request(
+        update = await hub.tool.nsx_alb.session.request(
             ctx,
             method="put",
             path="/healthmonitor/{uuid}".format(**{"uuid": resource_id}),
             query_params={},
             data=payload,
         )
 
@@ -1415,55 +1388,51 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated vmware_alb.healthmonitor '{name}'",
+            f"Updated nsx_alb.alb.healthmonitor '{name}'",
         )
 
     return result
 
 
-async def delete(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
+async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-
-        resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.healthmonitor.absent:
-                - x_avi_version: value
-                - uuid: value
+              nsx_alb.alb.healthmonitor.absent:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.healthmonitor.delete x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.healthmonitor.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    delete = await hub.tool.vmware_alb.session.request(
+    delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
         path="/healthmonitor/{uuid}".format(**{"uuid": resource_id}),
         query_params={},
         data={},
     )
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/pool.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,63 +5,60 @@
 """
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-# __contracts__ = ['auto_state', 'soft_fail']
+__contracts__ = ["soft_fail"]
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        resource_id(str): resource_id of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: vmware_alb.pool.get
+                - path: nsx_alb.alb.pool.get
                 - kwargs:
-                  name: value
-                  resource_id: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.pool.get name=value, resource_id=value
+            idem exec nsx_alb.alb.pool.get
     """
-
     result = dict(comment=[], ret=None, result=True)
-
-    get = await hub.tool.vmware_alb.session.request(
+    get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
-        path="/pool/{resource_id}".format(**{"resource_id": resource_id}),
-        query_params={},
+        path="/pool/{uuid}/".format(**{"uuid": resource_id})
+        if resource_id
+        else "/pool",
+        query_params={"name": name},
         data={},
+        headers={"X-Avi-Tenant": "*"},
     )
-
     if not get["result"]:
         # Send empty result for not found
         if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             result["result"] = False
             return result
 
@@ -70,104 +67,85 @@
         return result
 
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(f"Get '{name}' result is empty")
         return result
 
-    get["ret"]["resource_id"] = resource_id
-    result["ret"] = get["ret"]
+    if "results" in get["ret"].keys():
+        if get["ret"]["count"] != 0:
+            get["ret"]["resource_id"] = get["ret"]["results"][0]["uuid"]
+            result["ret"] = get["ret"]
+    else:
+        get["ret"]["resource_id"] = resource_id
+        result["ret"] = get["ret"]
 
     return result
 
 
 async def list_(
-    hub,
-    ctx,
-    refers_to: str = None,
-    referred_by: str = None,
-    fields: str = None,
-    include_name: bool = None,
-    skip_default: bool = None,
-    join_subresources: str = None,
-    cloud_resource_id: str = None,
-    cloud_ref_name: str = None,
+    hub, ctx, cloud_uuid: str = None, cloud_ref_name: str = None
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
     Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_resource_id>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_resource_id. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_resource_id>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_resource_id. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, resource_id etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
-        cloud_resource_id(str, optional): Filter to get objects that belongs to a specific cloud using its resource_id. Eg. cloud_resource_id=cloud-xyz. Defaults to None.
-        cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than resource_id. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
+        cloud_uuid(str, optional): Filter to get objects that belongs to a specific cloud using its uuid. Eg. cloud_uuid=cloud-xyz. Defaults to None.
+        cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than uuid. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: vmware_alb.pool.list
+                - path: nsx_alb.alb.pool.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.pool.list
+            idem exec nsx_alb.alb.pool.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.pool
+            $ idem describe nsx_alb.alb.pool
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    list = await hub.tool.vmware_alb.session.request(
+    list = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
         path="/pool",
-        query_params={
-            "refers_to": refers_to,
-            "referred_by": referred_by,
-            "fields": fields,
-            "include_name": include_name,
-            "skip_default": skip_default,
-            "join_subresources": join_subresources,
-            "cloud_resource_id": cloud_resource_id,
-            "cloud_ref.name": cloud_ref_name,
-        },
+        query_params={"cloud_uuid": cloud_uuid, "cloud_ref.name": cloud_ref_name},
         data={},
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
 
     for resource in list["ret"]["results"]:
         # TODO Handle pagination if required
-        resource["resource_id"] = resource.get("resource_id")
+        resource["resource_id"] = resource.get("uuid")
         result["ret"].append(resource)
 
     return result
 
 
 async def create(
     hub,
@@ -539,15 +517,15 @@
                             ],
                         )
                     ],
                     field(default=None),
                 ),
                 ("enabled", bool, field(default=None)),
                 ("external_orchestration_id", str, field(default=None)),
-                ("external_resource_id", str, field(default=None)),
+                ("external_uuid", str, field(default=None)),
                 ("hostname", str, field(default=None)),
                 (
                     "location",
                     make_dataclass(
                         "location",
                         [
                             ("latitude", float, field(default=None)),
@@ -579,15 +557,14 @@
         "sp_gs_info",
         [("fqdns", list, field(default=None)), ("gs_ref", str, field(default=None))],
     ) = None,
     ssl_key_and_certificate_ref: str = None,
     ssl_profile_ref: str = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_service_port: bool = None,
     use_service_ssl_mode: bool = None,
     vrf_ref: str = None,
     name: str = None,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
@@ -749,15 +726,15 @@
                 * subnet6 (list[Dict[str, Any]], optional): Discovered IPv6 subnet for this IP. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * ip_addr (Dict[str, Any]): ip_addr
                         * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * mask (int):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * enabled (bool, optional): Enable, Disable or Graceful Disable determine if new or existing connections to the server are allowed. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * external_orchestration_id (str, optional): UID of server in external orchestration systems. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-            * external_resource_id (str, optional): resource_id identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
+            * external_uuid (str, optional): UUID identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * hostname (str, optional): DNS resolvable name of the server.  May be used in place of the IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * ip (Dict[str, Any]): ip
                 * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * location (Dict[str, Any], optional): location
                 * latitude (float, optional): Latitude of the location. This is represented as degrees.minutes. The range is from -90.0 (south) to +90.0 (north). Allowed values are -90.0-+90.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * longitude (float, optional): Longitude of the location. This is represented as degrees.minutes. The range is from -180.0 (west) to +180.0 (east). Allowed values are -180.0-+180.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -775,50 +752,49 @@
             * static (bool, optional): If statically learned. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * verify_network (bool, optional): Verify server belongs to a discovered network or reachable via a discovered network. Verify reachable network isn't the OpenStack management network. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * vm_ref (str, optional): (internal-use) This field is used internally by Avi, not editable by the user. It is a reference to an object of type VIMgrVMRuntime. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         service_metadata(str, optional): Metadata pertaining to the service provided by this Pool. In Openshift/Kubernetes environments, app metadata info is stored. Any user input to this field will be overwritten by Avi Vantage. Field introduced in 17.2.14,18.1.5,18.2.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sni_enabled(bool, optional): Enable TLS SNI for server connections. If disabled, Avi will not send the SNI extension as part of the handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sp_gs_info(Dict[str, Any], optional): sp_gs_info. Defaults to None.
             * fqdns (list, optional): FQDNs associated with the GSLB service. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
-            * gs_ref (str, optional): GSLB service resource_id associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
+            * gs_ref (str, optional): GSLB service uuid associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         ssl_key_and_certificate_ref(str, optional): Service Engines will present a client SSL certificate to the server. It is a reference to an object of type SSLKeyAndCertificate. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         ssl_profile_ref(str, optional): When enabled, Avi re-encrypts traffic to the backend servers. The specific SSL profile defines which ciphers and SSL versions will be supported. It is a reference to an object of type SSLProfile. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This tier1_lr field should be set same as VirtualService associated for NSX-T. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_service_port(bool, optional): Do not translate the client's destination port when sending the connection to the server. Monitor port needs to be specified for health monitors. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
         use_service_ssl_mode(bool, optional): This applies only when use_service_port is set to true. If enabled, SSL mode of the connection to the server is decided by the SSL mode on the Virtualservice service port, on which the request was received. Field introduced in 21.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         vrf_ref(str, optional): Virtual Routing Context that the pool is bound to. This is used to provide the isolation of the set of networks the pool is attached to. The pool inherits the Virtual Routing Context of the Virtual Service, and this field is used only internally, and is set by pb-transform. It is a reference to an object of type VrfContext. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.pool.present:
-                - name: value
+              nsx_alb.alb.pool.present:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.pool.create name=value
+            idem exec nsx_alb.alb.pool.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "analytics_policy": "analytics_policy",
         "analytics_profile_ref": "analytics_profile_ref",
         "append_port": "append_port",
         "application_persistence_profile_ref": "application_persistence_profile_ref",
@@ -883,45 +859,44 @@
         "service_metadata": "service_metadata",
         "sni_enabled": "sni_enabled",
         "sp_gs_info": "sp_gs_info",
         "ssl_key_and_certificate_ref": "ssl_key_and_certificate_ref",
         "ssl_profile_ref": "ssl_profile_ref",
         "tenant_ref": "tenant_ref",
         "tier1_lr": "tier1_lr",
-        "url": "url",
         "use_service_port": "use_service_port",
         "use_service_ssl_mode": "use_service_ssl_mode",
         "vrf_ref": "vrf_ref",
     }
 
     payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
             payload[resource_to_raw_input_mapping[key]] = value
 
-    create = await hub.tool.vmware_alb.session.request(
+    create = await hub.tool.nsx_alb.session.request(
         ctx,
         method="post",
         path="/pool",
         query_params={},
         data=payload,
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created vmware_alb.pool '{name}'",
+        f"Created nsx_alb.alb.pool '{name}'",
     )
 
     result["ret"] = create["ret"]
 
-    result["ret"]["resource_id"] = create["ret"]["resource_id"]
+    result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
 
 async def update(
     hub,
     ctx,
     resource_id: str,
@@ -1292,15 +1267,15 @@
                             ],
                         )
                     ],
                     field(default=None),
                 ),
                 ("enabled", bool, field(default=None)),
                 ("external_orchestration_id", str, field(default=None)),
-                ("external_resource_id", str, field(default=None)),
+                ("external_uuid", str, field(default=None)),
                 ("hostname", str, field(default=None)),
                 (
                     "location",
                     make_dataclass(
                         "location",
                         [
                             ("latitude", float, field(default=None)),
@@ -1332,20 +1307,18 @@
         "sp_gs_info",
         [("fqdns", list, field(default=None)), ("gs_ref", str, field(default=None))],
     ) = None,
     ssl_key_and_certificate_ref: str = None,
     ssl_profile_ref: str = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_service_port: bool = None,
     use_service_ssl_mode: bool = None,
     vrf_ref: str = None,
     name: str = None,
-    **kwargs,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
@@ -1503,15 +1476,15 @@
                 * subnet6 (list[Dict[str, Any]], optional): Discovered IPv6 subnet for this IP. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * ip_addr (Dict[str, Any]): ip_addr
                         * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * mask (int):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * enabled (bool, optional): Enable, Disable or Graceful Disable determine if new or existing connections to the server are allowed. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * external_orchestration_id (str, optional): UID of server in external orchestration systems. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-            * external_resource_id (str, optional): resource_id identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
+            * external_uuid (str, optional): UUID identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * hostname (str, optional): DNS resolvable name of the server.  May be used in place of the IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * ip (Dict[str, Any]): ip
                 * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * location (Dict[str, Any], optional): location
                 * latitude (float, optional): Latitude of the location. This is represented as degrees.minutes. The range is from -90.0 (south) to +90.0 (north). Allowed values are -90.0-+90.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * longitude (float, optional): Longitude of the location. This is represented as degrees.minutes. The range is from -180.0 (west) to +180.0 (east). Allowed values are -180.0-+180.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -1529,50 +1502,49 @@
             * static (bool, optional): If statically learned. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * verify_network (bool, optional): Verify server belongs to a discovered network or reachable via a discovered network. Verify reachable network isn't the OpenStack management network. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * vm_ref (str, optional): (internal-use) This field is used internally by Avi, not editable by the user. It is a reference to an object of type VIMgrVMRuntime. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         service_metadata(str, optional): Metadata pertaining to the service provided by this Pool. In Openshift/Kubernetes environments, app metadata info is stored. Any user input to this field will be overwritten by Avi Vantage. Field introduced in 17.2.14,18.1.5,18.2.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sni_enabled(bool, optional): Enable TLS SNI for server connections. If disabled, Avi will not send the SNI extension as part of the handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sp_gs_info(Dict[str, Any], optional): sp_gs_info. Defaults to None.
             * fqdns (list, optional): FQDNs associated with the GSLB service. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
-            * gs_ref (str, optional): GSLB service resource_id associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
+            * gs_ref (str, optional): GSLB service uuid associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         ssl_key_and_certificate_ref(str, optional): Service Engines will present a client SSL certificate to the server. It is a reference to an object of type SSLKeyAndCertificate. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         ssl_profile_ref(str, optional): When enabled, Avi re-encrypts traffic to the backend servers. The specific SSL profile defines which ciphers and SSL versions will be supported. It is a reference to an object of type SSLProfile. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This tier1_lr field should be set same as VirtualService associated for NSX-T. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_service_port(bool, optional): Do not translate the client's destination port when sending the connection to the server. Monitor port needs to be specified for health monitors. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
         use_service_ssl_mode(bool, optional): This applies only when use_service_port is set to true. If enabled, SSL mode of the connection to the server is decided by the SSL mode on the Virtualservice service port, on which the request was received. Field introduced in 21.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         vrf_ref(str, optional): Virtual Routing Context that the pool is bound to. This is used to provide the isolation of the set of networks the pool is attached to. The pool inherits the Virtual Routing Context of the Virtual Service, and this field is used only internally, and is set by pb-transform. It is a reference to an object of type VrfContext. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.pool.present:
+              nsx_alb.alb.pool.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.pool.update
+            idem exec nsx_alb.alb.pool.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "analytics_policy": "analytics_policy",
         "analytics_profile_ref": "analytics_profile_ref",
         "append_port": "append_port",
         "application_persistence_profile_ref": "application_persistence_profile_ref",
@@ -1637,15 +1609,14 @@
         "service_metadata": "service_metadata",
         "sni_enabled": "sni_enabled",
         "sp_gs_info": "sp_gs_info",
         "ssl_key_and_certificate_ref": "ssl_key_and_certificate_ref",
         "ssl_profile_ref": "ssl_profile_ref",
         "tenant_ref": "tenant_ref",
         "tier1_lr": "tier1_lr",
-        "url": "url",
         "use_service_port": "use_service_port",
         "use_service_ssl_mode": "use_service_ssl_mode",
         "vrf_ref": "vrf_ref",
     }
 
     payload = {}
     for key, value in desired_state.items():
@@ -1653,73 +1624,70 @@
             key in resource_to_raw_input_mapping.keys()
             and value is not None
             and key != "_last_modified"
         ):
             payload[resource_to_raw_input_mapping[key]] = value
 
     if payload:
-        update = await hub.tool.vmware_alb.session.request(
+        update = await hub.tool.nsx_alb.session.request(
             ctx,
             method="put",
-            path="/pool/{resource_id}".format(**{"resource_id": resource_id}),
+            path="/pool/{uuid}".format(**{"uuid": resource_id}),
             query_params={},
             data=payload,
         )
 
         if not update["result"]:
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
-        result["resource_id"] = update["ret"]["resource_id"]
+        result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated vmware_alb.pool '{name}'",
+            f"Updated nsx_alb.alb.pool '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        resource_id(str): resource_id of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.pool.absent:
-                - name: value
-                - resource_id: value
+              nsx_alb.alb.pool.absent:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.pool.delete name=value, resource_id=value
+            idem exec nsx_alb.alb.pool.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    delete = await hub.tool.vmware_alb.session.request(
+    delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
-        path="/pool/{resource_id}".format(**{"resource_id": resource_id}),
+        path="/pool/{uuid}".format(**{"uuid": resource_id}),
         query_params={},
         data={},
     )
 
     if not delete["result"]:
         result["comment"].append(delete["comment"])
         result["result"] = False
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/virtualservice.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/virtualservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,64 +6,61 @@
 from collections import OrderedDict
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-# __contracts__ = ['auto_state', 'soft_fail']
+__contracts__ = ["soft_fail"]
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: vmware_alb.virtualservice.get
+                - path: nsx_alb.alb.virtualservice.get
                 - kwargs:
-                  x_avi_version: value
-                  uuid: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.virtualservice.get x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.virtualservice.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
-    get = await hub.tool.vmware_alb.session.request(
+    get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
-        path="/virtualservice/{uuid}".format(**{"uuid": resource_id}),
-        query_params={},
+        path="/virtualservice/{uuid}".format(**{"uuid": resource_id})
+        if resource_id
+        else "/virtualservice",
+        query_params={"name": name},
         data={},
+        headers={"X-Avi-Tenant": "*"},
     )
 
     if not get["result"]:
         # Send empty result for not found
         if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             result["result"] = False
@@ -74,16 +71,24 @@
         return result
 
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(f"Get '{name}' result is empty")
         return result
 
-    # Convert raw response into present format
-    raw_resource = get["ret"]
+    if "results" in get["ret"].keys():
+        if get["ret"]["count"] != 0:
+            # Convert raw response into present format
+            raw_resource = get["ret"]["results"][0]
+            resource_id = get["ret"]["results"][0]["uuid"]
+        else:
+            return result
+    else:
+        # Convert raw response into present format
+        raw_resource = get["ret"]
 
     resource_in_present_format = {"name": name, "resource_id": resource_id}
     resource_parameters = OrderedDict(
         {
             "active_standby_se_tag": "active_standby_se_tag",
             "advertise_down_vs": "advertise_down_vs",
             "allow_invalid_client_cert": "allow_invalid_client_cert",
@@ -100,22 +105,24 @@
             "cloud_config_cksum": "cloud_config_cksum",
             "cloud_ref": "cloud_ref",
             "cloud_type": "cloud_type",
             "configpb_attributes": "configpb_attributes",
             "connections_rate_limit": "connections_rate_limit",
             "content_rewrite": "content_rewrite",
             "created_by": "created_by",
+            "csrf_policy_ref": "csrf_policy_ref",
             "delay_fairness": "delay_fairness",
             "description": "description",
             "dns_info": "dns_info",
             "dns_policies": "dns_policies",
             "east_west_placement": "east_west_placement",
             "enable_autogw": "enable_autogw",
             "enable_rhi": "enable_rhi",
             "enable_rhi_snat": "enable_rhi_snat",
+            "enable_session": "enable_session",
             "enabled": "enabled",
             "error_page_profile_ref": "error_page_profile_ref",
             "flow_dist": "flow_dist",
             "flow_label_type": "flow_label_type",
             "fqdn": "fqdn",
             "host_name_xlate": "host_name_xlate",
             "http_policies": "http_policies",
@@ -158,15 +165,14 @@
             "static_dns_records": "static_dns_records",
             "tenant_ref": "tenant_ref",
             "test_se_datastore_level_1_ref": "test_se_datastore_level_1_ref",
             "topology_policies": "topology_policies",
             "traffic_clone_profile_ref": "traffic_clone_profile_ref",
             "traffic_enabled": "traffic_enabled",
             "type": "type",
-            "url": "url",
             "use_bridge_ip_as_vip": "use_bridge_ip_as_vip",
             "use_vip_as_snat": "use_vip_as_snat",
             "vh_domain_name": "vh_domain_name",
             "vh_matches": "vh_matches",
             "vh_parent_vs_ref": "vh_parent_vs_ref",
             "vh_type": "vh_type",
             "vip": "vip",
@@ -187,90 +193,62 @@
 
     result["ret"] = resource_in_present_format
 
     return result
 
 
 async def list_(
-    hub,
-    ctx,
-    refers_to: str = None,
-    referred_by: str = None,
-    fields: str = None,
-    include_name: bool = None,
-    skip_default: bool = None,
-    join_subresources: str = None,
-    cloud_uuid: str = None,
-    cloud_ref_name: str = None,
+    hub, ctx, cloud_uuid: str = None, cloud_ref_name: str = None
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
     Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
-        x_avi_tenant(str, optional): Avi Tenant Header. Defaults to None.
-        x_avi_tenant_uuid(str, optional): Avi Tenant Header UUID. Defaults to None.
-        x_avi_version(str): The caller is required to set Avi Version Header to the expected version of configuration. The response from the controller will provide and accept data according to the specified version. The controller will reject POST and PUT requests where the data is not compatible with the specified version.
-        x_csrf_token(str, optional): Avi Controller may send back CSRF token in the response cookies. The caller should update the request headers with this token else controller will reject requests. Defaults to None.
         cloud_uuid(str, optional): Filter to get objects that belongs to a specific cloud using its uuid. Eg. cloud_uuid=cloud-xyz. Defaults to None.
         cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than uuid. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: vmware_alb.virtualservice.list
+                - path: nsx_alb.alb.virtualservice.list
                 - kwargs:
-                  x_avi_version: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.virtualservice.list x_avi_version=value
+            idem exec nsx_alb.alb.virtualservice.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.virtualservice
+            $ idem describe nsx_alb.alb.virtualservice
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    list = await hub.tool.vmware_alb.session.request(
+    list = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
         path="/virtualservice",
-        query_params={
-            "refers_to": refers_to,
-            "referred_by": referred_by,
-            "fields": fields,
-            "include_name": include_name,
-            "skip_default": skip_default,
-            "join_subresources": join_subresources,
-            "cloud_uuid": cloud_uuid,
-            "cloud_ref.name": cloud_ref_name,
-        },
+        query_params={"cloud_uuid": cloud_uuid, "cloud_ref.name": cloud_ref_name},
         data={},
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
@@ -282,15 +260,14 @@
 
     return result
 
 
 async def create(
     hub,
     ctx,
-    type: str,
     active_standby_se_tag: str = None,
     advertise_down_vs: bool = None,
     allow_invalid_client_cert: bool = None,
     analytics_policy: make_dataclass(
         "analytics_policy",
         [
             ("all_headers", bool, field(default=None)),
@@ -751,14 +728,15 @@
                     )
                 ],
                 field(default=None),
             ),
         ],
     ) = None,
     created_by: str = None,
+    csrf_policy_ref: str = None,
     delay_fairness: bool = None,
     description: str = None,
     dns_info: List[
         make_dataclass(
             "dns_info",
             [
                 ("algorithm", str, field(default=None)),
@@ -778,14 +756,15 @@
     dns_policies: List[
         make_dataclass("dns_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     east_west_placement: bool = None,
     enable_autogw: bool = None,
     enable_rhi: bool = None,
     enable_rhi_snat: bool = None,
+    enable_session: bool = None,
     enabled: bool = None,
     error_page_profile_ref: str = None,
     flow_dist: str = None,
     flow_label_type: str = None,
     fqdn: str = None,
     host_name_xlate: str = None,
     http_policies: List[
@@ -1333,15 +1312,15 @@
     tenant_ref: str = None,
     test_se_datastore_level_1_ref: str = None,
     topology_policies: List[
         make_dataclass("topology_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     traffic_clone_profile_ref: str = None,
     traffic_enabled: bool = None,
-    url: str = None,
+    type: str = None,
     use_bridge_ip_as_vip: bool = None,
     use_vip_as_snat: bool = None,
     vh_domain_name: list = None,
     vh_matches: List[
         make_dataclass(
             "vh_matches",
             [
@@ -2197,14 +2176,15 @@
                     * replacement_string (Dict[str, Any], optional): replacement_string
                         * type (str, optional): Type of replacement string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a string with all three combined. Enum options - DATASCRIPT_VAR, AVI_VAR, LITERAL_STRING, COMBINATION_STRING. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * val (str, optional): Value of the replacement string - name of variable exposed from datascript, name of the HTTP header, a custom user-input literal string, or a string with all three combined. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * search_string (Dict[str, Any]): search_string
                         * type (str, optional): Type of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Enum options - SEARCH_DATASCRIPT_VAR, SEARCH_AVI_VAR, SEARCH_LITERAL_STRING, SEARCH_REGEX. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                         * val (str): Value of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         created_by(str, optional): Creator name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
+        csrf_policy_ref(str, optional): CSRF Protection policy for the Virtual Service. It is a reference to an object of type CSRFPolicy. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         delay_fairness(bool, optional): Select the algorithm for QoS fairness.  This determines how multiple Virtual Services sharing the same Service Engines will prioritize traffic over a congested network. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         description(str, optional):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         dns_info(list[Dict[str, Any]], optional): Service discovery specific data including fully qualified domain name, type and Time-To-Live of the DNS record. Note that only one of fqdn and dns_info setting is allowed. Maximum of 1000 items allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * algorithm (str, optional): Specifies the algorithm to pick the IP address(es) to be returned, when multiple entries are configured. This does not apply if num_records_in_response is 0. Default is consistent hash. Enum options - DNS_RECORD_RESPONSE_ROUND_ROBIN, DNS_RECORD_RESPONSE_CONSISTENT_HASH. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * cname (Dict[str, Any], optional): cname
                 * cname (str): Canonical name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * fqdn (str, optional): Fully qualified domain name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -2215,14 +2195,15 @@
         dns_policies(list[Dict[str, Any]], optional): DNS Policies applied on the dns traffic of the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         east_west_placement(bool, optional): Force placement on all SE's in service group (Mesos mode only). Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         enable_autogw(bool, optional): Response traffic to clients will be sent back to the source MAC address of the connection, rather than statically sent to a default gateway. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Special default for Essentials edition is false, Basic edition is false, Enterprise is True. Defaults to None.
         enable_rhi(bool, optional): Enable Route Health Injection using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enable_rhi_snat(bool, optional): Enable Route Health Injection for Source NAT'ted floating IP Address using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
+        enable_session(bool, optional): Enable HTTP sessions for this virtual service. If enabled, a session cookie will be added to HTTP responses and persistent key-value store will be activated. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enabled(bool, optional): Enable or disable the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         error_page_profile_ref(str, optional): Error Page Profile to be used for this virtualservice.This profile is used to send the custom error page to the client generated by the proxy. It is a reference to an object of type ErrorPageProfile. Field introduced in 17.2.4. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         flow_dist(str, optional): Criteria for flow distribution among SEs. Enum options - LOAD_AWARE, CONSISTENT_HASH_SOURCE_IP_ADDRESS, CONSISTENT_HASH_SOURCE_IP_ADDRESS_AND_PORT. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- LOAD_AWARE), Basic edition(Allowed values- LOAD_AWARE), Enterprise with Cloud Services edition. Defaults to None.
         flow_label_type(str, optional): Criteria for flow labelling. Enum options - NO_LABEL, APPLICATION_LABEL, SERVICE_LABEL. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         fqdn(str, optional): DNS resolvable, fully qualified domain name of the virtualservice. Only one of 'fqdn' and 'dns_info' configuration is allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         host_name_xlate(str, optional): Translate the host name sent to the servers to this value.  Translate the host name sent from servers back to the value used by the client. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         http_policies(list[Dict[str, Any]], optional): HTTP Policies applied on the data traffic of the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
@@ -2435,16 +2416,15 @@
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         test_se_datastore_level_1_ref(str, optional): Used for testing SE Datastore Upgrade 2.0 functionality. It is a reference to an object of type TestSeDatastoreLevel1. Field introduced in 18.2.6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         topology_policies(list[Dict[str, Any]], optional): Topology Policies applied on the dns traffic of the Virtual Service based onGSLB Topology algorithm. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         traffic_clone_profile_ref(str, optional): Server network or list of servers for cloning traffic. It is a reference to an object of type TrafficCloneProfile. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         traffic_enabled(bool, optional): Knob to enable the Virtual Service traffic on its assigned service engines. This setting is effective only when the enabled flag is set to True. Field introduced in 17.2.8. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
+        type(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
         use_bridge_ip_as_vip(bool, optional): Use Bridge IP as VIP on each Host in Mesos deployments. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         use_vip_as_snat(bool, optional): Use the Virtual IP as the SNAT IP for health monitoring and sending traffic to the backend servers instead of the Service Engine interface IP. The caveat of enabling this option is that the VirtualService cannot be configued in an Active-Active HA mode. DNS based Multi VIP solution has to be used for HA & Non-disruptive Upgrade purposes. Field introduced in 17.1.9,17.2.3. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_domain_name(list, optional): The exact name requested from the client's SNI-enabled TLS hello domain name field. If this is a match, the parent VS will forward the connection to this child VS. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_matches(list[Dict[str, Any]], optional): Match criteria to select this child VS. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * host (str): Host/domain name match configuration. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * rules (list[Dict[str, Any]], optional): Add rules for selecting the virtual service. At least one rule must be configured. Field introduced in 22.1.3. Minimum of 1 items required. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                 * matches (Dict[str, Any]): matches
@@ -2632,30 +2612,30 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.virtualservice.present:
-                - x_avi_version: value
+              nsx_alb.alb.virtualservice.present:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.virtualservice.create x_avi_version=value
+            idem exec nsx_alb.alb.virtualservice.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "active_standby_se_tag": "active_standby_se_tag",
         "advertise_down_vs": "advertise_down_vs",
         "allow_invalid_client_cert": "allow_invalid_client_cert",
         "analytics_policy": "analytics_policy",
@@ -2671,22 +2651,24 @@
         "cloud_config_cksum": "cloud_config_cksum",
         "cloud_ref": "cloud_ref",
         "cloud_type": "cloud_type",
         "configpb_attributes": "configpb_attributes",
         "connections_rate_limit": "connections_rate_limit",
         "content_rewrite": "content_rewrite",
         "created_by": "created_by",
+        "csrf_policy_ref": "csrf_policy_ref",
         "delay_fairness": "delay_fairness",
         "description": "description",
         "dns_info": "dns_info",
         "dns_policies": "dns_policies",
         "east_west_placement": "east_west_placement",
         "enable_autogw": "enable_autogw",
         "enable_rhi": "enable_rhi",
         "enable_rhi_snat": "enable_rhi_snat",
+        "enable_session": "enable_session",
         "enabled": "enabled",
         "error_page_profile_ref": "error_page_profile_ref",
         "flow_dist": "flow_dist",
         "flow_label_type": "flow_label_type",
         "fqdn": "fqdn",
         "host_name_xlate": "host_name_xlate",
         "http_policies": "http_policies",
@@ -2729,15 +2711,14 @@
         "static_dns_records": "static_dns_records",
         "tenant_ref": "tenant_ref",
         "test_se_datastore_level_1_ref": "test_se_datastore_level_1_ref",
         "topology_policies": "topology_policies",
         "traffic_clone_profile_ref": "traffic_clone_profile_ref",
         "traffic_enabled": "traffic_enabled",
         "type": "type",
-        "url": "url",
         "use_bridge_ip_as_vip": "use_bridge_ip_as_vip",
         "use_vip_as_snat": "use_vip_as_snat",
         "vh_domain_name": "vh_domain_name",
         "vh_matches": "vh_matches",
         "vh_parent_vs_ref": "vh_parent_vs_ref",
         "vh_type": "vh_type",
         "vip": "vip",
@@ -2749,29 +2730,30 @@
         "weight": "weight",
     }
 
     payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
             payload[resource_to_raw_input_mapping[key]] = value
-    create = await hub.tool.vmware_alb.session.request(
+
+    create = await hub.tool.nsx_alb.session.request(
         ctx,
         method="post",
         path="/virtualservice",
         query_params={},
         data=payload,
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created vmware_alb.virtualservice '{name}'",
+        f"Created nsx_alb.alb.virtualservice '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -3244,14 +3226,15 @@
                     )
                 ],
                 field(default=None),
             ),
         ],
     ) = None,
     created_by: str = None,
+    csrf_policy_ref: str = None,
     delay_fairness: bool = None,
     description: str = None,
     dns_info: List[
         make_dataclass(
             "dns_info",
             [
                 ("algorithm", str, field(default=None)),
@@ -3271,14 +3254,15 @@
     dns_policies: List[
         make_dataclass("dns_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     east_west_placement: bool = None,
     enable_autogw: bool = None,
     enable_rhi: bool = None,
     enable_rhi_snat: bool = None,
+    enable_session: bool = None,
     enabled: bool = None,
     error_page_profile_ref: str = None,
     flow_dist: str = None,
     flow_label_type: str = None,
     fqdn: str = None,
     host_name_xlate: str = None,
     http_policies: List[
@@ -3827,15 +3811,14 @@
     test_se_datastore_level_1_ref: str = None,
     topology_policies: List[
         make_dataclass("topology_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     traffic_clone_profile_ref: str = None,
     traffic_enabled: bool = None,
     type: str = None,
-    url: str = None,
     use_bridge_ip_as_vip: bool = None,
     use_vip_as_snat: bool = None,
     vh_domain_name: list = None,
     vh_matches: List[
         make_dataclass(
             "vh_matches",
             [
@@ -4544,15 +4527,14 @@
         )
     ] = None,
     vsvip_cloud_config_cksum: str = None,
     vsvip_ref: str = None,
     waf_policy_ref: str = None,
     weight: int = None,
     name: str = None,
-    **kwargs,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
@@ -4692,14 +4674,15 @@
                     * replacement_string (Dict[str, Any], optional): replacement_string
                         * type (str, optional): Type of replacement string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a string with all three combined. Enum options - DATASCRIPT_VAR, AVI_VAR, LITERAL_STRING, COMBINATION_STRING. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * val (str, optional): Value of the replacement string - name of variable exposed from datascript, name of the HTTP header, a custom user-input literal string, or a string with all three combined. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * search_string (Dict[str, Any]): search_string
                         * type (str, optional): Type of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Enum options - SEARCH_DATASCRIPT_VAR, SEARCH_AVI_VAR, SEARCH_LITERAL_STRING, SEARCH_REGEX. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                         * val (str): Value of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         created_by(str, optional): Creator name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
+        csrf_policy_ref(str, optional): CSRF Protection policy for the Virtual Service. It is a reference to an object of type CSRFPolicy. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         delay_fairness(bool, optional): Select the algorithm for QoS fairness.  This determines how multiple Virtual Services sharing the same Service Engines will prioritize traffic over a congested network. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         description(str, optional):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         dns_info(list[Dict[str, Any]], optional): Service discovery specific data including fully qualified domain name, type and Time-To-Live of the DNS record. Note that only one of fqdn and dns_info setting is allowed. Maximum of 1000 items allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * algorithm (str, optional): Specifies the algorithm to pick the IP address(es) to be returned, when multiple entries are configured. This does not apply if num_records_in_response is 0. Default is consistent hash. Enum options - DNS_RECORD_RESPONSE_ROUND_ROBIN, DNS_RECORD_RESPONSE_CONSISTENT_HASH. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * cname (Dict[str, Any], optional): cname
                 * cname (str): Canonical name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * fqdn (str, optional): Fully qualified domain name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -4710,14 +4693,15 @@
         dns_policies(list[Dict[str, Any]], optional): DNS Policies applied on the dns traffic of the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         east_west_placement(bool, optional): Force placement on all SE's in service group (Mesos mode only). Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         enable_autogw(bool, optional): Response traffic to clients will be sent back to the source MAC address of the connection, rather than statically sent to a default gateway. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Special default for Essentials edition is false, Basic edition is false, Enterprise is True. Defaults to None.
         enable_rhi(bool, optional): Enable Route Health Injection using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enable_rhi_snat(bool, optional): Enable Route Health Injection for Source NAT'ted floating IP Address using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
+        enable_session(bool, optional): Enable HTTP sessions for this virtual service. If enabled, a session cookie will be added to HTTP responses and persistent key-value store will be activated. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enabled(bool, optional): Enable or disable the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         error_page_profile_ref(str, optional): Error Page Profile to be used for this virtualservice.This profile is used to send the custom error page to the client generated by the proxy. It is a reference to an object of type ErrorPageProfile. Field introduced in 17.2.4. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         flow_dist(str, optional): Criteria for flow distribution among SEs. Enum options - LOAD_AWARE, CONSISTENT_HASH_SOURCE_IP_ADDRESS, CONSISTENT_HASH_SOURCE_IP_ADDRESS_AND_PORT. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- LOAD_AWARE), Basic edition(Allowed values- LOAD_AWARE), Enterprise with Cloud Services edition. Defaults to None.
         flow_label_type(str, optional): Criteria for flow labelling. Enum options - NO_LABEL, APPLICATION_LABEL, SERVICE_LABEL. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         fqdn(str, optional): DNS resolvable, fully qualified domain name of the virtualservice. Only one of 'fqdn' and 'dns_info' configuration is allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         host_name_xlate(str, optional): Translate the host name sent to the servers to this value.  Translate the host name sent from servers back to the value used by the client. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         http_policies(list[Dict[str, Any]], optional): HTTP Policies applied on the data traffic of the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
@@ -4930,16 +4914,15 @@
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         test_se_datastore_level_1_ref(str, optional): Used for testing SE Datastore Upgrade 2.0 functionality. It is a reference to an object of type TestSeDatastoreLevel1. Field introduced in 18.2.6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         topology_policies(list[Dict[str, Any]], optional): Topology Policies applied on the dns traffic of the Virtual Service based onGSLB Topology algorithm. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         traffic_clone_profile_ref(str, optional): Server network or list of servers for cloning traffic. It is a reference to an object of type TrafficCloneProfile. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         traffic_enabled(bool, optional): Knob to enable the Virtual Service traffic on its assigned service engines. This setting is effective only when the enabled flag is set to True. Field introduced in 17.2.8. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
+        type(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
         use_bridge_ip_as_vip(bool, optional): Use Bridge IP as VIP on each Host in Mesos deployments. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         use_vip_as_snat(bool, optional): Use the Virtual IP as the SNAT IP for health monitoring and sending traffic to the backend servers instead of the Service Engine interface IP. The caveat of enabling this option is that the VirtualService cannot be configued in an Active-Active HA mode. DNS based Multi VIP solution has to be used for HA & Non-disruptive Upgrade purposes. Field introduced in 17.1.9,17.2.3. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_domain_name(list, optional): The exact name requested from the client's SNI-enabled TLS hello domain name field. If this is a match, the parent VS will forward the connection to this child VS. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_matches(list[Dict[str, Any]], optional): Match criteria to select this child VS. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * host (str): Host/domain name match configuration. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * rules (list[Dict[str, Any]], optional): Add rules for selecting the virtual service. At least one rule must be configured. Field introduced in 22.1.3. Minimum of 1 items required. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                 * matches (Dict[str, Any]): matches
@@ -5127,30 +5110,30 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.virtualservice.present:
-                - x_avi_version: value
+              nsx_alb.alb.virtualservice.present:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.virtualservice.update x_avi_version=value
+            idem exec nsx_alb.alb.virtualservice.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "active_standby_se_tag": "active_standby_se_tag",
         "advertise_down_vs": "advertise_down_vs",
         "allow_invalid_client_cert": "allow_invalid_client_cert",
         "analytics_policy": "analytics_policy",
@@ -5166,22 +5149,24 @@
         "cloud_config_cksum": "cloud_config_cksum",
         "cloud_ref": "cloud_ref",
         "cloud_type": "cloud_type",
         "configpb_attributes": "configpb_attributes",
         "connections_rate_limit": "connections_rate_limit",
         "content_rewrite": "content_rewrite",
         "created_by": "created_by",
+        "csrf_policy_ref": "csrf_policy_ref",
         "delay_fairness": "delay_fairness",
         "description": "description",
         "dns_info": "dns_info",
         "dns_policies": "dns_policies",
         "east_west_placement": "east_west_placement",
         "enable_autogw": "enable_autogw",
         "enable_rhi": "enable_rhi",
         "enable_rhi_snat": "enable_rhi_snat",
+        "enable_session": "enable_session",
         "enabled": "enabled",
         "error_page_profile_ref": "error_page_profile_ref",
         "flow_dist": "flow_dist",
         "flow_label_type": "flow_label_type",
         "fqdn": "fqdn",
         "host_name_xlate": "host_name_xlate",
         "http_policies": "http_policies",
@@ -5224,15 +5209,14 @@
         "static_dns_records": "static_dns_records",
         "tenant_ref": "tenant_ref",
         "test_se_datastore_level_1_ref": "test_se_datastore_level_1_ref",
         "topology_policies": "topology_policies",
         "traffic_clone_profile_ref": "traffic_clone_profile_ref",
         "traffic_enabled": "traffic_enabled",
         "type": "type",
-        "url": "url",
         "use_bridge_ip_as_vip": "use_bridge_ip_as_vip",
         "use_vip_as_snat": "use_vip_as_snat",
         "vh_domain_name": "vh_domain_name",
         "vh_matches": "vh_matches",
         "vh_parent_vs_ref": "vh_parent_vs_ref",
         "vh_type": "vh_type",
         "vip": "vip",
@@ -5250,16 +5234,15 @@
             key in resource_to_raw_input_mapping.keys()
             and value is not None
             and key != "_last_modified"
         ):
             payload[resource_to_raw_input_mapping[key]] = value
 
     if payload:
-        # print("payload",payload)
-        update = await hub.tool.vmware_alb.session.request(
+        update = await hub.tool.nsx_alb.session.request(
             ctx,
             method="put",
             path="/virtualservice/{uuid}".format(**{"uuid": resource_id}),
             query_params={},
             data=payload,
         )
 
@@ -5267,55 +5250,51 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated vmware_alb.virtualservice '{name}'",
+            f"Updated nsx_alb.alb.virtualservice '{name}'",
         )
 
     return result
 
 
-async def delete(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
+async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-
-        resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.virtualservice.absent:
-                - x_avi_version: value
-                - uuid: value
+              nsx_alb.alb.virtualservice.absent:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.virtualservice.delete x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.virtualservice.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    delete = await hub.tool.vmware_alb.session.request(
+    delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
         path="/virtualservice/{uuid}".format(**{"uuid": resource_id}),
         query_params={},
         data={},
     )
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/exec/vmware_alb/vsvip.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/vsvip.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,64 +6,61 @@
 from collections import OrderedDict
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-# __contracts__ = ['auto_state', 'soft_fail']
+__contracts__ = ["soft_fail"]
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: vmware_alb.vsvip.get
+                - path: nsx_alb.alb.vsvip.get
                 - kwargs:
-                  x_avi_version: value
-                  uuid: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.vsvip.get x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.vsvip.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
-    get = await hub.tool.vmware_alb.session.request(
+    get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
-        path="/vsvip/{uuid}".format(**{"uuid": resource_id}),
-        query_params={},
+        path="/vsvip/{uuid}".format(**{"uuid": resource_id})
+        if resource_id
+        else "/vsvip",
+        query_params={"name": name},
         data={},
+        headers={"X-Avi-Tenant": "*"},
     )
 
     if not get["result"]:
         # Send empty result for not found
         if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             result["result"] = False
@@ -74,16 +71,24 @@
         return result
 
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(f"Get '{name}' result is empty")
         return result
 
-    # Convert raw response into present format
-    raw_resource = get["ret"]
+    if "results" in get["ret"].keys():
+        if get["ret"]["count"] != 0:
+            # Convert raw response into present format
+            raw_resource = get["ret"]["results"][0]
+            resource_id = get["ret"]["results"][0]["uuid"]
+        else:
+            return result
+    else:
+        # Convert raw response into present format
+        raw_resource = get["ret"]
 
     resource_in_present_format = {"name": name, "resource_id": resource_id}
     resource_parameters = OrderedDict(
         {
             "bgp_local_preference": "bgp_local_preference",
             "bgp_num_as_path_prepend": "bgp_num_as_path_prepend",
             "bgp_peer_labels": "bgp_peer_labels",
@@ -92,15 +97,14 @@
             "dns_info": "dns_info",
             "east_west_placement": "east_west_placement",
             "ipam_selector": "ipam_selector",
             "markers": "markers",
             "name": "name",
             "tenant_ref": "tenant_ref",
             "tier1_lr": "tier1_lr",
-            "url": "url",
             "use_standard_alb": "use_standard_alb",
             "vip": "vip",
             "vrf_context_ref": "vrf_context_ref",
             "vsvip_cloud_config_cksum": "vsvip_cloud_config_cksum",
         }
     )
 
@@ -112,86 +116,62 @@
 
     result["ret"] = resource_in_present_format
 
     return result
 
 
 async def list_(
-    hub,
-    ctx,
-    refers_to: str = None,
-    referred_by: str = None,
-    fields: str = None,
-    include_name: bool = None,
-    skip_default: bool = None,
-    join_subresources: str = None,
-    cloud_uuid: str = None,
-    cloud_ref_name: str = None,
+    hub, ctx, cloud_uuid: str = None, cloud_ref_name: str = None
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
     Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
         cloud_uuid(str, optional): Filter to get objects that belongs to a specific cloud using its uuid. Eg. cloud_uuid=cloud-xyz. Defaults to None.
         cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than uuid. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: vmware_alb.vsvip.list
+                - path: nsx_alb.alb.vsvip.list
                 - kwargs:
-                  x_avi_version: value
+
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.vsvip.list x_avi_version=value
+            idem exec nsx_alb.alb.vsvip.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.vsvip
+            $ idem describe nsx_alb.alb.vsvip
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    list = await hub.tool.vmware_alb.session.request(
+    list = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
         path="/vsvip",
-        query_params={
-            "refers_to": refers_to,
-            "referred_by": referred_by,
-            "fields": fields,
-            "include_name": include_name,
-            "skip_default": skip_default,
-            "join_subresources": join_subresources,
-            "cloud_uuid": cloud_uuid,
-            "cloud_ref.name": cloud_ref_name,
-        },
+        query_params={"cloud_uuid": cloud_uuid, "cloud_ref.name": cloud_ref_name},
         data={},
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
@@ -249,15 +229,14 @@
         ],
     ) = None,
     markers: List[
         make_dataclass("markers", [("key", str), ("values", list, field(default=None))])
     ] = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_standard_alb: bool = None,
     vip: List[
         make_dataclass(
             "vip",
             [
                 ("vip_id", str),
                 ("auto_allocate_floating_ip", bool, field(default=None)),
@@ -504,17 +483,15 @@
                 * value (str, optional): Value. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * type (str): Selector type. Enum options - SELECTOR_IPAM. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         markers(list[Dict[str, Any]], optional): List of labels to be used for granular RBAC. Field introduced in 20.1.5. Allowed in Enterprise edition with any value, Essentials edition with any value, Basic edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * key (str): Key for filter match. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * values (list, optional): Values for filter match. Multiple values will be evaluated as OR. Example  key = value1 OR key = value2. Behavior for match is key = * if this field is empty. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This sets the placement scope of virtualservice to given tier1 logical router in Nsx-t. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_standard_alb(bool, optional): This overrides the cloud level default and needs to match the SE Group value in which it will be used if the SE Group use_standard_alb value is set. This is only used when FIP is used for VS on Azure Cloud. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
-        uuid(str, optional): UUID of the VsVip object. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         vip(list[Dict[str, Any]], optional): List of Virtual Service IPs and other shareable entities. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
             * auto_allocate_floating_ip (bool, optional): Auto-allocate floating/elastic IP from the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * auto_allocate_ip (bool, optional): Auto-allocate VIP from the provided subnet. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * auto_allocate_ip_type (str, optional): Specifies whether to auto-allocate only a V4 address, only a V6 address, or one of each type. Enum options - V4_ONLY, V6_ONLY, V4_V6. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- V4_ONLY), Basic edition(Allowed values- V4_ONLY), Enterprise with Cloud Services edition.
             * availability_zone (str, optional): Availability-zone to place the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * avi_allocated_fip (bool, optional): (internal-use) FIP allocated by Avi in the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * avi_allocated_vip (bool, optional): (internal-use) VIP allocated by Avi in the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
@@ -596,30 +573,30 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.vsvip.present:
-                - x_avi_version: value
+              nsx_alb.alb.vsvip.present:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.vsvip.create x_avi_version=value
+            idem exec nsx_alb.alb.vsvip.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "bgp_local_preference": "bgp_local_preference",
         "bgp_num_as_path_prepend": "bgp_num_as_path_prepend",
         "bgp_peer_labels": "bgp_peer_labels",
         "cloud_ref": "cloud_ref",
@@ -627,40 +604,40 @@
         "dns_info": "dns_info",
         "east_west_placement": "east_west_placement",
         "ipam_selector": "ipam_selector",
         "markers": "markers",
         "name": "name",
         "tenant_ref": "tenant_ref",
         "tier1_lr": "tier1_lr",
-        "url": "url",
         "use_standard_alb": "use_standard_alb",
         "vip": "vip",
         "vrf_context_ref": "vrf_context_ref",
         "vsvip_cloud_config_cksum": "vsvip_cloud_config_cksum",
     }
 
     payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
             payload[resource_to_raw_input_mapping[key]] = value
 
-    create = await hub.tool.vmware_alb.session.request(
+    create = await hub.tool.nsx_alb.session.request(
         ctx,
         method="post",
         path="/vsvip",
         query_params={},
         data=payload,
     )
+
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created vmware_alb.vsvip '{name}'",
+        f"Created nsx_alb.alb.vsvip '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -711,15 +688,14 @@
         ],
     ) = None,
     markers: List[
         make_dataclass("markers", [("key", str), ("values", list, field(default=None))])
     ] = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_standard_alb: bool = None,
     vip: List[
         make_dataclass(
             "vip",
             [
                 ("vip_id", str),
                 ("auto_allocate_floating_ip", bool, field(default=None)),
@@ -966,15 +942,14 @@
                 * value (str, optional): Value. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * type (str): Selector type. Enum options - SELECTOR_IPAM. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         markers(list[Dict[str, Any]], optional): List of labels to be used for granular RBAC. Field introduced in 20.1.5. Allowed in Enterprise edition with any value, Essentials edition with any value, Basic edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * key (str): Key for filter match. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * values (list, optional): Values for filter match. Multiple values will be evaluated as OR. Example  key = value1 OR key = value2. Behavior for match is key = * if this field is empty. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This sets the placement scope of virtualservice to given tier1 logical router in Nsx-t. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_standard_alb(bool, optional): This overrides the cloud level default and needs to match the SE Group value in which it will be used if the SE Group use_standard_alb value is set. This is only used when FIP is used for VS on Azure Cloud. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         vip(list[Dict[str, Any]], optional): List of Virtual Service IPs and other shareable entities. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
             * auto_allocate_floating_ip (bool, optional): Auto-allocate floating/elastic IP from the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * auto_allocate_ip (bool, optional): Auto-allocate VIP from the provided subnet. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * auto_allocate_ip_type (str, optional): Specifies whether to auto-allocate only a V4 address, only a V6 address, or one of each type. Enum options - V4_ONLY, V6_ONLY, V4_V6. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- V4_ONLY), Basic edition(Allowed values- V4_ONLY), Enterprise with Cloud Services edition.
             * availability_zone (str, optional): Availability-zone to place the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * avi_allocated_fip (bool, optional): (internal-use) FIP allocated by Avi in the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
@@ -1057,30 +1032,30 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.vsvip.present:
-                - x_avi_version: value
+              nsx_alb.alb.vsvip.present:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.vsvip.update x_avi_version=value
+            idem exec nsx_alb.alb.vsvip.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     resource_to_raw_input_mapping = {
         "bgp_local_preference": "bgp_local_preference",
         "bgp_num_as_path_prepend": "bgp_num_as_path_prepend",
         "bgp_peer_labels": "bgp_peer_labels",
         "cloud_ref": "cloud_ref",
@@ -1088,15 +1063,14 @@
         "dns_info": "dns_info",
         "east_west_placement": "east_west_placement",
         "ipam_selector": "ipam_selector",
         "markers": "markers",
         "name": "name",
         "tenant_ref": "tenant_ref",
         "tier1_lr": "tier1_lr",
-        "url": "url",
         "use_standard_alb": "use_standard_alb",
         "vip": "vip",
         "vrf_context_ref": "vrf_context_ref",
         "vsvip_cloud_config_cksum": "vsvip_cloud_config_cksum",
     }
 
     payload = {}
@@ -1105,15 +1079,15 @@
             key in resource_to_raw_input_mapping.keys()
             and value is not None
             and key != "_last_modified"
         ):
             payload[resource_to_raw_input_mapping[key]] = value
 
     if payload:
-        update = await hub.tool.vmware_alb.session.request(
+        update = await hub.tool.nsx_alb.session.request(
             ctx,
             method="put",
             path="/vsvip/{uuid}".format(**{"uuid": resource_id}),
             query_params={},
             data=payload,
         )
 
@@ -1121,55 +1095,51 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated vmware_alb.vsvip '{name}'",
+            f"Updated nsx_alb.alb.vsvip '{name}'",
         )
 
     return result
 
 
-async def delete(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
+async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-
-        resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.vsvip.absent:
-                - x_avi_version: value
-                - uuid: value
+              nsx_alb.alb.vsvip.absent:
+                -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec vmware_alb.vsvip.delete x_avi_version=value, uuid=value
+            idem exec nsx_alb.alb.vsvip.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
-    delete = await hub.tool.vmware_alb.session.request(
+    delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
         path="/vsvip/{uuid}".format(**{"uuid": resource_id}),
         query_params={},
         data={},
     )
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/healthmonitor.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/healthmonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,14 @@
         "udp_monitor",
         [
             ("maintenance_response", str, field(default=None)),
             ("udp_request", str, field(default=None)),
             ("udp_response", str, field(default=None)),
         ],
     ) = None,
-    url: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
@@ -511,85 +510,108 @@
         successful_checks(int, optional): Number of continuous successful health checks before server is marked up. Allowed values are 1-50. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tcp_monitor(Dict[str, Any], optional): tcp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * tcp_half_open (bool, optional): Configure TCP health monitor to use half-open TCP connections to monitor the health of backend servers thereby avoiding consumption of a full fledged server side connection and the overhead and logs associated with it.  This method is light-weight as it makes use of listener in server's kernel layer to measure the health and a child socket or user thread is not created on the server side. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * tcp_request (str, optional): Request data to send after completing the TCP handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * tcp_response (str, optional): Match for the desired keyword in the first 2Kb of the server's TCP response. If this field is left blank, no server response is required. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
+        type(str): Type of the health monitor. Enum options - HEALTH_MONITOR_PING, HEALTH_MONITOR_TCP, HEALTH_MONITOR_HTTP, HEALTH_MONITOR_HTTPS, HEALTH_MONITOR_EXTERNAL, HEALTH_MONITOR_UDP, HEALTH_MONITOR_DNS, HEALTH_MONITOR_GSLB, HEALTH_MONITOR_SIP, HEALTH_MONITOR_RADIUS, HEALTH_MONITOR_SMTP, HEALTH_MONITOR_SMTPS, HEALTH_MONITOR_POP3, HEALTH_MONITOR_POP3S, HEALTH_MONITOR_IMAP, HEALTH_MONITOR_IMAPS, HEALTH_MONITOR_FTP, HEALTH_MONITOR_FTPS, HEALTH_MONITOR_LDAP, HEALTH_MONITOR_LDAPS, HEALTH_MONITOR_SCTP. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP), Basic edition(Allowed values- HEALTH_MONITOR_PING,HEALTH_MONITOR_TCP,HEALTH_MONITOR_UDP,HEALTH_MONITOR_HTTP,HEALTH_MONITOR_HTTPS), Enterprise with Cloud Services edition.
         udp_monitor(Dict[str, Any], optional): udp_monitor. Defaults to None.
             * maintenance_response (str, optional): Match or look for this keyword in the first 2KB of server's response indicating server maintenance.  A successful match results in the server being marked down. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * udp_request (str, optional): Send UDP request. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * udp_response (str, optional): Match for keyword in the UDP response. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-        url(str, optional): url. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.healthmonitor.present:
-                - x_avi_version: value
-                - type_: value
+              nsx_alb.alb.healthmonitor.present:
+                - type: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     desired_state = {
         k: v
         for k, v in locals().items()
         if k not in ("hub", "ctx", "result") and v is not None
     }
+    if desired_state:
+        for k, v in desired_state.items():
+            if k == "tenant_ref" and v is not None:
+                tenant_ref_acct = ctx.acct.get("tenant_ref")
+                desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
+            if k == "cloud_ref" and v is not None:
+                cloud_ref_acct = ctx.acct.get("cloud_ref")
+                desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
+
+    before = await hub.exec.nsx_alb.alb.healthmonitor.get(
+        ctx,
+        name=name,
+    )
+    if before["ret"]:
+        result["old_state"] = before.ret
+        resource_id = before["ret"]["resource_id"]
+    else:
+        resource_id = None
 
     if resource_id:
-        before = await hub.exec.vmware_alb.healthmonitor.get(
+        before = await hub.exec.nsx_alb.alb.healthmonitor.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'vmware_alb.healthmonitor:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
+            desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
+                ctx, data=desired_state
+            )
+        if desired_state:
             for k, v in desired_state.items():
                 if ("_ref" in k and isinstance(v, str)) and ("name=" in v):
                     obj_name = desired_state.get(k).split("name=")[1]
                     obj_type = (
                         (desired_state.get(k).split("?")[0]).strip("/").split("/")[-1]
                     )
-                    url = await hub.tool.vmware_alb.session.get_url(
+                    url = await hub.tool.nsx_alb.session.get_url(
                         ctx, obj_name=obj_name, obj_type=obj_type
                     )
                     desired_state.update({k: url})
         changes = differ.deep_diff(before.ret if before.ret else {}, desired_state)
+
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
-                ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+                ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
-                result["comment"] = (f"Would update vmware_alb.healthmonitor '{name}'",)
+                result["comment"] = (
+                    f"Would update nsx_alb.alb.healthmonitor '{name}'",
+                )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.vmware_alb.healthmonitor.update(
+                update_ret = await hub.exec.nsx_alb.alb.healthmonitor.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "allow_duplicate_monitors": allow_duplicate_monitors,
                         "authentication": authentication,
                         "configpb_attributes": configpb_attributes,
@@ -625,29 +647,29 @@
                         "udp_monitor": udp_monitor,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'vmware_alb.healthmonitor:{name}'"
+                        f"Updated 'nsx_alb.alb.healthmonitor:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
-            ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+            ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create vmware_alb.healthmonitor {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.healthmonitor {name}",)
             return result
         else:
-            create_ret = await hub.exec.vmware_alb.healthmonitor.create(
+            create_ret = await hub.exec.nsx_alb.alb.healthmonitor.create(
                 ctx,
                 name=name,
                 **{
                     "allow_duplicate_monitors": allow_duplicate_monitors,
                     "authentication": authentication,
                     "configpb_attributes": configpb_attributes,
                     "description": description,
@@ -681,28 +703,28 @@
                     "type": type,
                     "udp_monitor": udp_monitor,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'vmware_alb.healthmonitor:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.healthmonitor:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.vmware_alb.healthmonitor.get(
+    after = await hub.exec.nsx_alb.alb.healthmonitor.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -712,66 +734,63 @@
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-
-        resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.healthmonitor.absent:
+              nsx_alb.alb.healthmonitor.absent:
                 -
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'vmware_alb.healthmonitor:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already absent")
         return result
 
-    before = await hub.exec.vmware_alb.healthmonitor.get(
+    before = await hub.exec.nsx_alb.alb.healthmonitor.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete vmware_alb.healthmonitor:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.healthmonitor:{name}"
             return result
 
-        delete_ret = await hub.exec.vmware_alb.healthmonitor.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.healthmonitor.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'vmware_alb.healthmonitor:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.healthmonitor:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'vmware_alb.healthmonitor:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -780,43 +799,36 @@
 
     Describe the resource in a way that can be recreated/managed with the corresponding "present" function
 
 
     None
         None
 
-    Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.healthmonitor
+            $ idem describe nsx_alb.alb.healthmonitor
     """
 
     result = {}
 
-    ret = await hub.exec.vmware_alb.healthmonitor.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.healthmonitor.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe vmware_alb.healthmonitor {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.healthmonitor {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "vmware_alb.healthmonitor.present": [
+            "nsx_alb.alb.healthmonitor.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/pool.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    resource_id: str = None,
     analytics_policy: make_dataclass(
         "analytics_policy", [("enable_realtime_metrics", bool, field(default=None))]
     ) = None,
     analytics_profile_ref: str = None,
     append_port: str = None,
     application_persistence_profile_ref: str = None,
     autoscale_launch_config_ref: str = None,
@@ -386,15 +385,15 @@
                             ],
                         )
                     ],
                     field(default=None),
                 ),
                 ("enabled", bool, field(default=None)),
                 ("external_orchestration_id", str, field(default=None)),
-                ("external_resource_id", str, field(default=None)),
+                ("external_uuid", str, field(default=None)),
                 ("hostname", str, field(default=None)),
                 (
                     "location",
                     make_dataclass(
                         "location",
                         [
                             ("latitude", float, field(default=None)),
@@ -426,18 +425,19 @@
         "sp_gs_info",
         [("fqdns", list, field(default=None)), ("gs_ref", str, field(default=None))],
     ) = None,
     ssl_key_and_certificate_ref: str = None,
     ssl_profile_ref: str = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_service_port: bool = None,
     use_service_ssl_mode: bool = None,
     vrf_ref: str = None,
+    resource_id: str = None,
+    **kwargs,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
@@ -595,15 +595,15 @@
                 * subnet6 (list[Dict[str, Any]], optional): Discovered IPv6 subnet for this IP. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * ip_addr (Dict[str, Any]): ip_addr
                         * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * mask (int):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * enabled (bool, optional): Enable, Disable or Graceful Disable determine if new or existing connections to the server are allowed. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * external_orchestration_id (str, optional): UID of server in external orchestration systems. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
-            * external_resource_id (str, optional): resource_id identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
+            * external_uuid (str, optional): UUID identifying VM in OpenStack and other external compute. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * hostname (str, optional): DNS resolvable name of the server.  May be used in place of the IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * ip (Dict[str, Any]): ip
                 * addr (str): IP address. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * type (str):  Enum options - V4, DNS, V6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * location (Dict[str, Any], optional): location
                 * latitude (float, optional): Latitude of the location. This is represented as degrees.minutes. The range is from -90.0 (south) to +90.0 (north). Allowed values are -90.0-+90.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                 * longitude (float, optional): Longitude of the location. This is represented as degrees.minutes. The range is from -180.0 (west) to +180.0 (east). Allowed values are -180.0-+180.0. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -621,88 +621,109 @@
             * static (bool, optional): If statically learned. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * verify_network (bool, optional): Verify server belongs to a discovered network or reachable via a discovered network. Verify reachable network isn't the OpenStack management network. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * vm_ref (str, optional): (internal-use) This field is used internally by Avi, not editable by the user. It is a reference to an object of type VIMgrVMRuntime. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         service_metadata(str, optional): Metadata pertaining to the service provided by this Pool. In Openshift/Kubernetes environments, app metadata info is stored. Any user input to this field will be overwritten by Avi Vantage. Field introduced in 17.2.14,18.1.5,18.2.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sni_enabled(bool, optional): Enable TLS SNI for server connections. If disabled, Avi will not send the SNI extension as part of the handshake. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         sp_gs_info(Dict[str, Any], optional): sp_gs_info. Defaults to None.
             * fqdns (list, optional): FQDNs associated with the GSLB service. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
-            * gs_ref (str, optional): GSLB service resource_id associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
+            * gs_ref (str, optional): GSLB service uuid associated with the site persistence pool. It is a reference to an object of type GslbService. Field introduced in 22.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         ssl_key_and_certificate_ref(str, optional): Service Engines will present a client SSL certificate to the server. It is a reference to an object of type SSLKeyAndCertificate. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         ssl_profile_ref(str, optional): When enabled, Avi re-encrypts traffic to the backend servers. The specific SSL profile defines which ciphers and SSL versions will be supported. It is a reference to an object of type SSLProfile. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This tier1_lr field should be set same as VirtualService associated for NSX-T. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_service_port(bool, optional): Do not translate the client's destination port when sending the connection to the server. Monitor port needs to be specified for health monitors. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
         use_service_ssl_mode(bool, optional): This applies only when use_service_port is set to true. If enabled, SSL mode of the connection to the server is decided by the SSL mode on the Virtualservice service port, on which the request was received. Field introduced in 21.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         vrf_ref(str, optional): Virtual Routing Context that the pool is bound to. This is used to provide the isolation of the set of networks the pool is attached to. The pool inherits the Virtual Routing Context of the Virtual Service, and this field is used only internally, and is set by pb-transform. It is a reference to an object of type VrfContext. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.pool.present:
+              nsx_alb.alb.pool.present:
                 - name: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
-
     desired_state = {
         k: v
         for k, v in locals().items()
         if k not in ("hub", "ctx", "result") and v is not None
     }
+    if desired_state:
+        for k, v in desired_state.items():
+            if k == "tenant_ref" and v is not None:
+                tenant_ref_acct = ctx.acct.get("tenant_ref")
+                desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
+
+            if k == "cloud_ref" and v is not None:
+                cloud_ref_acct = ctx.acct.get("cloud_ref")
+                desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
+
+    before = await hub.exec.nsx_alb.alb.pool.get(
+        ctx,
+        name=name,
+    )
+    if before["ret"]:
+        result["old_state"] = before.ret
+        resource_id = before["ret"]["resource_id"]
+    else:
+        resource_id = None
 
     if resource_id:
-        before = await hub.exec.vmware_alb.pool.get(
+        before = await hub.exec.nsx_alb.alb.pool.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'vmware_alb.pool:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.pool:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
+            desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
+                ctx, data=desired_state
+            )
+        if desired_state:
             for k, v in desired_state.items():
                 if ("_ref" in k and isinstance(v, str)) and ("name=" in v):
                     obj_name = desired_state.get(k).split("name=")[1]
                     obj_type = (
                         (desired_state.get(k).split("?")[0]).strip("/").split("/")[-1]
                     )
-                    url = await hub.tool.vmware_alb.session.get_url(
+                    url = await hub.tool.nsx_alb.session.get_url(
                         ctx, obj_name=obj_name, obj_type=obj_type
                     )
                     desired_state.update({k: url})
         changes = differ.deep_diff(before.ret if before.ret else {}, desired_state)
 
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
-                ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+                ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
-                result["comment"] = (f"Would update vmware_alb.pool '{name}'",)
+                result["comment"] = (f"Would update nsx_alb.alb.pool '{name}'",)
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.vmware_alb.pool.update(
+                update_ret = await hub.exec.nsx_alb.alb.pool.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "analytics_policy": analytics_policy,
                         "analytics_profile_ref": analytics_profile_ref,
                         "append_port": append_port,
@@ -767,37 +788,34 @@
                         "service_metadata": service_metadata,
                         "sni_enabled": sni_enabled,
                         "sp_gs_info": sp_gs_info,
                         "ssl_key_and_certificate_ref": ssl_key_and_certificate_ref,
                         "ssl_profile_ref": ssl_profile_ref,
                         "tenant_ref": tenant_ref,
                         "tier1_lr": tier1_lr,
-                        "url": url,
                         "use_service_port": use_service_port,
                         "use_service_ssl_mode": use_service_ssl_mode,
                         "vrf_ref": vrf_ref,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
-                    result["comment"].append(f"Updated 'vmware_alb.pool:{name}'")
+                    result["comment"].append(f"Updated 'nsx_alb.alb.pool:{name}'")
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
-            result[
-                "new_state"
-            ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+            result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create vmware_alb.pool {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.pool {name}",)
             return result
         else:
-            create_ret = await hub.exec.vmware_alb.pool.create(
+            create_ret = await hub.exec.nsx_alb.alb.pool.create(
                 ctx,
                 name=name,
                 **{
                     "analytics_policy": analytics_policy,
                     "analytics_profile_ref": analytics_profile_ref,
                     "append_port": append_port,
                     "application_persistence_profile_ref": application_persistence_profile_ref,
@@ -861,109 +879,104 @@
                     "service_metadata": service_metadata,
                     "sni_enabled": sni_enabled,
                     "sp_gs_info": sp_gs_info,
                     "ssl_key_and_certificate_ref": ssl_key_and_certificate_ref,
                     "ssl_profile_ref": ssl_profile_ref,
                     "tenant_ref": tenant_ref,
                     "tier1_lr": tier1_lr,
-                    "url": url,
                     "use_service_port": use_service_port,
                     "use_service_ssl_mode": use_service_ssl_mode,
                     "vrf_ref": vrf_ref,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'vmware_alb.pool:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.pool:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
-
-    after = await hub.exec.vmware_alb.pool.get(
+    after = await hub.exec.nsx_alb.alb.pool.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
 
 async def absent(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str = None,
-    **kwargs,
+    hub, ctx, name: str, resource_id: str = None, **kwargs
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
     Args:
-        resource_id(str): resource_id of the object to fetch.
+
+        resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.pool.absent:
+              nsx_alb.alb.pool.absent:
                 - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'vmware_alb.pool:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.pool:{name}' already absent")
         return result
 
-    before = await hub.exec.vmware_alb.pool.get(
+    before = await hub.exec.nsx_alb.alb.pool.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete vmware_alb.pool:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.pool:{name}"
             return result
 
-        delete_ret = await hub.exec.vmware_alb.pool.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.pool.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'vmware_alb.pool:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.pool:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'vmware_alb.pool:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.pool:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -973,36 +986,42 @@
     Describe the resource in a way that can be recreated/managed with the corresponding "present" function
 
 
     None
         None
 
     Args:
-        None
+        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
+        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
+        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
+        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
+        skip_default(bool, optional): Default values are not set. Defaults to None.
+        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
+
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.pool
+            $ idem describe nsx_alb.alb.pool
     """
 
     result = {}
 
-    ret = await hub.exec.vmware_alb.pool.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.pool.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe vmware_alb.pool {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.pool {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "vmware_alb.pool.present": [
+            "nsx_alb.alb.pool.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/virtualservice.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/virtualservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,15 @@
                     )
                 ],
                 field(default=None),
             ),
         ],
     ) = None,
     created_by: str = None,
+    csrf_policy_ref: str = None,
     delay_fairness: bool = None,
     description: str = None,
     dns_info: List[
         make_dataclass(
             "dns_info",
             [
                 ("algorithm", str, field(default=None)),
@@ -509,14 +510,15 @@
     dns_policies: List[
         make_dataclass("dns_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     east_west_placement: bool = None,
     enable_autogw: bool = None,
     enable_rhi: bool = None,
     enable_rhi_snat: bool = None,
+    enable_session: bool = None,
     enabled: bool = None,
     error_page_profile_ref: str = None,
     flow_dist: str = None,
     flow_label_type: str = None,
     fqdn: str = None,
     host_name_xlate: str = None,
     http_policies: List[
@@ -1065,15 +1067,14 @@
     test_se_datastore_level_1_ref: str = None,
     topology_policies: List[
         make_dataclass("topology_policies", [("dns_policy_ref", str), ("index", int)])
     ] = None,
     traffic_clone_profile_ref: str = None,
     traffic_enabled: bool = None,
     type: str = None,
-    url: str = None,
     use_bridge_ip_as_vip: bool = None,
     use_vip_as_snat: bool = None,
     vh_domain_name: list = None,
     vh_matches: List[
         make_dataclass(
             "vh_matches",
             [
@@ -1929,14 +1930,15 @@
                     * replacement_string (Dict[str, Any], optional): replacement_string
                         * type (str, optional): Type of replacement string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a string with all three combined. Enum options - DATASCRIPT_VAR, AVI_VAR, LITERAL_STRING, COMBINATION_STRING. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                         * val (str, optional): Value of the replacement string - name of variable exposed from datascript, name of the HTTP header, a custom user-input literal string, or a string with all three combined. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
                     * search_string (Dict[str, Any]): search_string
                         * type (str, optional): Type of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Enum options - SEARCH_DATASCRIPT_VAR, SEARCH_AVI_VAR, SEARCH_LITERAL_STRING, SEARCH_REGEX. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                         * val (str): Value of search string - can be a variable exposed from datascript, value of an HTTP variable, a custom user-input literal string, or a regular expression. Field introduced in 21.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         created_by(str, optional): Creator name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
+        csrf_policy_ref(str, optional): CSRF Protection policy for the Virtual Service. It is a reference to an object of type CSRFPolicy. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         delay_fairness(bool, optional): Select the algorithm for QoS fairness.  This determines how multiple Virtual Services sharing the same Service Engines will prioritize traffic over a congested network. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         description(str, optional):  Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         dns_info(list[Dict[str, Any]], optional): Service discovery specific data including fully qualified domain name, type and Time-To-Live of the DNS record. Note that only one of fqdn and dns_info setting is allowed. Maximum of 1000 items allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * algorithm (str, optional): Specifies the algorithm to pick the IP address(es) to be returned, when multiple entries are configured. This does not apply if num_records_in_response is 0. Default is consistent hash. Enum options - DNS_RECORD_RESPONSE_ROUND_ROBIN, DNS_RECORD_RESPONSE_CONSISTENT_HASH. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * cname (Dict[str, Any], optional): cname
                 * cname (str): Canonical name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * fqdn (str, optional): Fully qualified domain name. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
@@ -1947,14 +1949,15 @@
         dns_policies(list[Dict[str, Any]], optional): DNS Policies applied on the dns traffic of the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         east_west_placement(bool, optional): Force placement on all SE's in service group (Mesos mode only). Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         enable_autogw(bool, optional): Response traffic to clients will be sent back to the source MAC address of the connection, rather than statically sent to a default gateway. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Special default for Essentials edition is false, Basic edition is false, Enterprise is True. Defaults to None.
         enable_rhi(bool, optional): Enable Route Health Injection using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enable_rhi_snat(bool, optional): Enable Route Health Injection for Source NAT'ted floating IP Address using the BGP Config in the vrf context. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
+        enable_session(bool, optional): Enable HTTP sessions for this virtual service. If enabled, a session cookie will be added to HTTP responses and persistent key-value store will be activated. Field introduced in 30.2.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         enabled(bool, optional): Enable or disable the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         error_page_profile_ref(str, optional): Error Page Profile to be used for this virtualservice.This profile is used to send the custom error page to the client generated by the proxy. It is a reference to an object of type ErrorPageProfile. Field introduced in 17.2.4. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         flow_dist(str, optional): Criteria for flow distribution among SEs. Enum options - LOAD_AWARE, CONSISTENT_HASH_SOURCE_IP_ADDRESS, CONSISTENT_HASH_SOURCE_IP_ADDRESS_AND_PORT. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- LOAD_AWARE), Basic edition(Allowed values- LOAD_AWARE), Enterprise with Cloud Services edition. Defaults to None.
         flow_label_type(str, optional): Criteria for flow labelling. Enum options - NO_LABEL, APPLICATION_LABEL, SERVICE_LABEL. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         fqdn(str, optional): DNS resolvable, fully qualified domain name of the virtualservice. Only one of 'fqdn' and 'dns_info' configuration is allowed. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         host_name_xlate(str, optional): Translate the host name sent to the servers to this value.  Translate the host name sent from servers back to the value used by the client. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         http_policies(list[Dict[str, Any]], optional): HTTP Policies applied on the data traffic of the Virtual Service. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
@@ -2167,19 +2170,17 @@
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         test_se_datastore_level_1_ref(str, optional): Used for testing SE Datastore Upgrade 2.0 functionality. It is a reference to an object of type TestSeDatastoreLevel1. Field introduced in 18.2.6. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         topology_policies(list[Dict[str, Any]], optional): Topology Policies applied on the dns traffic of the Virtual Service based onGSLB Topology algorithm. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * dns_policy_ref (str): UUID of the dns policy. It is a reference to an object of type DnsPolicy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * index (int): Index of the dns policy. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
         traffic_clone_profile_ref(str, optional): Server network or list of servers for cloning traffic. It is a reference to an object of type TrafficCloneProfile. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         traffic_enabled(bool, optional): Knob to enable the Virtual Service traffic on its assigned service engines. This setting is effective only when the enabled flag is set to True. Field introduced in 17.2.8. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        type_(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
+        type(str, optional): Specify if this is a normal Virtual Service, or if it is the parent or child of an SNI-enabled virtual hosted Virtual Service. Enum options - VS_TYPE_NORMAL, VS_TYPE_VH_PARENT, VS_TYPE_VH_CHILD. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- VS_TYPE_NORMAL), Basic edition(Allowed values- VS_TYPE_NORMAL,VS_TYPE_VH_PARENT), Enterprise with Cloud Services edition. Defaults to None.
         use_bridge_ip_as_vip(bool, optional): Use Bridge IP as VIP on each Host in Mesos deployments. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition. Defaults to None.
         use_vip_as_snat(bool, optional): Use the Virtual IP as the SNAT IP for health monitoring and sending traffic to the backend servers instead of the Service Engine interface IP. The caveat of enabling this option is that the VirtualService cannot be configued in an Active-Active HA mode. DNS based Multi VIP solution has to be used for HA & Non-disruptive Upgrade purposes. Field introduced in 17.1.9,17.2.3. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic, Enterprise with Cloud Services edition. Defaults to None.
-        uuid(str, optional): UUID of the VirtualService. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_domain_name(list, optional): The exact name requested from the client's SNI-enabled TLS hello domain name field. If this is a match, the parent VS will forward the connection to this child VS. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         vh_matches(list[Dict[str, Any]], optional): Match criteria to select this child VS. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * host (str): Host/domain name match configuration. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * rules (list[Dict[str, Any]], optional): Add rules for selecting the virtual service. At least one rule must be configured. Field introduced in 22.1.3. Minimum of 1 items required. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
                 * matches (Dict[str, Any]): matches
                     * bot_detection_result (Dict[str, Any], optional): bot_detection_result
                         * classifications (list[Dict[str, Any]], optional): Bot classification types. Field introduced in 21.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
@@ -2363,71 +2364,96 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.virtualservice.present:
-                - x_avi_version: value
+              nsx_alb.alb.virtualservice.present:
+                - name: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     desired_state = {
         k: v
         for k, v in locals().items()
         if k not in ("hub", "ctx", "result") and v is not None
     }
 
+    if desired_state:
+        for k, v in desired_state.items():
+            if k == "tenant_ref" and v is not None:
+                tenant_ref_acct = ctx.acct.get("tenant_ref")
+                desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
+
+            if k == "cloud_ref" and v is not None:
+                cloud_ref_acct = ctx.acct.get("cloud_ref")
+                desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
+
+    before = await hub.exec.nsx_alb.alb.virtualservice.get(
+        ctx,
+        name=name,
+    )
+    if before["ret"]:
+        result["old_state"] = before.ret
+        resource_id = before["ret"]["resource_id"]
+    else:
+        resource_id = None
+
     if resource_id:
-        before = await hub.exec.vmware_alb.virtualservice.get(
+        before = await hub.exec.nsx_alb.alb.virtualservice.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'vmware_alb.virtualservice:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
+            desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
+                ctx, data=desired_state
+            )
+        if desired_state:
             for k, v in desired_state.items():
                 if ("_ref" in k and isinstance(v, str)) and ("name=" in v):
                     obj_name = desired_state.get(k).split("name=")[1]
                     obj_type = (
                         (desired_state.get(k).split("?")[0]).strip("/").split("/")[-1]
                     )
-                    url = await hub.tool.vmware_alb.session.get_url(
+                    url = await hub.tool.nsx_alb.session.get_url(
                         ctx, obj_name=obj_name, obj_type=obj_type
                     )
                     desired_state.update({k: url})
         changes = differ.deep_diff(before.ret if before.ret else {}, desired_state)
+
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
-                ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+                ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update vmware_alb.virtualservice '{name}'",
+                    f"Would update nsx_alb.alb.virtualservice '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.vmware_alb.virtualservice.update(
+                update_ret = await hub.exec.nsx_alb.alb.virtualservice.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "active_standby_se_tag": active_standby_se_tag,
                         "advertise_down_vs": advertise_down_vs,
                         "allow_invalid_client_cert": allow_invalid_client_cert,
@@ -2444,22 +2470,24 @@
                         "cloud_config_cksum": cloud_config_cksum,
                         "cloud_ref": cloud_ref,
                         "cloud_type": cloud_type,
                         "configpb_attributes": configpb_attributes,
                         "connections_rate_limit": connections_rate_limit,
                         "content_rewrite": content_rewrite,
                         "created_by": created_by,
+                        "csrf_policy_ref": csrf_policy_ref,
                         "delay_fairness": delay_fairness,
                         "description": description,
                         "dns_info": dns_info,
                         "dns_policies": dns_policies,
                         "east_west_placement": east_west_placement,
                         "enable_autogw": enable_autogw,
                         "enable_rhi": enable_rhi,
                         "enable_rhi_snat": enable_rhi_snat,
+                        "enable_session": enable_session,
                         "enabled": enabled,
                         "error_page_profile_ref": error_page_profile_ref,
                         "flow_dist": flow_dist,
                         "flow_label_type": flow_label_type,
                         "fqdn": fqdn,
                         "host_name_xlate": host_name_xlate,
                         "http_policies": http_policies,
@@ -2501,15 +2529,14 @@
                         "static_dns_records": static_dns_records,
                         "tenant_ref": tenant_ref,
                         "test_se_datastore_level_1_ref": test_se_datastore_level_1_ref,
                         "topology_policies": topology_policies,
                         "traffic_clone_profile_ref": traffic_clone_profile_ref,
                         "traffic_enabled": traffic_enabled,
                         "type": type,
-                        "url": url,
                         "use_bridge_ip_as_vip": use_bridge_ip_as_vip,
                         "use_vip_as_snat": use_vip_as_snat,
                         "vh_domain_name": vh_domain_name,
                         "vh_matches": vh_matches,
                         "vh_parent_vs_ref": vh_parent_vs_ref,
                         "vh_type": vh_type,
                         "vip": vip,
@@ -2521,29 +2548,29 @@
                         "weight": weight,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'vmware_alb.virtualservice:{name}'"
+                        f"Updated 'nsx_alb.alb.virtualservice:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
-            ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+            ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create vmware_alb.virtualservice {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.virtualservice {name}",)
             return result
         else:
-            create_ret = await hub.exec.vmware_alb.virtualservice.create(
+            create_ret = await hub.exec.nsx_alb.alb.virtualservice.create(
                 ctx,
                 name=name,
                 **{
                     "active_standby_se_tag": active_standby_se_tag,
                     "advertise_down_vs": advertise_down_vs,
                     "allow_invalid_client_cert": allow_invalid_client_cert,
                     "analytics_policy": analytics_policy,
@@ -2559,22 +2586,24 @@
                     "cloud_config_cksum": cloud_config_cksum,
                     "cloud_ref": cloud_ref,
                     "cloud_type": cloud_type,
                     "configpb_attributes": configpb_attributes,
                     "connections_rate_limit": connections_rate_limit,
                     "content_rewrite": content_rewrite,
                     "created_by": created_by,
+                    "csrf_policy_ref": csrf_policy_ref,
                     "delay_fairness": delay_fairness,
                     "description": description,
                     "dns_info": dns_info,
                     "dns_policies": dns_policies,
                     "east_west_placement": east_west_placement,
                     "enable_autogw": enable_autogw,
                     "enable_rhi": enable_rhi,
                     "enable_rhi_snat": enable_rhi_snat,
+                    "enable_session": enable_session,
                     "enabled": enabled,
                     "error_page_profile_ref": error_page_profile_ref,
                     "flow_dist": flow_dist,
                     "flow_label_type": flow_label_type,
                     "fqdn": fqdn,
                     "host_name_xlate": host_name_xlate,
                     "http_policies": http_policies,
@@ -2616,15 +2645,14 @@
                     "static_dns_records": static_dns_records,
                     "tenant_ref": tenant_ref,
                     "test_se_datastore_level_1_ref": test_se_datastore_level_1_ref,
                     "topology_policies": topology_policies,
                     "traffic_clone_profile_ref": traffic_clone_profile_ref,
                     "traffic_enabled": traffic_enabled,
                     "type": type,
-                    "url": url,
                     "use_bridge_ip_as_vip": use_bridge_ip_as_vip,
                     "use_vip_as_snat": use_vip_as_snat,
                     "vh_domain_name": vh_domain_name,
                     "vh_matches": vh_matches,
                     "vh_parent_vs_ref": vh_parent_vs_ref,
                     "vh_type": vh_type,
                     "vip": vip,
@@ -2635,28 +2663,28 @@
                     "waf_policy_ref": waf_policy_ref,
                     "weight": weight,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'vmware_alb.virtualservice:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.virtualservice:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.vmware_alb.virtualservice.get(
+    after = await hub.exec.nsx_alb.alb.virtualservice.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -2666,69 +2694,63 @@
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
-    Args:
-        x_avi_tenant(str, optional): Avi Tenant Header. Defaults to None.
-        x_avi_tenant_uuid(str, optional): Avi Tenant Header UUID. Defaults to None.
-        x_avi_version(str): The caller is required to set Avi Version Header to the expected version of configuration. The response from the controller will provide and accept data according to the specified version. The controller will reject POST and PUT requests where the data is not compatible with the specified version.
-        x_csrf_token(str, optional): Avi Controller may send back CSRF token in the response cookies. The caller should update the request headers with this token else controller will reject requests. Defaults to None.
-        uuid(str): UUID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.virtualservice.absent:
-                -
+              nsx_alb.alb.virtualservice.absent:
+                - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'vmware_alb.virtualservice:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already absent")
         return result
 
-    before = await hub.exec.vmware_alb.virtualservice.get(
+    before = await hub.exec.nsx_alb.alb.virtualservice.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete vmware_alb.virtualservice:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.virtualservice:{name}"
             return result
 
-        delete_ret = await hub.exec.vmware_alb.virtualservice.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.virtualservice.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'vmware_alb.virtualservice:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.virtualservice:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'vmware_alb.virtualservice:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -2738,48 +2760,38 @@
     Describe the resource in a way that can be recreated/managed with the corresponding "present" function
 
 
     None
         None
 
     Args:
-        refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
-        referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
-        fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
-        include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
-        skip_default(bool, optional): Default values are not set. Defaults to None.
-        join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
-        x_avi_tenant(str, optional): Avi Tenant Header. Defaults to None.
-        x_avi_tenant_uuid(str, optional): Avi Tenant Header UUID. Defaults to None.
-        x_avi_version(str): The caller is required to set Avi Version Header to the expected version of configuration. The response from the controller will provide and accept data according to the specified version. The controller will reject POST and PUT requests where the data is not compatible with the specified version.
-        x_csrf_token(str, optional): Avi Controller may send back CSRF token in the response cookies. The caller should update the request headers with this token else controller will reject requests. Defaults to None.
         cloud_uuid(str, optional): Filter to get objects that belongs to a specific cloud using its uuid. Eg. cloud_uuid=cloud-xyz. Defaults to None.
         cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than uuid. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.virtualservice
+            $ idem describe nsx_alb.alb.virtualservice
     """
 
     result = {}
 
-    ret = await hub.exec.vmware_alb.virtualservice.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.virtualservice.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe vmware_alb.virtualservice {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.virtualservice {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "vmware_alb.virtualservice.present": [
+            "nsx_alb.alb.virtualservice.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/states/vmware_alb/vsvip.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/vsvip.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         ],
     ) = None,
     markers: List[
         make_dataclass("markers", [("key", str), ("values", list, field(default=None))])
     ] = None,
     tenant_ref: str = None,
     tier1_lr: str = None,
-    url: str = None,
     use_standard_alb: bool = None,
     vip: List[
         make_dataclass(
             "vip",
             [
                 ("vip_id", str),
                 ("auto_allocate_floating_ip", bool, field(default=None)),
@@ -281,14 +280,15 @@
                 ("subnet_uuid", str, field(default=None)),
             ],
         )
     ] = None,
     vrf_context_ref: str = None,
     vsvip_cloud_config_cksum: str = None,
     resource_id: str = None,
+    **kwargs,
 ) -> Dict[str, Any]:
     r"""
     **Autogenerated function**
 
     None
         None
 
@@ -315,15 +315,14 @@
                 * value (str, optional): Value. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * type (str): Selector type. Enum options - SELECTOR_IPAM. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         markers(list[Dict[str, Any]], optional): List of labels to be used for granular RBAC. Field introduced in 20.1.5. Allowed in Enterprise edition with any value, Essentials edition with any value, Basic edition with any value, Enterprise with Cloud Services edition. Defaults to None.
             * key (str): Key for filter match. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * values (list, optional): Values for filter match. Multiple values will be evaluated as OR. Example  key = value1 OR key = value2. Behavior for match is key = * if this field is empty. Field introduced in 20.1.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
         tenant_ref(str, optional):  It is a reference to an object of type Tenant. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
         tier1_lr(str, optional): This sets the placement scope of virtualservice to given tier1 logical router in Nsx-t. Field introduced in 20.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
-        url(str, optional): url. Defaults to None.
         use_standard_alb(bool, optional): This overrides the cloud level default and needs to match the SE Group value in which it will be used if the SE Group use_standard_alb value is set. This is only used when FIP is used for VS on Azure Cloud. Field introduced in 18.2.3. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition. Defaults to None.
         vip(list[Dict[str, Any]], optional): List of Virtual Service IPs and other shareable entities. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition. Defaults to None.
             * auto_allocate_floating_ip (bool, optional): Auto-allocate floating/elastic IP from the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
             * auto_allocate_ip (bool, optional): Auto-allocate VIP from the provided subnet. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials, Basic, Enterprise with Cloud Services edition.
             * auto_allocate_ip_type (str, optional): Specifies whether to auto-allocate only a V4 address, only a V6 address, or one of each type. Enum options - V4_ONLY, V6_ONLY, V4_V6. Field introduced in 18.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- V4_ONLY), Basic edition(Allowed values- V4_ONLY), Enterprise with Cloud Services edition.
             * availability_zone (str, optional): Availability-zone to place the Virtual Service. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Enterprise with Cloud Services edition.
             * avi_allocated_fip (bool, optional): (internal-use) FIP allocated by Avi in the Cloud infrastructure. Field introduced in 17.1.1. Allowed in Enterprise edition with any value, Essentials edition(Allowed values- false), Basic edition(Allowed values- false), Enterprise with Cloud Services edition.
@@ -404,69 +403,93 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              vmware_alb.vsvip.present:
+              nsx_alb.alb.vsvip.present:
                 - x_avi_version: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     desired_state = {
         k: v
         for k, v in locals().items()
         if k not in ("hub", "ctx", "result") and v is not None
     }
+    if desired_state:
+        for k, v in desired_state.items():
+            if k == "tenant_ref" and v is not None:
+                tenant_ref_acct = ctx.acct.get("tenant_ref")
+                desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
+
+            if k == "cloud_ref" and v is not None:
+                cloud_ref_acct = ctx.acct.get("cloud_ref")
+                desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
+
+    before = await hub.exec.nsx_alb.alb.vsvip.get(
+        ctx,
+        name=name,
+    )
+    if before["ret"]:
+        result["old_state"] = before.ret
+        resource_id = before["ret"]["resource_id"]
+    else:
+        resource_id = None
 
     if resource_id:
-        before = await hub.exec.vmware_alb.vsvip.get(
+        before = await hub.exec.nsx_alb.alb.vsvip.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'vmware_alb.vsvip:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
+            desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
+                ctx, data=desired_state
+            )
+        if desired_state:
             for k, v in desired_state.items():
                 if ("_ref" in k and isinstance(v, str)) and ("name=" in v):
                     obj_name = desired_state.get(k).split("name=")[1]
                     obj_type = (
                         (desired_state.get(k).split("?")[0]).strip("/").split("/")[-1]
                     )
-                    url = await hub.tool.vmware_alb.session.get_url(
+                    url = await hub.tool.nsx_alb.session.get_url(
                         ctx, obj_name=obj_name, obj_type=obj_type
                     )
                     desired_state.update({k: url})
         changes = differ.deep_diff(before.ret if before.ret else {}, desired_state)
+
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
-                ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+                ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
-                result["comment"] = (f"Would update vmware_alb.vsvip '{name}'",)
+                result["comment"] = (f"Would update nsx_alb.alb.vsvip '{name}'",)
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.vmware_alb.vsvip.update(
+                update_ret = await hub.exec.nsx_alb.alb.vsvip.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "bgp_local_preference": bgp_local_preference,
                         "bgp_num_as_path_prepend": bgp_num_as_path_prepend,
                         "bgp_peer_labels": bgp_peer_labels,
@@ -474,76 +497,72 @@
                         "configpb_attributes": configpb_attributes,
                         "dns_info": dns_info,
                         "east_west_placement": east_west_placement,
                         "ipam_selector": ipam_selector,
                         "markers": markers,
                         "tenant_ref": tenant_ref,
                         "tier1_lr": tier1_lr,
-                        "url": url,
                         "use_standard_alb": use_standard_alb,
                         "vip": vip,
                         "vrf_context_ref": vrf_context_ref,
                         "vsvip_cloud_config_cksum": vsvip_cloud_config_cksum,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
-                    result["comment"].append(f"Updated 'vmware_alb.vsvip:{name}'")
+                    result["comment"].append(f"Updated 'nsx_alb.alb.vsvip:{name}'")
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
-            result[
-                "new_state"
-            ] = hub.tool.vmware_alb.test_state_utils.generate_test_state(
+            result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create vmware_alb.vsvip {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.vsvip {name}",)
             return result
         else:
-            create_ret = await hub.exec.vmware_alb.vsvip.create(
+            create_ret = await hub.exec.nsx_alb.alb.vsvip.create(
                 ctx,
                 name=name,
                 **{
                     "bgp_local_preference": bgp_local_preference,
                     "bgp_num_as_path_prepend": bgp_num_as_path_prepend,
                     "bgp_peer_labels": bgp_peer_labels,
                     "cloud_ref": cloud_ref,
                     "configpb_attributes": configpb_attributes,
                     "dns_info": dns_info,
                     "east_west_placement": east_west_placement,
                     "ipam_selector": ipam_selector,
                     "markers": markers,
                     "tenant_ref": tenant_ref,
                     "tier1_lr": tier1_lr,
-                    "url": url,
                     "use_standard_alb": use_standard_alb,
                     "vip": vip,
                     "vrf_context_ref": vrf_context_ref,
                     "vsvip_cloud_config_cksum": vsvip_cloud_config_cksum,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'vmware_alb.vsvip:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.vsvip:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.vmware_alb.vsvip.get(
+    after = await hub.exec.nsx_alb.alb.vsvip.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -554,64 +573,65 @@
     r"""
     **Autogenerated function**
 
     None
         None
 
     Args:
+
         resource_id(str): resource ID of the object to fetch.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              vmware_alb.vsvip.absent:
-                -
+              nsx_alb.alb.vsvip.absent:
+                - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'vmware_alb.vsvip:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already absent")
         return result
 
-    before = await hub.exec.vmware_alb.vsvip.get(
+    before = await hub.exec.nsx_alb.alb.vsvip.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete vmware_alb.vsvip:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.vsvip:{name}"
             return result
 
-        delete_ret = await hub.exec.vmware_alb.vsvip.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.vsvip.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'vmware_alb.vsvip:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.vsvip:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'vmware_alb.vsvip:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -627,38 +647,36 @@
     Args:
         refers_to(str, optional): Filter to request all objects that refers to another Avi resource. Its syntax is refers_to=<obj_type>:<obj_uuid>. Eg. get all virtual services referring to pool p1 will be refers_to=pool:pool_p1_uuid. Defaults to None.
         referred_by(str, optional): Filter to request all objects that are referred by another Avi resource. Its syntax is referred_by=<obj_type>:<obj_uuid>. Eg. get all pools referred_by virtual service vs1 - referred_by=virtualservice:vs_vs1_uuid. Defaults to None.
         fields(str, optional): List of fields to be returned for the resource. Some fields like name, URL, uuid etc. are always returned. Defaults to None.
         include_name(bool, optional): All the Avi REST reference URIs have a name suffix as URI#name. It is useful to get the referenced resource name without performing get on that object. Defaults to None.
         skip_default(bool, optional): Default values are not set. Defaults to None.
         join_subresources(str, optional): It automatically returns additional dependent resources like runtime. Eg. join_subresources=runtime. Defaults to None.
-        cloud_uuid(str, optional): Filter to get objects that belongs to a specific cloud using its uuid. Eg. cloud_uuid=cloud-xyz. Defaults to None.
-        cloud_ref_name(str, optional): Filter to get objects that belongs to a specific cloud usings its name. This uses cloud name rather than uuid. Eg. cloud_ref.name=Default-Cloud. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe vmware_alb.vsvip
+            $ idem describe nsx_alb.alb.vsvip
     """
 
     result = {}
 
-    ret = await hub.exec.vmware_alb.vsvip.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.vsvip.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe vmware_alb.vsvip {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.vsvip {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "vmware_alb.vsvip.present": [
+            "nsx_alb.alb.vsvip.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/tool/vmware_alb/session.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,32 +12,40 @@
     path: str,
     query_params: Dict[str, str] = {},
     data: Dict[str, Any] = {},
     headers: Dict[str, Any] = {},
 ):
     # Enable trace logging listener for the http client
     trace_config = aiohttp.TraceConfig()
-    trace_config.on_request_start.append(hub.tool.vmware_alb.session.on_request_start)
-    trace_config.on_request_end.append(hub.tool.vmware_alb.session.on_request_end)
+    trace_config.on_request_start.append(hub.tool.nsx_alb.session.on_request_start)
+    trace_config.on_request_end.append(hub.tool.nsx_alb.session.on_request_end)
 
     # path usually starts with "/" in openapi spec
     url = "".join((ctx.acct.endpoint_url.rstrip("/"), path))
-
     async with aiohttp.ClientSession(
         loop=hub.pop.Loop,
         trace_configs=[trace_config],
     ) as session:
         result = dict(ret=None, result=True, status=200, comment=[], headers={})
         if not headers.get("content-type"):
             headers["content-type"] = "application/json"
             headers["accept"] = "application/json"
 
         if "headers" in ctx.acct:
             # The acct login could set authorization and other headers
             headers.update(ctx.acct.headers)
+        data = await hub.tool.nsx_alb.utils.get_appended_prefix(ctx, data=data)
+        if "tenant_ref" in data:
+            if "name" in data["tenant_ref"]:
+                tenant = data["tenant_ref"].split("=")[1]
+            else:
+                tenant = data["tenant_ref"].split("/")[-1]
+            headers.update({"X-Avi-Tenant": tenant})
+        if "X-Avi-Tenant" not in headers:
+            headers.update({"X-Avi-Tenant": "admin"})
 
         query_params_sanitized = {
             k: v for k, v in query_params.items() if v is not None
         }
         async with session.request(
             url=url,
             method=method.lower(),
@@ -48,38 +56,51 @@
             headers=headers,
         ) as response:
             result["status"] = response.status
             result["result"] = 200 <= response.status <= 204
             result["comment"].append(response.reason)
             result["headers"].update(response.headers)
             try:
-                response.raise_for_status()
                 result["ret"] = hub.tool.type.dict.namespaced(await response.json())
+                response.raise_for_status()
             except Exception as err:
+                result["comment"].append(result["ret"])
                 result["comment"].append(f"{err.__class__.__name__}: {err}")
                 result["result"] = False
                 if response.status != 404:
                     try:
                         ret = await response.read()
                         result["ret"] = ret.decode() if hasattr(ret, "decode") else ret
                     except Exception as ex_read_err:
                         result["comment"].append(
                             f"Failed to read response: {ex_read_err.__class__.__name__}: {ex_read_err}"
                         )
 
             return result
 
 
+async def append_prefix(
+    hub,
+    ctx,
+    value: str = None,
+    obj_prefix: str = None,
+) -> Dict[str, Any]:
+    if "_" in obj_prefix:
+        obj_prefix = obj_prefix.replace("_", "")
+    k = "/api/" + obj_prefix + "?name=" + value
+    return k
+
+
 async def get_url(
     hub,
     ctx,
     obj_name: str = None,
     obj_type: str = None,
 ) -> Dict[str, Any]:
-    after = await hub.tool.vmware_alb.session.request(
+    after = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
         path="/{obj_type}".format(**{"obj_type": obj_type}),
         query_params={"name": obj_name},
         data={},
     )
     if after["ret"]["results"]:
```

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb/tool/vmware_alb/test_state_utils.py` & `idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.1.0/idem_vmware_alb.egg-info/PKG-INFO` & `idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vmware-alb
-Version: 0.1.0
+Version: 0.3.0
 Summary: VMware ALB Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-vmware-alb
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-vmware-alb
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-vmware-alb/-/issues
@@ -23,49 +23,49 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Idem_vmware_alb
 ===============
 
-vmware_alb Cloud Provider for Idem
+NSX Advanced Load Balancer provider for Idem
 
 DEVELOPMENT
 ===========
 
 Clone the `idem_vmware_alb` repository and install with pip.
 
 .. code:: bash
 
     git clone git@gitlab.com:my-user/idem_vmware_alb.git
     pip install -e idem_vmware_alb
 
 ACCT
 ====
 
-After installation vmware_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
+After installation nsx_alb Idem Provider execution and state modules will be accessible to the pop `hub`.
 In order to use them we need to set up our credentials.
 
 Create a new file called `credentials.yaml` and populate it with profiles.
 The `default` profile will be used automatically by `idem` unless you specify one with `--acct-profile=profile_name` on the cli.
 
 `acct backends <https://gitlab.com/saltstack/pop/acct-backends>`_ provide alternate methods for storing profiles.
 
-The vmware_alb provider uses the vmware_alb acct plugin for authentication.
-A profile needs to specify the authentication parameters for vmware_alb.
+The nsx_alb provider uses the nsx_alb.alb acct plugin for authentication.
+A profile needs to specify the authentication parameters for nsx_alb.alb.
 
 credentials.yaml
 
 ..  code:: sls
 
-    vmware_alb:
+    nsx_alb.alb:
       default:
         username: my_user
         password: my_good_password
-        endpoint_url: https://console.vmware_alb.com/api
+        endpoint_url: https://console.nsx_alb.com/api
 
 Now encrypt the credentials file and add the encryption key and encrypted file path to the ENVIRONMENT.
 
 The `acct` command should be available as it is a requisite of `idem` and `idem_vmware_alb`.
 Encrypt the the credential file.
 
 .. code:: bash
@@ -88,25 +88,25 @@
 =====
 A profile can be specified for use with a specific state.
 If no profile is specified, the profile called "default", if one exists, will be used:
 
 .. code:: sls
 
     ensure_user_exists:
-      vmware_alb.user.present:
+      nsx_alb.user.present:
         - acct_profile: my-staging-env
         - name: a_user_name
         - kwarg1: val1
 
 It can also be specified from the command line when executing states.
 
 .. code:: bash
 
     idem state --acct-profile my-staging-env my_state.sls
 
 It can also be specified from the command line when calling an exec module directly.
 
 .. code:: bash
 
-    idem exec --acct-profile my-staging-env vmware_alb.user.list
+    idem exec --acct-profile my-staging-env nsx_alb.user.list
```

### Comparing `idem_vmware_alb-0.1.0/setup.py` & `idem_vmware_alb-0.3.0/setup.py`

 * *Files identical despite different names*

