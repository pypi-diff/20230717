# Comparing `tmp/inuits_policy_based_auth-5.0.0.tar.gz` & `tmp/inuits_policy_based_auth-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-5.0.0.tar", last modified: Wed Jul 12 13:54:23 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-5.1.0.tar", last modified: Mon Jul 17 14:14:28 2023, max compression
```

## Comparing `inuits_policy_based_auth-5.0.0.tar` & `inuits_policy_based_auth-5.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.826527 inuits_policy_based_auth-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.826527 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 13:54:23.000000 inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.830528 inuits_policy_based_auth-5.0.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/custom_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/flask_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.834528 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:23.838528 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-12 13:54:12.000000 inuits_policy_based_auth-5.0.0/src/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-17 14:14:28.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-17 14:14:28.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:14:28.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 14:14:28.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 14:14:28.000000 inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.168270 inuits_policy_based_auth-5.1.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/integration/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/custom_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/flask_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/unit/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:28.172270 inuits_policy_based_auth-5.1.0/src/tests/unit/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-07-17 14:14:06.000000 inuits_policy_based_auth-5.1.0/src/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-5.0.0/LICENSE` & `inuits_policy_based_auth-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/PKG-INFO` & `inuits_policy_based_auth-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits_policy_based_auth
-Version: 5.0.0
+Version: 5.1.0
 Summary: Module for securing API endpoints based on policies.
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `inuits_policy_based_auth-5.0.0/README.md` & `inuits_policy_based_auth-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/pyproject.toml` & `inuits_policy_based_auth-5.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inuits_policy_based_auth"
-version = "5.0.0"
+version = "5.1.0"
 description = "Module for securing API endpoints based on policies."
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Intended Audience :: Developers",
@@ -18,34 +18,34 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = ["inuits", "policy", "auth"]
 dependencies = [
-    "Authlib>=1.2.0",
+    "Authlib>=1.2.1",
     "cffi>=1.15.1",
-    "click>=8.1.3",
-    "cryptography>=40.0.2",
-    "MarkupSafe>=2.1.2",
+    "click>=8.1.5",
+    "cryptography>=41.0.2",
+    "MarkupSafe>=2.1.3",
     "pycparser>=2.21",
-    "requests>=2.28.2",
-    "Werkzeug>=2.2.3",
+    "requests>=2.31.0",
+    "Werkzeug>=2.3.6",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.7.0",
     "build==0.10.0",
     "coverage==7.2.7",
     "Flask-RESTful==0.3.10",
     "Flask==2.3.2",
     "mypy-extensions==1.0.0",
     "pathspec==0.11.1",
-    "platformdirs==3.8.1",
+    "platformdirs==3.9.1",
     "pyjwt==2.7.0",
     "pytest==7.4.0",
     "python-dotenv==1.0.0",
     "tomli==2.0.1",
     "twine==4.0.2",
 ]
```

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,30 +28,35 @@
         Path to a JSON file containing a mapping of scopes to their corresponding roles.
     static_issuer : str, optional
         A string representing the issuer of the JWT. This parameter is required
         if remote token validation is not enabled.
     static_public_key : str, optional
         A string representing the public key used to verify the signature of the
         JWT. This parameter is required if remote token validation is not enabled.
+    allowed_issuers : List[str], optional
+        A list of token issuers whose tokens are allowed. If this parameter is not
+        passed or the list is empty, all issuers are allowed.
     **kwargs : dict
         Any additional keyword arguments to be passed to the JWTValidator constructor.
     """
 
     def __init__(
         self,
         logger: Logger,
         role_scope_mapping_filepath=None,
         static_issuer=None,
         static_public_key=None,
+        allowed_issuers=None,
         **kwargs,
     ):
         validator = JWTValidator(
             logger,
             static_issuer,
             static_public_key,
+            allowed_issuers,
             **kwargs,
         )
         resource_protector = ResourceProtector()
         resource_protector.register_token_validator(validator)
         self._resource_protector = resource_protector
 
         self._logger = logger
@@ -123,14 +128,17 @@
         An instance of a logger object to be used for logging.
     static_issuer : str, optional
         A string representing the issuer of the JWT. This parameter is required
         if remote token validation is not enabled.
     static_public_key : str, optional
         A string representing the public key used to verify the signature of the
         JWT. This parameter is required if remote token validation is not enabled.
+    allowed_issuers : List[str], optional
+        A list of token issuers whose tokens are allowed. If this parameter is not
+        passed or the list is empty, all issuers are allowed.
     **kwargs : dict
         Additional keyword arguments to be passed to the parent class.
 
     Attributes:
     -----------
     TOKEN_TYPE : str
         A string representing the token type that this validator is responsible for.
@@ -161,20 +169,22 @@
     token_cls = JWTBearerToken
 
     def __init__(
         self,
         logger,
         static_issuer,
         static_public_key,
+        allowed_issuers,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.logger = logger
         self.static_issuer = static_issuer
         self.static_public_key = static_public_key
+        self.allowed_issuers = allowed_issuers
         self.claims_options = {
             "exp": {"essential": True},
             "azp": {"essential": True},
             "sub": {"essential": True},
         }
         self.jwks_cache = {}
 
@@ -214,14 +224,20 @@
         --------
         Optional[JWTBearerToken]
             If authentication is successful, returns a JWTBearerToken object containing
             the decoded JWT claims. If authentication fails, None is returned.
         """
         try:
             issuer = self.__get_issuer_from_token_string(token_string)
+            if not self.allowed_issuers:
+                self.logger.warning(
+                    "No allowed issuers configured, allowing all issuers!"
+                )
+            elif issuer not in self.allowed_issuers:
+                raise Exception(f"Issuer {issuer} not allowed")
             jwks = self.__get_jwks(issuer)
             token = self.__decode_token(token_string, jwks)
             if not token:
                 self.jwks_cache[issuer] = None
                 jwks = self.__get_jwks(issuer)
                 token = self.__decode_token(token_string, jwks)
             return token
```

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/authorization/policies/super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/request_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/contexts/user_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth/policy_factory.py` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth/policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/PKG-INFO` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-policy-based-auth
-Version: 5.0.0
+Version: 5.1.0
 Summary: Module for securing API endpoints based on policies.
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `inuits_policy_based_auth-5.0.0/src/inuits_policy_based_auth.egg-info/SOURCES.txt` & `inuits_policy_based_auth-5.1.0/src/inuits_policy_based_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/authorization/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/custom_token.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/flask_process.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/flask_process.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/app.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/app.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/test_api/policy_loader.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-5.1.0/src/tests/integration/test_policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-5.0.0/src/tests/unit/test_policy_factory.py` & `inuits_policy_based_auth-5.1.0/src/tests/unit/test_policy_factory.py`

 * *Files identical despite different names*

