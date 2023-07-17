# Comparing `tmp/onqlave-python-sdk-pilot-0.0.7.tar.gz` & `tmp/onqlave-python-sdk-pilot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-sdk-pilot-0.0.7.tar", last modified: Fri Jul 14 02:16:55 2023, max compression
+gzip compressed data, was "onqlave-python-sdk-pilot-0.0.8.tar", last modified: Mon Jul 17 18:07:13 2023, max compression
```

## Comparing `onqlave-python-sdk-pilot-0.0.7.tar` & `onqlave-python-sdk-pilot-0.0.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.164142 onqlave-python-sdk-pilot-0.0.7/onqlave/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/client.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-14 01:57:58.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-14 01:58:58.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-07-14 01:57:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encryption.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/options.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:13:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/errors/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:16:29.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/aes_gcm_factory.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/id_service.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 01:58:27.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-11 15:21:03.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 01:55:10.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:53.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-07-12 17:40:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/messages/messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.174142 onqlave-python-sdk-pilot-0.0.7/onqlave/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/hasher_test.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/master_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/test/test_pem_decrypt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:10:47.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-14 01:56:52.000000 onqlave-python-sdk-pilot-0.0.7/onqlave/utils/hasher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 02:16:55.000000 onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 02:16:55.184142 onqlave-python-sdk-pilot-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-14 02:16:50.000000 onqlave-python-sdk-pilot-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.463136 onqlave-python-sdk-pilot-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-17 18:07:13.463136 onqlave-python-sdk-pilot-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-02 14:43:10.000000 onqlave-python-sdk-pilot-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 03:10:41.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-14 15:10:12.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/connection/client.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-07-17 13:01:28.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-12 16:35:27.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:06:48.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/responses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 14:35:37.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-14 13:57:46.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 16:39:18.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/credentials/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:40:25.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)    12134 2023-07-17 17:56:06.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-12 16:42:49.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/options.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-07-17 18:02:52.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/errors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 14:04:04.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-17 18:01:31.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/errors/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 02:16:29.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-07-17 15:18:35.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/aes_gcm_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-17 15:19:10.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/id_service.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-07-17 17:52:56.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 14:53:37.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-07-17 18:02:38.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 06:40:20.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-17 15:18:21.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3860 2023-07-14 13:58:23.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-07-17 12:54:28.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-14 13:55:17.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-02 17:34:23.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:23:26.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-13 19:20:14.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/messages/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 14:04:33.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-07-17 18:01:50.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/messages/messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 02:31:41.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 16:09:49.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/test/hasher_test.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-13 19:20:03.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/test/master_test.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-02 17:49:47.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/test/test_pem_decrypt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.453136 onqlave-python-sdk-pilot-0.0.8/onqlave/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 14:04:41.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-07-17 13:05:43.000000 onqlave-python-sdk-pilot-0.0.8/onqlave/utils/hasher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 18:07:13.463136 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-17 18:07:13.000000 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-17 18:07:13.000000 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 18:07:13.000000 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-17 18:07:13.000000 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 18:07:13.000000 onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 18:07:13.463136 onqlave-python-sdk-pilot-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-17 18:06:59.000000 onqlave-python-sdk-pilot-0.0.8/setup.py
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/connection/client.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/connection/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import urllib.request
 import json
 
 from datetime import datetime
 
 from onqlave.contracts.requests.requests import OnqlaveRequest
 from onqlave.logger.logger import OnqlaveLogger
-
+from errors.errors import OnqlaveError, InvalidCountTimeException, InvalidWaitTimeException, InvalidMaxWaitTimeException
 from onqlave.messages import messages
 class RetrySettings:
     """A class for initializing the retry setting, default value is:
     - count = 3
     - wait_time = 400ms
     - max_wait_time = 2000ms
     """
@@ -23,25 +23,37 @@
     ) -> None:
         self._count = self._validate_and_get_count_value(count)
         self._wait_time = self._validate_and_get_count_value(wait_time)
         self._max_wait_time = self._validate_and_get_count_value(max_wait_time)
 
     def _validate_and_get_count_value(self, count: int) -> int:
         if count <= 0:
-            raise Exception # invalid count time
+            raise InvalidCountTimeException(
+                message=messages.INVALID_COUNT_TIME,
+                original_error=None,
+                code=OnqlaveError.InvalidInput
+            )
         return count
     
     def _validate_and_get_wait_time_value(self, wait_time: int) -> int:
         if wait_time <=0:
-            raise Exception # invalid wait time
+            raise InvalidWaitTimeException(
+                message=messages.INVALID_WAIT_TIME,
+                original_error=None,
+                code=OnqlaveError.InvalidInput
+            )
         return wait_time
 
     def _validate_and_get_max_wait_time_value(self, max_wait_time: int) -> int:
         if max_wait_time < 0:
-            raise Exception # invalid max wait time
+            raise InvalidMaxWaitTimeException(
+                message=messages.INVALID_MAX_WAIT_TIME,
+                original_error=None,
+                code=OnqlaveError.InvalidInput
+            )
         return max_wait_time 
 
 class Client:
     """A wrapper for the http client with the retry settings as an additional feature
     """
     def __init__(
             self,
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/connection/connection.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/connection/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,41 +58,45 @@
         self._configuration = configuration
 
     def post(self, resource: str, body: OnqlaveRequest) -> None:
         """Send a request to the Onqlave Platform to fetch the neccessary data for the encryption process
         """
         operation = "Post"
         start = datetime.utcnow()
-        # log the operation
+        
         self._logger.log_debug(messages.CLIENT_OPERATION_STARTED.format(operation))
+        
         url_string = self._configuration._arx_url + "/" + resource
         arx_id = self._configuration._arx_id
 
+        
+        content = body.get_content()
+
         digest = self._hasher.digest(body)
 
         headers_to_sign = {
             OnqlaveAPIKey: self._configuration._credentials._access_key,
             OnqlaveArx: arx_id,
             OnqlaveHost: self._configuration._arx_url,
             OnqlaveAgent: ServerType,
-            OnqlaveContentLength: str(len(body.get_content())),
+            OnqlaveContentLength: str(len(content)),
             OnqlaveDigest: digest,
             OnqlaveVersion: Version
         }
         
         signature = self._hasher.sign(headers_to_sign,self._configuration._credentials._signing_key)
         
         headers = {
             OnqlaveContent: Oonqlave_Content,
             OnqlaveAPIKey: self._configuration._credentials._access_key,
             OnqlaveArx: arx_id,
             OnqlaveHost: self._configuration._arx_url,
             OnqlaveAgent: ServerType,
             OnqlaveRequestTime:str(calendar.timegm(datetime.utcnow().timetuple())),
-            OnqlaveContentLength: str(len(body.get_content())),
+            OnqlaveContentLength: str(len(content)),
             OnqlaveDigest: digest,
             OnqlaveVersion: Version,
             OnqlaveSignature: signature
         }
         response = self._client.post(url_string,request_body=body, headers=headers)
         finish = datetime.utcnow()
         self._logger.log_debug(messages.CLIENT_OPERATION_SUCCESS.format(operation,str(f'{(finish-start).seconds} secs and {(finish-start).microseconds} microsecs')))
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/contracts/responses/responses.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/credentials/credentials.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/encryption.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/encryption.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import logging
 import io
 from datetime import datetime
-
+# from onqlave.logger.logger import OnqlaveLogging
 from onqlave.keymanager.random_service import CSPRNG
 from onqlave.keymanager.id_service import IDService
 from onqlave.keymanager.key_manager_client import KeyManager
 from onqlave.connection.connection import Configuration
 from onqlave.encryption.options import DebugOption,ArxOption
 from onqlave.connection.client import RetrySettings
 from onqlave.credentials.credentials import Credential
@@ -18,15 +17,16 @@
 from onqlave.keymanager.onqlave_types.types import Aesgcm128,Aesgcm256,XChacha20poly1305
 from onqlave.keymanager.onqlave_types.types import AlgorithmSerialiser, AlgorithmDeserialiser
 from onqlave.keymanager.factories.aes_gcm_factory import AEADGCMKeyFactory
 from onqlave.keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
 from onqlave.keymanager.operations.aes_128_gcm_operation import AesGcmKeyOperation
 from onqlave.keymanager.operations.aes_256_gcm_operation import Aes256GcmKeyOperation
 from onqlave.keymanager.operations.xchacha20_poly1305_operation import XChaCha20Poly1305KeyOperation
-
+from errors.errors import OnqlaveError, FetchEncryptionKeyException
+from errors.errors import OperationMappingException, CreatingKeyException, CreatingPrimitiveException, FetchDecryptionKeyException, EncryptionOperationException
 from onqlave.messages import messages
 
 
 class Encryption:
     """A class that models the encryption services with 2 main groups of features:
     - Encrypt/Decrypt data blocks
     - Encrypt/Decrypt data streams
@@ -92,22 +92,42 @@
         Args:
             operation: a string describe the name of the operation
         
         Returns:
             The algorithm & primitive
 
         """
-        # get the edk, dk, algo from Onqlave keymanager
-        edk, dk, algo = self._key_mamanger.fetch_encryption_key()
-        ops = self._operations[algo]
-        
-        factory = ops.get_factory()
-        key = factory.new_key_from_data(ops,dk)
-
-        primitive = factory.primitive(key)
+        edk, dk, algo = self._key_mamanger.fetch_encryption_key()        
+        try:
+            ops = self._operations[algo]
+        except Exception:
+            raise OperationMappingException(
+                message=messages.OPERATION_MAPPING_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
+
+        try:
+            factory = ops.get_factory()
+            key = factory.new_key_from_data(ops,dk)
+        except Exception:
+            raise CreatingKeyException(
+                message=messages.CREATING_KEY_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
+        
+        try:
+            primitive = factory.primitive(key)
+        except Exception:
+            raise CreatingPrimitiveException(
+                message=messages.CREATING_PRIMITIVE_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
 
         algorithm = AlgorithmSerialiser(version=0,algo=algo,key=edk)
 
         return algorithm, primitive
 
     def init_decrypt_operation(self, operation: str, algo: AlgorithmDeserialiser):
         """Init the decrypt operation by fetching the decryption key from the Onqlave Platform,
@@ -116,31 +136,39 @@
         Args:
             operation: a string indicates the name/type of the operation
             algo: a specified object contains the information about the selected algorithm
 
         Returns:
             The encryption primitive object
         """
-        # get the decryption key
-        # add a try catch here
-
+        
         dk = self._key_mamanger.fetch_decryption_key(algo._key)
-
-        # maybe some try-catch here too
-        ops = self._operations[algo.algorithm()] # modify a little bit compared to the Go SDK
-        factory = ops.get_factory()
-
-        # some try-catch here
-        key = factory.new_key_from_data(ops, dk)
-
-        primitive = factory.primitive(key)
-
+        
+        try:
+            ops = self._operations[algo.algorithm()]
+        except Exception as exc:
+            raise OperationMappingException(
+                messages=messages.OPERATION_MAPPING_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
+        
+        try:
+            factory = ops.get_factory()
+            key = factory.new_key_from_data(ops, dk)
+            primitive = factory.primitive(key)
+        except Exception:
+            raise EncryptionOperationException(
+                message=messages.ENCRYPTION_OPERATION_FAILED,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
+        
         return primitive
 
-    # encrypt/decrypt
     def encrypt(self, plaintext: bytearray, associated_data: bytearray) -> bytes:
         """ Encrypt plaintext (as a bytearray) with the combination of associated_data
         regarding to the application of AEAD - Authenticated Encryption with Associated Data
 
         Args:
             plaintext: a bytearray contains the plain data that needs to be encrypted
             associated_data: a bytearray contains the associated data that is going to be
@@ -154,15 +182,15 @@
         start = datetime.utcnow()
         self._logger.log_debug(messages.ENCRYPTING_OPERATION.format(operation))
         header, primitive = self.init_encrypt_operation(operation=operation)
         
         cipher_data = primitive.encrypt(
             plaintext=plaintext,
             associated_data=associated_data 
-        ) # should try-catch error if neccessary
+        )
         
         
         cipher_stream = io.BytesIO()
         processor = PlainStreamProcessor(cipher_stream=cipher_stream)
         processor.write_header(header)
         processor.write_packet(cipher_data)
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/options.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/encryption/plain_stream_processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import io
 import struct
 
 from onqlave.keymanager.onqlave_types.types import AlgorithmSerialiser
+from onqlave.errors.errors import OnqlaveError, PlainStreamWriteHeaderException
+from onqlave.messages import messages
+
 class PlainStreamProcessor:
     """A stream processor for the plain stream in the encryption process
     with two function including writing the header and writing the packet.
     """
     def __init__(self,cipher_stream: io.BytesIO) -> None:
         """Init an PlainStreamProcessor object which takes the cipher stream
         in the encryption process as its main attribute
@@ -27,27 +30,30 @@
 
         Returns:
             Nothing
         """
         header = algorithm.serialise()
         try:
             self._cipher_stream.write(header)
-        except Exception as exc:
-            raise exc # need to handle this specifically
+        except Exception:
+            raise PlainStreamWriteHeaderException(
+                message=messages.PLAIN_STREAM_WRITE_HEADER_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
         
     
     def write_packet(self, packet: bytearray):
         """Write the data into the cipher stream
 
         Args:
             packet: a bytearray contains data
 
         Returns:
             Nothing
         """
         data_len = struct.pack(">I",len(packet))
         try:
             self._cipher_stream.write(data_len)
-             # confirm with Matt to make sure what this means
             self._cipher_stream.write(packet)
         except Exception as exc:
             raise exc
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/aes_gcm_factory.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/aes_gcm_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def new_key(self,operation: KeyOperation):
         format = operation.get_format()
 
     def new_key_from_data(self, operation: KeyOperation, key_data: bytearray) -> Key:
         format = operation.get_format()
         if not self.validate_key_format(format):
-            return None # or raise error
+            return None
         return AesGcmKey(
             key_id=self._id_service.new_key_id(),
             operation=operation,
             data=AesGcmKeyData(
                 value=key_data,
                 key_material_type=KeyMaterialSYMMETRIC,
                 version=0
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/factories/xchacha20_poly1305_factory.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/factories/xchacha20_poly1305_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ctypes import c_uint32
 
 from onqlave.keymanager.onqlave_types.types import Key, KeyOperation, KeyMaterialSYMMETRIC
 from onqlave.keymanager.keys.xchacha_20_poly_1350 import XChaCha20Poly1305KeyData, XChaCha20Poly1305Key
 from onqlave.keymanager.primitives.xchacha20_poly1305_aead import XChaCha20Poly1305AEAD
 from onqlave.keymanager.operations.xchacha20_poly1305_operation import XchaCha20Poly1305KeyVersion
-from ..id_service import IDService
-from ..random_service import CSPRNG
-from ..onqlave_types.types import KeyOperation,Key,KeyFormat,KeyFactory
+from onqlave.keymanager.id_service import IDService
+from onqlave.keymanager.random_service import CSPRNG
+from onqlave.keymanager.onqlave_types.types import KeyOperation,Key,KeyFormat,KeyFactory
 
 ChaCha20Poly1305KeySize = 32
 class XChaCha20Poly1305KeyFactory(KeyFactory):
     def __init__(self, id_service: IDService, random_service: CSPRNG) -> None:
         self._id_service = id_service
         self._random_service = random_service
 
@@ -24,15 +24,14 @@
                 value=key_data,
                 key_material_type=KeyMaterialSYMMETRIC,
                 version=0
             )
         )
     
     def primitive(self, key: XChaCha20Poly1305Key):
-        # validate the key
         self.validate_key(key)
         ret = XChaCha20Poly1305AEAD(
             key=key,
             random_service=self._random_service
         )
         return ret
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/id_service.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/onqlave_types/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import struct
 import io
 
 from ctypes import c_int32, c_uint32
 
+from onqlave.errors.errors import OnqlaveError, AlgorithmSerialisingException, InvalidCipherDataException
+from onqlave.messages import messages
+
 HashTypeName = {
     0: "UNKNOWN_HASH",
     1: "SHA1",
     2: "SHA384",
     3: "SHA256",
     4: "SHA512",
     5: "SHA224",
@@ -201,21 +204,29 @@
 
         Args:
             Nothing
 
         Returns:
             an bytearray contains the data related to an algorithm
         """
-        buffer = io.BytesIO()
-        header_len = struct.pack(">I", 7 + len(self._key))
-        buffer.write(header_len)
-        buffer.write(bytes([self._version]))
-        buffer.write(bytes([int.from_bytes(self._algo,byteorder='big')]))
-        buffer.write(bytes([len(self._key)]))
-        buffer.write(self._key)
+        try:
+            buffer = io.BytesIO()
+            header_len = struct.pack(">I", 7 + len(self._key))
+            buffer.write(header_len)
+            buffer.write(bytes([self._version]))
+            buffer.write(bytes([int.from_bytes(self._algo,byteorder='big')]))
+            buffer.write(bytes([len(self._key)]))
+            buffer.write(self._key)
+        except Exception:
+            raise AlgorithmSerialisingException(
+                message=messages.ALGORITHM_SERIALISING_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
+
         return buffer.getvalue()
 
 
 class AlgorithmDeserialiser():
     """An object used in the decryption process that specifies
     the information of the selected encryption algorithm
     """
@@ -232,29 +243,37 @@
             buffer: a bytearray contains the encoded data of the selected
             algorithm
 
         Returns:
             Nothing
         """
         if len(buffer) < 7:
-            raise Exception # invalid cipher data
+            raise InvalidCipherDataException(
+                message=messages.INVALID_CIPHER_DATA_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
         
         header_len = int.from_bytes(buffer[:4],'big')
         if len(buffer) < header_len:
-            raise Exception # invalid cipher data
+            raise InvalidCipherDataException(
+                message=messages.INVALID_CIPHER_DATA_EXCEPTION,
+                original_error=None,
+                code=OnqlaveError.SdkErrorCode
+            )
         
         self._version = buffer[4]
         self._algo = buffer[5]
         key_len = buffer[6]
 
         self._key = buffer[7:7+key_len]
         
         return header_len
 
-    def key(self) -> bytearray:  # return a bytearray
+    def key(self) -> bytearray: 
         raise NotImplementedError
 
     def version(self) -> bytes:
         raise NotImplementedError
 
     def algorithm(self) -> str:
         return AlgorithmTypeName[self._algo]
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from ctypes import c_uint32
 from onqlave.keymanager.onqlave_types.types import KeyFactory,KeyFormat, KeyOperation
-# from onqlave.keymanager.factories.xchacha20_poly1305_factory import XChaCha20Poly1305KeyFactory
+
 XchaCha20Poly1305KeyVersion = 0
 
 class XChaChaKeyFormat(KeyFormat):
     def __init__(self,key_size: c_uint32, version: c_uint32) -> None:
         self._key_size = key_size
         self._version = version
 
     def size(self) -> c_uint32:
         return self._key_size
 
 class XChaCha20Poly1305KeyOperation(KeyOperation):
     def __init__(self, key_factory: KeyFactory) -> None:
         self._factory = key_factory
-        self._format = XChaChaKeyFormat(32,XchaCha20Poly1305KeyVersion) # need to change this 
+        self._format = XChaChaKeyFormat(32,XchaCha20Poly1305KeyVersion)
 
     def get_format(self):
         return self._format
     
     def get_factory(self):
         return self._factory
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import io
 
 from Crypto.Cipher import AES
 
 from onqlave.keymanager.onqlave_types.types import Key
 from onqlave.keymanager.random_service import CSPRNG
 
 AESGCMIVSize = 12 # aes-gcm init vector size
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/keymanager/random_service.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/test/hasher_test.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/test/hasher_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/test/master_test.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/test/master_test.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave/test/test_pem_decrypt.py` & `onqlave-python-sdk-pilot-0.0.8/onqlave/test/test_pem_decrypt.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/PKG-INFO` & `onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python-sdk-pilot
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SDK to use the encryption service provided by The Onqlave Platform
 Home-page: https://github.com/onqlavelabs/onqlave-python/tree/dev
 Author: Onqlave Pty
 Author-email: dc@onqlave.com
 Keywords: encryption
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/SOURCES.txt` & `onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/onqlave_python_sdk_pilot.egg-info/requires.txt` & `onqlave-python-sdk-pilot-0.0.8/onqlave_python_sdk_pilot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-sdk-pilot-0.0.7/setup.py` & `onqlave-python-sdk-pilot-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='onqlave-python-sdk-pilot',
-    version='0.0.7',
+    version='0.0.8',
     author='Onqlave Pty',
     author_email='dc@onqlave.com',
     description='A SDK to use the encryption service provided by The Onqlave Platform',
     long_description='',
     long_description_content_type='text/markdown',
     url='https://github.com/onqlavelabs/onqlave-python/tree/dev',  # Replace with your package URL
     packages=find_packages(),
```

